# Comparing `tmp/pwdusage-0.9.4.tar.gz` & `tmp/pwdusage-1.0.0.tar.gz`

## Comparing `pwdusage-0.9.4.tar` & `pwdusage-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pwdusage-0.9.4/src/pwdusage/__init__.py
--rw-r--r--   0        0        0     6365 2020-02-02 00:00:00.000000 pwdusage-0.9.4/src/pwdusage/base_agent.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 pwdusage-0.9.4/src/pwdusage/common.py
--rw-r--r--   0        0        0    49930 2020-02-02 00:00:00.000000 pwdusage-0.9.4/src/pwdusage/engine.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 pwdusage-0.9.4/src/pwdusage/example_usage.json
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 pwdusage-0.9.4/src/pwdusage/server.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 pwdusage-0.9.4/src/pwdusage/simple_agent.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 pwdusage-0.9.4/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pwdusage-0.9.4/LICENSE
--rw-r--r--   0        0        0    37309 2020-02-02 00:00:00.000000 pwdusage-0.9.4/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 pwdusage-0.9.4/pyproject.toml
--rw-r--r--   0        0        0    37134 2020-02-02 00:00:00.000000 pwdusage-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pwdusage-1.0.0/src/pwdusage/__init__.py
+-rw-r--r--   0        0        0     6365 2020-02-02 00:00:00.000000 pwdusage-1.0.0/src/pwdusage/base_agent.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 pwdusage-1.0.0/src/pwdusage/common.py
+-rw-r--r--   0        0        0    49930 2020-02-02 00:00:00.000000 pwdusage-1.0.0/src/pwdusage/engine.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 pwdusage-1.0.0/src/pwdusage/example_usage.json
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 pwdusage-1.0.0/src/pwdusage/server.py
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 pwdusage-1.0.0/src/pwdusage/simple_agent.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 pwdusage-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pwdusage-1.0.0/LICENSE
+-rw-r--r--   0        0        0    49234 2020-02-02 00:00:00.000000 pwdusage-1.0.0/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 pwdusage-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    48835 2020-02-02 00:00:00.000000 pwdusage-1.0.0/PKG-INFO
```

### Comparing `pwdusage-0.9.4/src/pwdusage/base_agent.py` & `pwdusage-1.0.0/src/pwdusage/base_agent.py`

 * *Files identical despite different names*

### Comparing `pwdusage-0.9.4/src/pwdusage/common.py` & `pwdusage-1.0.0/src/pwdusage/common.py`

 * *Files identical despite different names*

### Comparing `pwdusage-0.9.4/src/pwdusage/engine.py` & `pwdusage-1.0.0/src/pwdusage/engine.py`

 * *Files identical despite different names*

### Comparing `pwdusage-0.9.4/src/pwdusage/example_usage.json` & `pwdusage-1.0.0/src/pwdusage/example_usage.json`

 * *Files identical despite different names*

### Comparing `pwdusage-0.9.4/src/pwdusage/server.py` & `pwdusage-1.0.0/src/pwdusage/server.py`

 * *Files identical despite different names*

### Comparing `pwdusage-0.9.4/src/pwdusage/simple_agent.py` & `pwdusage-1.0.0/src/pwdusage/simple_agent.py`

 * *Files identical despite different names*

### Comparing `pwdusage-0.9.4/.gitignore` & `pwdusage-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pwdusage-0.9.4/LICENSE` & `pwdusage-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwdusage-0.9.4/README.md` & `pwdusage-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 <!---
 # cspell: ignore venv beautifulsoup tzdata numpy simplejson datasource pypi pwdusage
 ---> 
 
