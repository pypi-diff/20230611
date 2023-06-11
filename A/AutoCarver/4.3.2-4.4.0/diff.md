# Comparing `tmp/AutoCarver-4.3.2.tar.gz` & `tmp/AutoCarver-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AutoCarver-4.3.2.tar", last modified: Fri Jun  9 13:59:03 2023, max compression
+gzip compressed data, was "AutoCarver-4.4.0.tar", last modified: Sun Jun 11 09:49:42 2023, max compression
```

## Comparing `AutoCarver-4.3.2.tar` & `AutoCarver-4.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 13:59:03.000000 AutoCarver-4.3.2/
-drwxrwxrwx   0        0        0        0 2023-06-09 13:59:03.000000 AutoCarver-4.3.2/AutoCarver/
--rw-rw-rw-   0        0        0    24083 2023-05-25 10:56:20.000000 AutoCarver-4.3.2/AutoCarver/AutoCarver.py
--rw-rw-rw-   0        0        0     9449 2023-05-25 10:56:20.000000 AutoCarver-4.3.2/AutoCarver/Converters.py
--rw-rw-rw-   0        0        0    52826 2023-05-25 10:56:20.000000 AutoCarver-4.3.2/AutoCarver/Discretizers.py
--rw-rw-rw-   0        0        0    28159 2023-05-25 10:56:20.000000 AutoCarver-4.3.2/AutoCarver/FeatureSelector.py
--rw-rw-rw-   0        0        0        0 2023-01-10 08:49:10.000000 AutoCarver-4.3.2/AutoCarver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:59:03.000000 AutoCarver-4.3.2/AutoCarver.egg-info/
--rw-rw-rw-   0        0        0     7119 2023-06-09 13:58:57.000000 AutoCarver-4.3.2/AutoCarver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-09 13:59:01.000000 AutoCarver-4.3.2/AutoCarver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 13:58:57.000000 AutoCarver-4.3.2/AutoCarver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-09 13:58:57.000000 AutoCarver-4.3.2/AutoCarver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-01-05 13:13:13.000000 AutoCarver-4.3.2/LICENSE
--rw-rw-rw-   0        0        0     7119 2023-06-09 13:59:03.000000 AutoCarver-4.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     6346 2023-05-14 13:54:01.000000 AutoCarver-4.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 13:59:03.000000 AutoCarver-4.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-06-09 13:56:46.000000 AutoCarver-4.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:49:42.932103 AutoCarver-4.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:49:42.932103 AutoCarver-4.4.0/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)    23484 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/AutoCarver/AutoCarver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/AutoCarver/Converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51578 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/AutoCarver/Discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27407 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/AutoCarver/FeatureSelector.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/AutoCarver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:49:42.932103 AutoCarver-4.4.0/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-06-11 09:49:42.000000 AutoCarver-4.4.0/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-11 09:49:42.000000 AutoCarver-4.4.0/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 09:49:42.000000 AutoCarver-4.4.0/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 09:49:42.000000 AutoCarver-4.4.0/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-06-11 09:49:42.932103 AutoCarver-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17418 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 09:49:42.932103 AutoCarver-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `AutoCarver-4.3.2/AutoCarver/AutoCarver.py` & `AutoCarver-4.4.0/AutoCarver/AutoCarver.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,599 +1,599 @@
-from .Discretizers import GroupedList, GroupedListDiscretizer, is_equal
-from IPython.display import display_html
-from matplotlib.pyplot import subplots, show
-from matplotlib.ticker import PercentFormatter
-from numpy import sort, nan, inf, float32, where, isin, argsort, array, append, quantile, linspace, argmin, sqrt, random
-from pandas import DataFrame, Series, isna, qcut, notna, unique, concat, crosstab
-from pandas.api.types import is_string_dtype
-from scipy.stats import chi2_contingency
-from seaborn import color_palette, despine
-from tqdm.notebook import tqdm
-from typing import Any, Dict, List, Tuple
-
-
-class AutoCarver(GroupedListDiscretizer):
-    """ Automatic carving of continuous, categorical and categorical ordinal features 
-    that maximizes association with a binary target.
-
-    Modalities/values of features are carved/regrouped according to a computed specific
-    order defined based on their types:
-     - [Qualitative features] grouped based on modality target rate.
-     - [Qualitative ordinal features] grouped based on specified modality order.
-     - [Quantitative features] grouped based on the order of their values.
-    Uses Tschurpow's T to find the optimal carving (regrouping) of modalities/values
-    of features.
-
-    Parameters
-    ----------
-    values_orders: dict, default {}
-        Dictionnary of features and list of their respective values' order.
-        Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
-
-    sort_by: str, default 'tschuprowt'
-        Association measure used to find the optimal group modality combination.
-        Implemented: ['cramerv', 'tschuprowt']
-
-    max_n_mod: int, default 5
-        Maximum number of modalities for the carved features (excluding `numpy.nan`).
-         - All possible combinations of less than `max_n_mod` groups of modalities will be tested. 
-        Recommandation: `max_n_mod` should be set from 4 (faster) to 6 (preciser).
-
-    keep_nans: bool, default False
-        Whether or not to group `numpy.nan` to other modalities/values.
-
-    Examples
-    ----------
-
-    from AutoCarver import AutoCarver
-    from Discretizers import Discretizer
-    from sklearn.pipeline import Pipeline
-
-    # defining training and testing sets
-    X_train, y_train = train_set, train_set[target]
-    X_test, y_test = test_set, test_set[target]
-
-    # specifying features to be carved
-    selected_quanti = ['amount', 'distance', 'length', 'height']
-    selected_quali = ['age', 'type', 'grade', 'city']
-
-    # specifying orders of categorical ordinal features
-    values_orders = {
-        'age': ['0-18', '18-30', '30-50', '50+'],
-        'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
-    }
-
-    # pre-processing of features into categorical ordinal features
-    discretizer = Discretizer(selected_quanti, selected_quali, min_freq=0.02, q=20, values_orders=values_orders)
-    X_train = discretizer.fit_transform(X_train, y_train)
-    X_test = discretizer.transform(X_test)
-
-    # storing Discretizer
-    pipe = [('Discretizer', discretizer)]
-
-    # updating features' values orders (at this step every features are qualitative ordinal)
-    values_orders = discretizer.values_orders
-
-    # intiating AutoCarver
-    auto_carver = AutoCarver(values_orders, sort_by='cramerv', max_n_mod=5, sample_size=0.01)
-
-    # fitting on training sample
-    # a test sample can be specified to evaluate carving robustness
-    X_train = auto_carver.fit_transform(X_train, y_train, X_test, y_test)
-
-    # applying transformation on test sample
-    X_test = auto_carver.transform(X_test)
-
-    # identifying non stable/robust features
-    print(auto_carver.non_viable_features)
-
-    # storing fitted GroupedListDiscretizer in a sklearn.pipeline.Pipeline
-    pipe += [('AutoCarver', auto_carver)]
-    pipe = Pipeline(pipe)
-
-    # applying pipe to a validation set or in production
-    X_val = pipe.transform(X_val)
-
-    """
-   
-    def __init__(self, values_orders: Dict[str, Any], *, sort_by: str='tschuprowt',
-                 copy: bool=False, max_n_mod: int=5, dropna: bool=True,
-                 verbose: bool=True, str_nan: str='__NAN__') -> None:
-        
-        self.features = list(values_orders.keys())
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.non_viable_features: List[str] = []  # list of features non viable features
-        self.max_n_mod = max_n_mod  # maximum number of modality per feature
-        self.dropna = dropna  # whether or not to group NaNs with other modalities
-        
-        # association measure used to find the best groups
-        implemented = ['tschuprowt', 'cramerv']
-        assert sort_by in implemented, f"Measure {sort_by} is not yet implemented. Choose from: {', '.join(implemented)}."
-        self.sort_by = sort_by
-
-        self.copy = copy
-        self.verbose = verbose
-        self.str_nan = str_nan
-    
-    def prepare_data(self, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> Tuple[DataFrame, Series, DataFrame, Series]:
-        """ Checks validity of provided data"""
-        
-        # preparing train sample
-        # checking for binary target
-        y_values = unique(y)
-        assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
-        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
-        
-        # checking for quantitative columns
-        is_object = X[self.features].dtypes.apply(is_string_dtype)
-        assert all(is_object), f"Non-string features in X: {', '.join(is_object[~is_object].index)}, consider using Discretizer."
-        
-        # Copying DataFrame if requested
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-        
-        # preparing test sample
-        # checking for binary target
-        if y_test is not None:
-            assert X_test is not None, "y_test was provided but X_test is missing"
-            y_values = unique(y_test)
-            assert (0 in y_values) & (1 in y_values), "y_test must be a binary Series (int or float, not object)"
-            assert len(y_values) == 2, "y_test must be a binary Series (int or float, not object)"
-        
-        # Copying DataFrame if requested
-        Xtestc = X_test
-        if X_test is not None:
-            assert y_test is not None, "X_test was provided but y_test is missing"
-            if self.copy:
-                Xtestc = X_test.copy()
-        
-            # checking for quantitative columns
-            is_object = X_test[self.features].dtypes.apply(is_string_dtype)
-            assert all(is_object), f"Non-string features in X_test: {', '.join(is_object[~is_object].index)}, consider using Discretizer."
-            
-        return Xc, y, Xtestc, y_test
-    
-    def fit(self, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> None:
-
-        # preparing datasets and checking for wrong values
-        Xc, y, Xtestc, y_test = self.prepare_data(X, y, X_test, y_test)
-        
-        # automatic carving of each feature
-        for n, feature in tqdm(enumerate(self.features), total=len(self.features), disable=self.verbose):
-
-            # printing the group statistics and determining default ordering
-            if self.verbose:
-                print(f"\n---\n[AutoCarver] Fit {feature} ({n+1}/{len(self.features)})")
-
-            # getting best combination
-            best_groups = self.get_best_combination(feature, Xc, y, Xtestc, y_test)
-
-            # feature can not be carved robustly
-            if not bool(best_groups):
-                self.non_viable_features += [feature]  # adding it to list of non viable features
-
-        # discretizing features based on each feature's values_order
-        super().__init__(self.values_orders, str_nan=self.str_nan, copy=self.copy, output=float)
-        super().fit(X, y)
-
-        return self
-
-
-    def get_best_combination(self, feature: str, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> Dict[str, Any]:
-        """ Carves a feature"""
-
-        # computing crosstabs
-        # crosstab on TRAIN
-        xtab = nan_crosstab(X[feature], y, self.str_nan)
-
-        # crosstab on TEST
-        xtab_test = None
-        if X_test is not None:
-            xtab_test = nan_crosstab(X_test[feature], y_test, self.str_nan)
-
-        # printing the group statistics
-        if self.verbose:
-            self.display_xtabs(feature, 'Raw', xtab, xtab_test)
-
-        # measuring association with target for each combination and testing for stability on TEST
-        best_groups = best_combination(self.values_orders.get(feature), self.max_n_mod, self.sort_by, xtab, xtab_test, dropna=True, str_nan=self.str_nan)
-
-        # update of the values_orders grouped modalities in values_orders
-        if best_groups:
-            xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
-
-        # testing adding NaNs to built groups
-        if (self.str_nan in xtab.index) & self.dropna & (self.str_nan not in self.values_orders.get(feature)):
-
-            # measuring association with target for each combination and testing for stability on TEST
-            best_groups = best_combination(self.values_orders.get(feature), self.max_n_mod, self.sort_by, xtab, xtab_test, dropna=False, str_nan=self.str_nan)
-
-            # adding NaN to the order
-            self.insert_nan(feature, xtab)
-
-            # update of the values_orders grouped modalities in values_orders
-            if best_groups:
-                xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
-
-        # printing the new group statistics
-        if self.verbose and best_groups:
-            self.display_xtabs(feature, 'Fitted', xtab, xtab_test)
-
-        return best_groups
-
-    def insert_nan(self, feature: str, xtab: DataFrame) -> GroupedList:
-        """ Inserts NaNs in the order"""
-
-        # accessing order for specified feature
-        order = self.values_orders.get(feature)
-
-        # adding nans at the end of the order
-        if self.str_nan not in order:
-            order = order.append(self.str_nan)
-
-            # updating values_orders
-            self.values_orders.update({feature: order})
-
-
-    def update_order(self, feature: str, best_groups: GroupedList, xtab: DataFrame, xtab_test: DataFrame=None) -> Tuple[DataFrame, DataFrame]:
-        """ Updates the values_orders and xtabs according to the best_groups"""
-
-        # updating values_orders with best_combination 
-        self.values_orders.update({feature: best_groups})
-
-        # update of the TRAIN crosstab
-        best_combi = list(map(best_groups.get_group, xtab.index))
-        xtab = xtab.groupby(best_combi, dropna=False).sum()
-
-        # update of the TEST crosstab
-        if xtab_test is not None:
-            best_combi = list(map(best_groups.get_group, xtab_test.index))
-            xtab_test = xtab_test.groupby(best_combi, dropna=False).sum()
-        
-        return xtab, xtab_test
-    
-    def display_xtabs(self, feature: str, caption: str, xtab: DataFrame, xtab_test: DataFrame=None) -> None:
-        """ Pretty display of frequency and target rate per modality on the same line. """
-        
-        # known_order per feature
-        known_order = self.values_orders.get(feature)
-        
-        # target rate and frequency on TRAIN
-        train_stats = stats_xtab(xtab, known_order)
-    
-        # target rate and frequency on TEST
-        if xtab_test is not None:
-            test_stats = stats_xtab(xtab_test, train_stats.index, train_stats.labels)
-            test_stats = test_stats.set_index('labels')  # setting labels as indices
-        
-        # setting TRAIN labels as indices
-        train_stats = train_stats.set_index('labels')
-
-        # Displaying TRAIN modality level stats
-        train_style = train_stats.style.background_gradient(cmap='coolwarm')  # color scaling
-        train_style = train_style.set_table_attributes("style='display:inline'")  # printing in notebook
-        train_style = train_style.set_caption(f'{caption} distribution on X:')  # title
-        html = train_style._repr_html_()
-        
-        # adding TEST modality level stats
-        if xtab_test is not None:
-            test_style = test_stats.style.background_gradient(cmap='coolwarm')  # color scaling
-            test_style = test_style.set_table_attributes("style='display:inline'")  # printing in notebook
-            test_style = test_style.set_caption(f'{caption} distribution on X_test:')  # title
-            html += ' ' + test_style._repr_html_()
-
-        # displaying html of colored DataFrame
-        display_html(html, raw=True)
-
-def groupedlist_combination(combination: List[List[Any]], order: GroupedList) -> GroupedList:
-    """ Converts a list of combination to a GroupedList"""
-    
-    order_copy = GroupedList(order)
-    for combi in combination:
-        order_copy.group_list(combi, combi[0])
-    
-    return order_copy
-
-def stats_xtab(xtab: DataFrame, known_order: List[Any]=None, known_labels: List[Any]=None) -> DataFrame:
-    """ Computes column (target) rate per row (modality) and row frequency"""
-    
-    # target rate and frequency statistics per modality
-    stats = DataFrame({
-        # target rate per modality
-        'target_rate': xtab[1].divide(xtab.sum(axis=1)),
-        # frequency per modality
-        'frequency': xtab.sum(axis=1) / xtab.sum().sum()
-    })
-    
-    # sorting statistics
-    # case 0: default ordering based on observed target rate
-    if known_order is None:
-        order = list(stats.sort_values('target_rate', ascending=True).index)
-    
-    # case 1: a known_order was provided
-    else:
-        order = known_order[:]
-      
-    # modalities' labels
-    # case 0: default labels
-    if known_labels is None:
-        
-        # accessing string representation of the GroupedList
-        if isinstance(known_order, GroupedList):
-            labels = known_order.get_repr()
-
-        # labels are the default order
-        else:
-            labels = order[:]
-            
-    # case 1: known_labels were provided
-    else:
-        labels = known_labels[:]
-            
-            
-    # keeping values missing from the order at the end
-    unknown_modality = [mod for mod in xtab.index if mod not in order]
-    for mod in unknown_modality:
-        order = [c for c in order if not is_equal(c, mod)] + [mod]
-        labels = [c for c in labels if not is_equal(c, mod)] + [mod]
-    
-    # sorting statistics
-    stats = stats.reindex(order, fill_value=0)
-    stats['labels'] = labels
-    
-    return stats
-
-def apply_combination(xtab: DataFrame, combination: GroupedList) -> Dict[str, Any]:
-    """ applies a modality combination to a crosstab """
-
-    # initiating association dict
-    association = {'combination': combination}
-
-    # grouping modalities in the initial crosstab
-    groups = list(map(combination.get_group, xtab.index))
-    combi_xtab = xtab.groupby(groups, dropna=False).sum()
-    association.update({'combi_xtab': combi_xtab})
-
-    # measuring association with the target
-    association.update(association_xtab(combi_xtab))
-
-    return association
-
-def best_combination(order: GroupedList, max_n_mod: int, sort_by: str, xtab_train: DataFrame, xtab_dev: DataFrame=None, dropna: bool=True, str_nan: str=None):
-    """ Finds the best combination of groups of feature's values:
-     - Most associated combination on train sample 
-     - Stable target rate of combination on test sample.
-    """
-    
-    # copying crosstabs
-    xtab = xtab_train
-    xtab_test = xtab_dev
-    
-    # removing nans if requested
-    if dropna:
-        
-        # crosstab on TRAIN
-        xtab = xtab_train[xtab_train.index != str_nan]  # filtering out nans
-
-        # crosstab on TEST
-        if xtab_test is not None:
-            xtab_test = xtab_dev[xtab_dev.index != str_nan]  # filtering out nans
-    
-        # getting all possible combinations for the feature without NaNS
-        combinations = get_all_combinations(order, max_n_mod, raw=False)
-    
-    # keeping nans as a modality
-    else:
-    
-        # getting all possible combinations for the feature with NaNS
-        combinations = get_all_nan_combinations(order, str_nan, max_n_mod)
-
-    # computing association measure per combination 
-    associations = [apply_combination(xtab, combi) for combi in combinations]
-
-    # sort according to association measure
-    if len(combinations) > 0:
-        associations = DataFrame(associations)
-        associations.sort_values(sort_by, inplace=True, ascending=False)
-        associations = associations.to_dict(orient='records')
-
-    # testing associations
-    # case 0: no test set was provided
-    if xtab_test is None and len(associations) > 0:
-        return associations[0]
-    
-    # case 1: testing viability on provided TEST sample
-    else:
-        for association in associations:
-            
-            # needed parameters
-            combination, combi_xtab = association['combination'], association['combi_xtab']
-
-            # grouping modalities in the initial crosstab
-            combi_xtab_test = xtab_test.groupby(list(map(combination.get_group, xtab_test.index)), dropna=False).sum()
-
-            # checking that all non-nan groups are in TRAIN and TEST
-            unq_x =  [v for v in unique(combi_xtab.index) if v != notna(v)]
-            unq_xtest = [v for v in unique(combi_xtab_test.index) if v != notna(v)]
-            viability = all([e in unq_x for e in unq_xtest])
-            viability = viability and all([e in unq_xtest for e in unq_x])
-
-            # same target rate order in TRAIN and TEST
-            train_target_rate = combi_xtab[1].divide(combi_xtab[0]).sort_values()
-            test_target_rate = combi_xtab_test[1].divide(combi_xtab_test[0]).sort_values()
-            viability = viability and all(train_target_rate.index == test_target_rate.index)
-
-            # checking that some combinations were provided
-            if viability:
-
-                association.update({'combi_xtab_test': combi_xtab_test})
-
-                return association
-
-
-def get_all_combinations(values: GroupedList, max_n_mod: int=None, raw: bool=False) -> List[GroupedList]:
-
-    # maximum number of classes
-    q = len(values)
-
-    # desired max number of classes
-    if max_n_mod is None:
-        max_n_mod = q
-
-    # all possible combinations
-    combinations = list()
-    for n_class in range(2, max_n_mod + 1):
-        combinations += get_combinations(n_class, q)
-
-    # getting real feature values
-    combinations = [[values[int(c[0]): int(c[1]) + 1] for c in combi] for combi in combinations]
-    
-    # converting back to GroupedList
-    if not raw:
-        combinations = [groupedlist_combination(combination, values) for combination in combinations]
-
-    return combinations
-
-def get_all_nan_combinations(order: GroupedList, str_nan: str, max_n_mod: int) -> List[GroupedList]:
-    """ all possible combinations of modalities with numpy.nan"""
-    
-    # computing all non-NaN combinations
-    # case 0: several modalities -> several combinations
-    if len(order) > 1:
-        combinations = get_all_combinations(order, max_n_mod-1, raw=True)
-    # case 1: unique or no modality -> two combinations
-    else:
-        combinations = []
-
-    # iterating over each combinations of non-NaNs
-    new_combinations = []
-    for combi in combinations:
-
-         # NaNs not attributed to a group (own modality)
-        new_combinations += [combi + [[str_nan]]] 
-
-        # NaNs attributed to a group of non NaNs
-        for n in range(len(combi)):
-
-            # grouping NaNs with an existing group
-            new_combination = [combi[n] + [str_nan]]
-
-            # adding other groups unchanged
-            pre = [o for o in combi[:n]]
-            nex = [o for o in combi[n+1:]]
-            new_combinations += [pre + new_combination + nex]
-            
-    # adding NaN to order
-    if str_nan not in order:
-        order = order.append(str_nan)
-    
-    # converting back to GroupedList
-    new_combinations = [groupedlist_combination(combination, order) for combination in new_combinations] 
-
-    return new_combinations
-
-
-def consecutive_combinations(n_remaining: int, start: int, end: int, grp_for_this_step: list=None):
-    """HELPER finds all consecutive combinations between start and end.    """
-
-    # Import de la liste globale
-    global __li_of_res__
-
-    # initiating group
-    if not grp_for_this_step:
-        grp_for_this_step = []
-    
-    # stopping when there are non more remaining classes
-    if n_remaining == 0:
-        
-        ### On ajoute le dernier quantile restant au découpage ###
-        grp_for_this_step += [(start, end)]
-
-        ### Ajout du découpage réalisé au groupe des solutions ###
-        __li_of_res__ += [grp_for_this_step]
-
-    
-    # adding all possible combinations of each possible range
-    else:
-        
-        ### Parcours de toutes les valeurs possibles de fin pour le i-ème groupe du groupement à x quantiles ###
-        for i in range(start, end):
-
-            consecutive_combinations(n_remaining-1, i+1, end, grp_for_this_step + [(start, i)])
-            
-def get_combinations(n_class, q):
-    """HELPER recupération des combinaisons possibles de q quantiles pour n_class."""
-    
-    globals()['__li_of_res__'] = []
-
-    consecutive_combinations(n_class-1, 0, q-1)
-    
-    combinations = [list(map(lambda u: (str(u[0]).zfill(len(str(q-1))), str(u[1]).zfill(len(str(q-1)))), l)) for l in __li_of_res__]
-    
-    return combinations
-
-def association_xtab(xtab: DataFrame):
-    """ Computes measures of association between feature x and feature2. """
-
-    # numnber of observations
-    n_obs = xtab.sum().sum()
-
-    # number of values taken by the features
-    n_mod_x, n_mod_y = len(xtab.index), len(xtab.columns)
-    min_n_mod = min(n_mod_x, n_mod_y)
-
-    # Chi2 statistic
-    chi2 = chi2_contingency(xtab)[0]
-
-    # Cramer's V
-    cramerv = 0
-    if min_n_mod > 1:
-        cramerv = sqrt(chi2 / n_obs / (min_n_mod - 1))
-
-    # Tschuprow's T
-    dof_mods = sqrt((n_mod_x - 1) * (n_mod_y - 1))
-    tschuprowt = 0
-    if dof_mods > 0:
-        tschuprowt = sqrt(chi2 / n_obs / dof_mods)
-
-    results = {'cramerv': cramerv, 'tschuprowt': tschuprowt}
-    
-    return results
-
-def nan_crosstab(x: Series, y: Series, str_nan: str='__NAN__'):
-    """ Crosstab that keeps nans as a specific value"""
-    
-    # keeping NaNs as a specific modality
-    x_filled = x.fillna(str_nan)  # filling NaNs
-
-    # computing initial crosstabs
-    xtab = crosstab(x_filled, y)
-    
-    return xtab
-
-
-def plot_stats(stats):
-    """ Barplot of the volume and target rate"""
-    
-    x = [0] + [elt for e in stats['frequency'].cumsum()[:-1] for elt in [e] * 2] + [1]
-    y2 = [elt for e in list(stats['target_rate']) for elt in [e]*2]
-    s = list(stats.index)
-    scaled_y2 = [(y-min(y2)) / (max(y2) - min(y2)) for y in y2]
-    c = color_palette("coolwarm", as_cmap=True)(scaled_y2)
-
-    fig, ax = subplots()
-
-    for i in range(len(stats)):
-        k = i*2
-        ax.fill_between(x[k: k+2], [0, 0], y2[k: k+2], color=c[k])
-        ax.text(sum(x[k: k+2]) / 2, y2[k], s[i], rotation=90, ha='center', va='bottom')
-
-    ax.xaxis.set_major_formatter(PercentFormatter(xmax=1))    
-    ax.yaxis.set_major_formatter(PercentFormatter(xmax=1))    
-    ax.set_xlabel('Volume')
-    ax.set_ylabel('Target rate')
-    ax.set_xlim(0, 1)
-    ax.set_ylim(0)
-    despine()
-    
-    return fig, ax
+from .Discretizers import GroupedList, GroupedListDiscretizer, is_equal
+from IPython.display import display_html
+from matplotlib.pyplot import subplots, show
+from matplotlib.ticker import PercentFormatter
+from numpy import sort, nan, inf, float32, where, isin, argsort, array, append, quantile, linspace, argmin, sqrt, random
+from pandas import DataFrame, Series, isna, qcut, notna, unique, concat, crosstab
+from pandas.api.types import is_string_dtype
+from scipy.stats import chi2_contingency
+from seaborn import color_palette, despine
+from tqdm.notebook import tqdm
+from typing import Any, Dict, List, Tuple
+
+
+class AutoCarver(GroupedListDiscretizer):
+    """ Automatic carving of continuous, categorical and categorical ordinal features 
+    that maximizes association with a binary target.
+
+    Modalities/values of features are carved/regrouped according to a computed specific
+    order defined based on their types:
+     - [Qualitative features] grouped based on modality target rate.
+     - [Qualitative ordinal features] grouped based on specified modality order.
+     - [Quantitative features] grouped based on the order of their values.
+    Uses Tschurpow's T to find the optimal carving (regrouping) of modalities/values
+    of features.
+
+    Parameters
+    ----------
+    values_orders: dict, default {}
+        Dictionnary of features and list of their respective values' order.
+        Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
+
+    sort_by: str, default 'tschuprowt'
+        Association measure used to find the optimal group modality combination.
+        Implemented: ['cramerv', 'tschuprowt']
+
+    max_n_mod: int, default 5
+        Maximum number of modalities for the carved features (excluding `numpy.nan`).
+         - All possible combinations of less than `max_n_mod` groups of modalities will be tested. 
+        Recommandation: `max_n_mod` should be set from 4 (faster) to 6 (preciser).
+
+    keep_nans: bool, default False
+        Whether or not to group `numpy.nan` to other modalities/values.
+
+    Examples
+    ----------
+
+    from AutoCarver import AutoCarver
+    from Discretizers import Discretizer
+    from sklearn.pipeline import Pipeline
+
+    # defining training and testing sets
+    X_train, y_train = train_set, train_set[target]
+    X_test, y_test = test_set, test_set[target]
+
+    # specifying features to be carved
+    selected_quanti = ['amount', 'distance', 'length', 'height']
+    selected_quali = ['age', 'type', 'grade', 'city']
+
+    # specifying orders of categorical ordinal features
+    values_orders = {
+        'age': ['0-18', '18-30', '30-50', '50+'],
+        'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
+    }
+
+    # pre-processing of features into categorical ordinal features
+    discretizer = Discretizer(selected_quanti, selected_quali, min_freq=0.02, q=20, values_orders=values_orders)
+    X_train = discretizer.fit_transform(X_train, y_train)
+    X_test = discretizer.transform(X_test)
+
+    # storing Discretizer
+    pipe = [('Discretizer', discretizer)]
+
+    # updating features' values orders (at this step every features are qualitative ordinal)
+    values_orders = discretizer.values_orders
+
+    # intiating AutoCarver
+    auto_carver = AutoCarver(values_orders, sort_by='cramerv', max_n_mod=5, sample_size=0.01)
+
+    # fitting on training sample
+    # a test sample can be specified to evaluate carving robustness
+    X_train = auto_carver.fit_transform(X_train, y_train, X_test, y_test)
+
+    # applying transformation on test sample
+    X_test = auto_carver.transform(X_test)
+
+    # identifying non stable/robust features
+    print(auto_carver.non_viable_features)
+
+    # storing fitted GroupedListDiscretizer in a sklearn.pipeline.Pipeline
+    pipe += [('AutoCarver', auto_carver)]
+    pipe = Pipeline(pipe)
+
+    # applying pipe to a validation set or in production
+    X_val = pipe.transform(X_val)
+
+    """
+   
+    def __init__(self, values_orders: Dict[str, Any], *, sort_by: str='tschuprowt',
+                 copy: bool=False, max_n_mod: int=5, dropna: bool=True,
+                 verbose: bool=True, str_nan: str='__NAN__') -> None:
+        
+        self.features = list(values_orders.keys())
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.non_viable_features: List[str] = []  # list of features non viable features
+        self.max_n_mod = max_n_mod  # maximum number of modality per feature
+        self.dropna = dropna  # whether or not to group NaNs with other modalities
+        
+        # association measure used to find the best groups
+        implemented = ['tschuprowt', 'cramerv']
+        assert sort_by in implemented, f"Measure {sort_by} is not yet implemented. Choose from: {', '.join(implemented)}."
+        self.sort_by = sort_by
+
+        self.copy = copy
+        self.verbose = verbose
+        self.str_nan = str_nan
+    
+    def prepare_data(self, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> Tuple[DataFrame, Series, DataFrame, Series]:
+        """ Checks validity of provided data"""
+        
+        # preparing train sample
+        # checking for binary target
+        y_values = unique(y)
+        assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
+        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
+        
+        # checking for quantitative columns
+        is_object = X[self.features].dtypes.apply(is_string_dtype)
+        assert all(is_object), f"Non-string features in X: {', '.join(is_object[~is_object].index)}, consider using Discretizer."
+        
+        # Copying DataFrame if requested
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+        
+        # preparing test sample
+        # checking for binary target
+        if y_test is not None:
+            assert X_test is not None, "y_test was provided but X_test is missing"
+            y_values = unique(y_test)
+            assert (0 in y_values) & (1 in y_values), "y_test must be a binary Series (int or float, not object)"
+            assert len(y_values) == 2, "y_test must be a binary Series (int or float, not object)"
+        
+        # Copying DataFrame if requested
+        Xtestc = X_test
+        if X_test is not None:
+            assert y_test is not None, "X_test was provided but y_test is missing"
+            if self.copy:
+                Xtestc = X_test.copy()
+        
+            # checking for quantitative columns
+            is_object = X_test[self.features].dtypes.apply(is_string_dtype)
+            assert all(is_object), f"Non-string features in X_test: {', '.join(is_object[~is_object].index)}, consider using Discretizer."
+            
+        return Xc, y, Xtestc, y_test
+    
+    def fit(self, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> None:
+
+        # preparing datasets and checking for wrong values
+        Xc, y, Xtestc, y_test = self.prepare_data(X, y, X_test, y_test)
+        
+        # automatic carving of each feature
+        for n, feature in tqdm(enumerate(self.features), total=len(self.features), disable=self.verbose):
+
+            # printing the group statistics and determining default ordering
+            if self.verbose:
+                print(f"\n---\n[AutoCarver] Fit {feature} ({n+1}/{len(self.features)})")
+
+            # getting best combination
+            best_groups = self.get_best_combination(feature, Xc, y, Xtestc, y_test)
+
+            # feature can not be carved robustly
+            if not bool(best_groups):
+                self.non_viable_features += [feature]  # adding it to list of non viable features
+
+        # discretizing features based on each feature's values_order
+        super().__init__(self.values_orders, str_nan=self.str_nan, copy=self.copy, output=float)
+        super().fit(X, y)
+
+        return self
+
+
+    def get_best_combination(self, feature: str, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> Dict[str, Any]:
+        """ Carves a feature"""
+
+        # computing crosstabs
+        # crosstab on TRAIN
+        xtab = nan_crosstab(X[feature], y, self.str_nan)
+
+        # crosstab on TEST
+        xtab_test = None
+        if X_test is not None:
+            xtab_test = nan_crosstab(X_test[feature], y_test, self.str_nan)
+
+        # printing the group statistics
+        if self.verbose:
+            self.display_xtabs(feature, 'Raw', xtab, xtab_test)
+
+        # measuring association with target for each combination and testing for stability on TEST
+        best_groups = best_combination(self.values_orders.get(feature), self.max_n_mod, self.sort_by, xtab, xtab_test, dropna=True, str_nan=self.str_nan)
+
+        # update of the values_orders grouped modalities in values_orders
+        if best_groups:
+            xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
+
+        # testing adding NaNs to built groups
+        if (self.str_nan in xtab.index) & self.dropna & (self.str_nan not in self.values_orders.get(feature)):
+
+            # measuring association with target for each combination and testing for stability on TEST
+            best_groups = best_combination(self.values_orders.get(feature), self.max_n_mod, self.sort_by, xtab, xtab_test, dropna=False, str_nan=self.str_nan)
+
+            # adding NaN to the order
+            self.insert_nan(feature, xtab)
+
+            # update of the values_orders grouped modalities in values_orders
+            if best_groups:
+                xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
+
+        # printing the new group statistics
+        if self.verbose and best_groups:
+            self.display_xtabs(feature, 'Fitted', xtab, xtab_test)
+
+        return best_groups
+
+    def insert_nan(self, feature: str, xtab: DataFrame) -> GroupedList:
+        """ Inserts NaNs in the order"""
+
+        # accessing order for specified feature
+        order = self.values_orders.get(feature)
+
+        # adding nans at the end of the order
+        if self.str_nan not in order:
+            order = order.append(self.str_nan)
+
+            # updating values_orders
+            self.values_orders.update({feature: order})
+
+
+    def update_order(self, feature: str, best_groups: GroupedList, xtab: DataFrame, xtab_test: DataFrame=None) -> Tuple[DataFrame, DataFrame]:
+        """ Updates the values_orders and xtabs according to the best_groups"""
+
+        # updating values_orders with best_combination 
+        self.values_orders.update({feature: best_groups})
+
+        # update of the TRAIN crosstab
+        best_combi = list(map(best_groups.get_group, xtab.index))
+        xtab = xtab.groupby(best_combi, dropna=False).sum()
+
+        # update of the TEST crosstab
+        if xtab_test is not None:
+            best_combi = list(map(best_groups.get_group, xtab_test.index))
+            xtab_test = xtab_test.groupby(best_combi, dropna=False).sum()
+        
+        return xtab, xtab_test
+    
+    def display_xtabs(self, feature: str, caption: str, xtab: DataFrame, xtab_test: DataFrame=None) -> None:
+        """ Pretty display of frequency and target rate per modality on the same line. """
+        
+        # known_order per feature
+        known_order = self.values_orders.get(feature)
+        
+        # target rate and frequency on TRAIN
+        train_stats = stats_xtab(xtab, known_order)
+    
+        # target rate and frequency on TEST
+        if xtab_test is not None:
+            test_stats = stats_xtab(xtab_test, train_stats.index, train_stats.labels)
+            test_stats = test_stats.set_index('labels')  # setting labels as indices
+        
+        # setting TRAIN labels as indices
+        train_stats = train_stats.set_index('labels')
+
+        # Displaying TRAIN modality level stats
+        train_style = train_stats.style.background_gradient(cmap='coolwarm')  # color scaling
+        train_style = train_style.set_table_attributes("style='display:inline'")  # printing in notebook
+        train_style = train_style.set_caption(f'{caption} distribution on X:')  # title
+        html = train_style._repr_html_()
+        
+        # adding TEST modality level stats
+        if xtab_test is not None:
+            test_style = test_stats.style.background_gradient(cmap='coolwarm')  # color scaling
+            test_style = test_style.set_table_attributes("style='display:inline'")  # printing in notebook
+            test_style = test_style.set_caption(f'{caption} distribution on X_test:')  # title
+            html += ' ' + test_style._repr_html_()
+
+        # displaying html of colored DataFrame
+        display_html(html, raw=True)
+
+def groupedlist_combination(combination: List[List[Any]], order: GroupedList) -> GroupedList:
+    """ Converts a list of combination to a GroupedList"""
+    
+    order_copy = GroupedList(order)
+    for combi in combination:
+        order_copy.group_list(combi, combi[0])
+    
+    return order_copy
+
+def stats_xtab(xtab: DataFrame, known_order: List[Any]=None, known_labels: List[Any]=None) -> DataFrame:
+    """ Computes column (target) rate per row (modality) and row frequency"""
+    
+    # target rate and frequency statistics per modality
+    stats = DataFrame({
+        # target rate per modality
+        'target_rate': xtab[1].divide(xtab.sum(axis=1)),
+        # frequency per modality
+        'frequency': xtab.sum(axis=1) / xtab.sum().sum()
+    })
+    
+    # sorting statistics
+    # case 0: default ordering based on observed target rate
+    if known_order is None:
+        order = list(stats.sort_values('target_rate', ascending=True).index)
+    
+    # case 1: a known_order was provided
+    else:
+        order = known_order[:]
+      
+    # modalities' labels
+    # case 0: default labels
+    if known_labels is None:
+        
+        # accessing string representation of the GroupedList
+        if isinstance(known_order, GroupedList):
+            labels = known_order.get_repr()
+
+        # labels are the default order
+        else:
+            labels = order[:]
+            
+    # case 1: known_labels were provided
+    else:
+        labels = known_labels[:]
+            
+            
+    # keeping values missing from the order at the end
+    unknown_modality = [mod for mod in xtab.index if mod not in order]
+    for mod in unknown_modality:
+        order = [c for c in order if not is_equal(c, mod)] + [mod]
+        labels = [c for c in labels if not is_equal(c, mod)] + [mod]
+    
+    # sorting statistics
+    stats = stats.reindex(order, fill_value=0)
+    stats['labels'] = labels
+    
+    return stats
+
+def apply_combination(xtab: DataFrame, combination: GroupedList) -> Dict[str, Any]:
+    """ applies a modality combination to a crosstab """
+
+    # initiating association dict
+    association = {'combination': combination}
+
+    # grouping modalities in the initial crosstab
+    groups = list(map(combination.get_group, xtab.index))
+    combi_xtab = xtab.groupby(groups, dropna=False).sum()
+    association.update({'combi_xtab': combi_xtab})
+
+    # measuring association with the target
+    association.update(association_xtab(combi_xtab))
+
+    return association
+
+def best_combination(order: GroupedList, max_n_mod: int, sort_by: str, xtab_train: DataFrame, xtab_dev: DataFrame=None, dropna: bool=True, str_nan: str=None):
+    """ Finds the best combination of groups of feature's values:
+     - Most associated combination on train sample 
+     - Stable target rate of combination on test sample.
+    """
+    
+    # copying crosstabs
+    xtab = xtab_train
+    xtab_test = xtab_dev
+    
+    # removing nans if requested
+    if dropna:
+        
+        # crosstab on TRAIN
+        xtab = xtab_train[xtab_train.index != str_nan]  # filtering out nans
+
+        # crosstab on TEST
+        if xtab_test is not None:
+            xtab_test = xtab_dev[xtab_dev.index != str_nan]  # filtering out nans
+    
+        # getting all possible combinations for the feature without NaNS
+        combinations = get_all_combinations(order, max_n_mod, raw=False)
+    
+    # keeping nans as a modality
+    else:
+    
+        # getting all possible combinations for the feature with NaNS
+        combinations = get_all_nan_combinations(order, str_nan, max_n_mod)
+
+    # computing association measure per combination 
+    associations = [apply_combination(xtab, combi) for combi in combinations]
+
+    # sort according to association measure
+    if len(combinations) > 0:
+        associations = DataFrame(associations)
+        associations.sort_values(sort_by, inplace=True, ascending=False)
+        associations = associations.to_dict(orient='records')
+
+    # testing associations
+    # case 0: no test set was provided
+    if xtab_test is None and len(associations) > 0:
+        return associations[0]
+    
+    # case 1: testing viability on provided TEST sample
+    else:
+        for association in associations:
+            
+            # needed parameters
+            combination, combi_xtab = association['combination'], association['combi_xtab']
+
+            # grouping modalities in the initial crosstab
+            combi_xtab_test = xtab_test.groupby(list(map(combination.get_group, xtab_test.index)), dropna=False).sum()
+
+            # checking that all non-nan groups are in TRAIN and TEST
+            unq_x =  [v for v in unique(combi_xtab.index) if v != notna(v)]
+            unq_xtest = [v for v in unique(combi_xtab_test.index) if v != notna(v)]
+            viability = all([e in unq_x for e in unq_xtest])
+            viability = viability and all([e in unq_xtest for e in unq_x])
+
+            # same target rate order in TRAIN and TEST
+            train_target_rate = combi_xtab[1].divide(combi_xtab[0]).sort_values()
+            test_target_rate = combi_xtab_test[1].divide(combi_xtab_test[0]).sort_values()
+            viability = viability and all(train_target_rate.index == test_target_rate.index)
+
+            # checking that some combinations were provided
+            if viability:
+
+                association.update({'combi_xtab_test': combi_xtab_test})
+
+                return association
+
+
+def get_all_combinations(values: GroupedList, max_n_mod: int=None, raw: bool=False) -> List[GroupedList]:
+
+    # maximum number of classes
+    q = len(values)
+
+    # desired max number of classes
+    if max_n_mod is None:
+        max_n_mod = q
+
+    # all possible combinations
+    combinations = list()
+    for n_class in range(2, max_n_mod + 1):
+        combinations += get_combinations(n_class, q)
+
+    # getting real feature values
+    combinations = [[values[int(c[0]): int(c[1]) + 1] for c in combi] for combi in combinations]
+    
+    # converting back to GroupedList
+    if not raw:
+        combinations = [groupedlist_combination(combination, values) for combination in combinations]
+
+    return combinations
+
+def get_all_nan_combinations(order: GroupedList, str_nan: str, max_n_mod: int) -> List[GroupedList]:
+    """ all possible combinations of modalities with numpy.nan"""
+    
+    # computing all non-NaN combinations
+    # case 0: several modalities -> several combinations
+    if len(order) > 1:
+        combinations = get_all_combinations(order, max_n_mod-1, raw=True)
+    # case 1: unique or no modality -> two combinations
+    else:
+        combinations = []
+
+    # iterating over each combinations of non-NaNs
+    new_combinations = []
+    for combi in combinations:
+
+         # NaNs not attributed to a group (own modality)
+        new_combinations += [combi + [[str_nan]]] 
+
+        # NaNs attributed to a group of non NaNs
+        for n in range(len(combi)):
+
+            # grouping NaNs with an existing group
+            new_combination = [combi[n] + [str_nan]]
+
+            # adding other groups unchanged
+            pre = [o for o in combi[:n]]
+            nex = [o for o in combi[n+1:]]
+            new_combinations += [pre + new_combination + nex]
+            
+    # adding NaN to order
+    if str_nan not in order:
+        order = order.append(str_nan)
+    
+    # converting back to GroupedList
+    new_combinations = [groupedlist_combination(combination, order) for combination in new_combinations] 
+
+    return new_combinations
+
+
+def consecutive_combinations(n_remaining: int, start: int, end: int, grp_for_this_step: list=None):
+    """HELPER finds all consecutive combinations between start and end.    """
+
+    # Import de la liste globale
+    global __li_of_res__
+
+    # initiating group
+    if not grp_for_this_step:
+        grp_for_this_step = []
+    
+    # stopping when there are non more remaining classes
+    if n_remaining == 0:
+        
+        ### On ajoute le dernier quantile restant au découpage ###
+        grp_for_this_step += [(start, end)]
+
+        ### Ajout du découpage réalisé au groupe des solutions ###
+        __li_of_res__ += [grp_for_this_step]
+
+    
+    # adding all possible combinations of each possible range
+    else:
+        
+        ### Parcours de toutes les valeurs possibles de fin pour le i-ème groupe du groupement à x quantiles ###
+        for i in range(start, end):
+
+            consecutive_combinations(n_remaining-1, i+1, end, grp_for_this_step + [(start, i)])
+            
+def get_combinations(n_class, q):
+    """HELPER recupération des combinaisons possibles de q quantiles pour n_class."""
+    
+    globals()['__li_of_res__'] = []
+
+    consecutive_combinations(n_class-1, 0, q-1)
+    
+    combinations = [list(map(lambda u: (str(u[0]).zfill(len(str(q-1))), str(u[1]).zfill(len(str(q-1)))), l)) for l in __li_of_res__]
+    
+    return combinations
+
+def association_xtab(xtab: DataFrame):
+    """ Computes measures of association between feature x and feature2. """
+
+    # numnber of observations
+    n_obs = xtab.sum().sum()
+
+    # number of values taken by the features
+    n_mod_x, n_mod_y = len(xtab.index), len(xtab.columns)
+    min_n_mod = min(n_mod_x, n_mod_y)
+
+    # Chi2 statistic
+    chi2 = chi2_contingency(xtab)[0]
+
+    # Cramer's V
+    cramerv = 0
+    if min_n_mod > 1:
+        cramerv = sqrt(chi2 / n_obs / (min_n_mod - 1))
+
+    # Tschuprow's T
+    dof_mods = sqrt((n_mod_x - 1) * (n_mod_y - 1))
+    tschuprowt = 0
+    if dof_mods > 0:
+        tschuprowt = sqrt(chi2 / n_obs / dof_mods)
+
+    results = {'cramerv': cramerv, 'tschuprowt': tschuprowt}
+    
+    return results
+
+def nan_crosstab(x: Series, y: Series, str_nan: str='__NAN__'):
+    """ Crosstab that keeps nans as a specific value"""
+    
+    # keeping NaNs as a specific modality
+    x_filled = x.fillna(str_nan)  # filling NaNs
+
+    # computing initial crosstabs
+    xtab = crosstab(x_filled, y)
+    
+    return xtab
+
+
+def plot_stats(stats):
+    """ Barplot of the volume and target rate"""
+    
+    x = [0] + [elt for e in stats['frequency'].cumsum()[:-1] for elt in [e] * 2] + [1]
+    y2 = [elt for e in list(stats['target_rate']) for elt in [e]*2]
+    s = list(stats.index)
+    scaled_y2 = [(y-min(y2)) / (max(y2) - min(y2)) for y in y2]
+    c = color_palette("coolwarm", as_cmap=True)(scaled_y2)
+
+    fig, ax = subplots()
+
+    for i in range(len(stats)):
+        k = i*2
+        ax.fill_between(x[k: k+2], [0, 0], y2[k: k+2], color=c[k])
+        ax.text(sum(x[k: k+2]) / 2, y2[k], s[i], rotation=90, ha='center', va='bottom')
+
+    ax.xaxis.set_major_formatter(PercentFormatter(xmax=1))    
+    ax.yaxis.set_major_formatter(PercentFormatter(xmax=1))    
+    ax.set_xlabel('Volume')
+    ax.set_ylabel('Target rate')
+    ax.set_xlim(0, 1)
+    ax.set_ylim(0)
+    despine()
+    
+    return fig, ax
```

