# Comparing `tmp/chipscopy-2023.1.dev1676913681.tar.gz` & `tmp/chipscopy-2023.1.dev1677697072.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chipscopy-2023.1.dev1676913681.tar", max compression
+gzip compressed data, was "chipscopy-2023.1.dev1677697072.tar", max compression
```

## Comparing `chipscopy-2023.1.dev1676913681.tar` & `chipscopy-2023.1.dev1677697072.tar`

### file list

```diff
@@ -1,244 +1,244 @@
--rw-r--r--   0        0        0      741 2023-02-22 01:34:30.189179 chipscopy-2023.1.dev1676913681/LICENSE
--rw-r--r--   0        0        0     1908 2023-02-22 01:34:32.645195 chipscopy-2023.1.dev1676913681/README.md
--rw-r--r--   0        0        0     4556 2023-02-22 01:34:30.196209 chipscopy-2023.1.dev1676913681/chipscopy/__init__.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:30.204218 chipscopy-2023.1.dev1676913681/chipscopy/_cli/__init__.py
--rw-r--r--   0        0        0    17027 2023-02-22 01:34:32.650166 chipscopy-2023.1.dev1676913681/chipscopy/_cli/_chipscopy.py
--rw-r--r--   0        0        0     8982 2023-02-22 01:34:30.212202 chipscopy-2023.1.dev1676913681/chipscopy/_cli/example_delivery.py
--rw-r--r--   0        0        0     3731 2023-02-22 01:34:32.653159 chipscopy-2023.1.dev1676913681/chipscopy/api/__init__.py
--rw-r--r--   0        0        0      901 2023-02-22 01:34:30.240150 chipscopy-2023.1.dev1676913681/chipscopy/api/_detail/__init__.py
--rw-r--r--   0        0        0     2773 2023-02-22 01:34:30.252174 chipscopy-2023.1.dev1676913681/chipscopy/api/_detail/debug_core.py
--rw-r--r--   0        0        0    21551 2023-02-22 01:34:32.655177 chipscopy-2023.1.dev1676913681/chipscopy/api/_detail/ltx.py
--rw-r--r--   0        0        0     7456 2023-02-22 01:34:30.258146 chipscopy-2023.1.dev1676913681/chipscopy/api/_detail/property.py
--rw-r--r--   0        0        0      972 2023-02-22 01:34:30.260210 chipscopy-2023.1.dev1676913681/chipscopy/api/_detail/trace.py
--rw-r--r--   0        0        0     6817 2023-02-22 01:34:32.658165 chipscopy-2023.1.dev1676913681/chipscopy/api/cable.py
--rw-r--r--   0        0        0     7371 2023-02-22 01:34:30.296232 chipscopy-2023.1.dev1676913681/chipscopy/api/containers.py
--rw-r--r--   0        0        0      615 2023-02-22 01:34:30.301219 chipscopy-2023.1.dev1676913681/chipscopy/api/ddr/__init__.py
--rw-r--r--   0        0        0    70782 2023-02-22 01:34:32.662146 chipscopy-2023.1.dev1676913681/chipscopy/api/ddr/ddr.py
--rw-r--r--   0        0        0      759 2023-02-22 01:34:32.664190 chipscopy-2023.1.dev1676913681/chipscopy/api/device/__init__.py
--rw-r--r--   0        0        0    37439 2023-02-22 01:34:32.667163 chipscopy-2023.1.dev1676913681/chipscopy/api/device/device.py
--rw-r--r--   0        0        0    15503 2023-02-22 01:34:32.669169 chipscopy-2023.1.dev1676913681/chipscopy/api/device/device_scanner.py
--rw-r--r--   0        0        0    14434 2023-02-22 01:34:32.671185 chipscopy-2023.1.dev1676913681/chipscopy/api/device/device_spec.py
--rw-r--r--   0        0        0     6320 2023-02-22 01:34:32.673193 chipscopy-2023.1.dev1676913681/chipscopy/api/device/device_util.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:30.333224 chipscopy-2023.1.dev1676913681/chipscopy/api/hbm/__init__.py
--rw-r--r--   0        0        0     8772 2023-02-22 01:34:30.336282 chipscopy-2023.1.dev1676913681/chipscopy/api/hbm/hbm.py
--rw-r--r--   0        0        0     3987 2023-02-22 01:34:30.339209 chipscopy-2023.1.dev1676913681/chipscopy/api/hbm/hbmmc.py
--rw-r--r--   0        0        0     1432 2023-02-22 01:34:30.364172 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/__init__.py
--rw-r--r--   0        0        0     5217 2023-02-22 01:34:32.676141 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/aliases.py
--rw-r--r--   0        0        0    16493 2023-02-22 01:34:30.372198 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/eye_scan/__init__.py
--rw-r--r--   0        0        0     4264 2023-02-22 01:34:30.374253 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/eye_scan/manager.py
--rw-r--r--   0        0        0     1143 2023-02-22 01:34:30.378139 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/eye_scan/params.py
--rw-r--r--   0        0        0     9612 2023-02-22 01:34:30.382169 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/eye_scan/plotter.py
--rw-r--r--   0        0        0     3724 2023-02-22 01:34:32.678162 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/gt.py
--rw-r--r--   0        0        0     2980 2023-02-22 01:34:32.682145 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/gt_group.py
--rw-r--r--   0        0        0     3867 2023-02-22 01:34:32.684179 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/ibert.py
--rw-r--r--   0        0        0     7044 2023-02-22 01:34:30.395209 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/link/__init__.py
--rw-r--r--   0        0        0     2725 2023-02-22 01:34:30.412261 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/link/group.py
--rw-r--r--   0        0        0     7265 2023-02-22 01:34:30.432214 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/link/manager.py
--rw-r--r--   0        0        0     2318 2023-02-22 01:34:32.687144 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/pll.py
--rw-r--r--   0        0        0     2863 2023-02-22 01:34:32.688225 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/rx.py
--rw-r--r--   0        0        0    11482 2023-02-22 01:34:32.690214 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/serial_object_base.py
--rw-r--r--   0        0        0     2047 2023-02-22 01:34:32.693151 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/tx.py
--rw-r--r--   0        0        0     4482 2023-02-22 01:34:30.465150 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/yk_scan/__init__.py
--rw-r--r--   0        0        0     3714 2023-02-22 01:34:30.468154 chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/yk_scan/manager.py
--rw-r--r--   0        0        0     1415 2023-02-22 01:34:30.511149 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/__init__.py
--rw-r--r--   0        0        0    31933 2023-02-22 01:34:30.516148 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/ila.py
--rw-r--r--   0        0        0    10817 2023-02-22 01:34:30.519205 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/ila_capture.py
--rw-r--r--   0        0        0    11621 2023-02-22 01:34:30.523154 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/ila_external_trace.py
--rw-r--r--   0        0        0     7825 2023-02-22 01:34:30.526211 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/ila_external_trace_data.py
--rw-r--r--   0        0        0    17198 2023-02-22 01:34:30.531166 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/ila_probe.py
--rw-r--r--   0        0        0    34575 2023-02-22 01:34:30.534229 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/ila_waveform.py
--rw-r--r--   0        0        0    53339 2023-02-22 01:34:30.543223 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ILATsmLexer.py
--rw-r--r--   0        0        0    57471 2023-02-22 01:34:30.550139 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ILATsmParser.py
--rw-r--r--   0        0        0     5215 2023-02-22 01:34:30.555159 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ILATsmVisitor.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:30.558164 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/__init__.py
--rw-r--r--   0        0        0    25728 2023-02-22 01:34:30.560237 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ila_tsm_checker.py
--rw-r--r--   0        0        0     9802 2023-02-22 01:34:30.597156 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ila_tsm_data.py
--rw-r--r--   0        0        0    11380 2023-02-22 01:34:30.599178 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ila_tsm_mapper.py
--rw-r--r--   0        0        0     5792 2023-02-22 01:34:30.602182 chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ila_tsm_reader.py
--rw-r--r--   0        0        0     8774 2023-02-22 01:34:30.631142 chipscopy-2023.1.dev1676913681/chipscopy/api/jtag.py
--rw-r--r--   0        0        0     6102 2023-02-22 01:34:30.633144 chipscopy-2023.1.dev1676913681/chipscopy/api/memory.py
--rw-r--r--   0        0        0      741 2023-02-22 01:34:30.636156 chipscopy-2023.1.dev1676913681/chipscopy/api/noc/__init__.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:30.640140 chipscopy-2023.1.dev1676913681/chipscopy/api/noc/graphing/__init__.py
--rw-r--r--   0        0        0     6295 2023-02-22 01:34:30.669153 chipscopy-2023.1.dev1676913681/chipscopy/api/noc/graphing/hbmmc.py
--rw-r--r--   0        0        0    10922 2023-02-22 01:34:30.741153 chipscopy-2023.1.dev1676913681/chipscopy/api/noc/noc.py
--rw-r--r--   0        0        0    23450 2023-02-22 01:34:30.743144 chipscopy-2023.1.dev1676913681/chipscopy/api/noc/noc_perfmon_utils.py
--rw-r--r--   0        0        0    20203 2023-02-22 01:34:30.745143 chipscopy-2023.1.dev1676913681/chipscopy/api/noc/plotting_utils.py
--rw-r--r--   0        0        0    10732 2023-02-22 01:34:30.839175 chipscopy-2023.1.dev1676913681/chipscopy/api/pcie.py
--rw-r--r--   0        0        0     5577 2023-02-22 01:34:32.695166 chipscopy-2023.1.dev1676913681/chipscopy/api/report.py
--rw-r--r--   0        0        0    18128 2023-02-22 01:34:32.697193 chipscopy-2023.1.dev1676913681/chipscopy/api/session.py
--rw-r--r--   0        0        0     4170 2023-02-22 01:34:30.845148 chipscopy-2023.1.dev1676913681/chipscopy/api/sysmon.py
--rw-r--r--   0        0        0    20222 2023-02-22 01:34:30.847140 chipscopy-2023.1.dev1676913681/chipscopy/api/vio.py
--rw-r--r--   0        0        0     3685 2023-02-22 01:34:30.864157 chipscopy-2023.1.dev1676913681/chipscopy/client/__init__.py
--rw-r--r--   0        0        0     3610 2023-02-22 01:34:30.868149 chipscopy-2023.1.dev1676913681/chipscopy/client/axis_ddr_client.py
--rw-r--r--   0        0        0    31875 2023-02-22 01:34:30.870153 chipscopy-2023.1.dev1676913681/chipscopy/client/axis_ila_core_client.py
--rw-r--r--   0        0        0     2138 2023-02-22 01:34:30.873176 chipscopy-2023.1.dev1676913681/chipscopy/client/axis_pcie_core_client.py
--rw-r--r--   0        0        0     2098 2023-02-22 01:34:30.875160 chipscopy-2023.1.dev1676913681/chipscopy/client/axis_trace_core_client.py
--rw-r--r--   0        0        0    20401 2023-02-22 01:34:30.877146 chipscopy-2023.1.dev1676913681/chipscopy/client/axis_vio_core_client.py
--rw-r--r--   0        0        0     4435 2023-02-22 01:34:30.879142 chipscopy-2023.1.dev1676913681/chipscopy/client/core.py
--rw-r--r--   0        0        0    10760 2023-02-22 01:34:30.880183 chipscopy-2023.1.dev1676913681/chipscopy/client/core_property_client.py
--rw-r--r--   0        0        0     8213 2023-02-22 01:34:30.883144 chipscopy-2023.1.dev1676913681/chipscopy/client/ddrmc_client.py
--rw-r--r--   0        0        0     8335 2023-02-22 01:34:30.884167 chipscopy-2023.1.dev1676913681/chipscopy/client/debug_core_client.py
--rw-r--r--   0        0        0     4238 2023-02-22 01:34:30.887156 chipscopy-2023.1.dev1676913681/chipscopy/client/hbm_client.py
--rw-r--r--   0        0        0     2119 2023-02-22 01:34:30.891139 chipscopy-2023.1.dev1676913681/chipscopy/client/hbm_mc_client.py
--rw-r--r--   0        0        0    27347 2023-02-22 01:34:32.700200 chipscopy-2023.1.dev1676913681/chipscopy/client/ibert_core_client.py
--rw-r--r--   0        0        0    19864 2023-02-22 01:34:30.895186 chipscopy-2023.1.dev1676913681/chipscopy/client/jtagdevice.py
--rw-r--r--   0        0        0     9759 2023-02-22 01:34:30.898158 chipscopy-2023.1.dev1676913681/chipscopy/client/mem.py
--rw-r--r--   0        0        0    18428 2023-02-22 01:34:32.703150 chipscopy-2023.1.dev1676913681/chipscopy/client/mila_core_client.py
--rw-r--r--   0        0        0     9285 2023-02-22 01:34:30.903146 chipscopy-2023.1.dev1676913681/chipscopy/client/noc_perfmon_core_client.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:30.906162 chipscopy-2023.1.dev1676913681/chipscopy/client/node/__init__.py
--rw-r--r--   0        0        0     3301 2023-02-22 01:34:30.909176 chipscopy-2023.1.dev1676913681/chipscopy/client/node/example.py
--rw-r--r--   0        0        0     9398 2023-02-22 01:34:30.950152 chipscopy-2023.1.dev1676913681/chipscopy/client/server_info.py
--rw-r--r--   0        0        0     2909 2023-02-22 01:34:30.953141 chipscopy-2023.1.dev1676913681/chipscopy/client/sysmon_core_client.py
--rw-r--r--   0        0        0     3184 2023-02-22 01:34:30.957156 chipscopy-2023.1.dev1676913681/chipscopy/client/util/__init__.py
--rw-r--r--   0        0        0     5171 2023-02-22 01:34:30.960140 chipscopy-2023.1.dev1676913681/chipscopy/client/util/config.py
--rw-r--r--   0        0        0    13812 2023-02-22 01:34:30.961148 chipscopy-2023.1.dev1676913681/chipscopy/client/view_info.py
--rw-r--r--   0        0        0    18411 2023-02-22 01:34:31.049157 chipscopy-2023.1.dev1676913681/chipscopy/dm/__init__.py
--rw-r--r--   0        0        0     5974 2023-02-22 01:34:31.051152 chipscopy-2023.1.dev1676913681/chipscopy/dm/chipscope.py
--rw-r--r--   0        0        0     6100 2023-02-22 01:34:31.053147 chipscopy-2023.1.dev1676913681/chipscopy/dm/debugcore.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:31.056150 chipscopy-2023.1.dev1676913681/chipscopy/dm/harden/__init__.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:31.059151 chipscopy-2023.1.dev1676913681/chipscopy/dm/harden/noc_perfmon/__init__.py
--rw-r--r--   0        0        0      925 2023-02-22 01:34:31.061169 chipscopy-2023.1.dev1676913681/chipscopy/dm/harden/noc_perfmon/noc_types.py
--rw-r--r--   0        0        0     1124 2023-02-22 01:34:31.063153 chipscopy-2023.1.dev1676913681/chipscopy/dm/harden/noc_perfmon/traffic_classes.py
--rw-r--r--   0        0        0     4944 2023-02-22 01:34:31.065144 chipscopy-2023.1.dev1676913681/chipscopy/dm/jtag.py
--rw-r--r--   0        0        0     7470 2023-02-22 01:34:31.066177 chipscopy-2023.1.dev1676913681/chipscopy/dm/memory.py
--rw-r--r--   0        0        0     8573 2023-02-22 01:34:31.069140 chipscopy-2023.1.dev1676913681/chipscopy/dm/poll.py
--rw-r--r--   0        0        0    23201 2023-02-22 01:34:31.070172 chipscopy-2023.1.dev1676913681/chipscopy/dm/request.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:31.138141 chipscopy-2023.1.dev1676913681/chipscopy/examples/ddr/__init__.py
--rw-r--r--   0        0        0    14150 2023-02-22 01:34:32.706170 chipscopy-2023.1.dev1676913681/chipscopy/examples/ddr/ddr_2d_eye_scan.ipynb
--rw-r--r--   0        0        0     8844 2023-02-22 01:34:31.144144 chipscopy-2023.1.dev1676913681/chipscopy/examples/ddr/ddr_2d_eye_scan.py
--rw-r--r--   0        0        0     9211 2023-02-22 01:34:32.709175 chipscopy-2023.1.dev1676913681/chipscopy/examples/ddr/ddr_example.ipynb
--rw-r--r--   0        0        0     5534 2023-02-22 01:34:31.152141 chipscopy-2023.1.dev1676913681/chipscopy/examples/ddr/ddr_example.py
--rw-r--r--   0        0        0     6885 2023-02-22 01:34:31.153156 chipscopy-2023.1.dev1676913681/chipscopy/examples/ddr/ddr_scan_util.py
--rw-r--r--   0        0        0   285630 2023-02-22 01:34:31.165152 chipscopy-2023.1.dev1676913681/chipscopy/examples/designs/vck190/production/chipscopy_ced/chipscopy_wrapper.ltx
--rw-r--r--   0        0        0  4174096 2023-02-22 01:34:31.201154 chipscopy-2023.1.dev1676913681/chipscopy/examples/designs/vck190/production/chipscopy_ced/chipscopy_wrapper.pdi
--rw-r--r--   0        0        0   285630 2023-02-22 01:34:31.232156 chipscopy-2023.1.dev1676913681/chipscopy/examples/designs/vmk180/production/chipscopy_ced/chipscopy_wrapper.ltx
--rw-r--r--   0        0        0  4186736 2023-02-22 01:34:31.272167 chipscopy-2023.1.dev1676913681/chipscopy/examples/designs/vmk180/production/chipscopy_ced/chipscopy_wrapper.pdi
--rw-r--r--   0        0        0   285630 2023-02-22 01:34:31.281189 chipscopy-2023.1.dev1676913681/chipscopy/examples/designs/vpk120/production/chipscopy_ced/chipscopy_wrapper.ltx
--rw-r--r--   0        0        0  4396576 2023-02-22 01:34:31.318205 chipscopy-2023.1.dev1676913681/chipscopy/examples/designs/vpk120/production/chipscopy_ced/chipscopy_wrapper.pdi
--rw-r--r--   0        0        0    11818 2023-02-22 01:34:32.711191 chipscopy-2023.1.dev1676913681/chipscopy/examples/ibert/versal_gtm/yk_scan_example.ipynb
--rw-r--r--   0        0        0    51894 2023-02-22 01:34:31.345142 chipscopy-2023.1.dev1676913681/chipscopy/examples/ibert/versal_gtm/yk_scan_example.png
--rw-r--r--   0        0        0     7804 2023-02-22 01:34:32.713197 chipscopy-2023.1.dev1676913681/chipscopy/examples/ibert/versal_gtm/yk_scan_example.py
--rw-r--r--   0        0        0    23629 2023-02-22 01:34:32.716177 chipscopy-2023.1.dev1676913681/chipscopy/examples/ibert/versal_gty/link_and_eye_scan.ipynb
--rw-r--r--   0        0        0    16529 2023-02-22 01:34:32.719155 chipscopy-2023.1.dev1676913681/chipscopy/examples/ibert/versal_gty/link_and_eye_scan.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:31.374144 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/__init__.py
--rw-r--r--   0        0        0    16096 2023-02-22 01:34:32.721177 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/ila_advanced_trigger.ipynb
--rw-r--r--   0        0        0     9880 2023-02-22 01:34:31.379189 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/ila_advanced_trigger.py
--rw-r--r--   0        0        0    16011 2023-02-22 01:34:32.724164 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/ila_and_vio.ipynb
--rw-r--r--   0        0        0     9847 2023-02-22 01:34:31.384147 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/ila_and_vio.py
--rw-r--r--   0        0        0    25309 2023-02-22 01:34:32.726188 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/ila_monitor_status.ipynb
--rw-r--r--   0        0        0    17276 2023-02-22 01:34:31.399143 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/ila_monitor_status.py
--rw-r--r--   0        0        0    11738 2023-02-22 01:34:31.402167 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/img/capture_data.png
--rw-r--r--   0        0        0    26920 2023-02-22 01:34:31.405174 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/img/create_session.png
--rw-r--r--   0        0        0    34689 2023-02-22 01:34:31.409163 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/img/edge_trigger.png
--rw-r--r--   0        0        0     9290 2023-02-22 01:34:31.412141 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/img/free_running_counter.png
--rw-r--r--   0        0        0     5394 2023-02-22 01:34:31.415166 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/img/vio_control_counter.png
--rw-r--r--   0        0        0    12951 2023-02-22 01:34:32.729153 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/vio.ipynb
--rw-r--r--   0        0        0     8093 2023-02-22 01:34:31.421144 chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/vio.py
--rw-r--r--   0        0        0    35011 2023-02-22 01:34:31.472161 chipscopy-2023.1.dev1676913681/chipscopy/examples/img/api_overview.png
--rw-r--r--   0        0        0      576 2023-02-22 01:34:31.475211 chipscopy-2023.1.dev1676913681/chipscopy/examples/jtag/__init__.py
--rw-r--r--   0        0        0     9239 2023-02-22 01:34:32.733163 chipscopy-2023.1.dev1676913681/chipscopy/examples/jtag/jtag_example.ipynb
--rw-r--r--   0        0        0     5870 2023-02-22 01:34:31.483139 chipscopy-2023.1.dev1676913681/chipscopy/examples/jtag/jtag_example.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:31.498147 chipscopy-2023.1.dev1676913681/chipscopy/examples/memory/__init__.py
--rw-r--r--   0        0        0    10156 2023-02-22 01:34:32.735168 chipscopy-2023.1.dev1676913681/chipscopy/examples/memory/memory_example.ipynb
--rw-r--r--   0        0        0     6598 2023-02-22 01:34:31.503149 chipscopy-2023.1.dev1676913681/chipscopy/examples/memory/memory_example.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:31.507155 chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/__init__.py
--rw-r--r--   0        0        0    14052 2023-02-22 01:34:32.739151 chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/hbm_perfmon.ipynb
--rw-r--r--   0        0        0     8848 2023-02-22 01:34:31.512144 chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/hbm_perfmon.py
--rw-r--r--   0        0        0    12886 2023-02-22 01:34:32.741163 chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/noc_perfmon.ipynb
--rw-r--r--   0        0        0     8722 2023-02-22 01:34:31.517145 chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/noc_perfmon.py
--rw-r--r--   0        0        0    12582 2023-02-22 01:34:32.744187 chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/noc_perfmon_basic.ipynb
--rw-r--r--   0        0        0     8450 2023-02-22 01:34:32.747147 chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/noc_perfmon_basic.py
--rw-r--r--   0        0        0    14421 2023-02-22 01:34:32.749180 chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/sptg_example.ipynb
--rw-r--r--   0        0        0     9706 2023-02-22 01:34:31.528146 chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/sptg_example.py
--rw-r--r--   0        0        0     5267 2023-02-22 01:34:32.752143 chipscopy-2023.1.dev1676913681/chipscopy/examples/program/program.ipynb
--rw-r--r--   0        0        0     3004 2023-02-22 01:34:31.558164 chipscopy-2023.1.dev1676913681/chipscopy/examples/program/program.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:31.561152 chipscopy-2023.1.dev1676913681/chipscopy/examples/sysmon/__init__.py
--rw-r--r--   0        0        0     8375 2023-02-22 01:34:32.754189 chipscopy-2023.1.dev1676913681/chipscopy/examples/sysmon/sysmon_example.ipynb
--rw-r--r--   0        0        0     5224 2023-02-22 01:34:31.565159 chipscopy-2023.1.dev1676913681/chipscopy/examples/sysmon/sysmon_example.py
--rw-r--r--   0        0        0     2040 2023-02-22 01:34:31.576144 chipscopy-2023.1.dev1676913681/chipscopy/proxies/AxisDDRProxy.py
--rw-r--r--   0        0        0     3584 2023-02-22 01:34:31.578142 chipscopy-2023.1.dev1676913681/chipscopy/proxies/AxisILAProxy.py
--rw-r--r--   0        0        0     1586 2023-02-22 01:34:31.579155 chipscopy-2023.1.dev1676913681/chipscopy/proxies/AxisPCIeProxy.py
--rw-r--r--   0        0        0     1918 2023-02-22 01:34:31.582142 chipscopy-2023.1.dev1676913681/chipscopy/proxies/AxisTraceProxy.py
--rw-r--r--   0        0        0     4722 2023-02-22 01:34:31.584142 chipscopy-2023.1.dev1676913681/chipscopy/proxies/AxisVIOProxy.py
--rw-r--r--   0        0        0     8594 2023-02-22 01:34:31.586146 chipscopy-2023.1.dev1676913681/chipscopy/proxies/ChipScopeProxy.py
--rw-r--r--   0        0        0     1955 2023-02-22 01:34:31.588143 chipscopy-2023.1.dev1676913681/chipscopy/proxies/ContextXvcProxy.py
--rw-r--r--   0        0        0     4951 2023-02-22 01:34:31.590142 chipscopy-2023.1.dev1676913681/chipscopy/proxies/CorePropertyProxy.py
--rw-r--r--   0        0        0     5129 2023-02-22 01:34:31.644149 chipscopy-2023.1.dev1676913681/chipscopy/proxies/DDRMCProxy.py
--rw-r--r--   0        0        0    13766 2023-02-22 01:34:31.646151 chipscopy-2023.1.dev1676913681/chipscopy/proxies/DebugCorePollingProxy.py
--rw-r--r--   0        0        0     7953 2023-02-22 01:34:31.648146 chipscopy-2023.1.dev1676913681/chipscopy/proxies/DebugCoreProxy.py
--rw-r--r--   0        0        0     1817 2023-02-22 01:34:31.649178 chipscopy-2023.1.dev1676913681/chipscopy/proxies/ExampleProxy.py
--rw-r--r--   0        0        0     2910 2023-02-22 01:34:31.651164 chipscopy-2023.1.dev1676913681/chipscopy/proxies/HBMMCProxy.py
--rw-r--r--   0        0        0     3445 2023-02-22 01:34:31.654149 chipscopy-2023.1.dev1676913681/chipscopy/proxies/HBMProxy.py
--rw-r--r--   0        0        0     5435 2023-02-22 01:34:32.758147 chipscopy-2023.1.dev1676913681/chipscopy/proxies/IBERTProxy.py
--rw-r--r--   0        0        0     4595 2023-02-22 01:34:31.659151 chipscopy-2023.1.dev1676913681/chipscopy/proxies/JtagCableProxy.py
--rw-r--r--   0        0        0     1989 2023-02-22 01:34:31.661185 chipscopy-2023.1.dev1676913681/chipscopy/proxies/JtagDeviceProxy.py
--rw-r--r--   0        0        0    11116 2023-02-22 01:34:31.663163 chipscopy-2023.1.dev1676913681/chipscopy/proxies/JtagProxy.py
--rw-r--r--   0        0        0     2020 2023-02-22 01:34:31.665154 chipscopy-2023.1.dev1676913681/chipscopy/proxies/NoCPerfMonProxy.py
--rw-r--r--   0        0        0     3264 2023-02-22 01:34:31.667145 chipscopy-2023.1.dev1676913681/chipscopy/proxies/ProfilerProxy.py
--rw-r--r--   0        0        0     2149 2023-02-22 01:34:32.770144 chipscopy-2023.1.dev1676913681/chipscopy/proxies/RecorderProxy.py
--rw-r--r--   0        0        0     2268 2023-02-22 01:34:31.669141 chipscopy-2023.1.dev1676913681/chipscopy/proxies/SysMonProxy.py
--rw-r--r--   0        0        0     6354 2023-02-22 01:34:31.671141 chipscopy-2023.1.dev1676913681/chipscopy/proxies/XicomProxy.py
--rw-r--r--   0        0        0     1488 2023-02-22 01:34:31.685167 chipscopy-2023.1.dev1676913681/chipscopy/proxies/__init__.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:31.708148 chipscopy-2023.1.dev1676913681/chipscopy/shared/__init__.py
--rw-r--r--   0        0        0     7510 2023-02-22 01:34:31.711154 chipscopy-2023.1.dev1676913681/chipscopy/shared/ila_data.py
--rw-r--r--   0        0        0    21023 2023-02-22 01:34:31.713141 chipscopy-2023.1.dev1676913681/chipscopy/shared/ila_mapper.py
--rw-r--r--   0        0        0     5768 2023-02-22 01:34:31.714164 chipscopy-2023.1.dev1676913681/chipscopy/shared/ila_util.py
--rw-r--r--   0        0        0     3327 2023-02-22 01:34:31.718144 chipscopy-2023.1.dev1676913681/chipscopy/tcf/EventQueue.py
--rw-r--r--   0        0        0     2381 2023-02-22 01:34:31.720140 chipscopy-2023.1.dev1676913681/chipscopy/tcf/__init__.py
--rw-r--r--   0        0        0    34484 2023-02-22 01:34:31.723149 chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/AbstractChannel.py
--rw-r--r--   0        0        0     4928 2023-02-22 01:34:31.725155 chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/ChannelProxy.py
--rw-r--r--   0        0        0     3891 2023-02-22 01:34:31.727155 chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/ChannelTCP.py
--rw-r--r--   0        0        0     4451 2023-02-22 01:34:31.729170 chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/Command.py
--rw-r--r--   0        0        0     3651 2023-02-22 01:34:31.732156 chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/LoopbackChannel.py
--rw-r--r--   0        0        0     4583 2023-02-22 01:34:31.759155 chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/StreamChannel.py
--rw-r--r--   0        0        0     6551 2023-02-22 01:34:31.762157 chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/__init__.py
--rw-r--r--   0        0        0     1410 2023-02-22 01:34:31.813151 chipscopy-2023.1.dev1676913681/chipscopy/tcf/compat.py
--rw-r--r--   0        0        0     6550 2023-02-22 01:34:31.815149 chipscopy-2023.1.dev1676913681/chipscopy/tcf/errors.py
--rw-r--r--   0        0        0    16053 2023-02-22 01:34:31.817144 chipscopy-2023.1.dev1676913681/chipscopy/tcf/peer.py
--rw-r--r--   0        0        0    13600 2023-02-22 01:34:31.819146 chipscopy-2023.1.dev1676913681/chipscopy/tcf/protocol.py
--rw-r--r--   0        0        0    15705 2023-02-22 01:34:31.822165 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/__init__.py
--rwxr-xr-x   0        0        0     4269 2023-02-22 01:34:31.824157 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/arguments.py
--rw-r--r--   0        0        0    43290 2023-02-22 01:34:32.773142 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/local/LocatorService.py
--rw-r--r--   0        0        0     4369 2023-02-22 01:34:31.829146 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/local/TestService.py
--rwxr-xr-x   0        0        0     1237 2023-02-22 01:34:31.831147 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/local/ZeroCopyService.py
--rwxr-xr-x   0        0        0     3781 2023-02-22 01:34:32.775163 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/local/__init__.py
--rw-r--r--   0        0        0     7540 2023-02-22 01:34:31.834176 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/local/default_core_service.py
--rw-r--r--   0        0        0     9152 2023-02-22 01:34:31.836171 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/locator.py
--rw-r--r--   0        0        0    21563 2023-02-22 01:34:31.874150 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/memory.py
--rw-r--r--   0        0        0    40053 2023-02-22 01:34:32.777169 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/mila.py
--rw-r--r--   0        0        0     9163 2023-02-22 01:34:31.881140 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/LocatorProxy.py
--rw-r--r--   0        0        0     4576 2023-02-22 01:34:31.883140 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/MILAProxy.py
--rw-r--r--   0        0        0    10750 2023-02-22 01:34:31.885145 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/MemoryProxy.py
--rw-r--r--   0        0        0     8064 2023-02-22 01:34:31.886168 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/RunControlProxy.py
--rw-r--r--   0        0        0     1295 2023-02-22 01:34:31.971164 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/TestProxy.py
--rw-r--r--   0        0        0     1599 2023-02-22 01:34:31.974155 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/XicomEverestProxy.py
--rwxr-xr-x   0        0        0      479 2023-02-22 01:34:31.976163 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/__init__.py
--rw-r--r--   0        0        0     1149 2023-02-22 01:34:31.978145 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/svfProxy.py
--rw-r--r--   0        0        0    42864 2023-02-22 01:34:31.995149 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/runcontrol.py
--rw-r--r--   0        0        0     1860 2023-02-22 01:34:31.997175 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/svf.py
--rw-r--r--   0        0        0     3222 2023-02-22 01:34:32.000157 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/test.py
--rwxr-xr-x   0        0        0     7149 2023-02-22 01:34:32.002142 chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/xicom.py
--rw-r--r--   0        0        0     3867 2023-02-22 01:34:32.022177 chipscopy-2023.1.dev1676913681/chipscopy/tcf/shell.py
--rw-r--r--   0        0        0    27981 2023-02-22 01:34:32.025173 chipscopy-2023.1.dev1676913681/chipscopy/tcf/tests/BasicTests.py
--rw-r--r--   0        0        0    23525 2023-02-22 01:34:32.027191 chipscopy-2023.1.dev1676913681/chipscopy/tcf/tests/ProcessStart.py
--rwxr-xr-x   0        0        0      479 2023-02-22 01:34:32.030171 chipscopy-2023.1.dev1676913681/chipscopy/tcf/tests/__init__.py
--rw-r--r--   0        0        0     6095 2023-02-22 01:34:32.033182 chipscopy-2023.1.dev1676913681/chipscopy/tcf/transport.py
--rw-r--r--   0        0        0      554 2023-02-22 01:34:32.036172 chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/__init__.py
--rw-r--r--   0        0        0    10373 2023-02-22 01:34:32.038192 chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/cache.py
--rw-r--r--   0        0        0     3251 2023-02-22 01:34:32.041141 chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/event.py
--rw-r--r--   0        0        0     2151 2023-02-22 01:34:32.043157 chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/logging.py
--rwxr-xr-x   0        0        0     2940 2023-02-22 01:34:32.046169 chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/server_discovery.py
--rw-r--r--   0        0        0     9507 2023-02-22 01:34:32.048173 chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/sync.py
--rw-r--r--   0        0        0     6600 2023-02-22 01:34:32.050162 chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/task.py
--rw-r--r--   0        0        0     2938 2023-02-22 01:34:32.054176 chipscopy-2023.1.dev1676913681/chipscopy/utils/__init__.py
--rw-r--r--   0        0        0     5185 2023-02-22 01:34:32.058155 chipscopy-2023.1.dev1676913681/chipscopy/utils/logger/__init__.py
--rw-r--r--   0        0        0      576 2023-02-22 01:34:32.062154 chipscopy-2023.1.dev1676913681/chipscopy/utils/noc_utils/__init__.py
--rw-r--r--   0        0        0     6468 2023-02-22 01:34:32.064200 chipscopy-2023.1.dev1676913681/chipscopy/utils/printer.py
--rw-r--r--   0        0        0     6064 2023-02-22 01:34:32.067179 chipscopy-2023.1.dev1676913681/chipscopy/utils/version.py
--rw-r--r--   0        0        0      739 2023-02-22 01:34:32.780170 chipscopy-2023.1.dev1676913681/chipscopy/vivado_version.py
--rw-r--r--   0        0        0    17431 2023-02-22 01:34:32.783142 chipscopy-2023.1.dev1676913681/chipscopy/xvc/__init__.py
--rw-r--r--   0        0        0    12550 2023-02-22 01:34:32.075172 chipscopy-2023.1.dev1676913681/chipscopy/xvc/reg.py
--rw-r--r--   0        0        0    17300 2023-02-22 01:34:32.548190 chipscopy-2023.1.dev1676913681/epl-v20.html
--rw-r--r--   0        0        0     2853 2023-02-22 01:34:32.790172 chipscopy-2023.1.dev1676913681/pyproject.toml
--rw-r--r--   0        0        0     4856 1970-01-01 00:00:00.000000 chipscopy-2023.1.dev1676913681/setup.py
--rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 chipscopy-2023.1.dev1676913681/PKG-INFO
+-rw-r--r--   0        0        0      741 2023-03-01 19:56:01.014869 chipscopy-2023.1.dev1677697072/LICENSE
+-rw-r--r--   0        0        0     1908 2023-03-01 19:56:02.628869 chipscopy-2023.1.dev1677697072/README.md
+-rw-r--r--   0        0        0     4662 2023-03-01 19:56:02.632863 chipscopy-2023.1.dev1677697072/chipscopy/__init__.py
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:02.634863 chipscopy-2023.1.dev1677697072/chipscopy/_cli/__init__.py
+-rw-r--r--   0        0        0    17195 2023-03-01 19:56:02.636864 chipscopy-2023.1.dev1677697072/chipscopy/_cli/_chipscopy.py
+-rw-r--r--   0        0        0     9048 2023-03-01 19:56:02.637871 chipscopy-2023.1.dev1677697072/chipscopy/_cli/example_delivery.py
+-rw-r--r--   0        0        0     3797 2023-03-01 19:56:02.640862 chipscopy-2023.1.dev1677697072/chipscopy/api/__init__.py
+-rw-r--r--   0        0        0      967 2023-03-01 19:56:02.641869 chipscopy-2023.1.dev1677697072/chipscopy/api/_detail/__init__.py
+-rw-r--r--   0        0        0     2839 2023-03-01 19:56:02.643864 chipscopy-2023.1.dev1677697072/chipscopy/api/_detail/debug_core.py
+-rw-r--r--   0        0        0    21612 2023-03-01 19:56:02.645864 chipscopy-2023.1.dev1677697072/chipscopy/api/_detail/ltx.py
+-rw-r--r--   0        0        0     7522 2023-03-01 19:56:02.646871 chipscopy-2023.1.dev1677697072/chipscopy/api/_detail/property.py
+-rw-r--r--   0        0        0     1038 2023-03-01 19:56:02.648869 chipscopy-2023.1.dev1677697072/chipscopy/api/_detail/trace.py
+-rw-r--r--   0        0        0     6878 2023-03-01 19:56:02.650863 chipscopy-2023.1.dev1677697072/chipscopy/api/cable.py
+-rw-r--r--   0        0        0     7437 2023-03-01 19:56:02.652863 chipscopy-2023.1.dev1677697072/chipscopy/api/containers.py
+-rw-r--r--   0        0        0      676 2023-03-01 19:56:02.653873 chipscopy-2023.1.dev1677697072/chipscopy/api/ddr/__init__.py
+-rw-r--r--   0        0        0    76277 2023-03-01 19:56:02.656868 chipscopy-2023.1.dev1677697072/chipscopy/api/ddr/ddr.py
+-rw-r--r--   0        0        0      774 2023-03-01 19:56:02.657872 chipscopy-2023.1.dev1677697072/chipscopy/api/device/__init__.py
+-rw-r--r--   0        0        0    37454 2023-03-01 19:56:02.660864 chipscopy-2023.1.dev1677697072/chipscopy/api/device/device.py
+-rw-r--r--   0        0        0    15518 2023-03-01 19:56:02.662863 chipscopy-2023.1.dev1677697072/chipscopy/api/device/device_scanner.py
+-rw-r--r--   0        0        0    14449 2023-03-01 19:56:02.663872 chipscopy-2023.1.dev1677697072/chipscopy/api/device/device_spec.py
+-rw-r--r--   0        0        0     6335 2023-03-01 19:56:02.665874 chipscopy-2023.1.dev1677697072/chipscopy/api/device/device_util.py
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:02.667865 chipscopy-2023.1.dev1677697072/chipscopy/api/hbm/__init__.py
+-rw-r--r--   0        0        0     8838 2023-03-01 19:56:02.668876 chipscopy-2023.1.dev1677697072/chipscopy/api/hbm/hbm.py
+-rw-r--r--   0        0        0     4053 2023-03-01 19:56:02.670870 chipscopy-2023.1.dev1677697072/chipscopy/api/hbm/hbmmc.py
+-rw-r--r--   0        0        0     1498 2023-03-01 19:56:02.672871 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/__init__.py
+-rw-r--r--   0        0        0     5283 2023-03-01 19:56:02.674864 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/aliases.py
+-rw-r--r--   0        0        0    16559 2023-03-01 19:56:02.676863 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/eye_scan/__init__.py
+-rw-r--r--   0        0        0     4330 2023-03-01 19:56:02.678863 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/eye_scan/manager.py
+-rw-r--r--   0        0        0     1209 2023-03-01 19:56:02.679869 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/eye_scan/params.py
+-rw-r--r--   0        0        0     9678 2023-03-01 19:56:02.681864 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/eye_scan/plotter.py
+-rw-r--r--   0        0        0     3790 2023-03-01 19:56:02.683864 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/gt.py
+-rw-r--r--   0        0        0     3046 2023-03-01 19:56:02.685863 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/gt_group.py
+-rw-r--r--   0        0        0     3933 2023-03-01 19:56:02.686869 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/ibert.py
+-rw-r--r--   0        0        0     7110 2023-03-01 19:56:02.688866 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/link/__init__.py
+-rw-r--r--   0        0        0     2791 2023-03-01 19:56:02.690864 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/link/group.py
+-rw-r--r--   0        0        0     7331 2023-03-01 19:56:02.692864 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/link/manager.py
+-rw-r--r--   0        0        0     2384 2023-03-01 19:56:02.694864 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/pll.py
+-rw-r--r--   0        0        0     2929 2023-03-01 19:56:02.695871 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/rx.py
+-rw-r--r--   0        0        0    11548 2023-03-01 19:56:02.697868 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/serial_object_base.py
+-rw-r--r--   0        0        0     2113 2023-03-01 19:56:02.699870 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/tx.py
+-rw-r--r--   0        0        0     4548 2023-03-01 19:56:02.701865 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/yk_scan/__init__.py
+-rw-r--r--   0        0        0     3780 2023-03-01 19:56:02.703865 chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/yk_scan/manager.py
+-rw-r--r--   0        0        0     1476 2023-03-01 19:56:02.704871 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/__init__.py
+-rw-r--r--   0        0        0    31994 2023-03-01 19:56:02.707863 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/ila.py
+-rw-r--r--   0        0        0    10883 2023-03-01 19:56:02.709864 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/ila_capture.py
+-rw-r--r--   0        0        0    11682 2023-03-01 19:56:02.710872 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/ila_external_trace.py
+-rw-r--r--   0        0        0     7886 2023-03-01 19:56:02.712872 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/ila_external_trace_data.py
+-rw-r--r--   0        0        0    17264 2023-03-01 19:56:02.714869 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/ila_probe.py
+-rw-r--r--   0        0        0    34641 2023-03-01 19:56:02.717863 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/ila_waveform.py
+-rw-r--r--   0        0        0    53400 2023-03-01 19:56:02.719869 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ILATsmLexer.py
+-rw-r--r--   0        0        0    57532 2023-03-01 19:56:02.722864 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ILATsmParser.py
+-rw-r--r--   0        0        0     5276 2023-03-01 19:56:02.724866 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ILATsmVisitor.py
+-rw-r--r--   0        0        0      637 2023-03-01 19:56:02.726862 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/__init__.py
+-rw-r--r--   0        0        0    25789 2023-03-01 19:56:02.728865 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ila_tsm_checker.py
+-rw-r--r--   0        0        0     9863 2023-03-01 19:56:02.730870 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ila_tsm_data.py
+-rw-r--r--   0        0        0    11441 2023-03-01 19:56:02.731889 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ila_tsm_mapper.py
+-rw-r--r--   0        0        0     5853 2023-03-01 19:56:02.733880 chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ila_tsm_reader.py
+-rw-r--r--   0        0        0     8835 2023-03-01 19:56:02.735884 chipscopy-2023.1.dev1677697072/chipscopy/api/jtag.py
+-rw-r--r--   0        0        0     6168 2023-03-01 19:56:02.737865 chipscopy-2023.1.dev1677697072/chipscopy/api/memory.py
+-rw-r--r--   0        0        0      807 2023-03-01 19:56:02.738886 chipscopy-2023.1.dev1677697072/chipscopy/api/noc/__init__.py
+-rw-r--r--   0        0        0      637 2023-03-01 19:56:02.740869 chipscopy-2023.1.dev1677697072/chipscopy/api/noc/graphing/__init__.py
+-rw-r--r--   0        0        0     6356 2023-03-01 19:56:02.742872 chipscopy-2023.1.dev1677697072/chipscopy/api/noc/graphing/hbmmc.py
+-rw-r--r--   0        0        0    10988 2023-03-01 19:56:02.744871 chipscopy-2023.1.dev1677697072/chipscopy/api/noc/noc.py
+-rw-r--r--   0        0        0    23516 2023-03-01 19:56:02.746870 chipscopy-2023.1.dev1677697072/chipscopy/api/noc/noc_perfmon_utils.py
+-rw-r--r--   0        0        0    20269 2023-03-01 19:56:02.748870 chipscopy-2023.1.dev1677697072/chipscopy/api/noc/plotting_utils.py
+-rw-r--r--   0        0        0    10798 2023-03-01 19:56:02.750868 chipscopy-2023.1.dev1677697072/chipscopy/api/pcie.py
+-rw-r--r--   0        0        0     5643 2023-03-01 19:56:02.752863 chipscopy-2023.1.dev1677697072/chipscopy/api/report.py
+-rw-r--r--   0        0        0    18143 2023-03-01 19:56:02.754867 chipscopy-2023.1.dev1677697072/chipscopy/api/session.py
+-rw-r--r--   0        0        0     4236 2023-03-01 19:56:02.755881 chipscopy-2023.1.dev1677697072/chipscopy/api/sysmon.py
+-rw-r--r--   0        0        0    20288 2023-03-01 19:56:02.757883 chipscopy-2023.1.dev1677697072/chipscopy/api/vio.py
+-rw-r--r--   0        0        0     3751 2023-03-01 19:56:02.759877 chipscopy-2023.1.dev1677697072/chipscopy/client/__init__.py
+-rw-r--r--   0        0        0     3676 2023-03-01 19:56:02.761865 chipscopy-2023.1.dev1677697072/chipscopy/client/axis_ddr_client.py
+-rw-r--r--   0        0        0    31941 2023-03-01 19:56:02.763865 chipscopy-2023.1.dev1677697072/chipscopy/client/axis_ila_core_client.py
+-rw-r--r--   0        0        0     2204 2023-03-01 19:56:02.782877 chipscopy-2023.1.dev1677697072/chipscopy/client/axis_pcie_core_client.py
+-rw-r--r--   0        0        0     2159 2023-03-01 19:56:02.784872 chipscopy-2023.1.dev1677697072/chipscopy/client/axis_trace_core_client.py
+-rw-r--r--   0        0        0    20467 2023-03-01 19:56:02.786889 chipscopy-2023.1.dev1677697072/chipscopy/client/axis_vio_core_client.py
+-rw-r--r--   0        0        0     4501 2023-03-01 19:56:02.788874 chipscopy-2023.1.dev1677697072/chipscopy/client/core.py
+-rw-r--r--   0        0        0    10826 2023-03-01 19:56:02.790869 chipscopy-2023.1.dev1677697072/chipscopy/client/core_property_client.py
+-rw-r--r--   0        0        0     8279 2023-03-01 19:56:02.792869 chipscopy-2023.1.dev1677697072/chipscopy/client/ddrmc_client.py
+-rw-r--r--   0        0        0     8401 2023-03-01 19:56:02.794874 chipscopy-2023.1.dev1677697072/chipscopy/client/debug_core_client.py
+-rw-r--r--   0        0        0     4304 2023-03-01 19:56:02.796881 chipscopy-2023.1.dev1677697072/chipscopy/client/hbm_client.py
+-rw-r--r--   0        0        0     2185 2023-03-01 19:56:02.798881 chipscopy-2023.1.dev1677697072/chipscopy/client/hbm_mc_client.py
+-rw-r--r--   0        0        0    27413 2023-03-01 19:56:02.800885 chipscopy-2023.1.dev1677697072/chipscopy/client/ibert_core_client.py
+-rw-r--r--   0        0        0    19930 2023-03-01 19:56:02.802871 chipscopy-2023.1.dev1677697072/chipscopy/client/jtagdevice.py
+-rw-r--r--   0        0        0     9825 2023-03-01 19:56:02.804873 chipscopy-2023.1.dev1677697072/chipscopy/client/mem.py
+-rw-r--r--   0        0        0    18494 2023-03-01 19:56:02.806867 chipscopy-2023.1.dev1677697072/chipscopy/client/mila_core_client.py
+-rw-r--r--   0        0        0     9351 2023-03-01 19:56:02.808871 chipscopy-2023.1.dev1677697072/chipscopy/client/noc_perfmon_core_client.py
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:02.810865 chipscopy-2023.1.dev1677697072/chipscopy/client/node/__init__.py
+-rw-r--r--   0        0        0     3367 2023-03-01 19:56:02.811893 chipscopy-2023.1.dev1677697072/chipscopy/client/node/example.py
+-rw-r--r--   0        0        0     9464 2023-03-01 19:56:02.825866 chipscopy-2023.1.dev1677697072/chipscopy/client/server_info.py
+-rw-r--r--   0        0        0     2975 2023-03-01 19:56:02.827870 chipscopy-2023.1.dev1677697072/chipscopy/client/sysmon_core_client.py
+-rw-r--r--   0        0        0     3250 2023-03-01 19:56:02.829865 chipscopy-2023.1.dev1677697072/chipscopy/client/util/__init__.py
+-rw-r--r--   0        0        0     5237 2023-03-01 19:56:02.830884 chipscopy-2023.1.dev1677697072/chipscopy/client/util/config.py
+-rw-r--r--   0        0        0    13878 2023-03-01 19:56:02.833866 chipscopy-2023.1.dev1677697072/chipscopy/client/view_info.py
+-rw-r--r--   0        0        0    18477 2023-03-01 19:56:02.835877 chipscopy-2023.1.dev1677697072/chipscopy/dm/__init__.py
+-rw-r--r--   0        0        0     6040 2023-03-01 19:56:02.837867 chipscopy-2023.1.dev1677697072/chipscopy/dm/chipscope.py
+-rw-r--r--   0        0        0     6166 2023-03-01 19:56:02.838891 chipscopy-2023.1.dev1677697072/chipscopy/dm/debugcore.py
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:02.840878 chipscopy-2023.1.dev1677697072/chipscopy/dm/harden/__init__.py
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:02.842868 chipscopy-2023.1.dev1677697072/chipscopy/dm/harden/noc_perfmon/__init__.py
+-rw-r--r--   0        0        0      991 2023-03-01 19:56:02.843877 chipscopy-2023.1.dev1677697072/chipscopy/dm/harden/noc_perfmon/noc_types.py
+-rw-r--r--   0        0        0     1190 2023-03-01 19:56:02.845866 chipscopy-2023.1.dev1677697072/chipscopy/dm/harden/noc_perfmon/traffic_classes.py
+-rw-r--r--   0        0        0     5010 2023-03-01 19:56:02.846891 chipscopy-2023.1.dev1677697072/chipscopy/dm/jtag.py
+-rw-r--r--   0        0        0     7536 2023-03-01 19:56:02.848879 chipscopy-2023.1.dev1677697072/chipscopy/dm/memory.py
+-rw-r--r--   0        0        0     8639 2023-03-01 19:56:02.850872 chipscopy-2023.1.dev1677697072/chipscopy/dm/poll.py
+-rw-r--r--   0        0        0    23267 2023-03-01 19:56:02.852864 chipscopy-2023.1.dev1677697072/chipscopy/dm/request.py
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:02.853884 chipscopy-2023.1.dev1677697072/chipscopy/examples/ddr/__init__.py
+-rw-r--r--   0        0        0    14150 2023-03-01 19:56:02.856870 chipscopy-2023.1.dev1677697072/chipscopy/examples/ddr/ddr_2d_eye_scan.ipynb
+-rw-r--r--   0        0        0     8908 2023-03-01 19:56:02.858874 chipscopy-2023.1.dev1677697072/chipscopy/examples/ddr/ddr_2d_eye_scan.py
+-rw-r--r--   0        0        0     9211 2023-03-01 19:56:02.860881 chipscopy-2023.1.dev1677697072/chipscopy/examples/ddr/ddr_example.ipynb
+-rw-r--r--   0        0        0     5598 2023-03-01 19:56:02.862878 chipscopy-2023.1.dev1677697072/chipscopy/examples/ddr/ddr_example.py
+-rw-r--r--   0        0        0     6951 2023-03-01 19:56:02.870869 chipscopy-2023.1.dev1677697072/chipscopy/examples/ddr/ddr_scan_util.py
+-rw-r--r--   0        0        0   285630 2023-03-01 19:56:01.494882 chipscopy-2023.1.dev1677697072/chipscopy/examples/designs/vck190/production/chipscopy_ced/chipscopy_wrapper.ltx
+-rw-r--r--   0        0        0  4174096 2023-03-01 19:56:01.529902 chipscopy-2023.1.dev1677697072/chipscopy/examples/designs/vck190/production/chipscopy_ced/chipscopy_wrapper.pdi
+-rw-r--r--   0        0        0   285630 2023-03-01 19:56:01.538876 chipscopy-2023.1.dev1677697072/chipscopy/examples/designs/vmk180/production/chipscopy_ced/chipscopy_wrapper.ltx
+-rw-r--r--   0        0        0  4186736 2023-03-01 19:56:01.573892 chipscopy-2023.1.dev1677697072/chipscopy/examples/designs/vmk180/production/chipscopy_ced/chipscopy_wrapper.pdi
+-rw-r--r--   0        0        0   285630 2023-03-01 19:56:01.602874 chipscopy-2023.1.dev1677697072/chipscopy/examples/designs/vpk120/production/chipscopy_ced/chipscopy_wrapper.ltx
+-rw-r--r--   0        0        0  4396576 2023-03-01 19:56:01.639878 chipscopy-2023.1.dev1677697072/chipscopy/examples/designs/vpk120/production/chipscopy_ced/chipscopy_wrapper.pdi
+-rw-r--r--   0        0        0    11818 2023-03-01 19:56:02.872872 chipscopy-2023.1.dev1677697072/chipscopy/examples/ibert/versal_gtm/yk_scan_example.ipynb
+-rw-r--r--   0        0        0    51894 2023-03-01 19:56:01.658863 chipscopy-2023.1.dev1677697072/chipscopy/examples/ibert/versal_gtm/yk_scan_example.png
+-rw-r--r--   0        0        0     7868 2023-03-01 19:56:02.874865 chipscopy-2023.1.dev1677697072/chipscopy/examples/ibert/versal_gtm/yk_scan_example.py
+-rw-r--r--   0        0        0    23629 2023-03-01 19:56:02.877867 chipscopy-2023.1.dev1677697072/chipscopy/examples/ibert/versal_gty/link_and_eye_scan.ipynb
+-rw-r--r--   0        0        0    16593 2023-03-01 19:56:02.879867 chipscopy-2023.1.dev1677697072/chipscopy/examples/ibert/versal_gty/link_and_eye_scan.py
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:02.881863 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/__init__.py
+-rw-r--r--   0        0        0    16096 2023-03-01 19:56:02.883866 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/ila_advanced_trigger.ipynb
+-rw-r--r--   0        0        0     9941 2023-03-01 19:56:02.885864 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/ila_advanced_trigger.py
+-rw-r--r--   0        0        0    16011 2023-03-01 19:56:02.887872 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/ila_and_vio.ipynb
+-rw-r--r--   0        0        0     9911 2023-03-01 19:56:02.889883 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/ila_and_vio.py
+-rw-r--r--   0        0        0    25309 2023-03-01 19:56:02.891882 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/ila_monitor_status.ipynb
+-rw-r--r--   0        0        0    17340 2023-03-01 19:56:02.893879 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/ila_monitor_status.py
+-rw-r--r--   0        0        0    11738 2023-03-01 19:56:01.708862 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/img/capture_data.png
+-rw-r--r--   0        0        0    26920 2023-03-01 19:56:01.709876 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/img/create_session.png
+-rw-r--r--   0        0        0    34689 2023-03-01 19:56:01.711876 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/img/edge_trigger.png
+-rw-r--r--   0        0        0     9290 2023-03-01 19:56:01.713865 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/img/free_running_counter.png
+-rw-r--r--   0        0        0     5394 2023-03-01 19:56:01.714881 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/img/vio_control_counter.png
+-rw-r--r--   0        0        0    12951 2023-03-01 19:56:02.896865 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/vio.ipynb
+-rw-r--r--   0        0        0     8157 2023-03-01 19:56:02.897882 chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/vio.py
+-rw-r--r--   0        0        0    35011 2023-03-01 19:56:01.740862 chipscopy-2023.1.dev1677697072/chipscopy/examples/img/api_overview.png
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:02.899883 chipscopy-2023.1.dev1677697072/chipscopy/examples/jtag/__init__.py
+-rw-r--r--   0        0        0     9239 2023-03-01 19:56:02.903873 chipscopy-2023.1.dev1677697072/chipscopy/examples/jtag/jtag_example.ipynb
+-rw-r--r--   0        0        0     5934 2023-03-01 19:56:02.907868 chipscopy-2023.1.dev1677697072/chipscopy/examples/jtag/jtag_example.py
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:02.909865 chipscopy-2023.1.dev1677697072/chipscopy/examples/memory/__init__.py
+-rw-r--r--   0        0        0    10156 2023-03-01 19:56:02.911874 chipscopy-2023.1.dev1677697072/chipscopy/examples/memory/memory_example.ipynb
+-rw-r--r--   0        0        0     6662 2023-03-01 19:56:02.913874 chipscopy-2023.1.dev1677697072/chipscopy/examples/memory/memory_example.py
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:02.915881 chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/__init__.py
+-rw-r--r--   0        0        0    14052 2023-03-01 19:56:02.917878 chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/hbm_perfmon.ipynb
+-rw-r--r--   0        0        0     8917 2023-03-01 19:56:02.919886 chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/hbm_perfmon.py
+-rw-r--r--   0        0        0    12886 2023-03-01 19:56:02.921883 chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/noc_perfmon.ipynb
+-rw-r--r--   0        0        0     8786 2023-03-01 19:56:02.923872 chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/noc_perfmon.py
+-rw-r--r--   0        0        0    12582 2023-03-01 19:56:02.925865 chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/noc_perfmon_basic.ipynb
+-rw-r--r--   0        0        0     8519 2023-03-01 19:56:02.926890 chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/noc_perfmon_basic.py
+-rw-r--r--   0        0        0    14421 2023-03-01 19:56:02.929864 chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/sptg_example.ipynb
+-rw-r--r--   0        0        0     9770 2023-03-01 19:56:02.930884 chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/sptg_example.py
+-rw-r--r--   0        0        0     5267 2023-03-01 19:56:02.932872 chipscopy-2023.1.dev1677697072/chipscopy/examples/program/program.ipynb
+-rw-r--r--   0        0        0     3068 2023-03-01 19:56:02.934865 chipscopy-2023.1.dev1677697072/chipscopy/examples/program/program.py
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:02.935886 chipscopy-2023.1.dev1677697072/chipscopy/examples/sysmon/__init__.py
+-rw-r--r--   0        0        0     8375 2023-03-01 19:56:02.937878 chipscopy-2023.1.dev1677697072/chipscopy/examples/sysmon/sysmon_example.ipynb
+-rw-r--r--   0        0        0     5288 2023-03-01 19:56:02.939874 chipscopy-2023.1.dev1677697072/chipscopy/examples/sysmon/sysmon_example.py
+-rw-r--r--   0        0        0     2106 2023-03-01 19:56:02.941869 chipscopy-2023.1.dev1677697072/chipscopy/proxies/AxisDDRProxy.py
+-rw-r--r--   0        0        0     3650 2023-03-01 19:56:02.943866 chipscopy-2023.1.dev1677697072/chipscopy/proxies/AxisILAProxy.py
+-rw-r--r--   0        0        0     1652 2023-03-01 19:56:02.945863 chipscopy-2023.1.dev1677697072/chipscopy/proxies/AxisPCIeProxy.py
+-rw-r--r--   0        0        0     1979 2023-03-01 19:56:02.946884 chipscopy-2023.1.dev1677697072/chipscopy/proxies/AxisTraceProxy.py
+-rw-r--r--   0        0        0     4788 2023-03-01 19:56:02.967868 chipscopy-2023.1.dev1677697072/chipscopy/proxies/AxisVIOProxy.py
+-rw-r--r--   0        0        0     8660 2023-03-01 19:56:02.969882 chipscopy-2023.1.dev1677697072/chipscopy/proxies/ChipScopeProxy.py
+-rw-r--r--   0        0        0     2021 2023-03-01 19:56:02.971885 chipscopy-2023.1.dev1677697072/chipscopy/proxies/ContextXvcProxy.py
+-rw-r--r--   0        0        0     5017 2023-03-01 19:56:02.973868 chipscopy-2023.1.dev1677697072/chipscopy/proxies/CorePropertyProxy.py
+-rw-r--r--   0        0        0     5195 2023-03-01 19:56:02.976863 chipscopy-2023.1.dev1677697072/chipscopy/proxies/DDRMCProxy.py
+-rw-r--r--   0        0        0    13832 2023-03-01 19:56:02.977890 chipscopy-2023.1.dev1677697072/chipscopy/proxies/DebugCorePollingProxy.py
+-rw-r--r--   0        0        0     8019 2023-03-01 19:56:02.979878 chipscopy-2023.1.dev1677697072/chipscopy/proxies/DebugCoreProxy.py
+-rw-r--r--   0        0        0     1883 2023-03-01 19:56:02.981876 chipscopy-2023.1.dev1677697072/chipscopy/proxies/ExampleProxy.py
+-rw-r--r--   0        0        0     2976 2023-03-01 19:56:02.983870 chipscopy-2023.1.dev1677697072/chipscopy/proxies/HBMMCProxy.py
+-rw-r--r--   0        0        0     3511 2023-03-01 19:56:02.984887 chipscopy-2023.1.dev1677697072/chipscopy/proxies/HBMProxy.py
+-rw-r--r--   0        0        0     5501 2023-03-01 19:56:02.986887 chipscopy-2023.1.dev1677697072/chipscopy/proxies/IBERTProxy.py
+-rw-r--r--   0        0        0     4661 2023-03-01 19:56:02.988886 chipscopy-2023.1.dev1677697072/chipscopy/proxies/JtagCableProxy.py
+-rw-r--r--   0        0        0     2055 2023-03-01 19:56:02.990866 chipscopy-2023.1.dev1677697072/chipscopy/proxies/JtagDeviceProxy.py
+-rw-r--r--   0        0        0    11182 2023-03-01 19:56:02.992869 chipscopy-2023.1.dev1677697072/chipscopy/proxies/JtagProxy.py
+-rw-r--r--   0        0        0     2086 2023-03-01 19:56:03.018870 chipscopy-2023.1.dev1677697072/chipscopy/proxies/NoCPerfMonProxy.py
+-rw-r--r--   0        0        0     3330 2023-03-01 19:56:03.019890 chipscopy-2023.1.dev1677697072/chipscopy/proxies/ProfilerProxy.py
+-rw-r--r--   0        0        0     2215 2023-03-01 19:56:03.021872 chipscopy-2023.1.dev1677697072/chipscopy/proxies/RecorderProxy.py
+-rw-r--r--   0        0        0     2334 2023-03-01 19:56:03.022900 chipscopy-2023.1.dev1677697072/chipscopy/proxies/SysMonProxy.py
+-rw-r--r--   0        0        0     6420 2023-03-01 19:56:03.024885 chipscopy-2023.1.dev1677697072/chipscopy/proxies/XicomProxy.py
+-rw-r--r--   0        0        0     1554 2023-03-01 19:56:03.026869 chipscopy-2023.1.dev1677697072/chipscopy/proxies/__init__.py
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:03.027893 chipscopy-2023.1.dev1677697072/chipscopy/shared/__init__.py
+-rw-r--r--   0        0        0     7576 2023-03-01 19:56:03.029891 chipscopy-2023.1.dev1677697072/chipscopy/shared/ila_data.py
+-rw-r--r--   0        0        0    21084 2023-03-01 19:56:03.031880 chipscopy-2023.1.dev1677697072/chipscopy/shared/ila_mapper.py
+-rw-r--r--   0        0        0     5834 2023-03-01 19:56:03.033870 chipscopy-2023.1.dev1677697072/chipscopy/shared/ila_util.py
+-rw-r--r--   0        0        0     3327 2023-03-01 19:56:01.940863 chipscopy-2023.1.dev1677697072/chipscopy/tcf/EventQueue.py
+-rw-r--r--   0        0        0     2381 2023-03-01 19:56:01.942864 chipscopy-2023.1.dev1677697072/chipscopy/tcf/__init__.py
+-rw-r--r--   0        0        0    34484 2023-03-01 19:56:01.944871 chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/AbstractChannel.py
+-rw-r--r--   0        0        0     4928 2023-03-01 19:56:01.946870 chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/ChannelProxy.py
+-rw-r--r--   0        0        0     3891 2023-03-01 19:56:01.948868 chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/ChannelTCP.py
+-rw-r--r--   0        0        0     4451 2023-03-01 19:56:01.950865 chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/Command.py
+-rw-r--r--   0        0        0     3713 2023-03-01 19:56:03.035864 chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/LoopbackChannel.py
+-rw-r--r--   0        0        0     4583 2023-03-01 19:56:01.987862 chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/StreamChannel.py
+-rw-r--r--   0        0        0     6551 2023-03-01 19:56:01.988868 chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/__init__.py
+-rw-r--r--   0        0        0     1410 2023-03-01 19:56:01.990863 chipscopy-2023.1.dev1677697072/chipscopy/tcf/compat.py
+-rw-r--r--   0        0        0     6550 2023-03-01 19:56:01.992863 chipscopy-2023.1.dev1677697072/chipscopy/tcf/errors.py
+-rw-r--r--   0        0        0    16053 2023-03-01 19:56:01.994863 chipscopy-2023.1.dev1677697072/chipscopy/tcf/peer.py
+-rw-r--r--   0        0        0    13600 2023-03-01 19:56:01.995868 chipscopy-2023.1.dev1677697072/chipscopy/tcf/protocol.py
+-rw-r--r--   0        0        0    15705 2023-03-01 19:56:01.998867 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/__init__.py
+-rwxr-xr-x   0        0        0     4331 2023-03-01 19:56:03.036886 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/arguments.py
+-rw-r--r--   0        0        0    43352 2023-03-01 19:56:03.039871 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/local/LocatorService.py
+-rw-r--r--   0        0        0     4431 2023-03-01 19:56:03.040888 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/local/TestService.py
+-rwxr-xr-x   0        0        0     1299 2023-03-01 19:56:03.042870 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/local/ZeroCopyService.py
+-rwxr-xr-x   0        0        0     3843 2023-03-01 19:56:03.044868 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/local/__init__.py
+-rw-r--r--   0        0        0     7602 2023-03-01 19:56:03.046867 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/local/default_core_service.py
+-rw-r--r--   0        0        0     9152 2023-03-01 19:56:02.035869 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/locator.py
+-rw-r--r--   0        0        0    21563 2023-03-01 19:56:02.037863 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/memory.py
+-rw-r--r--   0        0        0    40115 2023-03-01 19:56:03.048868 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/mila.py
+-rw-r--r--   0        0        0     9163 2023-03-01 19:56:02.042863 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/LocatorProxy.py
+-rw-r--r--   0        0        0     4638 2023-03-01 19:56:03.050864 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/MILAProxy.py
+-rw-r--r--   0        0        0    10750 2023-03-01 19:56:02.045871 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/MemoryProxy.py
+-rw-r--r--   0        0        0     8064 2023-03-01 19:56:02.068865 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/RunControlProxy.py
+-rw-r--r--   0        0        0     1357 2023-03-01 19:56:03.051876 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/TestProxy.py
+-rw-r--r--   0        0        0     1661 2023-03-01 19:56:03.053865 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/XicomEverestProxy.py
+-rwxr-xr-x   0        0        0      541 2023-03-01 19:56:03.054886 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/__init__.py
+-rw-r--r--   0        0        0     1211 2023-03-01 19:56:03.056875 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/svfProxy.py
+-rw-r--r--   0        0        0    42864 2023-03-01 19:56:02.096865 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/runcontrol.py
+-rw-r--r--   0        0        0     1922 2023-03-01 19:56:03.058864 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/svf.py
+-rw-r--r--   0        0        0     3284 2023-03-01 19:56:03.060871 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/test.py
+-rwxr-xr-x   0        0        0     7211 2023-03-01 19:56:03.062864 chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/xicom.py
+-rw-r--r--   0        0        0     3867 2023-03-01 19:56:02.112867 chipscopy-2023.1.dev1677697072/chipscopy/tcf/shell.py
+-rw-r--r--   0        0        0    27981 2023-03-01 19:56:02.130864 chipscopy-2023.1.dev1677697072/chipscopy/tcf/tests/BasicTests.py
+-rw-r--r--   0        0        0    23525 2023-03-01 19:56:02.132863 chipscopy-2023.1.dev1677697072/chipscopy/tcf/tests/ProcessStart.py
+-rwxr-xr-x   0        0        0      541 2023-03-01 19:56:03.063876 chipscopy-2023.1.dev1677697072/chipscopy/tcf/tests/__init__.py
+-rw-r--r--   0        0        0     6095 2023-03-01 19:56:02.135864 chipscopy-2023.1.dev1677697072/chipscopy/tcf/transport.py
+-rw-r--r--   0        0        0      554 2023-03-01 19:56:02.137871 chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/__init__.py
+-rw-r--r--   0        0        0    10373 2023-03-01 19:56:02.139865 chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/cache.py
+-rw-r--r--   0        0        0     3251 2023-03-01 19:56:02.140871 chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/event.py
+-rw-r--r--   0        0        0     2151 2023-03-01 19:56:02.142871 chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/logging.py
+-rwxr-xr-x   0        0        0     3002 2023-03-01 19:56:03.065867 chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/server_discovery.py
+-rw-r--r--   0        0        0     9507 2023-03-01 19:56:02.146867 chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/sync.py
+-rw-r--r--   0        0        0     6600 2023-03-01 19:56:02.148864 chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/task.py
+-rw-r--r--   0        0        0     3004 2023-03-01 19:56:03.067868 chipscopy-2023.1.dev1677697072/chipscopy/utils/__init__.py
+-rw-r--r--   0        0        0     5251 2023-03-01 19:56:03.068885 chipscopy-2023.1.dev1677697072/chipscopy/utils/logger/__init__.py
+-rw-r--r--   0        0        0      642 2023-03-01 19:56:03.070876 chipscopy-2023.1.dev1677697072/chipscopy/utils/noc_utils/__init__.py
+-rw-r--r--   0        0        0     6534 2023-03-01 19:56:03.072870 chipscopy-2023.1.dev1677697072/chipscopy/utils/printer.py
+-rw-r--r--   0        0        0     6144 2023-03-01 19:56:03.074865 chipscopy-2023.1.dev1677697072/chipscopy/utils/version.py
+-rw-r--r--   0        0        0      805 2023-03-01 19:56:03.075882 chipscopy-2023.1.dev1677697072/chipscopy/vivado_version.py
+-rw-r--r--   0        0        0    17497 2023-03-01 19:56:03.077864 chipscopy-2023.1.dev1677697072/chipscopy/xvc/__init__.py
+-rw-r--r--   0        0        0    12616 2023-03-01 19:56:03.079874 chipscopy-2023.1.dev1677697072/chipscopy/xvc/reg.py
+-rw-r--r--   0        0        0    17300 2023-03-01 19:56:02.535864 chipscopy-2023.1.dev1677697072/epl-v20.html
+-rw-r--r--   0        0        0     2853 2023-03-01 19:56:03.087865 chipscopy-2023.1.dev1677697072/pyproject.toml
+-rw-r--r--   0        0        0     4856 1970-01-01 00:00:00.000000 chipscopy-2023.1.dev1677697072/setup.py
+-rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 chipscopy-2023.1.dev1677697072/PKG-INFO
```

### Comparing `chipscopy-2023.1.dev1676913681/LICENSE` & `chipscopy-2023.1.dev1677697072/LICENSE`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/README.md` & `chipscopy-2023.1.dev1677697072/README.md`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,17 +22,17 @@
 
 # NOTE - Only utility functions that are user visible should be added here to avoid circular imports
 from chipscopy.api import CoreType
 from chipscopy.api.session import create_session, delete_session
 from chipscopy.dm.request import null_callback
 from chipscopy.api.report import report_versions, report_devices, report_hierarchy
 
