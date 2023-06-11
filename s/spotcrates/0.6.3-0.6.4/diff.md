# Comparing `tmp/spotcrates-0.6.3.tar.gz` & `tmp/spotcrates-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotcrates-0.6.3.tar", max compression
+gzip compressed data, was "spotcrates-0.6.4.tar", max compression
```

## Comparing `spotcrates-0.6.3.tar` & `spotcrates-0.6.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1068 2022-12-15 22:50:22.212154 spotcrates-0.6.3/LICENSE
--rw-r--r--   0        0        0    11842 2023-03-22 02:23:26.155732 spotcrates-0.6.3/README.md
--rw-r--r--   0        0        0      792 2023-05-07 03:32:40.794955 spotcrates-0.6.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-04 22:49:46.694616 spotcrates-0.6.3/spotcrates/__init__.py
--rw-r--r--   0        0        0     9738 2023-05-06 22:40:36.400846 spotcrates-0.6.3/spotcrates/cli.py
--rw-r--r--   0        0        0     2601 2023-05-06 22:08:20.007380 spotcrates-0.6.3/spotcrates/common.py
--rw-r--r--   0        0        0     9738 2023-03-20 16:44:29.264590 spotcrates-0.6.3/spotcrates/filters.py
--rw-r--r--   0        0        0    16392 2023-03-20 21:08:56.572940 spotcrates-0.6.3/spotcrates/playlists.py
--rw-r--r--   0        0        0      401 2022-12-15 22:03:25.519119 spotcrates-0.6.3/spotcrates/templates/auth_index.html
--rw-r--r--   0        0        0      173 2022-12-15 22:03:25.523119 spotcrates-0.6.3/spotcrates/templates/base.html
--rw-r--r--   0        0        0      150 2022-12-15 22:03:25.523119 spotcrates-0.6.3/spotcrates/templates/index.html
--rw-r--r--   0        0        0    13098 1970-01-01 00:00:00.000000 spotcrates-0.6.3/setup.py
--rw-r--r--   0        0        0    12594 1970-01-01 00:00:00.000000 spotcrates-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-10 20:26:58.614364 spotcrates-0.6.4/LICENSE
+-rw-r--r--   0        0        0    11842 2023-06-10 20:26:58.614364 spotcrates-0.6.4/README.md
+-rw-r--r--   0        0        0      792 2023-06-11 03:41:03.306695 spotcrates-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 20:26:59.810367 spotcrates-0.6.4/spotcrates/__init__.py
+-rw-r--r--   0        0        0    10264 2023-06-11 03:07:12.056616 spotcrates-0.6.4/spotcrates/cli.py
+-rw-r--r--   0        0        0     2557 2023-06-10 23:12:51.552434 spotcrates-0.6.4/spotcrates/common.py
+-rw-r--r--   0        0        0     9707 2023-06-10 23:13:05.032468 spotcrates-0.6.4/spotcrates/filters.py
+-rw-r--r--   0        0        0    16425 2023-06-11 02:35:29.291569 spotcrates-0.6.4/spotcrates/playlists.py
+-rw-r--r--   0        0        0      401 2023-06-10 20:26:59.810367 spotcrates-0.6.4/spotcrates/templates/auth_index.html
+-rw-r--r--   0        0        0      173 2023-06-10 20:26:59.810367 spotcrates-0.6.4/spotcrates/templates/base.html
+-rw-r--r--   0        0        0      150 2023-06-10 20:26:59.810367 spotcrates-0.6.4/spotcrates/templates/index.html
+-rw-r--r--   0        0        0    12594 1970-01-01 00:00:00.000000 spotcrates-0.6.4/PKG-INFO
```

### Comparing `spotcrates-0.6.3/LICENSE` & `spotcrates-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spotcrates-0.6.3/README.md` & `spotcrates-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `spotcrates-0.6.3/pyproject.toml` & `spotcrates-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotcrates"
-version = "0.6.3"
+version = "0.6.4"
 description = ""
 authors = ["Chris Mayes <cmayes@cmay.es>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 jinja2 = "^3.1.2"
```

### Comparing `spotcrates-0.6.3/spotcrates/cli.py` & `spotcrates-0.6.4/spotcrates/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,18 @@
 from pathlib import Path
 
 import spotipy
 
 from spotcrates.playlists import Playlists, PlaylistResult
 from appdirs import user_config_dir, user_cache_dir
 
