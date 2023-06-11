# Comparing `tmp/fastapi_module_register-0.0.1.tar.gz` & `tmp/fastapi_module_register-0.0.2.tar.gz`

## Comparing `fastapi_module_register-0.0.1.tar` & `fastapi_module_register-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/src/fastapi_module_register/__init__.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/src/fastapi_module_register/base_register.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/src/fastapi_module_register/constants.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/src/fastapi_module_register/exceptions.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/src/fastapi_module_register/logger.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/src/fastapi_module_register/schema.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/src/fastapi_module_register/utils.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/src/fastapi_module_register/tortoise/__init__.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/src/fastapi_module_register/tortoise/tortoise_register.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/README.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    13442 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/README.en.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/__init__.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/base_method.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/base_register.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/constants.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/exceptions.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/logger.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/schema.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/utils.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/tortoise/__init__.py
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/tortoise/tortoise_method.py
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/tortoise/tortoise_register.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/LICENSE
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/PKG-INFO
```

### Comparing `fastapi_module_register-0.0.1/src/fastapi_module_register/base_register.py` & `fastapi_module_register-0.0.2/src/fastapi_module_register/base_register.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from abc import abstractmethod, ABC
 from typing import Union, Dict, List, Any
 
 from fastapi import FastAPI
 
-from .schema import ModuleConfig
+from fastapi_module_register.schema import ModuleConfig
+
 
 class BaseRegister(ABC):
 
     modules: Dict[str, Union[ModuleConfig, Any]] = {}
     _inited: bool = False
 
     @classmethod
     @abstractmethod
     def init(cls, app: FastAPI, module_configs: List[ModuleConfig], *args, **kwargs) -> None:
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
-    def load_modules(cls, module_dirs: List[str], *args, **kwargs) -> List[Any]:
+    def load_modules(cls, module_dirs: List[str], *args, **kwargs) -> None:
         raise NotImplementedError
     
     @classmethod
     @abstractmethod
-    def load_routers(cls) -> None:
+    def load_routers(cls) -> List[Any]:
         raise NotImplementedError
```

### Comparing `fastapi_module_register-0.0.1/src/fastapi_module_register/utils.py` & `fastapi_module_register-0.0.2/src/fastapi_module_register/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 from importlib import import_module
 from typing import Any, Dict, List, Union
 import warnings
 
