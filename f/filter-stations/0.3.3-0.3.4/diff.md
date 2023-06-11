# Comparing `tmp/filter_stations-0.3.3.tar.gz` & `tmp/filter_stations-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter_stations-0.3.3.tar", last modified: Thu May  4 10:47:32 2023, max compression
+gzip compressed data, was "filter_stations-0.3.4.tar", last modified: Sun Jun 11 16:28:34 2023, max compression
```

## Comparing `filter_stations-0.3.3.tar` & `filter_stations-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 10:47:32.887698 filter_stations-0.3.3/
--rw-rw-rw-   0        0        0      361 2023-05-04 10:47:32.887202 filter_stations-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-05-04 10:44:45.000000 filter_stations-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 10:47:32.856774 filter_stations-0.3.3/filter_stations/
--rw-rw-rw-   0        0        0    36858 2023-05-04 10:42:33.000000 filter_stations-0.3.3/filter_stations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:47:32.885290 filter_stations-0.3.3/filter_stations.egg-info/
--rw-rw-rw-   0        0        0      361 2023-05-04 10:47:32.000000 filter_stations-0.3.3/filter_stations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-04 10:47:32.000000 filter_stations-0.3.3/filter_stations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 10:47:32.000000 filter_stations-0.3.3/filter_stations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-04 10:47:32.000000 filter_stations-0.3.3/filter_stations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-05-04 10:47:32.000000 filter_stations-0.3.3/filter_stations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-04 10:47:32.000000 filter_stations-0.3.3/filter_stations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 10:47:32.888298 filter_stations-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-05-04 10:43:04.000000 filter_stations-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:28:34.312691 filter_stations-0.3.4/
+-rw-rw-rw-   0        0        0      361 2023-06-11 16:28:34.312265 filter_stations-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-05-04 10:44:45.000000 filter_stations-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 16:28:34.265847 filter_stations-0.3.4/filter_stations/
+-rw-rw-rw-   0        0        0    46699 2023-06-11 16:25:59.000000 filter_stations-0.3.4/filter_stations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:28:34.309377 filter_stations-0.3.4/filter_stations.egg-info/
+-rw-rw-rw-   0        0        0      361 2023-06-11 16:28:33.000000 filter_stations-0.3.4/filter_stations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-11 16:28:33.000000 filter_stations-0.3.4/filter_stations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 16:28:33.000000 filter_stations-0.3.4/filter_stations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-11 16:28:33.000000 filter_stations-0.3.4/filter_stations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-06-11 16:28:33.000000 filter_stations-0.3.4/filter_stations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-11 16:28:33.000000 filter_stations-0.3.4/filter_stations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 16:28:34.313190 filter_stations-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-06-11 15:52:04.000000 filter_stations-0.3.4/setup.py
```

### Comparing `filter_stations-0.3.3/filter_stations/__init__.py` & `filter_stations-0.3.4/filter_stations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 from io import BytesIO
 import base64
 import json
 from folium.plugins import MeasureControl
 import os
 import datetime
 import gc
+from math import ceil
 
 
 # Constants
 API_BASE_URL = 'https://datahub.tahmo.org'
-API_MAX_PERIOD = '365D'
+API_MAX_PERIOD = '1Y'
 
 endpoints = {'VARIABLES': 'services/assets/v2/variables', # 28 different variables
              'STATION_INFO': 'services/assets/v2/stations',
              'WEATHER_DATA': 'services/measurements/v2/stations', # Configured before requesting
              'DATA_COMPLETE': 'custom/sensordx/latestmeasurements',
              'STATION_STATUS': 'custom/stations/status'}
 
