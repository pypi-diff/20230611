# Comparing `tmp/psychrochart-0.7.0.tar.gz` & `tmp/psychrochart-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychrochart-0.7.0.tar", max compression
+gzip compressed data, was "psychrochart-0.8.0.tar", max compression
```

## Comparing `psychrochart-0.7.0.tar` & `psychrochart-0.8.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     7837 2023-06-09 12:36:51.287968 psychrochart-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-06-09 12:36:51.287968 psychrochart-0.7.0/LICENSE
--rw-r--r--   0        0        0     7077 2023-06-09 12:36:51.287968 psychrochart-0.7.0/README.md
--rw-r--r--   0        0        0      711 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/__init__.py
--rw-r--r--   0        0        0      336 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/__main__.py
--rw-r--r--   0        0        0    12221 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart.py
--rw-r--r--   0        0        0      178 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_entities.py
--rw-r--r--   0        0        0     2157 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_styles/ashrae_chart_style.json
--rw-r--r--   0        0        0     2380 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_styles/ashrae_ip_chart_style.json
--rw-r--r--   0        0        0     3080 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_styles/default_chart_config.json
--rw-r--r--   0        0        0      585 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_styles/default_comfort_zones.json
--rw-r--r--   0        0        0     2436 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_styles/interior_chart_style.json
--rw-r--r--   0        0        0     2490 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_styles/minimal_chart_style.json
--rw-r--r--   0        0        0    17122 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chartdata.py
--rw-r--r--   0        0        0        0 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/__init__.py
--rw-r--r--   0        0        0     4427 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/annots.py
--rw-r--r--   0        0        0     1246 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/base.py
--rw-r--r--   0        0        0     6715 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/config.py
--rw-r--r--   0        0        0     3584 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/curves.py
--rw-r--r--   0        0        0     5852 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/parsers.py
--rw-r--r--   0        0        0     1909 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/styles.py
--rw-r--r--   0        0        0     1924 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/validators.py
--rw-r--r--   0        0        0    13156 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/plot_logic.py
--rw-r--r--   0        0        0     9048 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/process_logic.py
--rw-r--r--   0        0        0     3977 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/util.py
--rw-r--r--   0        0        0     2222 2023-06-09 12:36:51.299968 psychrochart-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8406 1970-01-01 00:00:00.000000 psychrochart-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     9831 2023-06-11 10:04:18.635505 psychrochart-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-06-11 10:04:18.635505 psychrochart-0.8.0/LICENSE
+-rw-r--r--   0        0        0     7077 2023-06-11 10:04:18.635505 psychrochart-0.8.0/README.md
+-rw-r--r--   0        0        0      711 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/__main__.py
+-rw-r--r--   0        0        0    13944 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart.py
+-rw-r--r--   0        0        0     2231 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_entities.py
+-rw-r--r--   0        0        0     2157 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_styles/ashrae_chart_style.json
+-rw-r--r--   0        0        0     2380 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_styles/ashrae_ip_chart_style.json
+-rw-r--r--   0        0        0     3097 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_styles/default_chart_config.json
+-rw-r--r--   0        0        0      585 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_styles/default_comfort_zones.json
+-rw-r--r--   0        0        0     2436 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_styles/interior_chart_style.json
+-rw-r--r--   0        0        0     2490 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_styles/minimal_chart_style.json
+-rw-r--r--   0        0        0    15847 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chartdata.py
+-rw-r--r--   0        0        0     2296 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chartzones.py
+-rw-r--r--   0        0        0        0 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/__init__.py
+-rw-r--r--   0        0        0     3350 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/annots.py
+-rw-r--r--   0        0        0     1246 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/base.py
+-rw-r--r--   0        0        0     8628 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/config.py
+-rw-r--r--   0        0        0     3604 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/curves.py
+-rw-r--r--   0        0        0     5844 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/parsers.py
+-rw-r--r--   0        0        0     1909 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/styles.py
+-rw-r--r--   0        0        0     1924 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/validators.py
+-rw-r--r--   0        0        0    15951 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/plot_logic.py
+-rw-r--r--   0        0        0     7978 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/process_logic.py
+-rw-r--r--   0        0        0     3977 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/util.py
+-rw-r--r--   0        0        0     2222 2023-06-11 10:04:18.651506 psychrochart-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8406 1970-01-01 00:00:00.000000 psychrochart-0.8.0/PKG-INFO
```

### Comparing `psychrochart-0.7.0/CHANGELOG.md` & `psychrochart-0.8.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.8.0] - ✨ Lazy generation of chart data, 'Artist' registry, and better SVG export - 2023-06-11
+
+Now all chart-data parameters, including the overlayed zones, are included in the `ChartConfig`,
+and generation of curves only happens when chart is plotted (or saved to disk).
+
+Any change in the chart configuration will trigger a data-regen for all items before plotting.
+
+When plotting over some matplotlib `Axes`, all objects created have meaningful (and deterministic) ids,
+and are tracked and accessible under `chart.artists`, for easier customization of single matplotlib objects,
+also adding a **recognizable hierarchy** in generated SVGs, (enabling potential for **CSS over SVG charts** 🌈)
+
+##### Changes
+
+- ✨ Name each matplotlib `Artist` obj in plot with custom readable IDs, for easier recognition and **readable object hierarchy in SVGs**, and maintain a registry of all objects in plot to access them by kind under `chart.artists` property, allowing fine-grain control to customize all details in the psychrochart
+- ♻️ Refactor chart 'zones' and store zone definitions in ChartConfig, to regenerate plot patches (closed `PsychroCurve`, with `ZoneStyle`) on-demand, same as the other chart curves, generating new 'xy' points when config is changed. If `ChartParams.with_zones` is enabled, but there are no zones in config when chart is created, the default winter/summer 'dbt-rh' zones are added.
+- ⚡️ Add **lazy generation** of psychro curves to avoid updating the chart data until it's needed to plot, and add a `chart.process_chart()` method to trigger data regeneration if the chart config has changed or there is no chart data yet
+- 💥 Make `chart.saturation` a single `PsychroCurve`, instead of a collection of curves
+- ✅ tests: Add unit tests for new ChartRegistry and adapt to behaviour changes and readable hierarchy in SVG output
+- 📝 Update example notebook showing `chart.artists` usage
+- 🚀 env: Update deps, bump version, and update CHANGELOG
+
 ## [0.7.0] - ♻️ Testing suite refactor + model changes - 2023-06-09
 
 Maintenance-only update, without new features.
 
 ##### Changes
 
 - 💥 Remove plotting methods from `PsychroCurve`/`PsychroCurves` for a more functional approach, using methods in `plot_logic.py`
```

### Comparing `psychrochart-0.7.0/LICENSE` & `psychrochart-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psychrochart-0.7.0/README.md` & `psychrochart-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `psychrochart-0.7.0/psychrochart/__init__.py` & `psychrochart-0.8.0/psychrochart/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A library to make psychrometric charts and overlay information in them."""
 from psychrochart.chart import PsychroChart
-from psychrochart.models.annots import ChartAnnots, ChartZones
-from psychrochart.models.config import ChartConfig
+from psychrochart.models.annots import ChartAnnots
+from psychrochart.models.config import ChartConfig, ChartZones
 from psychrochart.models.curves import PsychroCurve, PsychroCurves
 from psychrochart.models.parsers import load_config, load_zones
 from psychrochart.models.styles import (
     CurveStyle,
     LabelStyle,
     TickStyle,
     ZoneStyle,
```

### Comparing `psychrochart-0.7.0/psychrochart/chart.py` & `psychrochart-0.8.0/psychrochart/chart.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """A library to make psychrometric charts and overlay information in them."""
 import gc
 from io import StringIO
 from pathlib import Path
 from typing import Any, Iterable, Type
 
 from matplotlib import figure
