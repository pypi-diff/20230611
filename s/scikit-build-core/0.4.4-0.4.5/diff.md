# Comparing `tmp/scikit_build_core-0.4.4.tar.gz` & `tmp/scikit_build_core-0.4.5.tar.gz`

## Comparing `scikit_build_core-0.4.4.tar` & `scikit_build_core-0.4.5.tar`

### file list

```diff
@@ -1,237 +1,252 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.gitattributes
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.packit.yaml
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.readthedocs.yml
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/noxfile.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/packit.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/python-scikit-build-core.spec
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/.fmf/version
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/plans/main.fmf.dist-git
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/plans/rpmlint.fmf
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/plans/smoke.fmf
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/tests/rpmlint.fmf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/tests/smoke.fmf
--rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.github/codecov.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.github/matchers/pylint.json
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.github/workflows/cd.yml
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0    15738 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/changelog.md
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/cmakelists.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/conf.py
--rw-r--r--   0        0        0    12730 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/configuration.md
--rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/getting_started.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/index.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0    10438 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/settings/metadata.py
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/setuptools/build_cmake.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/setuptools/wrapper.py
--rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/conftest.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/constraints.txt
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_builder.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_cmake_config.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_custom_modules.py
--rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_fileapi.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_generator_default.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_get_requires.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_logging.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_name_main.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_program_search.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_settings.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_simple_pure.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_simplest_c.py
--rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/CMakeLists.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/pyproject.toml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/setup.cfg
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/setup.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/src/main.cpp
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_ext/LICENSE
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_source_dir/LICENSE
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_source_dir/pyproject.toml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_source_dir/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/_module.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/LICENSE
--rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/README.md
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.gitattributes
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.packit.yaml
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.readthedocs.yml
+-rw-r--r--   0        0        0     5990 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/noxfile.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/packit.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/python-scikit-build-core.spec
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/.fmf/version
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/plans/main.fmf.dist-git
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/plans/rpmlint.fmf
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/plans/smoke.fmf
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/tests/rpmlint.fmf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/tests/smoke.fmf
+-rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.github/codecov.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/changelog.md
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/cmakelists.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/conf.py
+-rw-r--r--   0        0        0    12730 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/configuration.md
+-rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/getting_started.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/index.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/CMakeLists.txt
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/LICENSE
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/README.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/pyproject.toml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/tests/test_basic.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/CMakeLists.txt
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/LICENSE
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/README.md
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/pyproject.toml
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/src/main.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/tests/test_basic.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0    10674 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/settings/metadata.py
+-rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/setuptools/build_cmake.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/setuptools/wrapper.py
+-rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/conftest.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/constraints.txt
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_builder.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_file_processor.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_fileapi.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_generator_default.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_get_requires.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_logging.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_name_main.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_program_search.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_settings.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/CMakeLists.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/pyproject.toml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/setup.cfg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/setup.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/src/main.cpp
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_ext/LICENSE
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_source_dir/LICENSE
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_source_dir/pyproject.toml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_source_dir/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/_module.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/LICENSE
+-rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/README.md
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/PKG-INFO
```

### Comparing `scikit_build_core-0.4.4/.packit.yaml` & `scikit_build_core-0.4.5/.packit.yaml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/.pre-commit-config.yaml` & `scikit_build_core-0.4.5/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
       - id: codespell
         exclude: ^(LICENSE$|src/scikit_build_core/resources/find_python)
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.2
+    rev: v0.9.0.5
     hooks:
       - id: shellcheck
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
```

### Comparing `scikit_build_core-0.4.4/noxfile.py` & `scikit_build_core-0.4.5/noxfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,22 +124,27 @@
     session.install("build")
     session.run("python", "-m", "build", **session.posargs)
 
 
 EXAMPLES = ["c", "abi3", "pybind11", "swig", "cython"]
 if not sys.platform.startswith("win") and shutil.which("gfortran"):
     EXAMPLES.append("fortran")
+EXAMPLES = [f"getting_started/{n}" for n in EXAMPLES]
+EXAMPLES += ["downstream/pybind11_example", "downstream/nanobind_example"]
 
 
 @nox.session
 @nox.parametrize("example", EXAMPLES, ids=EXAMPLES)
 def test_doc_examples(session: nox.Session, example: str) -> None:
-    session.chdir(f"docs/examples/getting_started/{example}")
-    session.install(".", "--config-settings=cmake.verbose=true")
-    session.run("python", "../test.py")
+    session.chdir(f"docs/examples/{example}")
+    session.install(".", "--config-settings=cmake.verbose=true", "pytest")
+    if Path("../test.py").is_file():
+        session.run("python", "../test.py")
+    else:
+        session.run("pytest")
 
 
 @nox.session(reuse_venv=True)
 def downstream(session: nox.Session) -> None:
     """
     Build a downstream project.
     """
```

### Comparing `scikit_build_core-0.4.4/.distro/python-scikit-build-core.spec` & `scikit_build_core-0.4.5/.distro/python-scikit-build-core.spec`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/.github/CONTRIBUTING.md` & `scikit_build_core-0.4.5/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/.github/matchers/pylint.json` & `scikit_build_core-0.4.5/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/.github/workflows/cd.yml` & `scikit_build_core-0.4.5/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/.github/workflows/ci.yml` & `scikit_build_core-0.4.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/changelog.md` & `scikit_build_core-0.4.5/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 # Changelog
 
+## Version 0.4.5
+
+This version fixes issues with output being incorrectly interleaved with logging
+messages. Symlinks are now followed when making SDists. And finally,
+`SKBUILD_SOABI` is now correctly set when cross-compiling on Windows (Warning!
+FindPython still does not report the correct SOABI when cross-compiling to ARM).
+
+Fixes:
+
+- Proper printout ordering and more displayed details by @henryiii in #365
+- Sort `RUNENV` debugging log output by @jameslamb in #357
+- Follow symlinks when making SDists by @henryiii in #362
+- Report correct ABI when cross-compiling by @henryiii in #366
+
+Tests:
+
+- Fedora downstream CI by @LecrisUT in #358
+- Add downstream examples by @henryiii in #363
+- Add testing for scripts processing by @henryiii in #364
+
 ## Version 0.4.4
 
 This version fixes some issues cross-compiling to Windows ARM when making
 Limited API / Stable ABI extensions, and supports multiple config generators in
 editable mode.
 
 - Conditional ABI3 logic fixed by @henryiii in #352
```

### Comparing `scikit_build_core-0.4.4/docs/cmakelists.md` & `scikit_build_core-0.4.5/docs/cmakelists.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/conf.py` & `scikit_build_core-0.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/configuration.md` & `scikit_build_core-0.4.5/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/getting_started.md` & `scikit_build_core-0.4.5/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/index.md` & `scikit_build_core-0.4.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.4.5/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.4.5/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.4.5/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.4.5/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.4.5/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/api/scikit_build_core.rst` & `scikit_build_core-0.4.5/docs/api/scikit_build_core.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.4.5/docs/api/scikit_build_core.settings.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.4.5/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.4.5/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.4.5/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.4.5/docs/examples/getting_started/cython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.4.5/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.4.5/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/_logging.py` & `scikit_build_core-0.4.5/src/scikit_build_core/_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,8 +124,8 @@
     )
 
 
 def rich_print(*args: object, **kwargs: object) -> None:
     args_2 = tuple(_process_rich(arg) for arg in args)
     if args != args_2:
         args_2 = (*args_2[:-1], args_2[-1] + colors()["reset"])
-    print(*args_2, **kwargs)  # type: ignore[call-overload] # noqa: T201
+    print(*args_2, **kwargs, flush=True)  # type: ignore[call-overload] # noqa: T201
```

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/cmake.py` & `scikit_build_core-0.4.5/src/scikit_build_core/cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/errors.py` & `scikit_build_core-0.4.5/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/program_search.py` & `scikit_build_core-0.4.5/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.4.5/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/_compat/importlib/metadata.py` & `scikit_build_core-0.4.5/src/scikit_build_core/_compat/importlib/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.4.5/src/scikit_build_core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.4.5/src/scikit_build_core/build/_file_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     gi = Path(".gitignore")
     with contextlib.suppress(FileNotFoundError), gi.open(encoding="utf-8") as f:
         exclude_lines += f.readlines()
 
     exclude_spec = pathspec.GitIgnoreSpec.from_lines(exclude_lines)
     include_spec = pathspec.GitIgnoreSpec.from_lines(include)
 
-    for dirpath, _, filenames in os.walk(str(starting_path)):
+    for dirpath, _, filenames in os.walk(str(starting_path), followlinks=True):
         all_paths = (Path(dirpath) / fn for fn in filenames)
         paths = (
             p
             for p in all_paths
             if not exclude_spec.match_file(p) or include_spec.match_file(p)
         )
         yield from paths
```

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.4.5/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.4.5/src/scikit_build_core/build/_pathutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.4.5/src/scikit_build_core/build/_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.4.5/src/scikit_build_core/build/_wheelfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.4.5/src/scikit_build_core/build/sdist.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.4.5/src/scikit_build_core/build/wheel.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,21 @@
         raise AssertionError(msg)
 
     normalized_name = metadata.name.replace("-", "_").replace(".", "_")
 
     cmake = CMake.default_search(
         minimum_version=Version(settings.cmake.minimum_version)
     )