@@ -170,20 +171,33 @@
                 If None, all columns are included. Defaults to None.
 
         Returns:
         -----------
         - pandas.DataFrame: DataFrame containing trained models with the specified columns.
         """
         reqUrl = "https://tahmorqctest.eu-de.mybluemix.net/api/models" # endpoint
-        response = self.__request(reqUrl, {})
-        if columns:
-            return pd.DataFrame(response.json())[columns]
+        # response = self.__request(reqUrl, {})
+        print(f'API request: {reqUrl}')
+        apiRequest = requests.get(f'{reqUrl}',
+                                    params={},
+                                    auth=requests.auth.HTTPBasicAuth(
+                                    self.apiKey,
+                                    self.apiSecret
+                                )
+        )
+        if apiRequest.status_code == 200:
+            response =  apiRequest.json()
+            # print(response)
+            if columns:
+                return pd.DataFrame(response)[columns]
+            else:
+                return pd.DataFrame(response)
         else:
-            return pd.DataFrame(response.json())
-
+            return self.__handleApiError(apiRequest)     
+        
     
     def aggregate_variables(self, dataframe):
         """
         Aggregates a pandas DataFrame of weather variables by summing values across each day.
 
         Parameters:
         -----------
@@ -195,41 +209,58 @@
         """
         # Reset index and rename columns
         dataframe = dataframe.reset_index()
         dataframe.rename(columns={'index':'Date'}, inplace=True)
         
         # Group by date and sum values
         return dataframe.groupby(pd.Grouper(key='Date', axis=0, freq='1D')).sum()
+    
+    # aggregate qualityflags
+    def aggregate_qualityflags(self, dataframe):
+        """
+        Aggregate quality flags in a DataFrame by day.
+
+        Parameters:
+        -----------
+        - dataframe (pd.DataFrame): The DataFrame containing the measurements.
+
+        Returns:
+        -----------
+        - pd.DataFrame: A DataFrame with aggregated quality flags, where values greater than 1 are rounded up.
+
+        """
+        dataframe = dataframe.reset_index()
+        dataframe.rename(columns={'index': 'Date'}, inplace=True)
+        
+        # Group by day and calculate the mean. If value that day is greater than 1, get the ceiling.
+        return dataframe.groupby(pd.Grouper(key='Date', axis=0, freq='1D')).mean().applymap(lambda x: ceil(x) if x > 1 else x)
+
+
 
     
     # Get the variables only
-    def get_measurements(self, station, startDate=None, endDate=None, variables=None, dataset='controlled', aggregate=False):
+    def get_measurements(self, station, startDate=None, endDate=None, variables=None, dataset='controlled', aggregate=False, quality_flags=False):
             """
-            Get measurements from a station.
+                Get measurements from a station.
 
-            Parameters:
-            -----------
-            - station: str
-                The station ID.
-            - startDate: str, optional
-                The start date of the measurement period in the format 'YYYY-MM-DD'.
-            - endDate: str, optional
-                The end date of the measurement period in the format 'YYYY-MM-DD'.
-            - variables: list, optional
-                The variables to retrieve measurements for. If None, all variables are retrieved.
-            - dataset: str, optional
-                The dataset to retrieve measurements from. Default is 'controlled'.
-            - aggregate: bool, optional
-                Whether to aggregate the measurements by variable. Default is False.
+                Parameters:
+                -----------
+                - station (str): The station ID.
+                - startDate (str, optional): The start date of the measurement period in the format 'YYYY-MM-DD'.
+                - endDate (str, optional): The end date of the measurement period in the format 'YYYY-MM-DD'.
+                - variables (list, optional): The variables to retrieve measurements for. If None, all variables are retrieved.
+                - dataset (str, optional): The dataset to retrieve measurements from. Default is 'controlled'.
+                - aggregate (bool, optional): Whether to aggregate the measurements by variable. Default is False.
+                - quality_flags (bool, optional): Whether to include quality flag data. Default is False.
+
+                Returns:
+                -----------
+                - A DataFrame containing the measurements.
 
-            Returns:
-            --------
-            - pd.DataFrame
-                A DataFrame containing the measurements.
-            """            
+            """         
             #print('Get measurements', station, startDate, endDate, variables)
             endpoint = 'services/measurements/v2/stations/%s/measurements/%s' % (station, dataset)
 
             dateSplit = self.__splitDateRange(startDate, endDate)
             series = []
             seriesHolder = {}
 