-__author__ = "Xilinx, Inc."
-__copyright__ = "Copyright 2020, Xilinx, Inc."
-__email__ = "labtools@xilinx.com"
+__author__ = "Advanced Micro Devices, Inc."
+__copyright__ = "Copyright (C) 2022-2023, Advanced Micro Devices, Inc."
+__email__ = "support@xilinx.com"
 try:
     __version__ = importlib_metadata.version(__package__)
 except importlib_metadata.PackageNotFoundError:  # for frozen app support, enter correct version here
     __version__ = "XXXXXXX"
 
 
 def get_examples_dir_or_die():
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/_cli/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/vivado_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+# Vivado version - each time a rel branch is cut, this needs to change
+# expected format is 'YYYY.release' e.g.: '2019.2', '2020.1'
+__vivado_version__ = "2023.2"
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/_cli/_chipscopy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/_cli/_chipscopy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -87,15 +88,16 @@
 # GLOBALS FOR COMMAND LINE MODULE
 _hw_url: str = os.getenv("HW_SERVER_URL", "localhost:3121")
 _cs_url: str = os.getenv("CS_SERVER_URL", "localhost:3042")
 
 
 def display_banner():
     print(f"\n******** Xilinx ChipScoPy v{chipscopy.__version__}")
-    print("  ****** Copyright 2021-2022 Xilinx, Inc. All Rights Reserved.\n")
+    print("  ****** Copyright (C) 2021-2022 Xilinx, Inc. All Rights Reserved.\n")
+    print("  ****** Copyright (C) 2022-2023 Advanced Micro Devices, Inc. All Rights Reserved.\n")
     print("WARNING: Commands and options are subject to change.")
     print()
 
 
 def report(devices, servers):
     session = create_session(hw_server_url=_hw_url, cs_server_url=_cs_url)
     if devices:
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/_cli/example_delivery.py` & `chipscopy-2023.1.dev1677697072/chipscopy/_cli/example_delivery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/_detail/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/_detail/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/_detail/debug_core.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/_detail/debug_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/_detail/ltx.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/_detail/ltx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/_detail/property.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/_detail/property.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/_detail/trace.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/_detail/trace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/cable.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/cable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/containers.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/containers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ddr/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ddr/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ddr/ddr.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ddr/ddr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1256,42 +1257,59 @@
         incr_size = 0
         ddr4_range_one = 60
         ddr4_range_two = 45
         lp4_range_one = 10
         lp4_range_two = 20.4
         ddr4_incr_size = 0.65
         lp4_incr_size = 0.4