### Comparing `AutoCarver-4.3.2/AutoCarver/Converters.py` & `AutoCarver-4.4.0/AutoCarver/Converters.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,286 +1,286 @@
-from numpy import select, nan, tanh
-from pandas import isna, notna, DataFrame, Series, to_datetime
-from sklearn.base import BaseEstimator, TransformerMixin
-from typing import List, Tuple, Any, Dict
-
-
-class StringConverter(BaseEstimator, TransformerMixin):
-    """ Converts specified columns a DataFrame into str
-    
-     - Keeps NaN inplace
-     - Converts floats of int to int
-
-    Parameters
-    ----------
-    features: list, default []
-        List of columns to be converted to string.
-    """
-    
-    def __init__(self, features: List[str]=[], copy: bool=False) -> None:
-    
-        self.features = features[:]
-        self.copy = copy
-        
-    def fit(self, X: DataFrame, y: Series=None):
-        
-        return self
-        
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
-        # copying DataFrame if requested
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-
-        # storing nans
-        nans = isna(Xc[self.features])
-
-        # storing ints
-        ints = Xc[self.features].applymap(lambda u: isinstance(u, float) and float.is_integer(u))
-        
-        # converting to string
-        Xc[self.features] = Xc[self.features].astype(str)
-        
-        # converting to int-strings
-        converted_ints = Xc[ints][self.features].applymap(lambda u: str(int(float(u))) if isinstance(u, str) else u)
-        Xc[self.features] = select([ints], [converted_ints], default=Xc[self.features])
-        
-        # converting back to nan
-        Xc[nans] = nan
-        
-        return Xc
-
-
-class TimeDeltaConverter(BaseEstimator, TransformerMixin):
-    """ Converts specified DateTime columns into TimeDeltas between themselves
-
-     - Str Columns are converted to pandas datetime columns
-     - New TimeDelta column names are stored in TimeDeltaConverter.delta_features
-
-    Parameters
-    ----------
-    features: List[str]
-        List of DateTime columns to be converted to string.
-    nans: Any, default numpy.nan
-        Date value to be considered as missing data.
-    drop: bool, default True
-        Whether or not to drop initial DateTime columns (specified in features).
-    """
-    
-    def __init__(self, features: List[str], nans: Any=nan, copy: bool=False, drop: bool=True) -> None:
-        
-        self.features = features[:]
-        self.copy = copy
-        self.new_features: List[str] = []
-        self.nans = nans
-        self.drop = drop
-        
-    def fit(self, X: DataFrame, y=None) -> None:
-        
-        # creating list of names of delta featuers
-        for i, date1 in enumerate(self.features):
-            for date2 in self.features[i+1:]:
-                self.new_features += [f'delta_{date1}_{date2}']
-        
-        return self
-    
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
-        # copying dataset
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-            
-        # converting back nans
-        if notna(self.nans):
-            Xc[self.features] = Xc[self.features].where(Xc[self.features]!=self.nans, nan)
-        
-        # converting to datetime
-        Xc[self.features] = to_datetime(Xc[self.features].stack()).unstack()
-        
-        # iterating over each combination of dates
-        for i, date1 in enumerate(self.features):
-            for date2 in self.features[i+1:]:
-                
-                # computing timedelta of days
-                Xc[f'delta_{date1}_{date2}'] = (Xc[date1] - Xc[date2]).dt.days
-        
-        # dropping date columns
-        Xc = Xc.drop(self.features, axis=1)
-        
-        return Xc
-
-class GroupNormalizer(BaseEstimator, TransformerMixin):
-    """ Normalizes a feature's values based on specified means and stds per groups' values
-
-    Parameters
-    ----------
-    groups: List[str]
-        List of qualitative features used to compute feature's mean/std per there modalities.
-    features: List[str]
-        List of quantitative features to be normalized.
-    """
-
-    def __init__(self, groups: List[str], features: List[str], copy: bool=True) -> None:
-        
-        self.features = features[:]
-        self.groups = groups[:]
-        
-        self.copy = copy
-        
-        self.group_means = dict()
-        self.group_stds = dict()
-        
-        self.new_features = list()
-
-    def fit(self, X: DataFrame, y: Series=None) -> None:
-        
-        # iterating over each grouping column
-        for group in self.groups:
-            
-            # computing group mean
-            self.group_means.update({group: X.groupby(group)[self.features].mean().to_dict()})
-            
-            # computing group std
-            self.group_stds.update({group: X.groupby(group)[self.features].std().to_dict()})
-            
-            # adding built features
-            self.new_features += [f"{f}_norm_{group}" for f in self.features]
-
-        return self
-
-    
-
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
-        # coppying dataframe
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-        
-        # iterating over each group
-        for group in self.groups:
-            
-            # computing observation level mean
-            means = Xc[self.features].apply(lambda u: Xc[group].apply(self.group_means[group][u.name].get))
-
-            # computing observation level std
-            stds = Xc[self.features].apply(lambda u: Xc[group].apply(self.group_stds[group][u.name].get))
-            
-            # applying normalization to the feature
-            Xc = Xc.join(
-                Xc[self.features].sub(means)\
-                                 .replace(0, nan)\
-                                 .divide(stds)\
-                                 .rename({f: f"{f}_norm_{group}" for f in self.features}, axis=1)
-            )
-
-        del means
-        del stds
-        
-        return Xc
-
-class TanhNormalizer(BaseEstimator, TransformerMixin):
-    """ Tanh Normalization that keeps data distribution and borns between 0 and 1
-
-    Parameters
-    ----------
-    features: List[str]
-        List of quantitative features to be normalized.
-    """
-    
-    def __init__(self, features: List[str], copy: bool=False) -> None:
-        
-        self.features = features[:]
-        self.copy = copy
-        
-    def fit(self, X: DataFrame, y=None) -> None:
-        
-        self.distribs = X[self.features].agg(['mean', 'std']).to_dict(orient='index')
-        
-        return self
-    
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
-        # copying dataset
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-        
-        # applying tanh normalization
-        Xc[self.features] = (tanh(Xc[self.features].sub(self.distribs['mean']).divide(self.distribs['std']) * 0.01) + 1 ) / 2
-        
-        return Xc
-
-class CrossConverter(BaseEstimator, TransformerMixin):
-    """ Normalizes a feature's values based on specified means and stds per groups' values
-
-    Parameters
-    ----------
-    features: List[str]
-        List of qualitative features to be crossed should be passed through AutoCarver early on.
-    """
-
-    def __init__(self, features: List[str], copy: bool=True) -> None:
-        
-        self.features = features[:]
-        self.copy = copy
-        self.new_features: List[str] = list()
-        self.values: Dict[str, List[Any]] = dict()
-
-    def fit(self, X: DataFrame, y: Series=None) -> None:
-        
-        # iterating over each feature
-        for i, feature1 in enumerate(self.features):
-            
-            # unique values of feature1
-            unq1 = X[feature1].astype(str).unique()
-            
-            for feature2 in self.features[i+1:]:
-            
-                # adding features names to the list of built features
-                self.new_features += [f'{feature2}_x_{feature1}']
-            
-                # unique values of feature2
-                unq2 = X[feature2].astype(str).unique()
-                
-                self.values.update({
-                    f'{feature2}_x_{feature1}': [u2 + '_x_' + u1 for u2 in unq2 for u1 in unq1]
-                })
-
-        return self
-
-    
-
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
-        # coppying dataframe
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-            
-        # converting features to strings
-        Xc_features = Xc[self.features].astype(str)
-        
-        # iterating over each group
-        for i, feature in enumerate(self.features):
-            
-            # features to cross with
-            Xc_tocross = Xc_features[self.features[i+1:]]
-            
-            # feature to be crossed
-            Xc_crosser = Xc_features[feature]
-
-            # crossing features
-            Xc_crossed = Xc_tocross.apply(lambda u: u + '_x_' + Xc_crosser)\
-                                   .rename({f: f"{f}_x_{feature}" for f in self.features[i+1:]}, axis=1)
-            
-            # applying normalization to the feature
-            Xc = Xc.join(Xc_crossed)
-        
-        del Xc_features
-        del Xc_crossed
-        del Xc_tocross
-        del Xc_crosser
-        
+from numpy import select, nan, tanh
+from pandas import isna, notna, DataFrame, Series, to_datetime
+from sklearn.base import BaseEstimator, TransformerMixin
+from typing import List, Tuple, Any, Dict
+
+
+class StringConverter(BaseEstimator, TransformerMixin):
+    """ Converts specified columns a DataFrame into str
+    
+     - Keeps NaN inplace
+     - Converts floats of int to int
+
+    Parameters
+    ----------
+    features: list, default []
+        List of columns to be converted to string.
+    """
+    
+    def __init__(self, features: List[str]=[], copy: bool=False) -> None:
+    
+        self.features = features[:]
+        self.copy = copy
+        
+    def fit(self, X: DataFrame, y: Series=None):
+        
+        return self
+        
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        
+        # copying DataFrame if requested
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+
+        # storing nans
+        nans = isna(Xc[self.features])
+
+        # storing ints
+        ints = Xc[self.features].applymap(lambda u: isinstance(u, float) and float.is_integer(u))
+        
+        # converting to string
+        Xc[self.features] = Xc[self.features].astype(str)
+        
+        # converting to int-strings
+        converted_ints = Xc[ints][self.features].applymap(lambda u: str(int(float(u))) if isinstance(u, str) else u)
+        Xc[self.features] = select([ints], [converted_ints], default=Xc[self.features])
+        
+        # converting back to nan
+        Xc[nans] = nan
+        
+        return Xc
+
+
+class TimeDeltaConverter(BaseEstimator, TransformerMixin):
+    """ Converts specified DateTime columns into TimeDeltas between themselves
+
+     - Str Columns are converted to pandas datetime columns
+     - New TimeDelta column names are stored in TimeDeltaConverter.delta_features
+
+    Parameters
+    ----------
+    features: List[str]
+        List of DateTime columns to be converted to string.
+    nans: Any, default numpy.nan
+        Date value to be considered as missing data.
+    drop: bool, default True
+        Whether or not to drop initial DateTime columns (specified in features).
+    """
+    
+    def __init__(self, features: List[str], nans: Any=nan, copy: bool=False, drop: bool=True) -> None:
+        
+        self.features = features[:]
+        self.copy = copy
+        self.new_features: List[str] = []
+        self.nans = nans
+        self.drop = drop
+        
+    def fit(self, X: DataFrame, y=None) -> None:
+        
+        # creating list of names of delta featuers
+        for i, date1 in enumerate(self.features):
+            for date2 in self.features[i+1:]:
+                self.new_features += [f'delta_{date1}_{date2}']
+        
+        return self
+    
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        
+        # copying dataset
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+            
+        # converting back nans
+        if notna(self.nans):
+            Xc[self.features] = Xc[self.features].where(Xc[self.features]!=self.nans, nan)
+        
+        # converting to datetime
+        Xc[self.features] = to_datetime(Xc[self.features].stack()).unstack()
+        
+        # iterating over each combination of dates
+        for i, date1 in enumerate(self.features):
+            for date2 in self.features[i+1:]:
+                
+                # computing timedelta of days
+                Xc[f'delta_{date1}_{date2}'] = (Xc[date1] - Xc[date2]).dt.days
+        
+        # dropping date columns
+        Xc = Xc.drop(self.features, axis=1)
+        
+        return Xc
+
+class GroupNormalizer(BaseEstimator, TransformerMixin):
+    """ Normalizes a feature's values based on specified means and stds per groups' values
+
+    Parameters
+    ----------
+    groups: List[str]
+        List of qualitative features used to compute feature's mean/std per there modalities.
+    features: List[str]
+        List of quantitative features to be normalized.
+    """
+
+    def __init__(self, groups: List[str], features: List[str], copy: bool=True) -> None:
+        
+        self.features = features[:]
+        self.groups = groups[:]
+        
+        self.copy = copy
+        
+        self.group_means = dict()
+        self.group_stds = dict()
+        
+        self.new_features = list()
+
+    def fit(self, X: DataFrame, y: Series=None) -> None:
+        
+        # iterating over each grouping column
+        for group in self.groups:
+            
+            # computing group mean
+            self.group_means.update({group: X.groupby(group)[self.features].mean().to_dict()})
+            
+            # computing group std
+            self.group_stds.update({group: X.groupby(group)[self.features].std().to_dict()})
+            
+            # adding built features
+            self.new_features += [f"{f}_norm_{group}" for f in self.features]
+
+        return self
+
+    
+
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        
+        # coppying dataframe
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+        
+        # iterating over each group
+        for group in self.groups:
+            
+            # computing observation level mean
+            means = Xc[self.features].apply(lambda u: Xc[group].apply(self.group_means[group][u.name].get))
+
+            # computing observation level std
+            stds = Xc[self.features].apply(lambda u: Xc[group].apply(self.group_stds[group][u.name].get))
+            
+            # applying normalization to the feature
+            Xc = Xc.join(
+                Xc[self.features].sub(means)\
+                                 .replace(0, nan)\
+                                 .divide(stds)\
+                                 .rename({f: f"{f}_norm_{group}" for f in self.features}, axis=1)
+            )
+
+        del means
+        del stds
+        
+        return Xc
+
+class TanhNormalizer(BaseEstimator, TransformerMixin):
+    """ Tanh Normalization that keeps data distribution and borns between 0 and 1
+
+    Parameters
+    ----------
+    features: List[str]
+        List of quantitative features to be normalized.
+    """
+    
+    def __init__(self, features: List[str], copy: bool=False) -> None:
+        
+        self.features = features[:]
+        self.copy = copy
+        
+    def fit(self, X: DataFrame, y=None) -> None:
+        
+        self.distribs = X[self.features].agg(['mean', 'std']).to_dict(orient='index')
+        
+        return self
+    
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        
+        # copying dataset
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+        
+        # applying tanh normalization
+        Xc[self.features] = (tanh(Xc[self.features].sub(self.distribs['mean']).divide(self.distribs['std']) * 0.01) + 1 ) / 2
+        
+        return Xc
+
+class CrossConverter(BaseEstimator, TransformerMixin):
+    """ Normalizes a feature's values based on specified means and stds per groups' values
+
+    Parameters
+    ----------
+    features: List[str]
+        List of qualitative features to be crossed should be passed through AutoCarver early on.
+    """
+
+    def __init__(self, features: List[str], copy: bool=True) -> None:
+        
+        self.features = features[:]
+        self.copy = copy
+        self.new_features: List[str] = list()
+        self.values: Dict[str, List[Any]] = dict()
+
+    def fit(self, X: DataFrame, y: Series=None) -> None:
+        
+        # iterating over each feature
+        for i, feature1 in enumerate(self.features):
+            
+            # unique values of feature1
+            unq1 = X[feature1].astype(str).unique()
+            
+            for feature2 in self.features[i+1:]:
+            
+                # adding features names to the list of built features
+                self.new_features += [f'{feature2}_x_{feature1}']
+            
+                # unique values of feature2
+                unq2 = X[feature2].astype(str).unique()
+                
+                self.values.update({
+                    f'{feature2}_x_{feature1}': [u2 + '_x_' + u1 for u2 in unq2 for u1 in unq1]
+                })
+
+        return self
+
+    
+
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        
+        # coppying dataframe
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+            
+        # converting features to strings
+        Xc_features = Xc[self.features].astype(str)
+        
+        # iterating over each group
+        for i, feature in enumerate(self.features):
+            
+            # features to cross with
+            Xc_tocross = Xc_features[self.features[i+1:]]
+            
+            # feature to be crossed
+            Xc_crosser = Xc_features[feature]
+
+            # crossing features
+            Xc_crossed = Xc_tocross.apply(lambda u: u + '_x_' + Xc_crosser)\
+                                   .rename({f: f"{f}_x_{feature}" for f in self.features[i+1:]}, axis=1)
+            
+            # applying normalization to the feature
+            Xc = Xc.join(Xc_crossed)
+        
+        del Xc_features
+        del Xc_crossed
+        del Xc_tocross
+        del Xc_crosser
+        
         return Xc
