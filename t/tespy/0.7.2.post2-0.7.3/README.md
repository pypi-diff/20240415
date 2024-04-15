# Comparing `tmp/tespy-0.7.2.post2.tar.gz` & `tmp/tespy-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tespy-0.7.2.post2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tespy-0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tespy-0.7.2.post2.tar` & `tespy-0.7.3.tar`

### file list

```diff
@@ -1,342 +1,343 @@
--rw-r--r--   0        0        0      265 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/.editorconfig
--rw-r--r--   0        0        0     1446 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/.pep8speaks.yml
--rw-r--r--   0        0        0      341 2023-11-14 11:35:05.186734 tespy-0.7.2.post2/.readthedocs.yml
--rw-r--r--   0        0        0     3269 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      154 2022-01-28 07:48:36.000000 tespy-0.7.2.post2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1088 2024-01-23 20:58:10.441293 tespy-0.7.2.post2/LICENSE
--rw-r--r--   0        0        0      281 2023-11-14 11:35:05.190735 tespy-0.7.2.post2/MANIFEST.in
--rw-r--r--   0        0        0      765 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     9116 2024-01-21 17:52:35.706781 tespy-0.7.2.post2/README.rst
--rw-r--r--   0        0        0      180 2023-11-14 11:35:05.203247 tespy-0.7.2.post2/docs/_static/css/custom.css
--rw-r--r--   0        0        0   129643 2023-11-14 11:35:05.207242 tespy-0.7.2.post2/docs/_static/images/advanced/exergy/flowsheet.svg
--rw-r--r--   0        0        0   136810 2023-11-14 11:35:05.210242 tespy-0.7.2.post2/docs/_static/images/advanced/exergy/flowsheet_darkmode.svg
--rw-r--r--   0        0        0    32134 2023-11-14 11:35:05.212242 tespy-0.7.2.post2/docs/_static/images/advanced/exergy/sankey.svg
--rw-r--r--   0        0        0    17276 2023-11-14 11:35:05.213286 tespy-0.7.2.post2/docs/_static/images/basics/district_heating.svg
--rw-r--r--   0        0        0    18111 2023-11-14 11:35:05.215279 tespy-0.7.2.post2/docs/_static/images/basics/district_heating_darkmode.svg
--rw-r--r--   0        0        0    69064 2023-11-14 11:35:05.218243 tespy-0.7.2.post2/docs/_static/images/basics/district_heating_partload.svg
--rw-r--r--   0        0        0    71199 2023-11-14 11:35:05.220243 tespy-0.7.2.post2/docs/_static/images/basics/district_heating_partload_darkmode.svg
--rw-r--r--   0        0        0    15810 2023-11-14 11:35:05.222242 tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine.svg
--rw-r--r--   0        0        0    16340 2023-11-14 11:35:05.223244 tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_darkmode.svg
--rw-r--r--   0        0        0    32095 2023-11-14 11:35:05.225250 tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_fuel_composition.svg
--rw-r--r--   0        0        0    32756 2023-11-14 11:35:05.227255 tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_fuel_composition_darkmode.svg
--rw-r--r--   0        0        0    29612 2023-11-14 11:35:05.228284 tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_oxygen.svg
--rw-r--r--   0        0        0    30202 2023-11-14 11:35:05.230296 tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_oxygen_darkmode.svg
--rw-r--r--   0        0        0    57559 2023-11-14 11:35:05.231295 tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_parametric.svg
--rw-r--r--   0        0        0    59255 2023-11-14 11:35:05.233242 tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_parametric_darkmode.svg
--rw-r--r--   0        0        0    14362 2023-11-14 11:35:05.234243 tespy-0.7.2.post2/docs/_static/images/basics/heat_pump.svg
--rw-r--r--   0        0        0    14866 2023-11-14 11:35:05.236243 tespy-0.7.2.post2/docs/_static/images/basics/heat_pump_darkmode.svg
--rw-r--r--   0        0        0    53423 2023-11-14 11:35:05.237245 tespy-0.7.2.post2/docs/_static/images/basics/heat_pump_parametric.svg
--rw-r--r--   0        0        0    54994 2023-11-14 11:35:05.240244 tespy-0.7.2.post2/docs/_static/images/basics/heat_pump_parametric_darkmode.svg
--rw-r--r--   0        0        0    16030 2023-11-14 11:35:05.241287 tespy-0.7.2.post2/docs/_static/images/basics/modeling_concept.svg
--rw-r--r--   0        0        0    16137 2023-11-14 11:35:05.242303 tespy-0.7.2.post2/docs/_static/images/basics/rankine_cycle.svg
--rw-r--r--   0        0        0    16871 2023-11-14 11:35:05.243245 tespy-0.7.2.post2/docs/_static/images/basics/rankine_cycle_darkmode.svg
--rw-r--r--   0        0        0    59916 2023-11-14 11:35:05.245276 tespy-0.7.2.post2/docs/_static/images/basics/rankine_parametric.svg
--rw-r--r--   0        0        0    61115 2023-11-14 11:35:05.247242 tespy-0.7.2.post2/docs/_static/images/basics/rankine_parametric_darkmode.svg
--rw-r--r--   0        0        0    26962 2023-11-14 11:35:05.248242 tespy-0.7.2.post2/docs/_static/images/basics/rankine_partload.svg
--rw-r--r--   0        0        0    27517 2023-11-14 11:35:05.250241 tespy-0.7.2.post2/docs/_static/images/basics/rankine_partload_darkmode.svg
--rw-r--r--   0        0        0   139795 2023-11-14 11:35:05.254645 tespy-0.7.2.post2/docs/_static/images/examples/GRC_flowsheet.svg
--rw-r--r--   0        0        0   157545 2023-11-14 11:35:05.259751 tespy-0.7.2.post2/docs/_static/images/examples/GRC_flowsheet_darkmode.svg
--rw-r--r--   0        0        0    88269 2023-11-14 11:35:05.262970 tespy-0.7.2.post2/docs/_static/images/examples/ORC_parametric_flowsheet.svg
--rw-r--r--   0        0        0    88176 2023-11-14 11:35:05.266014 tespy-0.7.2.post2/docs/_static/images/examples/ORC_parametric_flowsheet_darkmode.svg
--rw-r--r--   0        0        0   409001 2023-11-14 11:35:05.275027 tespy-0.7.2.post2/docs/_static/images/examples/PM_CAES_graphical-abstract.svg
--rw-r--r--   0        0        0   417664 2023-11-14 11:35:05.283696 tespy-0.7.2.post2/docs/_static/images/examples/PM_CAES_graphical-abstract_darkmode.svg
--rw-r--r--   0        0        0    39020 2023-11-14 11:35:05.284697 tespy-0.7.2.post2/docs/_static/images/logo_tespy_big.svg
--rw-r--r--   0        0        0    39647 2023-11-14 11:35:05.285746 tespy-0.7.2.post2/docs/_static/images/logo_tespy_big_darkmode.svg
--rw-r--r--   0        0        0    17145 2023-11-14 11:35:05.287696 tespy-0.7.2.post2/docs/_static/images/logo_tespy_big_editable_font.svg
--rw-r--r--   0        0        0    23121 2023-11-14 11:35:05.288727 tespy-0.7.2.post2/docs/_static/images/logo_tespy_mid.svg
--rw-r--r--   0        0        0    24693 2024-01-08 20:21:14.247472 tespy-0.7.2.post2/docs/_static/images/logo_tespy_mid_christmas.svg
--rw-r--r--   0        0        0    23260 2023-11-14 11:35:05.289734 tespy-0.7.2.post2/docs/_static/images/logo_tespy_mid_darkmode.svg
--rw-r--r--   0        0        0    24872 2024-01-08 20:21:14.247472 tespy-0.7.2.post2/docs/_static/images/logo_tespy_mid_darkmode_christmas.svg
--rw-r--r--   0        0        0    15239 2023-11-14 11:35:05.290696 tespy-0.7.2.post2/docs/_static/images/logo_tespy_mid_editable_font.svg
--rw-r--r--   0        0        0    13985 2023-11-27 18:42:13.344791 tespy-0.7.2.post2/docs/_static/images/logo_tespy_mini.svg
--rw-r--r--   0        0        0    13302 2023-11-14 11:35:05.293737 tespy-0.7.2.post2/docs/_static/images/logo_tespy_small.svg
--rw-r--r--   0        0        0   157002 2023-11-14 11:35:05.299887 tespy-0.7.2.post2/docs/_static/images/modules/Ts_diagram_states.svg
--rw-r--r--   0        0        0     8644 2023-11-14 11:35:05.301873 tespy-0.7.2.post2/docs/_static/images/modules/characteristics.svg
--rw-r--r--   0        0        0     8414 2023-11-14 11:35:05.302847 tespy-0.7.2.post2/docs/_static/images/modules/characteristics_darkmode.svg
--rw-r--r--   0        0        0    11300 2023-11-14 11:35:05.304847 tespy-0.7.2.post2/docs/_static/images/modules/connections.svg
--rw-r--r--   0        0        0    11315 2023-11-14 11:35:05.305848 tespy-0.7.2.post2/docs/_static/images/modules/connections_darkmode.svg
--rw-r--r--   0        0        0   134345 2023-11-14 11:35:05.308847 tespy-0.7.2.post2/docs/_static/images/modules/fluid_properties.svg
--rw-r--r--   0        0        0   125300 2023-11-14 11:35:05.310847 tespy-0.7.2.post2/docs/_static/images/modules/fluid_properties_darkmode.svg
--rw-r--r--   0        0        0   168665 2023-11-14 11:35:05.315851 tespy-0.7.2.post2/docs/_static/images/modules/logph_diagram_states.svg
--rw-r--r--   0        0        0    17587 2023-11-14 11:35:05.317845 tespy-0.7.2.post2/docs/_static/images/modules/subsystem_waste_heat_generator.svg
--rw-r--r--   0        0        0    17663 2023-11-14 11:35:05.320845 tespy-0.7.2.post2/docs/_static/images/modules/subsystem_waste_heat_generator_darkmode.svg
--rw-r--r--   0        0        0   121692 2023-11-14 11:35:05.322846 tespy-0.7.2.post2/docs/_static/images/modules/ude.svg
--rw-r--r--   0        0        0   125035 2023-11-14 11:35:05.324845 tespy-0.7.2.post2/docs/_static/images/modules/ude_darkmode.svg
--rw-r--r--   0        0        0    33944 2023-11-14 11:35:05.327439 tespy-0.7.2.post2/docs/_static/images/tutorials/district_heating_system/dhs.svg
--rw-r--r--   0        0        0    20206 2023-11-14 11:35:05.329488 tespy-0.7.2.post2/docs/_static/images/tutorials/district_heating_system/dhs_closed.svg
--rw-r--r--   0        0        0    12074 2023-11-14 11:35:05.331495 tespy-0.7.2.post2/docs/_static/images/tutorials/district_heating_system/dhs_forks.svg
--rw-r--r--   0        0        0    21711 2023-11-14 11:35:05.333492 tespy-0.7.2.post2/docs/_static/images/tutorials/district_heating_system/dhs_open.svg
--rw-r--r--   0        0        0   168149 2023-11-14 11:35:05.337492 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/NH3_logph.svg
--rw-r--r--   0        0        0    23347 2023-11-14 11:35:05.338492 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/NH3_sankey.svg
--rw-r--r--   0        0        0    60290 2023-11-14 11:35:05.339484 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D.svg
--rw-r--r--   0        0        0    61853 2023-11-14 11:35:05.340503 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D_darkmode.svg
--rw-r--r--   0        0        0    61177 2023-11-14 11:35:05.342490 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q.svg
--rw-r--r--   0        0        0    62156 2023-11-14 11:35:05.342490 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q_darkmode.svg
--rw-r--r--   0        0        0    66033 2023-11-14 11:35:05.344487 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths.svg
--rw-r--r--   0        0        0    67428 2023-11-14 11:35:05.345486 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths_darkmode.svg
--rw-r--r--   0        0        0    52499 2023-11-14 11:35:05.346490 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo.svg
--rw-r--r--   0        0        0    53372 2023-11-14 11:35:05.347488 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo_darkmode.svg
--rw-r--r--   0        0        0    29826 2023-11-14 11:35:05.348490 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/flowsheet.svg
--rw-r--r--   0        0        0    29835 2023-11-14 11:35:05.349496 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/flowsheet_darkmode.svg
--rw-r--r--   0        0        0    27850 2023-11-14 11:35:05.350453 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf.svg
--rw-r--r--   0        0        0    28404 2023-11-14 11:35:05.351485 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf_darkmode.svg
--rw-r--r--   0        0        0    30290 2023-11-14 11:35:05.352501 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet.svg
--rw-r--r--   0        0        0    30299 2023-11-14 11:35:05.353493 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet_darkmode.svg
--rw-r--r--   0        0        0   227184 2023-11-14 11:35:05.356486 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_starting_values/logph.svg
--rw-r--r--   0        0        0    46257 2023-11-14 11:35:05.357488 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet.svg
--rw-r--r--   0        0        0    46240 2023-11-14 11:35:05.358489 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_darkmode.svg
--rw-r--r--   0        0        0    46286 2023-11-14 11:35:05.359486 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1.svg
--rw-r--r--   0        0        0    46277 2023-11-14 11:35:05.360489 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1_darkmode.svg
--rw-r--r--   0        0        0    46669 2023-11-14 11:35:05.361488 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2.svg
--rw-r--r--   0        0        0    46657 2023-11-14 11:35:05.362482 tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2_darkmode.svg
--rw-r--r--   0        0        0    52832 2023-11-14 11:35:05.364488 tespy-0.7.2.post2/docs/_static/images/tutorials/osmses-2023.svg
--rw-r--r--   0        0        0    53182 2023-11-14 11:35:05.366491 tespy-0.7.2.post2/docs/_static/images/tutorials/osmses-2023_darkmode.svg
--rw-r--r--   0        0        0    33530 2023-11-14 11:35:05.368487 tespy-0.7.2.post2/docs/_static/images/tutorials/pygmo_optimization/flowsheet.svg
--rw-r--r--   0        0        0    34684 2023-11-14 11:35:05.369487 tespy-0.7.2.post2/docs/_static/images/tutorials/pygmo_optimization/flowsheet_darkmode.svg
--rw-r--r--   0        0        0   190475 2023-11-14 11:35:05.371488 tespy-0.7.2.post2/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization.svg
--rw-r--r--   0        0        0   192983 2023-11-14 11:35:05.372490 tespy-0.7.2.post2/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization_darkmode.svg
--rw-r--r--   0        0        0      578 2024-01-07 12:40:50.487754 tespy-0.7.2.post2/docs/_static/js/custom.js
--rw-r--r--   0        0        0        0 2023-11-14 11:35:05.375500 tespy-0.7.2.post2/docs/_templates/index.html
--rw-r--r--   0        0        0    20686 2023-11-27 18:42:13.344791 tespy-0.7.2.post2/docs/advanced/exergy.rst
--rw-r--r--   0        0        0       92 2023-11-14 11:35:05.377489 tespy-0.7.2.post2/docs/advanced/optimization.rst
--rw-r--r--   0        0        0      532 2023-11-27 18:42:13.352886 tespy-0.7.2.post2/docs/api.rst
--rw-r--r--   0        0        0     9313 2023-11-14 11:35:05.380489 tespy-0.7.2.post2/docs/api/_images/CombustionChamber.svg
--rw-r--r--   0        0        0     9682 2023-11-14 11:35:05.380489 tespy-0.7.2.post2/docs/api/_images/CombustionChamber_darkmode.svg
--rw-r--r--   0        0        0    15877 2023-11-14 11:35:05.382455 tespy-0.7.2.post2/docs/api/_images/CombustionEngine.svg
--rw-r--r--   0        0        0    16472 2023-11-14 11:35:05.383486 tespy-0.7.2.post2/docs/api/_images/CombustionEngine_darkmode.svg
--rw-r--r--   0        0        0     7484 2023-11-14 11:35:05.384453 tespy-0.7.2.post2/docs/api/_images/Compressor.svg
--rw-r--r--   0        0        0     7661 2023-11-14 11:35:05.384453 tespy-0.7.2.post2/docs/api/_images/Compressor_darkmode.svg
--rw-r--r--   0        0        0     9565 2023-11-14 11:35:05.385452 tespy-0.7.2.post2/docs/api/_images/Condenser.svg
--rw-r--r--   0        0        0    10115 2023-11-14 11:35:05.386452 tespy-0.7.2.post2/docs/api/_images/Condenser_darkmode.svg
--rw-r--r--   0        0        0     8889 2024-01-21 17:37:08.873999 tespy-0.7.2.post2/docs/api/_images/DropletSeparator.svg
--rw-r--r--   0        0        0     9030 2024-01-21 17:37:08.873999 tespy-0.7.2.post2/docs/api/_images/DropletSeparator_darkmode.svg
--rw-r--r--   0        0        0    10414 2023-11-14 11:35:05.389475 tespy-0.7.2.post2/docs/api/_images/Drum.svg
--rw-r--r--   0        0        0    10583 2023-11-14 11:35:05.389475 tespy-0.7.2.post2/docs/api/_images/Drum_darkmode.svg
--rw-r--r--   0        0        0    15148 2023-11-14 11:35:05.390494 tespy-0.7.2.post2/docs/api/_images/FuelCell.svg
--rw-r--r--   0        0        0    15153 2023-11-14 11:35:05.391488 tespy-0.7.2.post2/docs/api/_images/FuelCell_darkmode.svg
--rw-r--r--   0        0        0    10283 2023-11-14 11:35:05.392501 tespy-0.7.2.post2/docs/api/_images/HeatExchanger.svg
--rw-r--r--   0        0        0    10403 2023-11-14 11:35:05.393481 tespy-0.7.2.post2/docs/api/_images/HeatExchanger_darkmode.svg
--rw-r--r--   0        0        0    12851 2023-11-14 11:35:05.394490 tespy-0.7.2.post2/docs/api/_images/Merge.svg
--rw-r--r--   0        0        0    13017 2023-11-14 11:35:05.394490 tespy-0.7.2.post2/docs/api/_images/Merge_darkmode.svg
--rw-r--r--   0        0        0     8013 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/ORCEvaporator.svg
--rw-r--r--   0        0        0     7643 2023-11-14 11:35:05.396453 tespy-0.7.2.post2/docs/api/_images/ParabolicTrough.svg
--rw-r--r--   0        0        0     7823 2023-11-14 11:35:05.396453 tespy-0.7.2.post2/docs/api/_images/ParabolicTrough_darkmode.svg
--rw-r--r--   0        0        0     6462 2023-11-14 11:35:05.398490 tespy-0.7.2.post2/docs/api/_images/Pipe.svg
--rw-r--r--   0        0        0     6640 2023-11-14 11:35:05.399484 tespy-0.7.2.post2/docs/api/_images/Pipe_darkmode.svg
--rw-r--r--   0        0        0     7414 2023-11-14 11:35:05.400485 tespy-0.7.2.post2/docs/api/_images/Pump.svg
--rw-r--r--   0        0        0     7478 2023-11-14 11:35:05.400485 tespy-0.7.2.post2/docs/api/_images/Pump_darkmode.svg
--rw-r--r--   0        0        0     6810 2023-11-14 11:35:05.401451 tespy-0.7.2.post2/docs/api/_images/SolarCollector.svg
--rw-r--r--   0        0        0     6875 2023-11-14 11:35:05.402487 tespy-0.7.2.post2/docs/api/_images/SolarCollector_darkmode.svg
--rw-r--r--   0        0        0    12813 2023-11-14 11:35:05.403490 tespy-0.7.2.post2/docs/api/_images/Splitter.svg
--rw-r--r--   0        0        0    12979 2023-11-14 11:35:05.404518 tespy-0.7.2.post2/docs/api/_images/Splitter_darkmode.svg
--rw-r--r--   0        0        0    12381 2023-11-14 11:35:05.405488 tespy-0.7.2.post2/docs/api/_images/SubsystemInterface.svg
--rw-r--r--   0        0        0    12558 2023-11-14 11:35:05.405488 tespy-0.7.2.post2/docs/api/_images/SubsystemInterface_darkmode.svg
--rw-r--r--   0        0        0     6668 2023-11-14 11:35:05.406452 tespy-0.7.2.post2/docs/api/_images/Turbine.svg
--rw-r--r--   0        0        0     6677 2023-11-14 11:35:05.407500 tespy-0.7.2.post2/docs/api/_images/Turbine_darkmode.svg
--rw-r--r--   0        0        0     6491 2023-11-14 11:35:05.408451 tespy-0.7.2.post2/docs/api/_images/Valve.svg
--rw-r--r--   0        0        0     6668 2023-11-14 11:35:05.409492 tespy-0.7.2.post2/docs/api/_images/Valve_darkmode.svg
--rw-r--r--   0        0        0    13372 2023-11-14 11:35:05.410490 tespy-0.7.2.post2/docs/api/_images/WaterElectrolyzer.svg
--rw-r--r--   0        0        0    15165 2023-11-14 11:35:05.410490 tespy-0.7.2.post2/docs/api/_images/WaterElectrolyzer_darkmode.svg
--rw-r--r--   0        0        0    40711 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/combustion_engine_Q1_char_DEFAULT.svg
--rw-r--r--   0        0        0    40966 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/combustion_engine_Q2_char_DEFAULT.svg
--rw-r--r--   0        0        0    38781 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/combustion_engine_Qloss_char_DEFAULT.svg
--rw-r--r--   0        0        0    37655 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/combustion_engine_tiP_char_DEFAULT.svg
--rw-r--r--   0        0        0    49048 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/compressor_char_map_eta_s_DEFAULT.svg
--rw-r--r--   0        0        0    46950 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/compressor_char_map_pr_DEFAULT.svg
--rw-r--r--   0        0        0    39251 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/compressor_eta_s_char_DEFAULT.svg
--rw-r--r--   0        0        0    40197 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/condenser_kA_char1_DEFAULT.svg
--rw-r--r--   0        0        0    41171 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/condenser_kA_char2_DEFAULT.svg
--rw-r--r--   0        0        0    42372 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/desuperheater_kA_char1_DEFAULT.svg
--rw-r--r--   0        0        0    41171 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/desuperheater_kA_char2_DEFAULT.svg
--rw-r--r--   0        0        0    43523 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/heat_exchanger_kA_char1_CONDENSING_FLUID.svg
--rw-r--r--   0        0        0    42372 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/heat_exchanger_kA_char1_DEFAULT.svg
--rw-r--r--   0        0        0    41171 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/heat_exchanger_kA_char2_DEFAULT.svg
--rw-r--r--   0        0        0    45010 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/heat_exchanger_kA_char2_EVAPORATING_FLUID.svg
--rw-r--r--   0        0        0    42314 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/heat_exchanger_simple_kA_char_DEFAULT.svg
--rw-r--r--   0        0        0    42314 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/pipe_kA_char_DEFAULT.svg
--rw-r--r--   0        0        0    40653 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/pump_eta_s_char_DEFAULT.svg
--rw-r--r--   0        0        0    39798 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/turbine_eta_s_char_DEFAULT.svg
--rw-r--r--   0        0        0    40222 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/turbine_eta_s_char_TRAUPEL.svg
--rw-r--r--   0        0        0    36210 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/api/_images/water_electrolyzer_eta_char_DEFAULT.svg
--rw-r--r--   0        0        0     6139 2024-01-07 12:40:50.487754 tespy-0.7.2.post2/docs/api/components.rst
--rw-r--r--   0        0        0      496 2023-11-14 11:35:05.412490 tespy-0.7.2.post2/docs/api/connections.rst
--rw-r--r--   0        0        0     4204 2023-11-14 11:35:05.414490 tespy-0.7.2.post2/docs/api/data.rst
--rw-r--r--   0        0        0      493 2023-11-14 11:35:05.415452 tespy-0.7.2.post2/docs/api/networks.rst
--rw-r--r--   0        0        0     2161 2024-01-07 12:40:50.487754 tespy-0.7.2.post2/docs/api/tools.rst
--rw-r--r--   0        0        0     2463 2023-11-14 11:35:05.417470 tespy-0.7.2.post2/docs/basics.rst
--rw-r--r--   0        0        0     5528 2024-01-07 12:40:50.487754 tespy-0.7.2.post2/docs/basics/district_heating.rst
--rw-r--r--   0        0        0    10772 2024-01-07 12:40:50.501717 tespy-0.7.2.post2/docs/basics/gas_turbine.rst
--rw-r--r--   0        0        0     6691 2023-11-27 18:42:13.352886 tespy-0.7.2.post2/docs/basics/heat_pump.rst
--rw-r--r--   0        0        0     7125 2024-01-07 12:40:50.503799 tespy-0.7.2.post2/docs/basics/intro.rst
--rw-r--r--   0        0        0    10668 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/docs/basics/rankine_cycle.rst
--rw-r--r--   0        0        0     2743 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/docs/benchmarks.rst
--rw-r--r--   0        0        0     4695 2024-01-21 17:37:08.873999 tespy-0.7.2.post2/docs/conf.py
--rw-r--r--   0        0        0     7315 2023-11-27 18:42:13.352886 tespy-0.7.2.post2/docs/development/how.rst
--rw-r--r--   0        0        0     3192 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/docs/development/what.rst
--rw-r--r--   0        0        0     4319 2023-11-27 18:42:13.352886 tespy-0.7.2.post2/docs/examples.rst
--rw-r--r--   0        0        0      661 2023-11-14 11:35:05.429456 tespy-0.7.2.post2/docs/index.rst
--rw-r--r--   0        0        0     2890 2023-11-14 11:35:05.431452 tespy-0.7.2.post2/docs/installation.rst
--rw-r--r--   0        0        0     3853 2023-11-27 18:42:13.352886 tespy-0.7.2.post2/docs/introduction.rst
--rw-r--r--   0        0        0     2398 2023-11-14 11:35:05.433499 tespy-0.7.2.post2/docs/modules.rst
--rw-r--r--   0        0        0     5082 2023-11-27 18:42:13.368512 tespy-0.7.2.post2/docs/modules/characteristics.rst
--rw-r--r--   0        0        0    34468 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/docs/modules/components.rst
--rw-r--r--   0        0        0    15728 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/docs/modules/connections.rst
--rw-r--r--   0        0        0    15251 2024-01-21 17:37:08.873999 tespy-0.7.2.post2/docs/modules/fluid_properties.rst
--rw-r--r--   0        0        0    32940 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/docs/modules/networks.rst
--rw-r--r--   0        0        0    12702 2024-01-21 17:37:08.873999 tespy-0.7.2.post2/docs/modules/ude.rst
--rw-r--r--   0        0        0    12186 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/docs/references.bib
--rw-r--r--   0        0        0      886 2023-11-14 11:35:05.443458 tespy-0.7.2.post2/docs/regular_meeting.rst
--rw-r--r--   0        0        0       77 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/docs/requirements.txt
--rw-r--r--   0        0        0     2914 2023-11-14 11:35:05.445457 tespy-0.7.2.post2/docs/scripts/generate_tespy_data_module.py
--rw-r--r--   0        0        0     3594 2023-11-27 18:42:13.369520 tespy-0.7.2.post2/docs/tutorials.rst
--rw-r--r--   0        0        0     2365 2023-11-27 18:42:13.369520 tespy-0.7.2.post2/docs/tutorials/district_heating.rst
--rw-r--r--   0        0        0    32094 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/docs/tutorials/heat_pump_exergy.rst
--rw-r--r--   0        0        0    21439 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/docs/tutorials/heat_pump_steps.rst
--rw-r--r--   0        0        0     7904 2023-11-27 18:42:13.369520 tespy-0.7.2.post2/docs/tutorials/pygmo_optimization.rst
--rw-r--r--   0        0        0     8543 2023-11-27 18:42:13.369520 tespy-0.7.2.post2/docs/tutorials/starting_values.rst
--rw-r--r--   0        0        0     1325 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/docs/whats_new.rst
--rw-r--r--   0        0        0      240 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/whats_new/v0-0-1.rst
--rw-r--r--   0        0        0     1548 2023-11-14 11:35:05.456506 tespy-0.7.2.post2/docs/whats_new/v0-0-2.rst
--rw-r--r--   0        0        0     4807 2023-11-14 11:35:05.457491 tespy-0.7.2.post2/docs/whats_new/v0-0-3.rst
--rw-r--r--   0        0        0     1994 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/whats_new/v0-0-4.rst
--rw-r--r--   0        0        0     3293 2023-07-20 10:11:41.150532 tespy-0.7.2.post2/docs/whats_new/v0-0-5.rst
--rw-r--r--   0        0        0     3987 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/whats_new/v0-1-0.rst
--rw-r--r--   0        0        0     4347 2023-11-14 11:35:05.459497 tespy-0.7.2.post2/docs/whats_new/v0-1-1.rst
--rw-r--r--   0        0        0     3842 2023-11-14 11:35:05.460492 tespy-0.7.2.post2/docs/whats_new/v0-1-2.rst
--rw-r--r--   0        0        0     2675 2023-11-14 11:35:05.462483 tespy-0.7.2.post2/docs/whats_new/v0-1-3.rst
--rw-r--r--   0        0        0      616 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/whats_new/v0-1-4.rst
--rw-r--r--   0        0        0     8338 2023-11-14 11:35:05.463455 tespy-0.7.2.post2/docs/whats_new/v0-2-0.rst
--rw-r--r--   0        0        0     1982 2022-05-26 10:30:52.000000 tespy-0.7.2.post2/docs/whats_new/v0-2-1.rst
--rw-r--r--   0        0        0     3064 2023-11-14 11:35:05.465487 tespy-0.7.2.post2/docs/whats_new/v0-2-2.rst
--rw-r--r--   0        0        0    11252 2023-11-14 11:35:05.466489 tespy-0.7.2.post2/docs/whats_new/v0-3-0.rst
--rw-r--r--   0        0        0      314 2022-05-26 10:30:52.000000 tespy-0.7.2.post2/docs/whats_new/v0-3-1.rst
--rw-r--r--   0        0        0     2062 2023-07-20 10:11:41.153549 tespy-0.7.2.post2/docs/whats_new/v0-3-2.rst
--rw-r--r--   0        0        0     1345 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/whats_new/v0-3-3.rst
--rw-r--r--   0        0        0     1471 2023-11-14 11:35:05.467454 tespy-0.7.2.post2/docs/whats_new/v0-3-4.rst
--rw-r--r--   0        0        0    11174 2023-11-14 11:35:05.468458 tespy-0.7.2.post2/docs/whats_new/v0-4-0.rst
--rw-r--r--   0        0        0     1126 2023-11-14 11:35:05.469487 tespy-0.7.2.post2/docs/whats_new/v0-4-1.rst
--rw-r--r--   0        0        0     1589 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/whats_new/v0-4-2.rst
--rw-r--r--   0        0        0      563 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/docs/whats_new/v0-4-3-001.rst
--rw-r--r--   0        0        0      656 2023-11-14 11:35:05.470480 tespy-0.7.2.post2/docs/whats_new/v0-4-3-003.rst
--rw-r--r--   0        0        0     3355 2023-11-14 11:35:05.471499 tespy-0.7.2.post2/docs/whats_new/v0-4-3.rst
--rw-r--r--   0        0        0     1183 2022-01-28 07:48:36.000000 tespy-0.7.2.post2/docs/whats_new/v0-4-4.rst
--rw-r--r--   0        0        0      801 2022-01-28 07:48:36.000000 tespy-0.7.2.post2/docs/whats_new/v0-5-0.rst
--rw-r--r--   0        0        0      930 2022-05-26 10:30:52.000000 tespy-0.7.2.post2/docs/whats_new/v0-5-1.rst
--rw-r--r--   0        0        0     2644 2023-11-14 11:35:05.473451 tespy-0.7.2.post2/docs/whats_new/v0-6-0.rst
--rw-r--r--   0        0        0     2064 2023-11-14 11:35:05.474453 tespy-0.7.2.post2/docs/whats_new/v0-6-1.rst
--rw-r--r--   0        0        0      385 2023-11-14 11:35:05.475486 tespy-0.7.2.post2/docs/whats_new/v0-6-2.rst
--rw-r--r--   0        0        0     2841 2023-11-14 11:35:05.476510 tespy-0.7.2.post2/docs/whats_new/v0-6-3.rst
--rw-r--r--   0        0        0     4014 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/docs/whats_new/v0-7-0.rst
--rw-r--r--   0        0        0      427 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/docs/whats_new/v0-7-1.rst
--rw-r--r--   0        0        0      841 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/docs/whats_new/v0-7-2.rst
--rw-r--r--   0        0        0       90 2023-11-14 11:35:05.478498 tespy-0.7.2.post2/docs/zliterature.rst
--rw-r--r--   0        0        0     6582 2023-11-14 11:35:05.480483 tespy-0.7.2.post2/paper.bib
--rw-r--r--   0        0        0    11023 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/paper.md
--rw-r--r--   0        0        0     2613 2024-01-23 20:58:53.804599 tespy-0.7.2.post2/pyproject.toml
--rw-r--r--   0        0        0     1193 2024-01-23 20:58:46.075564 tespy-0.7.2.post2/src/tespy/__init__.py
--rw-r--r--   0        0        0     1655 2024-01-07 12:40:50.504403 tespy-0.7.2.post2/src/tespy/components/__init__.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/src/tespy/components/basics/__init__.py
--rw-r--r--   0        0        0     5537 2024-01-07 12:40:50.519414 tespy-0.7.2.post2/src/tespy/components/basics/cycle_closer.py
--rw-r--r--   0        0        0     2695 2024-01-07 12:40:50.520397 tespy-0.7.2.post2/src/tespy/components/basics/sink.py
--rw-r--r--   0        0        0     3223 2024-01-17 14:37:56.458491 tespy-0.7.2.post2/src/tespy/components/basics/source.py
--rw-r--r--   0        0        0     5247 2024-01-07 12:40:50.522420 tespy-0.7.2.post2/src/tespy/components/basics/subsystem_interface.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/src/tespy/components/combustion/__init__.py
--rw-r--r--   0        0        0    47281 2024-01-23 20:58:10.441293 tespy-0.7.2.post2/src/tespy/components/combustion/base.py
--rw-r--r--   0        0        0    13831 2024-01-07 12:40:50.523434 tespy-0.7.2.post2/src/tespy/components/combustion/diabatic.py
--rw-r--r--   0        0        0    55747 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/components/combustion/engine.py
--rw-r--r--   0        0        0    41128 2024-01-23 20:14:46.213633 tespy-0.7.2.post2/src/tespy/components/component.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/src/tespy/components/customs/__init__.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/src/tespy/components/heat_exchangers/__init__.py
--rw-r--r--   0        0        0    38259 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/components/heat_exchangers/base.py
--rw-r--r--   0        0        0    18098 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/components/heat_exchangers/condenser.py
--rw-r--r--   0        0        0     8531 2024-01-07 12:40:50.526398 tespy-0.7.2.post2/src/tespy/components/heat_exchangers/desuperheater.py
--rw-r--r--   0        0        0    13129 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/components/heat_exchangers/parabolic_trough.py
--rw-r--r--   0        0        0    43440 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/components/heat_exchangers/simple.py
--rw-r--r--   0        0        0    11356 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/components/heat_exchangers/solar_collector.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/src/tespy/components/nodes/__init__.py
--rw-r--r--   0        0        0     6116 2024-01-07 12:40:50.528394 tespy-0.7.2.post2/src/tespy/components/nodes/base.py
--rw-r--r--   0        0        0    13308 2024-01-07 12:40:50.529399 tespy-0.7.2.post2/src/tespy/components/nodes/droplet_separator.py
--rw-r--r--   0        0        0    14951 2024-01-07 12:40:50.530460 tespy-0.7.2.post2/src/tespy/components/nodes/drum.py
--rw-r--r--   0        0        0    17177 2024-01-07 12:40:50.530460 tespy-0.7.2.post2/src/tespy/components/nodes/merge.py
--rw-r--r--   0        0        0    11927 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/components/nodes/separator.py
--rw-r--r--   0        0        0     6693 2024-01-07 12:40:50.532411 tespy-0.7.2.post2/src/tespy/components/nodes/splitter.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/src/tespy/components/piping/__init__.py
--rw-r--r--   0        0        0     5352 2024-01-07 12:40:50.533396 tespy-0.7.2.post2/src/tespy/components/piping/pipe.py
--rw-r--r--   0        0        0    13658 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/components/piping/valve.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/src/tespy/components/reactors/__init__.py
--rw-r--r--   0        0        0    27777 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/components/reactors/fuel_cell.py
--rw-r--r--   0        0        0    40264 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/components/reactors/water_electrolyzer.py
--rw-r--r--   0        0        0     2343 2024-01-07 12:40:50.535395 tespy-0.7.2.post2/src/tespy/components/subsystem.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/src/tespy/components/turbomachinery/__init__.py
--rw-r--r--   0        0        0     8475 2024-01-07 12:40:50.536394 tespy-0.7.2.post2/src/tespy/components/turbomachinery/base.py
--rw-r--r--   0        0        0    25801 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/components/turbomachinery/compressor.py
--rw-r--r--   0        0        0    19150 2024-01-07 12:40:50.537412 tespy-0.7.2.post2/src/tespy/components/turbomachinery/pump.py
--rw-r--r--   0        0        0    19110 2024-01-17 14:37:56.462489 tespy-0.7.2.post2/src/tespy/components/turbomachinery/turbine.py
--rw-r--r--   0        0        0      147 2022-01-28 07:48:36.000000 tespy-0.7.2.post2/src/tespy/connections/__init__.py
--rw-r--r--   0        0        0    16915 2024-01-07 12:40:50.539466 tespy-0.7.2.post2/src/tespy/connections/bus.py
--rw-r--r--   0        0        0    44573 2024-01-23 20:58:10.441293 tespy-0.7.2.post2/src/tespy/connections/connection.py
--rw-r--r--   0        0        0     9270 2023-11-14 11:35:05.528493 tespy-0.7.2.post2/src/tespy/data/ChemEx/Ahrendts.json
--rw-r--r--   0        0        0     8407 2023-11-14 11:35:05.530494 tespy-0.7.2.post2/src/tespy/data/ChemEx/Szargut1988.json
--rw-r--r--   0        0        0     8578 2023-11-14 11:35:05.532488 tespy-0.7.2.post2/src/tespy/data/ChemEx/Szargut2007.json
--rw-r--r--   0        0        0     8047 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/src/tespy/data/char_lines.json
--rw-r--r--   0        0        0     3726 2021-10-04 06:28:48.000000 tespy-0.7.2.post2/src/tespy/data/char_maps.json
--rw-r--r--   0        0        0      118 2022-01-28 07:48:36.000000 tespy-0.7.2.post2/src/tespy/networks/__init__.py
--rw-r--r--   0        0        0   107376 2024-01-23 20:46:37.673766 tespy-0.7.2.post2/src/tespy/networks/network.py
--rw-r--r--   0        0        0    15070 2024-01-07 12:40:50.541391 tespy-0.7.2.post2/src/tespy/networks/network_reader.py
--rw-r--r--   0        0        0      884 2023-11-14 11:35:05.537509 tespy-0.7.2.post2/src/tespy/tools/__init__.py
--rw-r--r--   0        0        0    38453 2024-01-17 14:37:56.463488 tespy-0.7.2.post2/src/tespy/tools/analyses.py
--rw-r--r--   0        0        0    17456 2024-01-07 12:40:50.543394 tespy-0.7.2.post2/src/tespy/tools/characteristics.py
--rw-r--r--   0        0        0    17336 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/tools/data_containers.py
--rw-r--r--   0        0        0    38786 2024-01-07 12:40:50.544396 tespy-0.7.2.post2/src/tespy/tools/document_models.py
--rw-r--r--   0        0        0     1046 2024-01-07 12:40:50.544396 tespy-0.7.2.post2/src/tespy/tools/fluid_properties/__init__.py
--rw-r--r--   0        0        0     9666 2024-01-10 06:48:11.693962 tespy-0.7.2.post2/src/tespy/tools/fluid_properties/functions.py
--rw-r--r--   0        0        0     9700 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/tools/fluid_properties/helpers.py
--rw-r--r--   0        0        0    12386 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/tools/fluid_properties/mixtures.py
--rw-r--r--   0        0        0    13368 2024-01-21 17:37:08.882147 tespy-0.7.2.post2/src/tespy/tools/fluid_properties/wrappers.py
--rw-r--r--   0        0        0     3454 2024-01-21 17:37:08.897791 tespy-0.7.2.post2/src/tespy/tools/global_vars.py
--rw-r--r--   0        0        0    22936 2024-01-21 17:37:08.898325 tespy-0.7.2.post2/src/tespy/tools/helpers.py
--rw-r--r--   0        0        0    15049 2024-01-07 12:40:50.548394 tespy-0.7.2.post2/src/tespy/tools/logger.py
--rw-r--r--   0        0        0    10421 2024-01-21 17:37:08.898325 tespy-0.7.2.post2/src/tespy/tools/optimization.py
--rw-r--r--   0        0        0      427 2024-01-07 12:40:50.549396 tespy-0.7.2.post2/tests/test_advanced_tutorials.py
--rw-r--r--   0        0        0     4337 2024-01-07 12:40:50.549396 tespy-0.7.2.post2/tests/test_analyses/test_entropy_analysis.py
--rw-r--r--   0        0        0    24440 2024-01-07 12:40:50.550392 tespy-0.7.2.post2/tests/test_analyses/test_exergy_analysis.py
--rw-r--r--   0        0        0      315 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_basic_tutorials.py
--rw-r--r--   0        0        0    10214 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_busses.py
--rw-r--r--   0        0        0    11728 2024-01-21 17:37:08.898325 tespy-0.7.2.post2/tests/test_components/test_combustion.py
--rw-r--r--   0        0        0      346 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_components/test_customs.py
--rw-r--r--   0        0        0     1627 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_components/test_drum.py
--rw-r--r--   0        0        0    23305 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_components/test_heat_exchangers.py
--rw-r--r--   0        0        0     4028 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_components/test_merge.py
--rw-r--r--   0        0        0     3150 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_components/test_piping.py
--rw-r--r--   0        0        0     7107 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_components/test_reactors.py
--rw-r--r--   0        0        0    17021 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_components/test_turbomachinery.py
--rw-r--r--   0        0        0     4025 2024-01-21 17:37:08.900857 tespy-0.7.2.post2/tests/test_connections.py
--rw-r--r--   0        0        0    20109 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_errors.py
--rw-r--r--   0        0        0      455 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_heat_pump_exergy.py
--rw-r--r--   0        0        0      996 2023-11-14 11:35:05.574460 tespy-0.7.2.post2/tests/test_models/cgam-ebsilon-results.csv
--rw-r--r--   0        0        0     7604 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_models/test_CGAM_model.py
--rw-r--r--   0        0        0    12500 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_models/test_heat_pump_model.py
--rw-r--r--   0        0        0    18609 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_models/test_solar_energy_generating_system.py
--rw-r--r--   0        0        0     1664 2024-01-21 17:37:08.900857 tespy-0.7.2.post2/tests/test_networks/test_binary_incompressible.py
--rw-r--r--   0        0        0     5571 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_networks/test_mixing_rules.py
--rw-r--r--   0        0        0    24711 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_networks/test_network.py
--rw-r--r--   0        0        0     7913 2023-11-27 18:42:13.447683 tespy-0.7.2.post2/tests/test_tools/test_characteristics.py
--rw-r--r--   0        0        0    12983 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_tools/test_fluid_properties/test_coolprop.py
--rw-r--r--   0        0        0     2106 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_tools/test_fluid_properties/test_iapws.py
--rw-r--r--   0        0        0     1385 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tests/test_tools/test_fluid_properties/test_pyromat.py
--rw-r--r--   0        0        0     2004 2021-12-29 09:05:28.000000 tespy-0.7.2.post2/tests/test_tools/test_helpers.py
--rw-r--r--   0        0        0     2000 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tox.ini
--rw-r--r--   0        0        0      261 2024-01-07 12:40:50.551498 tespy-0.7.2.post2/tutorial/README.rst
--rw-r--r--   0        0        0     9727 2024-01-07 12:40:50.567166 tespy-0.7.2.post2/tutorial/advanced/optimization_example.py
--rw-r--r--   0        0        0     9541 2024-01-07 12:40:50.567166 tespy-0.7.2.post2/tutorial/advanced/starting_values.py
--rw-r--r--   0        0        0     6090 2024-01-07 12:40:50.567166 tespy-0.7.2.post2/tutorial/advanced/stepwise.py
--rw-r--r--   0        0        0     4264 2024-01-07 12:40:50.567166 tespy-0.7.2.post2/tutorial/basics/district_heating.py
--rw-r--r--   0        0        0     4978 2024-01-07 12:40:50.567166 tespy-0.7.2.post2/tutorial/basics/gas_turbine.py
--rw-r--r--   0        0        0     3216 2024-01-07 12:40:50.567166 tespy-0.7.2.post2/tutorial/basics/heat_pump.py
--rw-r--r--   0        0        0     4661 2024-01-07 12:40:50.571705 tespy-0.7.2.post2/tutorial/basics/rankine.py
--rw-r--r--   0        0        0     4201 2024-01-07 12:40:50.571705 tespy-0.7.2.post2/tutorial/heat_pump_exergy/NH3.py
--rw-r--r--   0        0        0    10920 2024-01-21 17:37:08.900857 tespy-0.7.2.post2/tutorial/heat_pump_exergy/NH3_calculations.py
--rw-r--r--   0        0        0     4217 2024-01-07 12:40:50.571705 tespy-0.7.2.post2/tutorial/heat_pump_exergy/R410A.py
--rw-r--r--   0        0        0    10943 2024-01-21 17:37:08.900857 tespy-0.7.2.post2/tutorial/heat_pump_exergy/R410A_calculations.py
--rw-r--r--   0        0        0     8277 2024-01-07 12:40:50.571705 tespy-0.7.2.post2/tutorial/heat_pump_exergy/plots.py
--rw-r--r--   0        0        0    10593 1970-01-01 00:00:00.000000 tespy-0.7.2.post2/PKG-INFO
+-rw-r--r--   0        0        0      265 2021-10-04 06:28:48.000000 tespy-0.7.3/.editorconfig
+-rw-r--r--   0        0        0     1446 2021-10-04 06:28:48.000000 tespy-0.7.3/.pep8speaks.yml
+-rw-r--r--   0        0        0      341 2023-11-14 11:35:05.186734 tespy-0.7.3/.readthedocs.yml
+-rw-r--r--   0        0        0     3269 2021-10-04 06:28:48.000000 tespy-0.7.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      154 2022-01-28 07:48:36.000000 tespy-0.7.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1088 2024-04-15 11:16:02.638416 tespy-0.7.3/LICENSE
+-rw-r--r--   0        0        0      281 2023-11-14 11:35:05.190735 tespy-0.7.3/MANIFEST.in
+-rw-r--r--   0        0        0      765 2021-10-04 06:28:48.000000 tespy-0.7.3/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     9116 2024-04-15 11:16:02.639417 tespy-0.7.3/README.rst
+-rw-r--r--   0        0        0      180 2023-11-14 11:35:05.203247 tespy-0.7.3/docs/_static/css/custom.css
+-rw-r--r--   0        0        0   129643 2023-11-14 11:35:05.207242 tespy-0.7.3/docs/_static/images/advanced/exergy/flowsheet.svg
+-rw-r--r--   0        0        0   136810 2023-11-14 11:35:05.210242 tespy-0.7.3/docs/_static/images/advanced/exergy/flowsheet_darkmode.svg
+-rw-r--r--   0        0        0    32134 2023-11-14 11:35:05.212242 tespy-0.7.3/docs/_static/images/advanced/exergy/sankey.svg
+-rw-r--r--   0        0        0    17276 2023-11-14 11:35:05.213286 tespy-0.7.3/docs/_static/images/basics/district_heating.svg
+-rw-r--r--   0        0        0    18111 2023-11-14 11:35:05.215279 tespy-0.7.3/docs/_static/images/basics/district_heating_darkmode.svg
+-rw-r--r--   0        0        0    69064 2023-11-14 11:35:05.218243 tespy-0.7.3/docs/_static/images/basics/district_heating_partload.svg
+-rw-r--r--   0        0        0    71199 2023-11-14 11:35:05.220243 tespy-0.7.3/docs/_static/images/basics/district_heating_partload_darkmode.svg
+-rw-r--r--   0        0        0    15810 2023-11-14 11:35:05.222242 tespy-0.7.3/docs/_static/images/basics/gas_turbine.svg
+-rw-r--r--   0        0        0    16340 2023-11-14 11:35:05.223244 tespy-0.7.3/docs/_static/images/basics/gas_turbine_darkmode.svg
+-rw-r--r--   0        0        0    32095 2023-11-14 11:35:05.225250 tespy-0.7.3/docs/_static/images/basics/gas_turbine_fuel_composition.svg
+-rw-r--r--   0        0        0    32756 2023-11-14 11:35:05.227255 tespy-0.7.3/docs/_static/images/basics/gas_turbine_fuel_composition_darkmode.svg
+-rw-r--r--   0        0        0    29612 2023-11-14 11:35:05.228284 tespy-0.7.3/docs/_static/images/basics/gas_turbine_oxygen.svg
+-rw-r--r--   0        0        0    30202 2023-11-14 11:35:05.230296 tespy-0.7.3/docs/_static/images/basics/gas_turbine_oxygen_darkmode.svg
+-rw-r--r--   0        0        0    57559 2023-11-14 11:35:05.231295 tespy-0.7.3/docs/_static/images/basics/gas_turbine_parametric.svg
+-rw-r--r--   0        0        0    59255 2023-11-14 11:35:05.233242 tespy-0.7.3/docs/_static/images/basics/gas_turbine_parametric_darkmode.svg
+-rw-r--r--   0        0        0    14362 2023-11-14 11:35:05.234243 tespy-0.7.3/docs/_static/images/basics/heat_pump.svg
+-rw-r--r--   0        0        0    14866 2023-11-14 11:35:05.236243 tespy-0.7.3/docs/_static/images/basics/heat_pump_darkmode.svg
+-rw-r--r--   0        0        0    53423 2023-11-14 11:35:05.237245 tespy-0.7.3/docs/_static/images/basics/heat_pump_parametric.svg
+-rw-r--r--   0        0        0    54994 2023-11-14 11:35:05.240244 tespy-0.7.3/docs/_static/images/basics/heat_pump_parametric_darkmode.svg
+-rw-r--r--   0        0        0    16030 2023-11-14 11:35:05.241287 tespy-0.7.3/docs/_static/images/basics/modeling_concept.svg
+-rw-r--r--   0        0        0    16137 2023-11-14 11:35:05.242303 tespy-0.7.3/docs/_static/images/basics/rankine_cycle.svg
+-rw-r--r--   0        0        0    16871 2023-11-14 11:35:05.243245 tespy-0.7.3/docs/_static/images/basics/rankine_cycle_darkmode.svg
+-rw-r--r--   0        0        0    59916 2023-11-14 11:35:05.245276 tespy-0.7.3/docs/_static/images/basics/rankine_parametric.svg
+-rw-r--r--   0        0        0    61115 2023-11-14 11:35:05.247242 tespy-0.7.3/docs/_static/images/basics/rankine_parametric_darkmode.svg
+-rw-r--r--   0        0        0    26962 2023-11-14 11:35:05.248242 tespy-0.7.3/docs/_static/images/basics/rankine_partload.svg
+-rw-r--r--   0        0        0    27517 2023-11-14 11:35:05.250241 tespy-0.7.3/docs/_static/images/basics/rankine_partload_darkmode.svg
+-rw-r--r--   0        0        0   139795 2023-11-14 11:35:05.254645 tespy-0.7.3/docs/_static/images/examples/GRC_flowsheet.svg
+-rw-r--r--   0        0        0   157545 2023-11-14 11:35:05.259751 tespy-0.7.3/docs/_static/images/examples/GRC_flowsheet_darkmode.svg
+-rw-r--r--   0        0        0    88269 2023-11-14 11:35:05.262970 tespy-0.7.3/docs/_static/images/examples/ORC_parametric_flowsheet.svg
+-rw-r--r--   0        0        0    88176 2023-11-14 11:35:05.266014 tespy-0.7.3/docs/_static/images/examples/ORC_parametric_flowsheet_darkmode.svg
+-rw-r--r--   0        0        0   409001 2023-11-14 11:35:05.275027 tespy-0.7.3/docs/_static/images/examples/PM_CAES_graphical-abstract.svg
+-rw-r--r--   0        0        0   417664 2023-11-14 11:35:05.283696 tespy-0.7.3/docs/_static/images/examples/PM_CAES_graphical-abstract_darkmode.svg
+-rw-r--r--   0        0        0    39020 2023-11-14 11:35:05.284697 tespy-0.7.3/docs/_static/images/logo_tespy_big.svg
+-rw-r--r--   0        0        0    39647 2023-11-14 11:35:05.285746 tespy-0.7.3/docs/_static/images/logo_tespy_big_darkmode.svg
+-rw-r--r--   0        0        0    17145 2023-11-14 11:35:05.287696 tespy-0.7.3/docs/_static/images/logo_tespy_big_editable_font.svg
+-rw-r--r--   0        0        0    23121 2024-04-15 08:10:01.844502 tespy-0.7.3/docs/_static/images/logo_tespy_mid.svg
+-rw-r--r--   0        0        0    24693 2024-04-15 11:16:02.639417 tespy-0.7.3/docs/_static/images/logo_tespy_mid_christmas.svg
+-rw-r--r--   0        0        0    23260 2023-11-14 11:35:05.289734 tespy-0.7.3/docs/_static/images/logo_tespy_mid_darkmode.svg
+-rw-r--r--   0        0        0    24872 2024-04-15 11:16:02.640417 tespy-0.7.3/docs/_static/images/logo_tespy_mid_darkmode_christmas.svg
+-rw-r--r--   0        0        0    15239 2023-11-14 11:35:05.290696 tespy-0.7.3/docs/_static/images/logo_tespy_mid_editable_font.svg
+-rw-r--r--   0        0        0    13985 2023-11-27 18:42:13.344791 tespy-0.7.3/docs/_static/images/logo_tespy_mini.svg
+-rw-r--r--   0        0        0    13302 2023-11-14 11:35:05.293737 tespy-0.7.3/docs/_static/images/logo_tespy_small.svg
+-rw-r--r--   0        0        0   157002 2023-11-14 11:35:05.299887 tespy-0.7.3/docs/_static/images/modules/Ts_diagram_states.svg
+-rw-r--r--   0        0        0     8644 2023-11-14 11:35:05.301873 tespy-0.7.3/docs/_static/images/modules/characteristics.svg
+-rw-r--r--   0        0        0     8414 2023-11-14 11:35:05.302847 tespy-0.7.3/docs/_static/images/modules/characteristics_darkmode.svg
+-rw-r--r--   0        0        0    11300 2023-11-14 11:35:05.304847 tespy-0.7.3/docs/_static/images/modules/connections.svg
+-rw-r--r--   0        0        0    11315 2023-11-14 11:35:05.305848 tespy-0.7.3/docs/_static/images/modules/connections_darkmode.svg
+-rw-r--r--   0        0        0   134345 2023-11-14 11:35:05.308847 tespy-0.7.3/docs/_static/images/modules/fluid_properties.svg
+-rw-r--r--   0        0        0   125300 2023-11-14 11:35:05.310847 tespy-0.7.3/docs/_static/images/modules/fluid_properties_darkmode.svg
+-rw-r--r--   0        0        0   168665 2023-11-14 11:35:05.315851 tespy-0.7.3/docs/_static/images/modules/logph_diagram_states.svg
+-rw-r--r--   0        0        0    17587 2023-11-14 11:35:05.317845 tespy-0.7.3/docs/_static/images/modules/subsystem_waste_heat_generator.svg
+-rw-r--r--   0        0        0    17663 2023-11-14 11:35:05.320845 tespy-0.7.3/docs/_static/images/modules/subsystem_waste_heat_generator_darkmode.svg
+-rw-r--r--   0        0        0   121692 2023-11-14 11:35:05.322846 tespy-0.7.3/docs/_static/images/modules/ude.svg
+-rw-r--r--   0        0        0   125035 2023-11-14 11:35:05.324845 tespy-0.7.3/docs/_static/images/modules/ude_darkmode.svg
+-rw-r--r--   0        0        0    33944 2023-11-14 11:35:05.327439 tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs.svg
+-rw-r--r--   0        0        0    20206 2023-11-14 11:35:05.329488 tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs_closed.svg
+-rw-r--r--   0        0        0    12074 2023-11-14 11:35:05.331495 tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs_forks.svg
+-rw-r--r--   0        0        0    21711 2023-11-14 11:35:05.333492 tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs_open.svg
+-rw-r--r--   0        0        0   168149 2023-11-14 11:35:05.337492 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/NH3_logph.svg
+-rw-r--r--   0        0        0    23347 2023-11-14 11:35:05.338492 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/NH3_sankey.svg
+-rw-r--r--   0        0        0    60290 2023-11-14 11:35:05.339484 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D.svg
+-rw-r--r--   0        0        0    61853 2023-11-14 11:35:05.340503 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D_darkmode.svg
+-rw-r--r--   0        0        0    61177 2023-11-14 11:35:05.342490 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q.svg
+-rw-r--r--   0        0        0    62156 2023-11-14 11:35:05.342490 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q_darkmode.svg
+-rw-r--r--   0        0        0    66033 2023-11-14 11:35:05.344487 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths.svg
+-rw-r--r--   0        0        0    67428 2023-11-14 11:35:05.345486 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths_darkmode.svg
+-rw-r--r--   0        0        0    52499 2023-11-14 11:35:05.346490 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo.svg
+-rw-r--r--   0        0        0    53372 2023-11-14 11:35:05.347488 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo_darkmode.svg
+-rw-r--r--   0        0        0    29826 2023-11-14 11:35:05.348490 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/flowsheet.svg
+-rw-r--r--   0        0        0    29835 2023-11-14 11:35:05.349496 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/flowsheet_darkmode.svg
+-rw-r--r--   0        0        0    27850 2023-11-14 11:35:05.350453 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf.svg
+-rw-r--r--   0        0        0    28404 2023-11-14 11:35:05.351485 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf_darkmode.svg
+-rw-r--r--   0        0        0    30290 2023-11-14 11:35:05.352501 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet.svg
+-rw-r--r--   0        0        0    30299 2023-11-14 11:35:05.353493 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet_darkmode.svg
+-rw-r--r--   0        0        0   227184 2023-11-14 11:35:05.356486 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/logph.svg
+-rw-r--r--   0        0        0    46257 2023-11-14 11:35:05.357488 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet.svg
+-rw-r--r--   0        0        0    46240 2023-11-14 11:35:05.358489 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_darkmode.svg
+-rw-r--r--   0        0        0    46286 2023-11-14 11:35:05.359486 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1.svg
+-rw-r--r--   0        0        0    46277 2023-11-14 11:35:05.360489 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1_darkmode.svg
+-rw-r--r--   0        0        0    46669 2023-11-14 11:35:05.361488 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2.svg
+-rw-r--r--   0        0        0    46657 2023-11-14 11:35:05.362482 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2_darkmode.svg
+-rw-r--r--   0        0        0    52832 2023-11-14 11:35:05.364488 tespy-0.7.3/docs/_static/images/tutorials/osmses-2023.svg
+-rw-r--r--   0        0        0    53182 2023-11-14 11:35:05.366491 tespy-0.7.3/docs/_static/images/tutorials/osmses-2023_darkmode.svg
+-rw-r--r--   0        0        0    33530 2023-11-14 11:35:05.368487 tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/flowsheet.svg
+-rw-r--r--   0        0        0    34684 2023-11-14 11:35:05.369487 tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/flowsheet_darkmode.svg
+-rw-r--r--   0        0        0   190475 2023-11-14 11:35:05.371488 tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization.svg
+-rw-r--r--   0        0        0   192983 2023-11-14 11:35:05.372490 tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization_darkmode.svg
+-rw-r--r--   0        0        0      578 2024-02-08 10:33:11.103316 tespy-0.7.3/docs/_static/js/custom.js
+-rw-r--r--   0        0        0        0 2023-11-14 11:35:05.375500 tespy-0.7.3/docs/_templates/index.html
+-rw-r--r--   0        0        0    20686 2023-11-27 18:42:13.344791 tespy-0.7.3/docs/advanced/exergy.rst
+-rw-r--r--   0        0        0       92 2023-11-14 11:35:05.377489 tespy-0.7.3/docs/advanced/optimization.rst
+-rw-r--r--   0        0        0      532 2023-11-27 18:42:13.352886 tespy-0.7.3/docs/api.rst
+-rw-r--r--   0        0        0     9313 2023-11-14 11:35:05.380489 tespy-0.7.3/docs/api/_images/CombustionChamber.svg
+-rw-r--r--   0        0        0     9682 2023-11-14 11:35:05.380489 tespy-0.7.3/docs/api/_images/CombustionChamber_darkmode.svg
+-rw-r--r--   0        0        0    15877 2023-11-14 11:35:05.382455 tespy-0.7.3/docs/api/_images/CombustionEngine.svg
+-rw-r--r--   0        0        0    16472 2023-11-14 11:35:05.383486 tespy-0.7.3/docs/api/_images/CombustionEngine_darkmode.svg
+-rw-r--r--   0        0        0     7484 2023-11-14 11:35:05.384453 tespy-0.7.3/docs/api/_images/Compressor.svg
+-rw-r--r--   0        0        0     7661 2023-11-14 11:35:05.384453 tespy-0.7.3/docs/api/_images/Compressor_darkmode.svg
+-rw-r--r--   0        0        0     9565 2023-11-14 11:35:05.385452 tespy-0.7.3/docs/api/_images/Condenser.svg
+-rw-r--r--   0        0        0    10115 2023-11-14 11:35:05.386452 tespy-0.7.3/docs/api/_images/Condenser_darkmode.svg
+-rw-r--r--   0        0        0     8889 2024-04-15 11:16:02.640417 tespy-0.7.3/docs/api/_images/DropletSeparator.svg
+-rw-r--r--   0        0        0     9030 2024-04-15 11:16:02.641417 tespy-0.7.3/docs/api/_images/DropletSeparator_darkmode.svg
+-rw-r--r--   0        0        0    10414 2023-11-14 11:35:05.389475 tespy-0.7.3/docs/api/_images/Drum.svg
+-rw-r--r--   0        0        0    10583 2023-11-14 11:35:05.389475 tespy-0.7.3/docs/api/_images/Drum_darkmode.svg
+-rw-r--r--   0        0        0    15148 2023-11-14 11:35:05.390494 tespy-0.7.3/docs/api/_images/FuelCell.svg
+-rw-r--r--   0        0        0    15153 2023-11-14 11:35:05.391488 tespy-0.7.3/docs/api/_images/FuelCell_darkmode.svg
+-rw-r--r--   0        0        0    10283 2023-11-14 11:35:05.392501 tespy-0.7.3/docs/api/_images/HeatExchanger.svg
+-rw-r--r--   0        0        0    10403 2023-11-14 11:35:05.393481 tespy-0.7.3/docs/api/_images/HeatExchanger_darkmode.svg
+-rw-r--r--   0        0        0    12851 2023-11-14 11:35:05.394490 tespy-0.7.3/docs/api/_images/Merge.svg
+-rw-r--r--   0        0        0    13017 2023-11-14 11:35:05.394490 tespy-0.7.3/docs/api/_images/Merge_darkmode.svg
+-rw-r--r--   0        0        0     8013 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/ORCEvaporator.svg
+-rw-r--r--   0        0        0     7643 2023-11-14 11:35:05.396453 tespy-0.7.3/docs/api/_images/ParabolicTrough.svg
+-rw-r--r--   0        0        0     7823 2023-11-14 11:35:05.396453 tespy-0.7.3/docs/api/_images/ParabolicTrough_darkmode.svg
+-rw-r--r--   0        0        0     6462 2023-11-14 11:35:05.398490 tespy-0.7.3/docs/api/_images/Pipe.svg
+-rw-r--r--   0        0        0     6640 2023-11-14 11:35:05.399484 tespy-0.7.3/docs/api/_images/Pipe_darkmode.svg
+-rw-r--r--   0        0        0     7414 2023-11-14 11:35:05.400485 tespy-0.7.3/docs/api/_images/Pump.svg
+-rw-r--r--   0        0        0     7478 2023-11-14 11:35:05.400485 tespy-0.7.3/docs/api/_images/Pump_darkmode.svg
+-rw-r--r--   0        0        0     6810 2023-11-14 11:35:05.401451 tespy-0.7.3/docs/api/_images/SolarCollector.svg
+-rw-r--r--   0        0        0     6875 2023-11-14 11:35:05.402487 tespy-0.7.3/docs/api/_images/SolarCollector_darkmode.svg
+-rw-r--r--   0        0        0    12813 2023-11-14 11:35:05.403490 tespy-0.7.3/docs/api/_images/Splitter.svg
+-rw-r--r--   0        0        0    12979 2023-11-14 11:35:05.404518 tespy-0.7.3/docs/api/_images/Splitter_darkmode.svg
+-rw-r--r--   0        0        0    12381 2023-11-14 11:35:05.405488 tespy-0.7.3/docs/api/_images/SubsystemInterface.svg
+-rw-r--r--   0        0        0    12558 2023-11-14 11:35:05.405488 tespy-0.7.3/docs/api/_images/SubsystemInterface_darkmode.svg
+-rw-r--r--   0        0        0     6668 2023-11-14 11:35:05.406452 tespy-0.7.3/docs/api/_images/Turbine.svg
+-rw-r--r--   0        0        0     6677 2023-11-14 11:35:05.407500 tespy-0.7.3/docs/api/_images/Turbine_darkmode.svg
+-rw-r--r--   0        0        0     6491 2023-11-14 11:35:05.408451 tespy-0.7.3/docs/api/_images/Valve.svg
+-rw-r--r--   0        0        0     6668 2023-11-14 11:35:05.409492 tespy-0.7.3/docs/api/_images/Valve_darkmode.svg
+-rw-r--r--   0        0        0    13372 2023-11-14 11:35:05.410490 tespy-0.7.3/docs/api/_images/WaterElectrolyzer.svg
+-rw-r--r--   0        0        0    15165 2023-11-14 11:35:05.410490 tespy-0.7.3/docs/api/_images/WaterElectrolyzer_darkmode.svg
+-rw-r--r--   0        0        0    40711 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/combustion_engine_Q1_char_DEFAULT.svg
+-rw-r--r--   0        0        0    40966 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/combustion_engine_Q2_char_DEFAULT.svg
+-rw-r--r--   0        0        0    38781 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/combustion_engine_Qloss_char_DEFAULT.svg
+-rw-r--r--   0        0        0    37655 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/combustion_engine_tiP_char_DEFAULT.svg
+-rw-r--r--   0        0        0    49048 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/compressor_char_map_eta_s_DEFAULT.svg
+-rw-r--r--   0        0        0    46950 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/compressor_char_map_pr_DEFAULT.svg
+-rw-r--r--   0        0        0    39251 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/compressor_eta_s_char_DEFAULT.svg
+-rw-r--r--   0        0        0    40197 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/condenser_kA_char1_DEFAULT.svg
+-rw-r--r--   0        0        0    41171 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/condenser_kA_char2_DEFAULT.svg
+-rw-r--r--   0        0        0    42372 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/desuperheater_kA_char1_DEFAULT.svg
+-rw-r--r--   0        0        0    41171 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/desuperheater_kA_char2_DEFAULT.svg
+-rw-r--r--   0        0        0    43523 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char1_CONDENSING_FLUID.svg
+-rw-r--r--   0        0        0    42372 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char1_DEFAULT.svg
+-rw-r--r--   0        0        0    41171 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char2_DEFAULT.svg
+-rw-r--r--   0        0        0    45010 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char2_EVAPORATING_FLUID.svg
+-rw-r--r--   0        0        0    42314 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/heat_exchanger_simple_kA_char_DEFAULT.svg
+-rw-r--r--   0        0        0    42314 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/pipe_kA_char_DEFAULT.svg
+-rw-r--r--   0        0        0    40653 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/pump_eta_s_char_DEFAULT.svg
+-rw-r--r--   0        0        0    39798 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/turbine_eta_s_char_DEFAULT.svg
+-rw-r--r--   0        0        0    40222 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/turbine_eta_s_char_TRAUPEL.svg
+-rw-r--r--   0        0        0    36210 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/water_electrolyzer_eta_char_DEFAULT.svg
+-rw-r--r--   0        0        0     6139 2024-04-15 11:16:02.648090 tespy-0.7.3/docs/api/components.rst
+-rw-r--r--   0        0        0      496 2023-11-14 11:35:05.412490 tespy-0.7.3/docs/api/connections.rst
+-rw-r--r--   0        0        0     4204 2023-11-14 11:35:05.414490 tespy-0.7.3/docs/api/data.rst
+-rw-r--r--   0        0        0      493 2023-11-14 11:35:05.415452 tespy-0.7.3/docs/api/networks.rst
+-rw-r--r--   0        0        0     2161 2024-04-15 11:16:02.649119 tespy-0.7.3/docs/api/tools.rst
+-rw-r--r--   0        0        0     2463 2023-11-14 11:35:05.417470 tespy-0.7.3/docs/basics.rst
+-rw-r--r--   0        0        0     5528 2024-04-15 11:16:02.649119 tespy-0.7.3/docs/basics/district_heating.rst
+-rw-r--r--   0        0        0    10772 2024-04-15 11:16:02.650113 tespy-0.7.3/docs/basics/gas_turbine.rst
+-rw-r--r--   0        0        0     6691 2023-11-27 18:42:13.352886 tespy-0.7.3/docs/basics/heat_pump.rst
+-rw-r--r--   0        0        0     7125 2024-04-15 11:16:02.650113 tespy-0.7.3/docs/basics/intro.rst
+-rw-r--r--   0        0        0    10668 2024-04-15 11:16:02.652129 tespy-0.7.3/docs/basics/rankine_cycle.rst
+-rw-r--r--   0        0        0     2743 2024-04-15 11:16:02.653137 tespy-0.7.3/docs/benchmarks.rst
+-rw-r--r--   0        0        0     4695 2024-04-15 11:16:02.653137 tespy-0.7.3/docs/conf.py
+-rw-r--r--   0        0        0     7315 2023-11-27 18:42:13.352886 tespy-0.7.3/docs/development/how.rst
+-rw-r--r--   0        0        0     3192 2024-04-15 11:16:02.654136 tespy-0.7.3/docs/development/what.rst
+-rw-r--r--   0        0        0     4319 2023-11-27 18:42:13.352886 tespy-0.7.3/docs/examples.rst
+-rw-r--r--   0        0        0      661 2023-11-14 11:35:05.429456 tespy-0.7.3/docs/index.rst
+-rw-r--r--   0        0        0     2890 2023-11-14 11:35:05.431452 tespy-0.7.3/docs/installation.rst
+-rw-r--r--   0        0        0     3853 2023-11-27 18:42:13.352886 tespy-0.7.3/docs/introduction.rst
+-rw-r--r--   0        0        0     2398 2023-11-14 11:35:05.433499 tespy-0.7.3/docs/modules.rst
+-rw-r--r--   0        0        0     5082 2023-11-27 18:42:13.368512 tespy-0.7.3/docs/modules/characteristics.rst
+-rw-r--r--   0        0        0    34468 2024-04-15 11:16:02.655136 tespy-0.7.3/docs/modules/components.rst
+-rw-r--r--   0        0        0    15728 2024-04-15 11:16:02.655136 tespy-0.7.3/docs/modules/connections.rst
+-rw-r--r--   0        0        0    15251 2024-04-15 11:16:02.656135 tespy-0.7.3/docs/modules/fluid_properties.rst
+-rw-r--r--   0        0        0    32940 2024-04-15 11:16:02.657137 tespy-0.7.3/docs/modules/networks.rst
+-rw-r--r--   0        0        0    12661 2024-04-15 17:02:58.316540 tespy-0.7.3/docs/modules/ude.rst
+-rw-r--r--   0        0        0    12186 2024-04-15 11:16:02.658135 tespy-0.7.3/docs/references.bib
+-rw-r--r--   0        0        0      886 2023-11-14 11:35:05.443458 tespy-0.7.3/docs/regular_meeting.rst
+-rw-r--r--   0        0        0       77 2024-02-08 10:33:11.165315 tespy-0.7.3/docs/requirements.txt
+-rw-r--r--   0        0        0     2914 2023-11-14 11:35:05.445457 tespy-0.7.3/docs/scripts/generate_tespy_data_module.py
+-rw-r--r--   0        0        0     3594 2023-11-27 18:42:13.369520 tespy-0.7.3/docs/tutorials.rst
+-rw-r--r--   0        0        0     2365 2023-11-27 18:42:13.369520 tespy-0.7.3/docs/tutorials/district_heating.rst
+-rw-r--r--   0        0        0    32094 2024-04-15 11:16:02.659136 tespy-0.7.3/docs/tutorials/heat_pump_exergy.rst
+-rw-r--r--   0        0        0    21439 2024-04-15 11:16:02.660136 tespy-0.7.3/docs/tutorials/heat_pump_steps.rst
+-rw-r--r--   0        0        0     7904 2023-11-27 18:42:13.369520 tespy-0.7.3/docs/tutorials/pygmo_optimization.rst
+-rw-r--r--   0        0        0     8543 2023-11-27 18:42:13.369520 tespy-0.7.3/docs/tutorials/starting_values.rst
+-rw-r--r--   0        0        0     1360 2024-04-15 17:02:58.316540 tespy-0.7.3/docs/whats_new.rst
+-rw-r--r--   0        0        0      240 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-0-1.rst
+-rw-r--r--   0        0        0     1548 2023-11-14 11:35:05.456506 tespy-0.7.3/docs/whats_new/v0-0-2.rst
+-rw-r--r--   0        0        0     4807 2023-11-14 11:35:05.457491 tespy-0.7.3/docs/whats_new/v0-0-3.rst
+-rw-r--r--   0        0        0     1994 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-0-4.rst
+-rw-r--r--   0        0        0     3293 2023-07-20 10:11:41.150532 tespy-0.7.3/docs/whats_new/v0-0-5.rst
+-rw-r--r--   0        0        0     3987 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-1-0.rst
+-rw-r--r--   0        0        0     4347 2023-11-14 11:35:05.459497 tespy-0.7.3/docs/whats_new/v0-1-1.rst
+-rw-r--r--   0        0        0     3842 2023-11-14 11:35:05.460492 tespy-0.7.3/docs/whats_new/v0-1-2.rst
+-rw-r--r--   0        0        0     2675 2023-11-14 11:35:05.462483 tespy-0.7.3/docs/whats_new/v0-1-3.rst
+-rw-r--r--   0        0        0      616 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-1-4.rst
+-rw-r--r--   0        0        0     8338 2023-11-14 11:35:05.463455 tespy-0.7.3/docs/whats_new/v0-2-0.rst
+-rw-r--r--   0        0        0     1982 2022-05-26 10:30:52.000000 tespy-0.7.3/docs/whats_new/v0-2-1.rst
+-rw-r--r--   0        0        0     3064 2023-11-14 11:35:05.465487 tespy-0.7.3/docs/whats_new/v0-2-2.rst
+-rw-r--r--   0        0        0    11252 2023-11-14 11:35:05.466489 tespy-0.7.3/docs/whats_new/v0-3-0.rst
+-rw-r--r--   0        0        0      314 2022-05-26 10:30:52.000000 tespy-0.7.3/docs/whats_new/v0-3-1.rst
+-rw-r--r--   0        0        0     2062 2023-07-20 10:11:41.153549 tespy-0.7.3/docs/whats_new/v0-3-2.rst
+-rw-r--r--   0        0        0     1345 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-3-3.rst
+-rw-r--r--   0        0        0     1471 2023-11-14 11:35:05.467454 tespy-0.7.3/docs/whats_new/v0-3-4.rst
+-rw-r--r--   0        0        0    11174 2023-11-14 11:35:05.468458 tespy-0.7.3/docs/whats_new/v0-4-0.rst
+-rw-r--r--   0        0        0     1126 2023-11-14 11:35:05.469487 tespy-0.7.3/docs/whats_new/v0-4-1.rst
+-rw-r--r--   0        0        0     1589 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-4-2.rst
+-rw-r--r--   0        0        0      563 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-4-3-001.rst
+-rw-r--r--   0        0        0      656 2023-11-14 11:35:05.470480 tespy-0.7.3/docs/whats_new/v0-4-3-003.rst
+-rw-r--r--   0        0        0     3355 2023-11-14 11:35:05.471499 tespy-0.7.3/docs/whats_new/v0-4-3.rst
+-rw-r--r--   0        0        0     1183 2022-01-28 07:48:36.000000 tespy-0.7.3/docs/whats_new/v0-4-4.rst
+-rw-r--r--   0        0        0      801 2022-01-28 07:48:36.000000 tespy-0.7.3/docs/whats_new/v0-5-0.rst
+-rw-r--r--   0        0        0      930 2022-05-26 10:30:52.000000 tespy-0.7.3/docs/whats_new/v0-5-1.rst
+-rw-r--r--   0        0        0     2644 2023-11-14 11:35:05.473451 tespy-0.7.3/docs/whats_new/v0-6-0.rst
+-rw-r--r--   0        0        0     2064 2023-11-14 11:35:05.474453 tespy-0.7.3/docs/whats_new/v0-6-1.rst
+-rw-r--r--   0        0        0      385 2023-11-14 11:35:05.475486 tespy-0.7.3/docs/whats_new/v0-6-2.rst
+-rw-r--r--   0        0        0     2841 2023-11-14 11:35:05.476510 tespy-0.7.3/docs/whats_new/v0-6-3.rst
+-rw-r--r--   0        0        0     4014 2024-04-15 11:16:02.661136 tespy-0.7.3/docs/whats_new/v0-7-0.rst
+-rw-r--r--   0        0        0      427 2024-04-15 11:16:02.661136 tespy-0.7.3/docs/whats_new/v0-7-1.rst
+-rw-r--r--   0        0        0      841 2024-04-15 11:16:02.662135 tespy-0.7.3/docs/whats_new/v0-7-2.rst
+-rw-r--r--   0        0        0      363 2024-04-15 17:01:52.744160 tespy-0.7.3/docs/whats_new/v0-7-3.rst
+-rw-r--r--   0        0        0       90 2023-11-14 11:35:05.478498 tespy-0.7.3/docs/zliterature.rst
+-rw-r--r--   0        0        0     6582 2023-11-14 11:35:05.480483 tespy-0.7.3/paper.bib
+-rw-r--r--   0        0        0    11023 2021-10-04 06:28:48.000000 tespy-0.7.3/paper.md
+-rw-r--r--   0        0        0     2607 2024-04-15 17:02:58.327058 tespy-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1187 2024-04-15 17:02:58.327058 tespy-0.7.3/src/tespy/__init__.py
+-rw-r--r--   0        0        0     1655 2024-04-15 11:16:02.664135 tespy-0.7.3/src/tespy/components/__init__.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/basics/__init__.py
+-rw-r--r--   0        0        0     5537 2024-02-20 16:14:00.450472 tespy-0.7.3/src/tespy/components/basics/cycle_closer.py
+-rw-r--r--   0        0        0     2695 2024-02-08 10:33:11.197316 tespy-0.7.3/src/tespy/components/basics/sink.py
+-rw-r--r--   0        0        0     3223 2024-02-20 16:14:00.450472 tespy-0.7.3/src/tespy/components/basics/source.py
+-rw-r--r--   0        0        0     5247 2024-02-08 10:33:11.202317 tespy-0.7.3/src/tespy/components/basics/subsystem_interface.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/combustion/__init__.py
+-rw-r--r--   0        0        0    47281 2024-04-15 11:16:02.664135 tespy-0.7.3/src/tespy/components/combustion/base.py
+-rw-r--r--   0        0        0    13831 2024-02-08 10:33:11.210315 tespy-0.7.3/src/tespy/components/combustion/diabatic.py
+-rw-r--r--   0        0        0    55747 2024-04-15 11:16:02.665135 tespy-0.7.3/src/tespy/components/combustion/engine.py
+-rw-r--r--   0        0        0    41460 2024-04-15 17:02:58.327058 tespy-0.7.3/src/tespy/components/component.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/customs/__init__.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/heat_exchangers/__init__.py
+-rw-r--r--   0        0        0    38259 2024-04-15 11:16:02.666134 tespy-0.7.3/src/tespy/components/heat_exchangers/base.py
+-rw-r--r--   0        0        0    18098 2024-04-15 11:16:02.667135 tespy-0.7.3/src/tespy/components/heat_exchangers/condenser.py
+-rw-r--r--   0        0        0     8531 2024-04-15 11:16:02.667135 tespy-0.7.3/src/tespy/components/heat_exchangers/desuperheater.py
+-rw-r--r--   0        0        0    13129 2024-04-15 11:16:02.667135 tespy-0.7.3/src/tespy/components/heat_exchangers/parabolic_trough.py
+-rw-r--r--   0        0        0    43440 2024-04-15 11:16:02.668135 tespy-0.7.3/src/tespy/components/heat_exchangers/simple.py
+-rw-r--r--   0        0        0    11356 2024-04-15 11:16:02.668135 tespy-0.7.3/src/tespy/components/heat_exchangers/solar_collector.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/nodes/__init__.py
+-rw-r--r--   0        0        0     6116 2024-04-15 11:16:02.669134 tespy-0.7.3/src/tespy/components/nodes/base.py
+-rw-r--r--   0        0        0    13308 2024-02-15 15:31:08.395117 tespy-0.7.3/src/tespy/components/nodes/droplet_separator.py
+-rw-r--r--   0        0        0    14951 2024-04-15 11:16:02.670135 tespy-0.7.3/src/tespy/components/nodes/drum.py
+-rw-r--r--   0        0        0    17177 2024-04-15 11:16:02.670135 tespy-0.7.3/src/tespy/components/nodes/merge.py
+-rw-r--r--   0        0        0    11927 2024-04-15 11:16:02.670135 tespy-0.7.3/src/tespy/components/nodes/separator.py
+-rw-r--r--   0        0        0     6693 2024-02-15 15:31:08.395117 tespy-0.7.3/src/tespy/components/nodes/splitter.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/piping/__init__.py
+-rw-r--r--   0        0        0     5352 2024-02-08 10:33:11.253315 tespy-0.7.3/src/tespy/components/piping/pipe.py
+-rw-r--r--   0        0        0    13658 2024-04-15 11:16:02.671136 tespy-0.7.3/src/tespy/components/piping/valve.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/reactors/__init__.py
+-rw-r--r--   0        0        0    27777 2024-04-15 11:16:02.671136 tespy-0.7.3/src/tespy/components/reactors/fuel_cell.py
+-rw-r--r--   0        0        0    40264 2024-04-15 11:16:02.672134 tespy-0.7.3/src/tespy/components/reactors/water_electrolyzer.py
+-rw-r--r--   0        0        0     2343 2024-04-15 11:16:02.673153 tespy-0.7.3/src/tespy/components/subsystem.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/turbomachinery/__init__.py
+-rw-r--r--   0        0        0     8475 2024-04-15 11:16:02.674135 tespy-0.7.3/src/tespy/components/turbomachinery/base.py
+-rw-r--r--   0        0        0    25801 2024-04-15 11:16:02.674135 tespy-0.7.3/src/tespy/components/turbomachinery/compressor.py
+-rw-r--r--   0        0        0    19150 2024-02-20 16:14:00.485473 tespy-0.7.3/src/tespy/components/turbomachinery/pump.py
+-rw-r--r--   0        0        0    19110 2024-02-15 15:31:08.411864 tespy-0.7.3/src/tespy/components/turbomachinery/turbine.py
+-rw-r--r--   0        0        0      147 2022-01-28 07:48:36.000000 tespy-0.7.3/src/tespy/connections/__init__.py
+-rw-r--r--   0        0        0    16918 2024-04-15 17:02:58.327058 tespy-0.7.3/src/tespy/connections/bus.py
+-rw-r--r--   0        0        0    44576 2024-04-15 17:02:58.327058 tespy-0.7.3/src/tespy/connections/connection.py
+-rw-r--r--   0        0        0     9270 2023-11-14 11:35:05.528493 tespy-0.7.3/src/tespy/data/ChemEx/Ahrendts.json
+-rw-r--r--   0        0        0     8407 2023-11-14 11:35:05.530494 tespy-0.7.3/src/tespy/data/ChemEx/Szargut1988.json
+-rw-r--r--   0        0        0     8578 2023-11-14 11:35:05.532488 tespy-0.7.3/src/tespy/data/ChemEx/Szargut2007.json
+-rw-r--r--   0        0        0     8047 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/data/char_lines.json
+-rw-r--r--   0        0        0     3726 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/data/char_maps.json
+-rw-r--r--   0        0        0      118 2022-01-28 07:48:36.000000 tespy-0.7.3/src/tespy/networks/__init__.py
+-rw-r--r--   0        0        0   107289 2024-04-15 17:02:58.327058 tespy-0.7.3/src/tespy/networks/network.py
+-rw-r--r--   0        0        0    15070 2024-04-15 11:16:02.676160 tespy-0.7.3/src/tespy/networks/network_reader.py
+-rw-r--r--   0        0        0      940 2024-04-15 17:02:58.327058 tespy-0.7.3/src/tespy/tools/__init__.py
+-rw-r--r--   0        0        0    38453 2024-04-15 11:16:02.677134 tespy-0.7.3/src/tespy/tools/analyses.py
+-rw-r--r--   0        0        0    17458 2024-04-15 17:02:58.342708 tespy-0.7.3/src/tespy/tools/characteristics.py
+-rw-r--r--   0        0        0    17346 2024-04-15 17:02:58.342708 tespy-0.7.3/src/tespy/tools/data_containers.py
+-rw-r--r--   0        0        0    38786 2024-02-08 10:33:11.297315 tespy-0.7.3/src/tespy/tools/document_models.py
+-rw-r--r--   0        0        0     1046 2024-04-15 11:16:02.678134 tespy-0.7.3/src/tespy/tools/fluid_properties/__init__.py
+-rw-r--r--   0        0        0     9666 2024-04-15 11:16:02.678134 tespy-0.7.3/src/tespy/tools/fluid_properties/functions.py
+-rw-r--r--   0        0        0     9700 2024-04-15 11:16:02.679134 tespy-0.7.3/src/tespy/tools/fluid_properties/helpers.py
+-rw-r--r--   0        0        0    12386 2024-04-15 11:16:02.679134 tespy-0.7.3/src/tespy/tools/fluid_properties/mixtures.py
+-rw-r--r--   0        0        0    13368 2024-04-15 11:16:02.680134 tespy-0.7.3/src/tespy/tools/fluid_properties/wrappers.py
+-rw-r--r--   0        0        0     3454 2024-04-15 11:16:02.680134 tespy-0.7.3/src/tespy/tools/global_vars.py
+-rw-r--r--   0        0        0    20301 2024-04-15 17:02:58.342708 tespy-0.7.3/src/tespy/tools/helpers.py
+-rw-r--r--   0        0        0    15049 2024-04-15 11:16:02.681134 tespy-0.7.3/src/tespy/tools/logger.py
+-rw-r--r--   0        0        0    10421 2024-04-15 11:16:02.682134 tespy-0.7.3/src/tespy/tools/optimization.py
+-rw-r--r--   0        0        0      427 2024-04-15 11:16:02.682134 tespy-0.7.3/tests/test_advanced_tutorials.py
+-rw-r--r--   0        0        0     4337 2024-02-08 10:33:11.326315 tespy-0.7.3/tests/test_analyses/test_entropy_analysis.py
+-rw-r--r--   0        0        0    24440 2024-02-08 10:33:11.329316 tespy-0.7.3/tests/test_analyses/test_exergy_analysis.py
+-rw-r--r--   0        0        0      315 2024-04-15 11:16:02.683135 tespy-0.7.3/tests/test_basic_tutorials.py
+-rw-r--r--   0        0        0    10214 2024-04-15 11:16:02.684136 tespy-0.7.3/tests/test_busses.py
+-rw-r--r--   0        0        0    11728 2024-04-15 11:16:02.685134 tespy-0.7.3/tests/test_components/test_combustion.py
+-rw-r--r--   0        0        0      346 2024-02-08 10:33:11.339314 tespy-0.7.3/tests/test_components/test_customs.py
+-rw-r--r--   0        0        0     1627 2024-04-15 11:16:02.685134 tespy-0.7.3/tests/test_components/test_drum.py
+-rw-r--r--   0        0        0    23305 2024-02-08 10:33:11.344314 tespy-0.7.3/tests/test_components/test_heat_exchangers.py
+-rw-r--r--   0        0        0     4028 2024-04-15 11:16:02.685134 tespy-0.7.3/tests/test_components/test_merge.py
+-rw-r--r--   0        0        0     3150 2024-02-08 10:33:11.349315 tespy-0.7.3/tests/test_components/test_piping.py
+-rw-r--r--   0        0        0     7107 2024-04-15 11:16:02.686134 tespy-0.7.3/tests/test_components/test_reactors.py
+-rw-r--r--   0        0        0    17021 2024-02-08 10:33:11.356315 tespy-0.7.3/tests/test_components/test_turbomachinery.py
+-rw-r--r--   0        0        0     4025 2024-04-15 11:16:02.686134 tespy-0.7.3/tests/test_connections.py
+-rw-r--r--   0        0        0    20109 2024-04-15 16:52:09.433248 tespy-0.7.3/tests/test_errors.py
+-rw-r--r--   0        0        0      455 2024-04-15 11:16:02.686134 tespy-0.7.3/tests/test_heat_pump_exergy.py
+-rw-r--r--   0        0        0      996 2023-11-14 11:35:05.574460 tespy-0.7.3/tests/test_models/cgam-ebsilon-results.csv
+-rw-r--r--   0        0        0     7604 2024-02-08 10:33:11.365316 tespy-0.7.3/tests/test_models/test_CGAM_model.py
+-rw-r--r--   0        0        0    12500 2024-02-08 10:33:11.369315 tespy-0.7.3/tests/test_models/test_heat_pump_model.py
+-rw-r--r--   0        0        0    18609 2024-02-08 10:33:11.371315 tespy-0.7.3/tests/test_models/test_solar_energy_generating_system.py
+-rw-r--r--   0        0        0     1664 2024-04-15 11:16:02.687135 tespy-0.7.3/tests/test_networks/test_binary_incompressible.py
+-rw-r--r--   0        0        0     5571 2024-04-15 11:16:02.688135 tespy-0.7.3/tests/test_networks/test_mixing_rules.py
+-rw-r--r--   0        0        0    24711 2024-04-15 11:16:02.688135 tespy-0.7.3/tests/test_networks/test_network.py
+-rw-r--r--   0        0        0     7913 2023-11-27 18:42:13.447683 tespy-0.7.3/tests/test_tools/test_characteristics.py
+-rw-r--r--   0        0        0    12983 2024-02-08 10:33:11.383315 tespy-0.7.3/tests/test_tools/test_fluid_properties/test_coolprop.py
+-rw-r--r--   0        0        0     2106 2024-02-08 10:33:11.385316 tespy-0.7.3/tests/test_tools/test_fluid_properties/test_iapws.py
+-rw-r--r--   0        0        0     1385 2024-02-08 10:33:11.387315 tespy-0.7.3/tests/test_tools/test_fluid_properties/test_pyromat.py
+-rw-r--r--   0        0        0     2237 2024-04-15 17:02:58.342708 tespy-0.7.3/tests/test_tools/test_helpers.py
+-rw-r--r--   0        0        0     2000 2024-02-08 10:33:11.392315 tespy-0.7.3/tox.ini
+-rw-r--r--   0        0        0      261 2024-02-08 10:33:11.396315 tespy-0.7.3/tutorial/README.rst
+-rw-r--r--   0        0        0     9727 2024-04-15 11:16:02.689135 tespy-0.7.3/tutorial/advanced/optimization_example.py
+-rw-r--r--   0        0        0     9541 2024-04-15 11:16:02.690135 tespy-0.7.3/tutorial/advanced/starting_values.py
+-rw-r--r--   0        0        0     6090 2024-04-15 11:16:02.691134 tespy-0.7.3/tutorial/advanced/stepwise.py
+-rw-r--r--   0        0        0     4264 2024-02-08 10:33:11.406315 tespy-0.7.3/tutorial/basics/district_heating.py
+-rw-r--r--   0        0        0     4978 2024-04-15 11:16:02.691134 tespy-0.7.3/tutorial/basics/gas_turbine.py
+-rw-r--r--   0        0        0     3216 2024-02-08 10:33:11.411315 tespy-0.7.3/tutorial/basics/heat_pump.py
+-rw-r--r--   0        0        0     4661 2024-04-15 11:16:02.692154 tespy-0.7.3/tutorial/basics/rankine.py
+-rw-r--r--   0        0        0     4201 2024-02-08 10:33:11.416315 tespy-0.7.3/tutorial/heat_pump_exergy/NH3.py
+-rw-r--r--   0        0        0    10920 2024-04-15 11:16:02.693134 tespy-0.7.3/tutorial/heat_pump_exergy/NH3_calculations.py
+-rw-r--r--   0        0        0     4217 2024-02-08 10:33:11.421314 tespy-0.7.3/tutorial/heat_pump_exergy/R410A.py
+-rw-r--r--   0        0        0    10943 2024-04-15 11:16:02.693134 tespy-0.7.3/tutorial/heat_pump_exergy/R410A_calculations.py
+-rw-r--r--   0        0        0     8277 2024-02-08 10:33:11.426314 tespy-0.7.3/tutorial/heat_pump_exergy/plots.py
+-rw-r--r--   0        0        0    10587 1970-01-01 00:00:00.000000 tespy-0.7.3/PKG-INFO
```