+        lp5_base = 10.0
+        lp5_incr_size = 0.5
         read_incr_size = 0.0976563
         prop_list = []
+        # Gen5 Write Vref
+        vref_threshold = 128
 
         prop_list.append("mgchk_rw_mode")
         prop_list.append("mem_type")
-        prop_list.append("mgchk_def_wr_vref_range")
+        if not self.is_gen5:
+            prop_list.append("mgchk_def_wr_vref_range")
+            vref_threshold = 50
 
         results = self.ddr_node.get_property(prop_list)
         rw_mode = results["mgchk_rw_mode"]
         mem_type = results["mem_type"]
-        write_vref_range = results["mgchk_def_wr_vref_range"]
+        if not self.is_gen5:
+            write_vref_range = results["mgchk_def_wr_vref_range"]
 
         if rw_mode:
-            if vref > 50:
-                printer("ERROR: Cannot enter Vref values larger than 50 for Write Margin mode")
+            if vref > vref_threshold:
+                printer(
+                    "ERROR: Cannot enter Vref values larger than ",
+                    vref_threshold,
+                    " for Write Margin mode",
+                )
                 return
             if mem_type == 1:
                 if write_vref_range == 0:
                     base_value = ddr4_range_one
                 else:
                     base_value = ddr4_range_two
                 incr_size = ddr4_incr_size
             elif mem_type == 2:
                 if write_vref_range == 0:
                     base_value = lp4_range_one
                 else:
                     base_value = lp4_range_two
                 incr_size = lp4_incr_size