```

### Comparing `AutoCarver-4.3.2/AutoCarver/Discretizers.py` & `AutoCarver-4.4.0/AutoCarver/Discretizers.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,1248 +1,1248 @@
-from IPython.display import display_html
-from numpy import sort, nan, inf, float32, where, isin, argsort, array, select, append, quantile, linspace, argmin
-from pandas import DataFrame, Series, isna, qcut, notna, unique
-from pandas.api.types import is_numeric_dtype, is_string_dtype
-from sklearn.base import BaseEstimator, TransformerMixin
-from typing import Any, Dict, List
-from warnings import warn
-
-def nan_unique(x: Series):
-    """ Unique non-NaN values. """
-    
-    # unique values
-    uniques = unique(x)
-    
-    # filtering out nans
-    uniques = [u for u in uniques if notna(u)]
-    
-    return uniques
-
-class GroupedList(list):
-    
-    def __init__(self, iterable=()) -> None:
-        """ An ordered list that historizes its elements' merges."""
-
-        # case 0: iterable is the contained dict
-        if isinstance(iterable, dict):
-            # TODO: check thaht keys are in list
-            
-            # récupération des valeurs de la liste (déjà ordonné)
-            values = [key for key in iterable]
-
-            # initialsiation de la liste
-            super().__init__(values)
-
-            # attribution des valeurs contenues
-            self.contained = {k: v for k, v in iterable.items()}
-
-            # adding key to itself if that's not the case
-            for k in [k for k in values if k not in self.contained.get(k)]:
-                self.contained.update({k: self.contained.get(k) + [k]})
-        
-        # case 1: copying a GroupedList
-        elif hasattr(iterable, 'contained'):
-
-            # initialsiation de la liste
-            super().__init__(iterable)
-
-            # copie des groupes
-            self.contained = {k: v for k, v in iterable.contained.items()}
-        
-        # case 2: initiating GroupedList from a list
-        elif isinstance(iterable, list):
-
-            # initialsiation de la liste
-            super().__init__(iterable)
-
-            # création des groupes
-            self.contained = {v: [v] for v in iterable}
-
-    def group_list(self, to_discard: List[Any], to_keep: Any) -> None:
-        """ Groups elements to_discard into values to_keep"""
-        
-        for discarded, kept in zip(to_discard, [to_keep] * len(to_discard)):
-            self.group(discarded, kept)
-
-    def group(self, discarded: Any, kept: Any) -> None:
-        """ Groups the discarded value with the kept value"""
-
-        # checking that those values are distinct
-        if not is_equal(discarded, kept):
-
-            # checking that those values exist in the list
-            assert discarded in self, f"{discarded} not in list"
-            assert kept in self, f"{kept} not in list"
-
-            # accessing values contained in each value
-            contained_discarded = self.contained.get(discarded)
-            contained_kept = self.contained.get(kept)
-
-            # updating contained dict
-            self.contained.update({
-                kept: contained_discarded + contained_kept,
-                discarded: []
-            })
-
-            # removing discarded from the list
-            self.remove(discarded)
-        
-        return self
-        
-    def append(self, new_value: Any) -> None:
-        """ Appends a new_value to the GroupedList"""
-        
-        self += [new_value]
-        
-        self.contained.update({new_value: [new_value]})
-        
-        return self
-        
-    def update(self, new_value: Dict[Any, List[Any]]) -> None:
-        """ Updates the GroupedList via a dict"""
-        
-        # adding keys to the order if they are new values
-        for k in [c for c in new_value if c not in self]:
-            self += new_value.keys()
-        
-        # updating contained accord to new_value
-        self.contained.update(new_value)
-        
-        return self
-
-    def sort(self) -> None:
-        """ Sorts the values of the list and dict (if any, NaNs are last). """
-
-        # str values
-        keys_str = [key for key in self if isinstance(key, str)]
-
-        # non-str values
-        keys_float = [key for key in self if not isinstance(key, str)]
-
-        # sorting and merging keys
-        keys = list(sort(keys_str)) + list(sort(keys_float)) 
-
-        # recreating an ordered GroupedList
-        self = GroupedList({k: self.get(k) for k in keys})
-
-        return self
-
-    def sort_by(self, ordering: List[Any]) -> None:
-        """ Sorts the values of the list and dict, if any, NaNs are the last. """
-
-        # checking that all values are given an order
-        assert all([o in self for o in ordering]), f"Unknown values in ordering: {', '.join([str(v) for v in ordering if v not in self])}"
-        assert all([s in ordering for s in self]), f"Missing value from ordering: {', '.join([str(v) for v in self if v not in ordering])}"
-
-        # ordering the contained
-        self = GroupedList({k: self.get(k) for k in ordering})
-
-        return self
-
-    
-    def remove(self, value: Any) -> None:
-        
-        super().remove(value)
-        self.contained.pop(value)
-    
-    def pop(self, idx: int) -> None:
-        
-        value = self[idx]
-        self.remove(value)
-    
-    def get(self, key: Any) -> List[Any]:
-        """ returns list of values contained in key"""
-
-        # default to fing an element
-        found = self.contained.get(key)
-
-        # copying with dictionnaries (not working with numpy.nan)
-        # if isna(key):
-            # found = [value for dict_key, value in self.contained.items() if is_equal(dict_key, key)][0]
-
-        return found
-
-    def get_group(self, value: Any) -> Any:
-        """ returns the group containing the specified value """
-        
-        found = [key for key, values in self.contained.items() if any(is_equal(value, elt) for elt in values)]
-
-        if any(found):
-            return found[0]
-        else:
-            return value
-
-    def values(self) -> List[Any]:
-        """ returns all values contained in each group """
-
-        known = [value for values in self.contained.values() for value in values]
-
-        return known
-
-    def contains(self, value: Any) -> bool:
-        """ checks if a value if contained in any group """
-
-        known_values = self.values()
-
-        return any(is_equal(value, known) for known in known_values)
-
-    def get_repr(self, char_limit: int=10) -> List[str]:
-        """" Returns a representative list of strings of values of groups. """
-
-        # initiating list of group representation
-        repr: List[str] = []
-
-        # iterating over each group
-        for group in self:
-
-            # accessing group's values
-            values = self.get(group)
-
-            if len(values) == 0:  # case 0: there are no value in this group
-                pass
-            
-            elif len(values) == 1:  # case 1: there is only one value in this group
-                repr += [values[0]]
-            
-            elif len(values) == 2:  # case 2: two values in this group
-                repr += [f'{values[1]}'[:char_limit]+' and '+f'{values[0]}'[:char_limit]]
-            
-            elif len(values) > 2:  # case 3: more than two values in this group
-                repr += [f'{values[-1]}'[:char_limit]+' to '+f'{values[0]}'[:char_limit]]
-                
-        return repr
-
-
-class GroupedListDiscretizer(BaseEstimator, TransformerMixin):
-    
-    def __init__(self, values_orders: Dict[str, Any], *, 
-        copy: bool=False, output: type= float,
-        str_nan: str=None, verbose: bool=False) -> None:
-        
-        self.features = list(values_orders.keys())
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.copy = copy
-        self.output = output
-        self.verbose = verbose
-        self.str_nan = str_nan
-        
-    def fit(self, X, y=None) -> None:
-
-        return self
-    
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-
-        # copying dataframes
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-
-        # filling up nans with specified value
-        if self.str_nan:
-            Xc[self.features] = Xc[self.features].fillna(self.str_nan)
-
-        # iterating over each feature
-        for n, feature in enumerate(self.features):
-            
-            # verbose if requested
-            if self.verbose: 
-                print(f" - [GroupedListDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
-            
-            # bucketizing feature
-            order = self.values_orders.get(feature)  # récupération des groupes
-            to_discard = [order.get(group) for group in order]  # identification des valeur à regrouper
-            to_input = [Xc[feature].isin(discarded) for discarded in to_discard]  # identifying main bucket value
-            to_keep = [n if self.output == float else group for n, group in enumerate(order)]  # récupération du groupe dans lequel regrouper
-
-            # case when there are no values
-            if len(to_input)==0 & len(to_keep)==0:
-                pass
-
-            # grouping modalities
-            else:
-                Xc[feature] = select(to_input, to_keep, default=Xc[feature])
-
-        # converting to float
-        if self.output == float:
-            Xc[self.features] = Xc[self.features].astype(float32)
-
-        return Xc
-
-
-class QualitativeDiscretizer(BaseEstimator, TransformerMixin):
-    """ Automatic discretizing of categorical and categorical ordinal features.
-
-    Modalities/values of features are grouped according to there respective orders:
-     - [Qualitative features] order based on modality target rate.
-     - [Qualitative ordinal features] user-specified order.
-
-    TODO: pass ordinal_features/qualitati_features as parameters to be able to pass values_orders with other orders (ex: from chaineddiscretizer)
-
-    Parameters
-    ----------
-    features: list
-        Contains qualitative (categorical and categorical ordinal) features to be discretized.
-
-    min_freq: int
-        [Qualitative features] Minimal frequency of a modality.
-         - NaNs are considered a specific modality but will not be grouped.
-         - [Qualitative features] Less frequent modalities are grouped in the `__OTHER__` modality.
-         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
-        (smallest frequency or closest target rate), between the superior and inferior values (specified
-        in the `values_orders` dictionnary).
-        Recommandation: `min_freq` should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
-
-    values_orders: dict, default {}
-        [Qualitative ordinal features] dict of features values and list of orders of their values.
-         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
-        (smallest frequency or closest target rate), between the superior and inferior values (described
-        by the `values_orders`).
-        Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
-    """
-    
-    def __init__(self, features: List[str], min_freq: float, *,
-                 values_orders: Dict[str, Any]={}, copy: bool=False, 
-                 verbose: bool=False) -> None:
-    
-        self.features = features[:]
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.ordinal_features = [f for f in values_orders if f in features]  # ignores non qualitative features
-        self.non_ordinal_features = [f for f in features if f not in self.ordinal_features]
-        self.min_freq = min_freq
-        self.pipe: List[BaseEstimator] = []
-        self.copy = copy
-        self.verbose = verbose
-        
-    def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
-        """ Checking data for bucketization"""
-        
-        # checking for quantitative columns
-        is_object = X[self.features].dtypes.apply(is_string_dtype)
-        assert all(is_object), f"Non-string features: {', '.join(is_object[~is_object].index)}, consider using Converters.StringConverter."
-        
-        # checking for binary target
-        y_values = unique(y)
-        assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
-        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
-        
-        # checking that all unique values in X are in values_orders
-        uniques = X[self.features].apply(nan_unique)
-        for feature in self.ordinal_features:
-            missing = [val for val in uniques[feature] if val not in self.values_orders[feature]]
-            assert len(missing)==0, f"The ordering for {', '.join(missing)} of feature '{feature}' must be specified in values_orders (str-only)."
-        
-        # copying dataframe
-        Xc = X.copy()
-        
-        return Xc
-
-    def fit(self, X: DataFrame, y: Series) -> None:
-        """ Learning TRAIN distribution"""
-        
-        # checking data before bucketization
-        Xc = self.prepare_data(X, y)
-
-        # [Qualitative ordinal features] Grouping rare values into closest common one
-        if len(self.ordinal_features) > 0:
-
-            # discretizing
-            ordinal_orders = {k: GroupedList(v) for k, v in self.values_orders.items() if k in self.ordinal_features}
-            discretizer = ClosestDiscretizer(
-                ordinal_orders, min_freq=self.min_freq, verbose=self.verbose
-            )
-            discretizer.fit(Xc, y)
-
-            # storing results
-            self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
-            self.pipe += [('QualitativeClosestDiscretizer', discretizer)]  # adding discretizer to pipe
-
-        # [Qualitative non-ordinal features] Grouping rare values into default_value '__OTHER__'
-        if len(self.non_ordinal_features) > 0:
-
-            # Grouping rare modalities
-            discretizer = DefaultDiscretizer(self.non_ordinal_features, min_freq=self.min_freq, 
-                                             values_orders=self.values_orders,
-                                             verbose=self.verbose)
-            discretizer.fit(Xc, y)
-
-            # storing results
-            self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
-            self.pipe += [('DefaultDiscretizer', discretizer)]  # adding discretizer to pipe
-
-        return self
-
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        """ Applying learned bucketization on TRAIN and/or TEST"""
-
-        # copying dataframe if requested
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-
-        # iterating over each transformer
-        for _, step in self.pipe:
-            Xc = step.transform(Xc)
-
-        return Xc
-
-class QuantitativeDiscretizer(BaseEstimator, TransformerMixin):
-    """ Automatic discretizing of continuous features.
-
-    Modalities/values of features are grouped according to there respective orders:
-     - [Quantitative features] real order of the values.
-
-    Parameters
-    ----------
-    features: list
-        Contains quantitative (continuous) features to be discretized.
-
-    q: int, default None
-        [Quantitative features] Number of quantiles to initialy cut the feature.
-         - NaNs are considered a specific value but will not be grouped.
-         - Values more frequent than `1/q` will be set as their own group and remaining frequency will be
-        cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
-        Exemple: if q=10 and the value numpy.nan represent 50 % of the observed values, non-NaNs will be 
-        cut in q=5 quantiles.
-        Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
-
-    """
-    
-    def __init__(self, features: List[str], q: int, *, values_orders: Dict[str, Any]={}, copy: bool=False, 
-                 verbose: bool=False) -> None:
-        
-        self.features = features[:]
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.q = q
-        self.pipe: List[BaseEstimator] = []
-        self.copy = copy
-        self.verbose = verbose
-    
-    def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
-        """ Checking data for bucketization"""
-        
-        # checking for quantitative columns
-        is_numeric = X[self.features].dtypes.apply(is_numeric_dtype)
-        assert all(is_numeric), f"Non-numeric features: {', '.join(is_numeric[~is_numeric].index)}"
-        
-        # checking for binary target
-        y_values = unique(y)
-        assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
-        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
-        
-        # copying dataframe
-        Xc = X.copy()
-        
-        return Xc
-
-    def fit(self, X: DataFrame, y: Series) -> None:
-        """ Learning TRAIN distribution"""
-        
-        # checking data before bucketization
-        Xc = self.prepare_data(X, y)
-
-        # [Quantitative features] Grouping values into quantiles
-        discretizer = QuantileDiscretizer(self.features, q=self.q, values_orders=self.values_orders, verbose=self.verbose)
-        Xc = discretizer.fit_transform(Xc, y)
-
-        # storing results
-        self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
-        self.pipe += [('QuantileDiscretizer', discretizer)]  # adding discretizer to pipe
-
-        # [Quantitative features] Grouping rare quantiles into closest common one
-        #  -> can exist because of overrepresented values (values more frequent than 1/q)
-        # searching for features with rare quantiles: computing min frequency per feature
-        frequencies = Xc[self.features].apply(lambda u: min_value_counts(u, self.values_orders[u.name]), axis=0)
-        
-        # minimal frequency of a quantile
-        q_min_freq = 1 / self.q / 2
-        
-        # identifying features that have rare modalities
-        has_rare = list(frequencies[frequencies <= q_min_freq].index)
-        
-        # Grouping rare modalities
-        if len(has_rare) > 0:
-            
-            # Grouping only features with rare modalities 
-            rare_values_orders = {feature: order for feature, order in self.values_orders.items() if feature in has_rare}
-            discretizer = ClosestDiscretizer(rare_values_orders, min_freq=q_min_freq, verbose=self.verbose)
-            discretizer.fit(Xc, y)
-
-            # storing results
-            self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
-            self.pipe += [('QuantitativeClosestDiscretizer', discretizer)]  # adding discretizer to pipe
-
-        return self
-
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        """ Applying learned bucketization on TRAIN and/or TEST"""
-
-        # copying dataframe if requested
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-
-        # iterating over each transformer
-        for _, step in self.pipe:
-            Xc = step.transform(Xc)
-
-        return Xc
-
-class Discretizer(BaseEstimator, TransformerMixin):
-    """ Automatic discretizing of continuous, categorical and categorical ordinal features.
-
-    Modalities/values of features are grouped according to there respective orders:
-     - [Qualitative features] order based on modality target rate.
-     - [Qualitative ordinal features] user-specified order.
-     - [Quantitative features] real order of the values.
-
-    Parameters
-    ----------
-    quanti_features: list
-        Contains quantitative (continuous) features to be discretized.
-
-    quali_features: list
-        Contains qualitative (categorical and categorical ordinal) features to be discretized.
-
-    min_freq: int, default None
-        [Qualitative features] Minimal frequency of a modality.
-         - NaNs are considered a specific modality but will not be grouped.
-         - [Qualitative features] Less frequent modalities are grouped in the `__OTHER__` modality.
-         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
-        (smallest frequency or closest target rate), between the superior and inferior values (specified
-        in the `values_orders` dictionnary).
-        Recommandation: `min_freq` should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
-
-    q: int, default None
-        [Quantitative features] Number of quantiles to initialy cut the feature.
-         - NaNs are considered a specific value but will not be grouped.
-         - Values more frequent than `1/q` will be set as their own group and remaining frequency will be
-        cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
-        Exemple: if q=10 and the value numpy.nan represent 50 % of the observed values, non-NaNs will be 
-        cut in q=5 quantiles.
-        Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
-
-    values_orders: dict, default {}
-        [Qualitative ordinal features] dict of features values and list of orders of their values.
-         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
-        (smallest frequency or closest target rate), between the superior and inferior values (described
-        by the `values_orders`).
-        Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
-    """
-
-    def __init__(self, quanti_features: List[str], quali_features: List[str], min_freq: float, *, 
-                 values_orders: Dict[str, Any]={}, copy: bool=False, verbose: bool=False) -> None:
-
-        self.features = quanti_features[:] + quali_features[:]
-        self.quanti_features = quanti_features[:]
-        assert len(list(set(quanti_features))) == len(quanti_features), "Column duplicates in quanti_features"
-        self.quali_features = quali_features[:]
-        assert len(list(set(quali_features))) == len(quali_features), "Column duplicates in quali_features"
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.min_freq = min_freq
-        self.q = int(1 / min_freq)  # number of quantiles
-        self.pipe: List[BaseEstimator] = []
-        self.copy = copy
-        self.verbose = verbose
-
-    def fit(self, X: DataFrame, y: Series) -> None:
-
-        # [Qualitative features] Grouping qualitative features
-        if len(self.quali_features) > 0:
-
-            # verbose if requested
-            if self.verbose:
-                print("\n---\n[Discretizer] Fit Qualitative Features")
-
-            # grouping qualitative features
-            discretizer = QualitativeDiscretizer(
-                self.quali_features, min_freq=self.min_freq,
-                values_orders=self.values_orders, copy=self.copy,
-                verbose=self.verbose
-            )
-            discretizer.fit(X, y)
-
-            # storing results
-            self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
-            self.pipe += discretizer.pipe  # adding discretizer to pipe
-
-        # [Quantitative features] Grouping quantitative features
-        if len(self.quanti_features) > 0:
-
-            # verbose if requested
-            if self.verbose:
-                print("\n---\n[Discretizer] Fit Quantitative Features")
-
-            # grouping quantitative features
-            discretizer = QuantitativeDiscretizer(
-                self.quanti_features, q=self.q,
-                values_orders=self.values_orders, copy=self.copy,
-                verbose=self.verbose
-            )
-            discretizer.fit(X, y)
-
-            # storing results
-            self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
-            self.pipe += discretizer.pipe  # adding discretizer to pipe
-
-        return self
-
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-
-        # verbose if requested
-        if self.verbose:
-            print("\n---\n[Discretizer] Transform Features")
-        
-        # copying dataframe if requested
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-
-        # iterating over each transformer
-        for _, step in self.pipe:
-            Xc = step.transform(Xc)
-
-        return Xc
-
-
-
-class ChainedDiscretizer(GroupedListDiscretizer):
-    
-    def __init__(self, features: List[str], min_freq: float, chained_orders: List[GroupedList], *, 
-                 remove_unknown: bool=False, str_nan: str='__NAN__', copy: bool=False, verbose: bool=False) -> None:       
-        
-        self.min_freq = min_freq
-        self.features = features[:]
-        self.chained_orders = [GroupedList(order) for order in chained_orders]
-        self.copy = copy
-        self.verbose = verbose
-
-        # parameters to handle missing/unknown values
-        self.remove_unknown = remove_unknown
-        self.str_nan = str_nan
-        
-        # initiating features' values orders to all possible values
-        self.known_values = list(set([v for o in self.chained_orders for v in o.values()]))
-        self.values_orders = {f: GroupedList(self.known_values[:] + [self.str_nan]) for f in self.features}
-
-    def fit(self, X: DataFrame, y: Series=None) -> None:
-        
-        # filling nans
-        Xc = X[self.features].fillna(self.str_nan)
-        
-        # iterating over each feature
-        for n, feature in enumerate(self.features):
-
-            # verbose if requested
-            if self.verbose:
-                print(f" - [ChainedDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
-
-            # computing frequencies of each modality
-            frequencies = Xc[feature].value_counts(normalize=True)
-            values, frequencies = frequencies.index, frequencies.values
-
-            # checking for unknown values (values to present in an order of self.chained_orders)
-            missing = [value for value in values if notna(value) and (value not in self.known_values)]
-
-            # converting unknown values to NaN
-            if self.remove_unknown & (len(missing) > 0):
-
-                # alerting user
-                print(f"Order for {feature} was not provided for values: {missing}, these values will be converted to '{self.str_nan}' (policy remove_unknown=True)")
-
-                # adding missing valyes to the order
-                order = self.values_orders.get(feature)
-                order.update({self.str_nan: missing + order.get(self.str_nan)})
-
-            # alerting user
-            else:
-                assert not len(missing) > 0, f"Order for {feature} needs to be provided for values: {missing}, otherwise set remove_unknown=True"
-
-            # iterating over each specified orders
-            for order in self.chained_orders:
-                
-                # values that are frequent enough
-                to_keep = list(values[frequencies >= self.min_freq])
-
-                # all values from the order 
-                values_order = [o for v in order for o in order.get(v)]
-
-                # values from the order to group (not frequent enough or absent)
-                to_discard = [value for value in values_order if value not in to_keep]
-
-                # values to group into discarded values
-                value_to_group = [order.get_group(value) for value in to_discard]
-
-                # values of the series to input
-                df_to_input = [Xc[feature] == discarded for discarded in to_discard]  # identifying observation to input
-
-                # inputing non frequent values
-                Xc[feature] = select(df_to_input, value_to_group, default=Xc[feature])
-                
-                # historizing in the feature's order
-                for discarded, kept in zip(to_discard, value_to_group):
-                    self.values_orders.get(feature).group(discarded, kept)
-                    
-                # updating frequencies of each modality for the next ordering
-                frequencies = Xc[feature].value_counts(dropna=False, normalize=True).drop(nan, errors='ignore')  # dropping nans to keep them anyways
-                values, frequencies = frequencies.index, frequencies.values
-        
-        super().__init__(self.values_orders, str_nan=self.str_nan, copy=self.copy, output=str)
-        super().fit(X, y)
-            
-        return self
-
-class QuantileDiscretizer(BaseEstimator, TransformerMixin):
-    
-    def __init__(self, features: List[str], q: int, *, 
-    	         values_orders: Dict[str, Any]={},
-                 copy: bool=False, verbose: bool=False) -> None:
-        """ Discretizes quantitative features into groups of q quantiles"""
-        
-        self.features = features[:]
-        self.q = q
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.quantiles: Dict[str, Any] = {}
-        self.copy = copy
-        self.verbose = verbose
-
-    def fit(self, X: DataFrame, y: Series=None) -> None:
-        
-        # computing quantiles for the feature
-        self.quantiles = X[self.features].apply(find_quantiles, q=self.q, axis=0)
-
-        # case when only one feature is discretized
-        if len(self.features) == 1:
-        	self.quantiles = {self.features[0]: list(self.quantiles.get(self.features[0]).values)}
-
-        # building string of values to be displayed
-        values: List[str] = []
-        for n, feature in enumerate(self.features):
-
-            # verbose
-            if self.verbose:
-                print(f" - [QuantileDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
-
-            # quantiles as strings
-            feature_quantiles = self.quantiles.get(feature)
-            str_values = ['<= ' + q for q in format_list(feature_quantiles)]
-
-            # case when there is only one value
-            if len(feature_quantiles) == 0:
-                str_values = ['non-nan']
-
-            # last quantile is between the last value and inf
-            else:
-                str_values = str_values + [str_values[-1].replace('<= ', '>  ')]
-            values += [str_values]
-        
-        # adding inf for the last quantiles
-        self.quantiles = {f: q + [inf] for f, q in self.quantiles.items()}
-
-        # creating the values orders based on quantiles
-        self.values_orders.update({feature: GroupedList(str_values) for feature, str_values in zip(self.features, values)})
-
-        return self
-    
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
-        # copying dataset if requested
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-        
-        # iterating over each feature
-        for n, feature in enumerate(self.features):
-
-            # verbose if requested
-            if self.verbose:
-                print(f" - [QuantileDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
-
-            nans = isna(Xc[feature])  # keeping track of nans
-
-            # grouping values inside quantiles
-            to_input = [Xc[feature] <= q for q in self.quantiles.get(feature)]  # values that will be imputed
-            values = [[v] * len(X) for v in self.values_orders.get(feature)]  # new values to imput
-            Xc[feature] = select(to_input, values, default=Xc[feature])  # grouping modalities
-
-            # adding back nans
-            if any(nans):
-                Xc.loc[nans, feature] = nan
-        
-        return Xc
-
-class ClosestDiscretizer(BaseEstimator, TransformerMixin):
-    
-    def __init__(self, values_orders: Dict[str, Any], min_freq: float, *, default: str='worst', copy: bool=False, verbose: bool=False):
-        """ Discretizes ordered qualitative features into groups more frequent than min_freq"""
-        
-        self.features = list(values_orders.keys())
-        self.min_freq = min_freq
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.default = default[:]
-        self.default_values: Dict[str, Any] = {}
-        self.copy = copy
-        self.verbose = verbose
-
-    def fit(self, X: DataFrame, y: Series) -> None:
-        
-        # verbose
-        if self.verbose:
-            print(f" - [ClosestDiscretizer] Fit {', '.join(self.features)}")
-        
-        # grouping rare modalities for each feature
-        common_modalities = X[self.features].apply(
-            lambda u: find_common_modalities(u, y, self.min_freq, self.values_orders.get(u.name)), 
-            axis=0, result_type='expand'
-        ).T.to_dict()
-
-        # updating the order per feature
-        self.values_orders.update({f: common_modalities.get('order').get(f) for f in self.features})
-
-        # defining the default value based on the strategy
-        self.default_values = {f: common_modalities.get(self.default).get(f) for f in self.features}
-
-        return self
-    
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
-        # copying dataset if requested
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-
-        # iterating over each feature
-        for n, feature in enumerate(self.features):
-
-            # printing verbose if requested
-            if self.verbose:
-                print(f" - [ClosestDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
-
-            # accessing feature's modalities' order
-            order = self.values_orders.get(feature)
-
-            # imputation des valeurs inconnues le cas échéant
-            unknowns = [value for value in Xc[feature].unique() if not any(is_equal(value, known) for known in order.values())]
-            unknowns = [value for value in unknowns if notna(value)]  # suppression des NaNs
-            if any(unknowns):
-                to_input = [Xc[feature] == unknown for unknown in unknowns]  # identification des valeurs à regrouper
-                Xc[feature] = select(to_input, [self.default_values.get(feature)], default=Xc[feature])  # regroupement des valeurs
-                warn(f"Unknown modalities provided for {feature}: {unknowns}")
-
-            # grouping values inside groups of modalities
-            to_discard = [order.get(group) for group in order]  # identification des valeur à regrouper
-            to_input = [Xc[feature].isin(discarded) for discarded in to_discard]  # identification des valeurs à regrouper
-            Xc[feature] = select(to_input, order, default=Xc[feature])  # regroupement des valeurs
-
-        return Xc
-
-def min_value_counts(x: Series, order: List[Any]) -> float:
-    """ Minimum of modalities' frequencies. """
-
-    # modality frequency
-    values = x.value_counts(dropna=False, normalize=True)
-    
-    # ignoring NaNs
-    values = values.drop(nan, errors='ignore')
-    
-    # adding missing modalities
-    values = values.reindex(order).fillna(0)
-    
-    # minimal frequency 
-    min_values = values.values.min()
-
-    return min_values
-
-def value_counts(x: Series, dropna: bool=False, normalize: bool=True) -> dict:
-    """ Counts the values of each modality of a series into a dictionnary"""
-    
-    values = x.value_counts(dropna=dropna, normalize=normalize)
-    
-    return values.to_dict()
-
-def target_rate(x: Series, y: Series, dropna: bool=True, ascending=True) -> dict:
-    """ Target y rate per modality of x into a dictionnary"""
-    
-    rates = y.groupby(x, dropna=dropna).mean().sort_values(ascending=ascending)
-    
-    return rates.to_dict()
-
-def nunique(x: Series, dropna=False) -> int:
-    """ Computes number of unique modalities"""
-    
-    uniques = unique(x)
-    n = len(uniques)
-    
-    # removing nans
-    if dropna:
-        if any(isna(uniques)):
-            n -= 1
-    
-    return n
-
-class DefaultDiscretizer(BaseEstimator, TransformerMixin):
-    
-    def __init__(
-        self, features: List[str], min_freq: float, *, 
-        values_orders: Dict[str, Any]={},
-        default_value: str='__OTHER__',
-        str_nan: str='__NAN__',
-        copy: bool=False, verbose: bool=False) -> None:
-        """ Groups a qualitative features' values less frequent than min_freq into a default_value"""
-        
-        self.features = features[:]
-        self.min_freq = min_freq
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.default_value = default_value[:]
-        self.str_nan = str_nan[:]
-        self.copy = copy
-        self.verbose = verbose
-
-    def fit(self, X: DataFrame, y: Series) -> None:
-
-        # filling up NaNs
-        Xc = X[self.features].fillna(self.str_nan)
-
-        # computing frequencies of each modality
-        frequencies = Xc.apply(value_counts, normalize=True, axis=0)
-
-        # computing ordered target rate per modality for ordering
-        target_rates = Xc.apply(target_rate, y=y, ascending=True, axis=0)
-
-        # attributing orders to each feature
-        self.values_orders.update({f: GroupedList(list(target_rates[f])) for f in self.features})
-        
-        # number of unique modality per feature
-        nuniques = Xc.apply(nunique, axis=0)
-            
-        # identifying modalities which are the most common
-        self.to_keep: Dict[str, Any] = {}  # dict of features and corresponding kept modalities
-
-        # iterating over each feature
-        for feature in self.features:
-
-            # checking for binary features
-            if nuniques[feature] > 2:
-                kept = [val for val, freq in frequencies[feature].items() if freq >= self.min_freq]
-
-            # keeping all modalities of binary features
-            else:
-                kept = [val for val, freq in frequencies[feature].items()]
-
-            self.to_keep.update({feature: kept})
-
-        # grouping rare modalities 
-        for n, feature in enumerate(self.features):
-
-        	# printing verbose
-            if self.verbose:
-                print(f" - [DefaultDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
-
-            # identifying values to discard (rare modalities)
-            to_discard = [value for value in self.values_orders[feature] if value not in self.to_keep[feature]]
-
-            # discarding rare modalities
-            if len(to_discard) > 0:
-
-                # adding default_value to possible values
-                order = self.values_orders[feature]
-                order.append(self.default_value)
-
-                # grouping rare modalities into default_value
-                order.group_list(to_discard, self.default_value)
-
-                # computing target rate for default value and reordering values according to feature's target rate
-                default_target_rate = y.loc[X[feature].isin(order.get(self.default_value))].mean()  # computing target rate for default value
-                order_target_rate = [target_rates.get(feature).get(value) for value in order if value != self.default_value]
-                default_position = next(n for n, trate in enumerate(order_target_rate + [inf]) if trate > default_target_rate)
-
-                # updating the modalities' order                
-                new_order = order[:-1][:default_position] + [self.default_value] + order[:-1][default_position:]  # getting rid of default value already in order
-                order = order.sort_by(new_order)
-                self.values_orders.update({feature: order})
-
-        return self
-
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-
-        # copying dataset if requested
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-
-        # filling up NaNs
-        Xc[self.features] = Xc[self.features].fillna(self.str_nan)
-
-        # grouping values inside groups of modalities
-        for n, feature in enumerate(self.features):
-
-            # verbose if requested
-            if self.verbose: 
-                print(f" - [DefaultDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
-
-            # grouping modalities
-            Xc[feature] = select([~Xc[feature].isin(self.to_keep[feature])], [self.default_value], default=Xc[feature])
-
-        return Xc
-
-
-
-def find_quantiles(df_feature: Series, q: int, len_df: int=None, quantiles: List[float]=None) -> List[float]:
-    """ Découpage en quantile de la feature.
-    
-    Fonction récursive : on prend l'échantillon et on cherche des valeurs sur-représentées
-    Si la valeur existe on la met dans une classe et on cherche à gauche et à droite de celle-ci, d'autres variables sur-représentées
-    Une fois il n'y a plus de valeurs qui soient sur-représentées,
-    on fait un découpage classique avec qcut en multipliant le nombre de classes souhaité par le pourcentage de valeurs restantes sur le total
-    
-    """
-
-    # initialisation de la taille total du dataframe
-    if len_df is None:
-        len_df = len(df_feature)
-    
-    # initialisation de la liste des quantiles
-    if quantiles is None:
-        quantiles = []
-
-    # calcul du nombre d'occurences de chaque valeur
-    frequencies = df_feature.value_counts(dropna=False, normalize=False).drop(nan, errors='ignore') / len_df # dropping nans to keep them anyways
-    values, frequencies = array(frequencies.index), array(frequencies.values)
-    
-    # cas 1 : il n'y a pas d'observation dans le dataframe
-    if len(df_feature) == 0:
-        
-        return quantiles
-    
-    # cas 2 : il y a des valeurs manquantes NaN
-    elif any(isna(df_feature)):
-        
-        return find_quantiles(df_feature[notna(df_feature)], q, len_df=len_df, quantiles=quantiles)
-        
-    # cas 2 : il n'y a que des valeurs dans le dataframe (pas de NaN)
-    else:
-        
-        # cas 1 : il existe une valeur sur-représentée
-        if any(frequencies > 1 / q):
-
-            # identification de la valeur sur-représentée
-            frequent_value = values[frequencies.argmax()]
-            
-            # ajout de la valeur fréquente à la liste des quantiles
-            quantiles += [frequent_value]
-
-            # calcul des quantiles pour les parties inférieures et supérieures
-            quantiles_inf = find_quantiles(df_feature[df_feature < frequent_value], q, len_df=len_df)
-            quantiles_sup = find_quantiles(df_feature[df_feature > frequent_value], q, len_df=len_df)
-            
-            return quantiles_inf + quantiles + quantiles_sup
-
-        # cas 2 : il n'existe pas de valeur sur-représentée
-        else:
-            
-            # nouveau nombre de quantile en prenant en compte les classes déjà constituées
-            new_q = max(round(len(df_feature) / len_df * q), 1)
-            
-            # calcul des quantiles sur le dataframe
-            if new_q > 1:
-                quantiles += list(quantile(df_feature.values, linspace(0, 1, new_q + 1)[1:-1], interpolation='lower'))
-
-            # case when there are no enough observations to compute quantiles
-            else:
-                quantiles += [max(df_feature.values)]
-
-            return quantiles
-
-def is_equal(a: Any, b: Any) -> bool:
-    """ checks if a and b are equal (NaN insensitive)"""
-    
-    # default equality
-    equal = a == b
-    
-    # Case where a and b are NaNs
-    if isna(a) and isna(b):
-        equal = True
-    
-    return equal
-
-def find_common_modalities(df_feature: Series, y: Series, min_freq: float, order: GroupedList, len_df: int=None) -> Dict[str, Any]:
-    """ Découpage en modalités de fréquence minimal (Cas des variables ordonnées).
-    
-    Fonction récursive : on prend l'échantillon et on cherche des valeurs sur-représentées
-    Si la valeur existe on la met dans une classe et on cherche à gauche et à droite de celle-ci, d'autres variables sur-représentées
-    Une fois il n'y a plus de valeurs qui soient sur-représentées,
-    on fait un découpage classique avec qcut en multipliant le nombre de classes souhaité par le pourcentage de valeurs restantes sur le total
-    
-    """
-
-    # initialisation de la taille totale du dataframe
-    if len_df is None:
-        len_df = len(df_feature)
-    
-    # conversion en GroupedList si ce n'est pas le cas 
-    order = GroupedList(order)
-    
-    # cas 1 : il y a des valeurs manquantes NaN
-    if any(isna(df_feature)):
-        
-        return find_common_modalities(df_feature[notna(df_feature)], y[notna(df_feature)], min_freq, order, len_df)
-
-
-    # cas 2 : il n'y a que des valeurs dans le dataframe (pas de NaN)
-    else:
-        
-        # computing frequencies and target rate of each modality
-        init_frequencies = df_feature.value_counts(dropna=False, normalize=False) / len_df
-        init_values, init_frequencies = init_frequencies.index, init_frequencies.values
-        
-        # ordering
-        frequencies = [init_frequencies[init_values == value][0] if any(init_values == value) else 0 for value in order]  # sort selon l'ordre des modalités
-        values = [init_values[init_values == value][0] if any(init_values == value) else value for value in order]  # sort selon l'ordre des modalités
-        target_rate = y.groupby(df_feature).sum().reindex(order) / frequencies / len_df # target rate per modality
-        underrepresented = [value for value, frequency in zip(values, frequencies) if frequency < min_freq]  # valeur peu fréquentes
-
-        # cas 1 : il existe une valeur sous-représentée
-        while any(underrepresented) & (len(frequencies) > 1):
-
-            # identification de la valeur sous-représentée
-            discarded_idx = argmin(frequencies)
-            discarded = values[discarded_idx]
-
-            # identification de la modalité la plus proche (volume et taux de défaut)
-            kept = find_closest_modality(discarded, discarded_idx, list(zip(order, frequencies, target_rate)), min_freq)
-
-            # removing the value from the initial ordering
-            order.group(discarded, kept)
-            
-            # ordering
-            frequencies = [init_frequencies[init_values == value][0] if any(init_values == value) else 0 for value in order]  # sort selon l'ordre des modalités
-            values = [init_values[init_values == value][0] if any(init_values == value) else value for value in order]  # sort selon l'ordre des modalités
-            target_rate = y.groupby(df_feature).sum().reindex(order) / frequencies / len_df # target rate per modality
-            underrepresented = [value for value, frequency in zip(values, frequencies) if frequency < min_freq]  # valeur peu fréquentes
-
-        worst, best = target_rate.idxmin(), target_rate.idxmax()
-
-        # cas 2 : il n'existe pas de valeur sous-représentée
-        return {'order': order, 'worst': worst, 'best': best}
-
-def find_closest_modality(value, idx: int, freq_target: Series, min_freq: float) -> int:
-    """HELPER Finds the closest modality in terms of frequency and target rate"""
-
-    # case 1: lowest modality
-    if idx == 0:
-        closest_modality = 1
-        
-    # case 2: biggest modality
-    elif idx == len(freq_target) - 1:
-        closest_modality = len(freq_target) - 2
-    
-    # case 3: not the lowwest nor the biggest modality
-    else:
-        # previous modality's volume and target rate
-        previous_value, previous_volume, previous_target = freq_target[idx - 1]
-        
-        # current modality's volume and target rate
-        _, volume, target = freq_target[idx]
-        
-        # next modality's volume and target rate
-        next_value, next_volume, next_target = freq_target[idx + 1]
-        
-        # regroupement par volumétrie (préféré s'il n'y a pas beaucoup de volume)
-        # case 1: la modalité suivante est inférieure à min_freq 
-        if next_volume < min_freq <= previous_volume:
-            closest_modality = idx + 1
-            
-        # case 2: la modalité précédante est inférieure à min_freq 
-        elif previous_volume < min_freq <= next_volume:
-            closest_modality = idx - 1
-            
-        # case 3: les deux modalités sont inférieures à min_freq 
-        elif (previous_volume < min_freq) & (next_volume < min_freq):
-            
-            # cas 1: la modalité précédante est inférieure à la modalité suivante
-            if previous_volume < next_volume:
-                closest_modality = idx - 1
-            
-            # cas 2: la modalité suivante est inférieure à la modalité précédante
-            elif next_volume < previous_volume:
-                closest_modality = idx + 1
-            
-            # cas 3: les deux modalités ont la même fréquence
-            else:
-                
-                # cas1: la modalité précédante est plus prorche en taux de cible
-                if abs(previous_target - target) <= abs(next_target - target):
-                    closest_modality = idx - 1
-                    
-                # cas2: la modalité précédante est plus prorche en taux de cible
-                else:
-                    closest_modality = idx + 1
-                
-        # case 4: les deux modalités sont supérieures à min_freq 
-        else:
-                
-            # cas1: la modalité précédante est plus prorche en taux de cible
-            if abs(previous_target - target) <= abs(next_target - target):
-                closest_modality = idx - 1
-
-            # cas2: la modalité précédante est plus prorche en taux de cible
-            else:
-                closest_modality = idx + 1
-    
-    # récupération de la valeur associée
-    closest_value = freq_target[closest_modality][0]
-    
-    return closest_value
-
-
-def format_list(a_list: List[float]) -> List[str]:
-    """ Formats a list of floats to a list of unique rounded strings of floats"""
-
-    # finding the closest power of thousands for each element
-    closest_powers = [next((k for k in range(-3, 4) if abs(elt) / 100 // 1000**(k) < 10)) for elt in a_list]
-
-    # rounding elements to the closest power of thousands
-    rounded_to_powers = [elt / 1000**(k) for elt, k in zip(a_list, closest_powers)]
-
-    # computing optimal decimal per unique power of thousands
-    optimal_decimals: Dict[str, int] = {}
-    for power in unique(closest_powers):  # iterating over each power of thousands found
-
-        # filtering on the specific power of thousands
-        sub_array = array([elt for elt, p in zip(rounded_to_powers, closest_powers) if power == p])
-
-        # number of distinct values
-        n_uniques = sub_array.shape[0]
-
-        # computing the first rounding decimal that allows for distinction of each values when rounded
-        # by default None (no rounding)
-        optimal_decimal = next((k for k in range(1, 10) if len(unique(sub_array.round(k))) == n_uniques), None)
-
-        # storing in the dict    
-        optimal_decimals.update({
-            power: optimal_decimal
-        })
-
-    # rounding according to each optimal_decimal
-    rounded_list: List[float] = []
-    for elt, power in zip(rounded_to_powers, closest_powers):
-
-        # rounding each element
-        rounded = elt  # by default None (no rounding)
-        optimal_decimal = optimal_decimals.get(power)
-        if optimal_decimal:  # checking that the optimal decimal exists
-            rounded = round(elt, optimal_decimal)
-
-        # adding the rounded number to the list
-        rounded_list += [rounded]
-
-    # dict of suffixes per power of thousands
-    suffixes = {
-        -3: 'n', -2: 'mi', -1: 'm', 0: '', 1: 'K', 2: 'M', 3: 'B'
-    }
-
-    # adding the suffixes
-    formatted_list = [f'{elt: 3.3f}{suffixes[power]}' for elt, power in zip(rounded_list, closest_powers)]
-    
-    # keeping zeros
-    formatted_list = [rounded if raw != 0 else f'{raw: 3.3f}' for rounded, raw in zip(formatted_list, a_list)]
-    
-    return formatted_list
+from IPython.display import display_html
+from numpy import sort, nan, inf, float32, where, isin, argsort, array, select, append, quantile, linspace, argmin
+from pandas import DataFrame, Series, isna, qcut, notna, unique
+from pandas.api.types import is_numeric_dtype, is_string_dtype
+from sklearn.base import BaseEstimator, TransformerMixin
+from typing import Any, Dict, List
+from warnings import warn
+
+def nan_unique(x: Series):
+    """ Unique non-NaN values. """
+    
+    # unique values
+    uniques = unique(x)
+    
+    # filtering out nans
+    uniques = [u for u in uniques if notna(u)]
+    
+    return uniques
+
+class GroupedList(list):
+    
+    def __init__(self, iterable=()) -> None:
+        """ An ordered list that historizes its elements' merges."""
+
+        # case 0: iterable is the contained dict
+        if isinstance(iterable, dict):
+            # TODO: check thaht keys are in list
+            
+            # récupération des valeurs de la liste (déjà ordonné)
+            values = [key for key in iterable]
+
+            # initialsiation de la liste
+            super().__init__(values)
+
+            # attribution des valeurs contenues
+            self.contained = {k: v for k, v in iterable.items()}
+
+            # adding key to itself if that's not the case
+            for k in [k for k in values if k not in self.contained.get(k)]:
+                self.contained.update({k: self.contained.get(k) + [k]})
+        
+        # case 1: copying a GroupedList
+        elif hasattr(iterable, 'contained'):
+
+            # initialsiation de la liste
+            super().__init__(iterable)
+
+            # copie des groupes
+            self.contained = {k: v for k, v in iterable.contained.items()}
+        
+        # case 2: initiating GroupedList from a list
+        elif isinstance(iterable, list):
+
+            # initialsiation de la liste
+            super().__init__(iterable)
+
+            # création des groupes
+            self.contained = {v: [v] for v in iterable}
+
+    def group_list(self, to_discard: List[Any], to_keep: Any) -> None:
+        """ Groups elements to_discard into values to_keep"""
+        
+        for discarded, kept in zip(to_discard, [to_keep] * len(to_discard)):
+            self.group(discarded, kept)
+
+    def group(self, discarded: Any, kept: Any) -> None:
+        """ Groups the discarded value with the kept value"""
+
+        # checking that those values are distinct
+        if not is_equal(discarded, kept):
+
+            # checking that those values exist in the list
+            assert discarded in self, f"{discarded} not in list"
+            assert kept in self, f"{kept} not in list"
+
+            # accessing values contained in each value
+            contained_discarded = self.contained.get(discarded)
+            contained_kept = self.contained.get(kept)
+
+            # updating contained dict
+            self.contained.update({
+                kept: contained_discarded + contained_kept,
+                discarded: []
+            })
+
+            # removing discarded from the list
+            self.remove(discarded)
+        
+        return self
+        
+    def append(self, new_value: Any) -> None:
+        """ Appends a new_value to the GroupedList"""
+        
+        self += [new_value]
+        
+        self.contained.update({new_value: [new_value]})
+        
+        return self
+        
+    def update(self, new_value: Dict[Any, List[Any]]) -> None:
+        """ Updates the GroupedList via a dict"""
+        
+        # adding keys to the order if they are new values
+        for k in [c for c in new_value if c not in self]:
+            self += new_value.keys()
+        
+        # updating contained accord to new_value
+        self.contained.update(new_value)
+        
+        return self
+
+    def sort(self) -> None:
+        """ Sorts the values of the list and dict (if any, NaNs are last). """
+
+        # str values
+        keys_str = [key for key in self if isinstance(key, str)]
+
+        # non-str values
+        keys_float = [key for key in self if not isinstance(key, str)]
+
+        # sorting and merging keys
+        keys = list(sort(keys_str)) + list(sort(keys_float)) 
+
+        # recreating an ordered GroupedList
+        self = GroupedList({k: self.get(k) for k in keys})
+
+        return self
+
+    def sort_by(self, ordering: List[Any]) -> None:
+        """ Sorts the values of the list and dict, if any, NaNs are the last. """
+
+        # checking that all values are given an order
+        assert all([o in self for o in ordering]), f"Unknown values in ordering: {', '.join([str(v) for v in ordering if v not in self])}"
+        assert all([s in ordering for s in self]), f"Missing value from ordering: {', '.join([str(v) for v in self if v not in ordering])}"
+
+        # ordering the contained
+        self = GroupedList({k: self.get(k) for k in ordering})
+
+        return self
+
+    
+    def remove(self, value: Any) -> None:
+        
+        super().remove(value)
+        self.contained.pop(value)
+    
+    def pop(self, idx: int) -> None:
+        
+        value = self[idx]
+        self.remove(value)
+    
+    def get(self, key: Any) -> List[Any]:
+        """ returns list of values contained in key"""
+
+        # default to fing an element
+        found = self.contained.get(key)
+
+        # copying with dictionnaries (not working with numpy.nan)
+        # if isna(key):
+            # found = [value for dict_key, value in self.contained.items() if is_equal(dict_key, key)][0]
+
+        return found
+
+    def get_group(self, value: Any) -> Any:
+        """ returns the group containing the specified value """
+        
+        found = [key for key, values in self.contained.items() if any(is_equal(value, elt) for elt in values)]
+
+        if any(found):
+            return found[0]
+        else:
+            return value
+
+    def values(self) -> List[Any]:
+        """ returns all values contained in each group """
+
+        known = [value for values in self.contained.values() for value in values]
+
+        return known
+
+    def contains(self, value: Any) -> bool:
+        """ checks if a value if contained in any group """
+
+        known_values = self.values()
+
+        return any(is_equal(value, known) for known in known_values)
+
+    def get_repr(self, char_limit: int=10) -> List[str]:
+        """" Returns a representative list of strings of values of groups. """
+
+        # initiating list of group representation
+        repr: List[str] = []
+
+        # iterating over each group
+        for group in self:
+
+            # accessing group's values
+            values = self.get(group)
+
+            if len(values) == 0:  # case 0: there are no value in this group
+                pass
+            
+            elif len(values) == 1:  # case 1: there is only one value in this group
+                repr += [values[0]]
+            
+            elif len(values) == 2:  # case 2: two values in this group
+                repr += [f'{values[1]}'[:char_limit]+' and '+f'{values[0]}'[:char_limit]]
+            
+            elif len(values) > 2:  # case 3: more than two values in this group
+                repr += [f'{values[-1]}'[:char_limit]+' to '+f'{values[0]}'[:char_limit]]
+                
+        return repr
+
+
+class GroupedListDiscretizer(BaseEstimator, TransformerMixin):
+    
+    def __init__(self, values_orders: Dict[str, Any], *, 
+        copy: bool=False, output: type= float,
+        str_nan: str=None, verbose: bool=False) -> None:
+        
+        self.features = list(values_orders.keys())
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.copy = copy
+        self.output = output
+        self.verbose = verbose
+        self.str_nan = str_nan
+        
+    def fit(self, X, y=None) -> None:
+
+        return self
+    
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+
+        # copying dataframes
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+
+        # filling up nans with specified value
+        if self.str_nan:
+            Xc[self.features] = Xc[self.features].fillna(self.str_nan)
+
+        # iterating over each feature
+        for n, feature in enumerate(self.features):
+            
+            # verbose if requested
+            if self.verbose: 
+                print(f" - [GroupedListDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
+            
+            # bucketizing feature
+            order = self.values_orders.get(feature)  # récupération des groupes
+            to_discard = [order.get(group) for group in order]  # identification des valeur à regrouper
+            to_input = [Xc[feature].isin(discarded) for discarded in to_discard]  # identifying main bucket value
+            to_keep = [n if self.output == float else group for n, group in enumerate(order)]  # récupération du groupe dans lequel regrouper
+
+            # case when there are no values
+            if len(to_input)==0 & len(to_keep)==0:
+                pass
+
+            # grouping modalities
+            else:
+                Xc[feature] = select(to_input, to_keep, default=Xc[feature])
+
+        # converting to float
+        if self.output == float:
+            Xc[self.features] = Xc[self.features].astype(float32)
+
+        return Xc
+
+
+class QualitativeDiscretizer(BaseEstimator, TransformerMixin):
+    """ Automatic discretizing of categorical and categorical ordinal features.
+
+    Modalities/values of features are grouped according to there respective orders:
+     - [Qualitative features] order based on modality target rate.
+     - [Qualitative ordinal features] user-specified order.
+
+    TODO: pass ordinal_features/qualitati_features as parameters to be able to pass values_orders with other orders (ex: from chaineddiscretizer)
+
+    Parameters
+    ----------
+    features: list
+        Contains qualitative (categorical and categorical ordinal) features to be discretized.
+
+    min_freq: int
+        [Qualitative features] Minimal frequency of a modality.
+         - NaNs are considered a specific modality but will not be grouped.
+         - [Qualitative features] Less frequent modalities are grouped in the `__OTHER__` modality.
+         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
+        (smallest frequency or closest target rate), between the superior and inferior values (specified
+        in the `values_orders` dictionnary).
+        Recommandation: `min_freq` should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
+
+    values_orders: dict, default {}
+        [Qualitative ordinal features] dict of features values and list of orders of their values.
+         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
+        (smallest frequency or closest target rate), between the superior and inferior values (described
+        by the `values_orders`).
+        Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
+    """
+    
+    def __init__(self, features: List[str], min_freq: float, *,
+                 values_orders: Dict[str, Any]={}, copy: bool=False, 
+                 verbose: bool=False) -> None:
+    
+        self.features = features[:]
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.ordinal_features = [f for f in values_orders if f in features]  # ignores non qualitative features
+        self.non_ordinal_features = [f for f in features if f not in self.ordinal_features]
+        self.min_freq = min_freq
+        self.pipe: List[BaseEstimator] = []
+        self.copy = copy
+        self.verbose = verbose
+        
+    def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
+        """ Checking data for bucketization"""
+        
+        # checking for quantitative columns
+        is_object = X[self.features].dtypes.apply(is_string_dtype)
+        assert all(is_object), f"Non-string features: {', '.join(is_object[~is_object].index)}, consider using Converters.StringConverter."
+        
+        # checking for binary target
+        y_values = unique(y)
+        assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
+        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
+        
+        # checking that all unique values in X are in values_orders
+        uniques = X[self.features].apply(nan_unique)
+        for feature in self.ordinal_features:
+            missing = [val for val in uniques[feature] if val not in self.values_orders[feature]]
+            assert len(missing)==0, f"The ordering for {', '.join(missing)} of feature '{feature}' must be specified in values_orders (str-only)."
+        
+        # copying dataframe
+        Xc = X.copy()
+        
+        return Xc
+
+    def fit(self, X: DataFrame, y: Series) -> None:
+        """ Learning TRAIN distribution"""
+        
+        # checking data before bucketization
+        Xc = self.prepare_data(X, y)
+
+        # [Qualitative ordinal features] Grouping rare values into closest common one
+        if len(self.ordinal_features) > 0:
+
+            # discretizing
+            ordinal_orders = {k: GroupedList(v) for k, v in self.values_orders.items() if k in self.ordinal_features}
+            discretizer = ClosestDiscretizer(
+                ordinal_orders, min_freq=self.min_freq, verbose=self.verbose
+            )
+            discretizer.fit(Xc, y)
+
+            # storing results
+            self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
+            self.pipe += [('QualitativeClosestDiscretizer', discretizer)]  # adding discretizer to pipe
+
+        # [Qualitative non-ordinal features] Grouping rare values into default_value '__OTHER__'
+        if len(self.non_ordinal_features) > 0:
+
+            # Grouping rare modalities
+            discretizer = DefaultDiscretizer(self.non_ordinal_features, min_freq=self.min_freq, 
+                                             values_orders=self.values_orders,
+                                             verbose=self.verbose)
+            discretizer.fit(Xc, y)
+
+            # storing results
+            self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
+            self.pipe += [('DefaultDiscretizer', discretizer)]  # adding discretizer to pipe
+
+        return self
+
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        """ Applying learned bucketization on TRAIN and/or TEST"""
+
+        # copying dataframe if requested
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+
+        # iterating over each transformer
+        for _, step in self.pipe:
+            Xc = step.transform(Xc)
+
+        return Xc
+
+class QuantitativeDiscretizer(BaseEstimator, TransformerMixin):
+    """ Automatic discretizing of continuous features.
+
+    Modalities/values of features are grouped according to there respective orders:
+     - [Quantitative features] real order of the values.
+
+    Parameters
+    ----------
+    features: list
+        Contains quantitative (continuous) features to be discretized.
+
+    q: int, default None
+        [Quantitative features] Number of quantiles to initialy cut the feature.
+         - NaNs are considered a specific value but will not be grouped.
+         - Values more frequent than `1/q` will be set as their own group and remaining frequency will be
+        cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
+        Exemple: if q=10 and the value numpy.nan represent 50 % of the observed values, non-NaNs will be 
+        cut in q=5 quantiles.
+        Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
+
+    """
+    
+    def __init__(self, features: List[str], q: int, *, values_orders: Dict[str, Any]={}, copy: bool=False, 
+                 verbose: bool=False) -> None:
+        
+        self.features = features[:]
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.q = q
+        self.pipe: List[BaseEstimator] = []
+        self.copy = copy
+        self.verbose = verbose
+    
+    def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
+        """ Checking data for bucketization"""
+        
+        # checking for quantitative columns
+        is_numeric = X[self.features].dtypes.apply(is_numeric_dtype)
+        assert all(is_numeric), f"Non-numeric features: {', '.join(is_numeric[~is_numeric].index)}"
+        
+        # checking for binary target
+        y_values = unique(y)
+        assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
+        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
+        
+        # copying dataframe
+        Xc = X.copy()
+        
+        return Xc
+
+    def fit(self, X: DataFrame, y: Series) -> None:
+        """ Learning TRAIN distribution"""
+        
+        # checking data before bucketization
+        Xc = self.prepare_data(X, y)
+
+        # [Quantitative features] Grouping values into quantiles
+        discretizer = QuantileDiscretizer(self.features, q=self.q, values_orders=self.values_orders, verbose=self.verbose)
+        Xc = discretizer.fit_transform(Xc, y)
+
+        # storing results
+        self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
+        self.pipe += [('QuantileDiscretizer', discretizer)]  # adding discretizer to pipe
+
+        # [Quantitative features] Grouping rare quantiles into closest common one
+        #  -> can exist because of overrepresented values (values more frequent than 1/q)
+        # searching for features with rare quantiles: computing min frequency per feature
+        frequencies = Xc[self.features].apply(lambda u: min_value_counts(u, self.values_orders[u.name]), axis=0)
+        
+        # minimal frequency of a quantile
+        q_min_freq = 1 / self.q / 2
+        
+        # identifying features that have rare modalities
+        has_rare = list(frequencies[frequencies <= q_min_freq].index)
+        
+        # Grouping rare modalities
+        if len(has_rare) > 0:
+            
+            # Grouping only features with rare modalities 
+            rare_values_orders = {feature: order for feature, order in self.values_orders.items() if feature in has_rare}
+            discretizer = ClosestDiscretizer(rare_values_orders, min_freq=q_min_freq, verbose=self.verbose)
+            discretizer.fit(Xc, y)
+
+            # storing results
+            self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
+            self.pipe += [('QuantitativeClosestDiscretizer', discretizer)]  # adding discretizer to pipe
+
+        return self
+
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        """ Applying learned bucketization on TRAIN and/or TEST"""
+
+        # copying dataframe if requested
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+
+        # iterating over each transformer
+        for _, step in self.pipe:
+            Xc = step.transform(Xc)
+
+        return Xc
+
+class Discretizer(BaseEstimator, TransformerMixin):
+    """ Automatic discretizing of continuous, categorical and categorical ordinal features.
+
+    Modalities/values of features are grouped according to there respective orders:
+     - [Qualitative features] order based on modality target rate.
+     - [Qualitative ordinal features] user-specified order.
+     - [Quantitative features] real order of the values.
+
+    Parameters
+    ----------
+    quanti_features: list
+        Contains quantitative (continuous) features to be discretized.
+
+    quali_features: list
+        Contains qualitative (categorical and categorical ordinal) features to be discretized.
+
+    min_freq: int, default None
+        [Qualitative features] Minimal frequency of a modality.
+         - NaNs are considered a specific modality but will not be grouped.
+         - [Qualitative features] Less frequent modalities are grouped in the `__OTHER__` modality.
+         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
+        (smallest frequency or closest target rate), between the superior and inferior values (specified
+        in the `values_orders` dictionnary).
+        Recommandation: `min_freq` should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
+
+    q: int, default None
+        [Quantitative features] Number of quantiles to initialy cut the feature.
+         - NaNs are considered a specific value but will not be grouped.
+         - Values more frequent than `1/q` will be set as their own group and remaining frequency will be
+        cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
+        Exemple: if q=10 and the value numpy.nan represent 50 % of the observed values, non-NaNs will be 
+        cut in q=5 quantiles.
+        Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
+
+    values_orders: dict, default {}
+        [Qualitative ordinal features] dict of features values and list of orders of their values.
+         - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
+        (smallest frequency or closest target rate), between the superior and inferior values (described
+        by the `values_orders`).
+        Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
+    """
+
+    def __init__(self, quanti_features: List[str], quali_features: List[str], min_freq: float, *, 
+                 values_orders: Dict[str, Any]={}, copy: bool=False, verbose: bool=False) -> None:
+
+        self.features = quanti_features[:] + quali_features[:]
+        self.quanti_features = quanti_features[:]
+        assert len(list(set(quanti_features))) == len(quanti_features), "Column duplicates in quanti_features"
+        self.quali_features = quali_features[:]
+        assert len(list(set(quali_features))) == len(quali_features), "Column duplicates in quali_features"
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.min_freq = min_freq
+        self.q = int(1 / min_freq)  # number of quantiles
+        self.pipe: List[BaseEstimator] = []
+        self.copy = copy
+        self.verbose = verbose
+
+    def fit(self, X: DataFrame, y: Series) -> None:
+
+        # [Qualitative features] Grouping qualitative features
+        if len(self.quali_features) > 0:
+
+            # verbose if requested
+            if self.verbose:
+                print("\n---\n[Discretizer] Fit Qualitative Features")
+
+            # grouping qualitative features
+            discretizer = QualitativeDiscretizer(
+                self.quali_features, min_freq=self.min_freq,
+                values_orders=self.values_orders, copy=self.copy,
+                verbose=self.verbose
+            )
+            discretizer.fit(X, y)
+
+            # storing results
+            self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
+            self.pipe += discretizer.pipe  # adding discretizer to pipe
+
+        # [Quantitative features] Grouping quantitative features
+        if len(self.quanti_features) > 0:
+
+            # verbose if requested
+            if self.verbose:
+                print("\n---\n[Discretizer] Fit Quantitative Features")
+
+            # grouping quantitative features
+            discretizer = QuantitativeDiscretizer(
+                self.quanti_features, q=self.q,
+                values_orders=self.values_orders, copy=self.copy,
+                verbose=self.verbose
+            )
+            discretizer.fit(X, y)
+
+            # storing results
+            self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
+            self.pipe += discretizer.pipe  # adding discretizer to pipe
+
+        return self
+
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+
+        # verbose if requested
+        if self.verbose:
+            print("\n---\n[Discretizer] Transform Features")
+        
+        # copying dataframe if requested
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+
+        # iterating over each transformer
+        for _, step in self.pipe:
+            Xc = step.transform(Xc)
+
+        return Xc
+
+
+
+class ChainedDiscretizer(GroupedListDiscretizer):
+    
+    def __init__(self, features: List[str], min_freq: float, chained_orders: List[GroupedList], *, 
+                 remove_unknown: bool=False, str_nan: str='__NAN__', copy: bool=False, verbose: bool=False) -> None:       
+        
+        self.min_freq = min_freq
+        self.features = features[:]
+        self.chained_orders = [GroupedList(order) for order in chained_orders]
+        self.copy = copy
+        self.verbose = verbose
+
+        # parameters to handle missing/unknown values
+        self.remove_unknown = remove_unknown
+        self.str_nan = str_nan
+        
+        # initiating features' values orders to all possible values
+        self.known_values = list(set([v for o in self.chained_orders for v in o.values()]))
+        self.values_orders = {f: GroupedList(self.known_values[:] + [self.str_nan]) for f in self.features}
+
+    def fit(self, X: DataFrame, y: Series=None) -> None:
+        
+        # filling nans
+        Xc = X[self.features].fillna(self.str_nan)
+        
+        # iterating over each feature
+        for n, feature in enumerate(self.features):
+
+            # verbose if requested
+            if self.verbose:
+                print(f" - [ChainedDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
+
+            # computing frequencies of each modality
+            frequencies = Xc[feature].value_counts(normalize=True)
+            values, frequencies = frequencies.index, frequencies.values
+
+            # checking for unknown values (values to present in an order of self.chained_orders)
+            missing = [value for value in values if notna(value) and (value not in self.known_values)]
+
+            # converting unknown values to NaN
+            if self.remove_unknown & (len(missing) > 0):
+
+                # alerting user
+                print(f"Order for {feature} was not provided for values: {missing}, these values will be converted to '{self.str_nan}' (policy remove_unknown=True)")
+
+                # adding missing valyes to the order
+                order = self.values_orders.get(feature)
+                order.update({self.str_nan: missing + order.get(self.str_nan)})
+
+            # alerting user
+            else:
+                assert not len(missing) > 0, f"Order for {feature} needs to be provided for values: {missing}, otherwise set remove_unknown=True"
+
+            # iterating over each specified orders
+            for order in self.chained_orders:
+                
+                # values that are frequent enough
+                to_keep = list(values[frequencies >= self.min_freq])
+
+                # all values from the order 
+                values_order = [o for v in order for o in order.get(v)]
+
+                # values from the order to group (not frequent enough or absent)
+                to_discard = [value for value in values_order if value not in to_keep]
+
+                # values to group into discarded values
+                value_to_group = [order.get_group(value) for value in to_discard]
+
+                # values of the series to input
+                df_to_input = [Xc[feature] == discarded for discarded in to_discard]  # identifying observation to input
+
+                # inputing non frequent values
+                Xc[feature] = select(df_to_input, value_to_group, default=Xc[feature])
+                
+                # historizing in the feature's order
+                for discarded, kept in zip(to_discard, value_to_group):
+                    self.values_orders.get(feature).group(discarded, kept)
+                    
+                # updating frequencies of each modality for the next ordering
+                frequencies = Xc[feature].value_counts(dropna=False, normalize=True).drop(nan, errors='ignore')  # dropping nans to keep them anyways
+                values, frequencies = frequencies.index, frequencies.values
+        
+        super().__init__(self.values_orders, str_nan=self.str_nan, copy=self.copy, output=str)
+        super().fit(X, y)
+            
+        return self
+
+class QuantileDiscretizer(BaseEstimator, TransformerMixin):
+    
+    def __init__(self, features: List[str], q: int, *, 
+    	         values_orders: Dict[str, Any]={},
+                 copy: bool=False, verbose: bool=False) -> None:
+        """ Discretizes quantitative features into groups of q quantiles"""
+        
+        self.features = features[:]
+        self.q = q
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.quantiles: Dict[str, Any] = {}
+        self.copy = copy
+        self.verbose = verbose
+
+    def fit(self, X: DataFrame, y: Series=None) -> None:
+        
+        # computing quantiles for the feature
+        self.quantiles = X[self.features].apply(find_quantiles, q=self.q, axis=0)
+
+        # case when only one feature is discretized
+        if len(self.features) == 1:
+        	self.quantiles = {self.features[0]: list(self.quantiles.get(self.features[0]).values)}
+
+        # building string of values to be displayed
+        values: List[str] = []
+        for n, feature in enumerate(self.features):
+
+            # verbose
+            if self.verbose:
+                print(f" - [QuantileDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
+
+            # quantiles as strings
+            feature_quantiles = self.quantiles.get(feature)
+            str_values = ['<= ' + q for q in format_list(feature_quantiles)]
+
+            # case when there is only one value
+            if len(feature_quantiles) == 0:
+                str_values = ['non-nan']
+
+            # last quantile is between the last value and inf
+            else:
+                str_values = str_values + [str_values[-1].replace('<= ', '>  ')]
+            values += [str_values]
+        
+        # adding inf for the last quantiles
+        self.quantiles = {f: q + [inf] for f, q in self.quantiles.items()}
+
+        # creating the values orders based on quantiles
+        self.values_orders.update({feature: GroupedList(str_values) for feature, str_values in zip(self.features, values)})
+
+        return self
+    
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        
+        # copying dataset if requested
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+        
+        # iterating over each feature
+        for n, feature in enumerate(self.features):
+
+            # verbose if requested
+            if self.verbose:
+                print(f" - [QuantileDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
+
+            nans = isna(Xc[feature])  # keeping track of nans
+
+            # grouping values inside quantiles
+            to_input = [Xc[feature] <= q for q in self.quantiles.get(feature)]  # values that will be imputed
+            values = [[v] * len(X) for v in self.values_orders.get(feature)]  # new values to imput
+            Xc[feature] = select(to_input, values, default=Xc[feature])  # grouping modalities
+
+            # adding back nans
+            if any(nans):
+                Xc.loc[nans, feature] = nan
+        
+        return Xc
+
+class ClosestDiscretizer(BaseEstimator, TransformerMixin):
+    
+    def __init__(self, values_orders: Dict[str, Any], min_freq: float, *, default: str='worst', copy: bool=False, verbose: bool=False):
+        """ Discretizes ordered qualitative features into groups more frequent than min_freq"""
+        
+        self.features = list(values_orders.keys())
+        self.min_freq = min_freq
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.default = default[:]
+        self.default_values: Dict[str, Any] = {}
+        self.copy = copy
+        self.verbose = verbose
+
+    def fit(self, X: DataFrame, y: Series) -> None:
+        
+        # verbose
+        if self.verbose:
+            print(f" - [ClosestDiscretizer] Fit {', '.join(self.features)}")
+        
+        # grouping rare modalities for each feature
+        common_modalities = X[self.features].apply(
+            lambda u: find_common_modalities(u, y, self.min_freq, self.values_orders.get(u.name)), 
+            axis=0, result_type='expand'
+        ).T.to_dict()
+
+        # updating the order per feature
+        self.values_orders.update({f: common_modalities.get('order').get(f) for f in self.features})
+
+        # defining the default value based on the strategy
+        self.default_values = {f: common_modalities.get(self.default).get(f) for f in self.features}
+
+        return self
+    
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        
+        # copying dataset if requested
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+
+        # iterating over each feature
+        for n, feature in enumerate(self.features):
+
+            # printing verbose if requested
+            if self.verbose:
+                print(f" - [ClosestDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
+
+            # accessing feature's modalities' order
+            order = self.values_orders.get(feature)
+
+            # imputation des valeurs inconnues le cas échéant
+            unknowns = [value for value in Xc[feature].unique() if not any(is_equal(value, known) for known in order.values())]
+            unknowns = [value for value in unknowns if notna(value)]  # suppression des NaNs
+            if any(unknowns):
+                to_input = [Xc[feature] == unknown for unknown in unknowns]  # identification des valeurs à regrouper
+                Xc[feature] = select(to_input, [self.default_values.get(feature)], default=Xc[feature])  # regroupement des valeurs
+                warn(f"Unknown modalities provided for {feature}: {unknowns}")
+
+            # grouping values inside groups of modalities
+            to_discard = [order.get(group) for group in order]  # identification des valeur à regrouper
+            to_input = [Xc[feature].isin(discarded) for discarded in to_discard]  # identification des valeurs à regrouper
+            Xc[feature] = select(to_input, order, default=Xc[feature])  # regroupement des valeurs
+
+        return Xc
+
+def min_value_counts(x: Series, order: List[Any]) -> float:
+    """ Minimum of modalities' frequencies. """
+
+    # modality frequency
+    values = x.value_counts(dropna=False, normalize=True)
+    
+    # ignoring NaNs
+    values = values.drop(nan, errors='ignore')
+    
+    # adding missing modalities
+    values = values.reindex(order).fillna(0)
+    
+    # minimal frequency 
+    min_values = values.values.min()
+
+    return min_values
+
+def value_counts(x: Series, dropna: bool=False, normalize: bool=True) -> dict:
+    """ Counts the values of each modality of a series into a dictionnary"""
+    
+    values = x.value_counts(dropna=dropna, normalize=normalize)
+    
+    return values.to_dict()
+
+def target_rate(x: Series, y: Series, dropna: bool=True, ascending=True) -> dict:
+    """ Target y rate per modality of x into a dictionnary"""
+    
+    rates = y.groupby(x, dropna=dropna).mean().sort_values(ascending=ascending)
+    
+    return rates.to_dict()
+
+def nunique(x: Series, dropna=False) -> int:
+    """ Computes number of unique modalities"""
+    
+    uniques = unique(x)
+    n = len(uniques)
+    
+    # removing nans
+    if dropna:
+        if any(isna(uniques)):
+            n -= 1
+    
+    return n
+
+class DefaultDiscretizer(BaseEstimator, TransformerMixin):
+    
+    def __init__(
+        self, features: List[str], min_freq: float, *, 
+        values_orders: Dict[str, Any]={},
+        default_value: str='__OTHER__',
+        str_nan: str='__NAN__',
+        copy: bool=False, verbose: bool=False) -> None:
+        """ Groups a qualitative features' values less frequent than min_freq into a default_value"""
+        
+        self.features = features[:]
+        self.min_freq = min_freq
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.default_value = default_value[:]
+        self.str_nan = str_nan[:]
+        self.copy = copy
+        self.verbose = verbose
+
+    def fit(self, X: DataFrame, y: Series) -> None:
+
+        # filling up NaNs
+        Xc = X[self.features].fillna(self.str_nan)
+
+        # computing frequencies of each modality
+        frequencies = Xc.apply(value_counts, normalize=True, axis=0)
+
+        # computing ordered target rate per modality for ordering
+        target_rates = Xc.apply(target_rate, y=y, ascending=True, axis=0)
+
+        # attributing orders to each feature
+        self.values_orders.update({f: GroupedList(list(target_rates[f])) for f in self.features})
+        
+        # number of unique modality per feature
+        nuniques = Xc.apply(nunique, axis=0)
+            
+        # identifying modalities which are the most common
+        self.to_keep: Dict[str, Any] = {}  # dict of features and corresponding kept modalities
+
+        # iterating over each feature
+        for feature in self.features:
+
+            # checking for binary features
+            if nuniques[feature] > 2:
+                kept = [val for val, freq in frequencies[feature].items() if freq >= self.min_freq]
+
+            # keeping all modalities of binary features
+            else:
+                kept = [val for val, freq in frequencies[feature].items()]
+
+            self.to_keep.update({feature: kept})
+
+        # grouping rare modalities 
+        for n, feature in enumerate(self.features):
+
+        	# printing verbose
+            if self.verbose:
+                print(f" - [DefaultDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
+
+            # identifying values to discard (rare modalities)
+            to_discard = [value for value in self.values_orders[feature] if value not in self.to_keep[feature]]
+
+            # discarding rare modalities
+            if len(to_discard) > 0:
+
+                # adding default_value to possible values
+                order = self.values_orders[feature]
+                order.append(self.default_value)
+
+                # grouping rare modalities into default_value
+                order.group_list(to_discard, self.default_value)
+
+                # computing target rate for default value and reordering values according to feature's target rate
+                default_target_rate = y.loc[X[feature].isin(order.get(self.default_value))].mean()  # computing target rate for default value
+                order_target_rate = [target_rates.get(feature).get(value) for value in order if value != self.default_value]
+                default_position = next(n for n, trate in enumerate(order_target_rate + [inf]) if trate > default_target_rate)
+
+                # updating the modalities' order                
+                new_order = order[:-1][:default_position] + [self.default_value] + order[:-1][default_position:]  # getting rid of default value already in order
+                order = order.sort_by(new_order)
+                self.values_orders.update({feature: order})
+
+        return self
+
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+
+        # copying dataset if requested
+        Xc = X
+        if self.copy:
+            Xc = X.copy()
+
+        # filling up NaNs
+        Xc[self.features] = Xc[self.features].fillna(self.str_nan)
+
+        # grouping values inside groups of modalities
+        for n, feature in enumerate(self.features):
+
+            # verbose if requested
+            if self.verbose: 
+                print(f" - [DefaultDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
+
+            # grouping modalities
+            Xc[feature] = select([~Xc[feature].isin(self.to_keep[feature])], [self.default_value], default=Xc[feature])
+
+        return Xc
+
+
+
+def find_quantiles(df_feature: Series, q: int, len_df: int=None, quantiles: List[float]=None) -> List[float]:
+    """ Découpage en quantile de la feature.
+    
+    Fonction récursive : on prend l'échantillon et on cherche des valeurs sur-représentées
+    Si la valeur existe on la met dans une classe et on cherche à gauche et à droite de celle-ci, d'autres variables sur-représentées
+    Une fois il n'y a plus de valeurs qui soient sur-représentées,
+    on fait un découpage classique avec qcut en multipliant le nombre de classes souhaité par le pourcentage de valeurs restantes sur le total
+    
+    """
+
+    # initialisation de la taille total du dataframe
+    if len_df is None:
+        len_df = len(df_feature)
+    
+    # initialisation de la liste des quantiles
+    if quantiles is None:
+        quantiles = []
+
+    # calcul du nombre d'occurences de chaque valeur
+    frequencies = df_feature.value_counts(dropna=False, normalize=False).drop(nan, errors='ignore') / len_df # dropping nans to keep them anyways
+    values, frequencies = array(frequencies.index), array(frequencies.values)
+    
+    # cas 1 : il n'y a pas d'observation dans le dataframe
+    if len(df_feature) == 0:
+        
+        return quantiles
+    
+    # cas 2 : il y a des valeurs manquantes NaN
+    elif any(isna(df_feature)):
+        
+        return find_quantiles(df_feature[notna(df_feature)], q, len_df=len_df, quantiles=quantiles)
+        
+    # cas 2 : il n'y a que des valeurs dans le dataframe (pas de NaN)
+    else:
+        
+        # cas 1 : il existe une valeur sur-représentée
+        if any(frequencies > 1 / q):
+
+            # identification de la valeur sur-représentée
+            frequent_value = values[frequencies.argmax()]
+            
+            # ajout de la valeur fréquente à la liste des quantiles
+            quantiles += [frequent_value]
+
+            # calcul des quantiles pour les parties inférieures et supérieures
+            quantiles_inf = find_quantiles(df_feature[df_feature < frequent_value], q, len_df=len_df)
+            quantiles_sup = find_quantiles(df_feature[df_feature > frequent_value], q, len_df=len_df)
+            
+            return quantiles_inf + quantiles + quantiles_sup
+
+        # cas 2 : il n'existe pas de valeur sur-représentée
+        else:
+            
+            # nouveau nombre de quantile en prenant en compte les classes déjà constituées
+            new_q = max(round(len(df_feature) / len_df * q), 1)
+            
+            # calcul des quantiles sur le dataframe
+            if new_q > 1:
+                quantiles += list(quantile(df_feature.values, linspace(0, 1, new_q + 1)[1:-1], interpolation='lower'))
+
+            # case when there are no enough observations to compute quantiles
+            else:
+                quantiles += [max(df_feature.values)]
+
+            return quantiles
+
+def is_equal(a: Any, b: Any) -> bool:
+    """ checks if a and b are equal (NaN insensitive)"""
+    
+    # default equality
+    equal = a == b
+    
+    # Case where a and b are NaNs
+    if isna(a) and isna(b):
+        equal = True
+    
+    return equal
+
+def find_common_modalities(df_feature: Series, y: Series, min_freq: float, order: GroupedList, len_df: int=None) -> Dict[str, Any]:
+    """ Découpage en modalités de fréquence minimal (Cas des variables ordonnées).
+    
+    Fonction récursive : on prend l'échantillon et on cherche des valeurs sur-représentées
+    Si la valeur existe on la met dans une classe et on cherche à gauche et à droite de celle-ci, d'autres variables sur-représentées
+    Une fois il n'y a plus de valeurs qui soient sur-représentées,
+    on fait un découpage classique avec qcut en multipliant le nombre de classes souhaité par le pourcentage de valeurs restantes sur le total
+    
+    """
+
+    # initialisation de la taille totale du dataframe
+    if len_df is None:
+        len_df = len(df_feature)
+    
+    # conversion en GroupedList si ce n'est pas le cas 
+    order = GroupedList(order)
+    
+    # cas 1 : il y a des valeurs manquantes NaN
+    if any(isna(df_feature)):
+        
+        return find_common_modalities(df_feature[notna(df_feature)], y[notna(df_feature)], min_freq, order, len_df)
+
+
+    # cas 2 : il n'y a que des valeurs dans le dataframe (pas de NaN)
+    else:
+        
+        # computing frequencies and target rate of each modality
+        init_frequencies = df_feature.value_counts(dropna=False, normalize=False) / len_df
+        init_values, init_frequencies = init_frequencies.index, init_frequencies.values
+        
+        # ordering
+        frequencies = [init_frequencies[init_values == value][0] if any(init_values == value) else 0 for value in order]  # sort selon l'ordre des modalités
+        values = [init_values[init_values == value][0] if any(init_values == value) else value for value in order]  # sort selon l'ordre des modalités
+        target_rate = y.groupby(df_feature).sum().reindex(order) / frequencies / len_df # target rate per modality
+        underrepresented = [value for value, frequency in zip(values, frequencies) if frequency < min_freq]  # valeur peu fréquentes
+
+        # cas 1 : il existe une valeur sous-représentée
+        while any(underrepresented) & (len(frequencies) > 1):
+
+            # identification de la valeur sous-représentée
+            discarded_idx = argmin(frequencies)
+            discarded = values[discarded_idx]
+
+            # identification de la modalité la plus proche (volume et taux de défaut)
+            kept = find_closest_modality(discarded, discarded_idx, list(zip(order, frequencies, target_rate)), min_freq)
+
+            # removing the value from the initial ordering
+            order.group(discarded, kept)
+            
+            # ordering
+            frequencies = [init_frequencies[init_values == value][0] if any(init_values == value) else 0 for value in order]  # sort selon l'ordre des modalités
+            values = [init_values[init_values == value][0] if any(init_values == value) else value for value in order]  # sort selon l'ordre des modalités
+            target_rate = y.groupby(df_feature).sum().reindex(order) / frequencies / len_df # target rate per modality
+            underrepresented = [value for value, frequency in zip(values, frequencies) if frequency < min_freq]  # valeur peu fréquentes
+
+        worst, best = target_rate.idxmin(), target_rate.idxmax()
+
+        # cas 2 : il n'existe pas de valeur sous-représentée
+        return {'order': order, 'worst': worst, 'best': best}
+
+def find_closest_modality(value, idx: int, freq_target: Series, min_freq: float) -> int:
+    """HELPER Finds the closest modality in terms of frequency and target rate"""
+
+    # case 1: lowest modality
+    if idx == 0:
+        closest_modality = 1
+        
+    # case 2: biggest modality
+    elif idx == len(freq_target) - 1:
+        closest_modality = len(freq_target) - 2
+    
+    # case 3: not the lowwest nor the biggest modality
+    else:
+        # previous modality's volume and target rate
+        previous_value, previous_volume, previous_target = freq_target[idx - 1]
+        
+        # current modality's volume and target rate
+        _, volume, target = freq_target[idx]
+        
+        # next modality's volume and target rate
+        next_value, next_volume, next_target = freq_target[idx + 1]
+        
+        # regroupement par volumétrie (préféré s'il n'y a pas beaucoup de volume)
+        # case 1: la modalité suivante est inférieure à min_freq 
+        if next_volume < min_freq <= previous_volume:
+            closest_modality = idx + 1
+            
+        # case 2: la modalité précédante est inférieure à min_freq 
+        elif previous_volume < min_freq <= next_volume:
+            closest_modality = idx - 1
+            
+        # case 3: les deux modalités sont inférieures à min_freq 
+        elif (previous_volume < min_freq) & (next_volume < min_freq):
+            
+            # cas 1: la modalité précédante est inférieure à la modalité suivante
+            if previous_volume < next_volume:
+                closest_modality = idx - 1
+            
+            # cas 2: la modalité suivante est inférieure à la modalité précédante
+            elif next_volume < previous_volume:
+                closest_modality = idx + 1
+            
+            # cas 3: les deux modalités ont la même fréquence
+            else:
+                
+                # cas1: la modalité précédante est plus prorche en taux de cible
+                if abs(previous_target - target) <= abs(next_target - target):
+                    closest_modality = idx - 1
+                    
+                # cas2: la modalité précédante est plus prorche en taux de cible
+                else:
+                    closest_modality = idx + 1
+                
+        # case 4: les deux modalités sont supérieures à min_freq 
+        else:
+                
+            # cas1: la modalité précédante est plus prorche en taux de cible
+            if abs(previous_target - target) <= abs(next_target - target):
+                closest_modality = idx - 1
+
+            # cas2: la modalité précédante est plus prorche en taux de cible
+            else:
+                closest_modality = idx + 1
+    
+    # récupération de la valeur associée
+    closest_value = freq_target[closest_modality][0]
+    
+    return closest_value
+
+
+def format_list(a_list: List[float]) -> List[str]:
+    """ Formats a list of floats to a list of unique rounded strings of floats"""
+
+    # finding the closest power of thousands for each element
+    closest_powers = [next((k for k in range(-3, 4) if abs(elt) / 100 // 1000**(k) < 10)) for elt in a_list]
+
+    # rounding elements to the closest power of thousands
+    rounded_to_powers = [elt / 1000**(k) for elt, k in zip(a_list, closest_powers)]
+
+    # computing optimal decimal per unique power of thousands
+    optimal_decimals: Dict[str, int] = {}
+    for power in unique(closest_powers):  # iterating over each power of thousands found
+
+        # filtering on the specific power of thousands
+        sub_array = array([elt for elt, p in zip(rounded_to_powers, closest_powers) if power == p])
+
+        # number of distinct values
+        n_uniques = sub_array.shape[0]
+
+        # computing the first rounding decimal that allows for distinction of each values when rounded
+        # by default None (no rounding)
+        optimal_decimal = next((k for k in range(1, 10) if len(unique(sub_array.round(k))) == n_uniques), None)
+
+        # storing in the dict    
+        optimal_decimals.update({
+            power: optimal_decimal
+        })
+
+    # rounding according to each optimal_decimal
+    rounded_list: List[float] = []
+    for elt, power in zip(rounded_to_powers, closest_powers):
+
+        # rounding each element
+        rounded = elt  # by default None (no rounding)
+        optimal_decimal = optimal_decimals.get(power)
+        if optimal_decimal:  # checking that the optimal decimal exists
+            rounded = round(elt, optimal_decimal)
+
+        # adding the rounded number to the list
+        rounded_list += [rounded]
+
+    # dict of suffixes per power of thousands
+    suffixes = {
+        -3: 'n', -2: 'mi', -1: 'm', 0: '', 1: 'K', 2: 'M', 3: 'B'
+    }
+
+    # adding the suffixes
+    formatted_list = [f'{elt: 3.3f}{suffixes[power]}' for elt, power in zip(rounded_list, closest_powers)]
+    
+    # keeping zeros
+    formatted_list = [rounded if raw != 0 else f'{raw: 3.3f}' for rounded, raw in zip(formatted_list, a_list)]
+    
+    return formatted_list
```

### Comparing `AutoCarver-4.3.2/AutoCarver/FeatureSelector.py` & `AutoCarver-4.4.0/AutoCarver/FeatureSelector.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,752 +1,752 @@
-from IPython.display import display_html
-from math import sqrt
-from numpy import triu, ones, nan, inf
-from pandas import DataFrame, Series, notna, crosstab
-from random import shuffle
-from scipy.stats import kruskal, chi2_contingency
-from sklearn.base import BaseEstimator, TransformerMixin
-from statsmodels.formula.api import ols
-from statsmodels.stats.outliers_influence import variance_inflation_factor
-from typing import List, Dict, Any, Callable, Tuple
-
-
-class FeatureSelector(BaseEstimator, TransformerMixin):
-    """ A pipeline of measures to perform EDA and feature pre-selection
-     
-     - best features are the n_best of each measure
-     - selected features are stored in FeatureSelector.best_features
-        
-    Parameters
-    ----------
-    features: List[str]
-        Features on which to compute association.
-    n_best, int:
-        Number of features to be selected
-    sample_size: float, default 1.
-        Should be set between ]0, 1]
-        Size of sampled list of features speeds up computation. 
-        By default, all features are used. For sample_size=0.5,
-        FeatureSelector will search for the best features in 
-        features[:len(features)//2] and then in features[len(features)//2:]
-    measures, List[Callable]: default list().
-        List of association measures to be used.
-        Implemented measures are:
-            [Quantitative Features] 
-             - For association evaluation: `kruskal_measure`, `R_measure`
-             - For outlier detection: `zscore_measure`, `iqr_measure`
-            [Qualitative Features] 
-             - For correlation: `chi2_measure`, `cramerv_measure`, `tschuprowt_measure`
-        Ranks features based on last measure of the list.
-    filters, List[Callable]: default list().
-        List of filters to be used.
-        Implemented filters are:
-            [Quantitative Features] 
-             - For linear correlation: `spearman_filter`, `pearson_filter`
-             - For multicoloinearity: `vif_filter`
-            [Qualitative Features] 
-             - For correlation: `cramerv_filter`, `tschuprowt_filter`
-
-    Thresholds (to be passed as kwargs)
-    ----------
-    thresh_measure, float: default 0.
-        Minimum association between target and features
-        To be used with: `measure_filter`
-    name_measure, str
-        Measure to be used for minimum association filtering
-        To be used with: `measure_filter`
-    thresh_nan, float: default 1.
-        Maximum percentage of NaNs in a feature
-        To be used with: `nans_measure`
-    thresh_mode, float: default 1.
-        Maximum percentage of the mode of a feature
-        To be used with: `mode_measure`
-    thresh_outlier, float: default 1.
-        Maximum percentage of Outliers in a feature
-        To be used with: `iqr_measure`, `zscore_measure`
-    thresh_corr, float: default 1.
-        Maximum association between features
-        To be used with: `spearman_filter`, `pearson_filter`, `cramerv_filter`, `tschuprowt_filter`
-    thresh_vif, float: default inf
-        Maximum VIF between features
-        To be used with: `vif_filter`
-    ascending, bool default False
-        According to this measure:
-         - True: Lower values of the measure are to be considered as more associated to the target
-         - False: Higher values of the measure are to be considered as more associated to the target
-    """
-    
-    def __init__(self, features: List[str], n_best: int, measures: List[Callable]=list(), filters: List[Callable]=list(),
-                 sample_size: float=1., copy: bool=True, verbose: bool=True, **params) -> None:
-        
-        self.features = features[:]
-        self.n_best = n_best
-        assert n_best <= len(features), "Must set n_best <= len(features)"
-        self.best_features = features[:]
-        self.sample_size = sample_size
-        
-        self.measures = [dtype_measure, nans_measure, mode_measure] + measures[:]
-        self.filters = [thresh_filter] + filters[:]
-        self.sort_measures = [measure.__name__ for measure in measures[::-1]]
-
-        self.copy = copy
-        self.verbose = verbose
-        self.params = params
-    
-    def measure(self, x: Series, y: Series) -> Dict[str, Any]:
-        """ Measures association between x and y """
-        
-        passed = True  # measures keep going only if previous basic tests are passed
-        association = {}
-
-        # iterating over each measure
-        for measure in self.measures:
-            passed, association = measure(passed, association, x, y, **self.params)
-            
-        return association
-    
-    def measure_apply(self, X: DataFrame, y: Series, features: List[str]) -> None:
-        """ Measures association between columns of X and y
-
-    Parameters
-    ----------
-    ascending, bool default False
-        According to this measure:
-         - True: Lower values of the measure are to be considered as more associated to the target
-         - False: Higher values of the measure are to be considered as more associated to the target
-    """
-        
-        # applying association measure to each column
-        self.associations = X[features].apply(self.measure, y=y, result_type='expand', axis=0).T
-        
-        # filtering non association measure (pct_zscore, pct_iqr...)
-        asso_measures = [c for c in self.associations if '_measure' in c]
-        self.sort_measures = [c for c in self.sort_measures if c in asso_measures]
-        
-        # sorting statistics if an association measure was provided
-        self.associations = self.associations.sort_values(
-            self.sort_measures, ascending=self.params.get('ascending', False)
-        )
-    
-    def filter_apply(self, X: DataFrame, sort_measure: str) -> DataFrame:
-        """ Filters out too correlated features (least relevant first)
-
-    Parameters
-    ----------
-    ascending, bool default False
-        According to this measure:
-         - True: Lower values of the measure are to be considered as more associated to the target
-         - False: Higher values of the measure are to be considered as more associated to the target
-    """
-        
-        # ordering features by sort_by
-        self.filtered_associations = self.associations.sort_values(sort_measure, ascending=self.params.get('ascending', False))
-
-        # applying successive filters
-        for filtering in self.filters:
-
-            # ordered filtering
-            self.filtered_associations = filtering(X, self.filtered_associations, **self.params)
-    
-    def display_stats(self, association: DataFrame, caption: str) -> None:
-        """ EDA of fitted associations"""
-        
-        # appllying style 
-        subset = [c for c in association if 'pct_' in c or '_measure' in c or '_filter' in c]
-        style = association.style.background_gradient(cmap='coolwarm', subset=subset)
-        style = style.set_table_attributes("style='display:inline'")
-        style = style.set_caption(caption)
-        display_html(style._repr_html_(), raw=True)
-        
-    def fit_features(self, X: DataFrame, y: Series, features: List[str], n_best: int) -> List[str]:
-        """ Selects the n_best features amongst the specified ones"""
-        
-        # initial computation of all association measures
-        self.measure_apply(X, y, features)
-
-        # displaying association measure
-        if self.verbose:
-            self.display_stats(self.associations, 'Raw association')
-        
-        # iterating over each sort_measures 
-        # useful when measures hints to specific associations
-        ranks = []
-        for n, sort_measure in enumerate(self.sort_measures):
-            
-            # filtering by sort_measure
-            self.filter_apply(X, sort_measure)
-            ranks += [list(self.filtered_associations.index)]
-
-            # displaying filtered out association measure
-            if n == 0 and self.verbose and len(self.filters) > 1:
-                self.display_stats(self.filtered_associations, 'Filtered association')
-
-        # retrieving the n_best features per each ranking
-        best_features = []
-        if len(self.sort_measures) > 0:
-            best_features = [feature for rank in ranks for feature in rank[:n_best]]
-            best_features = list(set(best_features))  # deduplicating
-        
-        return best_features
-    
-    def fit(self, X: DataFrame, y: Series) -> None:
-        """ Selects the n_best features"""
-        
-        # splitting features in chunks
-        if self.sample_size < 1:
-            
-            # shuffling features to get random samples of features
-            shuffle(self.features)
-
-            # number of features per sample
-            chunks = int(len(self.features) // (1 / self.sample_size))
-
-            # splitting feature list in samples
-            feature_samples = [self.features[chunks * i: chunks * (i + 1)] for i in range(int(1 / self.sample_size)-1)]
-
-            # adding last sample with all remaining features
-            feature_samples += [self.features[chunks * (int(1 / self.sample_size) - 1):]]
-
-            # iterating over each feature samples
-            best_features = []
-            for features in feature_samples:
-
-                # fitting association on features
-                best_features += self.fit_features(X, y, features, int(self.n_best // 2))
-        
-        # splitting in chunks not requested
-        else:
-            best_features = self.features[:]
-        
-        # final selection with all best_features selected
-        self.best_features = self.fit_features(X, y, best_features, self.n_best)
-            
-        # dropped features
-        self.dropped_features = [c for c in self.features if c not in self.best_features]
-
-        return self
-
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-
-        # copying dataset
-        Xc = X
-        if self.copy:
-            Xc.copy()
-
-        # filtering out unwanted features
-        Xc = Xc.drop(self.dropped_features, axis=1)
-
-        return Xc
-
-
-# MEASURES
-def nans_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Measure of the percentage of NaNs
-
-    Parameters
-    ----------
-    thresh_nan, float: default 1.
-      Maximum percentage of NaNs in a feature
-    """
-    
-    # whether or not tests where passed
-    if active:
-    
-        nans = x.isnull()  # ckecking for nans
-        pct_nan = nans.mean()   # Computing percentage of nans
-    
-        # updating association
-        association.update({'pct_nan': pct_nan})
-    
-        # Excluding feature that have to many NaNs
-        active = pct_nan < params.get('thresh_nan', 1.)
-    
-    return active, association
-
-def dtype_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Gets dtype"""
-    
-    # updating association
-    association.update({'dtype': x.dtype})
-        
-    return active, association
-
-def mode_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Measure of the percentage of the Mode
-
-    Parameters
-    ----------
-    thresh_mode, float: default 1.
-      Maximum percentage of the mode of a feature
-    """
-    
-    # whether or not tests where passed
-    if active:
-    
-        mode = x.mode(dropna=True).values[0]  # computing mode
-        pct_mode = (x == mode).mean()  # Computing percentage of the mode
-    
-        # updating association
-        association.update({'pct_mode': pct_mode, 'mode': mode})
-    
-        # Excluding feature with too frequent modes
-        active = pct_mode < params.get('thresh_mode', 1.)
-    
-    return active, association
-
-def kruskal_measure(active: bool, association: Dict[str, Any], x: Series, y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Kruskal-Wallis statistic between x (quantitative) and y (binary)"""
-    
-    # check that previous steps where passed
-    if active:
-    
-        nans = x.isnull()  # ckecking for nans
-        
-        # computation of Kruskal-Wallis statistic
-        kw = kruskal(x[(~nans) & (y == 0)], x[(~nans) & (y == 1)])
-        
-        # updating association
-        if kw:
-            association.update({'kruskal_measure': kw[0]})
-        
-    return active, association
-
-def R_measure(active: bool, association: Dict[str, Any], x: Series, y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ R of the linear regression of x (quantitative) by y (binary)"""
-    
-    # check that previous steps where passed
-    if active:
-    
-        nans = x.isnull()  # ckecking for nans
-
-        # grouping feature and target
-        ols_df = DataFrame({'feature': x[~nans], 'target': y[~nans]})
-        
-        # fitting regression of feature by target
-        regression = ols('feature~C(target)', ols_df).fit()
-        
-        # updating association
-        if regression.rsquared:
-            if regression.rsquared >= 0:
-                association.update({'R_measure': sqrt(regression.rsquared)})
-            else:
-                association.update({'R_measure': nan})
-        
-    return active, association
-
-
-def zscore_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Computes outliers based on the z-score
-
-    Parameters
-    ----------
-    thresh_outlier, float: default 1.
-      Maximum percentage of Outliers in a feature
-    """
-    
-    # check that previous steps where passed for computational optimization
-    if active:
-        
-        mean = x.mean()  # mean of the feature
-        std = x.std()  # standard deviation of the feature
-        zscore = (x-mean) / std  # zscore per observation
-        
-        # checking for outliers
-        outliers = abs(zscore) > 3
-        pct_zscore = outliers.mean()
-        
-        # updating association
-        association.update({
-            'pct_zscore': pct_zscore,
-            'min': x.min(),
-            'max': x.max(),
-            'mean': mean,
-            'std': std
-        })
-
-        # Excluding feature with too frequent modes
-        active = pct_zscore < params.get('thresh_outlier', 1.)
-        
-    return active, association
-
-def iqr_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Computes outliers based on the inter-quartile range
-
-    Parameters
-    ----------
-    thresh_outlier, float: default 1.
-      Maximum percentage of Outliers in a feature
-    """
-    
-    # check that previous steps where passed for computational optimization
-    if active:
-        
-        q3 = x.quantile(0.75)  # 3rd quartile
-        q1 = x.quantile(0.25)  # 1st quartile
-        iqr = q3 - q1  # inter quartile range
-        iqr_bounds = q1 - 1.5 * iqr, q3 + 1.5 * iqr  # bounds of the iqr range
-        
-        # checking for outliers
-        outliers = ~x.between(*iqr_bounds)
-        pct_iqr = outliers.mean()
-        
-        # updating association
-        association.update({
-            'pct_iqr': pct_iqr,
-            'q1': q1,
-            'median': x.median(),
-            'q3': q3
-        })
-
-        # Excluding feature with too frequent modes
-        active = pct_iqr < params.get('thresh_outlier', 1.)
-        
-    return active, association
-
-def chi2_measure(active: bool, association: Dict[str, Any], x: Series,
-                 y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Chi2 Measure between two Series of qualitative features"""
-        
-    # check that previous steps where passed
-    if active:
-    
-        # computing crosstab between x and y
-        xtab = crosstab(x, y)
-
-        # numnber of observations
-        n_obs = xtab.sum(axis=None)
-
-        # number of values taken by the features
-        n_mod_x, n_mod_y = len(xtab.index), len(xtab.columns)
-
-        # Chi2 statistic
-        chi2 = chi2_contingency(xtab)[0]
-
-        # updating association
-        association.update({'chi2_measure': chi2})
-    
-    return active, association
-
-def cramerv_measure(active: bool, association: Dict[str, Any], x: Series,
-                    y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Carmer's V between two Series of qualitative features"""
-
-    # check that previous steps where passed
-    if active:
-    
-        # computing chi2
-        if 'chi2_measure' not in association:
-            active, association = chi2_measure(active, association, x, y, **params)
-
-        # numnber of observations
-        n_obs = (notna(x) & notna(y)).sum()
-
-        # number of values taken by the features
-        n_mod_x, n_mod_y = x.nunique(), y.nunique()
-        min_n_mod = min(n_mod_x, n_mod_y)
-        
-        # Chi2 statistic
-        chi2 = association.get('chi2_measure')
-
-        # Cramer's V
-        cramerv = sqrt(chi2 / n_obs / (min_n_mod - 1))
-
-        # updating association
-        association.update({'cramerv_measure': cramerv})
-    
-    return active, association
-
-def tschuprowt_measure(active: bool, association: Dict[str, Any],x: Series,
-                       y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Tschuprow's T between two Series of qualitative features"""
-        
-    # check that previous steps where passed
-    if active:
-    
-        # computing chi2
-        if 'chi2_measure' not in association:
-            active, association = chi2_measure(active, association, x, y, **params)
-
-        # numnber of observations
-        n_obs = (notna(x) & notna(y)).sum()
-
-        # number of values taken by the features
-        n_mod_x, n_mod_y = x.nunique(), y.nunique()
-        
-        # Chi2 statistic
-        chi2 = association.get('chi2_measure')
-
-        # Tschuprow's T
-        dof_mods = sqrt((n_mod_x - 1) * (n_mod_y - 1))
-        tschuprowt = 0
-        if dof_mods > 0:
-            tschuprowt = sqrt(chi2 / n_obs / dof_mods)
-
-        # updating association
-        association.update({'tschuprowt_measure': tschuprowt})
-    
-    return active, association
-
-    
-# FILTERS 
-def thresh_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Filters out missing association measure (did not pass a threshold)"""
-    
-    # drops rows with nans
-    associations = ranks.dropna(axis=0)
-    
-    return associations
-
-def measure_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Filters out specified measure's lower ranks than threshold
-
-    Parameters
-    ----------
-    thresh_measure, float: default 0.
-        Minimum association between target and features
-        To be used with: `association_filter`
-    name_measure, str
-        Measure to be used for minimum association filtering
-        To be used with: `association_filter`
-    """
-    
-    associations = ranks.copy()
-
-    # drops rows with nans
-    if 'name_measure' in params:
-        associations = ranks[ranks[params.get('name_measure')] > params.get('thresh_measure', 0.)]
-    
-    return associations
-
-def quantitative_filter(X: DataFrame, ranks: DataFrame, corr_measure: str, **params) -> Dict[str, Any]:
-    """ Computes max association between X and X (quantitative) excluding features 
-    that are correlated to a feature more associated with the target 
-    (defined by the ranks).
-
-    Parameters
-    ----------
-    thresh_corr, float: default 1.
-        Maximum association between features
-    """
-    
-    # accessing the prefered order
-    prefered_order = ranks.index
-
-    # computing correlation between features
-    X_corr = X[prefered_order].corr(corr_measure).abs()
-    X_corr = X_corr.where(triu(ones(X_corr.shape), k=1).astype(bool))
-    
-    # initiating list of maximum association per feature
-    associations = []
-    
-    # iterating over each feature by target association order
-    for feature in prefered_order:
-            
-        # correlation with features more associated to the target
-        corr_with_better_features = X_corr.loc[:feature, feature]
-        
-        # maximum correlation with a better feature
-        corr_with, worst_corr = corr_with_better_features.agg(['idxmax', 'max'])
-        
-        # dropping the feature if it was too correlated to a better feature
-        if worst_corr > params.get('thresh_corr', 1):
-            X_corr = X_corr.drop(feature, axis=0).drop(feature, axis=1)
-            
-        # kept feature: updating associations with this feature
-        else:
-            associations += [{
-                'feature': feature, 
-                f'{corr_measure}_filter': worst_corr,
-                f'{corr_measure}_with': corr_with
-            }]
-            
-    # formatting ouput to DataFrame
-    associations = DataFrame(associations).set_index('feature')
-            
-    # applying filter on association
-    associations = ranks.join(associations, how='right')
-    
-    return associations 
-
-
-def spearman_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Computes max Spearman between X and X (quantitative) excluding features 
-    that are correlated to a feature more associated with the target 
-    (defined by the ranks).
-
-    Parameters
-    ----------
-    thresh_corr, float: default 1.
-      Maximum association between features
-    """
-            
-    # applying quantitative filter with spearman correlation
-    return quantitative_filter(X, ranks, 'spearman', **params)
-
-def pearson_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Computes max Pearson between X and X (quantitative) excluding features 
-    that are correlated to a feature more associated with the target 
-    (defined by the ranks).
-
-    Parameters
-    ----------
-    thresh_corr, float: default 1.
-      Maximum association between features
-    """
-            
-    # applying quantitative filter with spearman correlation
-    return quantitative_filter(X, ranks, 'pearson', **params)
-
-def vif_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Computes Variance Inflation Factor (multicolinearity)
-
-    Parameters
-    ----------
-    thresh_vif, float: default inf
-      Maximum VIF between features
-    """
-    
-    # accessing the prefered order
-    prefered_order = ranks.index
-    
-    # initiating list association per feature
-    associations = []
-    
-    # list of dropped features
-    dropped = []
-    
-    # iterating over each column
-    for i, feature in enumerate(prefered_order):
-        
-        # identifying remaining more associated features
-        better_features = [f for f in prefered_order[:i+1] if f not in dropped]
-        
-        X_vif = X[better_features]  # keeping only better features
-        X_vif = X_vif.dropna(axis=0)  # dropping NaNs for OLS
-        
-        # computation of VIF
-        vif = nan
-        if len(better_features) > 1 and len(X_vif) > 0:
-            vif = variance_inflation_factor(X_vif.values, len(better_features)-1)
-        
-        # dropping the feature if it was too correlated to a better feature
-        if vif > params.get('thresh_vif', inf) and notna(vif):
-            dropped += [feature]
-            
-        # kept feature: updating associations with this feature
-        else:
-            associations += [{'feature': feature, 'vif_filter': vif}]
-    
-    # formatting ouput to DataFrame
-    associations = DataFrame(associations).set_index('feature')
-            
-    # applying filter on association
-    associations = ranks.join(associations, how='right')
-    
-    return associations
-
-def qualitative_worst_corr(X: DataFrame, feature: str, ranks: DataFrame, corr_measure: Callable, **params):
-    """ Computes maximum association between a feature and features 
-    more associated to the target (according to ranks)
-    """
-    
-    # measure name
-    measure_name = corr_measure.__name__
-    measure = measure_name.replace('_measure', '')
-        
-    # initiating worst correlation
-    worst_corr = {'feature': feature}
-    
-    # features more associated with target
-    better_features = list(ranks.loc[:feature].index)[:-1]
-
-    # iterating over each better feature
-    for better_feature in better_features:
-
-        # computing association with better feature
-        _, association = corr_measure(True, {f'{measure}_with': better_feature}, 
-                                      X[feature], X[better_feature], **params)
-
-
-        # updating association if it's greater than previous better features
-        if association.get(measure_name) > worst_corr.get(measure_name, 0):
-
-            # renaming association measure as filter
-            association[f'{measure}_filter'] = association.pop(measure_name)
-            
-            # removing temporary measures
-            association = {k: v for k, v in association.items() if '_measure' not in k}
-
-            # updating worst known association
-            worst_corr.update(association)
-
-        # stopping measurements if association is greater than threshold
-        if association.get(f'{measure}_filter') > params.get('thresh_corr', 1):
-            ranks = ranks.drop(feature, axis=0)  # removing feature from ranks
-            
-            return ranks, None
-    
-    return ranks, worst_corr
-
-def qualitative_filter(X: DataFrame, ranks: DataFrame, corr_measure: Callable, **params) -> Dict[str, Any]:
-    """ Computes max association between X and X (qualitative) excluding features 
-    that are correlated to a feature more associated with the target 
-    (defined by the ranks).
-
-    Parameters
-    ----------
-    thresh_corr, float: default 1.
-        Maximum association between features
-    """
-    
-    # accessing the prefered order
-    prefered_order = ranks.index
-
-    # initiating list of maximum association per feature
-    associations = []
-    
-    # iterating over each feature by target association order
-    for feature in prefered_order:
-        
-        
-        # computing correlation with better features anf filtering out ranks
-        ranks, worst_corr = qualitative_worst_corr(X, feature, ranks, corr_measure, **params)
-        
-        # updating associations
-        if worst_corr:
-            associations += [worst_corr]
-
-    # formatting ouput to DataFrame
-    associations = DataFrame(associations).set_index('feature')
-            
-    # applying filter on association
-    associations = ranks.join(associations, how='right')
-    
-    return associations 
-
-def cramerv_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Computes max Cramer's V between X and X (qualitative) excluding features 
-    that are correlated to a feature more associated with the target 
-    (defined by the ranks).
-
-    Parameters
-    ----------
-    thresh_corr, float: default 1.
-        Maximum association between features
-    """
-            
-    # applying quantitative filter with Cramer's V correlation    
-    return qualitative_filter(X, ranks, cramerv_measure, **params)
-
-def tschuprowt_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Computes max Tschuprow's T between X and X (qualitative) excluding features 
-    that are correlated to a feature more associated with the target 
-    (defined by the ranks).
-
-    Parameters
-    ----------
-    thresh_corr, float: default 1.
-        Maximum association between features
-    """
-            
-    # applying quantitative filter with Tschuprow's T correlation
-    return qualitative_filter(X, ranks, tschuprowt_measure, **params)
+from IPython.display import display_html
+from math import sqrt
+from numpy import triu, ones, nan, inf
+from pandas import DataFrame, Series, notna, crosstab
+from random import shuffle
+from scipy.stats import kruskal, chi2_contingency
+from sklearn.base import BaseEstimator, TransformerMixin
+from statsmodels.formula.api import ols
+from statsmodels.stats.outliers_influence import variance_inflation_factor
+from typing import List, Dict, Any, Callable, Tuple
+
+
+class FeatureSelector(BaseEstimator, TransformerMixin):
+    """ A pipeline of measures to perform EDA and feature pre-selection
+     
+     - best features are the n_best of each measure
+     - selected features are stored in FeatureSelector.best_features
+        
+    Parameters
+    ----------
+    features: List[str]
+        Features on which to compute association.
+    n_best, int:
+        Number of features to be selected
+    sample_size: float, default 1.
+        Should be set between ]0, 1]
+        Size of sampled list of features speeds up computation. 
+        By default, all features are used. For sample_size=0.5,
+        FeatureSelector will search for the best features in 
+        features[:len(features)//2] and then in features[len(features)//2:]
+    measures, List[Callable]: default list().
+        List of association measures to be used.
+        Implemented measures are:
+            [Quantitative Features] 
+             - For association evaluation: `kruskal_measure`, `R_measure`
+             - For outlier detection: `zscore_measure`, `iqr_measure`
+            [Qualitative Features] 
+             - For correlation: `chi2_measure`, `cramerv_measure`, `tschuprowt_measure`
+        Ranks features based on last measure of the list.
+    filters, List[Callable]: default list().
+        List of filters to be used.
+        Implemented filters are:
+            [Quantitative Features] 
+             - For linear correlation: `spearman_filter`, `pearson_filter`
+             - For multicoloinearity: `vif_filter`
+            [Qualitative Features] 
+             - For correlation: `cramerv_filter`, `tschuprowt_filter`
+
+    Thresholds (to be passed as kwargs)
+    ----------
+    thresh_measure, float: default 0.
+        Minimum association between target and features
+        To be used with: `measure_filter`
+    name_measure, str
+        Measure to be used for minimum association filtering
+        To be used with: `measure_filter`
+    thresh_nan, float: default 1.
+        Maximum percentage of NaNs in a feature
+        To be used with: `nans_measure`
+    thresh_mode, float: default 1.
+        Maximum percentage of the mode of a feature
+        To be used with: `mode_measure`
+    thresh_outlier, float: default 1.
+        Maximum percentage of Outliers in a feature
+        To be used with: `iqr_measure`, `zscore_measure`
+    thresh_corr, float: default 1.
+        Maximum association between features
+        To be used with: `spearman_filter`, `pearson_filter`, `cramerv_filter`, `tschuprowt_filter`
+    thresh_vif, float: default inf
+        Maximum VIF between features
+        To be used with: `vif_filter`
+    ascending, bool default False
+        According to this measure:
+         - True: Lower values of the measure are to be considered as more associated to the target
+         - False: Higher values of the measure are to be considered as more associated to the target
+    """
+    
+    def __init__(self, features: List[str], n_best: int, measures: List[Callable]=list(), filters: List[Callable]=list(),
+                 sample_size: float=1., copy: bool=True, verbose: bool=True, **params) -> None:
+        
+        self.features = features[:]
+        self.n_best = n_best
+        assert n_best <= len(features), "Must set n_best <= len(features)"
+        self.best_features = features[:]
+        self.sample_size = sample_size
+        
+        self.measures = [dtype_measure, nans_measure, mode_measure] + measures[:]
+        self.filters = [thresh_filter] + filters[:]
+        self.sort_measures = [measure.__name__ for measure in measures[::-1]]
+
+        self.copy = copy
+        self.verbose = verbose
+        self.params = params
+    
+    def measure(self, x: Series, y: Series) -> Dict[str, Any]:
+        """ Measures association between x and y """
+        
+        passed = True  # measures keep going only if previous basic tests are passed
+        association = {}
+
+        # iterating over each measure
+        for measure in self.measures:
+            passed, association = measure(passed, association, x, y, **self.params)
+            
+        return association
+    
+    def measure_apply(self, X: DataFrame, y: Series, features: List[str]) -> None:
+        """ Measures association between columns of X and y
+
+    Parameters
+    ----------
+    ascending, bool default False
+        According to this measure:
+         - True: Lower values of the measure are to be considered as more associated to the target
+         - False: Higher values of the measure are to be considered as more associated to the target
+    """
+        
+        # applying association measure to each column
+        self.associations = X[features].apply(self.measure, y=y, result_type='expand', axis=0).T
+        
+        # filtering non association measure (pct_zscore, pct_iqr...)
+        asso_measures = [c for c in self.associations if '_measure' in c]
+        self.sort_measures = [c for c in self.sort_measures if c in asso_measures]
+        
+        # sorting statistics if an association measure was provided
+        self.associations = self.associations.sort_values(
+            self.sort_measures, ascending=self.params.get('ascending', False)
+        )
+    
+    def filter_apply(self, X: DataFrame, sort_measure: str) -> DataFrame:
+        """ Filters out too correlated features (least relevant first)
+
+    Parameters
+    ----------
+    ascending, bool default False
+        According to this measure:
+         - True: Lower values of the measure are to be considered as more associated to the target
+         - False: Higher values of the measure are to be considered as more associated to the target
+    """
+        
+        # ordering features by sort_by
+        self.filtered_associations = self.associations.sort_values(sort_measure, ascending=self.params.get('ascending', False))
+
+        # applying successive filters
+        for filtering in self.filters:
+
+            # ordered filtering
+            self.filtered_associations = filtering(X, self.filtered_associations, **self.params)
+    
+    def display_stats(self, association: DataFrame, caption: str) -> None:
+        """ EDA of fitted associations"""
+        
+        # appllying style 
+        subset = [c for c in association if 'pct_' in c or '_measure' in c or '_filter' in c]
+        style = association.style.background_gradient(cmap='coolwarm', subset=subset)
+        style = style.set_table_attributes("style='display:inline'")
+        style = style.set_caption(caption)
+        display_html(style._repr_html_(), raw=True)
+        
+    def fit_features(self, X: DataFrame, y: Series, features: List[str], n_best: int) -> List[str]:
+        """ Selects the n_best features amongst the specified ones"""
+        
+        # initial computation of all association measures
+        self.measure_apply(X, y, features)
+
+        # displaying association measure
+        if self.verbose:
+            self.display_stats(self.associations, 'Raw association')
+        
+        # iterating over each sort_measures 
+        # useful when measures hints to specific associations
+        ranks = []
+        for n, sort_measure in enumerate(self.sort_measures):
+            
+            # filtering by sort_measure
+            self.filter_apply(X, sort_measure)
+            ranks += [list(self.filtered_associations.index)]
+
+            # displaying filtered out association measure
+            if n == 0 and self.verbose and len(self.filters) > 1:
+                self.display_stats(self.filtered_associations, 'Filtered association')
+
+        # retrieving the n_best features per each ranking
+        best_features = []
+        if len(self.sort_measures) > 0:
+            best_features = [feature for rank in ranks for feature in rank[:n_best]]
+            best_features = list(set(best_features))  # deduplicating
+        
+        return best_features
+    
+    def fit(self, X: DataFrame, y: Series) -> None:
+        """ Selects the n_best features"""
+        
+        # splitting features in chunks
+        if self.sample_size < 1:
+            
+            # shuffling features to get random samples of features
+            shuffle(self.features)
+
+            # number of features per sample
+            chunks = int(len(self.features) // (1 / self.sample_size))
+
+            # splitting feature list in samples
+            feature_samples = [self.features[chunks * i: chunks * (i + 1)] for i in range(int(1 / self.sample_size)-1)]
+
+            # adding last sample with all remaining features
+            feature_samples += [self.features[chunks * (int(1 / self.sample_size) - 1):]]
+
+            # iterating over each feature samples
+            best_features = []
+            for features in feature_samples:
+
+                # fitting association on features
+                best_features += self.fit_features(X, y, features, int(self.n_best // 2))
+        
+        # splitting in chunks not requested
+        else:
+            best_features = self.features[:]
+        
+        # final selection with all best_features selected
+        self.best_features = self.fit_features(X, y, best_features, self.n_best)
+            
+        # dropped features
+        self.dropped_features = [c for c in self.features if c not in self.best_features]
+
+        return self
+
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+
+        # copying dataset
+        Xc = X
+        if self.copy:
+            Xc.copy()
+
+        # filtering out unwanted features
+        Xc = Xc.drop(self.dropped_features, axis=1)
+
+        return Xc
+
+
+# MEASURES
+def nans_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Measure of the percentage of NaNs
+
+    Parameters
+    ----------
+    thresh_nan, float: default 1.
+      Maximum percentage of NaNs in a feature
+    """
+    
+    # whether or not tests where passed
+    if active:
+    
+        nans = x.isnull()  # ckecking for nans
+        pct_nan = nans.mean()   # Computing percentage of nans
+    
+        # updating association
+        association.update({'pct_nan': pct_nan})
+    
+        # Excluding feature that have to many NaNs
+        active = pct_nan < params.get('thresh_nan', 1.)
+    
+    return active, association
+
+def dtype_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Gets dtype"""
+    
+    # updating association
+    association.update({'dtype': x.dtype})
+        
+    return active, association
+
+def mode_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Measure of the percentage of the Mode
+
+    Parameters
+    ----------
+    thresh_mode, float: default 1.
+      Maximum percentage of the mode of a feature
+    """
+    
+    # whether or not tests where passed
+    if active:
+    
+        mode = x.mode(dropna=True).values[0]  # computing mode
+        pct_mode = (x == mode).mean()  # Computing percentage of the mode
+    
+        # updating association
+        association.update({'pct_mode': pct_mode, 'mode': mode})
+    
+        # Excluding feature with too frequent modes
+        active = pct_mode < params.get('thresh_mode', 1.)
+    
+    return active, association
+
+def kruskal_measure(active: bool, association: Dict[str, Any], x: Series, y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Kruskal-Wallis statistic between x (quantitative) and y (binary)"""
+    
+    # check that previous steps where passed
+    if active:
+    
+        nans = x.isnull()  # ckecking for nans
+        
+        # computation of Kruskal-Wallis statistic
+        kw = kruskal(x[(~nans) & (y == 0)], x[(~nans) & (y == 1)])
+        
+        # updating association
+        if kw:
+            association.update({'kruskal_measure': kw[0]})
+        
+    return active, association
+
+def R_measure(active: bool, association: Dict[str, Any], x: Series, y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ R of the linear regression of x (quantitative) by y (binary)"""
+    
+    # check that previous steps where passed
+    if active:
+    
+        nans = x.isnull()  # ckecking for nans
+
+        # grouping feature and target
+        ols_df = DataFrame({'feature': x[~nans], 'target': y[~nans]})
+        
+        # fitting regression of feature by target
+        regression = ols('feature~C(target)', ols_df).fit()
+        
+        # updating association
+        if regression.rsquared:
+            if regression.rsquared >= 0:
+                association.update({'R_measure': sqrt(regression.rsquared)})
+            else:
+                association.update({'R_measure': nan})
+        
+    return active, association
+
+
+def zscore_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Computes outliers based on the z-score
+
+    Parameters
+    ----------
+    thresh_outlier, float: default 1.
+      Maximum percentage of Outliers in a feature
+    """
+    
+    # check that previous steps where passed for computational optimization
+    if active:
+        
+        mean = x.mean()  # mean of the feature
+        std = x.std()  # standard deviation of the feature
+        zscore = (x-mean) / std  # zscore per observation
+        
+        # checking for outliers
+        outliers = abs(zscore) > 3
+        pct_zscore = outliers.mean()
+        
+        # updating association
+        association.update({
+            'pct_zscore': pct_zscore,
+            'min': x.min(),
+            'max': x.max(),
+            'mean': mean,
+            'std': std
+        })
+
+        # Excluding feature with too frequent modes
+        active = pct_zscore < params.get('thresh_outlier', 1.)
+        
+    return active, association
+
+def iqr_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Computes outliers based on the inter-quartile range
+
+    Parameters
+    ----------
+    thresh_outlier, float: default 1.
+      Maximum percentage of Outliers in a feature
+    """
+    
+    # check that previous steps where passed for computational optimization
+    if active:
+        
+        q3 = x.quantile(0.75)  # 3rd quartile
+        q1 = x.quantile(0.25)  # 1st quartile
+        iqr = q3 - q1  # inter quartile range
+        iqr_bounds = q1 - 1.5 * iqr, q3 + 1.5 * iqr  # bounds of the iqr range
+        
+        # checking for outliers
+        outliers = ~x.between(*iqr_bounds)
+        pct_iqr = outliers.mean()
+        
+        # updating association
+        association.update({
+            'pct_iqr': pct_iqr,
+            'q1': q1,
+            'median': x.median(),
+            'q3': q3
+        })
+
+        # Excluding feature with too frequent modes
+        active = pct_iqr < params.get('thresh_outlier', 1.)
+        
+    return active, association
+
+def chi2_measure(active: bool, association: Dict[str, Any], x: Series,
+                 y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Chi2 Measure between two Series of qualitative features"""
+        
+    # check that previous steps where passed
+    if active:
+    
+        # computing crosstab between x and y
+        xtab = crosstab(x, y)
+
+        # numnber of observations
+        n_obs = xtab.sum(axis=None)
+
+        # number of values taken by the features
+        n_mod_x, n_mod_y = len(xtab.index), len(xtab.columns)
+
+        # Chi2 statistic
+        chi2 = chi2_contingency(xtab)[0]
+
+        # updating association
+        association.update({'chi2_measure': chi2})
+    
+    return active, association
+
+def cramerv_measure(active: bool, association: Dict[str, Any], x: Series,
+                    y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Carmer's V between two Series of qualitative features"""
+
+    # check that previous steps where passed
+    if active:
+    
+        # computing chi2
+        if 'chi2_measure' not in association:
+            active, association = chi2_measure(active, association, x, y, **params)
+
+        # numnber of observations
+        n_obs = (notna(x) & notna(y)).sum()
+
+        # number of values taken by the features
+        n_mod_x, n_mod_y = x.nunique(), y.nunique()
+        min_n_mod = min(n_mod_x, n_mod_y)
+        
+        # Chi2 statistic
+        chi2 = association.get('chi2_measure')
+
+        # Cramer's V
+        cramerv = sqrt(chi2 / n_obs / (min_n_mod - 1))
+
+        # updating association
+        association.update({'cramerv_measure': cramerv})
+    
+    return active, association
+
+def tschuprowt_measure(active: bool, association: Dict[str, Any],x: Series,
+                       y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Tschuprow's T between two Series of qualitative features"""
+        
+    # check that previous steps where passed
+    if active:
+    
+        # computing chi2
+        if 'chi2_measure' not in association:
+            active, association = chi2_measure(active, association, x, y, **params)
+
+        # numnber of observations
+        n_obs = (notna(x) & notna(y)).sum()
+
+        # number of values taken by the features
+        n_mod_x, n_mod_y = x.nunique(), y.nunique()
+        
+        # Chi2 statistic
+        chi2 = association.get('chi2_measure')
+
+        # Tschuprow's T
+        dof_mods = sqrt((n_mod_x - 1) * (n_mod_y - 1))
+        tschuprowt = 0
+        if dof_mods > 0:
+            tschuprowt = sqrt(chi2 / n_obs / dof_mods)
+
+        # updating association
+        association.update({'tschuprowt_measure': tschuprowt})
+    
+    return active, association
+
+    
+# FILTERS 
+def thresh_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+    """ Filters out missing association measure (did not pass a threshold)"""
+    
+    # drops rows with nans
+    associations = ranks.dropna(axis=0)
+    
+    return associations
+
+def measure_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+    """ Filters out specified measure's lower ranks than threshold
+
+    Parameters
+    ----------
+    thresh_measure, float: default 0.
+        Minimum association between target and features
+        To be used with: `association_filter`
+    name_measure, str
+        Measure to be used for minimum association filtering
+        To be used with: `association_filter`
+    """
+    
+    associations = ranks.copy()
+
+    # drops rows with nans
+    if 'name_measure' in params:
+        associations = ranks[ranks[params.get('name_measure')] > params.get('thresh_measure', 0.)]
+    
+    return associations
+
+def quantitative_filter(X: DataFrame, ranks: DataFrame, corr_measure: str, **params) -> Dict[str, Any]:
+    """ Computes max association between X and X (quantitative) excluding features 
+    that are correlated to a feature more associated with the target 
+    (defined by the ranks).
+
+    Parameters
+    ----------
+    thresh_corr, float: default 1.
+        Maximum association between features
+    """
+    
+    # accessing the prefered order
+    prefered_order = ranks.index
+
+    # computing correlation between features
+    X_corr = X[prefered_order].corr(corr_measure).abs()
+    X_corr = X_corr.where(triu(ones(X_corr.shape), k=1).astype(bool))
+    
+    # initiating list of maximum association per feature
+    associations = []
+    
+    # iterating over each feature by target association order
+    for feature in prefered_order:
+            
+        # correlation with features more associated to the target
+        corr_with_better_features = X_corr.loc[:feature, feature]
+        
+        # maximum correlation with a better feature
+        corr_with, worst_corr = corr_with_better_features.agg(['idxmax', 'max'])
+        
+        # dropping the feature if it was too correlated to a better feature
+        if worst_corr > params.get('thresh_corr', 1):
+            X_corr = X_corr.drop(feature, axis=0).drop(feature, axis=1)
+            
+        # kept feature: updating associations with this feature
+        else:
+            associations += [{
+                'feature': feature, 
+                f'{corr_measure}_filter': worst_corr,
+                f'{corr_measure}_with': corr_with
+            }]
+            
+    # formatting ouput to DataFrame
+    associations = DataFrame(associations).set_index('feature')
+            
+    # applying filter on association
+    associations = ranks.join(associations, how='right')
+    
+    return associations 
+
+
+def spearman_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+    """ Computes max Spearman between X and X (quantitative) excluding features 
+    that are correlated to a feature more associated with the target 
+    (defined by the ranks).
+
+    Parameters
+    ----------
+    thresh_corr, float: default 1.
+      Maximum association between features
+    """
+            
+    # applying quantitative filter with spearman correlation
+    return quantitative_filter(X, ranks, 'spearman', **params)
+
+def pearson_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+    """ Computes max Pearson between X and X (quantitative) excluding features 
+    that are correlated to a feature more associated with the target 
+    (defined by the ranks).
+
+    Parameters
+    ----------
+    thresh_corr, float: default 1.
+      Maximum association between features
+    """
+            
+    # applying quantitative filter with spearman correlation
+    return quantitative_filter(X, ranks, 'pearson', **params)
+
+def vif_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+    """ Computes Variance Inflation Factor (multicolinearity)
+
+    Parameters
+    ----------
+    thresh_vif, float: default inf
+      Maximum VIF between features
+    """
+    
+    # accessing the prefered order
+    prefered_order = ranks.index
+    
+    # initiating list association per feature
+    associations = []
+    
+    # list of dropped features
+    dropped = []
+    
+    # iterating over each column
+    for i, feature in enumerate(prefered_order):
+        
+        # identifying remaining more associated features
+        better_features = [f for f in prefered_order[:i+1] if f not in dropped]
+        
+        X_vif = X[better_features]  # keeping only better features
+        X_vif = X_vif.dropna(axis=0)  # dropping NaNs for OLS
+        
+        # computation of VIF
+        vif = nan
+        if len(better_features) > 1 and len(X_vif) > 0:
+            vif = variance_inflation_factor(X_vif.values, len(better_features)-1)
+        
+        # dropping the feature if it was too correlated to a better feature
+        if vif > params.get('thresh_vif', inf) and notna(vif):
+            dropped += [feature]
+            
+        # kept feature: updating associations with this feature
+        else:
+            associations += [{'feature': feature, 'vif_filter': vif}]
+    
+    # formatting ouput to DataFrame
+    associations = DataFrame(associations).set_index('feature')
+            
+    # applying filter on association
+    associations = ranks.join(associations, how='right')
+    
+    return associations
+
+def qualitative_worst_corr(X: DataFrame, feature: str, ranks: DataFrame, corr_measure: Callable, **params):
+    """ Computes maximum association between a feature and features 
+    more associated to the target (according to ranks)
+    """
+    
+    # measure name
+    measure_name = corr_measure.__name__
+    measure = measure_name.replace('_measure', '')
+        
+    # initiating worst correlation
+    worst_corr = {'feature': feature}
+    
+    # features more associated with target
+    better_features = list(ranks.loc[:feature].index)[:-1]
+
+    # iterating over each better feature
+    for better_feature in better_features:
+
+        # computing association with better feature
+        _, association = corr_measure(True, {f'{measure}_with': better_feature}, 
+                                      X[feature], X[better_feature], **params)
+
+
+        # updating association if it's greater than previous better features
+        if association.get(measure_name) > worst_corr.get(measure_name, 0):
+
+            # renaming association measure as filter
+            association[f'{measure}_filter'] = association.pop(measure_name)
+            
+            # removing temporary measures
+            association = {k: v for k, v in association.items() if '_measure' not in k}
+
+            # updating worst known association
+            worst_corr.update(association)
+
+        # stopping measurements if association is greater than threshold
+        if association.get(f'{measure}_filter') > params.get('thresh_corr', 1):
+            ranks = ranks.drop(feature, axis=0)  # removing feature from ranks
+            
+            return ranks, None
+    
+    return ranks, worst_corr
+
+def qualitative_filter(X: DataFrame, ranks: DataFrame, corr_measure: Callable, **params) -> Dict[str, Any]:
+    """ Computes max association between X and X (qualitative) excluding features 
+    that are correlated to a feature more associated with the target 
+    (defined by the ranks).
+
+    Parameters
+    ----------
+    thresh_corr, float: default 1.
+        Maximum association between features
+    """
+    
+    # accessing the prefered order
+    prefered_order = ranks.index
+
+    # initiating list of maximum association per feature
+    associations = []
+    
+    # iterating over each feature by target association order
+    for feature in prefered_order:
+        
+        
+        # computing correlation with better features anf filtering out ranks
+        ranks, worst_corr = qualitative_worst_corr(X, feature, ranks, corr_measure, **params)
+        
+        # updating associations
+        if worst_corr:
+            associations += [worst_corr]
+
+    # formatting ouput to DataFrame
+    associations = DataFrame(associations).set_index('feature')
+            
+    # applying filter on association
+    associations = ranks.join(associations, how='right')
+    
+    return associations 
+
+def cramerv_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+    """ Computes max Cramer's V between X and X (qualitative) excluding features 
+    that are correlated to a feature more associated with the target 
+    (defined by the ranks).
+
+    Parameters
+    ----------
+    thresh_corr, float: default 1.
+        Maximum association between features
+    """
+            
+    # applying quantitative filter with Cramer's V correlation    
+    return qualitative_filter(X, ranks, cramerv_measure, **params)
+
+def tschuprowt_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+    """ Computes max Tschuprow's T between X and X (qualitative) excluding features 
+    that are correlated to a feature more associated with the target 
+    (defined by the ranks).
+
+    Parameters
+    ----------
+    thresh_corr, float: default 1.
+        Maximum association between features
+    """
+            
+    # applying quantitative filter with Tschuprow's T correlation
+    return qualitative_filter(X, ranks, tschuprowt_measure, **params)
```