-from matplotlib.artist import Artist
 from matplotlib.axes import Axes
 from matplotlib.backend_bases import FigureCanvasBase
 from matplotlib.backends.backend_agg import FigureCanvasAgg
 from matplotlib.backends.backend_svg import FigureCanvasSVG
-from matplotlib.legend import Legend
 
+from psychrochart.chart_entities import (
+    ChartRegistry,
+    make_item_gid,
+    reg_artist,
+)
 from psychrochart.chartdata import (
     gen_points_in_constant_relative_humidity,
     make_constant_dry_bulb_v_line,
+    make_saturation_line,
 )
-from psychrochart.models.annots import ChartAnnots, ChartZones
-from psychrochart.models.config import ChartConfig
+from psychrochart.models.annots import ChartAnnots
+from psychrochart.models.config import ChartConfig, ChartZones
 from psychrochart.models.curves import PsychroChartModel
 from psychrochart.models.parsers import (
     ConvexGroupTuple,
     load_extra_annots,
     load_points_dbt_rh,
     obj_loader,
 )
@@ -30,16 +34,15 @@
     add_label_to_curve,
     apply_axis_styling,
     plot_annots_dbt_rh,
     plot_chart,
     plot_curve,
 )
 from psychrochart.process_logic import (
-    append_zones_to_chart,
-    generate_psychrochart,
+    get_pressure_pa,
     update_psychrochart_data,
 )
 from psychrochart.util import mod_color
 
 
 def _select_fig_canvas(
     path_dest: Any, canvas_cls: Type[FigureCanvasBase] | None = None
@@ -57,68 +60,96 @@
 
 class PsychroChart(PsychroChartModel):
     """Psychrometric chart object handler."""
 
     config: ChartConfig
     _fig: figure.Figure | None = None
     _axes: Axes | None = None
-    _legend: Legend | None = None
-    _handlers_annotations: list[Artist | list[Artist]]
+    _artists: ChartRegistry
 
     class Config:
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
 
     def _init_private_attributes(self) -> None:
-        self._handlers_annotations = []
+        self._artists = ChartRegistry()
         super()._init_private_attributes()
+        self.config._has_changed = True
 
     @classmethod
     def create(
         cls,
         config: ChartConfig | dict[str, Any] | str | None = None,
         *,
         extra_zones: ChartZones | dict[str, Any] | str | None = None,
         use_unit_system_si: bool = True,
     ):
         chart_config = obj_loader(ChartConfig, config)
-        chart_config.commit_changes()
-        chart_data = generate_psychrochart(
-            chart_config, extra_zones, use_unit_system_si
+        if extra_zones is not None:
+            zones_use = obj_loader(ChartZones, extra_zones).zones
+            chart_config.chart_params.with_zones = True
+            chart_config.chart_params.zones = zones_use
+        pressure = get_pressure_pa(chart_config.limits, use_unit_system_si)
+        return cls(
+            config=chart_config,
+            unit_system_si=use_unit_system_si,
+            altitude_m=chart_config.limits.altitude_m,
+            pressure=pressure,
+            saturation=make_saturation_line(
+                chart_config.dbt_min,
+                chart_config.dbt_max,
+                chart_config.limits.step_temp,
+                pressure,
+                style=chart_config.saturation,
+            ),
         )
-        chart = cls(config=chart_config, **chart_data.dict())
-        return chart
 
     def __repr__(self) -> str:
         """Return a string representation of the PsychroChart object."""
         return (
             f"<PsychroChart [{self.config.dbt_min:g}"
             f"->{self.config.dbt_max:g} °C, "
             f"{self.config.w_min:g}"
             f"->{self.config.w_max:g} gr/kg_da]>"
         )
 
-    def _ensure_updated_data(self):
+    def process_chart(self) -> bool:
+        """Apply chart config on limits to generate all curves for plot."""
         if self.config.has_changed:
             update_psychrochart_data(self, self.config)
+            return True
+        return False
+
+    @property
+    def rendered(self) -> bool:
+        """Check if Axes object is assigned."""
+        return self._axes is not None
 
     @property
     def axes(self) -> Axes:
         """Return the Axes object plotting the chart if necessary."""
-        self._ensure_updated_data()
-        if self._axes is None:
+        self.process_chart()
+        if not self.rendered:
             self.plot()
         assert isinstance(self._axes, Axes)
         return self._axes
 
+    @property
+    def artists(self) -> ChartRegistry:
+        """Access to registry of all matplotlib Artists in plot."""
+        return self._artists
+
     def append_zones(
         self, zones: ChartZones | dict[str, Any] | str | None = None
     ) -> None:
         """Append zones as patches to the psychrometric chart."""
-        append_zones_to_chart(self.config, self, zones)
+        zones_use = obj_loader(ChartZones, zones).zones
+        self.config.chart_params.with_zones = True
+        self.config.chart_params.zones += zones_use
+        assert self.config.has_changed
 
     def plot_points_dbt_rh(
         self,
         points: dict[str, Any],
         connectors: list[dict[str, Any]] | None = None,
         convex_groups: list[dict[str, Any]]
         | list[ConvexGroupTuple]
@@ -197,17 +228,15 @@
         annots = ChartAnnots(
             points=data_points,
             series=data_series,
             connectors=data_lines,
             areas=data_areas,
             use_scatter=scatter_style is not None,
         )
-        self._handlers_annotations.extend(
-            plot_annots_dbt_rh(self.axes, annots)
-        )
+        self._artists.annotations.update(plot_annots_dbt_rh(self.axes, annots))
         return annots
 
     def plot_arrows_dbt_rh(
         self, points_pairs: dict[str, Any]
     ) -> dict[str, Any]:
         """Append individual points to the plot."""
         points_plot = {}
@@ -230,24 +259,24 @@
             temp2 = point2[0]
             w_g_ka1 = gen_points_in_constant_relative_humidity(
                 [temp1], point1[1], self.pressure
             )[0]
             w_g_ka2 = gen_points_in_constant_relative_humidity(
                 [temp2], point2[1], self.pressure
             )[0]
-
-            self._handlers_annotations.append(
-                self.axes.annotate(
-                    "",
-                    (temp2, w_g_ka2),
-                    xytext=(temp1, w_g_ka1),
-                    arrowprops=plot_params,
-                )
+            arrow = self.axes.annotate(
+                "",
+                (temp2, w_g_ka2),
+                xytext=(temp1, w_g_ka1),
+                arrowprops=plot_params,
             )
-
+            arrow_gid = make_item_gid(
+                f"arrow_{key}", name=f"{temp1}_{w_g_ka1}__{temp2}_{w_g_ka2}"
+            )
+            reg_artist(arrow_gid, arrow, self._artists.annotations)
             points_plot[key] = (temp1, w_g_ka1), (temp2, w_g_ka2), plot_params
 
         return points_plot
 
     def plot_vertical_dry_bulb_temp_line(
         self,
         temp: float,
@@ -264,86 +293,99 @@
             self.config.w_min,
             temp,
             self.pressure,
             style=style_curve,
             type_curve="constant-dbt",
             reverse=reverse,
         )
-
-        if plot_curve(curve, self.axes) and label is not None:
-            add_label_to_curve(curve, self.axes, label, **label_params)
+        new_artists = plot_curve(curve, self.axes)
+        self._artists.annotations.update(new_artists)
+        if new_artists and label is not None:
+            reg_artist(
+                make_item_gid(
+                    "label-vline", family_label="constant-dbt", name=label
+                ),
+                add_label_to_curve(curve, self.axes, label, **label_params),
+                self._artists.annotations,
+            )
 
     def plot_legend(
         self,
         loc: str = "upper left",
         markerscale: float = 0.9,
         frameon: bool = True,
         fancybox: bool = True,
         edgecolor: str | Iterable = "darkgrey",
         fontsize: float = 15.0,
         labelspacing: float = 1.5,
         **params,
     ) -> None:
         """Append a legend to the psychrochart plot."""
-        self._legend = self.axes.legend(
-            loc=loc,
-            markerscale=markerscale,
-            frameon=frameon,
-            edgecolor=edgecolor,
-            fontsize=fontsize,
-            fancybox=fancybox,
-            labelspacing=labelspacing,
-            **params,
+        reg_artist(
+            "chart_legend",
+            self.axes.legend(
+                loc=loc,
+                markerscale=markerscale,
+                frameon=frameon,
+                edgecolor=edgecolor,
+                fontsize=fontsize,
+                fancybox=fancybox,
+                labelspacing=labelspacing,
+                **params,
+            ),
+            self._artists.layout,
         )
 
     def plot(self, ax: Axes | None = None) -> Axes:
         """Plot the psychrochart and return the matplotlib Axes instance."""
-        self._ensure_updated_data()
+        self.process_chart()
         if ax is not None:
             self._fig = ax.get_figure()
         else:
             self._fig = figure.Figure(
                 figsize=self.config.figure.figsize,
                 dpi=self.config.figure.dpi,
                 frameon=False,
             )
+            self._fig.set_gid("figure_psychrochart")
             ax = self._fig.add_subplot(position=self.config.figure.position)
+            ax.set_gid("chart_axes")
+            reg_artist("chart_background", ax.patch, self._artists.layout)
         self._axes = ax
-        apply_axis_styling(self.config, self._axes)
-        return plot_chart(self, self._axes)
+        self._artists.layout.update(
+            apply_axis_styling(self.config, self._axes)
+        )
+        plot_chart(self, self._axes, self._artists)
+        return self._axes
 
     def remove_annotations(self) -> None:
         """Remove the annotations made in the chart to reuse it."""
-        for line in self._handlers_annotations:
-            if isinstance(line, list):
-                line[0].remove()
-            else:
-                line.remove()
-        self._handlers_annotations = []
+        for line in self._artists.annotations.values():
+            line.remove()
+        self._artists.annotations = {}
 
     def remove_legend(self) -> None:
         """Remove the legend of the chart."""
-        if self._legend is not None:
-            self._legend.remove()
-            self._legend = None
+        if "chart_legend" in self._artists.layout:
+            self._artists.layout.pop("chart_legend").remove()
 
     def save(
         self,
         path_dest: Any,
         canvas_cls: Type[FigureCanvasBase] | None = None,
         **params,
     ) -> None:
         """Write the chart to disk."""
         # ensure destination path if folder does not exist
         if (
             isinstance(path_dest, (str, Path))
             and not Path(path_dest).parent.exists()
         ):
             Path(path_dest).parent.mkdir(parents=True)
-        if self._axes is None or self.config.has_changed:
+        if not self.rendered or self.config.has_changed:
             self.plot()
         assert self._fig is not None
         canvas_use = _select_fig_canvas(path_dest, canvas_cls)
         canvas_use(self._fig).print_figure(path_dest, **params)
         gc.collect()
 
     def make_svg(self, **params) -> str:
```

### Comparing `psychrochart-0.7.0/psychrochart/chart_styles/ashrae_chart_style.json` & `psychrochart-0.8.0/psychrochart/chart_styles/ashrae_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.7.0/psychrochart/chart_styles/ashrae_ip_chart_style.json` & `psychrochart-0.8.0/psychrochart/chart_styles/ashrae_ip_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.7.0/psychrochart/chart_styles/default_chart_config.json` & `psychrochart-0.8.0/psychrochart/chart_styles/default_chart_config.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985714285714286%*

 * *Differences: {"'chart_params'": "{'zones': []}"}*

```diff
@@ -78,15 +78,16 @@
         ],
         "with_constant_dry_temp": true,
         "with_constant_h": true,
         "with_constant_humidity": true,
         "with_constant_rh": true,
         "with_constant_v": true,
         "with_constant_wet_temp": true,
-        "with_zones": true
+        "with_zones": true,
+        "zones": []
     },
     "constant_dry_temp": {
         "color": [
             0.855,
             0.145,
             0.114
         ],
```

### Comparing `psychrochart-0.7.0/psychrochart/chart_styles/default_comfort_zones.json` & `psychrochart-0.8.0/psychrochart/chart_styles/default_comfort_zones.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.7.0/psychrochart/chart_styles/interior_chart_style.json` & `psychrochart-0.8.0/psychrochart/chart_styles/interior_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.7.0/psychrochart/chart_styles/minimal_chart_style.json` & `psychrochart-0.8.0/psychrochart/chart_styles/minimal_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.7.0/psychrochart/chartdata.py` & `psychrochart-0.8.0/psychrochart/chartdata.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     GetTDryBulbFromMoistAirVolumeAndHumRatio,
     GetTWetBulbFromHumRatio,
     GetVapPresFromHumRatio,
     isIP,
 )
 from scipy.interpolate import interp1d
 
-from psychrochart.chart_entities import random_internal_value
-from psychrochart.models.annots import ChartZone
 from psychrochart.models.curves import PsychroCurve, PsychroCurves
 from psychrochart.models.styles import CurveStyle
 from psychrochart.util import solve_curves_with_iteration
 
 f_vec_hum_ratio_from_vap_press = np.vectorize(GetHumRatioFromVapPres)
 f_vec_moist_air_enthalpy = np.vectorize(GetMoistAirEnthalpy)
 f_vec_moist_air_volume = np.vectorize(GetMoistAirVolume)
@@ -110,26 +108,28 @@
 
 def make_constant_relative_humidity_lines(
     dbt_min: float,
     dbt_max: float,
     temp_step: float,
     pressure: float,
     rh_perc_values: list[int],
-    rh_label_values: list[int],
+    *,
     style: CurveStyle,
-    label_loc: float,
-    family_label: str | None,
+    rh_label_values: list[int] | None = None,
+    label_loc: float = 0.0,
+    family_label: str | None = None,
 ) -> PsychroCurves:
     """Generate curves of constant relative humidity for the chart."""
     rh_values = sorted(rh for rh in rh_perc_values if 0 <= rh <= 100)
     temps_ct_rh = np.arange(dbt_min, dbt_max + temp_step, temp_step)
     curves_ct_rh = [
         gen_points_in_constant_relative_humidity(temps_ct_rh, rh, pressure)
         for rh in rh_values
     ]
+    rh_label_values = rh_label_values or []
     return PsychroCurves(
         curves=[
             PsychroCurve(
                 x_data=temps_ct_rh,
                 y_data=curve_ct_rh,
                 style=style,
                 type_curve="constant_rh_data",
@@ -143,14 +143,15 @@
     )
 
 
 def make_constant_dry_bulb_v_line(
     w_humidity_ratio_min: float,
     temp: float,
     pressure: float,
+    *,
     style: CurveStyle,
     type_curve: str | None = None,
     reverse: bool = False,
 ) -> PsychroCurve:
     """Generate vertical line (constant dry bulb temp) up to saturation."""
     w_max = _factor_out_w() * GetHumRatioFromVapPres(
         GetSatVapPres(temp), pressure
@@ -168,16 +169,17 @@
     )
 
 
 def make_constant_dry_bulb_v_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     temps_vl: np.ndarray,
+    *,
     style: CurveStyle,
-    family_label: str | None,
+    family_label: str | None = None,
 ) -> PsychroCurves:
     """Generate curves of constant dry bulb temperature (vertical)."""
     w_max_vec = _get_humid_ratio_in_saturation(temps_vl, pressure)
     return PsychroCurves(
         curves=[
             PsychroCurve(
                 x_data=np.array([temp, temp]),
@@ -192,16 +194,17 @@
     )
 
 
 def make_constant_humidity_ratio_h_lines(
     dbt_max: float,
     pressure: float,
     ws_hl: np.ndarray,
+    *,
     style: CurveStyle,
-    family_label: str | None,
+    family_label: str | None = None,
 ) -> PsychroCurves:
     """Generate curves of constant absolute humidity (horizontal)."""
     arr_hum_ratios = np.array(ws_hl) / _factor_out_w()
     dew_points = f_vec_dew_point_from_vap_press(
         dbt_max, f_vec_vap_press_from_hum_ratio(arr_hum_ratios, pressure)
     )
     return PsychroCurves(
@@ -220,40 +223,40 @@
 
 
 def make_saturation_line(
     dbt_min: float,
     dbt_max: float,
     temp_step: float,
     pressure: float,
-    style: CurveStyle,
-) -> PsychroCurves:
+    style: CurveStyle | None = None,
+) -> PsychroCurve:
     """Generate line of saturation for the psychrochart."""
     temps_sat_line = np.arange(dbt_min, dbt_max + temp_step, temp_step)
     w_sat = gen_points_in_constant_relative_humidity(
         temps_sat_line, 100, pressure
     )
-    sat_c = PsychroCurve(
+    return PsychroCurve(
         x_data=temps_sat_line,
         y_data=w_sat,
-        style=style,
+        style=style if style is not None else CurveStyle(),
         type_curve="saturation",
         internal_value=100.0,
     )
-    return PsychroCurves(curves=[sat_c])
 
 
 def make_constant_enthalpy_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     enthalpy_values: np.ndarray,
-    h_label_values: list[float],
-    style: CurveStyle,
-    label_loc: float,
-    family_label: str | None,
+    *,
     saturation_curve: PsychroCurve,
+    style: CurveStyle,
+    h_label_values: list[float] | None = None,
+    label_loc: float = 0.0,
+    family_label: str | None = None,
     dbt_min_seen: float | None = None,
 ) -> PsychroCurves | None:
     """Generate curves of constant enthalpy for the chart."""
     h_in_sat = (
         f_vec_moist_air_enthalpy(
             saturation_curve.x_data, saturation_curve.y_data / _factor_out_w()
         )
@@ -307,15 +310,16 @@
                 x_data=np.array([t_sat, t_max]),
                 y_data=np.array([w_sat, w_humidity_ratio_min]),
                 style=style,
                 type_curve="constant_h_data",
                 label_loc=label_loc,
                 label=(
                     _make_enthalpy_label(h)
-                    if round(h, 3) in h_label_values
+                    if isinstance(h_label_values, list)
+                    and round(h, 3) in h_label_values
                     else None
                 ),
                 internal_value=round(h, 3),
             )
             for t_sat, w_sat, t_max, h in zip(
                 t_sat_points, w_in_sat, temps_max_constant_h, h_objective
             )
@@ -324,19 +328,20 @@
     )
 
 
 def make_constant_specific_volume_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     vol_values: np.ndarray,
-    v_label_values: list[float],
-    style: CurveStyle,
-    label_loc: float,
-    family_label: str | None,
+    *,
     saturation_curve: PsychroCurve,
+    style: CurveStyle,
+    v_label_values: list[float] | None = None,
+    label_loc: float = 0.0,
+    family_label: str | None = None,
     dbt_min_seen: float | None = None,
 ) -> PsychroCurves | None:
     """Generate curves of constant specific volume for the chart."""
     v_in_sat = f_vec_moist_air_volume(
         saturation_curve.x_data,
         saturation_curve.y_data / _factor_out_w(),
         pressure,
@@ -386,15 +391,16 @@
                 x_data=np.array([t_sat, t_max]),
                 y_data=np.array([w_sat, w_humidity_ratio_min]),
                 style=style,
                 type_curve="constant_v_data",
                 label_loc=label_loc,
                 label=(
                     _make_vol_label(vol)
-                    if round(vol, 3) in v_label_values
+                    if isinstance(v_label_values, list)
+                    and round(vol, 3) in v_label_values
                     else None
                 ),
                 internal_value=round(vol, 3),
             )
             for t_sat, w_sat, t_max, vol in zip(
                 t_sat_points, w_in_sat, temps_max_constant_v, v_objective
             )
@@ -406,18 +412,19 @@
 def make_constant_wet_bulb_temperature_lines(
     dry_bulb_temp_min: float,
     dry_bulb_temp_max: float,
     w_humidity_ratio_min: float,
     w_humidity_ratio_max: float,
     pressure: float,
     wbt_values: np.ndarray,
-    wbt_label_values: list[float],
+    *,
     style: CurveStyle,
-    label_loc: float,
-    family_label: str | None,
+    wbt_label_values: list[float] | None = None,
+    label_loc: float = 0.0,
+    family_label: str | None = None,
 ) -> PsychroCurves | None:
     """Generate curves of constant wet bulb temperature for the chart."""
     wt_min = GetTWetBulbFromHumRatio(
         dry_bulb_temp_min, w_humidity_ratio_min / _factor_out_w(), pressure
     )
     if -0.75 < wt_min < 0.0:  # slope change zone
         wt_min = 0
@@ -477,60 +484,18 @@
 
         c = PsychroCurve(
             x_data=np.array([wbt, dbt_objective]),
             y_data=np.array([w_left, w_right]),
             style=style,
             type_curve="constant_wbt_data",
             label_loc=label_loc,
-            label=(_make_temp_label(wbt) if wbt in wbt_label_values else None),
+            label=(
+                _make_temp_label(wbt)
+                if isinstance(wbt_label_values, list)
+                and round(wbt, 3) in wbt_label_values
+                else None
+            ),
             internal_value=wbt,
         )
         curves.append(c)
 
     return PsychroCurves(curves=curves, family_label=family_label)
-
-
-def make_zone_curve(
-    zone_conf: ChartZone, increment: float, pressure: float
-) -> PsychroCurve:
-    """Generate plot-points for zone."""
-    # todo better id for overlay zones if no label
-    zone_value = random_internal_value() if zone_conf.label is None else None
-    if zone_conf.zone_type == "xy-points":
-        # expect points in plot coordinates!
-        return PsychroCurve(
-            x_data=np.array(zone_conf.points_x),
-            y_data=np.array(zone_conf.points_y),
-            style=zone_conf.style,
-            type_curve="xy-points",
-            label=zone_conf.label,
-            internal_value=zone_value,
-        )
-
-    assert zone_conf.zone_type == "dbt-rh"
-    # points for zone between constant dry bulb temps and RH
-    t_min = zone_conf.points_x[0]
-    t_max = zone_conf.points_x[-1]
-    rh_min = zone_conf.points_y[0]
-    rh_max = zone_conf.points_y[-1]
-    assert rh_min >= 0.0 and rh_max <= 100.0
-    assert t_min < t_max
-
-    temps = np.arange(t_min, t_max + increment, increment)
-    curve_rh_up = gen_points_in_constant_relative_humidity(
-        temps, rh_max, pressure
-    )
-    curve_rh_down = gen_points_in_constant_relative_humidity(
-        temps, rh_min, pressure
-    )
-    abs_humid: list[float] = (
-        list(curve_rh_up) + list(curve_rh_down)[::-1] + [curve_rh_up[0]]
-    )
-    temps_zone: list[float] = list(temps) + list(temps)[::-1] + [temps[0]]
-    return PsychroCurve(
-        x_data=np.array(temps_zone),
-        y_data=np.array(abs_humid),
-        style=zone_conf.style,
-        type_curve="dbt-rh",
-        label=zone_conf.label,
-        internal_value=zone_value,
-    )
```

### Comparing `psychrochart-0.7.0/psychrochart/models/annots.py` & `psychrochart-0.8.0/psychrochart/models/annots.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Any, Literal
+from typing import Any
 
 import numpy as np
 from pydantic import BaseModel, Field, root_validator
 
-from psychrochart.models.styles import CurveStyle, ZoneStyle
+from psychrochart.models.styles import CurveStyle
 from psychrochart.models.validators import (
     check_connector_and_areas_by_point_name,
     parse_curve_arrays,
 )
 
 ConvexGroupTuple = tuple[list[str], dict[str, Any], dict[str, Any]]
 
 
 class ChartPoint(BaseModel):
-    """Pydantic model for single point annotation."""
+    """Input model for single point annotations."""
 
     xy: tuple[float | int, float | int]
     label: str | None = Field(default=None)
     style: dict[str, Any] = Field(default_factory=dict)
 
 
 class ChartSeries(BaseModel):
-    """Pydantic model for data-series point array annotation."""
+    """Input model for data-series point array annotation."""
 
     # TODO fusion with PsychroCurve, + pandas ready
     x_data: np.ndarray
     y_data: np.ndarray
     style: dict[str, Any] = Field(default_factory=dict)
     label: str | None = None
 
@@ -99,50 +99,7 @@
     def get_point_by_name(self, key: str) -> tuple[float, float]:
         """Access coords tuple for named point (or 1st point of series)."""
         if key in self.points:
             return self.points[key].xy
         else:
             assert key in self.series
             return self.series[key].x_data[0], self.series[key].y_data[0]
-
-
-class ChartZone(BaseModel):
-    """Pydantic model for styled fixed areas on the psychrochart."""
-
-    label: str | None
-    zone_type: Literal["dbt-rh", "xy-points"]
-    points_x: list[float]
-    points_y: list[float]
-    style: ZoneStyle
-
-
-class ChartZones(BaseModel):
-    """Container model for a list of ChartZone items."""
-
-    zones: list[ChartZone]
-
-
-# default fixed areas for winter/summer comfort zones
-DEFAULT_ZONES = ChartZones(
-    zones=[
-        ChartZone(
-            label="Summer",
-            zone_type="dbt-rh",
-            points_x=[23, 25],
-            points_y=[45, 60],
-            style=ZoneStyle(
-                edgecolor=[1.0, 0.749, 0.0, 0.8],
-                facecolor=[1.0, 0.749, 0.0, 0.5],
-            ),
-        ),
-        ChartZone(
-            label="Winter",
-            zone_type="dbt-rh",
-            points_x=[21, 23],
-            points_y=[40, 50],
-            style=ZoneStyle(
-                edgecolor=[0.498, 0.624, 0.8],
-                facecolor=[0.498, 0.624, 1.0, 0.5],
-            ),
-        ),
-    ]
-)
```

### Comparing `psychrochart-0.7.0/psychrochart/models/base.py` & `psychrochart-0.8.0/psychrochart/models/base.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.7.0/psychrochart/models/curves.py` & `psychrochart-0.8.0/psychrochart/models/curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             )
         return parse_curve_arrays(values)
 
     @property
     def curve_id(self) -> str:
         """Get Curve identifier (value or label)."""
         if self.internal_value is not None:
-            return f"{self.internal_value:g}"
+            return f"{self.internal_value:g}".replace("-", "minus")
         assert self.label is not None
         return self.label
 
     def dict(
         self,
         *,
         include: AbstractSet[int | str]
@@ -96,15 +96,15 @@
 class PsychroChartModel(BaseModel):
     """Pydantic model to store all psychrometric curves for PsychroChart."""
 
     unit_system_si: bool
     altitude_m: int
     pressure: float
 
-    saturation: PsychroCurves
+    saturation: PsychroCurve
     constant_dry_temp_data: PsychroCurves | None = None
     constant_humidity_data: PsychroCurves | None = None
     constant_rh_data: PsychroCurves | None = None
     constant_h_data: PsychroCurves | None = None
     constant_v_data: PsychroCurves | None = None
     constant_wbt_data: PsychroCurves | None = None
-    zones: list[PsychroCurves] = Field(default_factory=list)
+    zones: list[PsychroCurve] = Field(default_factory=list)
```

### Comparing `psychrochart-0.7.0/psychrochart/models/parsers.py` & `psychrochart-0.8.0/psychrochart/models/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 
 from psychrochart.chartdata import gen_points_in_constant_relative_humidity
 from psychrochart.models.annots import (
     ChartArea,
     ChartLine,
     ChartPoint,
     ChartSeries,
-    ChartZones,
     ConvexGroupTuple,
-    DEFAULT_ZONES,
 )
-from psychrochart.models.config import ChartConfig
+from psychrochart.models.config import ChartConfig, ChartZones, DEFAULT_ZONES
 
 PATH_STYLES = Path(__file__).absolute().parents[1] / "chart_styles"
 DEFAULT_CHART_CONFIG_FILE = str(PATH_STYLES / "default_chart_config.json")
 ASHRAE_CHART_CONFIG_FILE = str(PATH_STYLES / "ashrae_chart_style.json")
 ASHRAE_IP_CHART_CONFIG_FILE = str(PATH_STYLES / "ashrae_ip_chart_style.json")
 INTERIOR_CHART_CONFIG_FILE = str(PATH_STYLES / "interior_chart_style.json")
 MINIMAL_CHART_CONFIG_FILE = str(PATH_STYLES / "minimal_chart_style.json")
```

### Comparing `psychrochart-0.7.0/psychrochart/models/styles.py` & `psychrochart-0.8.0/psychrochart/models/styles.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.7.0/psychrochart/models/validators.py` & `psychrochart-0.8.0/psychrochart/models/validators.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.7.0/psychrochart/plot_logic.py` & `psychrochart-0.8.0/psychrochart/plot_logic.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 from matplotlib.artist import Artist
 from matplotlib.axes import Axes
 from matplotlib.path import Path
 from matplotlib.text import Annotation
 import numpy as np
 from scipy.spatial import ConvexHull, QhullError
 
+from psychrochart.chart_entities import (
+    ChartRegistry,
+    make_item_gid,
+    reg_artist,
+)
 from psychrochart.models.annots import ChartAnnots
 from psychrochart.models.config import ChartConfig
 from psychrochart.models.curves import (
     PsychroChartModel,
     PsychroCurve,
     PsychroCurves,
 )
@@ -105,16 +110,17 @@
         text_style.update(params)
 
     return _annotate_label(ax, label, text_x, text_y, rotation, text_style)
 
 
 def plot_curve(
     curve: PsychroCurve, ax: Axes, label_prefix: str | None = None
-) -> list[Artist]:
+) -> dict[str, Artist]:
     """Plot the curve, if it's between chart limits."""
+    artists: dict[str, Artist] = {}
     xmin, xmax = ax.get_xlim()
     ymin, ymax = ax.get_ylim()
     if (
         curve.x_data is None
         or curve.y_data is None
         or max(curve.y_data) < ymin
         or max(curve.x_data) < xmin
@@ -129,126 +135,158 @@
             xmin,
             xmax,
             ymin,
             ymax,
             curve.x_data,
             curve.y_data,
         )
-        return []
+        return {}
 
-    artists = []
     if isinstance(curve.style, ZoneStyle):
         assert len(curve.y_data) > 2
         verts = list(zip(curve.x_data, curve.y_data))
         codes = (
             [Path.MOVETO]
             + [Path.LINETO] * (len(curve.y_data) - 2)
             + [Path.CLOSEPOLY]
         )
         path = Path(verts, codes)
         patch = patches.PathPatch(path, **curve.style.dict())
         ax.add_patch(patch)
-        artists.append(patch)
-
+        gid_zone = make_item_gid(
+            "zone",
+            family_label=label_prefix or curve.type_curve,
+            name=curve.curve_id,
+        )
+        reg_artist(
+            gid_zone,
+            patch,
+            artists,
+        )
         if curve.label is not None:
             bbox_p = path.get_extents()
             text_x = 0.5 * (bbox_p.x0 + bbox_p.x1)
             text_y = 0.5 * (bbox_p.y0 + bbox_p.y1)
             style_params = {
                 "ha": "center",
                 "va": "center",
                 "backgroundcolor": [1, 1, 1, 0.4],
             }
             assert isinstance(curve.style, ZoneStyle)
             style_params["color"] = mod_color(curve.style.edgecolor, -25)
-            artist_label = _annotate_label(
-                ax, curve.label, text_x, text_y, 0, style_params
+            reg_artist(
+                "label_" + gid_zone,
+                _annotate_label(
+                    ax, curve.label, text_x, text_y, 0, style_params
+                ),
+                artists,
             )
-            artists.append(artist_label)
     else:
-        artist_line = ax.plot(curve.x_data, curve.y_data, **curve.style.dict())
-        artists.append(artist_line)
+        [artist_line] = ax.plot(
+            curve.x_data, curve.y_data, **curve.style.dict()
+        )
+        kind = (
+            (label_prefix or curve.type_curve)
+            if len(curve.x_data) > 1
+            else "point"
+        )
+        gid_line = make_item_gid(kind or "unknown", name=curve.curve_id)
+        reg_artist(gid_line, artist_line, artists)
         if curve.label is not None:
-            artists.append(add_label_to_curve(curve, ax))
+            reg_artist(
+                "label_" + gid_line, add_label_to_curve(curve, ax), artists
+            )
 
     return artists
 
 
-def plot_curves_family(family: PsychroCurves | None, ax: Axes) -> list[Artist]:
+def plot_curves_family(
+    family: PsychroCurves | None, ax: Axes
+) -> dict[str, Artist]:
     """Plot all curves in the family."""
-    artists: list[Artist] = []
     if family is None:
-        return artists
-
-    [
-        plot_curve(curve, ax, label_prefix=family.family_label)
+        return {}
+    artists: dict[str, Artist] = {
+        gid: item
         for curve in family.curves
-    ]
+        for gid, item in plot_curve(
+            curve, ax, label_prefix=family.family_label
+        ).items()
+    }
     # Curves family labelling
     if family.curves and family.family_label is not None:
-        artist_fam_label = ax.plot(
+        # artist for legend (1 label for each family)
+        min_params = {"marker": "D", "markersize": 10}
+        [artist_fam_label] = ax.plot(
             [-1],
             [-1],
             label=family.family_label,
-            marker="D",
-            markersize=10,
-            **family.curves[0].style.dict(),
-        )
-        artists.append(artist_fam_label)
-
-    # return [
-    #     art for art in artist_curves + artist_labels if art is not None
-    # ]
-    # TODO collect artists from plot_curve
-    return []
+            **(min_params | family.curves[0].style.dict()),
+        )
+        gid_family_label = make_item_gid(
+            "label_legend", name=family.family_label
+        )
+        artist_fam_label.set_gid(gid_family_label)
+        artists[gid_family_label] = artist_fam_label
+
+    return artists
 
 
 def _apply_spines_style(axes, style, location="right") -> None:
     for key in style:
         try:
             getattr(axes.spines[location], f"set_{key}")(style[key])
         except Exception as exc:  # pragma: no cover
             logging.error(
                 f"Error trying to apply spines attrs: {exc}. "
                 f"({dir(axes.spines[location])})"
             )
 
 
-def apply_axis_styling(config: ChartConfig, ax: Axes) -> None:
+def apply_axis_styling(config: ChartConfig, ax: Axes) -> dict[str, Artist]:
     """Setup matplotlib Axes object for the chart."""
+    layout_artists: dict[str, Artist] = {}
+    reg_artist("chart_x_axis", ax.xaxis, layout_artists)
+    reg_artist("chart_y_axis", ax.yaxis, layout_artists)
     ax.yaxis.tick_right()
     ax.yaxis.set_label_position("right")
     ax.set_xlim(config.dbt_min, config.dbt_max)
     ax.set_ylim(config.w_min, config.w_max)
     ax.grid(False, which="both")
     # Apply axis styles
     if config.figure.x_label is not None:
         style_axis = config.figure.x_axis_labels.dict()
         style_axis["fontsize"] *= 1.2
-        ax.set_xlabel(config.figure.x_label, **style_axis)
+        artist_xlabel = ax.set_xlabel(config.figure.x_label, **style_axis)
+        reg_artist("chart_x_axis_label", artist_xlabel, layout_artists)
     if config.figure.y_label is not None:
         style_axis = config.figure.y_axis_labels.dict()
         style_axis["fontsize"] *= 1.2
-        ax.set_ylabel(config.figure.y_label, **style_axis)
+        artist_ylabel = ax.set_ylabel(config.figure.y_label, **style_axis)
+        reg_artist("chart_y_axis_label", artist_ylabel, layout_artists)
     if config.figure.title is not None:
-        ax.set_title(
+        artist_title = ax.set_title(
             config.figure.title,
             fontsize=config.figure.fontsize * 1.5,
             fontweight="bold",
         )
+        reg_artist("chart_title", artist_title, layout_artists)
 
     _apply_spines_style(ax, config.figure.y_axis.dict(), location="right")
     _apply_spines_style(ax, config.figure.x_axis.dict(), location="bottom")
+    reg_artist("chart_x_axis_bottom_line", ax.spines["bottom"], layout_artists)
+    reg_artist("chart_y_axis_right_line", ax.spines["right"], layout_artists)
     if config.figure.partial_axis:  # Hide left and top axis
         ax.spines["left"].set_visible(False)
         ax.spines["top"].set_visible(False)
     else:
         _apply_spines_style(ax, config.figure.y_axis.dict(), location="left")
         _apply_spines_style(ax, config.figure.x_axis.dict(), location="top")
-
+        reg_artist("chart_x_axis_top_line", ax.spines["top"], layout_artists)
+        reg_artist("chart_y_axis_left_line", ax.spines["left"], layout_artists)
     if config.figure.x_axis_ticks is not None:
         ax.tick_params(axis="x", **config.figure.x_axis_ticks.dict())
     if config.figure.y_axis_ticks is not None:
         ax.tick_params(axis="y", **config.figure.y_axis_ticks.dict())
 
     # set tick labels in main axes
     if config.chart_params.with_constant_dry_temp:
@@ -282,105 +320,124 @@
                 ]
             ax.set_yticks(ticks)
             ax.set_yticklabels(
                 [f"{t:g}" for t in ticks], **config.figure.y_axis_labels.dict()
             )
     else:
         ax.set_yticks([])
+    return layout_artists
 
 
-def plot_chart(chart: PsychroChartModel, ax: Axes) -> Axes:
+def plot_chart(
+    chart: PsychroChartModel, ax: Axes, registry: ChartRegistry | None = None
+) -> ChartRegistry:
     """Plot the psychrochart curves on given Axes."""
+    if registry is None:
+        registry = ChartRegistry()
     # Plot curves:
-    plot_curves_family(chart.constant_dry_temp_data, ax)
-    plot_curves_family(chart.constant_humidity_data, ax)
-    plot_curves_family(chart.constant_h_data, ax)
-    plot_curves_family(chart.constant_v_data, ax)
-    plot_curves_family(chart.constant_rh_data, ax)
-    plot_curves_family(chart.constant_wbt_data, ax)
-    plot_curves_family(chart.saturation, ax)
+    if data := plot_curves_family(chart.constant_dry_temp_data, ax):
+        registry.constant_dry_temp = data
+    if data := plot_curves_family(chart.constant_humidity_data, ax):
+        registry.constant_humidity = data
+    if data := plot_curves_family(chart.constant_h_data, ax):
+        registry.constant_h = data
+    if data := plot_curves_family(chart.constant_v_data, ax):
+        registry.constant_v = data
+    if data := plot_curves_family(chart.constant_rh_data, ax):
+        registry.constant_rh = data
+    if data := plot_curves_family(chart.constant_wbt_data, ax):
+        registry.constant_wbt = data
+    registry.saturation = plot_curve(chart.saturation, ax)
 
     # Plot zones:
     for zone in chart.zones:
-        plot_curves_family(zone, ax)
-    return ax
+        registry.zones.update(plot_curve(zone, ax))
+    return registry
 
 
-def plot_annots_dbt_rh(
-    ax: Axes, annots: ChartAnnots
-) -> list[Artist | list[Artist]]:
+def plot_annots_dbt_rh(ax: Axes, annots: ChartAnnots) -> dict[str, Artist]:
     """Plot chat annotations in given matplotlib Axes, return `Artist` objs."""
-    _handlers_annotations = []
+    annot_artists: dict[str, Artist] = {}
     for d_con in annots.connectors:
         x_start, y_start = annots.get_point_by_name(d_con.start)
         x_end, y_end = annots.get_point_by_name(d_con.end)
         x_line = [x_start, x_end]
         y_line = [y_start, y_end]
-        _handlers_annotations.append(
-            ax.plot(
-                x_line,
-                y_line,
-                label=d_con.label,
-                dash_capstyle="round",
-                **d_con.style.dict(),
-            )
+        d_con_gid = make_item_gid(
+            "connector", name=d_con.label or f"{d_con.start}_{d_con.end}"
+        )
+        [artist_connector] = ax.plot(
+            x_line,
+            y_line,
+            label=d_con.label,
+            dash_capstyle="round",
+            **d_con.style.dict(),
         )
+        reg_artist(d_con_gid, artist_connector, annot_artists)
         if d_con.outline_marker_width:
-            _handlers_annotations.append(
-                ax.plot(
-                    x_line,
-                    y_line,
-                    color=[*d_con.style.color[:3], 0.15],
-                    lw=d_con.outline_marker_width,
-                    solid_capstyle="round",
-                )
+            [artist_connector_marker] = ax.plot(
+                x_line,
+                y_line,
+                color=[*d_con.style.color[:3], 0.15],
+                lw=d_con.outline_marker_width,
+                solid_capstyle="round",
+            )
+            reg_artist(
+                d_con_gid + "_outline_mark",
+                artist_connector_marker,
+                annot_artists,
             )
 
     forbidden = set()
     if annots.use_scatter:
         f_plot = ax.scatter
         forbidden.add("markersize")
     else:
         f_plot = ax.plot
-    for series in annots.series.values():
+    for name, series in annots.series.items():
         style = {k: v for k, v in series.style.items() if k not in forbidden}
-        _handlers_annotations.append(
-            f_plot(series.x_data, series.y_data, label=series.label, **style)
+        artists = f_plot(
+            series.x_data, series.y_data, label=series.label, **style
         )
+        artist_line = artists[0] if isinstance(artists, list) else artists
+        line_gid = make_item_gid("series", name=series.label or name)
+        reg_artist(line_gid, artist_line, annot_artists)
 
-    for point in annots.points.values():
+    for name, point in annots.points.items():
         style = {k: v for k, v in point.style.items() if k not in forbidden}
-        _handlers_annotations.append(
-            f_plot(point.xy[0], point.xy[1], label=point.label, **style)
-        )
+        artists = f_plot(point.xy[0], point.xy[1], label=point.label, **style)
+        artist_point = artists[0] if isinstance(artists, list) else artists
+        line_gid = make_item_gid("point", name=point.label or name)
+        reg_artist(line_gid, artist_point, annot_artists)
 
     if ConvexHull is None or not annots.areas:
-        return _handlers_annotations
+        return annot_artists
 
     for convex_area in annots.areas:
         int_points = np.array(
             [annots.get_point_by_name(key) for key in convex_area.point_names]
         )
         try:
             assert len(int_points) >= 3
             hull = ConvexHull(int_points)
         except (AssertionError, QhullError):  # pragma: no cover
             logging.error(f"QhullError with points: {int_points}")
             continue
 
-        for simplex in hull.simplices:
-            _handlers_annotations.append(
-                ax.plot(
-                    int_points[simplex, 0],
-                    int_points[simplex, 1],
-                    **convex_area.line_style,
-                )
-            )
-        _handlers_annotations.append(
-            ax.fill(
-                int_points[hull.vertices, 0],
-                int_points[hull.vertices, 1],
-                **convex_area.fill_style,
-            )
+        area_gid = make_item_gid(
+            "convexhull", name=",".join(convex_area.point_names)
+        )
+        for i, simplex in enumerate(hull.simplices):
+            [artist_contour] = ax.plot(
+                int_points[simplex, 0],
+                int_points[simplex, 1],
+                **convex_area.line_style,
+            )
+            reg_artist(area_gid + f"_s{i+1}", artist_contour, annot_artists)
+        [artist_area] = ax.fill(
+            int_points[hull.vertices, 0],
+            int_points[hull.vertices, 1],
+            **convex_area.fill_style,
         )
+        reg_artist(area_gid, artist_area, annot_artists)
 
-    return _handlers_annotations
+    return annot_artists
```

### Comparing `psychrochart-0.7.0/psychrochart/process_logic.py` & `psychrochart-0.8.0/psychrochart/process_logic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import Any
 
 import numpy as np
 import psychrolib as psy
 from psychrolib import (
     GetStandardAtmPressure,
     GetUnitSystem,
     IP,
@@ -17,20 +16,18 @@
     make_constant_dry_bulb_v_lines,
     make_constant_enthalpy_lines,
     make_constant_humidity_ratio_h_lines,
     make_constant_relative_humidity_lines,
     make_constant_specific_volume_lines,
     make_constant_wet_bulb_temperature_lines,
     make_saturation_line,
-    make_zone_curve,
 )
-from psychrochart.models.annots import ChartZones, DEFAULT_ZONES
-from psychrochart.models.config import ChartConfig, ChartLimits
-from psychrochart.models.curves import PsychroChartModel, PsychroCurves
-from psychrochart.models.parsers import obj_loader
+from psychrochart.chartzones import make_zone_curve
+from psychrochart.models.config import ChartConfig, ChartLimits, DEFAULT_ZONES
+from psychrochart.models.curves import PsychroChartModel
 
 spec_vol_vec = np.vectorize(psy.GetMoistAirVolume)
 
 
 def set_unit_system(use_unit_system_si: bool = True) -> None:
     """Set unit system for psychrolib."""
     if use_unit_system_si and GetUnitSystem() != SI:
@@ -46,68 +43,49 @@
     set_unit_system(unit_system_si)
     if limits.pressure_kpa is not None:
         return limits.pressure_kpa * 1000.0  # to Pa
     else:
         return GetStandardAtmPressure(limits.altitude_m)
 
 
-def append_zones_to_chart(
-    config: ChartConfig,
-    chart: PsychroChartModel,
-    zones: ChartZones | dict[str, Any] | str | None = None,
-) -> None:
-    """Append zones as patches to the psychrometric chart data-container."""
-    zones_use = obj_loader(ChartZones, zones, default_obj=DEFAULT_ZONES).zones
-    if zones_use:
-        curves = PsychroCurves(
-            curves=[
-                make_zone_curve(zone, config.limits.step_temp, chart.pressure)
-                for zone in zones_use
-            ]
-        )
-        chart.zones.append(curves)
-
-
-def _generate_chart_curves(
-    config: ChartConfig, chart: PsychroChartModel, pressure: float
-):
+def _generate_chart_curves(config: ChartConfig, chart: PsychroChartModel):
     # check chart limits are not fully above the saturation curve!
-    assert (chart.saturation.curves[0].y_data > config.w_min).any()
+    assert (chart.saturation.y_data > config.w_min).any()
     # check if sat curve cuts x-axis with T > config.dbt_min
     dbt_min_seen: float | None = None
-    if chart.saturation.curves[0].y_data[0] < config.w_min:
+    if chart.saturation.y_data[0] < config.w_min:
         temp_sat_interpolator = interp1d(
-            chart.saturation.curves[0].y_data,
-            chart.saturation.curves[0].x_data,
+            chart.saturation.y_data,
+            chart.saturation.x_data,
             assume_sorted=True,
         )
         dbt_min_seen = temp_sat_interpolator(config.w_min)
 
     # Dry bulb constant lines (vertical):
     if config.chart_params.with_constant_dry_temp:
         step = config.chart_params.constant_temp_step
         temps_vl = np.arange(config.dbt_min, config.dbt_max, step)
         if dbt_min_seen:
             temps_vl = temps_vl[temps_vl > dbt_min_seen]
         chart.constant_dry_temp_data = make_constant_dry_bulb_v_lines(
             config.w_min,
-            pressure,
+            chart.pressure,
             temps_vl=temps_vl,
             style=config.constant_dry_temp,
             family_label=config.chart_params.constant_temp_label,
         )
     else:
         chart.constant_dry_temp_data = None
 
     # Absolute humidity constant lines (horizontal):
     if config.chart_params.with_constant_humidity:
         step = config.chart_params.constant_humid_step
         chart.constant_humidity_data = make_constant_humidity_ratio_h_lines(
             config.dbt_max,
-            pressure,
+            chart.pressure,
             ws_hl=np.arange(
                 config.w_min + step,
                 config.w_max + step / 10,
                 step,
             ),
             style=config.constant_humidity,
             family_label=config.chart_params.constant_humid_label,
@@ -118,15 +96,15 @@
     # Constant relative humidity curves:
     if config.chart_params.with_constant_rh:
         rh_min, rh_max = get_rh_max_min_in_limits(
             dbt_min_seen or config.dbt_min,
             config.dbt_max,
             config.w_min,
             config.w_max,
-            pressure,
+            chart.pressure,
         )
         rh_values = sorted(
             rh
             for rh in config.chart_params.constant_rh_curves
             if rh_min < rh < rh_max
         )
         start = (
@@ -134,15 +112,15 @@
             if dbt_min_seen
             else config.dbt_min
         )
         chart.constant_rh_data = make_constant_relative_humidity_lines(
             start,
             config.dbt_max,
             config.limits.step_temp,
-            pressure,
+            chart.pressure,
             rh_perc_values=rh_values,
             rh_label_values=config.chart_params.constant_rh_labels,
             style=config.constant_rh,
             label_loc=config.chart_params.constant_rh_labels_loc,
             family_label=config.chart_params.constant_rh_label,
         )
     else:
@@ -150,94 +128,64 @@
 
     # Constant enthalpy lines:
     if config.chart_params.with_constant_h:
         step = config.chart_params.constant_h_step
         start, end = config.chart_params.range_h
         chart.constant_h_data = make_constant_enthalpy_lines(
             config.w_min,
-            pressure,
+            chart.pressure,
             enthalpy_values=np.arange(start, end, step),
             h_label_values=config.chart_params.constant_h_labels,
             style=config.constant_h,
             label_loc=config.chart_params.constant_h_labels_loc,
             family_label=config.chart_params.constant_h_label,
-            saturation_curve=chart.saturation.curves[0],
+            saturation_curve=chart.saturation,
             dbt_min_seen=dbt_min_seen,
         )
     else:
         chart.constant_h_data = None
 
     # Constant specific volume lines:
     if config.chart_params.with_constant_v:
         step = config.chart_params.constant_v_step
         start, end = config.chart_params.range_vol_m3_kg
         chart.constant_v_data = make_constant_specific_volume_lines(
             config.w_min,
-            pressure,
+            chart.pressure,
             vol_values=np.arange(start, end, step),
             v_label_values=config.chart_params.constant_v_labels,
             style=config.constant_v,
             label_loc=config.chart_params.constant_v_labels_loc,
             family_label=config.chart_params.constant_v_label,
-            saturation_curve=chart.saturation.curves[0],
+            saturation_curve=chart.saturation,
             dbt_min_seen=dbt_min_seen,
         )
     else:
         chart.constant_v_data = None
 
     # Constant wet bulb temperature lines:
     if config.chart_params.with_constant_wet_temp:
         step = config.chart_params.constant_wet_temp_step
         start, end = config.chart_params.range_wet_temp
         chart.constant_wbt_data = make_constant_wet_bulb_temperature_lines(
             dbt_min_seen or config.dbt_min,
             config.dbt_max,
             config.w_min,
             config.w_max,
-            pressure,
+            chart.pressure,
             wbt_values=np.arange(start, end, step),
             wbt_label_values=config.chart_params.constant_wet_temp_labels,
             style=config.constant_wet_temp,
             label_loc=config.chart_params.constant_wet_temp_labels_loc,
             family_label=config.chart_params.constant_wet_temp_label,
         )
     else:
         chart.constant_wbt_data = None
 
 
-def generate_psychrochart(
-    config: ChartConfig,
-    extra_zones: ChartZones | dict[str, Any] | str | None = None,
-    use_unit_system_si: bool = True,
-) -> PsychroChartModel:
-    """Create the PsychroChart object."""
-    # Set unit system for psychrolib and get standard pressure
-    pressure = get_pressure_pa(config.limits, use_unit_system_si)
-
-    # base chart with saturation line:
-    chart = PsychroChartModel(
-        unit_system_si=use_unit_system_si,
-        altitude_m=config.limits.altitude_m,
-        pressure=pressure,
-        saturation=make_saturation_line(
-            config.dbt_min,
-            config.dbt_max,
-            config.limits.step_temp,
-            pressure,
-            style=config.saturation,
-        ),
-    )
-    _generate_chart_curves(config, chart, pressure)
-
-    if config.chart_params.with_zones:
-        append_zones_to_chart(config, chart, extra_zones)
-
-    return chart
-
-
 def update_psychrochart_data(
     current_chart: PsychroChartModel, config: ChartConfig
 ) -> None:
     """Update the PsychroChart data with config changes."""
     if config.limits.has_changed:
         current_chart.altitude_m = config.limits.altitude_m
         current_chart.pressure = get_pressure_pa(
@@ -248,9 +196,25 @@
     current_chart.saturation = make_saturation_line(
         config.dbt_min,
         config.dbt_max,
         config.limits.step_temp,
         current_chart.pressure,
         style=config.saturation,
     )
-    _generate_chart_curves(config, current_chart, current_chart.pressure)
+    _generate_chart_curves(config, current_chart)
+    # regen all zones
+    if config.chart_params.with_zones and not config.chart_params.zones:
+        # add default zones
+        config.chart_params.zones = DEFAULT_ZONES.zones
+    zone_curves = [
+        make_zone_curve(
+            zone,
+            pressure=current_chart.pressure,
+            step_temp=config.limits.step_temp,
+            # dbt_min=config.dbt_min,
+            # dbt_max=config.dbt_max,
+            # w_min=config.w_min,
+        )
+        for zone in config.chart_params.zones
+    ]
+    current_chart.zones = [zc for zc in zone_curves if zc is not None]
     config.commit_changes()
```

### Comparing `psychrochart-0.7.0/psychrochart/util.py` & `psychrochart-0.8.0/psychrochart/util.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.7.0/pyproject.toml` & `psychrochart-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 log_level = "INFO"
 log_cli = true
 log_format = "%(asctime)s %(levelname)s: (%(filename)s:%(lineno)s): %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.poetry]
 name = "psychrochart"
-version = "0.7.0"
+version = "0.8.0"
 description = "A python 3 library to make psychrometric charts and overlay information on them"
 authors = ["Eugenio Panadero <eugenio.panadero@gmail.com>"]
 packages = [
     { include = "psychrochart" }
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `psychrochart-0.7.0/PKG-INFO` & `psychrochart-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychrochart
-Version: 0.7.0
+Version: 0.8.0
 Summary: A python 3 library to make psychrometric charts and overlay information on them
 Home-page: https://github.com/azogue/psychrochart
 License: MIT
 Keywords: psychrometrics,moist,humid air,climate control,matplotlib
 Author: Eugenio Panadero
 Author-email: eugenio.panadero@gmail.com
 Requires-Python: >=3.10,<3.12
```