+            elif mem_type == 5:
+                base_value = lp5_base
+                incr_size = lp5_incr_size
+            elif mem_type == 4:
+                # This needs to be finalized later
+                pass
         else:
             incr_size = read_incr_size
 
         offset_value = vref * incr_size
         output_vref = base_value + offset_value
 
         if not rw_mode:
@@ -1446,35 +1464,116 @@
                 temp_data = {key: val for key, val in data.items() if "rdmargin" not in key}
                 new_data = OrderedDict(sorted(temp_data.items()))
                 data_list.append(new_data)
 
         self.eye_scan_data = data_list
         self.ddr_node.set_property({"es_data_need_update": 0})
 
+    def __update_gen5_eye_scan_data(self):
+        edges = ["left", "right"]
+        clocks = ["nqtr", "pqtr"]
+        clock_defs = {
+            "nqtr": "fall_",
+            "pqtr": "rise_",
+        }
+        data_list = []
+
+        engine_data = self.ddr_node.get_eye_scan_data()
+        data_length = len(engine_data)
+
+        # If initial vref scan went wrong after enabled, needless to process data further
+        if not data_length > 1:
+            return
+
+        scan_mode = engine_data[0]["config.mode"]
+        bit_count = engine_data[0]["config.bits"]
+        byte_count = engine_data[0]["config.bytes"]
+        data_list.append(engine_data[0])
+
+        if "Read" in scan_mode:
+            old_key_base = "rdmargin_"
+            new_key_base = "read_"
+            for data in engine_data[1:]:
+                for bit in range(int(bit_count)):
+                    for clock in clocks:
+                        for edge in edges:
+                            old_key = (
+                                old_key_base + clock + "_" + edge + "_bit" + "{:02d}".format(bit)
+                            )
+                            ps_name = new_key_base + clock_defs[clock] + "{:02d}".format(bit)
+                            new_key = ps_name + "_" + edge
+                            tap_value = data[old_key]
+                            data[new_key] = tap_value
+                            del data[old_key]
+                temp_data = {key: val for key, val in data.items() if "wrmargin" not in key}
+                new_data = OrderedDict(sorted(temp_data.items()))
+                data_list.append(new_data)
+        else:
+            old_key_base = "wrmargin_"
+            new_key_base = "write_"
+            for data in engine_data[1:]:
+                temp_data = {key: val for key, val in data.items() if "rdmargin" not in key}
+                new_data = OrderedDict(sorted(temp_data.items()))
+                data_list.append(new_data)
+
+        self.eye_scan_data = data_list
+        self.ddr_node.set_property({"es_data_need_update": 0})
+
     def __draw_eye_scan_graph(
-        self, margin_data: List, base_name: str, margin_title: str, def_vref: float
+        self,
+        margin_data: List,
+        base_name: str,
+        margin_title: str,
+        def_vref: float,
+        unit_string: str = "",
     ):
         vrefs = []
         left_margs = []
         right_margs = []
         left_ps = []
         right_ps = []
         x_min = 0
         x_max = 0
 