+# pwdusage
+
+A usage (mainly time of use) proxy microservice for Powerwall-Dashboard.
+
+![Usage detail 7d](https://github.com/BuongiornoTexas/pwdusage/assets/48264358/f2a014e6-4f17-437e-8ab0-409f5126ea7f)
+
 # Change Log
 
 I'm tracking progress towards v1.0 at: 
 https://github.com/BuongiornoTexas/pwdusage/issues/1.
 
 From v0.9.4, the python/microservice is feature complete. Releases up to v1.0 will 
 address bug fixes and documentation (and incorporate any new agent contributions). 
@@ -13,32 +19,38 @@
 ## Breaking
 
 This section notes any breaking changes, from newest to oldest.
 
 - **v0.9.4**. 
   - Project renamed to pwdusage to give a shorter name for pypi package.
   - Separated python component from dashboard components. In the interim, the latter can
-  be found at:  https://github.com/BuongiornoTexas/Powerwall-Dashboard/tree/main/tools/usage-service, and should be integrated into the main tree after beta phase.
+  be found at:
+  https://github.com/BuongiornoTexas/Powerwall-Dashboard/tree/main/tools/usage-service,
+  and should be integrated into the main tree after beta phase.
   - First release of python package from pypi, new install procedure.
 - **v0.9.1**. "supplyPriority" in `usage.json` renamed to "supply_priority" to improve
 naming consistency.
 
 ## New Features
 
+**v1.0.0** 
+- Documentation for building and testing docker image, instructions for adding
+the docker container to the Powerwall-Dashboard stack. 
+- Documentation for grafana configuration.
+- Sample dashboards added to the Powerwall-Dashboard repo.
+
 **v0.9.1**
 - Resampling to more useful periods for bar charts.
 - Payload features implemented. You can now turn resampling on/off, request summary 
 reports, and select year to date or month to date reporting (which ignore the grafana
 range).
 - Month anchor for annual reporting, weekday anchor for monthly reporting by week.
 - CLI interface to dump out csv format files for debugging.
 
-# pwdusage
-
-Usage (mainly time of use) proxy microservice for Powerwall-Dashboard
+# Key Features
 
 The following dot points outline key elements of the usage engine:
 
 - The usage engine provides a framework for time of use energy and cost reporting.
 - The framework assumes that a utility's supply agreement/contract can be broken into: a 
 usage plan that describes the mostly-constant elements of the contract, and a calendar
 that specifies which usage plan should be active at any time and the variable parameters
@@ -72,44 +84,148 @@
 the pypowerwall server or influx instance (not applicable while developing new usage
 agents).
 4) It's easy to test the effects of different tariff types on historical data (albeit,
 the historical data may not reflect optimisation for the tariff).
 
 # Setup
 