@@ -292,29 +323,41 @@
                     print('Split observations for %s per sensor' % shortcode)
                     sensors = list(set(list(map(lambda x: x[2], seriesHolder[shortcode]))))
                     for sensor in sensors:
                         sensorSerie = list(filter(lambda x: x[2] == sensor, seriesHolder[shortcode]))
                         timestamps = list(map(lambda x: pd.Timestamp(x[0]), sensorSerie))
                         values = list(map(lambda x: x[1], sensorSerie))
                         serie = pd.Series(values, index=pd.DatetimeIndex(timestamps), dtype=np.float64)
+                        if quality_flags:
+                            q_flag = list(map(lambda x: x[3], sensorSerie))
+                            serie = pd.Series(q_flag, index=pd.DatetimeIndex(timestamps), dtype=np.int32)
+                            series.append(serie.to_frame('%s_%s_%s' % (station, sensor, 'Q_FLAG')))
+                            continue
                         if len(variables)==1:
                             series.append(serie.to_frame('%s_%s' % (station, sensor)))
                         else:
                             series.append(serie.to_frame('%s_%s_%s' % (shortcode, station, sensor)))
 
                         # Clean up scope.
                         del sensorSerie
                         del timestamps
                         del values
                         del serie
                 else:
+                    # print(pd.DataFrame(seriesHolder[shortcode]))
                     values = list(map(lambda x: x[1], seriesHolder[shortcode]))
                     serie = pd.Series(values, index=pd.DatetimeIndex(timestamps), dtype=np.float64)
 
                     if len(values) > 0:
+                        if quality_flags:
+                            q_flag = list(map(lambda x: x[3], seriesHolder[shortcode]))
+                            serie = pd.Series(q_flag, index=pd.DatetimeIndex(timestamps), dtype=np.int32)
+                            series.append(serie.to_frame('%s_%s' % (station, 'Q_FLAG')))
+                            continue
+                                # series.append(serie.to_frame('%s_%s_%s' % (station, 'quality_flag')))
                         sensors = list(set(list(map(lambda x: x[2], seriesHolder[shortcode]))))
                         serie = pd.Series(values, index=pd.DatetimeIndex(timestamps), dtype=np.float64)
                         if len(variables) == 1:
                             series.append(serie.to_frame('%s_%s' % (station, sensors[0])))
                         else:
                             series.append(serie.to_frame('%s_%s_%s' % (shortcode, station, sensors[0])))
 
@@ -334,18 +377,28 @@
                 df = pd.concat(series, axis=1, sort=True)
             else:
                 df = pd.DataFrame()
 
             # Clean up memory.
             del series
             gc.collect()
-            if aggregate:
-                return self.aggregate_variables(df)
+            if quality_flags:
+                # cols = [col for col in df.columns if col.split('_')[-1] == 'Q_FLAG']
+                # print(cols)
+                # df = df[cols]
+                # df = df[[f'{station}_Q_Flag']]
+                if aggregate:
+                    return self.aggregate_qualityflags(df)
+                else:
+                    return df
             else:
-                return df
+                if aggregate:
+                    return self.aggregate_variables(df)
+                else:
+                    return df
     
     # retrieve data from multiple at a time
     def multiple_measurements(self, stations_list, csv_file, startDate, endDate, variables, dataset='controlled'):
         """
         Retrieves measurements for multiple stations and saves the aggregated data to a CSV file.
 
         Parameters:
@@ -367,14 +420,15 @@
         """
         error_dict = dict()
         if isinstance(stations_list, list):
             df_stats = []
             
             for station in stations_list:
                 print(stations_list.index(station))
+                print(f'Retrieving data for station: {station}')
                 try:
                     data = self.get_measurements(station, startDate, endDate, variables)
                     agg_data = self.aggregate_variables(data)
                     df_stats.append(agg_data)
                 except Exception as e:
                     error_dict[station] = f'{e}'
             