-        for data in margin_data:
-            vrefs.append(float(data["config.vrefp"]))
-            key_name = base_name + "_left"
-            left_margs.append(int(data[key_name]))
-            key_name += "_ps"
-            left_ps.append(int(data[key_name]))
-            key_name = base_name + "_right"
-            right_margs.append(int(data[key_name]))
-            key_name += "_ps"
-            right_ps.append(int(data[key_name]))
+        if not self.is_gen5:
+            for data in margin_data:
+                vrefs.append(float(data["config.vrefp"]))
+                key_name = base_name + "_left"
+                left_margs.append(int(data[key_name]))
+                key_name += "_ps"
+                left_ps.append(int(data[key_name]))
+                key_name = base_name + "_right"
+                right_margs.append(int(data[key_name]))
+                key_name += "_ps"
+                right_ps.append(int(data[key_name]))
+        else:
+            ps_factors = self.ddr_node.get_margin_ps_factors()
+            ps_factor = ps_factors[0]
+
+            if "wrmargin" in base_name:
+                for data in margin_data:
+                    vrefs.append(float(data["config.vrefp"]))
+                    key_name = base_name + "left_lsb_" + unit_string
+                    tap_val = int(data[key_name])
+                    key_name = base_name + "left_msb_" + unit_string
+                    msb_val = int(data[key_name])
+                    left_marg = (msb_val * (2**9)) + tap_val
+                    left_margs.append(left_marg)
+                    ps_val = int(round(left_marg * ps_factor))
+                    left_ps.append(ps_val)
+                    key_name = base_name + "right_lsb_" + unit_string
+                    tap_val = int(data[key_name])
+                    key_name = base_name + "right_msb_" + unit_string
+                    msb_val = int(data[key_name])
+                    right_marg = (msb_val * (2**9)) + tap_val
+                    right_margs.append(right_marg)
+                    ps_val = int(round(right_marg * ps_factor))
+                    right_ps.append(ps_val)
+            else:
+                pass
 
         x_min = max(left_ps)
         x_max = max(right_ps)
 
         data_defs = {
             "VRef": vrefs,
             "Left_Margin": left_margs,
@@ -1565,15 +1664,18 @@
         out_file = None
 
         if not file_name:
             # Gives a default for users
             file_name = "eye_scan_data"
 
         file_name = os.path.splitext(file_name)[0] + ".csv"
-        self.__update_eye_scan_data()
+        if self.is_gen5:
+            self.__update_gen5_eye_scan_data()
+        else:
+            self.__update_eye_scan_data()
 
         if not self.eye_scan_data:
             printer("ERROR: No scan data is found. Please re-run 2D eye scan.")
             return
 
         data_list = self.eye_scan_data
         keys = list(data_list[0].keys())
@@ -1639,19 +1741,32 @@
         results = self.ddr_node.get_property(prop_list)
         rw_mode = results["mgchk_rw_mode"]
         vref_min = results["es_vref_min"]
         vref_max = results["es_vref_max"]
         vref_steps = results["es_vref_steps"]
 
         if rw_mode:
-            if (vref_min > 50) or (vref_max > 50):
-                printer("ERROR: Cannot set Vref values larger than 50 under Write margin mode.")
+            if self.is_gen5:
+                vref_threshold = 128
+            else:
+                vref_threshold = 50
+
+            if (vref_min > vref_threshold) or (vref_max > vref_threshold):
+                printer(
+                    "ERROR: Cannot set Vref values larger than ",
+                    vref_threshold,
+                    " under Write margin mode.",
+                )
                 return False
-            if vref_steps > 51:
-                printer("ERROR: Cannot set Vref step sizes larger than 51 for Write Margin mode")
+            if vref_steps > vref_threshold + 1:
+                printer(
+                    "ERROR: Cannot set Vref step sizes larger than ",
+                    vref_threshold + 1,
+                    " for Write Margin mode",
+                )
                 return False
 
         if vref_min > vref_max:
             printer("ERROR: Cannot set minimum Vref value larger than maximum Vref value.")
             return False
 
         percent_min = self.get_eye_scan_vref_percentage(vref_min)
@@ -1753,15 +1868,18 @@
             )
 
         result = self.ddr_node.get_property(["es_data_need_update"])
         data_need_update = result["es_data_need_update"]
 
         if data_need_update:
             self.eye_scan_data.clear()