### Comparing `tespy-0.7.2.post2/.pep8speaks.yml` & `tespy-0.7.3/.pep8speaks.yml`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/CODE_OF_CONDUCT.md` & `tespy-0.7.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/LICENSE` & `tespy-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/PULL_REQUEST_TEMPLATE.md` & `tespy-0.7.3/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/README.rst` & `tespy-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/advanced/exergy/flowsheet.svg` & `tespy-0.7.3/docs/_static/images/advanced/exergy/flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/advanced/exergy/flowsheet_darkmode.svg` & `tespy-0.7.3/docs/_static/images/advanced/exergy/flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/advanced/exergy/sankey.svg` & `tespy-0.7.3/docs/_static/images/advanced/exergy/sankey.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/district_heating.svg` & `tespy-0.7.3/docs/_static/images/basics/district_heating.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/district_heating_darkmode.svg` & `tespy-0.7.3/docs/_static/images/basics/district_heating_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/district_heating_partload.svg` & `tespy-0.7.3/docs/_static/images/basics/district_heating_partload.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/district_heating_partload_darkmode.svg` & `tespy-0.7.3/docs/_static/images/basics/district_heating_partload_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine.svg` & `tespy-0.7.3/docs/_static/images/basics/gas_turbine.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_darkmode.svg` & `tespy-0.7.3/docs/_static/images/basics/gas_turbine_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_fuel_composition.svg` & `tespy-0.7.3/docs/_static/images/basics/gas_turbine_fuel_composition.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_fuel_composition_darkmode.svg` & `tespy-0.7.3/docs/_static/images/basics/gas_turbine_fuel_composition_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_oxygen.svg` & `tespy-0.7.3/docs/_static/images/basics/gas_turbine_oxygen.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_oxygen_darkmode.svg` & `tespy-0.7.3/docs/_static/images/basics/gas_turbine_oxygen_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_parametric.svg` & `tespy-0.7.3/docs/_static/images/basics/gas_turbine_parametric.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/gas_turbine_parametric_darkmode.svg` & `tespy-0.7.3/docs/_static/images/basics/gas_turbine_parametric_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/heat_pump.svg` & `tespy-0.7.3/docs/_static/images/basics/heat_pump.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/heat_pump_darkmode.svg` & `tespy-0.7.3/docs/_static/images/basics/heat_pump_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/heat_pump_parametric.svg` & `tespy-0.7.3/docs/_static/images/basics/heat_pump_parametric.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/heat_pump_parametric_darkmode.svg` & `tespy-0.7.3/docs/_static/images/basics/heat_pump_parametric_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/modeling_concept.svg` & `tespy-0.7.3/docs/_static/images/basics/modeling_concept.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/rankine_cycle.svg` & `tespy-0.7.3/docs/_static/images/basics/rankine_cycle.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/rankine_cycle_darkmode.svg` & `tespy-0.7.3/docs/_static/images/basics/rankine_cycle_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/rankine_parametric.svg` & `tespy-0.7.3/docs/_static/images/basics/rankine_parametric.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/rankine_parametric_darkmode.svg` & `tespy-0.7.3/docs/_static/images/basics/rankine_parametric_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/rankine_partload.svg` & `tespy-0.7.3/docs/_static/images/basics/rankine_partload.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/basics/rankine_partload_darkmode.svg` & `tespy-0.7.3/docs/_static/images/basics/rankine_partload_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/examples/GRC_flowsheet.svg` & `tespy-0.7.3/docs/_static/images/examples/GRC_flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/examples/GRC_flowsheet_darkmode.svg` & `tespy-0.7.3/docs/_static/images/examples/GRC_flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/examples/ORC_parametric_flowsheet.svg` & `tespy-0.7.3/docs/_static/images/examples/ORC_parametric_flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/examples/ORC_parametric_flowsheet_darkmode.svg` & `tespy-0.7.3/docs/_static/images/examples/ORC_parametric_flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/examples/PM_CAES_graphical-abstract.svg` & `tespy-0.7.3/docs/_static/images/examples/PM_CAES_graphical-abstract.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/examples/PM_CAES_graphical-abstract_darkmode.svg` & `tespy-0.7.3/docs/_static/images/examples/PM_CAES_graphical-abstract_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/logo_tespy_big.svg` & `tespy-0.7.3/docs/_static/images/logo_tespy_big.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/logo_tespy_big_darkmode.svg` & `tespy-0.7.3/docs/_static/images/logo_tespy_big_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/logo_tespy_big_editable_font.svg` & `tespy-0.7.3/docs/_static/images/logo_tespy_big_editable_font.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/logo_tespy_mid.svg` & `tespy-0.7.3/docs/_static/images/logo_tespy_mid.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/logo_tespy_mid_christmas.svg` & `tespy-0.7.3/docs/_static/images/logo_tespy_mid_christmas.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/logo_tespy_mid_darkmode.svg` & `tespy-0.7.3/docs/_static/images/logo_tespy_mid_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/logo_tespy_mid_darkmode_christmas.svg` & `tespy-0.7.3/docs/_static/images/logo_tespy_mid_darkmode_christmas.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/logo_tespy_mid_editable_font.svg` & `tespy-0.7.3/docs/_static/images/logo_tespy_mid_editable_font.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/logo_tespy_mini.svg` & `tespy-0.7.3/docs/_static/images/logo_tespy_mini.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/logo_tespy_small.svg` & `tespy-0.7.3/docs/_static/images/logo_tespy_small.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/modules/Ts_diagram_states.svg` & `tespy-0.7.3/docs/_static/images/modules/Ts_diagram_states.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/modules/characteristics.svg` & `tespy-0.7.3/docs/_static/images/modules/characteristics.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/modules/characteristics_darkmode.svg` & `tespy-0.7.3/docs/_static/images/modules/characteristics_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/modules/connections.svg` & `tespy-0.7.3/docs/_static/images/modules/connections.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/modules/connections_darkmode.svg` & `tespy-0.7.3/docs/_static/images/modules/connections_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/modules/fluid_properties.svg` & `tespy-0.7.3/docs/_static/images/modules/fluid_properties.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/modules/fluid_properties_darkmode.svg` & `tespy-0.7.3/docs/_static/images/modules/fluid_properties_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/modules/logph_diagram_states.svg` & `tespy-0.7.3/docs/_static/images/modules/logph_diagram_states.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/modules/subsystem_waste_heat_generator.svg` & `tespy-0.7.3/docs/_static/images/modules/subsystem_waste_heat_generator.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/modules/subsystem_waste_heat_generator_darkmode.svg` & `tespy-0.7.3/docs/_static/images/modules/subsystem_waste_heat_generator_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/modules/ude.svg` & `tespy-0.7.3/docs/_static/images/modules/ude.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/modules/ude_darkmode.svg` & `tespy-0.7.3/docs/_static/images/modules/ude_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/district_heating_system/dhs.svg` & `tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/district_heating_system/dhs_closed.svg` & `tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs_closed.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/district_heating_system/dhs_forks.svg` & `tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs_forks.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/district_heating_system/dhs_open.svg` & `tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs_open.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/NH3_logph.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/NH3_logph.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/NH3_sankey.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/NH3_sankey.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/flowsheet.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_exergy/flowsheet_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_starting_values/logph.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/logph.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/osmses-2023.svg` & `tespy-0.7.3/docs/_static/images/tutorials/osmses-2023.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/osmses-2023_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/osmses-2023_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/pygmo_optimization/flowsheet.svg` & `tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/pygmo_optimization/flowsheet_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization.svg` & `tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization_darkmode.svg` & `tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/_static/js/custom.js` & `tespy-0.7.3/docs/_static/js/custom.js`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/advanced/exergy.rst` & `tespy-0.7.3/docs/advanced/exergy.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api.rst` & `tespy-0.7.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/CombustionChamber.svg` & `tespy-0.7.3/docs/api/_images/CombustionChamber.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/CombustionChamber_darkmode.svg` & `tespy-0.7.3/docs/api/_images/CombustionChamber_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/CombustionEngine.svg` & `tespy-0.7.3/docs/api/_images/CombustionEngine.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/CombustionEngine_darkmode.svg` & `tespy-0.7.3/docs/api/_images/CombustionEngine_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Compressor.svg` & `tespy-0.7.3/docs/api/_images/Compressor.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Compressor_darkmode.svg` & `tespy-0.7.3/docs/api/_images/Compressor_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Condenser.svg` & `tespy-0.7.3/docs/api/_images/Condenser.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Condenser_darkmode.svg` & `tespy-0.7.3/docs/api/_images/Condenser_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/DropletSeparator.svg` & `tespy-0.7.3/docs/api/_images/DropletSeparator.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/DropletSeparator_darkmode.svg` & `tespy-0.7.3/docs/api/_images/DropletSeparator_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Drum.svg` & `tespy-0.7.3/docs/api/_images/Drum.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Drum_darkmode.svg` & `tespy-0.7.3/docs/api/_images/Drum_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/FuelCell.svg` & `tespy-0.7.3/docs/api/_images/FuelCell.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/FuelCell_darkmode.svg` & `tespy-0.7.3/docs/api/_images/FuelCell_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/HeatExchanger.svg` & `tespy-0.7.3/docs/api/_images/HeatExchanger.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/HeatExchanger_darkmode.svg` & `tespy-0.7.3/docs/api/_images/HeatExchanger_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Merge.svg` & `tespy-0.7.3/docs/api/_images/Merge.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Merge_darkmode.svg` & `tespy-0.7.3/docs/api/_images/Merge_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/ORCEvaporator.svg` & `tespy-0.7.3/docs/api/_images/ORCEvaporator.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/ParabolicTrough.svg` & `tespy-0.7.3/docs/api/_images/ParabolicTrough.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/ParabolicTrough_darkmode.svg` & `tespy-0.7.3/docs/api/_images/ParabolicTrough_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Pipe.svg` & `tespy-0.7.3/docs/api/_images/Pipe.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Pipe_darkmode.svg` & `tespy-0.7.3/docs/api/_images/Pipe_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Pump.svg` & `tespy-0.7.3/docs/api/_images/Pump.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Pump_darkmode.svg` & `tespy-0.7.3/docs/api/_images/Pump_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/SolarCollector.svg` & `tespy-0.7.3/docs/api/_images/SolarCollector.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/SolarCollector_darkmode.svg` & `tespy-0.7.3/docs/api/_images/SolarCollector_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Splitter.svg` & `tespy-0.7.3/docs/api/_images/Splitter.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Splitter_darkmode.svg` & `tespy-0.7.3/docs/api/_images/Splitter_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/SubsystemInterface.svg` & `tespy-0.7.3/docs/api/_images/SubsystemInterface.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/SubsystemInterface_darkmode.svg` & `tespy-0.7.3/docs/api/_images/SubsystemInterface_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Turbine.svg` & `tespy-0.7.3/docs/api/_images/Turbine.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Turbine_darkmode.svg` & `tespy-0.7.3/docs/api/_images/Turbine_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Valve.svg` & `tespy-0.7.3/docs/api/_images/Valve.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/Valve_darkmode.svg` & `tespy-0.7.3/docs/api/_images/Valve_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/WaterElectrolyzer.svg` & `tespy-0.7.3/docs/api/_images/WaterElectrolyzer.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/WaterElectrolyzer_darkmode.svg` & `tespy-0.7.3/docs/api/_images/WaterElectrolyzer_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/combustion_engine_Q1_char_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/combustion_engine_Q1_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/combustion_engine_Q2_char_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/combustion_engine_Q2_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/combustion_engine_Qloss_char_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/combustion_engine_Qloss_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/combustion_engine_tiP_char_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/combustion_engine_tiP_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/compressor_char_map_eta_s_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/compressor_char_map_eta_s_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/compressor_char_map_pr_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/compressor_char_map_pr_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/compressor_eta_s_char_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/compressor_eta_s_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/condenser_kA_char1_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/condenser_kA_char1_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/condenser_kA_char2_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/condenser_kA_char2_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/desuperheater_kA_char1_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/desuperheater_kA_char1_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/desuperheater_kA_char2_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/desuperheater_kA_char2_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/heat_exchanger_kA_char1_CONDENSING_FLUID.svg` & `tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char1_CONDENSING_FLUID.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/heat_exchanger_kA_char1_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char1_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/heat_exchanger_kA_char2_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char2_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/heat_exchanger_kA_char2_EVAPORATING_FLUID.svg` & `tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char2_EVAPORATING_FLUID.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/heat_exchanger_simple_kA_char_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/heat_exchanger_simple_kA_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/pipe_kA_char_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/pipe_kA_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/pump_eta_s_char_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/pump_eta_s_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/turbine_eta_s_char_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/turbine_eta_s_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/turbine_eta_s_char_TRAUPEL.svg` & `tespy-0.7.3/docs/api/_images/turbine_eta_s_char_TRAUPEL.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/_images/water_electrolyzer_eta_char_DEFAULT.svg` & `tespy-0.7.3/docs/api/_images/water_electrolyzer_eta_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/components.rst` & `tespy-0.7.3/docs/api/components.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/data.rst` & `tespy-0.7.3/docs/api/data.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/api/tools.rst` & `tespy-0.7.3/docs/api/tools.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/basics.rst` & `tespy-0.7.3/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/basics/district_heating.rst` & `tespy-0.7.3/docs/basics/district_heating.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/basics/gas_turbine.rst` & `tespy-0.7.3/docs/basics/gas_turbine.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/basics/heat_pump.rst` & `tespy-0.7.3/docs/basics/heat_pump.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/basics/intro.rst` & `tespy-0.7.3/docs/basics/intro.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/basics/rankine_cycle.rst` & `tespy-0.7.3/docs/basics/rankine_cycle.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/benchmarks.rst` & `tespy-0.7.3/docs/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/conf.py` & `tespy-0.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/development/how.rst` & `tespy-0.7.3/docs/development/how.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/development/what.rst` & `tespy-0.7.3/docs/development/what.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/examples.rst` & `tespy-0.7.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/index.rst` & `tespy-0.7.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/installation.rst` & `tespy-0.7.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/introduction.rst` & `tespy-0.7.3/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/modules.rst` & `tespy-0.7.3/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/modules/characteristics.rst` & `tespy-0.7.3/docs/modules/characteristics.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/modules/components.rst` & `tespy-0.7.3/docs/modules/components.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/modules/connections.rst` & `tespy-0.7.3/docs/modules/connections.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/modules/fluid_properties.rst` & `tespy-0.7.3/docs/modules/fluid_properties.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/modules/networks.rst` & `tespy-0.7.3/docs/modules/networks.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/modules/ude.rst` & `tespy-0.7.3/docs/modules/ude.rst`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 create an instance with the respective data. First, we set up the TESPy model.
 
 .. code-block:: python
 
     >>> from tespy.networks import Network
     >>> from tespy.components import Sink, Source
     >>> from tespy.connections import Connection