-from .constants import DEFAULT_METHODS
-from .schema import RouterConfig, ModuleConfig
+from fastapi_module_register.schema import ModuleConfig
 
 
-def get_module_config(
-    module_config: Union[List[str], List[ModuleConfig], List[Dict[str, Any]]]
+def get_module_configs(
+    module_configs: Union[List[str], List[ModuleConfig], List[Dict[str, Any]]]
 ) -> List[ModuleConfig]:
     """_summary_
 
     Args:
-        module_config (Union[List[str], List[ModuleConfig], List[Dict[str, Any]]]): _description_
+        module_configs (Union[List[str], List[ModuleConfig], List[Dict[str, Any]]]): _description_
 
     Returns:
         List[ModuleConfig]: _description_
     """
-    configs: List[ModuleConfig] = []
-    if not module_config:
-        return configs
+    modules: List[ModuleConfig] = []
+    if not module_configs:
+        return modules
     
-    for item in module_config:
-        if isinstance(item, ModuleConfig):
-            configs.append(item)
+    for module_config in module_configs:
+        if isinstance(module_config, ModuleConfig):
+            modules.append(module_config)
             continue
-        if isinstance(item, str):
-            temp_module_config = ModuleConfig(module_path=item)
-            temp_module_config.router_config = [
-                RouterConfig(method=method)
-                for method in DEFAULT_METHODS
-            ]
-            configs.append(temp_module_config)
+        if isinstance(module_config, str):
+            temp_module_config = ModuleConfig(module_path=module_config)
+            temp_module_config.add_default_router_configs()
+            modules.append(temp_module_config)
             continue
-        if isinstance(item, Dict):
-            module_config = ModuleConfig(**item)
-            configs.append(module_config)
+        if isinstance(module_config, Dict):
+            temp_module_config = ModuleConfig(**module_config)
+            modules.append(temp_module_config)
             continue
-        warnings.warn(f'Unkonwn type "{item}"', RuntimeWarning, stacklevel=4)
-
-    return configs
+        warnings.warn(f'Unkonwn type "{module_config}"', RuntimeWarning, stacklevel=4)
+    return modules
 
 
 def import_string(dotted_path: str) -> Any:
     """import model and return cls
 
     Args:
         dotted_path (str): [description]
```

### Comparing `fastapi_module_register-0.0.1/src/fastapi_module_register/tortoise/__init__.py` & `fastapi_module_register-0.0.2/src/fastapi_module_register/tortoise/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Any, Dict, List, Union
 
 from fastapi import FastAPI
 
-from .tortoise_register import TortoiseRegister
-from ..logger import logger
-from ..schema import ModuleConfig
-from ..utils import get_module_config
+from fastapi_module_register.logger import logger
+from fastapi_module_register.schema import ModuleConfig
+from fastapi_module_register.tortoise.tortoise_register import TortoiseRegister
+from fastapi_module_register.utils import get_module_configs
 
 
 def router_register(
     app: FastAPI,
-    module_config: Union[List[str], List[ModuleConfig], List[Dict[str, Any]]]
+    module_configs: Union[List[str], List[ModuleConfig], List[Dict[str, Any]]]
 ) -> None:
     """_summary_
 
     Args:
         app (FastAPI): _description_
-        module_config (Union[List[str], List[ModuleConfig], List[Dict[str, Any]]]): _description_. Defaults to None.
+        module_configs (Union[List[str], List[ModuleConfig], List[Dict[str, Any]]]): _description_. Defaults to None.
     """
-    if not module_config:
+    if not module_configs:
         logger.info("No module register.")
         return
 
     if not isinstance(app, FastAPI):
         raise RuntimeError("Please given fastapi object.")
-    
-    module_config = get_module_config(module_config)
+
+    module_configs = get_module_configs(module_configs)
     @app.on_event("startup")
     async def init_router() -> None:  # pylint: disable=W0612
-        modules = TortoiseRegister.init(app, module_config)
+        modules = TortoiseRegister.init(app, module_configs)
         logger.info("Register tortoise router started, %s", modules)
```

### Comparing `fastapi_module_register-0.0.1/src/fastapi_module_register/tortoise/tortoise_register.py` & `fastapi_module_register-0.0.2/src/fastapi_module_register/tortoise/tortoise_register.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-from typing import Callable, Dict, Type, List, Optional
+from typing import Any, Dict, List, Optional, Type
 import warnings
 
 from fastapi import FastAPI
 from tortoise.models import Model
+from tortoise.contrib.fastapi import HTTPNotFoundError
 
-from ..base_register import BaseRegister
-from ..exceptions import ConfigurationError
-from ..schema import ModuleConfig
-from ..utils import api_path_handler, import_string 
+from fastapi_module_register.base_register import BaseRegister
+from fastapi_module_register.exceptions import ConfigurationError
+from fastapi_module_register.schema import ModuleConfig
+from fastapi_module_register.tortoise.tortoise_method import TortoiseMethod
+from fastapi_module_register.utils import import_string 
 
 
 class TortoiseRegister(BaseRegister):
 
     @classmethod
     def init(cls, app: FastAPI, module_configs: List[ModuleConfig]) -> None:
         if cls._inited or not module_configs:
             return
-        modules = cls.load_modules(module_configs)
-        routers = cls.load_routers(modules)
+        
+        cls.load_modules(module_configs)
+        routers = cls.load_routers()
         cls.add_router(app, routers)
 
     @classmethod
-    def load_modules(cls, module_configs: List[ModuleConfig]) -> Dict[str, ModuleConfig]:
-        """_summary_
+    def load_modules(cls, module_configs: List[ModuleConfig]) -> None:
+        """load modules
 
         Args:
             app (FastAPI): _description_
             modules (Optional[List[str]]): _description_
         """
         for module_config in module_configs:
             # Loading module
-            model = cls._discover_model(module_config.module_path)
-            if not model:
+            module = cls._discover_model(module_config.module_path)
+            if not module:
                 continue
-            module_config.model = model
+            module_config.module = module
             if not module_config.name:
-                module_config.name = model.__name__
-        return {model.name: model for model in module_configs}
+                module_config.name = module.__name__
+        cls.modules = {model.name: model for model in module_configs}
 
     @classmethod
     def _discover_model(
         cls,
         models_path: str
     ) -> Optional[Type["Model"]]:
         """_summary_
@@ -59,43 +62,50 @@
 
         if issubclass(module, Model) and not module._meta.abstract:
             if not module._meta.app:
                 return None
             return module
 
     @classmethod
-    def load_routers(cls, modules: Dict[str, ModuleConfig]) -> None:
-        """_summary_
-
-        Args:
-            modules (Dict[str, ModuleConfig]]): _description_
+    def load_routers(cls) -> List[Any]:
+        """load routers
 
         Returns:
             _type_: _description_
         """