-TODO: Set up docker container for microservice. Until this is done time, users will
-either need to prepare a custom docker image, or follow the 
-["Installation for development/testing"](#installation-for-developmenttesting) 
-instructions below to setup a stand alone server instance for running the
-usage engine.
-
-# Configuration
-
-Because there are so many different tariffs, configuration will require setting up a
-`usage.json` file to define usage plans and calendars, and you will very likely also
-need to do some customisation in grafana to get report out in the format you prefer.
-
-This repository contains a file named `example_usage.json` that you can use to build
-your own `usage.json`. If you are running a stand alone server, use a `USAGE_JSON` 
-environment variable to specify the path to your configuration file (the environment
-variable must specify the path and the file name, and you may use a different file name
-if you prefer). If you do not specify the environment variable it will default to it
-will default to searching for `usage.json` in the python working directory. 
-
-If you are running the usage engine from a docker instance, you **must** specify the 
-`USAGE_JSON` environment variable, as there is no default configuration file. TODO more 
-detail on USAGE_JSON environment variable for docker build. 
+This section details setup for end users. Developers and users who wish to use the CLI
+components should refer to 
+["Installation for development/testing"](#installation-for-developmenttesting), which
+details setting up a local server instance running under python.
 
-While most of the heavy lifting is done in the `usage.json` file, this configuration 
-file depends heavily on constants defined in `common.py`. The next sections
-details these constants, the structure of `usage.json`, and finally outlines grafana
-customisation steps.
+All of the script and configuration files referred to in this document can be found in
+the `tool/usage-service` subfolder of the 
+[`Powerwall-Dashboard` repo](https://github.com/jasonacox/Powerwall-Dashboard). (As 
+they belong with the Dashboard rather the python service.)
+
+(If you can't find files that this document refers to, it is possible that this
+version of `pwdusage` contains files that have not yet been committed to the main
+repository - check https://github.com/BuongiornoTexas/Powerwall-Dashboard for work in
+progress).
+
+## Open firewall port
+
+Decide which port the usage micro-service will use and make the changes required to
+allow your grafana host to access this port (and any other machine that might need 
+access). For example, I'm using ufw on my local network:
+```
+ufw allow from 192.168.xxx.0/24 to any port 9050 proto tcp
+```
+
+## Build Docker Image
+
+I have provided utility scripts to build the docker image for your local machine. 
+Depending on demand, this may become a distributed image in the future. 
+
+Open a terminal and navigate to the `tools/usage-service` sub-folder of 
+`Powerwall-Dashboard`. In this folder generate the image using:
+```
+bash build.sh
+```
+Note for developers: This script will delete any existing `pwdusage` images and 
+containers (if you are a normal end user, this is most likely what you want to happen).
+
+## Test Docker Image
+
+This is an optional step which may be useful for trouble shooting. The test process
+is as follows:
+
+- Navigate to the `tools/usage-service` sub-folder of `Powerwall-Dashboard`.
+- Copy the `example_usage.json` file to `usage.json` in the `usage-service` folder.
+- Edit `usage.json` so that file  so that `influx_url` points at your influx server
+(probably the same machine as your Powerwall-Dashboard) and, optionally, set the correct
+ `timezone` for your region.
+- Run a test script which performs the following actions:
+  - Stops and deletes the `pwdusage` container.
+  - Creates and start a new `pwdusage` container configured by the test `usage.json`.
+  - Pauses while you check the server status.
+  
+  The test script command is:
+  ```
+  bash test_service.sh
+  ```
+
+- Check that the usage server is responding by pointing a web browser at
+`http://server.address:<port>/usage_engine`. If everything is as it should be, you
+ should see a page containing the message:
+
+  ```
+  Usage Engine Status	"Engine OK, tariffs (re)loaded"
+  ```
+- Return to the terminal running the test script and hit enter. This will clean up the
+test by stopping and deleting the container (but keeps the image you created in the
+previous section). 
+
+The next sections details adding the usage service to your 
+`Powerwall-Dashboard` stack.
+
+## Add `pwdusage` to `Powerwall-Dashboard`
+
+This step assumes you have set up a `usage.json` configuration file in the 
+`tools/usage-service` subfolder of Powerwall-Dashboard. See the previous section for
+using the example file, and the following section for details on setting it up to
+match your own usage plan.
+
+The `pwdusage` install steps are:
+
+- If `powerwall.extend.yml` exists in your `Powerwall-Dashboard` folder, then copy the 
+contents of the `pwdusage.extend.yml` file starting from the line `pwdusage:` into 
+`powerwall.extend.yml` (this should be in the services section).
+- Otherwise, copy `pwdusage.extend.yml` into the `Powerwall-Dashboard` folder and rename
+it to `powerwall.extend.yml`.
+- Edit `powerwall.extend.yml` to reflect your user id and any changes you may have made
+to the default port and `USAGE_JSON` file path.
+
+Finally, restart the Powerwall-Dashboard services:
+```
+./compose-dash.sh stop
+./compose-dash.sh up -d
+```
+
+# `pwdusage` Configuration
+
+Because there are so many different usage plans, `pwdusage` requires a JSON
+configuration file to define *your* usage plans and calendars. This section discusses
+the layout of this file and the how usage engine locates this file. You will very likely
+also need to do some customisation in grafana to get report out in the format you
+prefer, which the next section covers.
+
+The project documentation assumes this file will be named  `usage.json` file. However,
+you can use any name you like in conjunction with the `USAGE_JSON` environment variable
+(see below).
+
+The `tools/usage-service` folder in Powerwall-Dashboard repository contains a file named `example_usage.json` that you can use to build your own `usage.json`. The recommended
+default location for your `usage.json` is the `tools/usage-service` folder. (As a 
+convenience for developers, this example file is also duplicated in the `pwdusage` usage repostory.)
+
+## Loading `usage.json`
+
+The usage engine will look for the configuration files in the following locations:
+- You can use the environment variable `USAGE_JSON` to specify the (optional) path and
+the file name for the configuration file. You **must** use this method for running a
+usage server in a **docker container** (most users). See the `pwdusage.extend.yml` and 
+`test_service.sh` files in the previous sections for examples of mapping a local copy of
+`usage.json` to a docker container volume.  
+- If the environment variable is not specified, the enginer will try to load 
+`usage.json` from the working directory. 
+- If you are running the engine in CLI mode to dump csv files, you **must** specify the
+location of the configuration file (optional path + file name) using the `--config`
+argument. `USAGE_JSON` is ignored in this mode.
+
+Note: if you have followed the steps for adding `pwdusage` to the Powerwall-Dashboard
+docker stack and your `usage.json` is in the recommended location, everything should run
+out of the box. 
 
 ## Strings from `common.py`
 
+While most of the heavy lifting is done in the `usage.json` file, this configuration 
+file depends heavily on constants defined in `common.py`. This section outlines these
+constants.
+
 The strings defined in the `PDColName` Enum in `common.py` are labels for key calculated
 data columns in the usage engine. You may choose to output any subset of the numeric
 calculations, and you can also change the default names of the outputs to your
 preferred labels.
 
 The following table summarises the strings available as at 13 May 2023. This set may be
 extended in future.
@@ -568,29 +684,31 @@
 section. However, the system provides hooks for extension with additional usage agents. 
 If you know your way around python, you can follow the structure of `simple_agent.py` to
 build your own agent (if not, let me know via an issue and I'll see if I can help built
 an agent for your use case).
 
 # Grafana setup
 
-## JSON datasource
-
-TODO add images to this section.
+This section assumes you have already got a 
+[docker](#add-pwdusage-to-powerwall-dashboard) or [stand alone](#installation-for-developmenttesting) `pwdusage` server up and running, and you know 
+the hostname/host address and port for the server.
 
-If you are using a test usage server, start it now. For a first time run, I'd suggest
-using the example `usage.json` with edits to reflect your influx hostname and 
-local timezone. 
+## JSON datasource
 
-From the general grafana configuration (bottom left):
+From the general grafana configuration (cog wheel icon, bottom left):
 
 - Select `Data sources`.
 - Click `Add data source` and add a JSON data source.
 - Give it a name - the example dash board uses `JSON Usage`. 
 - Set the URL to: `http://<hostname>:<port>/usage_engine`. The default usage engine port
-is 9050, but you can override this via the `USAGE_PORT` environment variable.
+is 9050, but you can override this via the docker `.yml` configuration or via 
+`USAGE_PORT` for a stand alone server.
+
+  ![image](https://github.com/BuongiornoTexas/pwdusage/assets/48264358/2bfe1062-b7b1-40a4-8870-32ca474a9421)
+
 - Hit "Save and Test". You should see two green tick messages "Datasource updated" and 
 "Data source is working". 
 
 ### Datasource troubleshooting
 
 If the usage engine service has not started properly, the second message will show a 
 green "Testing ..." for a while, followed by a red/pink "Gateway Timeout".
@@ -603,46 +721,162 @@
 
 - Using a web browser to open `http://<hostname>:<port>/usage_engine`. The page may 
 give some hints.
 - Check the server log (if you are running docker, check the docker log).
 - If none of this helps, raise an issue at: 
   `https://github.com/BuongiornoTexas/pwdusage/issues`.
 
-### JSON payload
+## Grafana Dashboard setup
+
+This section outlines setting up grafana dashboards based on usage queries. It refers to
+the example dashboards in the `tools/usage-service` folder, and these also provide
+useful starting points for developing your own dashboard. The sample dashboards are: 
+- A usage detail dashboard (the image at the top of this README), which uses
+hourly data generated from the example `usage.json`.
+- Two versions of of a summary statistics dashboard, which use the `summary` payload 
+entry. The [performance sidebar](#performance-sidebar) below explains the difference
+between the versions, and the [JSON payload](#json-payload) section details payload
+options. The v1 output is shown in the following image and is similar to that presented
+in the detailed dashboard. 
+
+![Usage mtd](https://github.com/BuongiornoTexas/pwdusage/assets/48264358/e344ec31-afea-4027-9a73-4d93756aceb4)
+
+The `usage-service` folder also includes an example drop in replacement panel for the
+main dashboard savings panel - built around `summary` and `month_to_date` reporting
+(via [JSON payload](#json-payload)) and the sample `usage.json` (you'll need to tweak it
+to match your utility). This panel loads a little slower than most of the dashboard
+elements, but still much faster than the Tesla power flow animation. 
+
+![Savings panel](https://github.com/BuongiornoTexas/pwdusage/assets/48264358/3c89e711-b775-4139-ba9b-11b17e222de6)
+
+Note 1: I have not spent much time on colors or layout, as each user will need
+to customise these reports to match their utility and their own reporting needs. (I know 
+I've still got a bit of work to do on my own!) However, the example dashboards do
+provide a reasonable idea of what you can do with the usage data and how you can
+manipulate it.
+
+Note 2: Both the detail usage and v1 summary dashboards can be slow to load regardless
+of reporting time interval - refer to the [performance sidebar](#performance-sidebar)
+for reasons and methods to address this issue. The v2 summary dashboard and savings
+panel are quick to load for shorter time intervals (< 1month), but like other grafana
+queries, these will slow down for longer intervals.
+
+The main thing to be aware of when setting up a usage dashboard is that the usage 
+datasource performs a set of computationally expensive (i.e. slow) calculations and then
+returns **all** time of use data in a **single table**. Because of this, and as 
+discussed in the [performance side bar](#performance-sidebar), you should call the usage datasource in only one hero panel per dashboard. If you want to use the same usage 
+data in any other panels on a dashboard, you should then **duplicate** this data using
+the internal grafana `-- Dashboard --` datasource. Finally, because the usage
+datasource returns all of the data, you will need to apply filter transforms in each
+usage panel to get the data that you want to present (and discard the data you don't
+want) - this process is outlined below.
+
+The process for setting up usage panels in a dashboard is:
+- Choose a **hero** panel which you will use as your main usage data source. In
+the "Usage Detail" example dashboard, the "Grid Import" panel is the hero panel. Set
+the Data source to match your JSON pwdusage data source ("JSON Usage" in the examples)
+and set the metric to "Usage".
+  
+  ![Datasource](https://github.com/BuongiornoTexas/pwdusage/assets/48264358/327c6f36-e0bd-4a9c-9c65-7b8104379dee)
+
+- For all other usage panels in the dashboard, set the data source to "-- Dashboard --"
+and set the *Use results from panel* field to the name of your hero panel ("Grid 
+Import").
+
+  ![Duplicate data source](https://github.com/BuongiornoTexas/pwdusage/assets/48264358/8492531b-4577-4a6a-a4f5-c68cee864267) 
+
+- For each usage panel, apply a "Filter by Name" transform to select the variables you
+want to present in the panel. You can either select the variables individually, or you
+can use a regex. Either way, if you want to plot against time, you must select "_time"
+or you will get "No data" errors (ask me how I know ...). An example of regexp that
+selects all grid export power and time is "_time|(Grid export).*\(kWh\)".
+
+- The "Add field from calculation" transform is useful for creating subtotals and 
+totals, and the "Organise fields" transform can be useful for hiding intermediate
+values and arranging fields. To see examples of these transforms, check the "Self 
+Consumption Value" summary stat table in the "Usage Detail" example dashboard.
+
+### Performance sidebar
+
+Unfortunately, there are two interacting performance issues that impact grafana 
+presentation of usage engine data. For reference, the performance benchmarks in this 
+section are for a 2013 Celeron NUC with 2GB(?) memory and a SATA SSD.
+
+1) A usage engine query is slower than a normal grafana/influxdb query. This is because
+it includes a set of transform calculations to generate the usage data and another
+set of transforms that convert the usage data to a JSON format for export to grafana.
+While it is definitely possible to improve this performance, it will be at the cost of 
+much harder development effort - I've accepted the performance hit as as consequence
+of simpler development using pandas under python.
+
+    The speed of usage engine responses is non-issue for shorter time intervals 
+  (< 1 month), but becomes significant above this: ~6s for 6 months, 14s for 10 months.
+  This is slower than other Powerwall-Dashboard queries, but still acceptable for most uses. 
+
+    However! Grafana usage panels will timeout if a dashboard includes two usage queries
+with long (6+ months)intervals. 
+
+    To avoid the timeout problem for long interval queries, I recommend using only one
+usage query per dashboard, and then duplicating the query via the grafana Dashboard data
+source. This process is detailed in the previous section. 
+
+2) The second performance problem arises if we want to use a lot of usage panels and we
+use the grafana Dashboard data source (e.g. the example detail dashboard and the v1
+summary dashboard). In this situation, the dashboard loads slowly for all time intervals
+(the first load can be very slow). But, they do load!
+
+There are two possible approaches to addressing the performance problems:
+
+- If you need multiple panels for complex views on the data (e.g. the detailed
+usage dashboard), you will have to accept the slow load times.
+
+- If the data you want to present is simpler, you may be able to rework your dashboard
+to use fewer usage panels. This is the approach taken in the v2 summary dashboard, which
+replaces the 7 panels in the v1 dashboard with 2 panels - albeit at the cost of some
+readability.
+
+In summary, regardless of the approach adopted, you should only use one usage engine 
+query per dashboard and duplicate data to other panels via grafana Dashboard data
+sources. If you don't you may run into panel timeouts.
+
+## JSON payload
 
 The usage datasource supports a `payload` dictionary, which can be specified in the 
-grafana query configuration, as shown in TODO insert screen shot. TODO This may belong
-in the next section?
+grafana query configuration, as shown in the following image.
+
+![JSON Payload](https://github.com/BuongiornoTexas/pwdusage/assets/48264358/4bf4d2ee-5575-4dbc-87b4-b6c9db7b7597)
 
 The supported payload entries are:
 
 ```
 {
   "summary": [true | false], 
   "month_to_date": [true | false], 
   "year_to_date": [true | false], 
-  "resample": [true | false], 
+  "resample": [true | false] 
 }
 ```
-1) If `summary` is `true` (default `false`), the values for each variable over the 
+1) Note that `true` and `false` are both uncapitalised and unquoted.
+
+2) If `summary` is `true` (default `false`), the values for each variable over the 
 reporting range are summed to give total power and total costs, and the resulting totals
 are returned (per interval values are not reported/discarded). Note that transforms
 can be used in grafana to get the same result if you want to work with both time series
 and summary values (use `false` in this case). 
 
-2) Setting `month_to_date` to `true` (default `false`), the report time range is 
+3) Setting `month_to_date` to `true` (default `false`), the report time range is 
 replaced with the current calendar month (utility for dashboard reporting). Both 
 `summary` and `resample` apply normally. 
 
-3) Setting `year_to_date` to `true` (default `false`), the report time range is 
+4) Setting `year_to_date` to `true` (default `false`), the report time range is 
 replaced with the current year based on the `year_anchor` setting (utility for dashboard
 reporting). Both `summary` and `resample` apply normally. If `month_to_date` and 
 `year_to_date` are both true, `year_to_date` takes priority and is reported.
 
-4) If `resample` is `true` (note: unquoted, lower case!), the usage data is resampled
+5) If `resample` is `true` (default), the usage data is resampled
    according to the following rules: 
 
     | Query time range | Resampling |
     |------------------|------------|
     | Within a single day    | Hourly     |
     | Within a single month  | Weekly     |
     | Within a single year   | Monthly    |
@@ -651,25 +885,14 @@
     In this context within a single day means the query interval is for one calendar day
     maximum, and so on for the other intervals. If resample is set to false, the data is 
     not resampled and output is returned at the raw influx database query intervals. 
 
     The default resampling is `true`, and this can also be over-ridden in `usage.json`.
     If `summary` is `true`, `resample` is ignored.
 
-## Grafana Dashboard setup
-
-TODO write this section.
-
-Note: as of version 0.9.4, the sample grafana files discussed in this section are held
-at: 
-https://github.com/BuongiornoTexas/Powerwall-Dashboard/tree/main/tools/usage-service.
-
-In the interim, I've provided example dashboard called `example_dashboard.json`. Import
-this into grafana and have an explore.
-
 # Installation for development/testing 
 
 ## Testing pwdusage
 
 As of version 0.9.4, `pwdusage` is available as a pypi package, and it and its 
 dependencies can be installed using pip. This is the recommended method if you want to
 test the service and don't want to set up the docker container or do any development.
@@ -742,32 +965,32 @@
                 "USAGE_PORT": "9050",
                 "USAGE_JSON": "C:/users/xxxx/yyy/usage.json"
             }
         }
     ]
 }
 ```
-- For initial testing, create a copy of the `example_usage.json` file, set the 
-`USAGE_JSON` environment variable to point at this file and modify the contents of the
-file  so that `influx_url` points at your influx server (probably the same machine as
-your Powerwall-Dashboard) and your `timezone` is correct.
+- For initial testing, create a `usage.json` configuration file as detailed in 
+[Test Docker Image](#test-docker-image).
+- Set the `USAGE_JSON` environment variable to point at this `usage.json`.
 - At this point, you should be able to run the server using: 
   ```
   py -m pwdusage.server
   ```
   You should then check that the usage server is responding by pointing a web browser at
   `http://server.address:<port>/usage_engine`. 
 - If everything is as it should be, you should see a page containing the message:
 
   ```
   Usage Engine Status	"Engine OK, tariffs (re)loaded"
   ```
-If you don't see this, please check that you are using the unmodified `usage.json`. If 
+If you don't see this, please check that `usage.json` matches the description in 
+[Test Docker Image](#test-docker-image). If 
 you still have problems, let us know on the dev issue thread to see if we can trouble 
 shoot.
 
 If you do get the expected response, you can now modify the `usage.json` file to
-reflect your own tariff structure.
+reflect your own tariff structure [`pwdusage` Configuration](#pwdusage-configuration).
 
 Finally, you can run the engine in cli mode to generate .csv dump files for debugging.
 For this, use `py -m pwdusage.engine [arguments]`, with help available from 
-`py pwdusage.engine -h`.
+`py pwdusage.engine -h`.
```

### Comparing `pwdusage-0.9.4/pyproject.toml` & `pwdusage-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pwdusage"
-version = "v0.9.4"
+version = "v1.0.0"
 authors = [
   {name="BuongiornoTexas"},
 ]
 description = "Usage (mainly time of use) proxy microservice for Powerwall-Dashboard."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