-    >>> from tespy.tools.helpers import UserDefinedEquation
+    >>> from tespy.tools import UserDefinedEquation
 
     >>> nw = Network(iterinfo=False)
     >>> nw.set_attr(p_unit='bar', T_unit='C', h_unit='kJ / kg')
 
     >>> so1 = Source('source 1')
     >>> so2 = Source('source 2')
     >>> si1 = Sink('sink 1')
@@ -61,23 +61,23 @@
 specification of the volumetric flow, we are missing the mass flow of the
 connection :code:`c1`. As described, its value should be quadratic to the
 (still unknown) mass flow of :code:`c2`. First, we now need to define the
 equation in a function which returns the residual value of the equation.
 
 .. code-block:: python
 
-    >>> def my_ude(self):
-    ...     return self.conns[0].m.val_SI - self.conns[1].m.val_SI ** 2
+    >>> def my_ude(ude):
+    ...     return ude.conns[0].m.val_SI - ude.conns[1].m.val_SI ** 2
 
 
 .. note::
 
     The function must only take one parameter, i.e. the UserDefinedEquation
     class instance. The **name of the parameter is arbitrary**. We will use
-    :code:`self` in this example. It serves to access some important parameters
+    :code:`ude` in this example. It serves to access some important parameters
     of the equation:
 
     - connections required in the equation
     - Jacobian matrix to place the partial derivatives
     - automatic numerical derivatives
     - other (external) parameters (e.g. the CharLine in the API docs example of
       :py:class:`tespy.tools.helpers.UserDefinedEquation`)