-logging.basicConfig(format="%(levelname)s: %(message)s", level=logging.INFO)
+# Turn down noisy third-party debug logs
+logging.getLogger('spotipy').setLevel(logging.INFO)
+logging.getLogger('urllib3').setLevel(logging.INFO)
+
 logger = logging.getLogger(__name__)
 
 DEFAULT_CONFIG_DIR = user_config_dir("spotcrates")
 DEFAULT_CONFIG_FILE = Path(DEFAULT_CONFIG_DIR, "spotcrates_config.toml")
 DEFAULT_CACHE_DIR = user_cache_dir("spotcrates")
 DEFAULT_AUTH_CACHE_FILE = Path(DEFAULT_CACHE_DIR, "spotcrates_auth_cache")
 DEFAULT_AUTH_SCOPES = ["playlist-modify-private", "playlist-read-private"]
@@ -50,14 +53,17 @@
 {'daily':<16} Add "Daily Mix" entries to the end of the target playlist, filtering for excluded entries.
 {'init-config':<16} Initializes the configuration file. Uses the --config_file location as the target. Will not overwrite.
 {'list-playlists':<16} Prints a table describing your playlists.
 {'randomize':<16} Randomizes the playlists with the given names, IDs, or in the given collections.
 {'subscriptions':<16} Add new tracks from configured playlists to the target playlist, filtering for excluded entries.
 """
 
+# LOG_FORMAT = "%(levelname)s (%(name)s): %(message)s"
+LOG_FORMAT = "%(message)s"
+
 
 def print_commands():
     """Prints available commands."""
     print(COMMAND_DESCRIPTION)
 
 
 def get_config(config_file: Path):
@@ -236,14 +242,20 @@
     parser.add_argument('--version', action='version', version=__version__)
     parser.add_argument("-t", "--target",
                         help="Specify the target name of the operation (overrides any default value)")
     parser.add_argument("command", metavar="COMMAND",
                         help=f"The command to run (one of {','.join(COMMANDS)})")
     parser.add_argument("arguments", metavar='ARGUMENTS', nargs='*',
                         help="the arguments to the command")
+    parser.add_argument('-log',
+                        '--loglevel',
+                        default='info',
+                        type=str.upper,
+                        choices=logging._nameToLevel.keys(),
+                        help='Provide logging level. Example: --loglevel debug, default is info')
     args = None
     try:
         args = parser.parse_args(argv)
     except IOError as e:
         logger.warning("Problems reading file:", e)
         parser.print_help()
         return args, 2
@@ -251,14 +263,16 @@
     return args, 0
 
 
 def main(argv=None):
     args, ret = parse_cmdline(argv)
     if ret != 0:
         return ret
+    logging.basicConfig(format=LOG_FORMAT, level=args.loglevel)
+
     config = get_config(args.config_file)
 
     command = CommandLookup().find(args.command.lower())
 
     if command == "commands":
         return print_commands()
     elif command == "copy":
```

### Comparing `spotcrates-0.6.3/spotcrates/common.py` & `spotcrates-0.6.4/spotcrates/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     return full_value
 
 
 class BaseLookup(ABC):
     def __init__(self):
         """Uses a trie to find the longest matching prefix for the given lookup value"""
         self.logger = logging.getLogger(__name__)
-        self.logger.setLevel(logging.DEBUG)
         self.lookup = self._init_lookup()
 
     def find(self, lookup_val):
         if not lookup_val:
             raise NotFoundException(f"Blank/null lookup value {lookup_val}")
 
         found_command = self.lookup.longest_prefix(lookup_val)
```

### Comparing `spotcrates-0.6.3/spotcrates/filters.py` & `spotcrates-0.6.4/spotcrates/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Dict, List
 
 import pygtrie
 
 from spotcrates.common import NotFoundException, BaseLookup
 
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
 
 
 class InvalidFilterException(Exception):
     pass
 
 
 class FilterType(Enum):
```

### Comparing `spotcrates-0.6.3/spotcrates/playlists.py` & `spotcrates-0.6.4/spotcrates/playlists.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         """Creates an instance of the playlist manipulation class.
 
         :param spotify: A handle for the initialized SpotiPy client.
         :param config: The configuration for the playlists class.
         """
         self.spotify = spotify
         self.logger = logging.getLogger(__name__)
-        self.logger.setLevel(logging.DEBUG)
 
         self.config = self._process_config(config)
 
     def get_all_playlists(self) -> List[Dict]:
         return get_all_items(self.spotify, self.spotify.current_user_playlists())
 
     def list_all_playlists(self, sort_fields=None, filters=None) -> List[Dict]:
@@ -205,14 +204,16 @@
                 me["id"], subscriptions_target, public=False
             )
 
         excludes = self._get_excludes(exclude_lists, target_list)
 
         playlist_ids = self._get_subscription_playlist_ids(oldest_timestamp, excludes)
 
+        self.logger.info(f"{len(playlist_ids)} subscription tracks to add")
+
         if randomize:
             playlist_ids = list(playlist_ids)
             random.shuffle(playlist_ids)
 
         for id_batch in batched(playlist_ids, 100):
             self.logger.debug(f"Batch size: {len(id_batch)}")
             self.spotify.playlist_add_items(target_list["id"], id_batch)
```

### Comparing `spotcrates-0.6.3/setup.py` & `spotcrates-0.6.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,290 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: spotcrates
+Version: 0.6.4
+Summary: 
+Author: Chris Mayes
+Author-email: cmayes@cmay.es
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: durations-nlp (>=1.0.1,<2.0.0)
+Requires-Dist: flask-session (>=0.4.0,<0.5.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: pygtrie (>=2.5.0,<3.0.0)
+Requires-Dist: redis (>=4.5.3,<5.0.0)
+Requires-Dist: spotipy (>=2.22.1,<3.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
+Requires-Dist: types-appdirs (>=1.4.3.5,<2.0.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['spotcrates']
+# Spotcrates
+## A set of tools for finding and managing music on Spotify
 
-package_data = \
-{'': ['*'], 'spotcrates': ['templates/*']}
+![Code Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/cmayes/3c8214e2bd942821496440b93acd3582/raw/covbadge.json)
 
-install_requires = \
-['appdirs>=1.4.4,<2.0.0',
- 'durations-nlp>=1.0.1,<2.0.0',
- 'flask-session>=0.4.0,<0.5.0',
- 'jinja2>=3.1.2,<4.0.0',
- 'pygtrie>=2.5.0,<3.0.0',
- 'redis>=4.5.3,<5.0.0',
- 'spotipy>=2.22.1,<3.0.0',
- 'tomli-w>=1.0.0,<2.0.0',
- 'tomli>=2.0.1,<3.0.0',
- 'types-appdirs>=1.4.3.5,<2.0.0.0']
-
-entry_points = \
-{'console_scripts': ['spotcrates = spotcrates.cli:main']}
-
-setup_kwargs = {
-    'name': 'spotcrates',
-    'version': '0.6.3',
-    'description': '',
-    'long_description': '# Spotcrates\n## A set of tools for finding and managing music on Spotify\n\n![Code Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/cmayes/3c8214e2bd942821496440b93acd3582/raw/covbadge.json)\n\n# Installation\n\n## Requirements\n\nSpotcrates requires [Python](https://www.python.org/) 10 or newer. You will also need a Spotify account.\n\n## Install from PyPI\n\n```shell\npip install spotcrates\n```\n\n## Configuration\n\nSpotcrates will need, at minimum, credentials for accessing your Spotify account. You may also specify\nplaylists to subscribe to, among other settings.\n\n### Initial Configuration File\n\nSpotcrates can create an initial configuration file for itself. It will write to the specified configuration file\nlocation, i.e. what you configure with `-c` or `--config_file`. If you don\'t specify anything, Spotcrates will use\na platform-specific configuration file location, e.g. `/home/$USER/.config/spotcrates/spotcrates_config.toml` \non Linux. The output of `spotcrates -h` includes the default location for your configuration file.\n\n```shell\nspotcrates init-config\n```\n\n### Spotify API Credentials\n\nThis bit is not terribly user-friendly as it\'s assumed that developers will be the ones creating these credentials.\nSince this app runs as a script on your own machine, you\'ll need to create your own credentials. You will need\na `Client ID` and a `Client Secret`. The process is a little involved, and the \n[Spotify docs on the subject](https://developer.spotify.com/documentation/general/guides/authorization/app-settings/) \nare a bit opaque for the casual user (as I very recently was). These pages do a pretty good job describing \nthe process:\n\n- https://support.heateor.com/get-spotify-client-id-client-secret/\n- https://cran.r-project.org/web/packages/spotidy/vignettes/Connecting-with-the-Spotify-API.html\n\nNote that these projects are mainly interested in extracting data for their respective applications, so the \ninstructions are geared to that end.\n\nOnce you have your client ID and client secret, paste them into your Spotcrates configuration file in the `[spotify]`\nsection:\n\n```toml\n[spotify]\nclient_id = "(your ID here)"\nclient_secret = "(your secret here)"\n```\n\n#### Testing Your Credentials\n\nSpotcrates will request and cache authorization info the first time you use your Spotify credentials. The cache location\nis platform-specific. On Linux, it\'s usually at `/home/$USER/.cache/spotcrates/spotcrates_auth_cache`.\n\nTo trigger this step, you can try listing your playlists:\n\n`spotcrates list-playlists`\n\nSpotcrates will initiate an authorization process with Spotify via your default browser. If the authorization\nsucceeds, the browser tab will close itself, and your playlists will be listed on the command line.\n\n### Customizable Settings for Spotify\n\nThese settings can be changed from their defaults, though you won\'t usually need to do so. They are defined\nunder the `[spotify]` config file heading.\n\n- `auth_cache`: The location of the Spotify authorization cache. This defaults to your platform\'s default cache\n    location base, plus `spotcrates/spotcrates_auth_cache`.\n- `auth_scopes`: A list of authorization scopes that Spotcrates requests. The default scopes are\n    `["playlist-modify-private", "playlist-read-private"]`.\n\n## Playlists\n\nThese settings control playlist-related commands like [daily](#daily) or [randomize](#randomize). They\ncan be customized under the [playlists] heading in the configuration file.\n\n- `daily_mix_target`: The name of the playlist to target, which is created if it does not exist. Defaults to "Now."\n- `daily_mix_prefix`: The prefix of the "Daily Mix" playlists to be aggregated. Defaults to "Daily Mix."\n- `daily_mix_excludes`: The prefix of the playlists that contain tracks to exclude. Defaults to "Overplayed."\n\n## Subscriptions\n\nThese settings are for the [subscriptions](#subscriptions) command. They can be configured under the `[subscriptions]` \nconfiguration file heading. \n\n- `subscriptions_target`: The name of the playlists where the new subscriptions will be appended. Created if \n    the playlist does not exist. Defaults to `NewSubscriptions`.\n- `max_age`: The maximum age of a track in a playlist for it to be considered "new." Values can be English\n    expressions like `2 weeks` or `96 hours`. Defaults to `3 days`.\n\n### Subscription Playlists\n\nThese are the playlist groups used by [subscriptions](#subscriptions) and related commands. All groups are included\nby default. The values are the "spotify IDs" listed in the [list-playlists](#list-playlists) command. These playlist \ngroups are configured under the [subscriptions.playlists] section of the configuration file.\n\n\n```toml\n[subscriptions.playlists]\n# IRL ANGEL, Twin Peaks Vibes, Folk Fabrique,\n# FADO PORTUGAL, While You Work\nquiet = ["37i9dQZF1DX7Ocjwy96xTX", "38rrtWgflrw7grB37aMlsO", "37i9dQZF1DX62XscWX9t6h",\n"67waO0NR8HTySxtB7wfMBZ", "6bUIofrj5PWNIeb67DbUqf"]\n# Japanese Shoegaze, Modern Psychedelia, Adrenaline Coding\nnoisy = ["2uiYiQFpynkWCpIXcBGir9", "37i9dQZF1DX8gDIpdqp1XJ", "3JEvwuKbVKoggEA75gWqET"]\n# State of Jazz, Jazz-Funk, Jazz Funk (Instrumental),\n# Jazz Funk & Groove\njazz = ["37i9dQZF1DX7YCknf2jT6s", "37i9dQZF1DWUb0uBnlJuTi", "4xRrCdkn4r5lrDOElek5oC",\n"2puFFdGTID0iJdQtjLvhal"]\n```\n\n# Commands\n\nThe installation script puts the command `spotcrates` in your Python environment\n(e.g. `/.pyenv/shims/spotcrates`). The command `spotcrates commands` lists all of the \ncommands available along with a short description of each.\n\nNote that Spotcrates will accept the shortest unique command substring, so for example you can run\n`spotcrates sub` for the `subscriptions` command.\n\n## daily\n`spotcrates daily` collects the contents of the "Daily Mix" playlists, filters them \nagainst an exclusion list ("Overplayed" by default), and adds them to the end of \na target list ("Now" by default).\n\n## subscriptions\n`spotcrates subscriptions` adds new tracks from configured playlists to the target playlist, \nfiltering for excluded entries. Three days is the default maximum age for a track to be \nconsidered "new."\n\n## list-playlists\n`spotcrates list-playlists` lists playlists\' name, owner, track count, and description.\nThe command accepts `-f` for filter expressions and `-s` for sort expressions. (TODO: \nadd description of filter and search expressions and link to it here)\n\n### Search Patterns\n\nThe command `list-playlists` accepts search filters passed via the `-f` option. Multiple\nfilter expressions are separated by commas.\n\n#### Search Examples\n\n`spotcrates li -f jazz`\n\nList playlists where any field contains the string "jazz" (case-insensitive)\n\n```\nPLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION\nJazz Piano Classics              100   37i9dQZF1DX5q7wCXFrkHh   spotify          The classic piano recordings in Jazz. Cover: Oscar Peterson\nAcid Jazz                        90    37i9dQZF1DWXHghfFFOaS6   spotify          Where hip-hop and soul meets jazz. Cover: Digable Planets\nJazz Funk                        6     61Q9DgzF3f1ULr3i1uRyUy   cmayes3          \nAcid Jazz                        3     1h6rEPX9qRpBCBbjuAysMz   cmayes3          \nGeneral Jazz                     513   1j6ndSnyYn6oUlnwpGiRWc   cmayes3          \nJazz Funk (Instrumental)         272   4xRrCdkn4r5lrDOElek5oC   1226030890       \nInstrumental Acid Jazz Mix       50    37i9dQZF1EIgnEnn8SKPjM   spotify          Instrumental Acid Jazz music picked just for you\nState of Jazz                    100   37i9dQZF1DX7YCknf2jT6s   spotify          New jazz for open minds. Cover: Walter Smith III\nJazz-Funk                        200   37i9dQZF1DWUb0uBnlJuTi   spotify          Jazz. But funky. Cover: Takuya Kuroda\nJazz                             1     6VH2cw8n115fbQ7Ls2wzdR   cmayes3          \nFaLaLaLaLa GREAT BIG Christmas V 4051  6A2Kj9cWUpuu0UcEbWVf5E   kingofjingaling  Over 170 hours of classic Christmas music. The focus is on classic Christma\n```\n\n`spotcrates li -f o:spotify,n:rise`\n\nList playlists where the owner contains `spotify` and name contains `rise`.\n\n```\nPLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION\nRise                             230   37i9dQZF1DWUOhRIDwDB7M   spotify          Positive and uplifting ambient instrumental tracks.\n```\n\n`spotcrates li -f n:ends:villains`\n\nList playlists where name ends with `villains`.\n\n```\nPLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION\nclassical music for villains     66    0zkl7eKzuUit1QRPVKtga2   225uye2hek5id23t \n```\n\n#### Search Fields\n\nThe default search field is `all`.\n\n- spotify_id\n- playlist_name\n- size\n- owner\n- playlist_description\n- all: Search any/all of the above fields.\n\n#### Search Types\n\nThe default search type is `contains`.\n\n- contains\n- equals\n- starts\n- ends\n- greater\n- less\n- greater_equal\n- less_equal\n\n### Sort Patterns\n\nThe command `list-playlists` accepts sort filters passed via the `-s` option. Multiple\nsort expressions are separated by commas.\n\n#### Sort Examples\n\n`spotcrates li -f n:jazz -s name`\n\nName contains `jazz`; sort by name ascending.\n\n```\nPLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION\nAcid Jazz                        90    37i9dQZF1DWXHghfFFOaS6   spotify          Where hip-hop and soul meets jazz. Cover: Digable Planets\nAcid Jazz                        3     1h6rEPX9qRpBCBbjuAysMz   cmayes3          \nGeneral Jazz                     513   1j6ndSnyYn6oUlnwpGiRWc   cmayes3          \nInstrumental Acid Jazz Mix       50    37i9dQZF1EIgnEnn8SKPjM   spotify          Instrumental Acid Jazz music picked just for you\nJazz                             1     6VH2cw8n115fbQ7Ls2wzdR   cmayes3          \nJazz Funk                        6     61Q9DgzF3f1ULr3i1uRyUy   cmayes3          \nJazz Funk (Instrumental)         272   4xRrCdkn4r5lrDOElek5oC   1226030890       \nJazz Piano Classics              100   37i9dQZF1DX5q7wCXFrkHh   spotify          The classic piano recordings in Jazz. Cover: Oscar Peterson\nJazz-Funk                        200   37i9dQZF1DWUb0uBnlJuTi   spotify          Jazz. But funky. Cover: Takuya Kuroda\nState of Jazz                    100   37i9dQZF1DX7YCknf2jT6s   spotify          New jazz for open minds. Cover: Walter Smith III\n```\n\n`spotcrates li -f jazz,size:ge:100 -s size:desc`\n\nAny field contains `jazz`; size is greater than or equal to 100, sort by size descending.\n\n```\nPLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION\nFaLaLaLaLa GREAT BIG Christmas V 4051  6A2Kj9cWUpuu0UcEbWVf5E   kingofjingaling  Over 170 hours of classic Christmas music. The focus is on classic Christma\nGeneral Jazz                     513   1j6ndSnyYn6oUlnwpGiRWc   cmayes3          \nJazz Funk (Instrumental)         272   4xRrCdkn4r5lrDOElek5oC   1226030890       \nJazz-Funk                        200   37i9dQZF1DWUb0uBnlJuTi   spotify          Jazz. But funky. Cover: Takuya Kuroda\nJazz Piano Classics              100   37i9dQZF1DX5q7wCXFrkHh   spotify          The classic piano recordings in Jazz. Cover: Oscar Peterson\nState of Jazz                    100   37i9dQZF1DX7YCknf2jT6s   spotify          New jazz for open minds. Cover: Walter Smith III\n```\n\n#### Sort Types\n\nThe default sort type is `ascending`, i.e. a-z.\n\n- ascending\n- descending\n\n## randomize\n`spotcrates randomize (playlist1) (playlist2)...` randomizes the playlists with the given names, \nIDs, or in the given collections. \n\n## copy\n`spotcrates copy (source) (dest)` copies a playlist into a new playlist. You may optionally specify \na destination playlist name; the default is to name the destination based on the source name with\nthe general form `f"{source_name}-{count:02d}"`.\n\n## commands\n`spotcrates commands` displays a summary of the available commands.',
-    'author': 'Chris Mayes',
-    'author_email': 'cmayes@cmay.es',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+# Installation
 
+## Requirements
 
-setup(**setup_kwargs)
+Spotcrates requires [Python](https://www.python.org/) 10 or newer. You will also need a Spotify account.
+
+## Install from PyPI
+
+```shell
+pip install spotcrates
+```
+
+## Configuration
+
+Spotcrates will need, at minimum, credentials for accessing your Spotify account. You may also specify
+playlists to subscribe to, among other settings.
+
+### Initial Configuration File
+
+Spotcrates can create an initial configuration file for itself. It will write to the specified configuration file
+location, i.e. what you configure with `-c` or `--config_file`. If you don't specify anything, Spotcrates will use
+a platform-specific configuration file location, e.g. `/home/$USER/.config/spotcrates/spotcrates_config.toml` 
+on Linux. The output of `spotcrates -h` includes the default location for your configuration file.
+
+```shell
+spotcrates init-config
+```
+
+### Spotify API Credentials
+
+This bit is not terribly user-friendly as it's assumed that developers will be the ones creating these credentials.
+Since this app runs as a script on your own machine, you'll need to create your own credentials. You will need
+a `Client ID` and a `Client Secret`. The process is a little involved, and the 
+[Spotify docs on the subject](https://developer.spotify.com/documentation/general/guides/authorization/app-settings/) 
+are a bit opaque for the casual user (as I very recently was). These pages do a pretty good job describing 
+the process:
+
+- https://support.heateor.com/get-spotify-client-id-client-secret/
+- https://cran.r-project.org/web/packages/spotidy/vignettes/Connecting-with-the-Spotify-API.html
+
+Note that these projects are mainly interested in extracting data for their respective applications, so the 
+instructions are geared to that end.
+
+Once you have your client ID and client secret, paste them into your Spotcrates configuration file in the `[spotify]`
+section:
+
+```toml
+[spotify]
+client_id = "(your ID here)"
+client_secret = "(your secret here)"
+```
+
+#### Testing Your Credentials
+
+Spotcrates will request and cache authorization info the first time you use your Spotify credentials. The cache location
+is platform-specific. On Linux, it's usually at `/home/$USER/.cache/spotcrates/spotcrates_auth_cache`.
+
+To trigger this step, you can try listing your playlists:
+
+`spotcrates list-playlists`
+
+Spotcrates will initiate an authorization process with Spotify via your default browser. If the authorization
+succeeds, the browser tab will close itself, and your playlists will be listed on the command line.
+
+### Customizable Settings for Spotify
+
+These settings can be changed from their defaults, though you won't usually need to do so. They are defined
+under the `[spotify]` config file heading.
+
+- `auth_cache`: The location of the Spotify authorization cache. This defaults to your platform's default cache
+    location base, plus `spotcrates/spotcrates_auth_cache`.
+- `auth_scopes`: A list of authorization scopes that Spotcrates requests. The default scopes are
+    `["playlist-modify-private", "playlist-read-private"]`.
+
+## Playlists
+
+These settings control playlist-related commands like [daily](#daily) or [randomize](#randomize). They
+can be customized under the [playlists] heading in the configuration file.
+
+- `daily_mix_target`: The name of the playlist to target, which is created if it does not exist. Defaults to "Now."
+- `daily_mix_prefix`: The prefix of the "Daily Mix" playlists to be aggregated. Defaults to "Daily Mix."
+- `daily_mix_excludes`: The prefix of the playlists that contain tracks to exclude. Defaults to "Overplayed."
+
+## Subscriptions
+
+These settings are for the [subscriptions](#subscriptions) command. They can be configured under the `[subscriptions]` 
+configuration file heading. 
+
+- `subscriptions_target`: The name of the playlists where the new subscriptions will be appended. Created if 
+    the playlist does not exist. Defaults to `NewSubscriptions`.
+- `max_age`: The maximum age of a track in a playlist for it to be considered "new." Values can be English
+    expressions like `2 weeks` or `96 hours`. Defaults to `3 days`.
+
+### Subscription Playlists
+
+These are the playlist groups used by [subscriptions](#subscriptions) and related commands. All groups are included
+by default. The values are the "spotify IDs" listed in the [list-playlists](#list-playlists) command. These playlist 
+groups are configured under the [subscriptions.playlists] section of the configuration file.
+
+
+```toml
+[subscriptions.playlists]
+# IRL ANGEL, Twin Peaks Vibes, Folk Fabrique,
+# FADO PORTUGAL, While You Work
+quiet = ["37i9dQZF1DX7Ocjwy96xTX", "38rrtWgflrw7grB37aMlsO", "37i9dQZF1DX62XscWX9t6h",
+"67waO0NR8HTySxtB7wfMBZ", "6bUIofrj5PWNIeb67DbUqf"]
+# Japanese Shoegaze, Modern Psychedelia, Adrenaline Coding
+noisy = ["2uiYiQFpynkWCpIXcBGir9", "37i9dQZF1DX8gDIpdqp1XJ", "3JEvwuKbVKoggEA75gWqET"]
+# State of Jazz, Jazz-Funk, Jazz Funk (Instrumental),
+# Jazz Funk & Groove
+jazz = ["37i9dQZF1DX7YCknf2jT6s", "37i9dQZF1DWUb0uBnlJuTi", "4xRrCdkn4r5lrDOElek5oC",
+"2puFFdGTID0iJdQtjLvhal"]
+```
+
+# Commands
+
+The installation script puts the command `spotcrates` in your Python environment
+(e.g. `/.pyenv/shims/spotcrates`). The command `spotcrates commands` lists all of the 
+commands available along with a short description of each.
+
+Note that Spotcrates will accept the shortest unique command substring, so for example you can run
+`spotcrates sub` for the `subscriptions` command.
+
+## daily
+`spotcrates daily` collects the contents of the "Daily Mix" playlists, filters them 
+against an exclusion list ("Overplayed" by default), and adds them to the end of 
+a target list ("Now" by default).
+
+## subscriptions
+`spotcrates subscriptions` adds new tracks from configured playlists to the target playlist, 
+filtering for excluded entries. Three days is the default maximum age for a track to be 
+considered "new."
+
+## list-playlists
+`spotcrates list-playlists` lists playlists' name, owner, track count, and description.
+The command accepts `-f` for filter expressions and `-s` for sort expressions. (TODO: 
+add description of filter and search expressions and link to it here)
+
+### Search Patterns
+
+The command `list-playlists` accepts search filters passed via the `-f` option. Multiple
+filter expressions are separated by commas.
+
+#### Search Examples
+
+`spotcrates li -f jazz`
+
+List playlists where any field contains the string "jazz" (case-insensitive)
+
+```
+PLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION
+Jazz Piano Classics              100   37i9dQZF1DX5q7wCXFrkHh   spotify          The classic piano recordings in Jazz. Cover: Oscar Peterson
+Acid Jazz                        90    37i9dQZF1DWXHghfFFOaS6   spotify          Where hip-hop and soul meets jazz. Cover: Digable Planets
+Jazz Funk                        6     61Q9DgzF3f1ULr3i1uRyUy   cmayes3          
+Acid Jazz                        3     1h6rEPX9qRpBCBbjuAysMz   cmayes3          
+General Jazz                     513   1j6ndSnyYn6oUlnwpGiRWc   cmayes3          
+Jazz Funk (Instrumental)         272   4xRrCdkn4r5lrDOElek5oC   1226030890       
+Instrumental Acid Jazz Mix       50    37i9dQZF1EIgnEnn8SKPjM   spotify          Instrumental Acid Jazz music picked just for you
+State of Jazz                    100   37i9dQZF1DX7YCknf2jT6s   spotify          New jazz for open minds. Cover: Walter Smith III
+Jazz-Funk                        200   37i9dQZF1DWUb0uBnlJuTi   spotify          Jazz. But funky. Cover: Takuya Kuroda
+Jazz                             1     6VH2cw8n115fbQ7Ls2wzdR   cmayes3          
+FaLaLaLaLa GREAT BIG Christmas V 4051  6A2Kj9cWUpuu0UcEbWVf5E   kingofjingaling  Over 170 hours of classic Christmas music. The focus is on classic Christma
+```
+
+`spotcrates li -f o:spotify,n:rise`
+
+List playlists where the owner contains `spotify` and name contains `rise`.
+
+```
+PLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION
+Rise                             230   37i9dQZF1DWUOhRIDwDB7M   spotify          Positive and uplifting ambient instrumental tracks.
+```
+
+`spotcrates li -f n:ends:villains`
+
+List playlists where name ends with `villains`.
+
+```
+PLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION
+classical music for villains     66    0zkl7eKzuUit1QRPVKtga2   225uye2hek5id23t 
+```
+
+#### Search Fields
+
+The default search field is `all`.
+
+- spotify_id
+- playlist_name
+- size
+- owner
+- playlist_description
+- all: Search any/all of the above fields.
+
+#### Search Types
+
+The default search type is `contains`.
+
+- contains
+- equals
+- starts
+- ends
+- greater
+- less
+- greater_equal
+- less_equal
+
+### Sort Patterns
+
+The command `list-playlists` accepts sort filters passed via the `-s` option. Multiple
+sort expressions are separated by commas.
+
+#### Sort Examples
+
+`spotcrates li -f n:jazz -s name`
+
+Name contains `jazz`; sort by name ascending.
+
+```
+PLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION
+Acid Jazz                        90    37i9dQZF1DWXHghfFFOaS6   spotify          Where hip-hop and soul meets jazz. Cover: Digable Planets
+Acid Jazz                        3     1h6rEPX9qRpBCBbjuAysMz   cmayes3          
+General Jazz                     513   1j6ndSnyYn6oUlnwpGiRWc   cmayes3          
+Instrumental Acid Jazz Mix       50    37i9dQZF1EIgnEnn8SKPjM   spotify          Instrumental Acid Jazz music picked just for you
+Jazz                             1     6VH2cw8n115fbQ7Ls2wzdR   cmayes3          
+Jazz Funk                        6     61Q9DgzF3f1ULr3i1uRyUy   cmayes3          
+Jazz Funk (Instrumental)         272   4xRrCdkn4r5lrDOElek5oC   1226030890       
+Jazz Piano Classics              100   37i9dQZF1DX5q7wCXFrkHh   spotify          The classic piano recordings in Jazz. Cover: Oscar Peterson
+Jazz-Funk                        200   37i9dQZF1DWUb0uBnlJuTi   spotify          Jazz. But funky. Cover: Takuya Kuroda
+State of Jazz                    100   37i9dQZF1DX7YCknf2jT6s   spotify          New jazz for open minds. Cover: Walter Smith III
+```
+
+`spotcrates li -f jazz,size:ge:100 -s size:desc`
+
+Any field contains `jazz`; size is greater than or equal to 100, sort by size descending.
+
+```
+PLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION
+FaLaLaLaLa GREAT BIG Christmas V 4051  6A2Kj9cWUpuu0UcEbWVf5E   kingofjingaling  Over 170 hours of classic Christmas music. The focus is on classic Christma
+General Jazz                     513   1j6ndSnyYn6oUlnwpGiRWc   cmayes3          
+Jazz Funk (Instrumental)         272   4xRrCdkn4r5lrDOElek5oC   1226030890       
+Jazz-Funk                        200   37i9dQZF1DWUb0uBnlJuTi   spotify          Jazz. But funky. Cover: Takuya Kuroda
+Jazz Piano Classics              100   37i9dQZF1DX5q7wCXFrkHh   spotify          The classic piano recordings in Jazz. Cover: Oscar Peterson
+State of Jazz                    100   37i9dQZF1DX7YCknf2jT6s   spotify          New jazz for open minds. Cover: Walter Smith III
+```
+
+#### Sort Types
+
+The default sort type is `ascending`, i.e. a-z.
+
+- ascending
+- descending
+
+## randomize
+`spotcrates randomize (playlist1) (playlist2)...` randomizes the playlists with the given names, 
+IDs, or in the given collections. 
+
+## copy
+`spotcrates copy (source) (dest)` copies a playlist into a new playlist. You may optionally specify 
+a destination playlist name; the default is to name the destination based on the source name with
+the general form `f"{source_name}-{count:02d}"`.
+
+## commands
+`spotcrates commands` displays a summary of the available commands.
```