+    action = (
+        "metadata" if wheel_directory is None else "editable" if editable else "wheel"
+    )
     rich_print(
-        f"[green]***[/green] [bold][green]scikit-build-core {__version__}[/green] using [blue]CMake {cmake.version}[/blue]"
+        f"[green]***[/green] [bold][green]scikit-build-core {__version__}[/green]",
+        f"using [blue]CMake {cmake.version}[/blue]",
+        f"[red]({action})[/red]",
     )
 
     with tempfile.TemporaryDirectory() as tmpdir:
         build_tmp_folder = Path(tmpdir)
         wheel_dir = build_tmp_folder / "wheel"
 
         tags = WheelTag.compute_best(
@@ -183,15 +188,15 @@
             for key, data in dist_info_contents.items():
                 path = dist_info / key
                 if not path.parent.is_dir():
                     path.parent.mkdir(exist_ok=True, parents=True)
                 path.write_bytes(data)
             return WheelImplReturn(wheel_filename=dist_info.name)
 
-        rich_print("[green]***[/green] [bold]Configurating CMake...")
+        rich_print("[green]***[/green] [bold]Configuring CMake...")
         defines: dict[str, str] = {}
         cache_entries = {f"SKBUILD_{k.upper()}_DIR": v for k, v in wheel_dirs.items()}
         builder.configure(
             defines=defines,
             cache_entries=cache_entries,
             name=metadata.name,
             version=metadata.version,
@@ -208,15 +213,15 @@
         )
         build_args: list[str] = []
         builder.build(build_args=build_args)
 
         rich_print("[green]***[/green] [bold]Installing project into wheel...")
         builder.install(install_dir)
 
-        rich_print("[green]***[/green] [bold]Making wheel...")
+        rich_print(f"[green]***[/green] [bold]Making {action}...")
         packages = _get_packages(
             packages=settings.wheel.packages,
             name=normalized_name,
         )
         mapping = packages_to_file_mapping(
             packages=packages,
             platlib_dir=wheel_dirs["platlib"],
@@ -291,8 +296,9 @@
             prevous_data = path.read_bytes()
             if prevous_data != data:
                 msg = f"Metadata mismatch in {key}"
                 logger.error("{}: {!r} != {!r}", msg, prevous_data, data)
                 raise AssertionError(msg)
 
     wheel_filename: str = wheel.wheelpath.name
+    rich_print(f"[green]***[/green] [bold]Created[/bold] {wheel_filename}...")
     return WheelImplReturn(wheel_filename=wheel_filename, mapping=mapping)
```

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.4.5/src/scikit_build_core/builder/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 from .. import __version__
 from .._compat.importlib import metadata, resources
 from .._logging import logger
 from ..cmake import CMaker
 from ..resources import find_python
 from ..settings.skbuild_model import ScikitBuildSettings
 from .generator import set_environment_for_gen
-from .sysconfig import get_platform, get_python_include_dir, get_python_library
+from .sysconfig import (
+    get_platform,
+    get_python_include_dir,
+    get_python_library,
+    get_soabi,
+)
 
 __all__: list[str] = ["Builder", "get_archs", "archs_to_tags"]
 
 DIR = Path(__file__).parent.resolve()
 
 
 def __dir__() -> list[str]:
@@ -153,31 +158,15 @@
             cache_config[f"{prefix}_FIND_REGISTRY"] = "NEVER"
             # FindPython may break if this is set - only useful on Windows
             if python_library and sysconfig.get_platform().startswith("win"):
                 cache_config[f"{prefix}_LIBRARY"] = python_library
             if python_sabi_library and sysconfig.get_platform().startswith("win"):
                 cache_config[f"{prefix}_SABI_LIBRARY"] = python_sabi_library
 
-        if limited_abi:
-            cache_config["SKBUILD_SOABI"] = (
-                "" if sysconfig.get_platform().startswith("win") else "abi3"
-            )
-        else:
-            # Workaround for bug in PyPy and packaging that is not handled in CMake
-            # According to PEP 3149, SOABI and EXT_SUFFIX are interchangeable (and
-            # the latter is much more likely to be correct as it is used elsewhere)
-            if sys.version_info < (3, 8, 7):
-                # See https://github.com/python/cpython/issues/84006
-                import distutils.sysconfig  # pylint: disable=deprecated-module
-
-                ext_suffix = distutils.sysconfig.get_config_var("EXT_SUFFIX")
-            else:
-                ext_suffix = sysconfig.get_config_var("EXT_SUFFIX")
-            assert isinstance(ext_suffix, str)
-            cache_config["SKBUILD_SOABI"] = ext_suffix.rsplit(".", 1)[0].lstrip(".")
+        cache_config["SKBUILD_SOABI"] = get_soabi(self.config.env, abi3=limited_abi)
 
         # Allow CMakeLists to detect this is supposed to be a limited ABI build
         cache_config["SKBUILD_SABI_COMPONENT"] = (
             "Development.SABIModule" if limited_abi else ""
         )
 
         if cache_entries:
```

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.4.5/src/scikit_build_core/builder/generator.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.4.5/src/scikit_build_core/builder/get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.4.5/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.4.5/src/scikit_build_core/builder/sysconfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,7 +126,28 @@
 
 def get_cmake_platform(env: Mapping[str, str] | None) -> str:
     """
     Return the CMake platform name for a platform, respecting VSCMD_ARG_TGT_ARCH.
     """
     plat = get_platform(env)
     return PLAT_TO_CMAKE.get(plat, plat)
+
+
+def get_soabi(env: Mapping[str, str], *, abi3: bool = False) -> str:
+    if abi3:
+        return "" if sysconfig.get_platform().startswith("win") else "abi3"
+
+    # Cross-compile support
+    setuptools_ext_suffix = env.get("SETUPTOOLS_EXT_SUFFIX", "")
+    if setuptools_ext_suffix:
+        return setuptools_ext_suffix.rsplit(".", 1)[0].lstrip(".")
+
+    if sys.version_info < (3, 8, 7):
+        # See https://github.com/python/cpython/issues/84006
+        import distutils.sysconfig  # pylint: disable=deprecated-module
+
+        ext_suffix = distutils.sysconfig.get_config_var("EXT_SUFFIX")
+    else:
+        ext_suffix = sysconfig.get_config_var("EXT_SUFFIX")
+
+    assert isinstance(ext_suffix, str)
+    return ext_suffix.rsplit(".", 1)[0].lstrip(".")
```

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.4.5/src/scikit_build_core/builder/wheel_tag.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.4.5/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.4.5/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.4.5/src/scikit_build_core/file_api/reply.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.4.5/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.4.5/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.4.5/src/scikit_build_core/resources/_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.4.5/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.4.5/src/scikit_build_core/settings/_load_provider.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/settings/metadata.py` & `scikit_build_core-0.4.5/src/scikit_build_core/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.4.5/src/scikit_build_core/settings/skbuild_model.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.4.5/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.4.5/src/scikit_build_core/settings/sources.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/setuptools/build_cmake.py` & `scikit_build_core-0.4.5/src/scikit_build_core/setuptools/build_cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.4.5/src/scikit_build_core/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/src/scikit_build_core/setuptools/wrapper.py` & `scikit_build_core-0.4.5/src/scikit_build_core/setuptools/wrapper.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/conftest.py` & `scikit_build_core-0.4.5/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,29 +99,31 @@
     def ensure_directories(
         self, env_dir: str | bytes | os.PathLike[str] | os.PathLike[bytes]
     ) -> types.SimpleNamespace:
         context = super().ensure_directories(env_dir)
         # Store the path to the venv Python interpreter.
         # See https://github.com/mesonbuild/meson-python/blob/8a180be7b4abd7e1939a63d5d59f63197ee27cc7/tests/conftest.py#LL79
         self.executable = Path(context.env_exe)
+        self.bin_path = Path(context.bin_path)
         self.env_dir = Path(context.env_dir)
         return context
 
     @overload
     def run(self, *args: str, capture: Literal[True]) -> str:
         ...
 
     @overload
     def run(self, *args: str, capture: Literal[False] = ...) -> None:
         ...
 
     def run(self, *args: str, capture: bool = False) -> str | None:
         __tracebackhide__ = True
         env = os.environ.copy()
-        env["PATH"] = f"{self.executable.parent}{os.pathsep}{env['PATH']}"
+        paths = {str(self.executable.parent), str(self.bin_path)}
+        env["PATH"] = os.pathsep.join([*paths, env["PATH"]])
         env["VIRTUAL_ENV"] = str(self.env_dir)
         env["PIP_DISABLE_PIP_VERSION_CHECK"] = "ON"
         if self.wheelhouse is not None:
             env["PIP_NO_INDEX"] = "ON"
             env["PIP_FIND_LINKS"] = str(self.wheelhouse)
 
         str_args = [os.fspath(a) for a in args]
```

### Comparing `scikit_build_core-0.4.4/tests/test_builder.py` & `scikit_build_core-0.4.5/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_cmake_config.py` & `scikit_build_core-0.4.5/tests/test_cmake_config.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_dynamic_metadata.py` & `scikit_build_core-0.4.5/tests/test_dynamic_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_fileapi.py` & `scikit_build_core-0.4.5/tests/test_fileapi.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_fortran.py` & `scikit_build_core-0.4.5/tests/test_fortran.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_generator_default.py` & `scikit_build_core-0.4.5/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_get_requires.py` & `scikit_build_core-0.4.5/tests/test_get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_module_dir.py` & `scikit_build_core-0.4.5/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_name_main.py` & `scikit_build_core-0.4.5/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_prepare_metadata.py` & `scikit_build_core-0.4.5/tests/test_prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_process_scripts.py` & `scikit_build_core-0.4.5/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_program_search.py` & `scikit_build_core-0.4.5/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_pyproject_abi3.py` & `scikit_build_core-0.4.5/tests/test_pyproject_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.4.5/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_pyproject_pep517.py` & `scikit_build_core-0.4.5/tests/test_pyproject_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_pyproject_pep518.py` & `scikit_build_core-0.4.5/tests/test_pyproject_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_pyproject_pep660.py` & `scikit_build_core-0.4.5/tests/test_pyproject_pep660.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_settings.py` & `scikit_build_core-0.4.5/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_setuptools_abi3.py` & `scikit_build_core-0.4.5/tests/test_setuptools_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_setuptools_pep517.py` & `scikit_build_core-0.4.5/tests/test_setuptools_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_setuptools_pep518.py` & `scikit_build_core-0.4.5/tests/test_setuptools_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_simple_pure.py` & `scikit_build_core-0.4.5/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_simplest_c.py` & `scikit_build_core-0.4.5/tests/test_simplest_c.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_skbuild_settings.py` & `scikit_build_core-0.4.5/tests/test_skbuild_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/test_wheelfile_utils.py` & `scikit_build_core-0.4.5/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.4.5/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.4.5/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.4.5/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.4.5/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.4.5/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.4.5/tests/packages/fortran_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/mixed_setuptools/CMakeLists.txt` & `scikit_build_core-0.4.5/tests/packages/mixed_setuptools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/simple_pyproject_ext/LICENSE` & `scikit_build_core-0.4.5/tests/packages/simple_pyproject_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.4.5/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/simple_pyproject_source_dir/LICENSE` & `scikit_build_core-0.4.5/tests/packages/simple_pyproject_source_dir/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/simple_pyproject_source_dir/src/main.cpp` & `scikit_build_core-0.4.5/tests/packages/simple_pyproject_source_dir/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/LICENSE` & `scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.4.5/tests/packages/simplest_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.4.5/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/.gitignore` & `scikit_build_core-0.4.5/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -170,7 +170,9 @@
 Thumbs.db
 
 .idea/
 # tmt setup
 /.distro/main.fmf
 /.distro/plans/main.fmf
 /.distro/tests/main.fmf
+
+/docs/**/build
```

### Comparing `scikit_build_core-0.4.4/LICENSE` & `scikit_build_core-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/README.md` & `scikit_build_core-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/pyproject.toml` & `scikit_build_core-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.4/PKG-INFO` & `scikit_build_core-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_build_core
-Version: 0.4.4
+Version: 0.4.5
 Summary: Build backend for CMake based projects
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Documentation, https://scikit-build-core.readthedocs.io
 Project-URL: Discussions, https://github.com/orgs/scikit-build/discussions
 Project-URL: Issues, https://github.com/scikit-build/scikit-build-core/issues
 Project-URL: Changelog, https://scikit-build-core.readthedocs.io/en/latest/changelog.html
 Author-email: Henry Schreiner <henryfs@princeton.edu>
```