@@ -90,15 +90,15 @@
 
 The second step is to define the derivatives with respect to all primary
 variables of the network, i.e. mass flow, pressure, enthalpy and fluid
 composition of every connection. The derivatives have to be passed to the
 Jacobian. In order to do this, we create a function that updates the values
 inside the Jacobian of the :code:`UserDefinedEquation` and returns it:
 
-- :code:`self.jacobian` is a dictionary containing numpy arrays for every
+- :code:`ude.jacobian` is a dictionary containing numpy arrays for every
   connection required by the :code:`UserDefinedEquation`.
 - derivatives to **mass flow** are placed in the first element of the numpy
   array (**index 0**)
 - derivatives to **pressure** are placed in the second element of the numpy
   array (**index 1**)
 - derivatives to **enthalpy** are placed in the third element of the numpy
   array (**index 2**)
@@ -110,21 +110,21 @@
 
 - The derivative to mass flow of connection :code:`c1` is equal to :math:`1`
 - The derivative to mass flow of connection :code:`c2` is equal to
   :math:`-2 \cdot \dot{m}_2`.
 
 .. code-block:: python
 
-    >>> def my_ude_deriv(self):
-    ...     c0 = self.conns[0]
-    ...     c1 = self.conns[1]
+    >>> def my_ude_deriv(ude):
+    ...     c0 = ude.conns[0]
+    ...     c1 = ude.conns[1]
     ...     if c0.m.is_var:
-    ...         self.jacobian[c0.m.J_col] = 1
+    ...         ude.jacobian[c0.m.J_col] = 1
     ...     if c1.m.is_var:
-    ...         self.jacobian[c1.m.J_col] = -2 * self.conns[1].m.val_SI
+    ...         ude.jacobian[c1.m.J_col] = -2 * ude.conns[1].m.val_SI
 
 Now we can create our instance of the :code:`UserDefinedEquation` and add it to
 the network. The class requires four mandatory arguments to be passed:
 
 - :code:`label` of type String.
 - :code:`func` which is the function holding the equation to be applied.
 - :code:`deriv` which is the function holding the calculation of the Jacobian.
@@ -181,29 +181,29 @@
 respectively to calculate the partial derivatives.
 
 .. code-block:: python
 
     >>> from tespy.tools.fluid_properties import dT_mix_dph
     >>> from tespy.tools.fluid_properties import dT_mix_pdh
 
-    >>> def my_ude_deriv(self):
-    ...     c0 = self.conns[0]
-    ...     c1 = self.conns[1]
+    >>> def my_ude_deriv(ude):
+    ...     c0 = ude.conns[0]
+    ...     c1 = ude.conns[1]
     ...     if c0.m.is_var:
-    ...         self.jacobian[c0.m.J_col] = 1 / self.conns[0].m.val_SI
+    ...         ude.jacobian[c0.m.J_col] = 1 / ude.conns[0].m.val_SI
     ...     if c0.p.is_var:
-    ...         self.jacobian[c0.p.J_col] = - 2 / self.conns[0].p.val_SI
+    ...         ude.jacobian[c0.p.J_col] = - 2 / ude.conns[0].p.val_SI
     ...     T = c1.calc_T()
     ...     if c1.p.is_var:
-    ...         self.jacobian[c1.p.J_col] = (
+    ...         ude.jacobian[c1.p.J_col] = (
     ...             dT_mix_dph(c1.p.val_SI, c1.h.val_SI, c1.fluid_data, c1.mixing_rule)
     ...             * 0.5 / (T ** 0.5)
     ...         )
     ...     if c1.h.is_var:
-    ...         self.jacobian[c1.h.J_col] = (
+    ...         ude.jacobian[c1.h.J_col] = (
     ...             dT_mix_pdh(c1.p.val_SI, c1.h.val_SI, c1.fluid_data, c1.mixing_rule)
     ...             * 0.5 / (T ** 0.5)
     ...         )
 
 But, what if the analytical derivative is not available? You can make use of
 generic numerical derivatives using the inbuilt method :code:`numeric_deriv`.
 The methods expects the variable :code:`'m'`, :code:`'p'`, :code:`'h'` or
@@ -261,35 +261,35 @@
     \left(h_2 - h\left(p_1, x=b \right)\right)
 
 .. code-block:: python
 
     >>> from tespy.tools.fluid_properties import h_mix_pQ
     >>> from tespy.tools.fluid_properties import dh_mix_dpQ
 
-    >>> def my_ude(self):
-    ...     a = self.params['a']
-    ...     b = self.params['b']
-    ...     c0 = self.conns[0]
-    ...     c1 = self.conns[1]
+    >>> def my_ude(ude):
+    ...     a = ude.params['a']
+    ...     b = ude.params['b']
+    ...     c0 = ude.conns[0]
+    ...     c1 = ude.conns[1]
     ...     return (
     ...         a * (c1.h.val_SI - c0.h.val_SI) -
     ...         (c1.h.val_SI - h_mix_pQ(c0.p.val_SI, b, c0.fluid_data))
     ...     )
 
-    >>> def my_ude_deriv(self):
-    ...     a = self.params['a']
-    ...     b = self.params['b']
-    ...     c0 = self.conns[0]
-    ...     c1 = self.conns[1]
+    >>> def my_ude_deriv(ude):
+    ...     a = ude.params['a']
+    ...     b = ude.params['b']
+    ...     c0 = ude.conns[0]
+    ...     c1 = ude.conns[1]
     ...     if c0.p.is_var:
-    ...         self.jacobian[c0.p.J_col] = dh_mix_dpQ(c0.p.val_SI, b, c0.fluid_data)
+    ...         ude.jacobian[c0.p.J_col] = dh_mix_dpQ(c0.p.val_SI, b, c0.fluid_data)
     ...     if c0.h.is_var:
-    ...         self.jacobian[c0.h.J_col] = -a
+    ...         ude.jacobian[c0.h.J_col] = -a
     ...     if c1.p.is_var:
-    ...         self.jacobian[c1.p.J_col] = a - 1
+    ...         ude.jacobian[c1.p.J_col] = a - 1
 
     >>> ude = UserDefinedEquation(
     ...     'my ude', my_ude, my_ude_deriv, [c1, c2], params={'a': 0.5, 'b': 1}
     ... )
 
 
 One more example (using a CharLine for data point interpolation) can be found in
```

### Comparing `tespy-0.7.2.post2/docs/references.bib` & `tespy-0.7.3/docs/references.bib`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/regular_meeting.rst` & `tespy-0.7.3/docs/regular_meeting.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/scripts/generate_tespy_data_module.py` & `tespy-0.7.3/docs/scripts/generate_tespy_data_module.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/tutorials.rst` & `tespy-0.7.3/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/tutorials/district_heating.rst` & `tespy-0.7.3/docs/tutorials/district_heating.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/tutorials/heat_pump_exergy.rst` & `tespy-0.7.3/docs/tutorials/heat_pump_exergy.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/tutorials/heat_pump_steps.rst` & `tespy-0.7.3/docs/tutorials/heat_pump_steps.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/tutorials/pygmo_optimization.rst` & `tespy-0.7.3/docs/tutorials/pygmo_optimization.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/tutorials/starting_values.rst` & `tespy-0.7.3/docs/tutorials/starting_values.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new.rst` & `tespy-0.7.3/docs/whats_new.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 What's New
 ~~~~~~~~~~
 
-Discover noteable new features and improvements in each release
+Discover notable new features and improvements in each release
 
+.. include::  whats_new/v0-7-3.rst
 .. include::  whats_new/v0-7-2.rst
 .. include::  whats_new/v0-7-1.rst
 .. include::  whats_new/v0-7-0.rst
 .. include::  whats_new/v0-6-3.rst
 .. include::  whats_new/v0-6-2.rst
 .. include::  whats_new/v0-6-1.rst
 .. include::  whats_new/v0-6-0.rst
```

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-0-2.rst` & `tespy-0.7.3/docs/whats_new/v0-0-2.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-0-3.rst` & `tespy-0.7.3/docs/whats_new/v0-0-3.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-0-4.rst` & `tespy-0.7.3/docs/whats_new/v0-0-4.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-0-5.rst` & `tespy-0.7.3/docs/whats_new/v0-0-5.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-1-0.rst` & `tespy-0.7.3/docs/whats_new/v0-1-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-1-1.rst` & `tespy-0.7.3/docs/whats_new/v0-1-1.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-1-2.rst` & `tespy-0.7.3/docs/whats_new/v0-1-2.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-1-3.rst` & `tespy-0.7.3/docs/whats_new/v0-1-3.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-1-4.rst` & `tespy-0.7.3/docs/whats_new/v0-1-4.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-2-0.rst` & `tespy-0.7.3/docs/whats_new/v0-2-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-2-1.rst` & `tespy-0.7.3/docs/whats_new/v0-2-1.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-2-2.rst` & `tespy-0.7.3/docs/whats_new/v0-2-2.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-3-0.rst` & `tespy-0.7.3/docs/whats_new/v0-3-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-3-2.rst` & `tespy-0.7.3/docs/whats_new/v0-3-2.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-3-3.rst` & `tespy-0.7.3/docs/whats_new/v0-3-3.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-3-4.rst` & `tespy-0.7.3/docs/whats_new/v0-3-4.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-4-0.rst` & `tespy-0.7.3/docs/whats_new/v0-4-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-4-1.rst` & `tespy-0.7.3/docs/whats_new/v0-4-1.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-4-2.rst` & `tespy-0.7.3/docs/whats_new/v0-4-2.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-4-3-001.rst` & `tespy-0.7.3/docs/whats_new/v0-4-3-001.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-4-3-003.rst` & `tespy-0.7.3/docs/whats_new/v0-4-3-003.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-4-3.rst` & `tespy-0.7.3/docs/whats_new/v0-4-3.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-4-4.rst` & `tespy-0.7.3/docs/whats_new/v0-4-4.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-5-0.rst` & `tespy-0.7.3/docs/whats_new/v0-5-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-5-1.rst` & `tespy-0.7.3/docs/whats_new/v0-5-1.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-6-0.rst` & `tespy-0.7.3/docs/whats_new/v0-6-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-6-1.rst` & `tespy-0.7.3/docs/whats_new/v0-6-1.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-6-3.rst` & `tespy-0.7.3/docs/whats_new/v0-6-3.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-7-0.rst` & `tespy-0.7.3/docs/whats_new/v0-7-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/docs/whats_new/v0-7-2.rst` & `tespy-0.7.3/docs/whats_new/v0-7-2.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/paper.bib` & `tespy-0.7.3/paper.bib`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/paper.md` & `tespy-0.7.3/paper.md`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/pyproject.toml` & `tespy-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "tests/",
     "tutorial/",
 ]
 exclude = ["docs/_build"]
 
 [project]
 name = "tespy"
-version = "0.7.2.post2"
+version = "0.7.3"
 description = "Thermal Engineering Systems in Python (TESPy)"
 readme = "README.rst"
 authors = [
     {name = "Francesco Witte", email = "tespy@witte.sh"},
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `tespy-0.7.2.post2/src/tespy/__init__.py` & `tespy-0.7.3/src/tespy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8
 import importlib.resources
 import os
 
 __datapath__ = os.path.join(importlib.resources.files("tespy"), "data")
-__version__ = '0.7.2.post2 - Newton\'s Nature'
+__version__ = '0.7.3 - Newton\'s Nature'
 
 # tespy data and connections import
 from . import connections  # noqa: F401
 from . import data  # noqa: F401
 # tespy components imports
 from .components import basics  # noqa: F401
 from .components import combustion  # noqa: F401
```

### Comparing `tespy-0.7.2.post2/src/tespy/components/__init__.py` & `tespy-0.7.3/src/tespy/components/__init__.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/basics/cycle_closer.py` & `tespy-0.7.3/src/tespy/components/basics/cycle_closer.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/basics/sink.py` & `tespy-0.7.3/src/tespy/components/basics/sink.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/basics/source.py` & `tespy-0.7.3/src/tespy/components/basics/source.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/basics/subsystem_interface.py` & `tespy-0.7.3/src/tespy/components/basics/subsystem_interface.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/combustion/base.py` & `tespy-0.7.3/src/tespy/components/combustion/base.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/combustion/diabatic.py` & `tespy-0.7.3/src/tespy/components/combustion/diabatic.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/combustion/engine.py` & `tespy-0.7.3/src/tespy/components/combustion/engine.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/component.py` & `tespy-0.7.3/src/tespy/components/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from tespy.tools.data_containers import SimpleDataContainer as dc_simple
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import v_mix_ph
 from tespy.tools.global_vars import ERR
 from tespy.tools.helpers import _numeric_deriv
 from tespy.tools.helpers import bus_char_derivative
 from tespy.tools.helpers import bus_char_evaluation
-from tespy.tools.helpers import newton
+from tespy.tools.helpers import newton_with_kwargs
 
 
 class Component:
     r"""
     Class Component is the base class of all TESPy components.
 
     Parameters
@@ -282,21 +282,21 @@
         if key in self.__dict__:
             return self.__dict__[key]
         else:
             msg = f"Component {self.label} has no attribute {key}."
             logger.error(msg)
             raise KeyError(msg)
 
-    def serialize(self):
+    def _serialize(self):
         export = {}
         for k in self._serializable():
             export.update({k: self.get_attr(k)})
         for k in self.parameters:
             data = self.get_attr(k)
-            export.update({k: data.serialize()})
+            export.update({k: data._serialize()})
 
         return {self.label: export}
 
     @staticmethod
     def _serializable():
         return [
             "design", "offdesign", "local_design", "local_offdesign",
@@ -484,18 +484,17 @@
                     self.inl[inconn].p.val_SI, self.inl[inconn].h.val_SI,
                     self.inl[inconn].fluid_data, self.inl[inconn].mixing_rule,
                     T0=self.inl[inconn].T.val_SI
                 )
                 return v / self.inl[inconn].v.design
             elif param == 'pr':
                 return (
-                    (self.outl[outconn].p.val_SI *
-                     self.inl[inconn].p.design) /
-                    (self.inl[inconn].p.val_SI *
-                     self.outl[outconn].p.design))
+                    (self.outl[outconn].p.val_SI * self.inl[inconn].p.design)
+                    / (self.inl[inconn].p.val_SI * self.outl[outconn].p.design)
+                )
             else:
                 msg = (
                     f"The parameter {param}) is not available for "
                     "characteristic function evaluation."
                 )
                 logger.error(msg)
                 raise ValueError(msg)
@@ -638,19 +637,29 @@
         if np.isnan(b['P_ref']) or b['P_ref'] == 0:
             return 1
         else:
             comp_val = self.bus_func(b)
             if b['base'] == 'component':
                 return abs(comp_val / b['P_ref'])
             else:
-                bus_value = newton(
-                    bus_char_evaluation,
-                    bus_char_derivative,
-                    [comp_val, b['P_ref'], b['char']], 0,
-                    val0=b['P_ref'], valmin=-1e15, valmax=1e15)
+                kwargs = {
+                    "function": bus_char_evaluation,
+                    "parameter": "bus_value",
+                    "component_value": comp_val,
+                    "reference_value": b["P_ref"],
+                    "char_func": b["char"]
+                }
+                bus_value = newton_with_kwargs(
+                    derivative=bus_char_derivative,
+                    target_value=0,
+                    val0=b['P_ref'],
+                    valmin=-1e15,
+                    valmax=1e15,
+                    **kwargs
+                )
                 return bus_value / b['P_ref']
 
     def calc_bus_efficiency(self, bus):
         r"""
         Return the busses' efficiency.
 
         Parameters
```

### Comparing `tespy-0.7.2.post2/src/tespy/components/heat_exchangers/base.py` & `tespy-0.7.3/src/tespy/components/heat_exchangers/base.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/heat_exchangers/condenser.py` & `tespy-0.7.3/src/tespy/components/heat_exchangers/condenser.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/heat_exchangers/desuperheater.py` & `tespy-0.7.3/src/tespy/components/heat_exchangers/desuperheater.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/heat_exchangers/parabolic_trough.py` & `tespy-0.7.3/src/tespy/components/heat_exchangers/parabolic_trough.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/heat_exchangers/simple.py` & `tespy-0.7.3/src/tespy/components/heat_exchangers/simple.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/heat_exchangers/solar_collector.py` & `tespy-0.7.3/src/tespy/components/heat_exchangers/solar_collector.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/nodes/base.py` & `tespy-0.7.3/src/tespy/components/nodes/base.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/nodes/droplet_separator.py` & `tespy-0.7.3/src/tespy/components/nodes/droplet_separator.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/nodes/drum.py` & `tespy-0.7.3/src/tespy/components/nodes/drum.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/nodes/merge.py` & `tespy-0.7.3/src/tespy/components/nodes/merge.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/nodes/separator.py` & `tespy-0.7.3/src/tespy/components/nodes/separator.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/nodes/splitter.py` & `tespy-0.7.3/src/tespy/components/nodes/splitter.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/piping/pipe.py` & `tespy-0.7.3/src/tespy/components/piping/pipe.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/piping/valve.py` & `tespy-0.7.3/src/tespy/components/piping/valve.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/reactors/fuel_cell.py` & `tespy-0.7.3/src/tespy/components/reactors/fuel_cell.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/reactors/water_electrolyzer.py` & `tespy-0.7.3/src/tespy/components/reactors/water_electrolyzer.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/subsystem.py` & `tespy-0.7.3/src/tespy/components/subsystem.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/turbomachinery/base.py` & `tespy-0.7.3/src/tespy/components/turbomachinery/base.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/turbomachinery/compressor.py` & `tespy-0.7.3/src/tespy/components/turbomachinery/compressor.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/turbomachinery/pump.py` & `tespy-0.7.3/src/tespy/components/turbomachinery/pump.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/components/turbomachinery/turbine.py` & `tespy-0.7.3/src/tespy/components/turbomachinery/turbine.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/connections/bus.py` & `tespy-0.7.3/src/tespy/connections/bus.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,22 +405,22 @@
                     'of bus.add_comps() for more information.')
                 logger.error(msg)
                 raise TypeError(msg)
 
             msg = f"Added component {comp.label} to bus {self.label}."
             logger.debug(msg)
 
-    def serialize(self):
+    def _serialize(self):
         export = {}
-        export["P"] = self.P.serialize()
+        export["P"] = self.P._serialize()
         for cp in self.comps.index:
             export[cp.label] = {}
             export[cp.label]["param"] = self.comps.loc[cp, "param"]
             export[cp.label]["base"] = self.comps.loc[cp, "base"]
-            export[cp.label]["char"] = self.comps.loc[cp, "char"].serialize()
+            export[cp.label]["char"] = self.comps.loc[cp, "char"]._serialize()
 
         return {self.label: export}
 
     def solve(self):
         self.residual = self.P.val
         for cp in self.comps.index:
             self.residual -= cp.calc_bus_value(self)
```

### Comparing `tespy-0.7.2.post2/src/tespy/connections/connection.py` & `tespy-0.7.3/src/tespy/connections/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -571,25 +571,25 @@
         if key in self.__dict__:
             return self.__dict__[key]
         else:
             msg = 'Connection has no attribute \"' + key + '\".'
             logger.error(msg)
             raise KeyError(msg)
 
-    def serialize(self):
+    def _serialize(self):
         export = {}
         export.update({"source": self.source.label})
         export.update({"target": self.target.label})
         for k in self._serializable():
             export.update({k: self.get_attr(k)})
         for k in self.property_data:
             data = self.get_attr(k)
-            export.update({k: data.serialize()})
+            export.update({k: data._serialize()})
 
-        export.update({"state": self.state.serialize()})
+        export.update({"state": self.state._serialize()})
 
         return {self.label: export}
 
     @staticmethod
     def _serializable():
         return [
             "source_id", "target_id",
```

### Comparing `tespy-0.7.2.post2/src/tespy/data/ChemEx/Ahrendts.json` & `tespy-0.7.3/src/tespy/data/ChemEx/Ahrendts.json`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/data/ChemEx/Szargut1988.json` & `tespy-0.7.3/src/tespy/data/ChemEx/Szargut1988.json`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/data/ChemEx/Szargut2007.json` & `tespy-0.7.3/src/tespy/data/ChemEx/Szargut2007.json`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/data/char_lines.json` & `tespy-0.7.3/src/tespy/data/char_lines.json`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/data/char_maps.json` & `tespy-0.7.3/src/tespy/data/char_maps.json`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/networks/network.py` & `tespy-0.7.3/src/tespy/networks/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,19 +140,19 @@
     >>> nw.add_busses(b)
     >>> b.set_attr(printout=False)
     >>> nw.set_attr(iterinfo=False)
     >>> nw.solve('design')
     >>> nw.print_results()
     """
 
-    def __init__(self, fluids=None, **kwargs):
+    def __init__(self, **kwargs):
         self.set_defaults()
         self.set_attr(**kwargs)
 
-    def serialize(self):
+    def _serialize(self):
         return {
             "m_unit": self.m_unit,
             "m_range": list(self.m_range),
             "p_unit": self.p_unit,
             "p_range": list(self.p_range),
             "h_unit": self.h_unit,
             "h_range": list(self.h_range),
@@ -269,59 +269,54 @@
             'l / h'.
 
         vol_unit : str
             Specify the unit for specific volume: 'm3 / kg', 'l / kg'.
         """
         # unit sets
         for prop in fpd.keys():
-            unit = prop + '_unit'
+            unit = f'{prop}_unit'
             if unit in kwargs:
                 if kwargs[unit] in fpd[prop]['units']:
                     self.__dict__.update({unit: kwargs[unit]})
-                    msg = (
-                        'Setting ' + fpd[prop]['text'] +
-                        ' unit: ' + kwargs[unit] + '.')
+                    msg = f'Setting {fpd[prop]["text"]} unit: {kwargs[unit]}.'
                     logger.debug(msg)
                 else:
                     keys = ', '.join(fpd[prop]['units'].keys())
-                    msg = (
-                        'Allowed units for ' +
-                        fpd[prop]['text'] + ' are: ' + keys)
+                    msg = f'Allowed units for {fpd[prop]["text"]} are: {keys}'
                     logger.error(msg)
                     raise ValueError(msg)
 
         for prop in ['m', 'p', 'h']:
-            if prop + '_range' in kwargs:
-                if isinstance(kwargs[prop + '_range'], list):
-                    self.__dict__.update(
-                        {prop + '_range_SI': hlp.convert_to_SI(
-                            prop, np.array(kwargs[prop + '_range']),
-                            self.get_attr(prop + '_unit'))})
+            if f'{prop}_range' in kwargs:
+                if isinstance(kwargs[f'{prop}_range'], list):
+                    self.__dict__.update({
+                        f'{prop}_range_SI': hlp.convert_to_SI(
+                            prop, np.array(kwargs[f'{prop}_range']),
+                            self.get_attr(f'{prop}_unit')
+                        )
+                    })
                 else:
-                    msg = (
-                        'Specify the value range as list: [' + prop +
-                        '_min, ' + prop + '_max]')
+                    msg = f'Specify the range as list: [{prop}_min, {prop}_max]'
                     logger.error(msg)
                     raise TypeError(msg)
 
-                limits = self.get_attr(prop + '_range_SI')
+                limits = self.get_attr(f'{prop}_range_SI')
                 msg = (
-                    'Setting ' + fpd[prop]['text'] +
-                    ' limits\nmin: ' + str(limits[0]) + ' ' +
-                    fpd[prop]['SI_unit'] + '\n'
-                    'max: ' + str(limits[1]) + ' ' +
-                    fpd[prop]['SI_unit'])
+                    f'Setting {fpd[prop]["text"]} limits\n'
+                    f'min: {limits[0]} {fpd[prop]["SI_unit"]}\n'
+                    f'max: {limits[1]} {fpd[prop]["SI_unit"]}'
+                )
                 logger.debug(msg)
 
         # update non SI value ranges
         for prop in ['m', 'p', 'h']:
             self.__dict__.update({
-                prop + '_range': hlp.convert_from_SI(
-                    prop, self.get_attr(prop + '_range_SI'),
-                    self.get_attr(prop + '_unit')
+                f'{prop}_range': hlp.convert_from_SI(
+                    prop, self.get_attr(f'{prop}_range_SI'),
+                    self.get_attr(f'{prop}_unit')
                 )
             })
 
         self.iterinfo = kwargs.get('iterinfo', self.iterinfo)
 
         if not isinstance(self.iterinfo, bool):
             msg = ('Network parameter iterinfo must be True or False!')
@@ -413,33 +408,36 @@
         ----------
         c : tespy.connections.connection.Connection
             The connection to be added to the network, connections objects ci
             :code:`add_conns(c1, c2, c3, ...)`.
         """
         for c in args:
             if not isinstance(c, con.Connection):
-                msg = ('Must provide tespy.connections.connection.Connection '
-                       'objects as parameters.')
+                msg = (
+                    'Must provide tespy.connections.connection.Connection '
+                    'objects as parameters.'
+                )
                 logger.error(msg)
                 raise TypeError(msg)
 
             elif c.label in self.conns.index:
                 msg = (
-                    'There is already a connection with the label ' +
-                    c.label + '. The connection labels must be unique!')
+                    'There is already a connection with the label '
+                    f'{c.label}. The connection labels must be unique!'
+                )
                 logger.error(msg)
                 raise ValueError(msg)
 
             c.good_starting_values = False
 
             self.conns.loc[c.label] = [
                 c, c.source, c.source_id, c.target, c.target_id
             ]
 
-            msg = 'Added connection ' + c.label + ' to network.'
+            msg = f'Added connection {c.label} to network.'
             logger.debug(msg)
             # set status "checked" to false, if connection is added to network.
             self.checked = False
         self._add_comps(*args)
 
     def del_conns(self, *args):
         """
@@ -454,31 +452,32 @@
         comps = list({cp for c in args for cp in [c.source, c.target]})
         for c in args:
             self.conns.drop(c.label, inplace=True)
             if "Connection" in self.results:
                 self.results["Connection"].drop(
                     c.label, inplace=True, errors="ignore"
                 )
-            msg = ('Deleted connection ' + c.label + ' from network.')
+            msg = f'Deleted connection {c.label} from network.'
             logger.debug(msg)
 
         self._del_comps(comps)
 
         # set status "checked" to false, if connection is deleted from network.
         self.checked = False
 
     def check_conns(self):
         r"""Check connections for multiple usage of inlets or outlets."""
         dub = self.conns.loc[self.conns.duplicated(["source", "source_id"])]
         for c in dub['object']:
             targets = []
-            for conns in self.conns.loc[
-                    (self.conns["source"].values == c.source) &
-                    (self.conns["source_id"].values == c.source_id),
-                    "object"]:
+            mask = (
+                (self.conns["source"].values == c.source)
+                & (self.conns["source_id"].values == c.source_id)
+            )
+            for conns in self.conns.loc[mask, "object"]:
                 targets += [f"\"{conns.target.label}\" ({conns.target_id})"]
             targets = ", ".join(targets)
 
             msg = (
                 f"The source \"{c.source.label}\" ({c.source_id}) is attached "
                 f"to more than one component on the target side: {targets}. "
                 "Please check your network configuration."
@@ -487,18 +486,19 @@
             raise hlp.TESPyNetworkError(msg)
 
         dub = self.conns.loc[
             self.conns.duplicated(['target', 'target_id'])
         ]
         for c in dub['object']:
             sources = []
-            for conns in self.conns.loc[
-                    (self.conns["target"].values == c.target) &
-                    (self.conns["target_id"].values == c.target_id),
-                    "object"]:
+            mask = (
+                (self.conns["target"].values == c.target)
+                & (self.conns["target_id"].values == c.target_id)
+            )
+            for conns in self.conns.loc[mask, "object"]:
                 sources += [f"\"{conns.source.label}\" ({conns.source_id})"]
             sources = ", ".join(sources)
             msg = (
                 f"The target \"{c.target.label}\" ({c.target_id}) is attached "
                 f"to more than one component on the source side: {sources}. "
                 "Please check your network configuration."
             )
@@ -572,24 +572,27 @@
         ----------
         c : tespy.tools.helpers.UserDefinedEquation
             The objects to be added to the network, UserDefinedEquation objects
             ci :code:`add_ude(c1, c2, c3, ...)`.
         """
         for c in args:
             if not isinstance(c, hlp.UserDefinedEquation):
-                msg = ('Must provide tespy.connections.connection.Connection '
-                       'objects as parameters.')
+                msg = (
+                    'Must provide tespy.tools.helpers.UserDefinedEquation '
+                    'objects as parameters.'
+                )
                 logger.error(msg)
                 raise TypeError(msg)
 
             elif c.label in self.user_defined_eq:
                 msg = (
-                    'There is already a UserDefinedEquation with the label ' +
-                    c.label + '. The UserDefinedEquation labels must be '
-                    'unique within a network')
+                    'There is already a UserDefinedEquation with the label '
+                    f'{c.label} . The UserDefinedEquation labels must be '
+                    'unique within a network'
+                )
                 logger.error(msg)
                 raise ValueError(msg)
 
             self.user_defined_eq[c.label] = c
             msg = f"Added UserDefinedEquation {c.label} to network."
             logger.debug(msg)
 
@@ -2704,15 +2707,15 @@
 
         Parameters
         ----------
         fn : str
             Path/filename for the network configuration file.
         """
         with open(fn + 'network.json', 'w') as f:
-            f.write(json.dumps(self.serialize(), indent=4))
+            f.write(json.dumps(self._serialize(), indent=4))
 
         logger.debug('Network information saved to %s.', fn)
 
     def save_connections(self, fn):
         r"""
         Save the connection properties.
 
@@ -2757,34 +2760,34 @@
             with open(fn, "w", encoding="utf-8") as f:
                 f.write(json.dumps(bus_data, indent=4))
             logger.debug('Bus information saved to %s.', fn)
 
     def export_connections(self, fn):
         connections = {}
         for c in self.conns["object"]:
-            connections.update(c.serialize())
+            connections.update(c._serialize())
 
         fn = fn + "connections.json"
         with open(fn, "w", encoding="utf-8") as f:
             f.write(json.dumps(connections, indent=4).replace("NaN", "null"))
         logger.debug('Connection information exported to %s.', fn)
 
     def export_components(self, fn):
         for c in self.comps["comp_type"].unique():
             components = {}
             for cp in self.comps.loc[self.comps["comp_type"] == c, "object"]:
-                components.update(cp.serialize())
+                components.update(cp._serialize())
 
             fname = f"{fn}{c}.json"
             with open(fname, "w", encoding="utf-8") as f:
                 f.write(json.dumps(components, indent=4).replace("NaN", "null"))
             logger.debug('Component information exported to %s.', fname)
 
     def export_busses(self, fn):
         if len(self.busses) > 0:
             busses = {}
             for bus in self.busses.values():
-                busses.update(bus.serialize())
+                busses.update(bus._serialize())
             fn = fn + 'busses.json'
             with open(fn, "w", encoding="utf-8") as f:
                 f.write(json.dumps(busses, indent=4).replace("NaN", "null"))
             logger.debug('Bus information exported to %s.', fn)
```

### Comparing `tespy-0.7.2.post2/src/tespy/networks/network_reader.py` & `tespy-0.7.3/src/tespy/networks/network_reader.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/tools/__init__.py` & `tespy-0.7.3/src/tespy/tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 from .data_containers import ComponentCharacteristics  # noqa: F401
 from .data_containers import ComponentProperties  # noqa: F401
 from .data_containers import FluidComposition  # noqa: F401
 from .data_containers import FluidProperties  # noqa: F401
 from .data_containers import GroupedComponentProperties  # noqa: F401
 from .data_containers import SimpleDataContainer  # noqa: F401
 from .document_models import document_model  # noqa: F401
+from .helpers import UserDefinedEquation  # noqa: F401
 from .optimization import OptimizationProblem  # noqa: F401
```

### Comparing `tespy-0.7.2.post2/src/tespy/tools/analyses.py` & `tespy-0.7.3/src/tespy/tools/analyses.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/tools/characteristics.py` & `tespy-0.7.3/src/tespy/tools/characteristics.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         if key in self.__dict__:
             return self.__dict__[key]
         else:
             msg = 'Char_map has no attribute \"' + key + '\".'
             logger.error(msg)
             raise KeyError(msg)
 
-    def serialize(self):
+    def _serialize(self):
         export = {}
         export["x"] = self.x.tolist()
         export["y"] = self.y.tolist()
         export["extrapolate"] = self.extrapolate
         return export
 
     def plot(self, path, title, xlabel, ylabel):
@@ -443,15 +443,15 @@
         if key in self.__dict__:
             return self.__dict__[key]
         else:
             msg = 'Char_map has no attribute \"' + key + '\".'
             logger.error(msg)
             raise KeyError(msg)
 
-    def serialize(self):
+    def _serialize(self):
         export = {}
         export["x"] = self.x.tolist()
         export["y"] = self.y.tolist()
         export["z"] = self.z.tolist()
         return export
 
     def plot(self, path, title, xlabel, ylabel):
```

### Comparing `tespy-0.7.2.post2/src/tespy/tools/data_containers.py` & `tespy-0.7.3/src/tespy/tools/data_containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         -------
         out : dict
             Dictionary of available attributes (dictionary keys) with default
             values.
         """
         return {}
 
-    def serialize(self):
+    def _serialize(self):
         return {}
 
 
 class ComponentCharacteristics(DataContainer):
     """
     Data container for component characteristics.
 
@@ -195,18 +195,18 @@
         return {
             'char_func': None, 'is_set': False, 'param': None,
             'func_params': {}, 'func': None, 'deriv': None, 'latex': None,
             'char_params': {'type': 'rel', 'inconn': 0, 'outconn': 0},
             'num_eq': 0
         }
 
-    def serialize(self):
+    def _serialize(self):
         export = {}
         if self.char_func is not None:
-            export.update({"char_func": self.char_func.serialize()})
+            export.update({"char_func": self.char_func._serialize()})
 
         for k in ["is_set", "param", "char_params"]:
             export.update({k: self.get_attr(k)})
         return export
 
 
 class ComponentCharacteristicMaps(DataContainer):
@@ -240,18 +240,18 @@
         """
         return {
             'char_func': None, 'is_set': False, 'param': None, 'latex': None,
             'func_params': {}, 'func': None, 'deriv': None,
             'num_eq': 0
         }
 
-    def serialize(self):
+    def _serialize(self):
         export = {}
         if self.char_func is not None:
-            export.update({"char_func": self.char_func.serialize()})
+            export.update({"char_func": self.char_func._serialize()})
 
         for k in ["is_set", "param"]:
             export.update({k: self.get_attr(k)})
         return export
 
 
 class ComponentProperties(DataContainer):
@@ -301,15 +301,15 @@
             'val': 1, 'val_SI': 0, 'is_set': False, 'd': 1e-4,
             'min_val': -1e12, 'max_val': 1e12, 'is_var': False,
             'design': np.nan, 'is_result': False,
             'num_eq': 0, 'func_params': {}, 'func': None, 'deriv': None,
             'latex': None
         }
 
-    def serialize(self):
+    def _serialize(self):
         keys = self._serializable_keys()
         return {k: self.get_attr(k) for k in keys}
 
     @staticmethod
     def _serializable_keys():
         return [
             "val", "val_SI", "is_set", "d", "min_val", "max_val", "is_var",
@@ -359,15 +359,15 @@
             'wrapper': dict(),
             'back_end': dict(),
             'engine': dict(),
             "is_var": set(),
             "J_col": dict(),
         }
 
-    def serialize(self):
+    def _serialize(self):
         export = {"val": self.val}
         export["is_set"] = list(self.is_set)
         export["engine"] = {k: e.__name__ for k, e in self.engine.items()}
         export["back_end"] = {k: b for k, b in self.back_end.items()}
         return export
 
 
@@ -495,15 +495,15 @@
             "latex": None,
             "num_eq": 0,
             "J_col": None,
             "func_params": {},
             "_solved": False
         }
 
-    def serialize(self):
+    def _serialize(self):
         keys = ["val", "val0", "val_SI", "is_set", "unit"]
         return {k: self.get_attr(k) for k in keys}
 
 
 class ReferencedFluidProperties(DataContainer):
 
     @staticmethod
@@ -524,15 +524,15 @@
             "func": None,
             "deriv": None,
             "num_eq": 0,
             "func_params": {},
             "_solved": False
         }
 
-    def serialize(self):
+    def _serialize(self):
         if self.ref is not None:
             keys = ["is_set", "unit"]
             export = {k: self.get_attr(k) for k in keys}
             export["conn"] = self.ref.obj.label
             export["factor"] = self.ref.factor
             export["delta"] = self.ref.delta
             return export
@@ -571,9 +571,9 @@
             "func": None,
             "deriv": None,
             "latex": None,
             "num_eq": 0,
             "_solved": False
         }
 
-    def serialize(self):
+    def _serialize(self):
         return {"val": self.val, "is_set": self.is_set}
```

### Comparing `tespy-0.7.2.post2/src/tespy/tools/document_models.py` & `tespy-0.7.3/src/tespy/tools/document_models.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/tools/fluid_properties/__init__.py` & `tespy-0.7.3/src/tespy/tools/fluid_properties/__init__.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/tools/fluid_properties/functions.py` & `tespy-0.7.3/src/tespy/tools/fluid_properties/functions.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/tools/fluid_properties/helpers.py` & `tespy-0.7.3/src/tespy/tools/fluid_properties/helpers.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/tools/fluid_properties/mixtures.py` & `tespy-0.7.3/src/tespy/tools/fluid_properties/mixtures.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/tools/fluid_properties/wrappers.py` & `tespy-0.7.3/src/tespy/tools/fluid_properties/wrappers.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/tools/global_vars.py` & `tespy-0.7.3/src/tespy/tools/global_vars.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/tools/helpers.py` & `tespy-0.7.3/src/tespy/tools/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         some fluid property functions. We specify fluid property information
         for the inflow and assume that no pressure losses occur in the
         pipeline.
 
         >>> from tespy.components import Source, Sink, Pipe
         >>> from tespy.networks import Network
         >>> from tespy.connections import Connection
-        >>> from tespy.tools.helpers import UserDefinedEquation
+        >>> from tespy.tools import UserDefinedEquation
         >>> from tespy.tools import CharLine
         >>> from tespy.tools.fluid_properties import T_mix_ph, v_mix_ph
         >>> nw = Network(p_unit='bar', T_unit='C')
         >>> nw.set_attr(iterinfo=False)
         >>> so = Source('source')
         >>> si = Sink('sink')
         >>> pipeline = Pipe('pipeline')
@@ -467,15 +467,15 @@
             "p, h or the name of a component variable."
         )
         logger.exception(msg)
         raise ValueError(msg)
     return deriv
 
 
-def bus_char_evaluation(params, bus_value):
+def bus_char_evaluation(component_value, char_func, reference_value, bus_value, **kwargs):
     r"""
     Calculate the value of a bus.
 
     Parameters
     ----------
     comp_value : float
         Value of the energy transfer at the component.
@@ -493,146 +493,44 @@
 
         .. math::
 
             residual = \dot{E}_\mathrm{bus} - \frac{\dot{E}_\mathrm{component}}
             {f\left(\frac{\dot{E}_\mathrm{bus}}
             {\dot{E}_\mathrm{bus,ref}}\right)}
     """
-    comp_value = params[0]
-    reference_value = params[1]
-    char_func = params[2]
-    return bus_value - comp_value / char_func.evaluate(
-        bus_value / reference_value)
+    return bus_value - component_value / char_func.evaluate(
+        bus_value / reference_value
+    )
 
 
-def bus_char_derivative(params, bus_value):
+def bus_char_derivative(component_value, char_func, reference_value, bus_value, **kwargs):
     """Calculate derivative for bus char evaluation."""
-    reference_value = params[1]
-    char_func = params[2]
     d = 1e-3
     return (1 - (
         1 / char_func.evaluate((bus_value + d) / reference_value) -
         1 / char_func.evaluate((bus_value - d) / reference_value)
     ) / (2 * d))
 
 
-def newton(func, deriv, params, y, **kwargs):
-    r"""
-    Find zero crossings with 1-D newton algorithm.
-
-    Parameters
-    ----------
-    func : function
-        Function to find zero crossing in,
-        :math:`0=y-func\left(x,\text{params}\right)`.
-
-    deriv : function
-        First derivative of the function.
-
-    params : list
-        Additional parameters for function, optional.
-
-    y : float
-        Target function value.
-
-    val0 : float
-        Starting value, default: val0=300.
-
-    valmin : float
-        Lower value boundary, default: valmin=70.
-
-    valmax : float
-        Upper value boundary, default: valmax=3000.
-
-    max_iter : int
-        Maximum number of iterations, default: max_iter=10.
-
-    tol_rel : float
-        Maximum relative tolerance :math:`|\frac{y - f(x)}{f(x)}|`, default
-        value: 1e-6.
-
-    tol_abs : float
-        Maximum absolute tolerance :math:`|y - f(x)|`, default value: 1e-6.
-
-    tol_mode : str
-        Check for relative, absolute or both tolerances:
-
-        - :code:`tol_mode='abs'` (default)
-        - :code:`tol_mode='rel'`
-        - :code:`tol_mode='both'`
-
-    Returns
-    -------
-    val : float
-        x-value of zero crossing.
-
-    Note
-    ----
-    Algorithm
-
-    .. math::
-
-        x_{i+1} = x_{i} - \frac{f(x_{i})}{\frac{df}{dx}(x_{i})}\\
-        f(x_{i}) \leq \epsilon
-    """
-    # default valaues
-    x = kwargs.get('val0', 300)
-    valmin = kwargs.get('valmin', 70)
-    valmax = kwargs.get('valmax', 3000)
-    max_iter = kwargs.get('max_iter', 10)
-    tol_rel = kwargs.get('tol_rel', ERR )
-    tol_abs = kwargs.get('tol_abs', ERR )
-    tol_mode = kwargs.get('tol_mode', 'abs')
-
-    # start newton loop
-    expr = True
-    i = 0
-    while expr:
-        # calculate function residual and new value
-        res = y - func(params, x)
-        x += res / deriv(params, x)
-
-        # check for value ranges
-        if x < valmin:
-            x = valmin
-        if x > valmax:
-            x = valmax
-        i += 1
-
-        if i > max_iter:
-            msg = ('Newton algorithm was not able to find a feasible value '
-                   'for function ' + str(func) + '. Current value with x=' +
-                   str(x) + ' is ' + str(func(params, x)) +
-                   ', target value is ' + str(y) + '.')
-            logger.debug(msg)
-
-            break
-        if tol_mode == 'abs' or y == 0:
-            expr = abs(res) >= tol_abs
-        elif tol_mode == 'rel':
-            expr = abs(res / y) >= tol_rel
-        else:
-            expr = abs(res / y) >= tol_rel or abs(res) >= tol_abs
-
-    return x
-
-
 def newton_with_kwargs(
         derivative, target_value, val0=300, valmin=70, valmax=3000, max_iter=10,
-        tol_rel=ERR, tol_abs=ERR, tol_mode="rel", **function_kwargs
+        tol_rel=ERR, tol_abs=ERR ** 2, tol_mode="rel", **function_kwargs
     ):
 
     # start newton loop
     iteration = 0
     expr = True
     x = val0
     parameter = function_kwargs["parameter"]
     function = function_kwargs["function"]
     relax = 1
 
+    if tol_mode == "rel" and abs(target_value) <= 2 * tol_rel:
+        tol_mode = "abs"
+
     while expr:
         # calculate function residual and new value
         function_kwargs[parameter] = x
         residual = target_value - function(**function_kwargs)
         x += residual / derivative(**function_kwargs) * relax
 
         # check for value ranges
```

### Comparing `tespy-0.7.2.post2/src/tespy/tools/logger.py` & `tespy-0.7.3/src/tespy/tools/logger.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/src/tespy/tools/optimization.py` & `tespy-0.7.3/src/tespy/tools/optimization.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_analyses/test_entropy_analysis.py` & `tespy-0.7.3/tests/test_analyses/test_entropy_analysis.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_analyses/test_exergy_analysis.py` & `tespy-0.7.3/tests/test_analyses/test_exergy_analysis.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_busses.py` & `tespy-0.7.3/tests/test_busses.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_components/test_combustion.py` & `tespy-0.7.3/tests/test_components/test_combustion.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_components/test_drum.py` & `tespy-0.7.3/tests/test_components/test_drum.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_components/test_heat_exchangers.py` & `tespy-0.7.3/tests/test_components/test_heat_exchangers.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_components/test_merge.py` & `tespy-0.7.3/tests/test_components/test_merge.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_components/test_piping.py` & `tespy-0.7.3/tests/test_components/test_piping.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_components/test_reactors.py` & `tespy-0.7.3/tests/test_components/test_reactors.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_components/test_turbomachinery.py` & `tespy-0.7.3/tests/test_components/test_turbomachinery.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_connections.py` & `tespy-0.7.3/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_errors.py` & `tespy-0.7.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_models/cgam-ebsilon-results.csv` & `tespy-0.7.3/tests/test_models/cgam-ebsilon-results.csv`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_models/test_CGAM_model.py` & `tespy-0.7.3/tests/test_models/test_CGAM_model.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_models/test_heat_pump_model.py` & `tespy-0.7.3/tests/test_models/test_heat_pump_model.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_models/test_solar_energy_generating_system.py` & `tespy-0.7.3/tests/test_models/test_solar_energy_generating_system.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_networks/test_binary_incompressible.py` & `tespy-0.7.3/tests/test_networks/test_binary_incompressible.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_networks/test_mixing_rules.py` & `tespy-0.7.3/tests/test_networks/test_mixing_rules.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_networks/test_network.py` & `tespy-0.7.3/tests/test_networks/test_network.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_tools/test_characteristics.py` & `tespy-0.7.3/tests/test_tools/test_characteristics.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_tools/test_fluid_properties/test_coolprop.py` & `tespy-0.7.3/tests/test_tools/test_fluid_properties/test_coolprop.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_tools/test_fluid_properties/test_iapws.py` & `tespy-0.7.3/tests/test_tools/test_fluid_properties/test_iapws.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_tools/test_fluid_properties/test_pyromat.py` & `tespy-0.7.3/tests/test_tools/test_fluid_properties/test_pyromat.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tests/test_tools/test_helpers.py` & `tespy-0.7.3/tests/test_tools/test_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-# -*- coding: utf-8
-
-"""Module for testing helper functions.
-
-This file is part of project TESPy (github.com/oemof/tespy). It's copyrighted
-by the contributors recorded in the version control history of the file,
-available from its original location
-tests/test_tools/test_helpers.py
-
-SPDX-License-Identifier: MIT
-"""
-
-from tespy.tools.helpers import newton
-
-
-def func(params, x):
-    return x ** 2 + x - 20
-
-
-def deriv(params, x):
-    return 2 * x + 1
-
-
-def test_newton_bounds():
-    """
-    Test newton algorithm value limit handling.
-
-    Try to calculate a zero crossing of a quadratic function in three
-    tries.
-
-    - zero crossing within limits, starting value near 4
-    - zero crossing within limits, starting value near -5
-
-    - zero crossing below minimum
-    - zero crossing above maximum
-
-    The function is x^2 + x - 20, there crossings are -5 and 4.
-    """
-    result = newton(func, deriv, [], 0, valmin=-10, valmax=10, val0=0)
-    msg = ('The newton algorithm should find the zero crossing at 4.0. ' +
-           str(round(result, 1)) + ' was found instead.')
-    assert 4.0 == result, msg
-
-    result = newton(func, deriv, [], 0, valmin=-10, valmax=10, val0=-10)
-    msg = ('The newton algorithm should find the zero crossing at -5.0. ' +
-           str(round(result, 1)) + ' was found instead.')
-    assert -5.0 == result, msg
-
-    result = newton(func, deriv, [], 0, valmin=-4, valmax=-2, val0=-3)
-    msg = ('The newton algorithm should not be able to find a zero crossing. '
-           'The value ' + str(round(result, 1)) + ' was found, but the '
-           'algorithm should have found the lower boundary of -4.0.')
-    assert -4.0 == result, msg
-
-    result = newton(func, deriv, [], 0, valmin=-20, valmax=-10, val0=-10)
-    msg = ('The newton algorithm should not be able to find a zero crossing. '
-           'The value ' + str(round(result, 1)) + ' was found, but the '
-           'algorithm should have found the upper boundary of -10.0.')
-    assert -10.0 == result, msg
+# -*- coding: utf-8
+
+"""Module for testing helper functions.
+
+This file is part of project TESPy (github.com/oemof/tespy). It's copyrighted
+by the contributors recorded in the version control history of the file,
+available from its original location
+tests/test_tools/test_helpers.py
+
+SPDX-License-Identifier: MIT
+"""
+from pytest import approx
+
+from tespy.tools.helpers import newton_with_kwargs
+
+
+def func(x, **kwargs):
+    return x ** 2 + x - 20
+
+
+def deriv(x, **kwargs):
+    return 2 * x + 1
+
+
+def test_newton_bounds():
+    """
+    Test newton algorithm value limit handling.
+
+    Try to calculate a zero crossing of a quadratic function in three
+    tries.
+
+    - zero crossing within limits, starting value near 4
+    - zero crossing within limits, starting value near -5
+
+    - zero crossing below minimum
+    - zero crossing above maximum
+
+    The function is x^2 + x - 20, there crossings are -5 and 4.
+    """
+    kwargs = {"function": func, "parameter": "x"}
+    result = newton_with_kwargs(deriv, 0, valmin=-10, valmax=10, val0=0, **kwargs)
+    msg = ('The newton algorithm should find the zero crossing at 4.0. ' +
+           str(round(result, 1)) + ' was found instead.')
+    assert 4.0 == approx(result), msg
+
+    result = newton_with_kwargs(deriv, 0, valmin=-10, valmax=10, val0=-10, **kwargs)
+    msg = ('The newton algorithm should find the zero crossing at -5.0. ' +
+           str(round(result, 1)) + ' was found instead.')
+    assert -5.0 == approx(result), msg
+
+    result = newton_with_kwargs(deriv, 0, valmin=-4, valmax=-2, val0=-3, **kwargs)
+    msg = ('The newton algorithm should not be able to find a zero crossing. '
+           'The value ' + str(round(result, 1)) + ' was found, but the '
+           'algorithm should have found the lower boundary of -4.0.')
+    assert -4.0 == approx(result), msg
+
+    result = newton_with_kwargs(deriv, 0, valmin=-20, valmax=-10, val0=-10, **kwargs)
+    msg = ('The newton algorithm should not be able to find a zero crossing. '
+           'The value ' + str(round(result, 1)) + ' was found, but the '
+           'algorithm should have found the upper boundary of -10.0.')
+    assert -10.0 == approx(result), msg
```

### Comparing `tespy-0.7.2.post2/tox.ini` & `tespy-0.7.3/tox.ini`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tutorial/advanced/optimization_example.py` & `tespy-0.7.3/tutorial/advanced/optimization_example.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tutorial/advanced/starting_values.py` & `tespy-0.7.3/tutorial/advanced/starting_values.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tutorial/advanced/stepwise.py` & `tespy-0.7.3/tutorial/advanced/stepwise.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tutorial/basics/district_heating.py` & `tespy-0.7.3/tutorial/basics/district_heating.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tutorial/basics/gas_turbine.py` & `tespy-0.7.3/tutorial/basics/gas_turbine.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tutorial/basics/heat_pump.py` & `tespy-0.7.3/tutorial/basics/heat_pump.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tutorial/basics/rankine.py` & `tespy-0.7.3/tutorial/basics/rankine.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tutorial/heat_pump_exergy/NH3.py` & `tespy-0.7.3/tutorial/heat_pump_exergy/NH3.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tutorial/heat_pump_exergy/NH3_calculations.py` & `tespy-0.7.3/tutorial/heat_pump_exergy/NH3_calculations.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tutorial/heat_pump_exergy/R410A.py` & `tespy-0.7.3/tutorial/heat_pump_exergy/R410A.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tutorial/heat_pump_exergy/R410A_calculations.py` & `tespy-0.7.3/tutorial/heat_pump_exergy/R410A_calculations.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/tutorial/heat_pump_exergy/plots.py` & `tespy-0.7.3/tutorial/heat_pump_exergy/plots.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.2.post2/PKG-INFO` & `tespy-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tespy
-Version: 0.7.2.post2
+Version: 0.7.3
 Summary: Thermal Engineering Systems in Python (TESPy)
 Author-email: Francesco Witte <tespy@witte.sh>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