-            self.__update_eye_scan_data()
+            if self.is_gen5:
+                self.__update_gen5_eye_scan_data()
+            else:
+                self.__update_eye_scan_data()
 
         if not self.eye_scan_data:
             printer(
                 "ERROR: No scan data is found. Please re-run 2D eye scan, "
                 "or load scan data first from a data file."
             )
             return
@@ -1774,21 +1892,38 @@
         data_list = self.eye_scan_data
         scan_mode = data_list[0]["config.mode"]
         unit_mode = data_list[0]["config.unit"]
         rank_num = data_list[0]["config.rank"]
         mem_type = data_list[0]["config.mem_type"]
         df_vref = data_list[0]["config.df_vrefp"]
         df_vref = float(df_vref)
-        nibble_count = data_list[0]["config.nibbles"]
+        if not self.is_gen5:
+            nibble_count = data_list[0]["config.nibbles"]
+        else:
+            bit_count = data_list[0]["config.bits"]
         byte_count = data_list[0]["config.bytes"]
         unit_val = "{:02d}".format(unit_index)
         data_list = data_list[1:]
+        unit_str = ""
 
         # Some logical data check first on user inputs
-        if unit_mode == "nibble":
+        if unit_mode == "bit":
+            if (unit_index < 0) or (unit_index >= int(bit_count)):
+                max_unit = int(bit_count) - 1
+                err_msg = (
+                    "ERROR: unit_index given for "
+                    + unit_mode
+                    + " mode needs to be between 0 and "
+                    + str(max_unit)
+                )
+                err_msg += ", based on current memory configuration."
+                printer(err_msg)
+                return
+            unit_str = unit_mode + unit_val
+        elif unit_mode == "nibble":
             if (unit_index < 0) or (unit_index >= int(nibble_count)):
                 max_unit = int(nibble_count) - 1
                 err_msg = (
                     "ERROR: unit_index given for "
                     + unit_mode
                     + " mode needs to be between 0 and "
                     + str(max_unit)
@@ -1804,14 +1939,15 @@
                     + unit_mode
                     + " mode needs to be between 0 and "
                     + str(max_unit)
                 )
                 err_msg += ", based on current memory configuration."
                 printer(err_msg)
                 return