@@ -385,16 +439,60 @@
                 df = pd.concat(df_stats, axis=1)
                 df.to_csv(f'{csv_file}.csv')
                 return df
 
         
         else:
             raise ValueError('Pass in a list')
+        
+    # multiple quality flags for multiple stations
+    def multiple_qualityflags(self, stations_list, startDate, endDate, csv_file=None):
+        """
+        Retrieves and aggregates quality flag data for multiple stations within a specified date range.
+
+        Parameters:
+        -----------
+        - stations_list (list): A list of station codes for which to retrieve data.
+        - startDate (str): The start date in 'YYYY-MM-DD' format.
+        - endDate (str): The end date in 'YYYY-MM-DD' format.
+        - csv_file (str, optional): The name of the CSV file to save the aggregated data. Default is None.
 
+        Returns:
+        -----------
+        - pandas.DataFrame or None: A DataFrame containing the aggregated quality flag data for the specified stations,
+        or None if an error occurs.
+
+        Raises:
+            Exception: If an error occurs while retrieving data for a station.
+
+        """
+        error_dict = dict()
+
+        if isinstance(stations_list, list):
+            df_stats = []
+            
+            for station in stations_list:
+                print(stations_list.index(station))
+                print(f'Retrieving data for station: {station}')
+                try:
+                    data = self.get_measurements(station, startDate, endDate, variables=['pr'], quality_flags=True)
+                    agg_data = self.aggregate_qualityflags(data)
+                    df_stats.append(agg_data)
+                except Exception as e:
+                    error_dict[station] = f'{e}'
+            
+            with open("Errors.json", "w") as outfile:
+                json.dump(error_dict, outfile, indent=4)
+            
+            if len(df_stats) > 0:
+                df = pd.concat(df_stats, axis=1)
+                df.to_csv(f'{csv_file}.csv')
+                return df.reindex(sorted(df.columns),axis=1) #sorted dataframe
 
+        
 
 # Move the functions to a class
 class Filter(retreive_data):
     # inherit from retrieve_data class
     def __init__(self, apiKey, apiSecret):
         super().__init__(apiKey, apiSecret)
     