+        
         routers = []
-        for name, module in modules.items():
-            if not issubclass(module.model, Model):
+        for _, module_config in cls.modules.items():
+            if not issubclass(module_config.module, Model):
                 warnings.warn(f"The module is not a type model")
+                continue
 
-            api_path = api_path_handler(module.model.__name__)
-            for config in module.router_config:
-                exec_fun = getattr(cls, config.method, None)
+            tortoise_method = TortoiseMethod(module_config.module)
+            for config in module_config.router_config:
+                exec_fun = getattr(tortoise_method, config.method, None)
                 if not exec_fun:
                     warnings.warn(f"Unsupported http method: {config.method}")
                     continue
-                exec_fun_obj = exec_fun()
+
+                if config.method.lower() == "get":
+                    filter_by_pk = True if '{pk}' in config.api_path else False
+                    exec_fun_obj, req_schema = exec_fun(filter_by_pk)
+                else:
+                    exec_fun_obj, req_schema = exec_fun()
                 if not callable(exec_fun_obj):
                     continue
+
                 router = {
-                    "path": api_path,
+                    "path": config.api_path,
                     "endpoint": exec_fun_obj,
                     "methods": [config.method],
-                    "tags": [name],
+                    "response_model": req_schema,
+                    "responses": {404: {"model": HTTPNotFoundError}}
                 }
+                router.update(config.parameters)
                 routers.append(router)
         return routers
 
     @classmethod
     def add_router(cls, app: FastAPI, routers: List[Dict]) -> None:
         """_summary_
 
@@ -104,33 +114,7 @@
             routers (List[Dict]): _description_
         """
         if not routers:
             return
         
         for router in routers:
             app.add_api_route(**router)
-
-    @classmethod
-    def get(cls) -> Callable:
-        async def get_method():
-            return {"1": 2}        
-        return get_method
-
-    @classmethod
-    def post(cls) -> None:
-        async def post_method():
-            pass
-
-    @classmethod
-    def put(cls) -> None:
-        async def put_method():
-            pass
-
-    @classmethod
-    def patch(cls) -> None:
-        async def patch_method():
-            pass
-
-    @classmethod
-    def delete(cls) -> None:
-        async def delete_method():
-            pass
```

### Comparing `fastapi_module_register-0.0.1/.gitignore` & `fastapi_module_register-0.0.2/.gitignore`

 * *Files 21% similar despite different names*

```diff
@@ -42,53 +42,68 @@
 .nox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *.cover
+*.py,cover
 .hypothesis/
 .pytest_cache/
+cover/
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
 local_settings.py
 db.sqlite3
-db.sqlite3-shm
-db.sqlite3-wal
+db.sqlite3-journal
 
 # Flask stuff:
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
 
 # PyBuilder
+.pybuilder/
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
 
 # IPython
 profile_default/
 ipython_config.py
 
 # pyenv
-.python-version
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
 
-# celery beat schedule file
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
 celerybeat-schedule
+celerybeat.pid
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
 .env
 .venv
@@ -111,7 +126,15 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+.pypirc
```

### Comparing `fastapi_module_register-0.0.1/pyproject.toml` & `fastapi_module_register-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_module_register"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="stan", email="gd19920125@hotmail.com"},
 ]
 description = "通过将fastapi的模型自动注册路由"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "fastapi>=0.95.1",
-    "tortoise-orm>=0.19.3"
+    "tortoise-orm>=0.19.3",
+    "ujson>=5.7.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dcshoecousa"
```