+            unit_str = unit_mode + str(unit_index)
 
         mc_name = "MC" + str(self.mc_index)
         mc_name += "(" + self.mc_loc + ")"
 
         if "Read" in scan_mode:
             clocks = ["rise_", "fall_"]
             clock_defs = {
@@ -1829,19 +1965,25 @@
                     + "<br>"
                 )
                 margin_mode += mc_name + " - "
                 margin_mode += mem_type + " - Rank" + str(rank_num)
                 fig = self.__draw_eye_scan_graph(data_list, name_base, margin_mode, df_vref)
                 figure_list.append(fig)
         else:
-            name_base = "write_" + unit_val
             margin_mode = scan_mode + " - " + unit_mode.capitalize() + str(unit_index) + "<br>"
             margin_mode += mc_name + " - "
             margin_mode += mem_type + " - Rank" + str(rank_num)
-            fig = self.__draw_eye_scan_graph(data_list, name_base, margin_mode, df_vref)
+            if not self.is_gen5:
+                name_base = "write_" + unit_val
+                fig = self.__draw_eye_scan_graph(data_list, name_base, margin_mode, df_vref)
+            else:
+                name_base = "wrmargin_"
+                fig = self.__draw_eye_scan_graph(
+                    data_list, name_base, margin_mode, df_vref, unit_str
+                )
             figure_list.append(fig)
 
         if not return_as_list:
             for fig in figure_list:
                 if display_type == "dynamic":
                     fig.show()
                 elif display_type == "static":
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/device/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/noc/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-# Copyright 2021-2022 Xilinx, Inc.
-# Copyright 2023 Advanced Micro Devices, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#
-import dataclasses
-from typing import Optional, TypeVar
 
-from chipscopy.api.device.device import Device, FeatureNotAvailableError
+from chipscopy.dm.harden.noc_perfmon.traffic_classes import TC_BEW, TC_BER
+from chipscopy.api.noc.noc_perfmon_utils import NoCPerfMonNodeListener, PerfTGController
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/device/device.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/device/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright 2021-2022 Xilinx, Inc.
-# Copyright 2023 Advanced Micro Devices, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/device/device_scanner.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/device/device_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright 2021-2022 Xilinx, Inc.
-# Copyright 2023 Advanced Micro Devices, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/device/device_spec.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/device/device_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright 2021-2022 Xilinx, Inc.
-# Copyright 2023 Advanced Micro Devices, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/device/device_util.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/device/device_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
-# Copyright 2023 Advanced Micro Devices, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/hbm/hbm.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/hbm/hbm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/hbm/hbmmc.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/hbm/hbmmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/aliases.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/aliases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/eye_scan/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/eye_scan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/eye_scan/manager.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/eye_scan/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/eye_scan/params.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/eye_scan/params.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/eye_scan/plotter.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/eye_scan/plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/gt.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/gt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/gt_group.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/gt_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/ibert.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/ibert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/link/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/link/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/link/group.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/link/group.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/link/manager.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/link/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/pll.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/pll.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/rx.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/rx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/serial_object_base.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/serial_object_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/tx.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/tx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/yk_scan/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/yk_scan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ibert/yk_scan/manager.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ibert/yk_scan/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/ila.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/ila.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/ila_capture.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/ila_capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/ila_external_trace.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/ila_external_trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/ila_external_trace_data.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/ila_external_trace_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/ila_probe.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/ila_probe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/ila_waveform.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/ila_waveform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ILATsmLexer.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ILATsmLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
 
 
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ILATsmParser.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ILATsmParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
 
 
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ILATsmVisitor.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ILATsmVisitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from antlr4 import *
 
 if __name__ is not None and "." in __name__:
     from .ILATsmParser import ILATsmParser
 else:
     from ILATsmParser import ILATsmParser
 
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ila_tsm_checker.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ila_tsm_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ila_tsm_data.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ila_tsm_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ila_tsm_mapper.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ila_tsm_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/ila/tsm/ila_tsm_reader.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/ila/tsm/ila_tsm_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/jtag.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/jtag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/memory.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/noc/graphing/hbmmc.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/noc/graphing/hbmmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/noc/noc.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/noc/noc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/noc/noc_perfmon_utils.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/noc/noc_perfmon_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/noc/plotting_utils.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/noc/plotting_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/pcie.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/pcie.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/report.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/session.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright 2021-2022 Xilinx, Inc.
-# Copyright 2023 Advanced Micro Devices, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/sysmon.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/sysmon.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/api/vio.py` & `chipscopy-2023.1.dev1677697072/chipscopy/api/vio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/axis_ddr_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/axis_ddr_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/axis_ila_core_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/axis_ila_core_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/axis_pcie_core_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/axis_pcie_core_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/axis_trace_core_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/axis_trace_core_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/axis_vio_core_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/axis_vio_core_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/core.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/core_property_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/core_property_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/ddrmc_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/ddrmc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/debug_core_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/debug_core_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/hbm_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/hbm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/hbm_mc_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/hbm_mc_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/ibert_core_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/ibert_core_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/jtagdevice.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/jtagdevice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/mem.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/mem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/mila_core_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/mila_core_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/noc_perfmon_core_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/noc_perfmon_core_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/node/example.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/node/example.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/server_info.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/server_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/sysmon_core_client.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/sysmon_core_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/util/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/util/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/util/config.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/util/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/client/view_info.py` & `chipscopy-2023.1.dev1677697072/chipscopy/client/view_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/dm/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/dm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/dm/chipscope.py` & `chipscopy-2023.1.dev1677697072/chipscopy/dm/chipscope.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/dm/debugcore.py` & `chipscopy-2023.1.dev1677697072/chipscopy/dm/debugcore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/dm/harden/noc_perfmon/noc_types.py` & `chipscopy-2023.1.dev1677697072/chipscopy/dm/harden/noc_perfmon/noc_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/dm/harden/noc_perfmon/traffic_classes.py` & `chipscopy-2023.1.dev1677697072/chipscopy/dm/harden/noc_perfmon/traffic_classes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/dm/jtag.py` & `chipscopy-2023.1.dev1677697072/chipscopy/dm/jtag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/dm/memory.py` & `chipscopy-2023.1.dev1677697072/chipscopy/dm/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/dm/poll.py` & `chipscopy-2023.1.dev1677697072/chipscopy/dm/poll.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/dm/request.py` & `chipscopy-2023.1.dev1677697072/chipscopy/dm/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ddr/ddr_2d_eye_scan.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ddr/ddr_2d_eye_scan.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ddr/ddr_2d_eye_scan.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ddr/ddr_2d_eye_scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2021-2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 # --- # jupyter: # jupytext: # text_representation: # extension: .py #
 format_name: percent # format_version: '1.3' # jupytext_version: 1.10.1 #
 kernelspec: # display_name: Python 3 (ipykernel) # language: python # name:
 python3 # --- # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2021-2022 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced
+Micro Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ddr/ddr_example.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ddr/ddr_example.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ddr/ddr_example.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ddr/ddr_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2021-2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2021-2022 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced
+Micro Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ddr/ddr_scan_util.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ddr/ddr_scan_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/designs/vck190/production/chipscopy_ced/chipscopy_wrapper.ltx` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/designs/vck190/production/chipscopy_ced/chipscopy_wrapper.ltx`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/designs/vck190/production/chipscopy_ced/chipscopy_wrapper.pdi` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/designs/vck190/production/chipscopy_ced/chipscopy_wrapper.pdi`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/designs/vmk180/production/chipscopy_ced/chipscopy_wrapper.ltx` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/designs/vmk180/production/chipscopy_ced/chipscopy_wrapper.ltx`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/designs/vmk180/production/chipscopy_ced/chipscopy_wrapper.pdi` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/designs/vmk180/production/chipscopy_ced/chipscopy_wrapper.pdi`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/designs/vpk120/production/chipscopy_ced/chipscopy_wrapper.ltx` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/designs/vpk120/production/chipscopy_ced/chipscopy_wrapper.ltx`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/designs/vpk120/production/chipscopy_ced/chipscopy_wrapper.pdi` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/designs/vpk120/production/chipscopy_ced/chipscopy_wrapper.pdi`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ibert/versal_gtm/yk_scan_example.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ibert/versal_gtm/yk_scan_example.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ibert/versal_gtm/yk_scan_example.png` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ibert/versal_gtm/yk_scan_example.png`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ibert/versal_gtm/yk_scan_example.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ibert/versal_gtm/yk_scan_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ibert/versal_gty/link_and_eye_scan.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ibert/versal_gty/link_and_eye_scan.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ibert/versal_gty/link_and_eye_scan.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ibert/versal_gty/link_and_eye_scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2021-2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 # --- # jupyter: # jupytext: # formats: ipynb,py:percent # text_representation:
 # extension: .py # format_name: percent # format_version: '1.3' #
 jupytext_version: 1.10.1 # kernelspec: # display_name: Python 3 # language:
 python # name: python3 # --- # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2021-2022 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced
+Micro Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/ila_advanced_trigger.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/ila_advanced_trigger.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/ila_advanced_trigger.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/ila_advanced_trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # %%
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/ila_and_vio.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/ila_and_vio.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/ila_and_vio.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/ila_and_vio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced Micro
+Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/ila_monitor_status.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/ila_monitor_status.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/ila_monitor_status.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/ila_monitor_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced Micro
+Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/img/capture_data.png` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/img/capture_data.png`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/img/create_session.png` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/img/create_session.png`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/img/edge_trigger.png` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/img/edge_trigger.png`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/img/free_running_counter.png` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/img/free_running_counter.png`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/img/vio_control_counter.png` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/img/vio_control_counter.png`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/vio.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/vio.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/ila_and_vio/vio.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/ila_and_vio/vio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced Micro
+Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/img/api_overview.png` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/img/api_overview.png`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/jtag/jtag_example.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/jtag/jtag_example.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990234375%*

 * *Differences: {"'cells'": "{0: {'id': '3f157599'}}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "9c0025d3",
+            "id": "3f157599",
             "metadata": {
                 "collapsed": false
             },
             "source": [
                 "<link rel=\"preconnect\" href=\"https://fonts.gstatic.com\">\n",
                 "<link href=\"https://fonts.googleapis.com/css2?family=Fira+Code&display=swap\" rel=\"stylesheet\">\n",
                 "\n",
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/jtag/jtag_example.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/jtag/jtag_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced Micro
+Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/memory/memory_example.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/memory/memory_example.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/memory/memory_example.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/memory/memory_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2021-2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2021-2022 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced
+Micro Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/hbm_perfmon.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/hbm_perfmon.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/hbm_perfmon.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/hbm_perfmon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 # 
 # ### License
 # 
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2021 Xilinx, Inc.<br><br>
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced
+Micro Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/noc_perfmon.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/noc_perfmon.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/noc_perfmon.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/noc_perfmon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2021-2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2021-2022 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced
+Micro Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/noc_perfmon_basic.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/noc_perfmon_basic.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/noc_perfmon_basic.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/noc_perfmon_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2021 Xilinx, Inc.<br><br>
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced
+Micro Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/sptg_example.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/sptg_example.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/noc_perfmon/sptg_example.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/noc_perfmon/sptg_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2021-2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2021-2022 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced
+Micro Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/program/program.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/program/program.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/program/program.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/program/program.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2021-2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 # %% [markdown] #
  #
  # # ### License # #
-# Copyright 2021-2022 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc. # Copyright (C) 2022-2023, Advanced
+Micro Devices, Inc. #
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 
 # You may obtain a copy of the License at >http://www.apache.org/licenses/
 LICENSE-2.0
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/sysmon/sysmon_example.ipynb` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/sysmon/sysmon_example.ipynb`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/examples/sysmon/sysmon_example.py` & `chipscopy-2023.1.dev1677697072/chipscopy/examples/sysmon/sysmon_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% [markdown]
 # <link rel="preconnect" href="https://fonts.gstatic.com">
 # <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
 #
 # ### License
 #
 # <p style="font-family: 'Fira Code', monospace; font-size: 1.2rem">
-# Copyright 2021-2022 Xilinx, Inc.<br><br>
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
+# <br><br>
 # Licensed under the Apache License, Version 2.0 (the "License");<br>
 # you may not use this file except in compliance with the License.<br><br>
 # You may obtain a copy of the License at <a href="http://www.apache.org/licenses/LICENSE-2.0"?>http://www.apache.org/licenses/LICENSE-2.0</a><br><br>
 # Unless required by applicable law or agreed to in writing, software<br>
 # distributed under the License is distributed on an "AS IS" BASIS,<br>
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.<br>
 # See the License for the specific language governing permissions and<br>
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/AxisDDRProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/AxisDDRProxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/AxisILAProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/AxisILAProxy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/AxisPCIeProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/AxisPCIeProxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/AxisTraceProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/AxisTraceProxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/AxisVIOProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/AxisVIOProxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/ChipScopeProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/ChipScopeProxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/ContextXvcProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/ContextXvcProxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/CorePropertyProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/CorePropertyProxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/DDRMCProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/DDRMCProxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/DebugCorePollingProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/DebugCorePollingProxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/DebugCoreProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/DebugCoreProxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/ExampleProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/ExampleProxy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/HBMMCProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/HBMMCProxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/HBMProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/HBMProxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/IBERTProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/IBERTProxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/JtagCableProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/JtagCableProxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/JtagDeviceProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/JtagDeviceProxy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/JtagProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/JtagProxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/NoCPerfMonProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/NoCPerfMonProxy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/ProfilerProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/ProfilerProxy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/RecorderProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/RecorderProxy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/SysMonProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/SysMonProxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/XicomProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/XicomProxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/proxies/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/proxies/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/shared/ila_data.py` & `chipscopy-2023.1.dev1677697072/chipscopy/shared/ila_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/shared/ila_mapper.py` & `chipscopy-2023.1.dev1677697072/chipscopy/shared/ila_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2022 Xilinx, Inc.
+# Copyright (C) 2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/shared/ila_util.py` & `chipscopy-2023.1.dev1677697072/chipscopy/shared/ila_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/EventQueue.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/EventQueue.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/__init__.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/AbstractChannel.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/AbstractChannel.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/ChannelProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/ChannelProxy.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/ChannelTCP.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/ChannelTCP.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/Command.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/Command.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/LoopbackChannel.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/LoopbackChannel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/StreamChannel.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/StreamChannel.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/channel/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/compat.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/compat.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/errors.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/errors.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/peer.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/peer.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/protocol.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/protocol.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/__init__.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/arguments.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/local/LocatorService.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/local/LocatorService.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
 # * Copyright (c) 2011, 2016 Wind River Systems, Inc. and others.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Wind River Systems - initial API and implementation
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/local/TestService.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/local/TestService.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/local/ZeroCopyService.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/local/ZeroCopyService.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/local/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/local/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
 # * Copyright (c) 2011, 2013 Wind River Systems, Inc. and others.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Wind River Systems - initial API and implementation
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/local/default_core_service.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/local/default_core_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/locator.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/locator.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/memory.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/memory.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/mila.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/mila.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/LocatorProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/LocatorProxy.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/MILAProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/MILAProxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/MemoryProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/MemoryProxy.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/RunControlProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/RunControlProxy.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/TestProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/TestProxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/XicomEverestProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/XicomEverestProxy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/remote/svfProxy.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/remote/svfProxy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/runcontrol.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/runcontrol.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/svf.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/svf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/test.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/services/xicom.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/services/xicom.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/shell.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/shell.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/tests/BasicTests.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/tests/BasicTests.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/tests/ProcessStart.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/tests/ProcessStart.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/transport.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/transport.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/__init__.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/cache.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/cache.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/event.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/event.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/logging.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/logging.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/server_discovery.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/server_discovery.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # *****************************************************************************
-# * Copyright (c) 2020 Xilinx, Inc.
+# * Copyright(C) 2020-2022 Xilinx, Inc.
+# * Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 # * All rights reserved. This program and the accompanying materials
 # * are made available under the terms of the Eclipse Public License 2.0
 # * which accompanies this distribution, and is available at
 # * https://www.eclipse.org/legal/epl-2.0/
 # *
 # * Contributors:
 # *     Xilinx
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/sync.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/sync.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/tcf/util/task.py` & `chipscopy-2023.1.dev1677697072/chipscopy/tcf/util/task.py`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/utils/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/utils/logger/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/utils/logger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/utils/printer.py` & `chipscopy-2023.1.dev1677697072/chipscopy/utils/printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/utils/version.py` & `chipscopy-2023.1.dev1677697072/chipscopy/utils/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -118,29 +119,30 @@
     """
     mismatch_detected = False
     chipscopy_version = VersionDetails(__vivado_version__)
     hw_server_version = VersionDetails(ServerVersionInfo(hw_server, "hw_server").version)
 
     # First compare chipscopy and hw_server
     if (
-        chipscopy_version.year != hw_server_version.year
-        or chipscopy_version.major != hw_server_version.major
+        chipscopy_version.year
+        != hw_server_version.year
+        # or chipscopy_version.major != hw_server_version.major
     ):
         mismatch_detected = True
 
     cs_server_version = None
     if cs_server:
         cs_server_version = VersionDetails(ServerVersionInfo(cs_server, "cs_server").version)
 
         # Next compare cs_server with chipscopy and hw_server
         if (
             chipscopy_version.year != cs_server_version.year
-            or chipscopy_version.major != cs_server_version.major
+            # or chipscopy_version.major != cs_server_version.major
             or hw_server_version.year != cs_server_version.year
-            or hw_server_version.major != cs_server_version.major
+            # or hw_server_version.major != cs_server_version.major
         ):
             mismatch_detected = True
 
     if mismatch_detected:
         msg = (
             "A client/server version mismatch was detected while connecting!"
             f"\n   ChipScoPy client version - {chipscopy_version}"
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/xvc/__init__.py` & `chipscopy-2023.1.dev1677697072/chipscopy/xvc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/chipscopy/xvc/reg.py` & `chipscopy-2023.1.dev1677697072/chipscopy/xvc/reg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2021 Xilinx, Inc.
+# Copyright (C) 2021-2022, Xilinx, Inc.
+# Copyright (C) 2022-2023, Advanced Micro Devices, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `chipscopy-2023.1.dev1676913681/epl-v20.html` & `chipscopy-2023.1.dev1677697072/epl-v20.html`

 * *Files identical despite different names*

### Comparing `chipscopy-2023.1.dev1676913681/pyproject.toml` & `chipscopy-2023.1.dev1677697072/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool.poetry]
 name = "chipscopy"
-version = "2023.1.dev1676913681"
+version = "2023.1.dev1677697072"
 description = "Open-source project from Xilinx® that enables high-level control of Versal debug IP running in hardware"
 authors = ["Xilinx ChipScope Team"]
 maintainers = ["Xilinx ChipScope Team"]
 license = "Apache-2.0 AND EPL-2.0"
 repository = "https://github.com/Xilinx/chipscopy"
 documentation = "https://xilinx.github.io/chipscopy/"
 readme = "README.md"
```

### Comparing `chipscopy-2023.1.dev1676913681/setup.py` & `chipscopy-2023.1.dev1677697072/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 entry_points = \
 {'console_scripts': ['chipscopy-get-examples = '
                      'chipscopy._cli.example_delivery:main',
                      'csutil = chipscopy._cli._chipscopy:main']}
 
 setup_kwargs = {
     'name': 'chipscopy',
-    'version': '2023.1.dev1676913681',
+    'version': '2023.1.dev1677697072',
     'description': 'Open-source project from Xilinx® that enables high-level control of Versal debug IP running in hardware',
     'long_description': '# 🐍 ChipScoPy README\n\n[![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n![](https://raw.githubusercontent.com/Xilinx/chipscopy/master/docs/images/chipscopy_logo_head_right_transparent_background.png)\n\nChipScoPy is an open-source project from Xilinx® that enables high-level control of Versal debug IP running in hardware.\nUsing a simple Python API, developers can control and communicate with ChipScope® debug IP such as the Integrated Logic\nAnalyzer (ILA), Virtual IO (VIO), device memory access, and more.\n\nChipScoPy communicates with Versal devices. It does not work with older devices such as Ultrascale+ and 7-Series devices.\n\n-------------------------------------------------------------------------------\n\n![](https://raw.githubusercontent.com/Xilinx/chipscopy/master/docs/images/chipscopy_overview.png)\n\n-------------------------------------------------------------------------------\n\n[ChipScoPy Overview](https://xilinx.github.io/chipscopy/2023.1/overview.html)\n\n-------------------------------------------------------------------------------\n\n[System Requirements](https://xilinx.github.io/chipscopy/2023.1/system_requirements.html)\n\n-------------------------------------------------------------------------------\n\n[ChipScoPy Installation](https://xilinx.github.io/chipscopy/2023.1/chipscopy_installation.html)\n\n-------------------------------------------------------------------------------\n\n[ChipScoPy Examples](https://github.com/Xilinx/chipscopy/tree/master/chipscopy/examples)\n\n-------------------------------------------------------------------------------\n\n[FAQ](https://github.com/Xilinx/chipscopy/blob/master/FAQ.md)\n\n-------------------------------------------------------------------------------\n\n[API Documentation](https://xilinx.github.io/chipscopy/)\n\n-------------------------------------------------------------------------------\n',
     'author': 'Xilinx ChipScope Team',
     'author_email': 'None',
     'maintainer': 'Xilinx ChipScope Team',
     'maintainer_email': 'None',
     'url': 'https://github.com/Xilinx/chipscopy',
```

### Comparing `chipscopy-2023.1.dev1676913681/PKG-INFO` & `chipscopy-2023.1.dev1677697072/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chipscopy
-Version: 2023.1.dev1676913681
+Version: 2023.1.dev1677697072
 Summary: Open-source project from Xilinx® that enables high-level control of Versal debug IP running in hardware
 Home-page: https://github.com/Xilinx/chipscopy
 License: Apache-2.0 AND EPL-2.0
 Author: Xilinx ChipScope Team
 Maintainer: Xilinx ChipScope Team
 Requires-Python: >=3.8.3,<4.0.0
 Classifier: License :: Other/Proprietary License
```