@@ -545,15 +643,107 @@
         
         Returns:
         -----------
         - List of station codes that fall within the specified distance from the given address.
         """
         return list(set([i.split('_')[0] for i in self.filter_stations(f'{address}', distance).columns if i.split('_')[-1] != 'clogFlag']))
 
-    
+    # get clogs for a certain duration based on quality objects file
+    def clogs(self, startdate, enddate, flags_json='qualityobjects.json', as_csv=False, csv_file=None):
+        """
+        Generate clog flags DataFrame based on start and end dates.
+
+        Parameters:
+        -----------
+        - startdate (str): Start date in 'YYYY-MM-DD' format.
+        - enddate (str): End date in 'YYYY-MM-DD' format.
+        - flags_json (str, optional): Path to the JSON file containing clog flags data. Defaults to 'qualityobjects.json'.
+        - questionable (bool, optional): Whether to return questionable clog flags. Defaults to False.
+        - as_csv (bool, optional): Whether to save the resulting DataFrame as a CSV file. Defaults to False.
+        - csv_file (str, optional): Name of the CSV file to save. Only applicable if as_csv is True. Defaults to None.
+
+        Returns:
+        -----------
+        - pandas.DataFrame: DataFrame containing the clog flags.
+
+        """
+
+        json_data = pd.read_json(flags_json)
+        startdate = datetime.datetime.strptime(startdate, '%Y-%m-%d')
+        enddate = datetime.datetime.strptime(enddate, '%Y-%m-%d')
+
+        # merge the sensorcode and the stationcode to equate to the station_sensor format 
+        json_data['station_sensor'] = json_data['stationCode'] + '_' + json_data['sensorCode']
+        # convert the start and end time to datetime format datetime[ns]
+        json_data['startDate'] = json_data['startDate'].astype('datetime64[ns]')
+        json_data['endDate'] = pd.to_datetime([dateutil.parser.parse(i).strftime('%Y-%m-%d') for i in json_data['endDate']])
+
+        json_data = json_data.drop(['stationCode', 'sensorCode'], axis=1)
+        json_data = json_data[['description', 'startDate', 'endDate', 'station_sensor']]
+
+        other_failure = list(json_data[json_data['description'].str.contains('batter')].index)
+        clog = list(json_data[~json_data['description'].str.contains('batter')].index)
+
+        clog_flags = pd.DataFrame(pd.date_range(startdate, enddate, freq='D'), columns=['Date'])
+
+        clogs_dict = dict()
+        for i in json_data.station_sensor.unique():
+            clogs_dict[f'{i}_clogFlags'] = [np.nan for i in range(len(clog_flags))]
+
+        flags_df = pd.concat([clog_flags, pd.DataFrame(clogs_dict)], axis=1)
+
+        def subset_flags_df(startdate, enddate, column, val):
+            """
+            Update a subset of flags in the DataFrame with a specific value.
+
+            Args:
+                startdate (datetime): Start date of the subset.
+                enddate (datetime): End date of the subset.
+                column (str): Name of the column to update.
+                val: Value to fill in the specified column.
+
+            Returns:
+                None
+
+            """
+            # print(f'Updating {column} from {startdate} to {enddate} to {val}')
+            flags_df.loc[((flags_df['Date'] >= startdate) & (flags_df['Date'] <= enddate)), column] = val
+
+        for ind, row in json_data.iterrows():
+            if ind in other_failure:
+                if row['startDate'] >= startdate and row['endDate'] <= enddate:
+                    subset_flags_df(row['startDate'], row['endDate'], f"{row['station_sensor']}_clogFlags", 2)
+                elif row['startDate'] >= startdate and row['endDate'] > enddate:
+                    subset_flags_df(row['startDate'], enddate, f"{row['station_sensor']}_clogFlags", 2)
+                elif row['startDate'] < startdate and row['endDate'] <= enddate:
+                    subset_flags_df(startdate, row['endDate'], f"{row['station_sensor']}_clogFlags", 2)
+                elif row['startDate'] < startdate and row['endDate'] > enddate:
+                    subset_flags_df(startdate, enddate, f"{row['station_sensor']}_clogFlags", 2)
+            elif ind in clog:
+                if row['startDate'] >= startdate and row['endDate'] <= enddate:
+                    subset_flags_df(row['startDate'], row['endDate'], f"{row['station_sensor']}_clogFlags", 1)
+                elif row['startDate'] >= startdate and row['endDate'] > enddate:
+                    subset_flags_df(row['startDate'], enddate, f"{row['station_sensor']}_clogFlags", 1)
+                elif row['startDate'] < startdate and row['endDate'] <= enddate:
+                    subset_flags_df(startdate, row['endDate'], f"{row['station_sensor']}_clogFlags", 1)
+                elif row['startDate'] < startdate and row['endDate'] > enddate:
+                    subset_flags_df(startdate, enddate, f"{row['station_sensor']}_clogFlags", 1)
+
+        flags_df = flags_df.set_index('Date')
+        flags_df = flags_df.reindex(sorted(flags_df.columns), axis=1)
+
+        if as_csv:
+            if csv_file is not None:
+                flags_df.to_csv(f'{csv_file}.csv', index=True)
+                return flags_df
+            else:
+                flags_df.to_csv('clog_flags.csv', index=True)
+                return flags_df
+        else:
+            return flags_df
 
 # A different class for visualisations
 class Interactive_maps(retreive_data):
     # inherit from retrieve_data class
     def __init__(self, apiKey, apiSecret):
         super().__init__(apiKey, apiSecret)
```

### Comparing `filter_stations-0.3.3/setup.py` & `filter_stations-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='filter_stations',
-    version='0.3.3',
+    version='0.3.4',
     packages=find_packages(),
     include_package_data=True,
     description='Making it easier to navigate and clean station data',
     author='Austin Kaburia',
     author_email='kaburiaaustin1@gmail.com',
     url='https://github.com/kaburia/Packaging/tree/main/filter_stations',
     install_requires=[
```

