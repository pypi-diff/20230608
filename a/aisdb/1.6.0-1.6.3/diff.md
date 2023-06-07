# Comparing `tmp/aisdb-1.6.0-cp39-none-win_amd64.whl.zip` & `tmp/aisdb-1.6.3-cp39-cp39-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,165 +1,67 @@
-Zip file size: 3478752 bytes, number of entries: 163
--rw-r--r--  4.6 unx     5005 b- defN 23-May-04 03:22 aisdb-1.6.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-May-04 03:22 aisdb-1.6.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     5010 b- defN 23-May-04 03:22 aisdb/aisdb_sql/coarsetype.sql
--rw-r--r--  4.6 unx      372 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_dynamic_clustered.sql
--rw-r--r--  4.6 unx      114 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_griddata.sql
--rw-r--r--  4.6 unx      561 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_static.sql
--rw-r--r--  4.6 unx      270 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_static_aggregate.sql
--rw-r--r--  4.6 unx      384 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
--rw-r--r--  4.6 unx       47 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_aliases.sql
--rw-r--r--  4.6 unx       97 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_coarsetype.sql
--rw-r--r--  4.6 unx      134 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
--rw-r--r--  4.6 unx      195 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_static.sql
--rw-r--r--  4.6 unx      221 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_static_aggregate.sql
--rw-r--r--  4.6 unx      247 b- defN 23-May-04 03:22 aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
--rw-r--r--  4.6 unx      424 b- defN 23-May-04 03:22 aisdb/aisdb_sql/insert_static.sql
--rw-r--r--  4.6 unx      790 b- defN 23-May-04 03:22 aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
--rw-r--r--  4.6 unx      330 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_columns_static.sql
--rw-r--r--  4.6 unx      513 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
--rw-r--r--  4.6 unx      910 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_merged_all.sql
--rw-r--r--  4.6 unx      677 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_static_join_webdata.sql
--rw-r--r--  4.6 unx     5035 b- defN 23-May-04 03:22 aisdb/database/create_tables.py
--rw-r--r--  4.6 unx     6558 b- defN 23-May-04 03:22 aisdb/database/dbconn.py
--rw-r--r--  4.6 unx    12239 b- defN 23-May-04 03:22 aisdb/database/dbqry.py
--rw-r--r--  4.6 unx     9948 b- defN 23-May-04 03:22 aisdb/database/decoder.py
--rw-r--r--  4.6 unx     3272 b- defN 23-May-04 03:22 aisdb/database/sqlfcn.py
--rw-r--r--  4.6 unx     1795 b- defN 23-May-04 03:22 aisdb/database/sqlfcn_callbacks.py
--rw-r--r--  4.6 unx     4318 b- defN 23-May-04 03:22 aisdb/database/sql_query_strings.py
--rw-r--r--  4.6 unx        2 b- defN 23-May-04 03:22 aisdb/database/__init__.py
--rw-r--r--  4.6 unx     7991 b- defN 23-May-04 03:22 aisdb/denoising_encoder.py
--rw-r--r--  4.6 unx    19098 b- defN 23-May-04 03:22 aisdb/gis.py
--rw-r--r--  4.6 unx     1655 b- defN 23-May-04 03:22 aisdb/interp.py
--rw-r--r--  4.6 unx    19380 b- defN 23-May-04 03:22 aisdb/network_graph.py
--rw-r--r--  4.6 unx     8306 b- defN 23-May-04 03:22 aisdb/proc_util.py
--rw-r--r--  4.6 unx     2534 b- defN 23-May-04 03:22 aisdb/receiver.py
--rw-r--r--  4.6 unx     3229 b- defN 23-May-04 03:22 aisdb/tests/create_testing_data.py
--rw-r--r--  4.6 unx    84630 b- defN 23-May-04 03:22 aisdb/tests/testdata/test_data_20211101.nm4
--rw-r--r--  4.6 unx    23613 b- defN 23-May-04 03:22 aisdb/tests/testdata/test_data_20211101.nm4.gz
--rw-r--r--  4.6 unx    23766 b- defN 23-May-04 03:22 aisdb/tests/testdata/test_data_20211101.nm4.zip
--rw-r--r--  4.6 unx     1454 b- defN 23-May-04 03:22 aisdb/tests/test_00_decode.py
--rw-r--r--  4.6 unx     2816 b- defN 23-May-04 03:22 aisdb/tests/test_01_createtables.py
--rw-r--r--  4.6 unx     2882 b- defN 23-May-04 03:22 aisdb/tests/test_02_dbqry.py
--rw-r--r--  4.6 unx     3050 b- defN 23-May-04 03:22 aisdb/tests/test_02_sqlfcn.py
--rw-r--r--  4.6 unx     3061 b- defN 23-May-04 03:22 aisdb/tests/test_03_gis.py
--rw-r--r--  4.6 unx     2399 b- defN 23-May-04 03:22 aisdb/tests/test_04_trackgen.py
--rw-r--r--  4.6 unx     4517 b- defN 23-May-04 03:22 aisdb/tests/test_05_proc_util.py
--rw-r--r--  4.6 unx     1124 b- defN 23-May-04 03:22 aisdb/tests/test_06_interp.py
--rw-r--r--  4.6 unx     1307 b- defN 23-May-04 03:22 aisdb/tests/test_07_bathymetry.py
--rw-r--r--  4.6 unx     1173 b- defN 23-May-04 03:22 aisdb/tests/test_07_shore_dist.py
--rw-r--r--  4.6 unx     2662 b- defN 23-May-04 03:22 aisdb/tests/test_08_marinetraffic.py
--rw-r--r--  4.6 unx     1732 b- defN 23-May-04 03:22 aisdb/tests/test_08_wsa.py
--rw-r--r--  4.6 unx     3722 b- defN 23-May-04 03:22 aisdb/tests/test_09_network_graph.py
--rw-r--r--  4.6 unx      810 b- defN 23-May-04 03:22 aisdb/tests/test_11_postgres.py
--rw-r--r--  4.6 unx       76 b- defN 23-May-04 03:22 aisdb/tests/test_rx.py
--rw-r--r--  4.6 unx   228241 b- defN 23-May-04 03:22 aisdb/tests/test_zones/test_zones.zip
--rw-r--r--  4.6 unx        0 b- defN 23-May-04 03:22 aisdb/tests/__init__.py
--rw-r--r--  4.6 unx     7874 b- defN 23-May-04 03:22 aisdb/track_gen.py
--rw-r--r--  4.6 unx     5590 b- defN 23-May-04 03:22 aisdb/webdata/bathymetry.py
--rw-r--r--  4.6 unx     2520 b- defN 23-May-04 03:22 aisdb/webdata/load_raster.py
--rw-r--r--  4.6 unx    11326 b- defN 23-May-04 03:22 aisdb/webdata/marinetraffic.py
--rw-r--r--  4.6 unx     2758 b- defN 23-May-04 03:22 aisdb/webdata/shore_dist.py
--rw-r--r--  4.6 unx     2565 b- defN 23-May-04 03:22 aisdb/webdata/_scraper.py
--rw-r--r--  4.6 unx        0 b- defN 23-May-04 03:22 aisdb/webdata/__init__.py
--rw-r--r--  4.6 unx     7200 b- defN 23-May-04 03:22 aisdb/web_interface.py
--rw-r--r--  4.6 unx     3959 b- defN 23-May-04 03:22 aisdb/wsa.py
--rw-r--r--  4.6 unx     1680 b- defN 23-May-04 03:22 aisdb/__init__.py
--rw-r--r--  4.6 unx     1680 b- defN 23-May-04 03:22 aisdb/__init__.py
--rw-r--r--  4.6 unx     7991 b- defN 23-May-04 03:22 aisdb/denoising_encoder.py
--rw-r--r--  4.6 unx    19098 b- defN 23-May-04 03:22 aisdb/gis.py
--rw-r--r--  4.6 unx     1655 b- defN 23-May-04 03:22 aisdb/interp.py
--rw-r--r--  4.6 unx    19380 b- defN 23-May-04 03:22 aisdb/network_graph.py
--rw-r--r--  4.6 unx     8306 b- defN 23-May-04 03:22 aisdb/proc_util.py
--rw-r--r--  4.6 unx     2534 b- defN 23-May-04 03:22 aisdb/receiver.py
--rw-r--r--  4.6 unx     7874 b- defN 23-May-04 03:22 aisdb/track_gen.py
--rw-r--r--  4.6 unx     7200 b- defN 23-May-04 03:22 aisdb/web_interface.py
--rw-r--r--  4.6 unx     3959 b- defN 23-May-04 03:22 aisdb/wsa.py
--rw-r--r--  4.6 unx     5010 b- defN 23-May-04 03:22 aisdb/aisdb_sql/coarsetype.sql
--rw-r--r--  4.6 unx      372 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_dynamic_clustered.sql
--rw-r--r--  4.6 unx      114 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_griddata.sql
--rw-r--r--  4.6 unx      561 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_static.sql
--rw-r--r--  4.6 unx      270 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_static_aggregate.sql
--rw-r--r--  4.6 unx      384 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
--rw-r--r--  4.6 unx       47 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_aliases.sql
--rw-r--r--  4.6 unx       97 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_coarsetype.sql
--rw-r--r--  4.6 unx      134 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
--rw-r--r--  4.6 unx      195 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_static.sql
--rw-r--r--  4.6 unx      221 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_static_aggregate.sql
--rw-r--r--  4.6 unx      247 b- defN 23-May-04 03:22 aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
--rw-r--r--  4.6 unx      424 b- defN 23-May-04 03:22 aisdb/aisdb_sql/insert_static.sql
--rw-r--r--  4.6 unx      790 b- defN 23-May-04 03:22 aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
--rw-r--r--  4.6 unx      330 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_columns_static.sql
--rw-r--r--  4.6 unx      513 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
--rw-r--r--  4.6 unx      910 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_merged_all.sql
--rw-r--r--  4.6 unx      677 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_static_join_webdata.sql
--rw-r--r--  4.6 unx        2 b- defN 23-May-04 03:22 aisdb/database/__init__.py
--rw-r--r--  4.6 unx     5035 b- defN 23-May-04 03:22 aisdb/database/create_tables.py
--rw-r--r--  4.6 unx     6558 b- defN 23-May-04 03:22 aisdb/database/dbconn.py
--rw-r--r--  4.6 unx    12239 b- defN 23-May-04 03:22 aisdb/database/dbqry.py
--rw-r--r--  4.6 unx     9948 b- defN 23-May-04 03:22 aisdb/database/decoder.py
--rw-r--r--  4.6 unx     4318 b- defN 23-May-04 03:22 aisdb/database/sql_query_strings.py
--rw-r--r--  4.6 unx     3272 b- defN 23-May-04 03:22 aisdb/database/sqlfcn.py
--rw-r--r--  4.6 unx     1795 b- defN 23-May-04 03:22 aisdb/database/sqlfcn_callbacks.py
--rw-r--r--  4.6 unx        0 b- defN 23-May-04 03:22 aisdb/tests/__init__.py
--rw-r--r--  4.6 unx     3229 b- defN 23-May-04 03:22 aisdb/tests/create_testing_data.py
--rw-r--r--  4.6 unx     1454 b- defN 23-May-04 03:22 aisdb/tests/test_00_decode.py
--rw-r--r--  4.6 unx     2816 b- defN 23-May-04 03:22 aisdb/tests/test_01_createtables.py
--rw-r--r--  4.6 unx     2882 b- defN 23-May-04 03:22 aisdb/tests/test_02_dbqry.py
--rw-r--r--  4.6 unx     3050 b- defN 23-May-04 03:22 aisdb/tests/test_02_sqlfcn.py
--rw-r--r--  4.6 unx     3061 b- defN 23-May-04 03:22 aisdb/tests/test_03_gis.py
--rw-r--r--  4.6 unx     2399 b- defN 23-May-04 03:22 aisdb/tests/test_04_trackgen.py
--rw-r--r--  4.6 unx     4517 b- defN 23-May-04 03:22 aisdb/tests/test_05_proc_util.py
--rw-r--r--  4.6 unx     1124 b- defN 23-May-04 03:22 aisdb/tests/test_06_interp.py
--rw-r--r--  4.6 unx     1307 b- defN 23-May-04 03:22 aisdb/tests/test_07_bathymetry.py
--rw-r--r--  4.6 unx     1173 b- defN 23-May-04 03:22 aisdb/tests/test_07_shore_dist.py
--rw-r--r--  4.6 unx     2662 b- defN 23-May-04 03:22 aisdb/tests/test_08_marinetraffic.py
--rw-r--r--  4.6 unx     1732 b- defN 23-May-04 03:22 aisdb/tests/test_08_wsa.py
--rw-r--r--  4.6 unx     3722 b- defN 23-May-04 03:22 aisdb/tests/test_09_network_graph.py
--rw-r--r--  4.6 unx      810 b- defN 23-May-04 03:22 aisdb/tests/test_11_postgres.py
--rw-r--r--  4.6 unx       76 b- defN 23-May-04 03:22 aisdb/tests/test_rx.py
--rw-r--r--  4.6 unx  1258678 b- defN 23-May-04 03:22 aisdb/tests/testdata/test_data_20210701.csv
--rw-r--r--  4.6 unx    84630 b- defN 23-May-04 03:22 aisdb/tests/testdata/test_data_20211101.nm4
--rw-r--r--  4.6 unx        0 b- defN 23-May-04 03:22 aisdb/webdata/__init__.py
--rw-r--r--  4.6 unx     2565 b- defN 23-May-04 03:22 aisdb/webdata/_scraper.py
--rw-r--r--  4.6 unx     5590 b- defN 23-May-04 03:22 aisdb/webdata/bathymetry.py
--rw-r--r--  4.6 unx     2520 b- defN 23-May-04 03:22 aisdb/webdata/load_raster.py
--rw-r--r--  4.6 unx    11326 b- defN 23-May-04 03:22 aisdb/webdata/marinetraffic.py
--rw-r--r--  4.6 unx     2758 b- defN 23-May-04 03:22 aisdb/webdata/shore_dist.py
--rw-r--r--  4.6 unx    38050 b- defN 23-May-04 03:22 aisdb_lib/Cargo.lock
--rw-r--r--  4.6 unx      990 b- defN 23-May-04 03:22 aisdb_lib/Cargo.toml
--rw-r--r--  4.6 unx      139 b- defN 23-May-04 03:22 aisdb_lib/build.rs
--rw-r--r--  4.6 unx     1672 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/OSM-113e35b9.js
--rw-r--r--  4.6 unx    17519 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/TileImage-0791bc86.js
--rw-r--r--  4.6 unx   152923 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/client_bg-7570c46f.wasm
--rw-r--r--  4.6 unx      688 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/constants-9b7da064.js
--rw-r--r--  4.6 unx     8224 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/index-f2c4f58e.css
--rw-r--r--  4.6 unx     1185 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/livestream-ef9daf96.js
--rw-r--r--  4.6 unx     2662 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/main-214e2e5c.js
--rw-r--r--  4.6 unx   405642 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/map-b944464c.js
--rw-r--r--  4.6 unx    15782 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/map-c04ede37.css
--rw-r--r--  4.6 unx    16622 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/proj-3e4e3ac0.js
--rw-r--r--  4.6 unx   203253 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/render-74985482.js
--rw-r--r--  4.6 unx     3092 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/tileserver-bd7f89a4.js
--rw-r--r--  4.6 unx     3114 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/url-91c1e158.js
--rw-r--r--  4.6 unx     1203 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/vessel_metadata-af75a617.js
--rw-r--r--  4.6 unx    26223 b- defN 23-May-04 03:22 aisdb_web/dist_map/favicon.png
--rw-r--r--  4.6 unx    21571 b- defN 23-May-04 03:22 aisdb_web/dist_map/favicon.svg
--rw-r--r--  4.6 unx     2675 b- defN 23-May-04 03:22 aisdb_web/dist_map/index.html
--rw-r--r--  4.6 unx   152923 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/client_bg-7570c46f.wasm
--rw-r--r--  4.6 unx      616 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/constants-f1a52cc9.js
--rw-r--r--  4.6 unx     8224 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/index-f2c4f58e.css
--rw-r--r--  4.6 unx     1185 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/livestream-faa61b7f.js
--rw-r--r--  4.6 unx     2662 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/main-b50358e6.js
--rw-r--r--  4.6 unx    15782 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/map-c04ede37.css
--rw-r--r--  4.6 unx   405242 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/map-e7b21464.js
--rw-r--r--  4.6 unx    16622 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/proj-04f64360.js
--rw-r--r--  4.6 unx   203253 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/render-0afdbaa3.js
--rw-r--r--  4.6 unx    20179 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/tileserver-54834007.js
--rw-r--r--  4.6 unx     3114 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/url-51dbde1e.js
--rw-r--r--  4.6 unx     1203 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-ee9a20c1.js
--rw-r--r--  4.6 unx    26223 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/favicon.png
--rw-r--r--  4.6 unx    21571 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/favicon.svg
--rw-r--r--  4.6 unx     2675 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/index.html
--rwxr-xr-x  4.6 unx  4936192 b- defN 23-May-04 03:22 aisdb/aisdb.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx    14775 b- defN 23-May-04 03:22 aisdb-1.6.0.dist-info/RECORD
-163 files, 8854155 bytes uncompressed, 3455216 bytes compressed:  61.0%
+Zip file size: 2370496 bytes, number of entries: 65
+-rw-r--r--  4.6 unx     4943 b- defN 23-Jun-07 22:44 aisdb-1.6.3.dist-info/METADATA
+-rw-r--r--  4.6 unx      103 b- defN 23-Jun-07 22:44 aisdb-1.6.3.dist-info/WHEEL
+-rw-r--r--  4.6 unx     9684 b- defN 23-Jun-07 22:44 aisdb/database/decoder.py
+-rw-r--r--  4.6 unx     1739 b- defN 23-Jun-07 22:44 aisdb/database/sqlfcn_callbacks.py
+-rw-r--r--  4.6 unx        1 b- defN 23-Jun-07 22:44 aisdb/database/__init__.py
+-rw-r--r--  4.6 unx    11962 b- defN 23-Jun-07 22:44 aisdb/database/dbqry.py
+-rw-r--r--  4.6 unx     4900 b- defN 23-Jun-07 22:44 aisdb/database/create_tables.py
+-rw-r--r--  4.6 unx     6358 b- defN 23-Jun-07 22:44 aisdb/database/dbconn.py
+-rw-r--r--  4.6 unx     3188 b- defN 23-Jun-07 22:44 aisdb/database/sqlfcn.py
+-rw-r--r--  4.6 unx     4170 b- defN 23-Jun-07 22:44 aisdb/database/sql_query_strings.py
+-rw-r--r--  4.6 unx     7650 b- defN 23-Jun-07 22:44 aisdb/track_gen.py
+-rw-r--r--  4.6 unx     2505 b- defN 23-Jun-07 22:44 aisdb/webdata/_scraper.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-07 22:44 aisdb/webdata/__init__.py
+-rw-r--r--  4.6 unx     2448 b- defN 23-Jun-07 22:44 aisdb/webdata/load_raster.py
+-rw-r--r--  4.6 unx    11002 b- defN 23-Jun-07 22:44 aisdb/webdata/marinetraffic.py
+-rw-r--r--  4.6 unx     5440 b- defN 23-Jun-07 22:44 aisdb/webdata/bathymetry.py
+-rw-r--r--  4.6 unx     2690 b- defN 23-Jun-07 22:44 aisdb/webdata/shore_dist.py
+-rw-r--r--  4.6 unx    18893 b- defN 23-Jun-07 22:44 aisdb/network_graph.py
+-rw-r--r--  4.6 unx    23613 b- defN 23-Jun-07 22:44 aisdb/tests/testdata/test_data_20211101.nm4.gz
+-rw-r--r--  4.6 unx    84630 b- defN 23-Jun-07 22:44 aisdb/tests/testdata/test_data_20211101.nm4
+-rw-r--r--  4.6 unx     2738 b- defN 23-Jun-07 22:44 aisdb/tests/test_01_createtables.py
+-rw-r--r--  4.6 unx     1420 b- defN 23-Jun-07 22:44 aisdb/tests/test_00_decode.py
+-rw-r--r--  4.6 unx     2803 b- defN 23-Jun-07 22:44 aisdb/tests/test_02_dbqry.py
+-rw-r--r--  4.6 unx     2580 b- defN 23-Jun-07 22:44 aisdb/tests/test_08_marinetraffic.py
+-rw-r--r--  4.6 unx     1131 b- defN 23-Jun-07 22:44 aisdb/tests/test_07_shore_dist.py
+-rw-r--r--  4.6 unx     1256 b- defN 23-Jun-07 22:44 aisdb/tests/test_07_bathymetry.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-07 22:44 aisdb/tests/__init__.py
+-rw-r--r--  4.6 unx     1679 b- defN 23-Jun-07 22:44 aisdb/tests/test_08_wsa.py
+-rw-r--r--  4.6 unx     2332 b- defN 23-Jun-07 22:44 aisdb/tests/test_04_trackgen.py
+-rw-r--r--  4.6 unx     1090 b- defN 23-Jun-07 22:44 aisdb/tests/test_06_interp.py
+-rw-r--r--  4.6 unx     4385 b- defN 23-Jun-07 22:44 aisdb/tests/test_05_proc_util.py
+-rw-r--r--  4.6 unx     2956 b- defN 23-Jun-07 22:44 aisdb/tests/test_03_gis.py
+-rw-r--r--  4.6 unx      778 b- defN 23-Jun-07 22:44 aisdb/tests/test_11_postgres.py
+-rw-r--r--  4.6 unx     3139 b- defN 23-Jun-07 22:44 aisdb/tests/create_testing_data.py
+-rw-r--r--  4.6 unx     3596 b- defN 23-Jun-07 22:44 aisdb/tests/test_09_network_graph.py
+-rw-r--r--  4.6 unx       74 b- defN 23-Jun-07 22:44 aisdb/tests/test_rx.py
+-rw-r--r--  4.6 unx     2956 b- defN 23-Jun-07 22:44 aisdb/tests/test_02_sqlfcn.py
+-rw-r--r--  4.6 unx     2470 b- defN 23-Jun-07 22:44 aisdb/receiver.py
+-rw-r--r--  4.6 unx     1605 b- defN 23-Jun-07 22:44 aisdb/__init__.py
+-rw-r--r--  4.6 unx     7783 b- defN 23-Jun-07 22:44 aisdb/denoising_encoder.py
+-rw-r--r--  4.6 unx      369 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
+-rw-r--r--  4.6 unx      258 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/createtable_static_aggregate.sql
+-rw-r--r--  4.6 unx      763 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
+-rw-r--r--  4.6 unx      125 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
+-rw-r--r--  4.6 unx      108 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/createtable_griddata.sql
+-rw-r--r--  4.6 unx     4924 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/coarsetype.sql
+-rw-r--r--  4.6 unx      881 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/select_merged_all.sql
+-rw-r--r--  4.6 unx       91 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/cte_coarsetype.sql
+-rw-r--r--  4.6 unx      185 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/cte_static.sql
+-rw-r--r--  4.6 unx      539 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/createtable_static.sql
+-rw-r--r--  4.6 unx      210 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/cte_static_aggregate.sql
+-rw-r--r--  4.6 unx      493 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
+-rw-r--r--  4.6 unx      400 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/insert_static.sql
+-rw-r--r--  4.6 unx      658 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/select_static_join_webdata.sql
+-rw-r--r--  4.6 unx      312 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/select_columns_static.sql
+-rw-r--r--  4.6 unx      230 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
+-rw-r--r--  4.6 unx      358 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/createtable_dynamic_clustered.sql
+-rw-r--r--  4.6 unx       43 b- defN 23-Jun-07 22:44 aisdb/aisdb_sql/cte_aliases.sql
+-rw-r--r--  4.6 unx     8060 b- defN 23-Jun-07 22:44 aisdb/proc_util.py
+-rw-r--r--  4.6 unx     6994 b- defN 23-Jun-07 22:44 aisdb/web_interface.py
+-rw-r--r--  4.6 unx     1599 b- defN 23-Jun-07 22:44 aisdb/interp.py
+-rw-r--r--  4.6 unx    18568 b- defN 23-Jun-07 22:44 aisdb/gis.py
+-rw-r--r--  4.6 unx     3845 b- defN 23-Jun-07 22:44 aisdb/wsa.py
+-rwxr-xr-x  4.6 unx  4624407 b- defN 23-Jun-07 22:44 aisdb/aisdb.cpython-39-darwin.so
+-rw-r--r--  4.6 unx     5658 b- defN 23-Jun-07 22:44 aisdb-1.6.3.dist-info/RECORD
+65 files, 4932768 bytes uncompressed, 2361474 bytes compressed:  52.1%
```

## zipnote {}

```diff
@@ -1,490 +1,196 @@
-Filename: aisdb-1.6.0.dist-info/METADATA
+Filename: aisdb-1.6.3.dist-info/METADATA
 Comment: 
 
-Filename: aisdb-1.6.0.dist-info/WHEEL
+Filename: aisdb-1.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: aisdb/aisdb_sql/coarsetype.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/createtable_dynamic_clustered.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/createtable_griddata.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/createtable_static.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/createtable_static_aggregate.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/cte_aliases.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/cte_coarsetype.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/cte_static.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/cte_static_aggregate.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/insert_static.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/select_columns_static.sql
+Filename: aisdb/database/decoder.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
+Filename: aisdb/database/sqlfcn_callbacks.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/select_merged_all.sql
+Filename: aisdb/database/__init__.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/select_static_join_webdata.sql
+Filename: aisdb/database/dbqry.py
 Comment: 
 
 Filename: aisdb/database/create_tables.py
 Comment: 
 
 Filename: aisdb/database/dbconn.py
 Comment: 
 
-Filename: aisdb/database/dbqry.py
-Comment: 
-
-Filename: aisdb/database/decoder.py
-Comment: 
-
 Filename: aisdb/database/sqlfcn.py
 Comment: 
 
-Filename: aisdb/database/sqlfcn_callbacks.py
-Comment: 
-
 Filename: aisdb/database/sql_query_strings.py
 Comment: 
 
-Filename: aisdb/database/__init__.py
-Comment: 
-
-Filename: aisdb/denoising_encoder.py
+Filename: aisdb/track_gen.py
 Comment: 
 
-Filename: aisdb/gis.py
+Filename: aisdb/webdata/_scraper.py
 Comment: 
 
-Filename: aisdb/interp.py
+Filename: aisdb/webdata/__init__.py
 Comment: 
 
-Filename: aisdb/network_graph.py
+Filename: aisdb/webdata/load_raster.py
 Comment: 
 
-Filename: aisdb/proc_util.py
+Filename: aisdb/webdata/marinetraffic.py
 Comment: 
 
-Filename: aisdb/receiver.py
+Filename: aisdb/webdata/bathymetry.py
 Comment: 
 
-Filename: aisdb/tests/create_testing_data.py
+Filename: aisdb/webdata/shore_dist.py
 Comment: 
 
-Filename: aisdb/tests/testdata/test_data_20211101.nm4
+Filename: aisdb/network_graph.py
 Comment: 
 
 Filename: aisdb/tests/testdata/test_data_20211101.nm4.gz
 Comment: 
 
-Filename: aisdb/tests/testdata/test_data_20211101.nm4.zip
-Comment: 
-
-Filename: aisdb/tests/test_00_decode.py
+Filename: aisdb/tests/testdata/test_data_20211101.nm4
 Comment: 
 
 Filename: aisdb/tests/test_01_createtables.py
 Comment: 
 
-Filename: aisdb/tests/test_02_dbqry.py
-Comment: 
-
-Filename: aisdb/tests/test_02_sqlfcn.py
-Comment: 
-
-Filename: aisdb/tests/test_03_gis.py
+Filename: aisdb/tests/test_00_decode.py
 Comment: 
 
-Filename: aisdb/tests/test_04_trackgen.py
+Filename: aisdb/tests/test_02_dbqry.py
 Comment: 
 
-Filename: aisdb/tests/test_05_proc_util.py
+Filename: aisdb/tests/test_08_marinetraffic.py
 Comment: 
 
-Filename: aisdb/tests/test_06_interp.py
+Filename: aisdb/tests/test_07_shore_dist.py
 Comment: 
 
 Filename: aisdb/tests/test_07_bathymetry.py
 Comment: 
 
-Filename: aisdb/tests/test_07_shore_dist.py
-Comment: 
-
-Filename: aisdb/tests/test_08_marinetraffic.py
+Filename: aisdb/tests/__init__.py
 Comment: 
 
 Filename: aisdb/tests/test_08_wsa.py
 Comment: 
 
-Filename: aisdb/tests/test_09_network_graph.py
-Comment: 
-
-Filename: aisdb/tests/test_11_postgres.py
-Comment: 
-
-Filename: aisdb/tests/test_rx.py
-Comment: 
-
-Filename: aisdb/tests/test_zones/test_zones.zip
-Comment: 
-
-Filename: aisdb/tests/__init__.py
-Comment: 
-
-Filename: aisdb/track_gen.py
+Filename: aisdb/tests/test_04_trackgen.py
 Comment: 
 
-Filename: aisdb/webdata/bathymetry.py
+Filename: aisdb/tests/test_06_interp.py
 Comment: 
 
-Filename: aisdb/webdata/load_raster.py
+Filename: aisdb/tests/test_05_proc_util.py
 Comment: 
 
-Filename: aisdb/webdata/marinetraffic.py
+Filename: aisdb/tests/test_03_gis.py
 Comment: 
 
-Filename: aisdb/webdata/shore_dist.py
+Filename: aisdb/tests/test_11_postgres.py
 Comment: 
 
-Filename: aisdb/webdata/_scraper.py
+Filename: aisdb/tests/create_testing_data.py
 Comment: 
 
-Filename: aisdb/webdata/__init__.py
+Filename: aisdb/tests/test_09_network_graph.py
 Comment: 
 
-Filename: aisdb/web_interface.py
+Filename: aisdb/tests/test_rx.py
 Comment: 
 
-Filename: aisdb/wsa.py
+Filename: aisdb/tests/test_02_sqlfcn.py
 Comment: 
 
-Filename: aisdb/__init__.py
+Filename: aisdb/receiver.py
 Comment: 
 
 Filename: aisdb/__init__.py
 Comment: 
 
 Filename: aisdb/denoising_encoder.py
 Comment: 
 
-Filename: aisdb/gis.py
-Comment: 
-
-Filename: aisdb/interp.py
-Comment: 
-
-Filename: aisdb/network_graph.py
-Comment: 
-
-Filename: aisdb/proc_util.py
-Comment: 
-
-Filename: aisdb/receiver.py
-Comment: 
-
-Filename: aisdb/track_gen.py
-Comment: 
-
-Filename: aisdb/web_interface.py
+Filename: aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
 Comment: 
 
-Filename: aisdb/wsa.py
+Filename: aisdb/aisdb_sql/createtable_static_aggregate.sql
 Comment: 
 
-Filename: aisdb/aisdb_sql/coarsetype.sql
+Filename: aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
 Comment: 
 
-Filename: aisdb/aisdb_sql/createtable_dynamic_clustered.sql
+Filename: aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
 Comment: 
 
 Filename: aisdb/aisdb_sql/createtable_griddata.sql
 Comment: 
 
-Filename: aisdb/aisdb_sql/createtable_static.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/createtable_static_aggregate.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
+Filename: aisdb/aisdb_sql/coarsetype.sql
 Comment: 
 
-Filename: aisdb/aisdb_sql/cte_aliases.sql
+Filename: aisdb/aisdb_sql/select_merged_all.sql
 Comment: 
 
 Filename: aisdb/aisdb_sql/cte_coarsetype.sql
 Comment: 
 
-Filename: aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
-Comment: 
-
 Filename: aisdb/aisdb_sql/cte_static.sql
 Comment: 
 
-Filename: aisdb/aisdb_sql/cte_static_aggregate.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/insert_static.sql
-Comment: 
-
-Filename: aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
+Filename: aisdb/aisdb_sql/createtable_static.sql
 Comment: 
 
-Filename: aisdb/aisdb_sql/select_columns_static.sql
+Filename: aisdb/aisdb_sql/cte_static_aggregate.sql
 Comment: 
 
 Filename: aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
 Comment: 
 
-Filename: aisdb/aisdb_sql/select_merged_all.sql
+Filename: aisdb/aisdb_sql/insert_static.sql
 Comment: 
 
 Filename: aisdb/aisdb_sql/select_static_join_webdata.sql
 Comment: 
 
-Filename: aisdb/database/__init__.py
-Comment: 
-
-Filename: aisdb/database/create_tables.py
-Comment: 
-
-Filename: aisdb/database/dbconn.py
-Comment: 
-
-Filename: aisdb/database/dbqry.py
-Comment: 
-
-Filename: aisdb/database/decoder.py
-Comment: 
-
-Filename: aisdb/database/sql_query_strings.py
-Comment: 
-
-Filename: aisdb/database/sqlfcn.py
-Comment: 
-
-Filename: aisdb/database/sqlfcn_callbacks.py
-Comment: 
-
-Filename: aisdb/tests/__init__.py
-Comment: 
-
-Filename: aisdb/tests/create_testing_data.py
-Comment: 
-
-Filename: aisdb/tests/test_00_decode.py
-Comment: 
-
-Filename: aisdb/tests/test_01_createtables.py
-Comment: 
-
-Filename: aisdb/tests/test_02_dbqry.py
-Comment: 
-
-Filename: aisdb/tests/test_02_sqlfcn.py
-Comment: 
-
-Filename: aisdb/tests/test_03_gis.py
-Comment: 
-
-Filename: aisdb/tests/test_04_trackgen.py
-Comment: 
-
-Filename: aisdb/tests/test_05_proc_util.py
-Comment: 
-
-Filename: aisdb/tests/test_06_interp.py
-Comment: 
-
-Filename: aisdb/tests/test_07_bathymetry.py
-Comment: 
-
-Filename: aisdb/tests/test_07_shore_dist.py
-Comment: 
-
-Filename: aisdb/tests/test_08_marinetraffic.py
-Comment: 
-
-Filename: aisdb/tests/test_08_wsa.py
-Comment: 
-
-Filename: aisdb/tests/test_09_network_graph.py
-Comment: 
-
-Filename: aisdb/tests/test_11_postgres.py
-Comment: 
-
-Filename: aisdb/tests/test_rx.py
-Comment: 
-
-Filename: aisdb/tests/testdata/test_data_20210701.csv
-Comment: 
-
-Filename: aisdb/tests/testdata/test_data_20211101.nm4
-Comment: 
-
-Filename: aisdb/webdata/__init__.py
-Comment: 
-
-Filename: aisdb/webdata/_scraper.py
-Comment: 
-
-Filename: aisdb/webdata/bathymetry.py
-Comment: 
-
-Filename: aisdb/webdata/load_raster.py
-Comment: 
-
-Filename: aisdb/webdata/marinetraffic.py
-Comment: 
-
-Filename: aisdb/webdata/shore_dist.py
-Comment: 
-
-Filename: aisdb_lib/Cargo.lock
-Comment: 
-
-Filename: aisdb_lib/Cargo.toml
-Comment: 
-
-Filename: aisdb_lib/build.rs
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/OSM-113e35b9.js
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/TileImage-0791bc86.js
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/client_bg-7570c46f.wasm
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/constants-9b7da064.js
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/index-f2c4f58e.css
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/livestream-ef9daf96.js
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/main-214e2e5c.js
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/map-b944464c.js
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/map-c04ede37.css
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/proj-3e4e3ac0.js
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/render-74985482.js
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/tileserver-bd7f89a4.js
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/url-91c1e158.js
-Comment: 
-
-Filename: aisdb_web/dist_map/assets/vessel_metadata-af75a617.js
-Comment: 
-
-Filename: aisdb_web/dist_map/favicon.png
-Comment: 
-
-Filename: aisdb_web/dist_map/favicon.svg
-Comment: 
-
-Filename: aisdb_web/dist_map/index.html
-Comment: 
-
-Filename: aisdb_web/dist_map_bingmaps/assets/client_bg-7570c46f.wasm
-Comment: 
-
-Filename: aisdb_web/dist_map_bingmaps/assets/constants-f1a52cc9.js
-Comment: 
-
-Filename: aisdb_web/dist_map_bingmaps/assets/index-f2c4f58e.css
-Comment: 
-
-Filename: aisdb_web/dist_map_bingmaps/assets/livestream-faa61b7f.js
-Comment: 
-
-Filename: aisdb_web/dist_map_bingmaps/assets/main-b50358e6.js
-Comment: 
-
-Filename: aisdb_web/dist_map_bingmaps/assets/map-c04ede37.css
-Comment: 
-
-Filename: aisdb_web/dist_map_bingmaps/assets/map-e7b21464.js
+Filename: aisdb/aisdb_sql/select_columns_static.sql
 Comment: 
 
-Filename: aisdb_web/dist_map_bingmaps/assets/proj-04f64360.js
+Filename: aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
 Comment: 
 
-Filename: aisdb_web/dist_map_bingmaps/assets/render-0afdbaa3.js
+Filename: aisdb/aisdb_sql/createtable_dynamic_clustered.sql
 Comment: 
 
-Filename: aisdb_web/dist_map_bingmaps/assets/tileserver-54834007.js
+Filename: aisdb/aisdb_sql/cte_aliases.sql
 Comment: 
 
-Filename: aisdb_web/dist_map_bingmaps/assets/url-51dbde1e.js
+Filename: aisdb/proc_util.py
 Comment: 
 
-Filename: aisdb_web/dist_map_bingmaps/assets/vessel_metadata-ee9a20c1.js
+Filename: aisdb/web_interface.py
 Comment: 
 
-Filename: aisdb_web/dist_map_bingmaps/favicon.png
+Filename: aisdb/interp.py
 Comment: 
 
-Filename: aisdb_web/dist_map_bingmaps/favicon.svg
+Filename: aisdb/gis.py
 Comment: 
 
-Filename: aisdb_web/dist_map_bingmaps/index.html
+Filename: aisdb/wsa.py
 Comment: 
 
-Filename: aisdb/aisdb.cp39-win_amd64.pyd
+Filename: aisdb/aisdb.cpython-39-darwin.so
 Comment: 
 
-Filename: aisdb-1.6.0.dist-info/RECORD
+Filename: aisdb-1.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aisdb/aisdb_sql/coarsetype.sql

 * *Ordering differences only*

```diff
@@ -1,86 +1,86 @@
-CREATE TABLE coarsetype_ref (
-    coarse_type integer,
-    coarse_type_txt character varying(75),
-    PRIMARY KEY (coarse_type)
-);
-INSERT INTO coarsetype_ref VALUES(20,'Wing In Grnd');
-INSERT INTO coarsetype_ref VALUES(21,'Wing In Grnd, hazardous category A');
-INSERT INTO coarsetype_ref VALUES(22,'Wing In Grnd, hazardous category B');
-INSERT INTO coarsetype_ref VALUES(23,'Wing In Grnd, hazardous category C');
-INSERT INTO coarsetype_ref VALUES(24,'Wing In Grnd, hazardous category D');
-INSERT INTO coarsetype_ref VALUES(25,'Wing In Grnd');
-INSERT INTO coarsetype_ref VALUES(26,'Wing In Grnd');
-INSERT INTO coarsetype_ref VALUES(27,'Wing In Grnd');
-INSERT INTO coarsetype_ref VALUES(28,'Wing In Grnd');
-INSERT INTO coarsetype_ref VALUES(29,'Wing In Grnd');
-INSERT INTO coarsetype_ref VALUES(30,'Fishing');
-INSERT INTO coarsetype_ref VALUES(31,'Towing');
-INSERT INTO coarsetype_ref VALUES(32,'Towing - length >200m or breadth >25m');
-INSERT INTO coarsetype_ref VALUES(33,'Dredger');
-INSERT INTO coarsetype_ref VALUES(34,'Dive Vessel');
-INSERT INTO coarsetype_ref VALUES(35,'Military Ops');
-INSERT INTO coarsetype_ref VALUES(36,'Sailing Vessel');
-INSERT INTO coarsetype_ref VALUES(37,'Pleasure Craft');
-INSERT INTO coarsetype_ref VALUES(38,'Reserved for future use');
-INSERT INTO coarsetype_ref VALUES(39,'Reserved for future use');
-INSERT INTO coarsetype_ref VALUES(40,'High speed craft');
-INSERT INTO coarsetype_ref VALUES(41,'High speed craft, hazardous category A');
-INSERT INTO coarsetype_ref VALUES(42,'High speed craft, hazardous category B');
-INSERT INTO coarsetype_ref VALUES(43,'High speed craft, hazardous category C');
-INSERT INTO coarsetype_ref VALUES(44,'High speed craft, hazardous category D');
-INSERT INTO coarsetype_ref VALUES(45,'High speed craft');
-INSERT INTO coarsetype_ref VALUES(46,'High speed craft');
-INSERT INTO coarsetype_ref VALUES(47,'High speed craft');
-INSERT INTO coarsetype_ref VALUES(48,'High speed craft');
-INSERT INTO coarsetype_ref VALUES(49,'High speed craft');
-INSERT INTO coarsetype_ref VALUES(50,'Pilot vessel');
-INSERT INTO coarsetype_ref VALUES(51,'SAR');
-INSERT INTO coarsetype_ref VALUES(52,'Tug');
-INSERT INTO coarsetype_ref VALUES(53,'Port Tender');
-INSERT INTO coarsetype_ref VALUES(54,'Anti-Pollution');
-INSERT INTO coarsetype_ref VALUES(55,'Law Enforce');
-INSERT INTO coarsetype_ref VALUES(56,'Spare - local vessels');
-INSERT INTO coarsetype_ref VALUES(57,'Spare - local vessels');
-INSERT INTO coarsetype_ref VALUES(58,'Medical Trans)');
-INSERT INTO coarsetype_ref VALUES(59,'Ships and aircraft of States not parties to an armed conflict');
-INSERT INTO coarsetype_ref VALUES(60,'Passenger');
-INSERT INTO coarsetype_ref VALUES(61,'Passenger, hazardous category A');
-INSERT INTO coarsetype_ref VALUES(62,'Passenger, hazardous category B');
-INSERT INTO coarsetype_ref VALUES(63,'Passenger, hazardous category C');
-INSERT INTO coarsetype_ref VALUES(64,'Passenger, hazardous category D');
-INSERT INTO coarsetype_ref VALUES(65,'Passenger');
-INSERT INTO coarsetype_ref VALUES(66,'Passenger');
-INSERT INTO coarsetype_ref VALUES(67,'Passenger');
-INSERT INTO coarsetype_ref VALUES(68,'Passenger');
-INSERT INTO coarsetype_ref VALUES(69,'Passenger');
-INSERT INTO coarsetype_ref VALUES(70,'Cargo');
-INSERT INTO coarsetype_ref VALUES(71,'Cargo, hazardous category A');
-INSERT INTO coarsetype_ref VALUES(72,'Cargo, hazardous category B');
-INSERT INTO coarsetype_ref VALUES(73,'Cargo, hazardous category C');
-INSERT INTO coarsetype_ref VALUES(74,'Cargo, hazardous category D');
-INSERT INTO coarsetype_ref VALUES(75,'Cargo');
-INSERT INTO coarsetype_ref VALUES(76,'Cargo');
-INSERT INTO coarsetype_ref VALUES(77,'Cargo');
-INSERT INTO coarsetype_ref VALUES(78,'Cargo');
-INSERT INTO coarsetype_ref VALUES(79,'Cargo');
-INSERT INTO coarsetype_ref VALUES(80,'Tanker');
-INSERT INTO coarsetype_ref VALUES(81,'Tanker, hazardous category A');
-INSERT INTO coarsetype_ref VALUES(82,'Tanker, hazardous category B');
-INSERT INTO coarsetype_ref VALUES(83,'Tanker, hazardous category C');
-INSERT INTO coarsetype_ref VALUES(84,'Tanker, hazardous category D');
-INSERT INTO coarsetype_ref VALUES(85,'Tanker');
-INSERT INTO coarsetype_ref VALUES(86,'Tanker');
-INSERT INTO coarsetype_ref VALUES(87,'Tanker');
-INSERT INTO coarsetype_ref VALUES(88,'Tanker');
-INSERT INTO coarsetype_ref VALUES(89,'Tanker');
-INSERT INTO coarsetype_ref VALUES(90,'Other');
-INSERT INTO coarsetype_ref VALUES(91,'Other, hazardous category A');
-INSERT INTO coarsetype_ref VALUES(92,'Other, hazardous category B');
-INSERT INTO coarsetype_ref VALUES(93,'Other, hazardous category C');
-INSERT INTO coarsetype_ref VALUES(94,'Other, hazardous category D');
-INSERT INTO coarsetype_ref VALUES(95,'Other');
-INSERT INTO coarsetype_ref VALUES(96,'Other');
-INSERT INTO coarsetype_ref VALUES(97,'Other');
-INSERT INTO coarsetype_ref VALUES(98,'Other');
-INSERT INTO coarsetype_ref VALUES(99,'Other');
-INSERT INTO coarsetype_ref VALUES(100,'Unknown');
+CREATE TABLE coarsetype_ref (
+    coarse_type integer,
+    coarse_type_txt character varying(75),
+    PRIMARY KEY (coarse_type)
+);
+INSERT INTO coarsetype_ref VALUES(20,'Wing In Grnd');
+INSERT INTO coarsetype_ref VALUES(21,'Wing In Grnd, hazardous category A');
+INSERT INTO coarsetype_ref VALUES(22,'Wing In Grnd, hazardous category B');
+INSERT INTO coarsetype_ref VALUES(23,'Wing In Grnd, hazardous category C');
+INSERT INTO coarsetype_ref VALUES(24,'Wing In Grnd, hazardous category D');
+INSERT INTO coarsetype_ref VALUES(25,'Wing In Grnd');
+INSERT INTO coarsetype_ref VALUES(26,'Wing In Grnd');
+INSERT INTO coarsetype_ref VALUES(27,'Wing In Grnd');
+INSERT INTO coarsetype_ref VALUES(28,'Wing In Grnd');
+INSERT INTO coarsetype_ref VALUES(29,'Wing In Grnd');
+INSERT INTO coarsetype_ref VALUES(30,'Fishing');
+INSERT INTO coarsetype_ref VALUES(31,'Towing');
+INSERT INTO coarsetype_ref VALUES(32,'Towing - length >200m or breadth >25m');
+INSERT INTO coarsetype_ref VALUES(33,'Dredger');
+INSERT INTO coarsetype_ref VALUES(34,'Dive Vessel');
+INSERT INTO coarsetype_ref VALUES(35,'Military Ops');
+INSERT INTO coarsetype_ref VALUES(36,'Sailing Vessel');
+INSERT INTO coarsetype_ref VALUES(37,'Pleasure Craft');
+INSERT INTO coarsetype_ref VALUES(38,'Reserved for future use');
+INSERT INTO coarsetype_ref VALUES(39,'Reserved for future use');
+INSERT INTO coarsetype_ref VALUES(40,'High speed craft');
+INSERT INTO coarsetype_ref VALUES(41,'High speed craft, hazardous category A');
+INSERT INTO coarsetype_ref VALUES(42,'High speed craft, hazardous category B');
+INSERT INTO coarsetype_ref VALUES(43,'High speed craft, hazardous category C');
+INSERT INTO coarsetype_ref VALUES(44,'High speed craft, hazardous category D');
+INSERT INTO coarsetype_ref VALUES(45,'High speed craft');
+INSERT INTO coarsetype_ref VALUES(46,'High speed craft');
+INSERT INTO coarsetype_ref VALUES(47,'High speed craft');
+INSERT INTO coarsetype_ref VALUES(48,'High speed craft');
+INSERT INTO coarsetype_ref VALUES(49,'High speed craft');
+INSERT INTO coarsetype_ref VALUES(50,'Pilot vessel');
+INSERT INTO coarsetype_ref VALUES(51,'SAR');
+INSERT INTO coarsetype_ref VALUES(52,'Tug');
+INSERT INTO coarsetype_ref VALUES(53,'Port Tender');
+INSERT INTO coarsetype_ref VALUES(54,'Anti-Pollution');
+INSERT INTO coarsetype_ref VALUES(55,'Law Enforce');
+INSERT INTO coarsetype_ref VALUES(56,'Spare - local vessels');
+INSERT INTO coarsetype_ref VALUES(57,'Spare - local vessels');
+INSERT INTO coarsetype_ref VALUES(58,'Medical Trans)');
+INSERT INTO coarsetype_ref VALUES(59,'Ships and aircraft of States not parties to an armed conflict');
+INSERT INTO coarsetype_ref VALUES(60,'Passenger');
+INSERT INTO coarsetype_ref VALUES(61,'Passenger, hazardous category A');
+INSERT INTO coarsetype_ref VALUES(62,'Passenger, hazardous category B');
+INSERT INTO coarsetype_ref VALUES(63,'Passenger, hazardous category C');
+INSERT INTO coarsetype_ref VALUES(64,'Passenger, hazardous category D');
+INSERT INTO coarsetype_ref VALUES(65,'Passenger');
+INSERT INTO coarsetype_ref VALUES(66,'Passenger');
+INSERT INTO coarsetype_ref VALUES(67,'Passenger');
+INSERT INTO coarsetype_ref VALUES(68,'Passenger');
+INSERT INTO coarsetype_ref VALUES(69,'Passenger');
+INSERT INTO coarsetype_ref VALUES(70,'Cargo');
+INSERT INTO coarsetype_ref VALUES(71,'Cargo, hazardous category A');
+INSERT INTO coarsetype_ref VALUES(72,'Cargo, hazardous category B');
+INSERT INTO coarsetype_ref VALUES(73,'Cargo, hazardous category C');
+INSERT INTO coarsetype_ref VALUES(74,'Cargo, hazardous category D');
+INSERT INTO coarsetype_ref VALUES(75,'Cargo');
+INSERT INTO coarsetype_ref VALUES(76,'Cargo');
+INSERT INTO coarsetype_ref VALUES(77,'Cargo');
+INSERT INTO coarsetype_ref VALUES(78,'Cargo');
+INSERT INTO coarsetype_ref VALUES(79,'Cargo');
+INSERT INTO coarsetype_ref VALUES(80,'Tanker');
+INSERT INTO coarsetype_ref VALUES(81,'Tanker, hazardous category A');
+INSERT INTO coarsetype_ref VALUES(82,'Tanker, hazardous category B');
+INSERT INTO coarsetype_ref VALUES(83,'Tanker, hazardous category C');
+INSERT INTO coarsetype_ref VALUES(84,'Tanker, hazardous category D');
+INSERT INTO coarsetype_ref VALUES(85,'Tanker');
+INSERT INTO coarsetype_ref VALUES(86,'Tanker');
+INSERT INTO coarsetype_ref VALUES(87,'Tanker');
+INSERT INTO coarsetype_ref VALUES(88,'Tanker');
+INSERT INTO coarsetype_ref VALUES(89,'Tanker');
+INSERT INTO coarsetype_ref VALUES(90,'Other');
+INSERT INTO coarsetype_ref VALUES(91,'Other, hazardous category A');
+INSERT INTO coarsetype_ref VALUES(92,'Other, hazardous category B');
+INSERT INTO coarsetype_ref VALUES(93,'Other, hazardous category C');
+INSERT INTO coarsetype_ref VALUES(94,'Other, hazardous category D');
+INSERT INTO coarsetype_ref VALUES(95,'Other');
+INSERT INTO coarsetype_ref VALUES(96,'Other');
+INSERT INTO coarsetype_ref VALUES(97,'Other');
+INSERT INTO coarsetype_ref VALUES(98,'Other');
+INSERT INTO coarsetype_ref VALUES(99,'Other');
+INSERT INTO coarsetype_ref VALUES(100,'Unknown');
```

## aisdb/aisdb_sql/createtable_dynamic_clustered.sql

 * *Ordering differences only*

```diff
@@ -1,14 +1,14 @@
-CREATE TABLE IF NOT EXISTS ais_{}_dynamic (
-    mmsi INTEGER NOT NULL,
-    time INTEGER NOT NULL,
-    longitude REAL NOT NULL,
-    latitude REAL NOT NULL,
-    rot REAL,
-    sog REAL,
-    cog REAL,
-    heading REAL,
-    maneuver BOOLEAN,
-    utc_second INTEGER,
-    source TEXT NOT NULL,
-    PRIMARY KEY (mmsi, time, longitude, latitude, sog, cog, source)
-);
+CREATE TABLE IF NOT EXISTS ais_{}_dynamic (
+    mmsi INTEGER NOT NULL,
+    time INTEGER NOT NULL,
+    longitude REAL NOT NULL,
+    latitude REAL NOT NULL,
+    rot REAL,
+    sog REAL,
+    cog REAL,
+    heading REAL,
+    maneuver BOOLEAN,
+    utc_second INTEGER,
+    source TEXT NOT NULL,
+    PRIMARY KEY (mmsi, time, longitude, latitude, sog, cog, source)
+);
```

## aisdb/aisdb_sql/createtable_griddata.sql

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-CREATE VIRTUAL TABLE IF NOT EXISTS gebco_2022 USING rtree(
-  id,
-  x0, x1,
-  y0, y1,
-  +depth_metres INT
-);
+CREATE VIRTUAL TABLE IF NOT EXISTS gebco_2022 USING rtree(
+  id,
+  x0, x1,
+  y0, y1,
+  +depth_metres INT
+);
```

## aisdb/aisdb_sql/createtable_static.sql

 * *Ordering differences only*

```diff
@@ -1,22 +1,22 @@
-CREATE TABLE IF NOT EXISTS ais_{}_static (
-    mmsi INTEGER NOT NULL,
-    time INTEGER NOT NULL,
-    vessel_name TEXT,
-    ship_type INTEGER,
-    call_sign TEXT,
-    imo INTEGER NOT NULL DEFAULT 0,
-    dim_bow INTEGER,
-    dim_stern INTEGER,
-    dim_port INTEGER,
-    dim_star INTEGER,
-    draught INTEGER,
-    destination TEXT,
-    ais_version INTEGER,
-    fixing_device TEXT,
-    eta_month INTEGER,
-    eta_day INTEGER,
-    eta_hour INTEGER,
-    eta_minute INTEGER,
-    source TEXT NOT NULL,
-    PRIMARY KEY (mmsi, time, imo, source)
-);
+CREATE TABLE IF NOT EXISTS ais_{}_static (
+    mmsi INTEGER NOT NULL,
+    time INTEGER NOT NULL,
+    vessel_name TEXT,
+    ship_type INTEGER,
+    call_sign TEXT,
+    imo INTEGER NOT NULL DEFAULT 0,
+    dim_bow INTEGER,
+    dim_stern INTEGER,
+    dim_port INTEGER,
+    dim_star INTEGER,
+    draught INTEGER,
+    destination TEXT,
+    ais_version INTEGER,
+    fixing_device TEXT,
+    eta_month INTEGER,
+    eta_day INTEGER,
+    eta_hour INTEGER,
+    eta_minute INTEGER,
+    source TEXT NOT NULL,
+    PRIMARY KEY (mmsi, time, imo, source)
+);
```

## aisdb/aisdb_sql/createtable_static_aggregate.sql

 * *Ordering differences only*

```diff
@@ -1,12 +1,12 @@
-CREATE TABLE static_{}_aggregate (
-    mmsi INTEGER PRIMARY KEY,
-    imo INTEGER,
-    vessel_name TEXT,
-    ship_type INTEGER,
-    call_sign TEXT,
-    dim_bow INTEGER,
-    dim_stern INTEGER,
-    dim_port INTEGER,
-    dim_star INTEGER,
-    draught INTEGER
-);
+CREATE TABLE static_{}_aggregate (
+    mmsi INTEGER PRIMARY KEY,
+    imo INTEGER,
+    vessel_name TEXT,
+    ship_type INTEGER,
+    call_sign TEXT,
+    dim_bow INTEGER,
+    dim_stern INTEGER,
+    dim_port INTEGER,
+    dim_star INTEGER,
+    draught INTEGER
+);
```

## aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql

 * *Ordering differences only*

```diff
@@ -1,15 +1,15 @@
-CREATE TABLE IF NOT EXISTS webdata_marinetraffic (
-    mmsi INTEGER PRIMARY KEY,
-    imo INTEGER,
-    name TEXT,
-    vesseltype_generic TEXT,
-    vesseltype_detailed TEXT,
-    callsign TEXT,
-    flag TEXT,
-    gross_tonnage INTEGER,
-    summer_dwt INTEGER,
-    length_breadth TEXT,
-    year_built INTEGER,
-    home_port TEXT,
-    error404 INTEGER NOT NULL DEFAULT 0
-);
+CREATE TABLE IF NOT EXISTS webdata_marinetraffic (
+    mmsi INTEGER PRIMARY KEY,
+    imo INTEGER,
+    name TEXT,
+    vesseltype_generic TEXT,
+    vesseltype_detailed TEXT,
+    callsign TEXT,
+    flag TEXT,
+    gross_tonnage INTEGER,
+    summer_dwt INTEGER,
+    length_breadth TEXT,
+    year_built INTEGER,
+    home_port TEXT,
+    error404 INTEGER NOT NULL DEFAULT 0
+);
```

## aisdb/aisdb_sql/cte_aliases.sql

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-dynamic_{} AS ( {}
-),
-static_{} AS ( {}
-),
+dynamic_{} AS ( {}
+),
+static_{} AS ( {}
+),
```

## aisdb/aisdb_sql/cte_coarsetype.sql

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-ref AS ( 
-  SELECT 
-    r.coarse_type, 
-    r.coarse_type_txt
-  FROM coarsetype_ref as r
-)
+ref AS ( 
+  SELECT 
+    r.coarse_type, 
+    r.coarse_type_txt
+  FROM coarsetype_ref as r
+)
```

## aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
-  SELECT 
-    d.mmsi, 
-    d.time, 
-    d.longitude,
-    d.latitude,
-    d.sog,
-    d.cog
-  FROM ais_{}_dynamic AS d
-  WHERE
+  SELECT 
+    d.mmsi, 
+    d.time, 
+    d.longitude,
+    d.latitude,
+    d.sog,
+    d.cog
+  FROM ais_{}_dynamic AS d
+  WHERE
```

## aisdb/aisdb_sql/cte_static.sql

 * *Ordering differences only*

```diff
@@ -1,10 +1,10 @@
-  SELECT 
-    s.mmsi, 
-    TRIM(s.vessel_name) as vessel_name, 
-    s.ship_type,
-    s.dim_bow, 
-    s.dim_stern, 
-    s.dim_port, 
-    s.dim_star, 
-    s.imo
-  FROM ais_{}_static AS s
+  SELECT 
+    s.mmsi, 
+    TRIM(s.vessel_name) as vessel_name, 
+    s.ship_type,
+    s.dim_bow, 
+    s.dim_stern, 
+    s.dim_port, 
+    s.dim_star, 
+    s.imo
+  FROM ais_{}_static AS s
```

## aisdb/aisdb_sql/cte_static_aggregate.sql

 * *Ordering differences only*

```diff
@@ -1,11 +1,11 @@
-
-  SELECT 
-    agg.mmsi, 
-    TRIM(agg.vessel_name) as vessel_name, 
-    agg.ship_type,
-    agg.dim_bow, 
-    agg.dim_stern, 
-    agg.dim_port, 
-    agg.dim_star, 
-    agg.imo
-  FROM static_{}_aggregate AS agg
+
+  SELECT 
+    agg.mmsi, 
+    TRIM(agg.vessel_name) as vessel_name, 
+    agg.ship_type,
+    agg.dim_bow, 
+    agg.dim_stern, 
+    agg.dim_port, 
+    agg.dim_star, 
+    agg.imo
+  FROM static_{}_aggregate AS agg
```

## aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-INSERT INTO ais_{}_dynamic
-(
-    mmsi,
-    time,
-    longitude,
-    latitude,
-    rot,
-    sog,
-    cog,
-    heading,
-    maneuver,
-    utc_second,
-    source
-)
-VALUES ($1,$2,$3,$4,$5,$6,$7,$8,$9,$10,$11)
-ON CONFLICT DO NOTHING
-;
+INSERT INTO ais_{}_dynamic
+(
+    mmsi,
+    time,
+    longitude,
+    latitude,
+    rot,
+    sog,
+    cog,
+    heading,
+    maneuver,
+    utc_second,
+    source
+)
+VALUES ($1,$2,$3,$4,$5,$6,$7,$8,$9,$10,$11)
+ON CONFLICT DO NOTHING
+;
```

## aisdb/aisdb_sql/insert_static.sql

 * *Ordering differences only*

```diff
@@ -1,24 +1,24 @@
-INSERT INTO ais_{}_static (
-    mmsi,
-    time,
-    vessel_name,
-    ship_type,
-    call_sign,
-    imo,
-    dim_bow,
-    dim_stern,
-    dim_port,
-    dim_star,
-    draught,
-    destination,
-    ais_version,
-    fixing_device,
-    eta_month,
-    eta_day,
-    eta_hour,
-    eta_minute,
-    source
-  )
-VALUES ($1,$2,$3,$4,$5,$6,$7,$8,$9,$10,$11,$12,$13,$14,$15,$16,$17,$18,$19)
-ON CONFLICT DO NOTHING
-;
+INSERT INTO ais_{}_static (
+    mmsi,
+    time,
+    vessel_name,
+    ship_type,
+    call_sign,
+    imo,
+    dim_bow,
+    dim_stern,
+    dim_port,
+    dim_star,
+    draught,
+    destination,
+    ais_version,
+    fixing_device,
+    eta_month,
+    eta_day,
+    eta_hour,
+    eta_minute,
+    source
+  )
+VALUES ($1,$2,$3,$4,$5,$6,$7,$8,$9,$10,$11,$12,$13,$14,$15,$16,$17,$18,$19)
+ON CONFLICT DO NOTHING
+;
```

## aisdb/aisdb_sql/insert_webdata_marinetraffic.sql

 * *Ordering differences only*

```diff
@@ -1,27 +1,27 @@
-INSERT INTO webdata_marinetraffic (
-    mmsi, 
-    imo, 
-    name,
-    vesseltype_generic,
-    vesseltype_detailed,
-    callsign,
-    flag,
-    gross_tonnage,
-    summer_dwt,
-    length_breadth,
-    year_built,
-    home_port
-  )
-VALUES (CAST($1 AS INT),CAST($2 AS INT),$3,$4,$5,$6,$7,$8,$9,$10,$11,$12)
-ON CONFLICT (mmsi) DO UPDATE SET 
-    imo = excluded.imo,
-    name = excluded.name, 
-    vesseltype_generic = excluded.vesseltype_generic,
-    vesseltype_detailed = excluded.vesseltype_detailed,
-    callsign = excluded.callsign,
-    flag = excluded.flag,
-    gross_tonnage = excluded.gross_tonnage,
-    summer_dwt = excluded.gross_tonnage,
-    length_breadth = excluded.length_breadth,
-    year_built = excluded.year_built,
-    home_port = excluded.home_port;
+INSERT INTO webdata_marinetraffic (
+    mmsi, 
+    imo, 
+    name,
+    vesseltype_generic,
+    vesseltype_detailed,
+    callsign,
+    flag,
+    gross_tonnage,
+    summer_dwt,
+    length_breadth,
+    year_built,
+    home_port
+  )
+VALUES (CAST($1 AS INT),CAST($2 AS INT),$3,$4,$5,$6,$7,$8,$9,$10,$11,$12)
+ON CONFLICT (mmsi) DO UPDATE SET 
+    imo = excluded.imo,
+    name = excluded.name, 
+    vesseltype_generic = excluded.vesseltype_generic,
+    vesseltype_detailed = excluded.vesseltype_detailed,
+    callsign = excluded.callsign,
+    flag = excluded.flag,
+    gross_tonnage = excluded.gross_tonnage,
+    summer_dwt = excluded.gross_tonnage,
+    length_breadth = excluded.length_breadth,
+    year_built = excluded.year_built,
+    home_port = excluded.home_port;
```

## aisdb/aisdb_sql/select_columns_static.sql

 * *Ordering differences only*

```diff
@@ -1,18 +1,18 @@
-SELECT
-    s.mmsi,
-    s.imo,
-    TRIM(vessel_name) as vessel_name,
-    s.ship_type,
-    s.call_sign,
-    s.dim_bow,
-    s.dim_stern,
-    s.dim_port,
-    s.dim_star,
-    s.draught, 
-    s.destination,
-    s.eta_month, 
-    s.eta_hour,
-    s.eta_day, 
-    s.eta_minute
-FROM ais_{}_static AS s
-WHERE s.mmsi = $7 ;
+SELECT
+    s.mmsi,
+    s.imo,
+    TRIM(vessel_name) as vessel_name,
+    s.ship_type,
+    s.call_sign,
+    s.dim_bow,
+    s.dim_stern,
+    s.dim_port,
+    s.dim_star,
+    s.draught, 
+    s.destination,
+    s.eta_month, 
+    s.eta_hour,
+    s.eta_day, 
+    s.eta_minute
+FROM ais_{}_static AS s
+WHERE s.mmsi = $7 ;
```

## aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql

 * *Ordering differences only*

```diff
@@ -1,20 +1,20 @@
-SELECT 
-    dynamic_{}.mmsi, 
-    dynamic_{}.time,
-    dynamic_{}.longitude,
-    dynamic_{}.latitude,
-    dynamic_{}.sog,
-    dynamic_{}.cog,
-    static_{}.imo,
-    static_{}.vessel_name,
-    static_{}.dim_bow,
-    static_{}.dim_stern,
-    static_{}.dim_port,
-    static_{}.dim_star,
-    static_{}.ship_type,
-    ref.coarse_type_txt AS ship_type_txt
-  FROM dynamic_{}
-  LEFT JOIN static_{} ON 
-    dynamic_{}.mmsi = static_{}.mmsi
-  LEFT JOIN ref ON 
-    static_{}.ship_type = ref.coarse_type
+SELECT 
+    dynamic_{}.mmsi, 
+    dynamic_{}.time,
+    dynamic_{}.longitude,
+    dynamic_{}.latitude,
+    dynamic_{}.sog,
+    dynamic_{}.cog,
+    static_{}.imo,
+    static_{}.vessel_name,
+    static_{}.dim_bow,
+    static_{}.dim_stern,
+    static_{}.dim_port,
+    static_{}.dim_star,
+    static_{}.ship_type,
+    ref.coarse_type_txt AS ship_type_txt
+  FROM dynamic_{}
+  LEFT JOIN static_{} ON 
+    dynamic_{}.mmsi = static_{}.mmsi
+  LEFT JOIN ref ON 
+    static_{}.ship_type = ref.coarse_type
```

## aisdb/aisdb_sql/select_merged_all.sql

 * *Ordering differences only*

```diff
@@ -1,29 +1,29 @@
-SELECT 
-    dynamic_{}.mmsi, 
-    dynamic_{}.time,
-    dynamic_{}.longitude,
-    dynamic_{}.latitude,
-    dynamic_{}.sog,
-    dynamic_{}.cog,
-    static_{}.imo,
-    static_{}.vessel_name,
-    static_{}.dim_bow,
-    static_{}.dim_stern,
-    static_{}.dim_port,
-    static_{}.dim_star,
-    static_{}.ship_type,
-    ref.coarse_type_txt AS ship_type_txt,
-    webdata_marinetraffic.name as vessel_name2,
-    webdata_marinetraffic.vesseltype_generic,
-    webdata_marinetraffic.vesseltype_detailed,
-    webdata_marinetraffic.gross_tonnage,
-    webdata_marinetraffic.summer_dwt, 
-    webdata_marinetraffic.length_breadth, 
-    webdata_marinetraffic.year_built
-  FROM dynamic_{}
-  LEFT JOIN static_{} ON 
-    dynamic_{}.mmsi = static_{}.mmsi
-  LEFT JOIN ref ON 
-    static_{}.ship_type = ref.coarse_type
-  LEFT JOIN webdata_marinetraffic ON
-    dynamic_{}.mmsi = webdata_marinetraffic.mmsi
+SELECT 
+    dynamic_{}.mmsi, 
+    dynamic_{}.time,
+    dynamic_{}.longitude,
+    dynamic_{}.latitude,
+    dynamic_{}.sog,
+    dynamic_{}.cog,
+    static_{}.imo,
+    static_{}.vessel_name,
+    static_{}.dim_bow,
+    static_{}.dim_stern,
+    static_{}.dim_port,
+    static_{}.dim_star,
+    static_{}.ship_type,
+    ref.coarse_type_txt AS ship_type_txt,
+    webdata_marinetraffic.name as vessel_name2,
+    webdata_marinetraffic.vesseltype_generic,
+    webdata_marinetraffic.vesseltype_detailed,
+    webdata_marinetraffic.gross_tonnage,
+    webdata_marinetraffic.summer_dwt, 
+    webdata_marinetraffic.length_breadth, 
+    webdata_marinetraffic.year_built
+  FROM dynamic_{}
+  LEFT JOIN static_{} ON 
+    dynamic_{}.mmsi = static_{}.mmsi
+  LEFT JOIN ref ON 
+    static_{}.ship_type = ref.coarse_type
+  LEFT JOIN webdata_marinetraffic ON
+    dynamic_{}.mmsi = webdata_marinetraffic.mmsi
```

## aisdb/aisdb_sql/select_static_join_webdata.sql

 * *Ordering differences only*

```diff
@@ -1,19 +1,19 @@
-SELECT
-    d_{}.mmsi,
-    --ais_{}_static.imo,
-    --ais_{}_static.vessel_name,
-    --coarsetype_ref.coarse_type_txt AS ship_type_txt,
-    webdata_marinetraffic.name as vessel_name2,
-    webdata_marinetraffic.vesseltype_generic,
-    webdata_marinetraffic.vesseltype_detailed,
-    webdata_marinetraffic.flag,
-    webdata_marinetraffic.gross_tonnage,
-    webdata_marinetraffic.summer_dwt, 
-    webdata_marinetraffic.length_breadth, 
-    webdata_marinetraffic.year_built
-  FROM (
-    SELECT DISTINCT mmsi FROM ais_{}_dynamic
-  ) as d_{}
-  LEFT JOIN webdata_marinetraffic ON
-    d_{}.mmsi = webdata_marinetraffic.mmsi
-  WHERE webdata_marinetraffic.error404 != 1
+SELECT
+    d_{}.mmsi,
+    --ais_{}_static.imo,
+    --ais_{}_static.vessel_name,
+    --coarsetype_ref.coarse_type_txt AS ship_type_txt,
+    webdata_marinetraffic.name as vessel_name2,
+    webdata_marinetraffic.vesseltype_generic,
+    webdata_marinetraffic.vesseltype_detailed,
+    webdata_marinetraffic.flag,
+    webdata_marinetraffic.gross_tonnage,
+    webdata_marinetraffic.summer_dwt, 
+    webdata_marinetraffic.length_breadth, 
+    webdata_marinetraffic.year_built
+  FROM (
+    SELECT DISTINCT mmsi FROM ais_{}_dynamic
+  ) as d_{}
+  LEFT JOIN webdata_marinetraffic ON
+    d_{}.mmsi = webdata_marinetraffic.mmsi
+  WHERE webdata_marinetraffic.error404 != 1
```

## aisdb/database/create_tables.py

 * *Ordering differences only*

```diff
@@ -1,135 +1,135 @@
-import os
-from collections import Counter
-
-import numpy as np
-import warnings
-
-from aisdb.database.dbconn import DBConn
-from aisdb import sqlpath
-
-
-def sqlite_createtable_dynamicreport(dbconn, month, dbpath):
-    assert isinstance(dbconn, (DBConn)), f'not a DBConn object {dbconn}'
-    dbconn._attach(dbpath)
-    with open(os.path.join(sqlpath, 'createtable_dynamic_clustered.sql'),
-              'r') as f:
-        sql = f.read().format(month).replace(
-            f'ais_{month}', f'{dbconn._get_dbname(dbpath)}.ais_{month}')
-    dbconn.execute(sql)
-
-
-def sqlite_createtable_staticreport(dbconn, month, dbpath):
-    assert isinstance(dbconn, (DBConn)), f'not a DBConn object {dbconn}'
-    dbconn._attach(dbpath)
-    with open(os.path.join(sqlpath, 'createtable_static.sql'), 'r') as f:
-        sql = f.read().format(month).replace(
-            f'ais_{month}', f'{dbconn._get_dbname(dbpath)}.ais_{month}')
-    dbconn.execute(sql)
-
-
-def aggregate_static_msgs(dbconn, months_str, verbose=False):
-    ''' collect an aggregate of static vessel reports for each unique MMSI
-        identifier. The most frequently repeated values for each MMSI will
-        be kept when multiple different reports appear for the same MMSI
-
-        this function should be called every time data is added to the database
-
-        args:
-            dbconn (:class:`aisdb.database.dbconn.DBConn`)
-                database connection object
-            months_str (array)
-                array of strings with format: YYYYmm
-            verbose (bool)
-                logs messages to stdout
-    '''
-
-    if not isinstance(dbconn, DBConn):  # pragma: no cover
-        raise ValueError('db argument must be a DBConn database connection')
-
-    assert not hasattr(dbconn, 'dbpath')
-    assert hasattr(dbconn, 'dbpaths')
-    assert 'main' not in dbconn.dbpaths
-
-    for dbpath in dbconn.dbpaths:
-        dbname = dbconn._get_dbname(dbpath)
-        assert dbname != 'main'
-        cur = dbconn.cursor()
-
-        for month in months_str:
-            # check for monthly tables in dbfiles containing static reports
-            cur.execute(
-                f'SELECT name FROM {dbname}.sqlite_master WHERE type="table" AND name=?',
-                [f'ais_{month}_static'])
-            if cur.fetchall() == []:
-                continue
-
-        sqlite_createtable_staticreport(dbconn, month, dbpath)
-        if verbose:
-            print('aggregating static reports into '
-                  f'{dbname}.static_{month}_aggregate...')
-        cur.execute('SELECT DISTINCT s.mmsi FROM '
-                    f'{dbname}.ais_{month}_static AS s')
-        mmsis = np.array(cur.fetchall(), dtype=int).flatten()
-
-        cur.execute('DROP TABLE IF EXISTS '
-                    f'{dbname}.static_{month}_aggregate')
-
-        #with open(os.path.join(sqlpath, 'select_columns_static.sql'), 'r') as f:
-        #    sql_select = f.read().format(month).replace( 'FROM ', f'FROM {dbname}.')
-
-        sql_select = '''
-          SELECT
-            s.mmsi, s.imo, TRIM(vessel_name) as vessel_name, s.ship_type,
-            s.call_sign, s.dim_bow, s.dim_stern, s.dim_port, s.dim_star,
-            s.draught
-          FROM ais_{}_static AS s WHERE s.mmsi = ?
-        '''.format(month).replace('FROM ', f'FROM {dbname}.')
-
-        agg_rows = []
-        for mmsi in mmsis:
-            _ = cur.execute(sql_select, (str(mmsi), ))
-            cols = np.array(cur.fetchall(), dtype=object).T
-            assert len(cols) > 0
-
-            filtercols = np.array(
-                [
-                    np.array(list(filter(None, col)), dtype=object)
-                    for col in cols
-                ],
-                dtype=object,
-            )
-
-            paddedcols = np.array(
-                [col if len(col) > 0 else [None] for col in filtercols],
-                dtype=object,
-            )
-
-            aggregated = [
-                Counter(col).most_common(1)[0][0] for col in paddedcols
-            ]
-
-            agg_rows.append(aggregated)
-
-        with open(os.path.join(sqlpath, 'createtable_static_aggregate.sql'),
-                  'r') as f:
-            sql_aggregate = f.read().format(month).replace(
-                f'static_{month}_aggregate',
-                f'{dbname}.static_{month}_aggregate')
-
-        cur.execute(sql_aggregate)
-
-        if len(agg_rows) == 0:  # pragma: no cover
-            warnings.warn('no rows to aggregate! '
-                          f'table: {dbname}.static_{month}_aggregate')
-            continue
-
-        skip_nommsi = np.array(agg_rows, dtype=object)
-        assert len(skip_nommsi.shape) == 2
-        skip_nommsi = skip_nommsi[skip_nommsi[:, 0] != None]
-        assert len(skip_nommsi) > 1
-        cur.executemany((
-            f'INSERT INTO {dbname}.static_{month}_aggregate '
-            f"VALUES ({','.join(['?' for _ in range(skip_nommsi.shape[1])])}) "
-        ), skip_nommsi)
-
-        dbconn.commit()
+import os
+from collections import Counter
+
+import numpy as np
+import warnings
+
+from aisdb.database.dbconn import DBConn
+from aisdb import sqlpath
+
+
+def sqlite_createtable_dynamicreport(dbconn, month, dbpath):
+    assert isinstance(dbconn, (DBConn)), f'not a DBConn object {dbconn}'
+    dbconn._attach(dbpath)
+    with open(os.path.join(sqlpath, 'createtable_dynamic_clustered.sql'),
+              'r') as f:
+        sql = f.read().format(month).replace(
+            f'ais_{month}', f'{dbconn._get_dbname(dbpath)}.ais_{month}')
+    dbconn.execute(sql)
+
+
+def sqlite_createtable_staticreport(dbconn, month, dbpath):
+    assert isinstance(dbconn, (DBConn)), f'not a DBConn object {dbconn}'
+    dbconn._attach(dbpath)
+    with open(os.path.join(sqlpath, 'createtable_static.sql'), 'r') as f:
+        sql = f.read().format(month).replace(
+            f'ais_{month}', f'{dbconn._get_dbname(dbpath)}.ais_{month}')
+    dbconn.execute(sql)
+
+
+def aggregate_static_msgs(dbconn, months_str, verbose=False):
+    ''' collect an aggregate of static vessel reports for each unique MMSI
+        identifier. The most frequently repeated values for each MMSI will
+        be kept when multiple different reports appear for the same MMSI
+
+        this function should be called every time data is added to the database
+
+        args:
+            dbconn (:class:`aisdb.database.dbconn.DBConn`)
+                database connection object
+            months_str (array)
+                array of strings with format: YYYYmm
+            verbose (bool)
+                logs messages to stdout
+    '''
+
+    if not isinstance(dbconn, DBConn):  # pragma: no cover
+        raise ValueError('db argument must be a DBConn database connection')
+
+    assert not hasattr(dbconn, 'dbpath')
+    assert hasattr(dbconn, 'dbpaths')
+    assert 'main' not in dbconn.dbpaths
+
+    for dbpath in dbconn.dbpaths:
+        dbname = dbconn._get_dbname(dbpath)
+        assert dbname != 'main'
+        cur = dbconn.cursor()
+
+        for month in months_str:
+            # check for monthly tables in dbfiles containing static reports
+            cur.execute(
+                f'SELECT name FROM {dbname}.sqlite_master WHERE type="table" AND name=?',
+                [f'ais_{month}_static'])
+            if cur.fetchall() == []:
+                continue
+
+        sqlite_createtable_staticreport(dbconn, month, dbpath)
+        if verbose:
+            print('aggregating static reports into '
+                  f'{dbname}.static_{month}_aggregate...')
+        cur.execute('SELECT DISTINCT s.mmsi FROM '
+                    f'{dbname}.ais_{month}_static AS s')
+        mmsis = np.array(cur.fetchall(), dtype=int).flatten()
+
+        cur.execute('DROP TABLE IF EXISTS '
+                    f'{dbname}.static_{month}_aggregate')
+
+        #with open(os.path.join(sqlpath, 'select_columns_static.sql'), 'r') as f:
+        #    sql_select = f.read().format(month).replace( 'FROM ', f'FROM {dbname}.')
+
+        sql_select = '''
+          SELECT
+            s.mmsi, s.imo, TRIM(vessel_name) as vessel_name, s.ship_type,
+            s.call_sign, s.dim_bow, s.dim_stern, s.dim_port, s.dim_star,
+            s.draught
+          FROM ais_{}_static AS s WHERE s.mmsi = ?
+        '''.format(month).replace('FROM ', f'FROM {dbname}.')
+
+        agg_rows = []
+        for mmsi in mmsis:
+            _ = cur.execute(sql_select, (str(mmsi), ))
+            cols = np.array(cur.fetchall(), dtype=object).T
+            assert len(cols) > 0
+
+            filtercols = np.array(
+                [
+                    np.array(list(filter(None, col)), dtype=object)
+                    for col in cols
+                ],
+                dtype=object,
+            )
+
+            paddedcols = np.array(
+                [col if len(col) > 0 else [None] for col in filtercols],
+                dtype=object,
+            )
+
+            aggregated = [
+                Counter(col).most_common(1)[0][0] for col in paddedcols
+            ]
+
+            agg_rows.append(aggregated)
+
+        with open(os.path.join(sqlpath, 'createtable_static_aggregate.sql'),
+                  'r') as f:
+            sql_aggregate = f.read().format(month).replace(
+                f'static_{month}_aggregate',
+                f'{dbname}.static_{month}_aggregate')
+
+        cur.execute(sql_aggregate)
+
+        if len(agg_rows) == 0:  # pragma: no cover
+            warnings.warn('no rows to aggregate! '
+                          f'table: {dbname}.static_{month}_aggregate')
+            continue
+
+        skip_nommsi = np.array(agg_rows, dtype=object)
+        assert len(skip_nommsi.shape) == 2
+        skip_nommsi = skip_nommsi[skip_nommsi[:, 0] != None]
+        assert len(skip_nommsi) > 1
+        cur.executemany((
+            f'INSERT INTO {dbname}.static_{month}_aggregate '
+            f"VALUES ({','.join(['?' for _ in range(skip_nommsi.shape[1])])}) "
+        ), skip_nommsi)
+
+        dbconn.commit()
```

## aisdb/database/dbconn.py

 * *Ordering differences only*

```diff
@@ -1,200 +1,200 @@
-''' SQLite Database connection
-
-    Also see: https://docs.python.org/3/library/sqlite3.html#connection-objects
-'''
-
-from calendar import monthrange
-from datetime import datetime
-from enum import Enum
-import os
-import re
-import warnings
-
-from aisdb import sqlite3, sqlpath
-
-import psycopg
-
-
-class _DBConn():
-    ''' AISDB Database connection handler '''
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_class, exc, tb):
-        #cur = self.cursor()
-        try:
-            for dbpath in self.dbpaths:
-                self.execute('DETACH DATABASE ?', [self._get_dbname(dbpath)])
-            #cur.close()
-        except Exception:
-            print('rolling back...')
-            self.rollback()
-        finally:
-            self.close()
-        self = None
-
-    def _create_table_coarsetype(self):
-        ''' create a table to describe integer vessel type as a human-readable
-            string.
-        '''
-        with open(os.path.join(sqlpath, 'coarsetype.sql'), 'r') as f:
-            coarsetype_sql = f.read().split(';')
-        #cur = self.cursor()
-        for stmt in coarsetype_sql:
-            if stmt == '\n':
-                continue
-            #cur.execute(stmt)
-            self.execute(stmt)
-        self.commit()
-        #cur.close()
-
-
-class SQLiteDBConn(_DBConn, sqlite3.Connection):
-    ''' SQLite3 database connection object
-
-        attributes:
-            dbpaths (list of strings)
-                list of currently attached databases
-            db_daterange (dict)
-                temporal range of monthly database tables. keys are DB file
-                names
-    '''
-
-    def __init__(self):
-        # configs
-        self.dbpaths = []
-        self.db_daterange = {}
-        super().__init__(':memory:',
-                         timeout=5,
-                         detect_types=sqlite3.PARSE_DECLTYPES
-                         | sqlite3.PARSE_COLNAMES)
-        self.row_factory = sqlite3.Row
-        self._create_table_coarsetype()
-
-    def _get_dbname(self, dbpath):
-        name_ext = os.path.split(dbpath)[1]
-        name = name_ext.split('.')[0]
-        return name
-
-    def _attach(self, dbpath):
-        ''' connect to an additional database file '''
-        assert dbpath is not None
-        dbname = self._get_dbname(dbpath)
-
-        assert dbname is not None
-        assert dbname != 'main'
-        assert dbname != 'temp'
-        assert dbname != ''
-
-        if dbpath not in self.dbpaths:
-            if os.environ.get('DEBUG'):
-                print('attaching database:', dbpath, dbname)
-            try:
-                self.execute('ATTACH ? AS ?', [dbpath, dbname])
-            except Exception as e:
-                print(f'failed: ATTACH {dbpath} AS {dbname}')
-                raise e
-            self.dbpaths.append(dbpath)
-        #cur.close()
-
-        # check if the database contains marinetraffic data
-        sql_qry_traffictable = (
-            f'SELECT * FROM {dbname}.sqlite_master '
-            'WHERE type="table" AND name = "webdata_marinetraffic"')
-        cur = self.execute(sql_qry_traffictable)
-        if len(cur.fetchall()) > 0:
-            self.trafficdb = dbpath
-        cur.close()
-
-        # query the temporal range of monthly database tables
-        # results will be stored as a dictionary attribute db_daterange
-        #cur = self.cursor()
-        sql_qry = (
-            f'SELECT * FROM {dbname}.sqlite_master '
-            'WHERE type="table" AND name LIKE "ais\\_%\\_dynamic" ESCAPE "\\" '
-        )
-        try:
-            cur = self.cursor()
-            cur.execute(sql_qry)
-            dynamic_tables = cur.fetchall()
-            if dynamic_tables != []:
-                db_months = sorted(
-                    [table['name'].split('_')[1] for table in dynamic_tables])
-                self.db_daterange[dbname] = {
-                    'start':
-                    datetime(int(db_months[0][:4]), int(db_months[0][4:]),
-                             1).date(),
-                    'end':
-                    datetime((y := int(db_months[-1][:4])),
-                             (m := int(db_months[-1][4:])),
-                             monthrange(y, m)[1]).date(),
-                }
-        except Exception as err:
-            warnings.warn(str(err.with_traceback(None)))
-        finally:
-            cur.close()
-
-
-# default to local SQLite database
-DBConn = SQLiteDBConn
-
-
-class PostgresDBConn(_DBConn, psycopg.Connection):
-    ''' This feature requires the optional dependency psycopg for interfacing Postgres
-        databases.
-
-        The following keyword arguments are accepted by Postgres:
-        | https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-PARAMKEYWORDS
-
-        Alternatively, a connection string may be used.
-        Information on connection strings and postgres URI format can be found here:
-        | https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-CONNSTRING
-
-        Example:
-
-        .. code-block:: python
-
-            import os
-            from aisdb.database.dbconn import PostgresDBConn
-
-            # keyword arguments
-            dbconn = PostgresDBConn(
-                hostaddr='127.0.0.1',
-                user='postgres',
-                port=5432,
-                password=os.environ.get('POSTGRES_PASSWORD'),
-            )
-
-            # Alternatively, connect using a connection string:
-            dbconn = PostgresDBConn('Postgresql://localhost:5433')
-
-    '''
-
-    def __init__(self, libpq_connstring=None, **kwargs):
-        if libpq_connstring is not None:
-            self.conn = psycopg.connect(libpq_connstring)
-        else:
-            self.conn = psycopg.connect(**kwargs)
-        self.cursor = self.conn.cursor
-        self.commit = self.conn.commit
-        self.rollback = self.conn.rollback
-        self.close = self.conn.close
-        self.__repr__ = self.conn.__repr__
-        #conn = psycopg.connect(conninfo=libpq_connstring)
-        self.pgconn = self.conn.pgconn
-        #self = conn
-
-        #self.dbpaths = []
-        self.db_daterange = {}
-
-    def execute(self, sql, args=[]):
-        sql = re.sub(r'\$[0-9][0-9]*', r'%s', sql)
-        with self.cursor() as cur:
-            cur.execute(sql, args)
-
-
-class ConnectionType(Enum):
-    ''' database connection types enum. used for static type hints '''
-    SQLITE = SQLiteDBConn
-    POSTGRES = PostgresDBConn
+''' SQLite Database connection
+
+    Also see: https://docs.python.org/3/library/sqlite3.html#connection-objects
+'''
+
+from calendar import monthrange
+from datetime import datetime
+from enum import Enum
+import os
+import re
+import warnings
+
+from aisdb import sqlite3, sqlpath
+
+import psycopg
+
+
+class _DBConn():
+    ''' AISDB Database connection handler '''
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_class, exc, tb):
+        #cur = self.cursor()
+        try:
+            for dbpath in self.dbpaths:
+                self.execute('DETACH DATABASE ?', [self._get_dbname(dbpath)])
+            #cur.close()
+        except Exception:
+            print('rolling back...')
+            self.rollback()
+        finally:
+            self.close()
+        self = None
+
+    def _create_table_coarsetype(self):
+        ''' create a table to describe integer vessel type as a human-readable
+            string.
+        '''
+        with open(os.path.join(sqlpath, 'coarsetype.sql'), 'r') as f:
+            coarsetype_sql = f.read().split(';')
+        #cur = self.cursor()
+        for stmt in coarsetype_sql:
+            if stmt == '\n':
+                continue
+            #cur.execute(stmt)
+            self.execute(stmt)
+        self.commit()
+        #cur.close()
+
+
+class SQLiteDBConn(_DBConn, sqlite3.Connection):
+    ''' SQLite3 database connection object
+
+        attributes:
+            dbpaths (list of strings)
+                list of currently attached databases
+            db_daterange (dict)
+                temporal range of monthly database tables. keys are DB file
+                names
+    '''
+
+    def __init__(self):
+        # configs
+        self.dbpaths = []
+        self.db_daterange = {}
+        super().__init__(':memory:',
+                         timeout=5,
+                         detect_types=sqlite3.PARSE_DECLTYPES
+                         | sqlite3.PARSE_COLNAMES)
+        self.row_factory = sqlite3.Row
+        self._create_table_coarsetype()
+
+    def _get_dbname(self, dbpath):
+        name_ext = os.path.split(dbpath)[1]
+        name = name_ext.split('.')[0]
+        return name
+
+    def _attach(self, dbpath):
+        ''' connect to an additional database file '''
+        assert dbpath is not None
+        dbname = self._get_dbname(dbpath)
+
+        assert dbname is not None
+        assert dbname != 'main'
+        assert dbname != 'temp'
+        assert dbname != ''
+
+        if dbpath not in self.dbpaths:
+            if os.environ.get('DEBUG'):
+                print('attaching database:', dbpath, dbname)
+            try:
+                self.execute('ATTACH ? AS ?', [dbpath, dbname])
+            except Exception as e:
+                print(f'failed: ATTACH {dbpath} AS {dbname}')
+                raise e
+            self.dbpaths.append(dbpath)
+        #cur.close()
+
+        # check if the database contains marinetraffic data
+        sql_qry_traffictable = (
+            f'SELECT * FROM {dbname}.sqlite_master '
+            'WHERE type="table" AND name = "webdata_marinetraffic"')
+        cur = self.execute(sql_qry_traffictable)
+        if len(cur.fetchall()) > 0:
+            self.trafficdb = dbpath
+        cur.close()
+
+        # query the temporal range of monthly database tables
+        # results will be stored as a dictionary attribute db_daterange
+        #cur = self.cursor()
+        sql_qry = (
+            f'SELECT * FROM {dbname}.sqlite_master '
+            'WHERE type="table" AND name LIKE "ais\\_%\\_dynamic" ESCAPE "\\" '
+        )
+        try:
+            cur = self.cursor()
+            cur.execute(sql_qry)
+            dynamic_tables = cur.fetchall()
+            if dynamic_tables != []:
+                db_months = sorted(
+                    [table['name'].split('_')[1] for table in dynamic_tables])
+                self.db_daterange[dbname] = {
+                    'start':
+                    datetime(int(db_months[0][:4]), int(db_months[0][4:]),
+                             1).date(),
+                    'end':
+                    datetime((y := int(db_months[-1][:4])),
+                             (m := int(db_months[-1][4:])),
+                             monthrange(y, m)[1]).date(),
+                }
+        except Exception as err:
+            warnings.warn(str(err.with_traceback(None)))
+        finally:
+            cur.close()
+
+
+# default to local SQLite database
+DBConn = SQLiteDBConn
+
+
+class PostgresDBConn(_DBConn, psycopg.Connection):
+    ''' This feature requires the optional dependency psycopg for interfacing Postgres
+        databases.
+
+        The following keyword arguments are accepted by Postgres:
+        | https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-PARAMKEYWORDS
+
+        Alternatively, a connection string may be used.
+        Information on connection strings and postgres URI format can be found here:
+        | https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-CONNSTRING
+
+        Example:
+
+        .. code-block:: python
+
+            import os
+            from aisdb.database.dbconn import PostgresDBConn
+
+            # keyword arguments
+            dbconn = PostgresDBConn(
+                hostaddr='127.0.0.1',
+                user='postgres',
+                port=5432,
+                password=os.environ.get('POSTGRES_PASSWORD'),
+            )
+
+            # Alternatively, connect using a connection string:
+            dbconn = PostgresDBConn('Postgresql://localhost:5433')
+
+    '''
+
+    def __init__(self, libpq_connstring=None, **kwargs):
+        if libpq_connstring is not None:
+            self.conn = psycopg.connect(libpq_connstring)
+        else:
+            self.conn = psycopg.connect(**kwargs)
+        self.cursor = self.conn.cursor
+        self.commit = self.conn.commit
+        self.rollback = self.conn.rollback
+        self.close = self.conn.close
+        self.__repr__ = self.conn.__repr__
+        #conn = psycopg.connect(conninfo=libpq_connstring)
+        self.pgconn = self.conn.pgconn
+        #self = conn
+
+        #self.dbpaths = []
+        self.db_daterange = {}
+
+    def execute(self, sql, args=[]):
+        sql = re.sub(r'\$[0-9][0-9]*', r'%s', sql)
+        with self.cursor() as cur:
+            cur.execute(sql, args)
+
+
+class ConnectionType(Enum):
+    ''' database connection types enum. used for static type hints '''
+    SQLITE = SQLiteDBConn
+    POSTGRES = PostgresDBConn
```

## aisdb/database/dbqry.py

 * *Ordering differences only*

```diff
@@ -1,277 +1,277 @@
-''' class to convert a dictionary of input parameters into SQL code, and
-    generate queries
-'''
-
-from collections import UserDict
-from datetime import datetime, timedelta, date
-from functools import reduce
-import warnings
-
-import numpy as np
-
-from aisdb.database import sqlfcn, sqlfcn_callbacks
-from aisdb.database.create_tables import (aggregate_static_msgs,
-                                          sqlite_createtable_dynamicreport,
-                                          sqlite_createtable_staticreport)
-from aisdb.database.dbconn import ConnectionType
-from aisdb.webdata.marinetraffic import VesselInfo
-
-
-class DBQuery(UserDict):
-    ''' A database abstraction allowing the creation of SQL code via arguments
-        passed to __init__(). Args are stored as a dictionary (UserDict).
-
-        Args:
-            dbconn (:class:`aisdb.database.dbconn.DBConn`)
-                database connection object
-            dbpath (string)
-                database filepath to connect to
-            dbpaths (list)
-                optionally pass a list of filepaths instead of a single dbpath
-            callback (function)
-                anonymous function yielding SQL code specifying "WHERE"
-                clauses. common queries are included in
-                :mod:`aisdb.database.sqlfcn_callbacks`, e.g.
-                >>> from aisdb.database.sqlfcn_callbacks import in_timerange_validmmsi
-                >>> callback = in_timerange_validmmsi
-
-                this generates SQL code to apply filtering on columns (mmsi,
-                time), and requires (start, end) as arguments in datetime
-                format.
-
-            **kwargs (dict)
-                more arguments that will be supplied to the query function
-                and callback function
-
-
-        Custom SQL queries are supported by modifying the fcn supplied to
-        .gen_qry() and .async_qry(), or by supplying a callback function.
-        Alternatively, the database can also be queried directly, see
-        DBConn.py for more info
-
-        complete example:
-
-        >>> import os
-        >>> from datetime import datetime
-        >>> from aisdb import DBConn, DBQuery, decode_msgs
-        >>> from aisdb.database.sqlfcn_callbacks import in_timerange_validmmsi
-
-        >>> dbpath = './testdata/test.db'
-        >>> start, end = datetime(2021, 7, 1), datetime(2021, 7, 7)
-        >>> filepaths = ['aisdb/tests/testdata/test_data_20210701.csv',
-        ...              'aisdb/tests/testdata/test_data_20211101.nm4']
-        >>> with DBConn() as dbconn:
-        ...     decode_msgs(filepaths=filepaths, dbconn=dbconn, dbpath=dbpath,
-        ...     source='TESTING')
-        ...     q = DBQuery(dbconn=dbconn,
-        ...                 dbpath=dbpath,
-        ...                 callback=in_timerange_validmmsi,
-        ...                 start=start,
-        ...                 end=end)
-        ...     for rows in q.gen_qry():
-        ...         print(str(dict(rows[0])))
-        ...         break
-        {'mmsi': 204242000, 'time': 1625176725, 'longitude': -8.93166666667, 'latitude': 41.45, 'sog': 4.0, 'cog': 176.0}
-    '''
-
-    def __init__(self, *, dbconn, dbpath=None, dbpaths=[], **kwargs):
-        if isinstance(dbconn, ConnectionType.SQLITE.value):
-            if dbpaths == [] and dbpath is None:
-                raise ValueError(
-                    'must supply either dbpaths list or dbpath string value')
-            elif dbpaths == []:  # pragma: no cover
-                dbpaths = [dbpath]
-        elif isinstance(dbconn, ConnectionType.POSTGRES):
-            if dbpath is not None:
-                raise ValueError(
-                    "the dbpath argument may not be used with a Postgres connection"
-                )
-        else:
-            raise ValueError("Invalid database connection")
-
-        for dbpath in dbpaths:
-            dbconn._attach(dbpath)
-        if isinstance(dbconn, ConnectionType):
-            raise ValueError('Invalid database connection.'
-                             f' Got: {dbconn}.'
-                             f'Requires: {ConnectionType.SQLITE.value}'
-                             f' or {ConnectionType.POSTGRES.value}')
-
-        self.data = kwargs
-        self.dbconn = dbconn
-        self.create_qry_params()
-
-    def create_qry_params(self):
-        assert 'start' in self.data.keys() and 'end' in self.data.keys()
-        if self.data['start'] >= self.data['end']:
-            raise ValueError('Start must occur before end')
-        assert isinstance(self.data['start'], (datetime, date))
-        self.data.update({'months': sqlfcn_callbacks.dt2monthstr(**self.data)})
-
-    def check_marinetraffic(self,
-                            dbpath,
-                            trafficDBpath,
-                            boundary,
-                            retry_404=False):
-        ''' scrape metadata for vessels in domain from marinetraffic
-
-            args:
-                dbpath (string)
-                    database file path
-                trafficDBpath (string)
-                    marinetraffic database path
-                boundary (dict)
-                    uses keys xmin, xmax, ymin, and ymax to denote the region
-                    of vessels that should be checked.
-                    if using :class:`aisdb.gis.Domain`, the `Domain.boundary`
-                    attribute can be supplied here
-        '''
-        self.dbconn._attach(dbpath)
-        vinfo = VesselInfo(trafficDBpath)
-        # TODO: determine which attached db to query
-
-        print(f'retrieving vessel info for {dbpath}', end='', flush=True)
-        for month in self.data['months']:
-            dbname = self.dbconn._get_dbname(dbpath)
-            self.dbconn._attach(dbpath)
-
-            # skip missing tables
-            if self.dbconn.execute(
-                (f'SELECT * FROM {dbname}.sqlite_master '
-                 'WHERE type="table" and name=?'),
-                [f'ais_{month}_dynamic']).fetchall() == 0:  # pragma: no cover
-                continue
-
-            # check unique mmsis
-            sql = (
-                'SELECT DISTINCT(mmsi) '
-                f'FROM {dbname}.ais_{month}_dynamic AS d WHERE '
-                f'{sqlfcn_callbacks.in_validmmsi_bbox(alias="d", **boundary)}')
-            mmsis = self.dbconn.execute(sql).fetchall()
-            print('.', end='', flush=True)  # first dot
-
-            # retrieve vessel metadata
-            if len(mmsis) > 0:  # pragma: no cover
-                # not covered due to caching used for testing
-                vinfo.vessel_info_callback(mmsis=np.array(mmsis),
-                                           retry_404=retry_404,
-                                           infotxt=f'{month} ')
-
-    def gen_qry(self,
-                fcn=sqlfcn.crawl_dynamic,
-                reaggregate_static=False,
-                verbose=False):
-        ''' queries the database using the supplied SQL function and dbpath.
-            generator only stores one item at at time before yielding
-
-            args:
-                self (UserDict)
-                    dictionary containing kwargs
-                dbpath (string)
-                    database location. defaults to the path configured
-                    in ~/.config/ais.cfg
-                fcn (function)
-                    callback function that will generate SQL code using
-                    the args stored in self
-                verbose (bool)
-                    log info to stdout
-
-            yields:
-                numpy array of rows for each unique MMSI
-                arrays are sorted by MMSI
-                rows are sorted by time
-        '''
-
-        # initialize dbconn, run query
-        assert 'dbpath' not in self.data.keys()
-        cur = self.dbconn.cursor()
-
-        for dbpath in self.dbconn.dbpaths:
-            if self.dbconn._get_dbname(dbpath) not in self.dbconn.db_daterange:
-                continue
-            db_rng = self.dbconn.db_daterange[self.dbconn._get_dbname(dbpath)]
-            if self['start'].date() > db_rng['end'] or self['end'].date(
-            ) < db_rng['start']:
-                if verbose:
-                    print(f'skipping query for {dbpath} (out of timerange)...')
-                continue
-            for month in self.data['months']:
-
-                month_date = datetime(int(month[:4]), int(month[4:]), 1)
-                qry_start = self["start"] - timedelta(days=self["start"].day)
-                assert qry_start <= month_date <= self[
-                    'end'], f'{month_date} not in range ({qry_start}->{self["end"]})'
-
-                rng_string = f'{db_rng["start"].year}-{db_rng["start"].month:02d}-{db_rng["start"].day:02d}'
-                rng_string += ' -> '
-                rng_string += f'{db_rng["end"].year}-{db_rng["end"].month:02d}-{db_rng["end"].day:02d}'
-
-                # check if static tables exist
-                cur.execute(
-                    f'SELECT * FROM {self.dbconn._get_dbname(dbpath)}.sqlite_master '
-                    'WHERE type="table" AND name=?', [f'ais_{month}_static'])
-                if len(cur.fetchall()) == 0:
-                    #sqlite_createtable_staticreport(self.dbconn, month, dbpath)
-                    warnings.warn('No static data for selected time range! '
-                                  f'{self.dbconn._get_dbname(dbpath)} '
-                                  f'{rng_string}')
-
-                # check if aggregate tables exist
-                cur.execute((
-                    f'SELECT * FROM {self.dbconn._get_dbname(dbpath)}.sqlite_master '
-                    'WHERE type="table" and name=?'),
-                            [f'static_{month}_aggregate'])
-                res = cur.fetchall()
-
-                if len(res) == 0 or reaggregate_static:
-                    if verbose:
-                        print(f'building static index for month {month}...',
-                              flush=True)
-                    aggregate_static_msgs(self.dbconn, [month], verbose)
-
-                # check if dynamic tables exist
-                cur.execute(
-                    f'SELECT * FROM {self.dbconn._get_dbname(dbpath)}.sqlite_master WHERE '
-                    'type="table" and name=?', [f'ais_{month}_dynamic'])
-                if len(cur.fetchall()) == 0:  # pragma: no cover
-                    if isinstance(self.dbconn, ConnectionType.SQLITE.value):
-                        sqlite_createtable_dynamicreport(
-                            self.dbconn, month, dbpath)
-
-                    warnings.warn('No data for selected time range! '
-                                  f'{self.dbconn._get_dbname(dbpath)} '
-                                  f'{rng_string}')
-
-            qry = fcn(dbpath=dbpath, **self.data)
-            if verbose:
-                print(qry)
-
-            # get 500k rows at a time, yield sets of rows for each unique MMSI
-            mmsi_rows = []
-            dt = datetime.now()
-            #cur = self.dbconn.cursor()
-            _ = cur.execute(qry)
-            res = cur.fetchmany(10**5)
-            delta = datetime.now() - dt
-            if verbose:
-                print(
-                    f'query time: {delta.total_seconds():.2f}s\nfetching rows...'
-                )
-            if res == []:
-                # raise SyntaxError(f'no results for query!\n{qry}')
-                warnings.warn('No results for query!')
-
-            while len(res) > 0:
-                mmsi_rows += res
-                ummsi_idx = np.where(
-                    np.array(mmsi_rows)[:-1, 0] != np.array(mmsi_rows)[1:, 0]
-                )[0] + 1
-                ummsi_idx = reduce(np.append,
-                                   ([0], ummsi_idx, [len(mmsi_rows)]))
-                for i in range(len(ummsi_idx) - 2):
-                    yield mmsi_rows[ummsi_idx[i]:ummsi_idx[i + 1]]
-                if len(ummsi_idx) > 2:
-                    mmsi_rows = mmsi_rows[ummsi_idx[i + 1]:]
-
-                res = cur.fetchmany(10**5)
-            yield mmsi_rows
+''' class to convert a dictionary of input parameters into SQL code, and
+    generate queries
+'''
+
+from collections import UserDict
+from datetime import datetime, timedelta, date
+from functools import reduce
+import warnings
+
+import numpy as np
+
+from aisdb.database import sqlfcn, sqlfcn_callbacks
+from aisdb.database.create_tables import (aggregate_static_msgs,
+                                          sqlite_createtable_dynamicreport,
+                                          sqlite_createtable_staticreport)
+from aisdb.database.dbconn import ConnectionType
+from aisdb.webdata.marinetraffic import VesselInfo
+
+
+class DBQuery(UserDict):
+    ''' A database abstraction allowing the creation of SQL code via arguments
+        passed to __init__(). Args are stored as a dictionary (UserDict).
+
+        Args:
+            dbconn (:class:`aisdb.database.dbconn.DBConn`)
+                database connection object
+            dbpath (string)
+                database filepath to connect to
+            dbpaths (list)
+                optionally pass a list of filepaths instead of a single dbpath
+            callback (function)
+                anonymous function yielding SQL code specifying "WHERE"
+                clauses. common queries are included in
+                :mod:`aisdb.database.sqlfcn_callbacks`, e.g.
+                >>> from aisdb.database.sqlfcn_callbacks import in_timerange_validmmsi
+                >>> callback = in_timerange_validmmsi
+
+                this generates SQL code to apply filtering on columns (mmsi,
+                time), and requires (start, end) as arguments in datetime
+                format.
+
+            **kwargs (dict)
+                more arguments that will be supplied to the query function
+                and callback function
+
+
+        Custom SQL queries are supported by modifying the fcn supplied to
+        .gen_qry() and .async_qry(), or by supplying a callback function.
+        Alternatively, the database can also be queried directly, see
+        DBConn.py for more info
+
+        complete example:
+
+        >>> import os
+        >>> from datetime import datetime
+        >>> from aisdb import DBConn, DBQuery, decode_msgs
+        >>> from aisdb.database.sqlfcn_callbacks import in_timerange_validmmsi
+
+        >>> dbpath = './testdata/test.db'
+        >>> start, end = datetime(2021, 7, 1), datetime(2021, 7, 7)
+        >>> filepaths = ['aisdb/tests/testdata/test_data_20210701.csv',
+        ...              'aisdb/tests/testdata/test_data_20211101.nm4']
+        >>> with DBConn() as dbconn:
+        ...     decode_msgs(filepaths=filepaths, dbconn=dbconn, dbpath=dbpath,
+        ...     source='TESTING')
+        ...     q = DBQuery(dbconn=dbconn,
+        ...                 dbpath=dbpath,
+        ...                 callback=in_timerange_validmmsi,
+        ...                 start=start,
+        ...                 end=end)
+        ...     for rows in q.gen_qry():
+        ...         print(str(dict(rows[0])))
+        ...         break
+        {'mmsi': 204242000, 'time': 1625176725, 'longitude': -8.93166666667, 'latitude': 41.45, 'sog': 4.0, 'cog': 176.0}
+    '''
+
+    def __init__(self, *, dbconn, dbpath=None, dbpaths=[], **kwargs):
+        if isinstance(dbconn, ConnectionType.SQLITE.value):
+            if dbpaths == [] and dbpath is None:
+                raise ValueError(
+                    'must supply either dbpaths list or dbpath string value')
+            elif dbpaths == []:  # pragma: no cover
+                dbpaths = [dbpath]
+        elif isinstance(dbconn, ConnectionType.POSTGRES):
+            if dbpath is not None:
+                raise ValueError(
+                    "the dbpath argument may not be used with a Postgres connection"
+                )
+        else:
+            raise ValueError("Invalid database connection")
+
+        for dbpath in dbpaths:
+            dbconn._attach(dbpath)
+        if isinstance(dbconn, ConnectionType):
+            raise ValueError('Invalid database connection.'
+                             f' Got: {dbconn}.'
+                             f'Requires: {ConnectionType.SQLITE.value}'
+                             f' or {ConnectionType.POSTGRES.value}')
+
+        self.data = kwargs
+        self.dbconn = dbconn
+        self.create_qry_params()
+
+    def create_qry_params(self):
+        assert 'start' in self.data.keys() and 'end' in self.data.keys()
+        if self.data['start'] >= self.data['end']:
+            raise ValueError('Start must occur before end')
+        assert isinstance(self.data['start'], (datetime, date))
+        self.data.update({'months': sqlfcn_callbacks.dt2monthstr(**self.data)})
+
+    def check_marinetraffic(self,
+                            dbpath,
+                            trafficDBpath,
+                            boundary,
+                            retry_404=False):
+        ''' scrape metadata for vessels in domain from marinetraffic
+
+            args:
+                dbpath (string)
+                    database file path
+                trafficDBpath (string)
+                    marinetraffic database path
+                boundary (dict)
+                    uses keys xmin, xmax, ymin, and ymax to denote the region
+                    of vessels that should be checked.
+                    if using :class:`aisdb.gis.Domain`, the `Domain.boundary`
+                    attribute can be supplied here
+        '''
+        self.dbconn._attach(dbpath)
+        vinfo = VesselInfo(trafficDBpath)
+        # TODO: determine which attached db to query
+
+        print(f'retrieving vessel info for {dbpath}', end='', flush=True)
+        for month in self.data['months']:
+            dbname = self.dbconn._get_dbname(dbpath)
+            self.dbconn._attach(dbpath)
+
+            # skip missing tables
+            if self.dbconn.execute(
+                (f'SELECT * FROM {dbname}.sqlite_master '
+                 'WHERE type="table" and name=?'),
+                [f'ais_{month}_dynamic']).fetchall() == 0:  # pragma: no cover
+                continue
+
+            # check unique mmsis
+            sql = (
+                'SELECT DISTINCT(mmsi) '
+                f'FROM {dbname}.ais_{month}_dynamic AS d WHERE '
+                f'{sqlfcn_callbacks.in_validmmsi_bbox(alias="d", **boundary)}')
+            mmsis = self.dbconn.execute(sql).fetchall()
+            print('.', end='', flush=True)  # first dot
+
+            # retrieve vessel metadata
+            if len(mmsis) > 0:  # pragma: no cover
+                # not covered due to caching used for testing
+                vinfo.vessel_info_callback(mmsis=np.array(mmsis),
+                                           retry_404=retry_404,
+                                           infotxt=f'{month} ')
+
+    def gen_qry(self,
+                fcn=sqlfcn.crawl_dynamic,
+                reaggregate_static=False,
+                verbose=False):
+        ''' queries the database using the supplied SQL function and dbpath.
+            generator only stores one item at at time before yielding
+
+            args:
+                self (UserDict)
+                    dictionary containing kwargs
+                dbpath (string)
+                    database location. defaults to the path configured
+                    in ~/.config/ais.cfg
+                fcn (function)
+                    callback function that will generate SQL code using
+                    the args stored in self
+                verbose (bool)
+                    log info to stdout
+
+            yields:
+                numpy array of rows for each unique MMSI
+                arrays are sorted by MMSI
+                rows are sorted by time
+        '''
+
+        # initialize dbconn, run query
+        assert 'dbpath' not in self.data.keys()
+        cur = self.dbconn.cursor()
+
+        for dbpath in self.dbconn.dbpaths:
+            if self.dbconn._get_dbname(dbpath) not in self.dbconn.db_daterange:
+                continue
+            db_rng = self.dbconn.db_daterange[self.dbconn._get_dbname(dbpath)]
+            if self['start'].date() > db_rng['end'] or self['end'].date(
+            ) < db_rng['start']:
+                if verbose:
+                    print(f'skipping query for {dbpath} (out of timerange)...')
+                continue
+            for month in self.data['months']:
+
+                month_date = datetime(int(month[:4]), int(month[4:]), 1)
+                qry_start = self["start"] - timedelta(days=self["start"].day)
+                assert qry_start <= month_date <= self[
+                    'end'], f'{month_date} not in range ({qry_start}->{self["end"]})'
+
+                rng_string = f'{db_rng["start"].year}-{db_rng["start"].month:02d}-{db_rng["start"].day:02d}'
+                rng_string += ' -> '
+                rng_string += f'{db_rng["end"].year}-{db_rng["end"].month:02d}-{db_rng["end"].day:02d}'
+
+                # check if static tables exist
+                cur.execute(
+                    f'SELECT * FROM {self.dbconn._get_dbname(dbpath)}.sqlite_master '
+                    'WHERE type="table" AND name=?', [f'ais_{month}_static'])
+                if len(cur.fetchall()) == 0:
+                    #sqlite_createtable_staticreport(self.dbconn, month, dbpath)
+                    warnings.warn('No static data for selected time range! '
+                                  f'{self.dbconn._get_dbname(dbpath)} '
+                                  f'{rng_string}')
+
+                # check if aggregate tables exist
+                cur.execute((
+                    f'SELECT * FROM {self.dbconn._get_dbname(dbpath)}.sqlite_master '
+                    'WHERE type="table" and name=?'),
+                            [f'static_{month}_aggregate'])
+                res = cur.fetchall()
+
+                if len(res) == 0 or reaggregate_static:
+                    if verbose:
+                        print(f'building static index for month {month}...',
+                              flush=True)
+                    aggregate_static_msgs(self.dbconn, [month], verbose)
+
+                # check if dynamic tables exist
+                cur.execute(
+                    f'SELECT * FROM {self.dbconn._get_dbname(dbpath)}.sqlite_master WHERE '
+                    'type="table" and name=?', [f'ais_{month}_dynamic'])
+                if len(cur.fetchall()) == 0:  # pragma: no cover
+                    if isinstance(self.dbconn, ConnectionType.SQLITE.value):
+                        sqlite_createtable_dynamicreport(
+                            self.dbconn, month, dbpath)
+
+                    warnings.warn('No data for selected time range! '
+                                  f'{self.dbconn._get_dbname(dbpath)} '
+                                  f'{rng_string}')
+
+            qry = fcn(dbpath=dbpath, **self.data)
+            if verbose:
+                print(qry)
+
+            # get 500k rows at a time, yield sets of rows for each unique MMSI
+            mmsi_rows = []
+            dt = datetime.now()
+            #cur = self.dbconn.cursor()
+            _ = cur.execute(qry)
+            res = cur.fetchmany(10**5)
+            delta = datetime.now() - dt
+            if verbose:
+                print(
+                    f'query time: {delta.total_seconds():.2f}s\nfetching rows...'
+                )
+            if res == []:
+                # raise SyntaxError(f'no results for query!\n{qry}')
+                warnings.warn('No results for query!')
+
+            while len(res) > 0:
+                mmsi_rows += res
+                ummsi_idx = np.where(
+                    np.array(mmsi_rows)[:-1, 0] != np.array(mmsi_rows)[1:, 0]
+                )[0] + 1
+                ummsi_idx = reduce(np.append,
+                                   ([0], ummsi_idx, [len(mmsi_rows)]))
+                for i in range(len(ummsi_idx) - 2):
+                    yield mmsi_rows[ummsi_idx[i]:ummsi_idx[i + 1]]
+                if len(ummsi_idx) > 2:
+                    mmsi_rows = mmsi_rows[ummsi_idx[i + 1]:]
+
+                res = cur.fetchmany(10**5)
+            yield mmsi_rows
```

## aisdb/database/decoder.py

 * *Ordering differences only*

```diff
@@ -1,264 +1,264 @@
-''' Parsing NMEA messages to create an SQL database.
-    See function decode_msgs() for usage
-'''
-
-from hashlib import md5
-import gzip
-import os
-import pickle
-import sqlite3
-import tempfile
-import zipfile
-
-from aisdb.database.dbconn import SQLiteDBConn, PostgresDBConn
-from aisdb.aisdb import decoder
-
-
-class FileChecksums():
-
-    def __init__(self, *, dbconn):
-        assert isinstance(dbconn, (PostgresDBConn, SQLiteDBConn))
-        if isinstance(dbconn, SQLiteDBConn):
-            assert len(dbconn.dbpaths) == 1, f'{dbconn.dbpaths}'
-        self.dbconn = dbconn
-        self.checksums_table()
-        if not os.path.isdir(
-                '/tmp') and os.name == 'posix':  # pragma: no cover
-            os.mkdir('/tmp')
-        self.tmp_dir = tempfile.mkdtemp()
-
-    def checksums_table(self):
-        ''' instantiates new database connection and creates a checksums
-            hashmap table if it doesn't exist yet.
-
-            creates a temporary directory with a path stored in ``self.tmp_dir``
-
-            creates SQLite connection attribute ``self.dbconn``, which should
-            be closed after use
-
-            e.g.
-                self.dbconn.close()
-        '''
-        # self.dbconn = sqlite3.connect(self.dbpath)
-        if isinstance(self.dbconn, SQLiteDBConn):
-            dbconn = sqlite3.connect(self.dbconn.dbpaths[0])
-            cur = dbconn.cursor()
-            cur.execute('''
-                CREATE TABLE IF NOT EXISTS
-                hashmap(
-                    hash INTEGER PRIMARY KEY,
-                    bytes BLOB
-                )
-                WITHOUT ROWID;''')
-            cur.execute('CREATE UNIQUE INDEX '
-                        'IF NOT EXISTS '
-                        'idx_map on hashmap(hash)')
-            dbconn.close()
-        elif isinstance(self.dbconn, PostgresDBConn):
-            dbconn = self.dbconn
-            cur = self.dbconn.cursor()
-            cur.execute('''
-                CREATE TABLE IF NOT EXISTS
-                hashmap(
-                    hash TEXT PRIMARY KEY,
-                    bytes BYTEA
-                );''')
-            cur.execute('CREATE UNIQUE INDEX IF NOT EXISTS '
-                        'idx_map on hashmap(hash);')
-
-    def insert_checksum(self, checksum):
-        if isinstance(self.dbconn, SQLiteDBConn):
-            dbconn = sqlite3.connect(self.dbconn.dbpaths[0])
-        elif isinstance(self.dbconn, PostgresDBConn):
-            dbconn = self.dbconn
-        dbconn.execute('INSERT INTO hashmap VALUES (?,?)',
-                       [checksum, pickle.dumps(None)])
-        dbconn.commit()
-        if isinstance(self.dbconn, SQLiteDBConn):
-            dbconn.close()
-
-    def checksum_exists(self, checksum):
-        # dbconn = sqlite3.connect(self.dbpath)
-        # cur = dbconn.cursor()
-        if isinstance(self.dbconn, SQLiteDBConn):
-            dbconn = sqlite3.connect(self.dbconn.dbpaths[0])
-            cur = dbconn.cursor()
-            cur.execute('SELECT * FROM hashmap WHERE hash = ?', [checksum])
-        elif isinstance(self.dbconn, PostgresDBConn):
-            dbconn = self.dbconn
-            cur = self.dbconn.cursor()
-            cur.execute('SELECT * FROM hashmap WHERE hash = %s', [checksum])
-        res = cur.fetchone()
-        dbconn.commit()
-        # dbconn.close()
-        if isinstance(self.dbconn, SQLiteDBConn):
-            dbconn.close()
-
-        if res is None or res is False:
-            return False
-        return True
-
-    def get_md5(self, path, f):
-        ''' get md5 hash from the first kilobyte of data '''
-        # skip header row in CSV format(~1.6kb)
-        if path[-4:].lower() == '.csv':
-            _ = f.read(1600)
-        signature = md5(f.read(1000)).hexdigest()
-        return signature
-
-
-def _decode_gz(file, tmp_dir, dbpath, psql_conn_string, source, verbose):
-    if dbpath is None:  # pragma: no cover
-        dbpath = ''
-    if psql_conn_string is None:  # pragma: no cover
-        psql_conn_string = ''
-    unzip_file = os.path.join(tmp_dir, file.rsplit(os.path.sep, 1)[-1][:-3])
-    with gzip.open(file, 'rb') as f1, open(unzip_file, 'wb') as f2:
-        f2.write(f1.read())
-    decoder(dbpath=dbpath,
-            psql_conn_string=psql_conn_string,
-            files=[unzip_file],
-            source=source,
-            verbose=verbose)
-    os.remove(unzip_file)
-
-
-def _decode_ziparchive(file, tmp_dir, dbpath, psql_conn_string, source,
-                       verbose):
-    if dbpath is None:  # pragma: no cover
-        dbpath = ''
-    if psql_conn_string is None:  # pragma: no cover
-        psql_conn_string = ''
-    zipf = zipfile.ZipFile(file)
-    for item in zipf.namelist():
-        unzip_file = os.path.join(tmp_dir, item)
-        with zipf.open(item, 'r') as f1, open(unzip_file, 'wb') as f2:
-            f2.write(f1.read())
-        decoder(dbpath=dbpath,
-                psql_conn_string=psql_conn_string,
-                files=[unzip_file],
-                source=source,
-                verbose=verbose)
-        os.remove(unzip_file)
-    zipf.close()
-
-
-def decode_msgs(filepaths,
-                dbconn,
-                source,
-                dbpath=None,
-                psql_conn_string=None,
-                vacuum=False,
-                skip_checksum=False,
-                verbose=False):
-    ''' Decode NMEA format AIS messages and store in an SQLite database.
-        To speed up decoding, create the database on a different hard drive
-        from where the raw data is stored.
-        A checksum of the first kilobyte of every file will be stored to
-        prevent loading the same file twice.
-
-        If the filepath has a .gz or .zip extension, the file will be
-        decompressed into a temporary directory before database insert.
-
-        args:
-            filepaths (list)
-                absolute filepath locations for AIS message files to be
-                ingested into the database
-            dbconn (:class:`aisdb.database.dbconn.DBConn`)
-                database connection object
-            dbpath (string)
-                SQLite database filepath to store results in. If dbconn is a
-                Postgres database connection, set this to ``None``.
-            psql_conn_string (string)
-                Postgres connection string. If dbconn is an SQLite database
-                connection, set this to ``None``.
-            source (string)
-                data source name or description. will be used as a primary key
-                column, so duplicate messages from different sources will not
-                be ignored as duplicates upon insert
-            vacuum (boolean, str)
-                if True, the database will be vacuumed after completion.
-                if string, the database will be vacuumed into the filepath
-                given. Consider vacuuming to second hard disk to speed this up
-
-        returns:
-            None
-
-        example:
-
-
-        .. _example_decode:
-
-        >>> import os
-        >>> from aisdb import decode_msgs, DBConn
-
-        >>> dbpath = 'test_decode_msgs.db'
-        >>> filepaths = ['aisdb/tests/testdata/test_data_20210701.csv',
-        ...              'aisdb/tests/testdata/test_data_20211101.nm4']
-        >>> with DBConn() as dbconn:
-        ...     decode_msgs(filepaths=filepaths, dbconn=dbconn, dbpath=dbpath, source='TESTING')
-        >>> os.remove(dbpath)
-    '''
-    if not isinstance(dbconn,
-                      (SQLiteDBConn, PostgresDBConn)):  # pragma: no cover
-        raise ValueError('db argument must be a DBConn database connection. '
-                         f'got {dbconn}')
-
-    if len(filepaths) == 0:  # pragma: no cover
-        raise ValueError('must supply atleast one filepath.')
-
-    if isinstance(dbconn, SQLiteDBConn):
-        dbconn._attach(dbpath)
-        assert dbpath is not None
-        assert psql_conn_string is None
-        psql_conn_string = ''
-    else:
-        assert psql_conn_string is not None
-        assert dbpath is None
-        dbpath = ''
-
-    dbindex = FileChecksums(dbconn=dbconn)
-    for file in filepaths:
-        if not skip_checksum:
-            with open(os.path.abspath(file), 'rb') as f:
-                signature = dbindex.get_md5(file, f)
-            if dbindex.checksum_exists(signature):
-                if verbose:  # pragma: no cover
-                    print(f'found matching checksum, skipping {file}')
-                continue
-        if file[-3:] == '.gz':
-            _decode_gz(file,
-                       dbindex.tmp_dir,
-                       source=source,
-                       verbose=verbose,
-                       psql_conn_string=psql_conn_string,
-                       dbpath=dbpath)
-        elif file[-4:] == '.zip':
-            _decode_ziparchive(file,
-                               dbindex.tmp_dir,
-                               source=source,
-                               verbose=verbose,
-                               psql_conn_string=psql_conn_string,
-                               dbpath=dbpath)
-        else:
-            decoder(dbpath=dbpath,
-                    psql_conn_string=psql_conn_string,
-                    files=[file],
-                    source=source,
-                    verbose=verbose)
-        if not skip_checksum:
-            dbindex.insert_checksum(signature)
-    os.removedirs(dbindex.tmp_dir)
-
-    if vacuum is not False:
-        print("finished parsing data\nvacuuming...")
-        if vacuum is True:
-            dbconn.execute('VACUUM')
-        elif isinstance(vacuum, str):
-            assert not os.path.isfile(vacuum)
-            dbconn.execute(f"VACUUM INTO '{vacuum}'")
-        else:
-            raise ValueError('vacuum arg must be boolean or filepath string')
-        dbconn.commit()
-
-    return
+''' Parsing NMEA messages to create an SQL database.
+    See function decode_msgs() for usage
+'''
+
+from hashlib import md5
+import gzip
+import os
+import pickle
+import sqlite3
+import tempfile
+import zipfile
+
+from aisdb.database.dbconn import SQLiteDBConn, PostgresDBConn
+from aisdb.aisdb import decoder
+
+
+class FileChecksums():
+
+    def __init__(self, *, dbconn):
+        assert isinstance(dbconn, (PostgresDBConn, SQLiteDBConn))
+        if isinstance(dbconn, SQLiteDBConn):
+            assert len(dbconn.dbpaths) == 1, f'{dbconn.dbpaths}'
+        self.dbconn = dbconn
+        self.checksums_table()
+        if not os.path.isdir(
+                '/tmp') and os.name == 'posix':  # pragma: no cover
+            os.mkdir('/tmp')
+        self.tmp_dir = tempfile.mkdtemp()
+
+    def checksums_table(self):
+        ''' instantiates new database connection and creates a checksums
+            hashmap table if it doesn't exist yet.
+
+            creates a temporary directory with a path stored in ``self.tmp_dir``
+
+            creates SQLite connection attribute ``self.dbconn``, which should
+            be closed after use
+
+            e.g.
+                self.dbconn.close()
+        '''
+        # self.dbconn = sqlite3.connect(self.dbpath)
+        if isinstance(self.dbconn, SQLiteDBConn):
+            dbconn = sqlite3.connect(self.dbconn.dbpaths[0])
+            cur = dbconn.cursor()
+            cur.execute('''
+                CREATE TABLE IF NOT EXISTS
+                hashmap(
+                    hash INTEGER PRIMARY KEY,
+                    bytes BLOB
+                )
+                WITHOUT ROWID;''')
+            cur.execute('CREATE UNIQUE INDEX '
+                        'IF NOT EXISTS '
+                        'idx_map on hashmap(hash)')
+            dbconn.close()
+        elif isinstance(self.dbconn, PostgresDBConn):
+            dbconn = self.dbconn
+            cur = self.dbconn.cursor()
+            cur.execute('''
+                CREATE TABLE IF NOT EXISTS
+                hashmap(
+                    hash TEXT PRIMARY KEY,
+                    bytes BYTEA
+                );''')
+            cur.execute('CREATE UNIQUE INDEX IF NOT EXISTS '
+                        'idx_map on hashmap(hash);')
+
+    def insert_checksum(self, checksum):
+        if isinstance(self.dbconn, SQLiteDBConn):
+            dbconn = sqlite3.connect(self.dbconn.dbpaths[0])
+        elif isinstance(self.dbconn, PostgresDBConn):
+            dbconn = self.dbconn
+        dbconn.execute('INSERT INTO hashmap VALUES (?,?)',
+                       [checksum, pickle.dumps(None)])
+        dbconn.commit()
+        if isinstance(self.dbconn, SQLiteDBConn):
+            dbconn.close()
+
+    def checksum_exists(self, checksum):
+        # dbconn = sqlite3.connect(self.dbpath)
+        # cur = dbconn.cursor()
+        if isinstance(self.dbconn, SQLiteDBConn):
+            dbconn = sqlite3.connect(self.dbconn.dbpaths[0])
+            cur = dbconn.cursor()
+            cur.execute('SELECT * FROM hashmap WHERE hash = ?', [checksum])
+        elif isinstance(self.dbconn, PostgresDBConn):
+            dbconn = self.dbconn
+            cur = self.dbconn.cursor()
+            cur.execute('SELECT * FROM hashmap WHERE hash = %s', [checksum])
+        res = cur.fetchone()
+        dbconn.commit()
+        # dbconn.close()
+        if isinstance(self.dbconn, SQLiteDBConn):
+            dbconn.close()
+
+        if res is None or res is False:
+            return False
+        return True
+
+    def get_md5(self, path, f):
+        ''' get md5 hash from the first kilobyte of data '''
+        # skip header row in CSV format(~1.6kb)
+        if path[-4:].lower() == '.csv':
+            _ = f.read(1600)
+        signature = md5(f.read(1000)).hexdigest()
+        return signature
+
+
+def _decode_gz(file, tmp_dir, dbpath, psql_conn_string, source, verbose):
+    if dbpath is None:  # pragma: no cover
+        dbpath = ''
+    if psql_conn_string is None:  # pragma: no cover
+        psql_conn_string = ''
+    unzip_file = os.path.join(tmp_dir, file.rsplit(os.path.sep, 1)[-1][:-3])
+    with gzip.open(file, 'rb') as f1, open(unzip_file, 'wb') as f2:
+        f2.write(f1.read())
+    decoder(dbpath=dbpath,
+            psql_conn_string=psql_conn_string,
+            files=[unzip_file],
+            source=source,
+            verbose=verbose)
+    os.remove(unzip_file)
+
+
+def _decode_ziparchive(file, tmp_dir, dbpath, psql_conn_string, source,
+                       verbose):
+    if dbpath is None:  # pragma: no cover
+        dbpath = ''
+    if psql_conn_string is None:  # pragma: no cover
+        psql_conn_string = ''
+    zipf = zipfile.ZipFile(file)
+    for item in zipf.namelist():
+        unzip_file = os.path.join(tmp_dir, item)
+        with zipf.open(item, 'r') as f1, open(unzip_file, 'wb') as f2:
+            f2.write(f1.read())
+        decoder(dbpath=dbpath,
+                psql_conn_string=psql_conn_string,
+                files=[unzip_file],
+                source=source,
+                verbose=verbose)
+        os.remove(unzip_file)
+    zipf.close()
+
+
+def decode_msgs(filepaths,
+                dbconn,
+                source,
+                dbpath=None,
+                psql_conn_string=None,
+                vacuum=False,
+                skip_checksum=False,
+                verbose=False):
+    ''' Decode NMEA format AIS messages and store in an SQLite database.
+        To speed up decoding, create the database on a different hard drive
+        from where the raw data is stored.
+        A checksum of the first kilobyte of every file will be stored to
+        prevent loading the same file twice.
+
+        If the filepath has a .gz or .zip extension, the file will be
+        decompressed into a temporary directory before database insert.
+
+        args:
+            filepaths (list)
+                absolute filepath locations for AIS message files to be
+                ingested into the database
+            dbconn (:class:`aisdb.database.dbconn.DBConn`)
+                database connection object
+            dbpath (string)
+                SQLite database filepath to store results in. If dbconn is a
+                Postgres database connection, set this to ``None``.
+            psql_conn_string (string)
+                Postgres connection string. If dbconn is an SQLite database
+                connection, set this to ``None``.
+            source (string)
+                data source name or description. will be used as a primary key
+                column, so duplicate messages from different sources will not
+                be ignored as duplicates upon insert
+            vacuum (boolean, str)
+                if True, the database will be vacuumed after completion.
+                if string, the database will be vacuumed into the filepath
+                given. Consider vacuuming to second hard disk to speed this up
+
+        returns:
+            None
+
+        example:
+
+
+        .. _example_decode:
+
+        >>> import os
+        >>> from aisdb import decode_msgs, DBConn
+
+        >>> dbpath = 'test_decode_msgs.db'
+        >>> filepaths = ['aisdb/tests/testdata/test_data_20210701.csv',
+        ...              'aisdb/tests/testdata/test_data_20211101.nm4']
+        >>> with DBConn() as dbconn:
+        ...     decode_msgs(filepaths=filepaths, dbconn=dbconn, dbpath=dbpath, source='TESTING')
+        >>> os.remove(dbpath)
+    '''
+    if not isinstance(dbconn,
+                      (SQLiteDBConn, PostgresDBConn)):  # pragma: no cover
+        raise ValueError('db argument must be a DBConn database connection. '
+                         f'got {dbconn}')
+
+    if len(filepaths) == 0:  # pragma: no cover
+        raise ValueError('must supply atleast one filepath.')
+
+    if isinstance(dbconn, SQLiteDBConn):
+        dbconn._attach(dbpath)
+        assert dbpath is not None
+        assert psql_conn_string is None
+        psql_conn_string = ''
+    else:
+        assert psql_conn_string is not None
+        assert dbpath is None
+        dbpath = ''
+
+    dbindex = FileChecksums(dbconn=dbconn)
+    for file in filepaths:
+        if not skip_checksum:
+            with open(os.path.abspath(file), 'rb') as f:
+                signature = dbindex.get_md5(file, f)
+            if dbindex.checksum_exists(signature):
+                if verbose:  # pragma: no cover
+                    print(f'found matching checksum, skipping {file}')
+                continue
+        if file[-3:] == '.gz':
+            _decode_gz(file,
+                       dbindex.tmp_dir,
+                       source=source,
+                       verbose=verbose,
+                       psql_conn_string=psql_conn_string,
+                       dbpath=dbpath)
+        elif file[-4:] == '.zip':
+            _decode_ziparchive(file,
+                               dbindex.tmp_dir,
+                               source=source,
+                               verbose=verbose,
+                               psql_conn_string=psql_conn_string,
+                               dbpath=dbpath)
+        else:
+            decoder(dbpath=dbpath,
+                    psql_conn_string=psql_conn_string,
+                    files=[file],
+                    source=source,
+                    verbose=verbose)
+        if not skip_checksum:
+            dbindex.insert_checksum(signature)
+    os.removedirs(dbindex.tmp_dir)
+
+    if vacuum is not False:
+        print("finished parsing data\nvacuuming...")
+        if vacuum is True:
+            dbconn.execute('VACUUM')
+        elif isinstance(vacuum, str):
+            assert not os.path.isfile(vacuum)
+            dbconn.execute(f"VACUUM INTO '{vacuum}'")
+        else:
+            raise ValueError('vacuum arg must be boolean or filepath string')
+        dbconn.commit()
+
+    return
```

## aisdb/database/sqlfcn.py

 * *Ordering differences only*

```diff
@@ -1,84 +1,84 @@
-''' pass these functions to DBQuery.gen_qry() as the function argument '''
-import os
-
-from aisdb import sqlpath
-from aisdb.database.dbconn import DBConn
-
-
-def _dynamic(*, dbpath, month, callback, **kwargs):
-    ''' SQL common table expression for selecting from dynamic tables '''
-    sqlfile = 'cte_dynamic_clusteredidx.sql'
-    with open(os.path.join(sqlpath, sqlfile), 'r') as f:
-        sql = f.read()
-    args = [month for _ in range(len(sql.split('{}')) - 1)]
-    return sql.format(*args).replace(
-        f'ais_{month}_dynamic',
-        f'{DBConn._get_dbname(None, dbpath)}.ais_{month}_dynamic') + callback(
-            month=month, alias='d', **kwargs)
-    return sql.format(*args)
-
-
-def _static(*, dbpath, month='197001', **_):
-    ''' SQL common table expression for selecting from static tables '''
-    sqlfile = 'cte_static_aggregate.sql'
-    with open(os.path.join(sqlpath, sqlfile), 'r') as f:
-        sql = f.read()
-    args = [month for _ in range(len(sql.split('{}')) - 1)]
-    return sql.format(*args).replace(
-        f'static_{month}_aggregate',
-        f'{DBConn._get_dbname(None, dbpath)}.static_{month}_aggregate')
-
-
-def _leftjoin(month='197001'):
-    ''' SQL select statement using common table expressions.
-        Joins columns from dynamic, static, and coarsetype_ref tables.
-    '''
-    sqlfile = 'select_join_dynamic_static_clusteredidx.sql'
-    with open(os.path.join(sqlpath, sqlfile), 'r') as f:
-        sql = f.read()
-    args = [month for _ in range(len(sql.split('{}')) - 1)]
-    return sql.format(*args)
-
-
-def _aliases(*, dbpath, month, callback, kwargs):
-    ''' declare common table expression aliases '''
-    sqlfile = 'cte_aliases.sql'
-    with open(os.path.join(sqlpath, sqlfile), 'r') as f:
-        sql = f.read()
-    args = (month,
-            _dynamic(dbpath=dbpath, month=month, callback=callback,
-                     **kwargs), month, _static(dbpath=dbpath, month=month))
-    return sql.format(*args)
-
-
-def crawl_dynamic(*, dbpath, months, callback, **kwargs):
-    ''' iterate over position reports tables to create SQL query spanning
-        desired time range
-
-        this function should be passed as a callback to DBQuery.gen_qry(),
-        and should not be called directly
-    '''
-    sql_dynamic = '\nUNION\n'.join([
-        _dynamic(dbpath=dbpath, month=month, callback=callback, **kwargs)
-        for month in months
-    ]) + '\nORDER BY 1,2'
-    return sql_dynamic
-
-
-def crawl_dynamic_static(*, dbpath, months, callback, **kwargs):
-    ''' iterate over position reports and static messages tables to create SQL
-        query spanning desired time range
-
-        this function should be passed as a callback to DBQuery.gen_qry(),
-        and should not be called directly
-    '''
-    sqlfile = 'cte_coarsetype.sql'
-    with open(os.path.join(sqlpath, sqlfile), 'r') as f:
-        sql_coarsetype = f.read()
-    sql_aliases = ''.join([
-        _aliases(dbpath=dbpath, month=month, callback=callback, kwargs=kwargs)
-        for month in months
-    ])
-    sql_union = '\nUNION\n'.join([_leftjoin(month=month) for month in months])
-    sql_qry = f'WITH\n{sql_aliases}\n{sql_coarsetype}\n{sql_union}' + 'ORDER BY 1,2'
-    return sql_qry
+''' pass these functions to DBQuery.gen_qry() as the function argument '''
+import os
+
+from aisdb import sqlpath
+from aisdb.database.dbconn import DBConn
+
+
+def _dynamic(*, dbpath, month, callback, **kwargs):
+    ''' SQL common table expression for selecting from dynamic tables '''
+    sqlfile = 'cte_dynamic_clusteredidx.sql'
+    with open(os.path.join(sqlpath, sqlfile), 'r') as f:
+        sql = f.read()
+    args = [month for _ in range(len(sql.split('{}')) - 1)]
+    return sql.format(*args).replace(
+        f'ais_{month}_dynamic',
+        f'{DBConn._get_dbname(None, dbpath)}.ais_{month}_dynamic') + callback(
+            month=month, alias='d', **kwargs)
+    return sql.format(*args)
+
+
+def _static(*, dbpath, month='197001', **_):
+    ''' SQL common table expression for selecting from static tables '''
+    sqlfile = 'cte_static_aggregate.sql'
+    with open(os.path.join(sqlpath, sqlfile), 'r') as f:
+        sql = f.read()
+    args = [month for _ in range(len(sql.split('{}')) - 1)]
+    return sql.format(*args).replace(
+        f'static_{month}_aggregate',
+        f'{DBConn._get_dbname(None, dbpath)}.static_{month}_aggregate')
+
+
+def _leftjoin(month='197001'):
+    ''' SQL select statement using common table expressions.
+        Joins columns from dynamic, static, and coarsetype_ref tables.
+    '''
+    sqlfile = 'select_join_dynamic_static_clusteredidx.sql'
+    with open(os.path.join(sqlpath, sqlfile), 'r') as f:
+        sql = f.read()
+    args = [month for _ in range(len(sql.split('{}')) - 1)]
+    return sql.format(*args)
+
+
+def _aliases(*, dbpath, month, callback, kwargs):
+    ''' declare common table expression aliases '''
+    sqlfile = 'cte_aliases.sql'
+    with open(os.path.join(sqlpath, sqlfile), 'r') as f:
+        sql = f.read()
+    args = (month,
+            _dynamic(dbpath=dbpath, month=month, callback=callback,
+                     **kwargs), month, _static(dbpath=dbpath, month=month))
+    return sql.format(*args)
+
+
+def crawl_dynamic(*, dbpath, months, callback, **kwargs):
+    ''' iterate over position reports tables to create SQL query spanning
+        desired time range
+
+        this function should be passed as a callback to DBQuery.gen_qry(),
+        and should not be called directly
+    '''
+    sql_dynamic = '\nUNION\n'.join([
+        _dynamic(dbpath=dbpath, month=month, callback=callback, **kwargs)
+        for month in months
+    ]) + '\nORDER BY 1,2'
+    return sql_dynamic
+
+
+def crawl_dynamic_static(*, dbpath, months, callback, **kwargs):
+    ''' iterate over position reports and static messages tables to create SQL
+        query spanning desired time range
+
+        this function should be passed as a callback to DBQuery.gen_qry(),
+        and should not be called directly
+    '''
+    sqlfile = 'cte_coarsetype.sql'
+    with open(os.path.join(sqlpath, sqlfile), 'r') as f:
+        sql_coarsetype = f.read()
+    sql_aliases = ''.join([
+        _aliases(dbpath=dbpath, month=month, callback=callback, kwargs=kwargs)
+        for month in months
+    ])
+    sql_union = '\nUNION\n'.join([_leftjoin(month=month) for month in months])
+    sql_qry = f'WITH\n{sql_aliases}\n{sql_coarsetype}\n{sql_union}' + 'ORDER BY 1,2'
+    return sql_qry
```

## aisdb/database/sqlfcn_callbacks.py

 * *Ordering differences only*

```diff
@@ -1,56 +1,56 @@
-''' redefinitions of functions in :py:mod:`aisdb.database.sql_query_strings`,
-    combined into lambdas for convenience
-'''
-
-from datetime import datetime, timedelta
-
-import numpy as np
-
-from aisdb.database.sql_query_strings import (
-    has_mmsi,
-    in_bbox,
-    in_mmsi,
-    in_timerange,
-    valid_mmsi,
-)
-
-dt2monthstr = lambda start, end, **_: np.unique([
-    t.strftime('%Y%m')
-    for t in np.arange(start, end, timedelta(days=1)).astype(datetime)
-]).astype(object)
-
-in_bbox_time = lambda **kwargs: f'''\
-    {in_bbox(**kwargs)} AND
-    {in_timerange(**kwargs)} '''
-in_bbox_time_validmmsi = lambda **kwargs: f'''\
-    {in_bbox(**kwargs)} AND
-    {in_timerange(**kwargs)} AND
-    {valid_mmsi(**kwargs)} '''
-in_time_bbox = lambda **kwargs: f'''\
-    {in_timerange(**kwargs)} AND
-    {in_bbox(**kwargs)} '''
-in_time_bbox_hasmmsi = lambda **kwargs: f'''\
-    {in_timerange(**kwargs)} AND
-    {in_bbox(**kwargs)} AND
-    {has_mmsi(**kwargs)}'''
-in_time_bbox_inmmsi = lambda **kwargs: f'''\
-    {in_timerange(**kwargs)} AND
-    {in_bbox(**kwargs)} AND
-    {in_mmsi(**kwargs)} '''
-in_time_bbox_validmmsi = lambda **kwargs: f'''\
-    {in_timerange(**kwargs)} AND
-    {in_bbox(**kwargs)} AND
-    {valid_mmsi(**kwargs)} '''
-in_time_mmsi = lambda **kwargs: f'''\
-    {in_timerange(**kwargs)} AND {valid_mmsi(**kwargs)}'''
-in_timerange_hasmmsi = lambda **kwargs: f'''\
-    {in_timerange(**kwargs)} AND {has_mmsi(**kwargs)}'''
-in_timerange_inmmsi = lambda **kwargs: f'''\
-    {in_timerange(**kwargs)} AND
-    {in_mmsi(**kwargs)}'''
-in_timerange_validmmsi = lambda **kwargs: f'''\
-    {in_timerange(**kwargs)} AND
-    {valid_mmsi(**kwargs)}'''
-in_validmmsi_bbox = lambda **kwargs: f'''\
-    {valid_mmsi(**kwargs)} AND
-    {in_bbox(**kwargs)} '''
+''' redefinitions of functions in :py:mod:`aisdb.database.sql_query_strings`,
+    combined into lambdas for convenience
+'''
+
+from datetime import datetime, timedelta
+
+import numpy as np
+
+from aisdb.database.sql_query_strings import (
+    has_mmsi,
+    in_bbox,
+    in_mmsi,
+    in_timerange,
+    valid_mmsi,
+)
+
+dt2monthstr = lambda start, end, **_: np.unique([
+    t.strftime('%Y%m')
+    for t in np.arange(start, end, timedelta(days=1)).astype(datetime)
+]).astype(object)
+
+in_bbox_time = lambda **kwargs: f'''\
+    {in_bbox(**kwargs)} AND
+    {in_timerange(**kwargs)} '''
+in_bbox_time_validmmsi = lambda **kwargs: f'''\
+    {in_bbox(**kwargs)} AND
+    {in_timerange(**kwargs)} AND
+    {valid_mmsi(**kwargs)} '''
+in_time_bbox = lambda **kwargs: f'''\
+    {in_timerange(**kwargs)} AND
+    {in_bbox(**kwargs)} '''
+in_time_bbox_hasmmsi = lambda **kwargs: f'''\
+    {in_timerange(**kwargs)} AND
+    {in_bbox(**kwargs)} AND
+    {has_mmsi(**kwargs)}'''
+in_time_bbox_inmmsi = lambda **kwargs: f'''\
+    {in_timerange(**kwargs)} AND
+    {in_bbox(**kwargs)} AND
+    {in_mmsi(**kwargs)} '''
+in_time_bbox_validmmsi = lambda **kwargs: f'''\
+    {in_timerange(**kwargs)} AND
+    {in_bbox(**kwargs)} AND
+    {valid_mmsi(**kwargs)} '''
+in_time_mmsi = lambda **kwargs: f'''\
+    {in_timerange(**kwargs)} AND {valid_mmsi(**kwargs)}'''
+in_timerange_hasmmsi = lambda **kwargs: f'''\
+    {in_timerange(**kwargs)} AND {has_mmsi(**kwargs)}'''
+in_timerange_inmmsi = lambda **kwargs: f'''\
+    {in_timerange(**kwargs)} AND
+    {in_mmsi(**kwargs)}'''
+in_timerange_validmmsi = lambda **kwargs: f'''\
+    {in_timerange(**kwargs)} AND
+    {valid_mmsi(**kwargs)}'''
+in_validmmsi_bbox = lambda **kwargs: f'''\
+    {valid_mmsi(**kwargs)} AND
+    {in_bbox(**kwargs)} '''
```

## aisdb/database/sql_query_strings.py

 * *Ordering differences only*

```diff
@@ -1,148 +1,148 @@
-import warnings
-
-from aisdb.gis import dt_2_epoch, shiftcoord
-
-
-# callback functions
-def in_bbox(*, alias, xmin, xmax, ymin, ymax, **_):
-    ''' SQL callback restricting vessels in bounding box region
-
-        args:
-            alias (string)
-                the 'alias' in a 'WITH tablename AS alias ...' SQL statement
-            xmin (float)
-                minimum longitude
-            xmax (float)
-                maximum longitude
-            ymin (float)
-                minimum latitude
-            ymax (float)
-                maximum latitude
-
-        returns:
-            SQL code (string)
-    '''
-    if not -180 <= xmin <= 180:
-        warnings.warn(f'got {xmin}')
-        xmin = shiftcoord([xmin])[0]
-    if not -180 <= xmax <= 180:
-        warnings.warn(f'got {xmax}')
-        xmax = shiftcoord([xmax])[0]
-    if not -90 <= ymin <= 90:
-        warnings.warn(f'got {ymin=}')
-    if not -90 <= ymax <= 90:
-        warnings.warn(f'got {ymax=}')
-    assert ymin < ymax, f'got {ymin=} {ymax=}'
-
-    if xmin == -180 and xmax == 180:
-        return f'''({alias}.longitude >= {xmin} AND {alias}.longitude <= {xmax}) AND
-    {alias}.latitude >= {ymin} AND
-    {alias}.latitude <= {ymax}'''
-
-    #if xmin < xmax:
-    assert xmin < xmax
-    #if xmin < -180 and xmax > 180:
-    #    raise ValueError(f'xmin, xmax are out of bounds! {xmin=} < -180,{xmax=} > 180')
-    #elif -180 <= xmin <= 180 and -180 <= xmax <= 180:
-    s = f'''{alias}.longitude >= {xmin} AND
-            {alias}.longitude <= {xmax} AND '''
-    """
-    elif xmin < -180:
-        s = f'''(
-    ({alias}.longitude >= -180 AND {alias}.longitude <= {xmax}) OR
-    ({alias}.longitude <= 180 AND {alias}.longitude >= {shiftcoord([xmin])[0]})
-) AND '''
-    elif xmax > 180:
-        s = f'''(
-    ({alias}.longitude <= 180 AND {alias}.longitude >= {shiftcoord([xmax])[0]}) OR
-    ({alias}.longitude >= -180 AND {alias}.longitude <= {xmin})
-) AND '''
-    else:
-        raise ValueError(
-            f'Error creating SQL query in longitude bounds {xmin=} {xmax=}'
-        )
-    """
-
-    query_args = f'''{s}
-    {alias}.latitude >= {ymin} AND
-    {alias}.latitude <= {ymax}'''
-
-    return query_args
-
-    #else:
-    '''
-    if xmin < -180:
-        x0 = shiftcoord([xmin])[0]
-    else:
-        x0 = xmin
-    if xmax > 180:
-        x1 = shiftcoord([xmax])[0]
-    else:
-        x1 = xmax
-    '''
-
-    #assert x0 <= x1
-
-    #return f'''({alias}.longitude >= {xmin} OR {alias}.longitude <= {xmax}) AND {alias}.latitude >= {ymin} AND {alias}.latitude <= {ymax}'''
-
-
-def in_timerange(*, alias, start, end, **_):
-    ''' SQL callback restricting vessels in temporal range.
-
-        args:
-            alias (string)
-                the 'alias' in a 'WITH tablename AS alias ...' SQL statement
-            start (datetime)
-            end (datetime)
-
-        returns:
-            SQL code (string)
-    '''
-    return f'''{alias}.time >= {dt_2_epoch(start)} AND
-    {alias}.time <= {dt_2_epoch(end)}'''
-
-
-def has_mmsi(*, alias, mmsi, **_):
-    ''' SQL callback selecting a single vessel identifier
-
-        args:
-            alias (string)
-                the 'alias' in a 'WITH tablename AS alias ...' SQL statement
-            mmsi (int)
-                vessel identifier
-
-        returns:
-            SQL code (string)
-    '''
-    return f'''CAST({alias}.mmsi AS INT) = {mmsi}'''
-
-
-def in_mmsi(*, alias, mmsis, **_):
-    ''' SQL callback selecting multiple vessel identifiers
-
-        args:
-            alias (string)
-                the 'alias' in a 'WITH tablename AS alias ...' SQL statement
-            mmsis (tuple)
-                tuple of vessel identifiers (int)
-
-        returns:
-            SQL code (string)
-    '''
-    return f'''{alias}.mmsi IN
-    ({", ".join(map(str, mmsis))})'''
-
-
-def valid_mmsi(*, alias='m123', **_):
-    ''' SQL callback selecting all vessel identifiers within the valid vessel
-        mmsi range, e.g. (201000000, 776000000)
-
-        args:
-            alias (string)
-                the 'alias' in a 'WITH tablename AS alias ...' SQL statement
-
-        returns:
-            SQL code (string)
-    '''
-    return f'''{alias}.mmsi >= 201000000 AND
-    {alias}.mmsi < 776000000 '''
+import warnings
+
+from aisdb.gis import dt_2_epoch, shiftcoord
+
+
+# callback functions
+def in_bbox(*, alias, xmin, xmax, ymin, ymax, **_):
+    ''' SQL callback restricting vessels in bounding box region
+
+        args:
+            alias (string)
+                the 'alias' in a 'WITH tablename AS alias ...' SQL statement
+            xmin (float)
+                minimum longitude
+            xmax (float)
+                maximum longitude
+            ymin (float)
+                minimum latitude
+            ymax (float)
+                maximum latitude
+
+        returns:
+            SQL code (string)
+    '''
+    if not -180 <= xmin <= 180:
+        warnings.warn(f'got {xmin}')
+        xmin = shiftcoord([xmin])[0]
+    if not -180 <= xmax <= 180:
+        warnings.warn(f'got {xmax}')
+        xmax = shiftcoord([xmax])[0]
+    if not -90 <= ymin <= 90:
+        warnings.warn(f'got {ymin=}')
+    if not -90 <= ymax <= 90:
+        warnings.warn(f'got {ymax=}')
+    assert ymin < ymax, f'got {ymin=} {ymax=}'
+
+    if xmin == -180 and xmax == 180:
+        return f'''({alias}.longitude >= {xmin} AND {alias}.longitude <= {xmax}) AND
+    {alias}.latitude >= {ymin} AND
+    {alias}.latitude <= {ymax}'''
+
+    #if xmin < xmax:
+    assert xmin < xmax
+    #if xmin < -180 and xmax > 180:
+    #    raise ValueError(f'xmin, xmax are out of bounds! {xmin=} < -180,{xmax=} > 180')
+    #elif -180 <= xmin <= 180 and -180 <= xmax <= 180:
+    s = f'''{alias}.longitude >= {xmin} AND
+            {alias}.longitude <= {xmax} AND '''
+    """
+    elif xmin < -180:
+        s = f'''(
+    ({alias}.longitude >= -180 AND {alias}.longitude <= {xmax}) OR
+    ({alias}.longitude <= 180 AND {alias}.longitude >= {shiftcoord([xmin])[0]})
+) AND '''
+    elif xmax > 180:
+        s = f'''(
+    ({alias}.longitude <= 180 AND {alias}.longitude >= {shiftcoord([xmax])[0]}) OR
+    ({alias}.longitude >= -180 AND {alias}.longitude <= {xmin})
+) AND '''
+    else:
+        raise ValueError(
+            f'Error creating SQL query in longitude bounds {xmin=} {xmax=}'
+        )
+    """
+
+    query_args = f'''{s}
+    {alias}.latitude >= {ymin} AND
+    {alias}.latitude <= {ymax}'''
+
+    return query_args
+
+    #else:
+    '''
+    if xmin < -180:
+        x0 = shiftcoord([xmin])[0]
+    else:
+        x0 = xmin
+    if xmax > 180:
+        x1 = shiftcoord([xmax])[0]
+    else:
+        x1 = xmax
+    '''
+
+    #assert x0 <= x1
+
+    #return f'''({alias}.longitude >= {xmin} OR {alias}.longitude <= {xmax}) AND {alias}.latitude >= {ymin} AND {alias}.latitude <= {ymax}'''
+
+
+def in_timerange(*, alias, start, end, **_):
+    ''' SQL callback restricting vessels in temporal range.
+
+        args:
+            alias (string)
+                the 'alias' in a 'WITH tablename AS alias ...' SQL statement
+            start (datetime)
+            end (datetime)
+
+        returns:
+            SQL code (string)
+    '''
+    return f'''{alias}.time >= {dt_2_epoch(start)} AND
+    {alias}.time <= {dt_2_epoch(end)}'''
+
+
+def has_mmsi(*, alias, mmsi, **_):
+    ''' SQL callback selecting a single vessel identifier
+
+        args:
+            alias (string)
+                the 'alias' in a 'WITH tablename AS alias ...' SQL statement
+            mmsi (int)
+                vessel identifier
+
+        returns:
+            SQL code (string)
+    '''
+    return f'''CAST({alias}.mmsi AS INT) = {mmsi}'''
+
+
+def in_mmsi(*, alias, mmsis, **_):
+    ''' SQL callback selecting multiple vessel identifiers
+
+        args:
+            alias (string)
+                the 'alias' in a 'WITH tablename AS alias ...' SQL statement
+            mmsis (tuple)
+                tuple of vessel identifiers (int)
+
+        returns:
+            SQL code (string)
+    '''
+    return f'''{alias}.mmsi IN
+    ({", ".join(map(str, mmsis))})'''
+
+
+def valid_mmsi(*, alias='m123', **_):
+    ''' SQL callback selecting all vessel identifiers within the valid vessel
+        mmsi range, e.g. (201000000, 776000000)
+
+        args:
+            alias (string)
+                the 'alias' in a 'WITH tablename AS alias ...' SQL statement
+
+        returns:
+            SQL code (string)
+    '''
+    return f'''{alias}.mmsi >= 201000000 AND
+    {alias}.mmsi < 776000000 '''
```

## aisdb/database/__init__.py

```diff
@@ -1 +1 @@
-00000000: 0d0a                                     ..
+00000000: 0a                                       .
```

## aisdb/denoising_encoder.py

 * *Ordering differences only*

```diff
@@ -1,208 +1,208 @@
-import warnings
-from functools import reduce
-
-import numpy as np
-
-from aisdb.aisdb import encoder_score_fcn
-from aisdb.gis import delta_knots, delta_meters
-
-
-def _score_idx(scores):
-    ''' Returns indices of score array where value at index is equal to the
-        highest score. In tie cases, the last index will be selected
-    '''
-    assert len(scores) > 0
-    return np.where(scores == np.max(scores))[0][-1]
-
-
-def _segments_idx(track, distance_threshold, speed_threshold, **_):
-    segments_idx1 = reduce(
-        np.append, ([0], np.where(delta_knots(track) > speed_threshold)[0] + 1,
-                    [track['time'].size]))
-    segments_idx2 = reduce(
-        np.append,
-        ([0], np.where(delta_meters(track) > distance_threshold)[0] + 1,
-         [track['time'].size]))
-
-    return reduce(np.union1d, (segments_idx1, segments_idx2))
-
-
-def _scoresarray(track, *, pathways, i, segments_idx, distance_threshold,
-                 speed_threshold, minscore):
-    scores = np.array(
-        [
-            encoder_score_fcn(
-                x1=pathway['lon'][-1],
-                y1=pathway['lat'][-1],
-                t1=pathway['time'][-1],
-                x2=track['lon'][segments_idx[i]],
-                y2=track['lat'][segments_idx[i]],
-                t2=track['time'][segments_idx[i]],
-                dist_thresh=distance_threshold,
-                speed_thresh=speed_threshold,
-            ) for pathway in pathways
-        ],
-        dtype=np.float32,
-    )
-    highscore = (scores[np.where(
-        scores == np.max(scores))[0][0]] if scores.size > 0 else minscore)
-    return scores, highscore
-
-
-def _append_highscore(track, *, highscoreidx, pathways, i, segments_idx):
-    return dict(
-        **{k: track[k]
-           for k in track['static']},
-        **{
-            k: np.append(pathways[highscoreidx][k],
-                         track[k][segments_idx[i]:segments_idx[i + 1]])
-            for k in track['dynamic']
-        },
-        static=track['static'],
-        dynamic=track['dynamic'],
-    )
-
-
-def _split_pathway(track, *, i, segments_idx):
-    path = dict(
-        **{k: track[k]
-           for k in track['static']},
-        **{
-            k: track[k][segments_idx[i]:segments_idx[i + 1]]
-            for k in track['dynamic']
-        },
-        static=track['static'],
-        dynamic=track['dynamic'],
-    )
-    return path
-
-
-def encode_score(track, distance_threshold, speed_threshold, minscore):
-    ''' Encodes likelihood of persistent track membership when given distance,
-        speed, and score thresholds, using track speed deltas computed using
-        distance computed by haversine function divided by elapsed time
-
-        A higher distance threshold will increase the maximum distance in
-        meters allowed between pings for same trajectory membership. A higher
-        speed threshold will allow vessels travelling up to this value in knots
-        to be kconsidered for persistent track membership.
-        The minscore assigns a minimum score needed to be considered for
-        membership, typically 0 or very close to 0 such as 1e-5.
-
-        For example: a vessel travelling at a lower speed with short intervals
-        between pings will have a higher likelihood of persistence.
-        A trajectory with higher average speed or long intervals between
-        pings may indicate two separate trajectories and will be segmented
-        forming alternate trajectories according to highest likelihood of
-        membership.
-    '''
-    assert 'time' in track.keys()
-    assert len(track['time']) > 0
-    params = dict(distance_threshold=distance_threshold,
-                  speed_threshold=speed_threshold,
-                  minscore=minscore)
-    segments_idx = _segments_idx(track, **params)
-    pathways = []
-    warned = False
-    for i in range(segments_idx.size - 1):
-        if len(pathways) == 0:
-            path = _split_pathway(track, i=i, segments_idx=segments_idx)
-            assert path is not None
-            pathways.append(path)
-            continue
-        elif not warned and len(pathways) > 100:
-            warnings.warn(
-                f'excessive number of pathways! mmsi={track["mmsi"]}')
-            warned = True
-        assert len(track['time']) > 0, f'{track=}'
-
-        scores, highscore = _scoresarray(track,
-                                         pathways=pathways,
-                                         i=i,
-                                         segments_idx=segments_idx,
-                                         **params)
-        assert len(scores) > 0, f'{track}'
-        if (highscore >= minscore):
-            highscoreidx = _score_idx(scores)
-            pathways[highscoreidx] = _append_highscore(
-                track,
-                highscoreidx=highscoreidx,
-                pathways=pathways,
-                i=i,
-                segments_idx=segments_idx)
-        else:
-            path = _split_pathway(track, i=i, segments_idx=segments_idx)
-            assert path is not None
-            pathways.append(path.copy())
-
-    for pathway, label in zip(pathways, range(len(pathways))):
-        pathway['label'] = label
-        pathway['static'] = set(pathway['static']).union({'label'})
-        assert 'label' in pathway.keys()
-        assert 'time' in pathway.keys(), f'{pathway=}'
-        yield pathway
-
-
-def encode_greatcircledistance(
-    tracks,
-    *,
-    distance_threshold,
-    speed_threshold=50,
-    minscore=1e-6,
-):
-    ''' partitions tracks where delta speeds exceed speed_threshold or
-        delta_meters exceeds distance_threshold.
-        concatenates track segments with the highest likelihood of being
-        sequential, as encoded by the encode_score function
-
-        args:
-            tracks (aisdb.track_gen.TrackGen)
-                track vectors generator
-            distance_threshold (int)
-                distance in meters that will be used as a
-                speed score numerator
-            time_threshold (datetime.timedelta)
-            minscore (float)
-                minimum score threshold at which to allow track
-                segments to be linked
-
-        >>> import os
-        >>> from datetime import datetime, timedelta
-        >>> from aisdb import DBConn, DBQuery, TrackGen
-        >>> from aisdb import decode_msgs, encode_greatcircledistance, sqlfcn_callbacks
-
-        >>> # create example database file
-        >>> dbpath = 'encoder_test.db'
-        >>> filepaths = ['aisdb/tests/testdata/test_data_20210701.csv',
-        ...              'aisdb/tests/testdata/test_data_20211101.nm4']
-
-        >>> with DBConn() as dbconn:
-        ...     decode_msgs(filepaths=filepaths, dbconn=dbconn,
-        ...     dbpath=dbpath, source='TESTING')
-
-        >>> with DBConn() as dbconn:
-        ...     q = DBQuery(callback=sqlfcn_callbacks.in_timerange_validmmsi,
-        ...             dbconn=dbconn,
-        ...             dbpath=dbpath,
-        ...             start=datetime(2021, 7, 1),
-        ...             end=datetime(2021, 7, 7))
-        ...     tracks = TrackGen(q.gen_qry(), decimate=True)
-        ...     for track in encode_greatcircledistance(
-        ...             tracks,
-        ...             distance_threshold=250000,  # metres
-        ...             speed_threshold=50,         # knots
-        ...             minscore=0,
-        ...         ):
-        ...         print(track['mmsi'])
-        ...         print(track['lon'], track['lat'])
-        ...         break
-        204242000
-        [-8.931666] [41.45]
-        >>> os.remove(dbpath)
-
-    '''
-    for track in tracks:
-        assert isinstance(track, dict), f'got {type(track)} {track}'
-        for path in encode_score(track, distance_threshold, speed_threshold,
-                                 minscore):
-            yield path
+import warnings
+from functools import reduce
+
+import numpy as np
+
+from aisdb.aisdb import encoder_score_fcn
+from aisdb.gis import delta_knots, delta_meters
+
+
+def _score_idx(scores):
+    ''' Returns indices of score array where value at index is equal to the
+        highest score. In tie cases, the last index will be selected
+    '''
+    assert len(scores) > 0
+    return np.where(scores == np.max(scores))[0][-1]
+
+
+def _segments_idx(track, distance_threshold, speed_threshold, **_):
+    segments_idx1 = reduce(
+        np.append, ([0], np.where(delta_knots(track) > speed_threshold)[0] + 1,
+                    [track['time'].size]))
+    segments_idx2 = reduce(
+        np.append,
+        ([0], np.where(delta_meters(track) > distance_threshold)[0] + 1,
+         [track['time'].size]))
+
+    return reduce(np.union1d, (segments_idx1, segments_idx2))
+
+
+def _scoresarray(track, *, pathways, i, segments_idx, distance_threshold,
+                 speed_threshold, minscore):
+    scores = np.array(
+        [
+            encoder_score_fcn(
+                x1=pathway['lon'][-1],
+                y1=pathway['lat'][-1],
+                t1=pathway['time'][-1],
+                x2=track['lon'][segments_idx[i]],
+                y2=track['lat'][segments_idx[i]],
+                t2=track['time'][segments_idx[i]],
+                dist_thresh=distance_threshold,
+                speed_thresh=speed_threshold,
+            ) for pathway in pathways
+        ],
+        dtype=np.float32,
+    )
+    highscore = (scores[np.where(
+        scores == np.max(scores))[0][0]] if scores.size > 0 else minscore)
+    return scores, highscore
+
+
+def _append_highscore(track, *, highscoreidx, pathways, i, segments_idx):
+    return dict(
+        **{k: track[k]
+           for k in track['static']},
+        **{
+            k: np.append(pathways[highscoreidx][k],
+                         track[k][segments_idx[i]:segments_idx[i + 1]])
+            for k in track['dynamic']
+        },
+        static=track['static'],
+        dynamic=track['dynamic'],
+    )
+
+
+def _split_pathway(track, *, i, segments_idx):
+    path = dict(
+        **{k: track[k]
+           for k in track['static']},
+        **{
+            k: track[k][segments_idx[i]:segments_idx[i + 1]]
+            for k in track['dynamic']
+        },
+        static=track['static'],
+        dynamic=track['dynamic'],
+    )
+    return path
+
+
+def encode_score(track, distance_threshold, speed_threshold, minscore):
+    ''' Encodes likelihood of persistent track membership when given distance,
+        speed, and score thresholds, using track speed deltas computed using
+        distance computed by haversine function divided by elapsed time
+
+        A higher distance threshold will increase the maximum distance in
+        meters allowed between pings for same trajectory membership. A higher
+        speed threshold will allow vessels travelling up to this value in knots
+        to be kconsidered for persistent track membership.
+        The minscore assigns a minimum score needed to be considered for
+        membership, typically 0 or very close to 0 such as 1e-5.
+
+        For example: a vessel travelling at a lower speed with short intervals
+        between pings will have a higher likelihood of persistence.
+        A trajectory with higher average speed or long intervals between
+        pings may indicate two separate trajectories and will be segmented
+        forming alternate trajectories according to highest likelihood of
+        membership.
+    '''
+    assert 'time' in track.keys()
+    assert len(track['time']) > 0
+    params = dict(distance_threshold=distance_threshold,
+                  speed_threshold=speed_threshold,
+                  minscore=minscore)
+    segments_idx = _segments_idx(track, **params)
+    pathways = []
+    warned = False
+    for i in range(segments_idx.size - 1):
+        if len(pathways) == 0:
+            path = _split_pathway(track, i=i, segments_idx=segments_idx)
+            assert path is not None
+            pathways.append(path)
+            continue
+        elif not warned and len(pathways) > 100:
+            warnings.warn(
+                f'excessive number of pathways! mmsi={track["mmsi"]}')
+            warned = True
+        assert len(track['time']) > 0, f'{track=}'
+
+        scores, highscore = _scoresarray(track,
+                                         pathways=pathways,
+                                         i=i,
+                                         segments_idx=segments_idx,
+                                         **params)
+        assert len(scores) > 0, f'{track}'
+        if (highscore >= minscore):
+            highscoreidx = _score_idx(scores)
+            pathways[highscoreidx] = _append_highscore(
+                track,
+                highscoreidx=highscoreidx,
+                pathways=pathways,
+                i=i,
+                segments_idx=segments_idx)
+        else:
+            path = _split_pathway(track, i=i, segments_idx=segments_idx)
+            assert path is not None
+            pathways.append(path.copy())
+
+    for pathway, label in zip(pathways, range(len(pathways))):
+        pathway['label'] = label
+        pathway['static'] = set(pathway['static']).union({'label'})
+        assert 'label' in pathway.keys()
+        assert 'time' in pathway.keys(), f'{pathway=}'
+        yield pathway
+
+
+def encode_greatcircledistance(
+    tracks,
+    *,
+    distance_threshold,
+    speed_threshold=50,
+    minscore=1e-6,
+):
+    ''' partitions tracks where delta speeds exceed speed_threshold or
+        delta_meters exceeds distance_threshold.
+        concatenates track segments with the highest likelihood of being
+        sequential, as encoded by the encode_score function
+
+        args:
+            tracks (aisdb.track_gen.TrackGen)
+                track vectors generator
+            distance_threshold (int)
+                distance in meters that will be used as a
+                speed score numerator
+            time_threshold (datetime.timedelta)
+            minscore (float)
+                minimum score threshold at which to allow track
+                segments to be linked
+
+        >>> import os
+        >>> from datetime import datetime, timedelta
+        >>> from aisdb import DBConn, DBQuery, TrackGen
+        >>> from aisdb import decode_msgs, encode_greatcircledistance, sqlfcn_callbacks
+
+        >>> # create example database file
+        >>> dbpath = 'encoder_test.db'
+        >>> filepaths = ['aisdb/tests/testdata/test_data_20210701.csv',
+        ...              'aisdb/tests/testdata/test_data_20211101.nm4']
+
+        >>> with DBConn() as dbconn:
+        ...     decode_msgs(filepaths=filepaths, dbconn=dbconn,
+        ...     dbpath=dbpath, source='TESTING')
+
+        >>> with DBConn() as dbconn:
+        ...     q = DBQuery(callback=sqlfcn_callbacks.in_timerange_validmmsi,
+        ...             dbconn=dbconn,
+        ...             dbpath=dbpath,
+        ...             start=datetime(2021, 7, 1),
+        ...             end=datetime(2021, 7, 7))
+        ...     tracks = TrackGen(q.gen_qry(), decimate=True)
+        ...     for track in encode_greatcircledistance(
+        ...             tracks,
+        ...             distance_threshold=250000,  # metres
+        ...             speed_threshold=50,         # knots
+        ...             minscore=0,
+        ...         ):
+        ...         print(track['mmsi'])
+        ...         print(track['lon'], track['lat'])
+        ...         break
+        204242000
+        [-8.931666] [41.45]
+        >>> os.remove(dbpath)
+
+    '''
+    for track in tracks:
+        assert isinstance(track, dict), f'got {type(track)} {track}'
+        for path in encode_score(track, distance_threshold, speed_threshold,
+                                 minscore):
+            yield path
```

## aisdb/gis.py

 * *Ordering differences only*

```diff
@@ -1,530 +1,530 @@
-'''Geometry and GIS utilities'''
-
-import os
-import pathlib
-import tempfile
-from datetime import datetime, timedelta
-from functools import partial
-
-import numpy as np
-import shapely.ops
-import shapely.geometry
-import warnings
-from shapely.geometry import Polygon, LineString, Point
-
-from aisdb.aisdb import haversine
-from aisdb.proc_util import glob_files
-
-
-def shiftcoord(x, rng=180):
-    ''' Correct longitude coordinates to be within range(-180, 180)
-        using a linear shift and modulus.
-        For latitude coordinate correction, set rng to 90.
-
-        For example: longitude 181 would be corrected to -179 deg.
-    '''
-    assert len(x) > 0, 'x must be array-like'
-    if not isinstance(x, np.ndarray):
-        x = np.array(x)
-    shift_idx = np.where(np.abs(x) != rng)[0]
-    for idx in shift_idx:
-        x[idx] = ((x[idx] + rng) % 360) - rng
-    flip_idx = np.where(np.abs(x) == rng)[0]
-    for idx in flip_idx:
-        x[idx] *= -1
-    assert (rng * -1 <= np.all(x) <= rng)
-    return x
-
-
-def dt_2_epoch(dt_arr, t0=datetime(1970, 1, 1, 0, 0, 0)):
-    ''' convert datetime.datetime to epoch minutes '''
-    delta = lambda dt: (dt - t0).total_seconds()
-    if isinstance(dt_arr, (list, np.ndarray)):
-        return np.array(list(map(float, map(delta, dt_arr))))
-    elif isinstance(dt_arr, (datetime)):
-        return int(delta(dt_arr))
-    else:
-        raise ValueError('input must be datetime or array of datetimes')
-
-
-def epoch_2_dt(ep_arr, t0=datetime(1970, 1, 1, 0, 0, 0), unit='seconds'):
-    ''' convert epoch minutes to datetime.datetime '''
-
-    delta = lambda ep, unit: t0 + timedelta(**{unit: ep})
-
-    if isinstance(ep_arr, (list, np.ndarray)):
-        return np.array(list(map(partial(delta, unit=unit), map(int, ep_arr))))
-
-    elif isinstance(ep_arr,
-                    (float, int, np.uint32, np.int32, np.uint64, np.int64)):
-        return delta(int(ep_arr), unit=unit)
-
-    else:
-        raise ValueError(
-            f'input must be integer or array of integers. got {ep_arr=}{type(ep_arr)}'
-        )
-
-
-def delta_meters(track, rng=None):
-    ''' compute haversine distance in meters between track positions for a
-        given track
-
-        args:
-            track (dict)
-                track vector dictionary
-            rng (range)
-                optionally restrict computed values to given index range
-    '''
-    rng = range(len(track['time'])) if rng is None else rng
-    return np.array(
-        list(
-            map(haversine, track['lon'][rng][:-1], track['lat'][rng][:-1],
-                track['lon'][rng][1:], track['lat'][rng][1:])))
-
-
-def delta_seconds(track, rng=None):
-    ''' compute elapsed time between track positions for a given track
-
-        args:
-            track (dict)
-                track vector dictionary
-            rng (range)
-                optionally restrict computed values to given index range
-    '''
-    if isinstance(track['time'], list):
-        track['time'] = np.array(track['time'])
-    assert isinstance(track['time'], np.ndarray), f'got {track["time"] = }'
-    rng = range(len(track['time'])) if rng is None else rng
-    return np.array(list((track['time'][rng][1:] - track['time'][rng][:-1])))
-
-
-def delta_knots(track, rng=None):
-    ''' compute speed over ground in knots between track positions for a given
-        track using (haversine distance / time)
-
-        args:
-            track (dict)
-                track vector dictionary
-            rng (range)
-                optionally restrict computed values to given index range
-    '''
-    rng = range(len(track['time'])) if rng is None else rng
-    ds = np.array([np.max((1, s)) for s in delta_seconds(track, rng)],
-                  dtype=object)
-    return delta_meters(track, rng) / ds * 1.9438445
-
-
-def radial_coordinate_boundary(x, y, radius=100000):
-    ''' Defines a bounding box area for a given point and radial
-        distance in meters. Returns degree boundaries with a minimum diameter
-        of approximately 2 * ``radius`` meters.
-
-        The boundaries are approximated by converting input coordinates
-        from degrees to radians, and computing a radial delta by
-        dividing an input value by the earth radius. The radial delta
-        is added or subtracted from the input point for each cardinal
-        direction, and then converted back from radians to degrees.
-
-        args:
-            x (float)
-                longitude
-            y (float)
-                latitude
-            radius (int, float)
-                minimum radial distance
-    '''
-    # radians
-    earth_radius_m = 6371088
-    rlon = np.pi * x / 180
-    rlat = np.pi * y / 180
-    parallel_radius = earth_radius_m * np.cos(rlat)
-
-    # radial delta
-    rlonmin = rlon - radius / parallel_radius
-    rlonmax = rlon + radius / parallel_radius
-    rlatmin = rlat - radius / earth_radius_m
-    rlatmax = rlat + radius / earth_radius_m
-
-    return {
-        'xmin': 180 * rlonmin / np.pi,
-        'xmax': 180 * rlonmax / np.pi,
-        'ymin': 180 * rlatmin / np.pi,
-        'ymax': 180 * rlatmax / np.pi
-    }
-
-
-def distance3D(x1, y1, x2, y2, depth_metres):
-    ''' haversine/pythagoras approximation of vessel distance to
-        point at given depth
-    '''
-    a2 = haversine(x1=x1, y1=y1, x2=x2, y2=y2)**2
-    b2 = abs(depth_metres)**2
-    c2 = a2 + b2
-    return np.sqrt(c2)
-
-
-def vesseltrack_3D_dist(tracks, x1, y1, z1, colname='distance_metres'):
-    ''' appends approximate distance to a submerged point at every
-        surface-level position. distance is approximated using the haversine
-        function and pythagoras.
-
-        x1 (float)
-            point longitude
-        y1 (float)
-            point latitude
-        z1 (float)
-            point depth (metres)
-        colname (string)
-            track dictionary key for which depth values will be set.
-            by default, distances are appended to the 'distance_metres'
-            key
-    '''
-    for track in tracks:
-        track['dynamic'] = track['dynamic'].union(set([colname]))
-        dists = [
-            distance3D(x1=x1, y1=y1, x2=x, y2=y, depth_metres=z1)
-            for x, y in zip(track['lon'], track['lat'])
-        ]
-        track[colname] = np.array(dists, dtype=object)
-        yield track
-
-
-def mask_in_radius_2D(tracks, xy, distance_meters):
-    ''' radial filtering using great circle distance at surface level
-
-        tracks (:class:`aisdb.track_gen.TrackGen`)
-            track dictionary iterator
-        xy (tuple of floats)
-            target longitude and latitude coordinate pair
-        distance_meters (int)
-            maximum distance in meters
-    '''
-    for track in tracks:
-        mask = [
-            haversine(track['lon'][i], track['lat'][i], xy[0], xy[1]) <
-            distance_meters for i in range(len(track['time']))
-        ]
-        if sum(mask) == 0:
-            continue
-        yield dict(
-            **{k: track[k]
-               for k in track['static']},
-            **{k: track[k][mask]
-               for k in track['dynamic']},
-            static=track['static'],
-            dynamic=track['dynamic'],
-        )
-
-
-class Domain():
-    ''' collection of zone geometry dictionaries, with additional
-        statistics such as hull bounding box
-
-        args:
-            name: string
-                Domain name
-            zones: list of dictionaries
-                Collection of zone geometry dictionaries.
-                Must have keys 'name' (string) and 'geometry'
-                (shapely.geometry.Polygon)
-
-        >>> domain = Domain(name='example', zones=[{
-        ...     'name': 'zone1',
-        ...     'geometry': shapely.geometry.Polygon([(-40,60), (-40, 61), (-41, 61), (-41, 60), (-40, 60)])
-        ...     }, ])
-
-        attr:
-            self.name
-            self.zones
-            self.boundary
-            self.minX
-            self.minY
-            self.maxX
-            self.maxY
-
-    '''
-
-    _meridian = LineString(
-        np.array((
-            (-180, -180, 180, 180),
-            (-90, 90, 90, -90),
-        )).T)
-
-    def _zone_max_radius(self, geom, zone_x, zone_y):
-        ''' computes the maximum distance to the centroid '''
-        return np.max([
-            haversine(geom.centroid.x, geom.centroid.y, x2, y2)
-            for x2, y2 in zip(zone_x, zone_y)
-        ])
-
-    def _add_zone(self, name, x, y):
-        '''
-        if name[-2:] == '_b':
-            if (x0b := np.min(x)) < self.minX_b:
-                self.minX_b = x0b
-            if (x0c := np.min(x)) > self.minX:
-                self.minX = x0c
-
-        elif name[-2:] == '_c':
-            if (x1b := np.max(x)) < self.maxX_c:
-                self.maxX_c = x1b
-            if (x1c := np.max(x)) > self.maxX:
-                self.maxX = x1c
-
-        else:
-        '''
-        if ((x0a := np.min(x)) < self.minX):
-            self.minX = x0a
-        if ((x1a := np.max(x)) > self.maxX):
-            self.maxX = x1a
-
-        if np.min(y) < self.minY:
-            self.minY = np.min(y)
-        if np.max(y) > self.maxY:
-            self.maxY = np.max(y)
-        '''
-        if np.min(x) < self.minX:
-            self.minX = np.min(x)
-        if np.max(x) > self.maxX:
-            self.maxX = np.max(x)
-        '''
-
-        assert self.minX < self.maxX
-        assert self.minY < self.maxY
-        assert -180 <= self.minX <= 180 and -180 <= self.maxX <= 180
-        assert -90 <= self.minY <= 90 and -90 <= self.maxY <= 90
-
-        geom = Polygon(zip(x, y))
-
-        self.zones.update({
-            name: {
-                'geometry': geom,
-                'maxradius': self._zone_max_radius(geom, x, y)
-            }
-        })
-
-        return
-
-    def _handle_outofbounds_zone(self, zone, zones_dir):
-        zones_west = zones_dir / 'west'
-        zones_east = zones_dir / 'east'
-        zones_corr = zones_dir / 'corr'
-        stringify = lambda x, y: map(
-            ','.join, zip(map(str, x), map(lambda y: y + '\n', map(str, y))))
-
-        for g in self.split_geom(zone):
-            if g.centroid.x < -180:
-                x, y = np.array(g.boundary.coords.xy)
-                if not os.path.isdir(zones_west):
-                    os.mkdir(zones_west)
-                with open(os.path.join(zones_west, zone['name'] + '_west.txt'),
-                          'w') as w:
-                    w.writelines(stringify(shiftcoord(x), y))
-            elif g.centroid.x > 180:
-                x, y = np.array(g.boundary.coords.xy)
-                if not os.path.isdir(zones_east):
-                    os.mkdir(zones_east)
-                with open(os.path.join(zones_east, zone['name'] + '_east.txt'),
-                          'w') as w:
-                    w.writelines(stringify(shiftcoord(x), y))
-            else:
-                x, y = np.array(g.boundary.coords.xy)
-                if not os.path.isdir(zones_corr):
-                    os.mkdir(zones_corr)
-                with open(os.path.join(zones_corr, zone['name'] + '_corr.txt'),
-                          'w') as w:
-                    w.writelines(stringify(x, y))
-
-    def __init__(self, name, zones=[], **kw):
-        ''' Initialize the domain from zone geometries '''
-
-        if len(zones) == 0:
-            raise ValueError(
-                'domain needs to have atleast one polygon geometry')
-        self.name = name
-        self.zones = {}
-        self.minX, self.maxX = 180, -180
-        # self.minX_b = 180
-        self.minY, self.maxY = 90, -90
-        # self.maxX_c = -180
-
-        valid_domain = True
-        zones_dir = pathlib.Path(tempfile.mkdtemp(prefix='aisdb_zones_'))
-
-        for zone in zones:
-            if 'name' not in zone.keys():
-                raise KeyError(f'Zone missing \'name\' key: {zone=}')
-            if 'geometry' not in zone.keys():
-                raise KeyError(f'Zone missing \'geometry\' key: {zone=}')
-
-            x, y = zone['geometry'].boundary.coords.xy
-            if not (np.min(x) >= -180 and np.max(x) <= 180):
-                #warnings.warn(f'dividing geometry... {zone["name"]}')
-                valid_domain = False
-                self._handle_outofbounds_zone(zone, zones_dir)
-            else:
-                self._add_zone(zone['name'], x, y)
-
-        if not valid_domain:
-            '''
-            if not os.path.isdir(os.path.dirname(
-                    zones_corr)) or not os.path.isdir(zones_corr):
-                print('Creating new output directory in ',
-                      os.path.dirname(zones_dir))
-                os.makedirs(zones_dir, exist_ok=True)
-            '''
-
-            for zonename, zone in self.zones.items():
-                zone['name'] = zonename
-                self._handle_outofbounds_zone(zone, zones_dir)
-
-            raise ValueError(
-                'Invalid zone geometry! '
-                'Exceeds longitude range -180 to 180. '
-                'If you want to query a bounding box spanning 180 degrees '
-                'longitude, consider querying multiple times instead.\n'
-                f'Saved modified geometries in {str(zones_dir)}, try using these corrected domains:\n'
-                f'\tdomain1 = aisdb.DomainFromTxts(domainName=\'{name}_corr\', folder={str(zones_dir)}{os.path.sep}corrected)\n'
-                f'\tdomain2 = aisdb.DomainFromTxts(domainName=\'{name}_west\', folder={str(zones_dir)}{os.path.sep}west))\n'
-                f'\tdomain3 = aisdb.DomainFromTxts(domainName=\'{name}_east\', folder={str(zones_dir)}{os.path.sep}east))\n'
-            )
-
-        assert self.minX < self.maxX
-        assert self.minY < self.maxY
-
-        self.boundary = {
-            'xmin': self.minX,
-            'xmax': self.maxX,
-            'ymin': self.minY,
-            'ymax': self.maxY
-        }
-
-    def nearest_polygons_to_point(self, x, y):
-        ''' compute great circle distance for this point to each polygon
-            centroid, subtracting the maximum polygon radius.
-            returns all zones with distances less than zero meters, sorted by
-            nearest first
-        '''
-        assert float(x) or x == 0.0, f'{type(x)} {x=}{y=}'
-        assert float(y) or y == 0.0, f'{type(y)} {x=}{y=}'
-        assert isinstance(self.zones, dict)
-        dist_to_centroids = {}
-        for name, z in self.zones.items():
-            dist_to_centroids.update({
-                name:
-                haversine(
-                    x,
-                    y,
-                    z['geometry'].centroid.x,
-                    z['geometry'].centroid.y,
-                ) - z['maxradius']
-            })
-        return dist_to_centroids
-
-    def point_in_polygon(self, x, y):
-        ''' Returns the zone containing the given coordinates.
-            if there are multiple zones containing the coordinates,
-            the zone with the nearest centroid will be selected.
-
-            args:
-                x (float)
-                    longitude value
-                y (float)
-                    latitude value
-        '''
-        assert float(x) or x == 0.0, f'{type(x)} {x=}{y=}'
-        assert float(y) or y == 0.0, f'{type(y)} {x=}{y=}'
-        assert len(self.zones) > 0
-        # first pass filter using distance to centroid, subtracting max radius.
-        # discard all geometry with a distance over zero
-        nearest = {
-            k: v
-            for k, v in sorted(self.nearest_polygons_to_point(x, y).items(),
-                               key=lambda item: item[1]) if v < 0
-        }
-        # check for zone containment, starting with the nearest centroid
-        for key, value in nearest.items():
-            if self.zones[key]['geometry'].contains(Point(x, y)):
-                return key
-        return 'Z0'
-
-    def split_geom(self, zone):
-        ''' Ensure that the zone doesn't intersect longitude 180 or -180.
-            If it does, divide it into two zones.
-        '''
-        merged = shapely.ops.linemerge(
-            [zone['geometry'].boundary, self._meridian])
-        border = shapely.ops.unary_union(merged)
-        decomp = shapely.ops.polygonize(border)
-        return decomp
-
-
-class DomainFromTxts(Domain):
-    ''' subclass of :class:`aisdb.gis.Domain`. used for convenience to load
-        zone geometry from .txt files directly
-    '''
-
-    def __init__(self, domainName, folder, ext='txt'):
-
-        files = glob_files(folder, ext=ext)
-        zones = []
-        for txt in files:
-            filename = txt.rsplit(os.path.sep, 1)[1].split('.')[0]
-            with open(txt, 'r') as f:
-                pts = f.read()
-            xy = list(
-                map(float,
-                    pts.replace('\n\n', '').replace('\n',
-                                                    ',').split(',')[:-1]))
-            x, y = np.array(xy[::2]), np.array(xy[1::2])
-            geom = Polygon(zip(x, y))
-            zones.append({'name': filename, 'geometry': geom})
-        super().__init__(domainName, zones, setattrs=False)
-
-
-class DomainFromPoints(Domain):
-    ''' Subclass of :class:`aisdb.gis.Domain`. Used for convenience to generate
-        bounding box polygons from longitude/latitude pairs and radial
-        distances, where the minimum radius is specified in meters.
-    '''
-
-    def __init__(self,
-                 points,
-                 radial_distances,
-                 names=[],
-                 domainName='domain'):
-        ''' Creates bounding-box polygons having a minimum radius atleast
-            approximately ``radial_distances`` in metres, centered on
-            ``points``.
-
-            args:
-                points (list)
-                    coordinate XY pairs
-                radial_distances (list)
-                    approximate distance in meters to extend the bounding box.
-                    the distance given will be used as the minimum distance to
-                    box boundaries
-                names (list)
-                    optionally assign a zone name for each point
-
-
-        '''
-        if names == []:
-            names = [f'{i:02d}' for i in range(len(points))]
-        zones = []
-        for xy, d, i in zip(points, radial_distances, names):
-            bounds = radial_coordinate_boundary(*xy, d)
-            geom = {
-                'name':
-                i,
-                'geometry':
-                Polygon([
-                    (bounds['xmin'], bounds['ymin']),
-                    (bounds['xmin'], bounds['ymax']),
-                    (bounds['xmax'], bounds['ymax']),
-                    (bounds['xmax'], bounds['ymin']),
-                    (bounds['xmin'], bounds['ymin']),
-                ]),
-            }
-            zones.append(geom)
-        super().__init__(name=domainName, zones=zones)
+'''Geometry and GIS utilities'''
+
+import os
+import pathlib
+import tempfile
+from datetime import datetime, timedelta
+from functools import partial
+
+import numpy as np
+import shapely.ops
+import shapely.geometry
+import warnings
+from shapely.geometry import Polygon, LineString, Point
+
+from aisdb.aisdb import haversine
+from aisdb.proc_util import glob_files
+
+
+def shiftcoord(x, rng=180):
+    ''' Correct longitude coordinates to be within range(-180, 180)
+        using a linear shift and modulus.
+        For latitude coordinate correction, set rng to 90.
+
+        For example: longitude 181 would be corrected to -179 deg.
+    '''
+    assert len(x) > 0, 'x must be array-like'
+    if not isinstance(x, np.ndarray):
+        x = np.array(x)
+    shift_idx = np.where(np.abs(x) != rng)[0]
+    for idx in shift_idx:
+        x[idx] = ((x[idx] + rng) % 360) - rng
+    flip_idx = np.where(np.abs(x) == rng)[0]
+    for idx in flip_idx:
+        x[idx] *= -1
+    assert (rng * -1 <= np.all(x) <= rng)
+    return x
+
+
+def dt_2_epoch(dt_arr, t0=datetime(1970, 1, 1, 0, 0, 0)):
+    ''' convert datetime.datetime to epoch minutes '''
+    delta = lambda dt: (dt - t0).total_seconds()
+    if isinstance(dt_arr, (list, np.ndarray)):
+        return np.array(list(map(float, map(delta, dt_arr))))
+    elif isinstance(dt_arr, (datetime)):
+        return int(delta(dt_arr))
+    else:
+        raise ValueError('input must be datetime or array of datetimes')
+
+
+def epoch_2_dt(ep_arr, t0=datetime(1970, 1, 1, 0, 0, 0), unit='seconds'):
+    ''' convert epoch minutes to datetime.datetime '''
+
+    delta = lambda ep, unit: t0 + timedelta(**{unit: ep})
+
+    if isinstance(ep_arr, (list, np.ndarray)):
+        return np.array(list(map(partial(delta, unit=unit), map(int, ep_arr))))
+
+    elif isinstance(ep_arr,
+                    (float, int, np.uint32, np.int32, np.uint64, np.int64)):
+        return delta(int(ep_arr), unit=unit)
+
+    else:
+        raise ValueError(
+            f'input must be integer or array of integers. got {ep_arr=}{type(ep_arr)}'
+        )
+
+
+def delta_meters(track, rng=None):
+    ''' compute haversine distance in meters between track positions for a
+        given track
+
+        args:
+            track (dict)
+                track vector dictionary
+            rng (range)
+                optionally restrict computed values to given index range
+    '''
+    rng = range(len(track['time'])) if rng is None else rng
+    return np.array(
+        list(
+            map(haversine, track['lon'][rng][:-1], track['lat'][rng][:-1],
+                track['lon'][rng][1:], track['lat'][rng][1:])))
+
+
+def delta_seconds(track, rng=None):
+    ''' compute elapsed time between track positions for a given track
+
+        args:
+            track (dict)
+                track vector dictionary
+            rng (range)
+                optionally restrict computed values to given index range
+    '''
+    if isinstance(track['time'], list):
+        track['time'] = np.array(track['time'])
+    assert isinstance(track['time'], np.ndarray), f'got {track["time"] = }'
+    rng = range(len(track['time'])) if rng is None else rng
+    return np.array(list((track['time'][rng][1:] - track['time'][rng][:-1])))
+
+
+def delta_knots(track, rng=None):
+    ''' compute speed over ground in knots between track positions for a given
+        track using (haversine distance / time)
+
+        args:
+            track (dict)
+                track vector dictionary
+            rng (range)
+                optionally restrict computed values to given index range
+    '''
+    rng = range(len(track['time'])) if rng is None else rng
+    ds = np.array([np.max((1, s)) for s in delta_seconds(track, rng)],
+                  dtype=object)
+    return delta_meters(track, rng) / ds * 1.9438445
+
+
+def radial_coordinate_boundary(x, y, radius=100000):
+    ''' Defines a bounding box area for a given point and radial
+        distance in meters. Returns degree boundaries with a minimum diameter
+        of approximately 2 * ``radius`` meters.
+
+        The boundaries are approximated by converting input coordinates
+        from degrees to radians, and computing a radial delta by
+        dividing an input value by the earth radius. The radial delta
+        is added or subtracted from the input point for each cardinal
+        direction, and then converted back from radians to degrees.
+
+        args:
+            x (float)
+                longitude
+            y (float)
+                latitude
+            radius (int, float)
+                minimum radial distance
+    '''
+    # radians
+    earth_radius_m = 6371088
+    rlon = np.pi * x / 180
+    rlat = np.pi * y / 180
+    parallel_radius = earth_radius_m * np.cos(rlat)
+
+    # radial delta
+    rlonmin = rlon - radius / parallel_radius
+    rlonmax = rlon + radius / parallel_radius
+    rlatmin = rlat - radius / earth_radius_m
+    rlatmax = rlat + radius / earth_radius_m
+
+    return {
+        'xmin': 180 * rlonmin / np.pi,
+        'xmax': 180 * rlonmax / np.pi,
+        'ymin': 180 * rlatmin / np.pi,
+        'ymax': 180 * rlatmax / np.pi
+    }
+
+
+def distance3D(x1, y1, x2, y2, depth_metres):
+    ''' haversine/pythagoras approximation of vessel distance to
+        point at given depth
+    '''
+    a2 = haversine(x1=x1, y1=y1, x2=x2, y2=y2)**2
+    b2 = abs(depth_metres)**2
+    c2 = a2 + b2
+    return np.sqrt(c2)
+
+
+def vesseltrack_3D_dist(tracks, x1, y1, z1, colname='distance_metres'):
+    ''' appends approximate distance to a submerged point at every
+        surface-level position. distance is approximated using the haversine
+        function and pythagoras.
+
+        x1 (float)
+            point longitude
+        y1 (float)
+            point latitude
+        z1 (float)
+            point depth (metres)
+        colname (string)
+            track dictionary key for which depth values will be set.
+            by default, distances are appended to the 'distance_metres'
+            key
+    '''
+    for track in tracks:
+        track['dynamic'] = track['dynamic'].union(set([colname]))
+        dists = [
+            distance3D(x1=x1, y1=y1, x2=x, y2=y, depth_metres=z1)
+            for x, y in zip(track['lon'], track['lat'])
+        ]
+        track[colname] = np.array(dists, dtype=object)
+        yield track
+
+
+def mask_in_radius_2D(tracks, xy, distance_meters):
+    ''' radial filtering using great circle distance at surface level
+
+        tracks (:class:`aisdb.track_gen.TrackGen`)
+            track dictionary iterator
+        xy (tuple of floats)
+            target longitude and latitude coordinate pair
+        distance_meters (int)
+            maximum distance in meters
+    '''
+    for track in tracks:
+        mask = [
+            haversine(track['lon'][i], track['lat'][i], xy[0], xy[1]) <
+            distance_meters for i in range(len(track['time']))
+        ]
+        if sum(mask) == 0:
+            continue
+        yield dict(
+            **{k: track[k]
+               for k in track['static']},
+            **{k: track[k][mask]
+               for k in track['dynamic']},
+            static=track['static'],
+            dynamic=track['dynamic'],
+        )
+
+
+class Domain():
+    ''' collection of zone geometry dictionaries, with additional
+        statistics such as hull bounding box
+
+        args:
+            name: string
+                Domain name
+            zones: list of dictionaries
+                Collection of zone geometry dictionaries.
+                Must have keys 'name' (string) and 'geometry'
+                (shapely.geometry.Polygon)
+
+        >>> domain = Domain(name='example', zones=[{
+        ...     'name': 'zone1',
+        ...     'geometry': shapely.geometry.Polygon([(-40,60), (-40, 61), (-41, 61), (-41, 60), (-40, 60)])
+        ...     }, ])
+
+        attr:
+            self.name
+            self.zones
+            self.boundary
+            self.minX
+            self.minY
+            self.maxX
+            self.maxY
+
+    '''
+
+    _meridian = LineString(
+        np.array((
+            (-180, -180, 180, 180),
+            (-90, 90, 90, -90),
+        )).T)
+
+    def _zone_max_radius(self, geom, zone_x, zone_y):
+        ''' computes the maximum distance to the centroid '''
+        return np.max([
+            haversine(geom.centroid.x, geom.centroid.y, x2, y2)
+            for x2, y2 in zip(zone_x, zone_y)
+        ])
+
+    def _add_zone(self, name, x, y):
+        '''
+        if name[-2:] == '_b':
+            if (x0b := np.min(x)) < self.minX_b:
+                self.minX_b = x0b
+            if (x0c := np.min(x)) > self.minX:
+                self.minX = x0c
+
+        elif name[-2:] == '_c':
+            if (x1b := np.max(x)) < self.maxX_c:
+                self.maxX_c = x1b
+            if (x1c := np.max(x)) > self.maxX:
+                self.maxX = x1c
+
+        else:
+        '''
+        if ((x0a := np.min(x)) < self.minX):
+            self.minX = x0a
+        if ((x1a := np.max(x)) > self.maxX):
+            self.maxX = x1a
+
+        if np.min(y) < self.minY:
+            self.minY = np.min(y)
+        if np.max(y) > self.maxY:
+            self.maxY = np.max(y)
+        '''
+        if np.min(x) < self.minX:
+            self.minX = np.min(x)
+        if np.max(x) > self.maxX:
+            self.maxX = np.max(x)
+        '''
+
+        assert self.minX < self.maxX
+        assert self.minY < self.maxY
+        assert -180 <= self.minX <= 180 and -180 <= self.maxX <= 180
+        assert -90 <= self.minY <= 90 and -90 <= self.maxY <= 90
+
+        geom = Polygon(zip(x, y))
+
+        self.zones.update({
+            name: {
+                'geometry': geom,
+                'maxradius': self._zone_max_radius(geom, x, y)
+            }
+        })
+
+        return
+
+    def _handle_outofbounds_zone(self, zone, zones_dir):
+        zones_west = zones_dir / 'west'
+        zones_east = zones_dir / 'east'
+        zones_corr = zones_dir / 'corr'
+        stringify = lambda x, y: map(
+            ','.join, zip(map(str, x), map(lambda y: y + '\n', map(str, y))))
+
+        for g in self.split_geom(zone):
+            if g.centroid.x < -180:
+                x, y = np.array(g.boundary.coords.xy)
+                if not os.path.isdir(zones_west):
+                    os.mkdir(zones_west)
+                with open(os.path.join(zones_west, zone['name'] + '_west.txt'),
+                          'w') as w:
+                    w.writelines(stringify(shiftcoord(x), y))
+            elif g.centroid.x > 180:
+                x, y = np.array(g.boundary.coords.xy)
+                if not os.path.isdir(zones_east):
+                    os.mkdir(zones_east)
+                with open(os.path.join(zones_east, zone['name'] + '_east.txt'),
+                          'w') as w:
+                    w.writelines(stringify(shiftcoord(x), y))
+            else:
+                x, y = np.array(g.boundary.coords.xy)
+                if not os.path.isdir(zones_corr):
+                    os.mkdir(zones_corr)
+                with open(os.path.join(zones_corr, zone['name'] + '_corr.txt'),
+                          'w') as w:
+                    w.writelines(stringify(x, y))
+
+    def __init__(self, name, zones=[], **kw):
+        ''' Initialize the domain from zone geometries '''
+
+        if len(zones) == 0:
+            raise ValueError(
+                'domain needs to have atleast one polygon geometry')
+        self.name = name
+        self.zones = {}
+        self.minX, self.maxX = 180, -180
+        # self.minX_b = 180
+        self.minY, self.maxY = 90, -90
+        # self.maxX_c = -180
+
+        valid_domain = True
+        zones_dir = pathlib.Path(tempfile.mkdtemp(prefix='aisdb_zones_'))
+
+        for zone in zones:
+            if 'name' not in zone.keys():
+                raise KeyError(f'Zone missing \'name\' key: {zone=}')
+            if 'geometry' not in zone.keys():
+                raise KeyError(f'Zone missing \'geometry\' key: {zone=}')
+
+            x, y = zone['geometry'].boundary.coords.xy
+            if not (np.min(x) >= -180 and np.max(x) <= 180):
+                #warnings.warn(f'dividing geometry... {zone["name"]}')
+                valid_domain = False
+                self._handle_outofbounds_zone(zone, zones_dir)
+            else:
+                self._add_zone(zone['name'], x, y)
+
+        if not valid_domain:
+            '''
+            if not os.path.isdir(os.path.dirname(
+                    zones_corr)) or not os.path.isdir(zones_corr):
+                print('Creating new output directory in ',
+                      os.path.dirname(zones_dir))
+                os.makedirs(zones_dir, exist_ok=True)
+            '''
+
+            for zonename, zone in self.zones.items():
+                zone['name'] = zonename
+                self._handle_outofbounds_zone(zone, zones_dir)
+
+            raise ValueError(
+                'Invalid zone geometry! '
+                'Exceeds longitude range -180 to 180. '
+                'If you want to query a bounding box spanning 180 degrees '
+                'longitude, consider querying multiple times instead.\n'
+                f'Saved modified geometries in {str(zones_dir)}, try using these corrected domains:\n'
+                f'\tdomain1 = aisdb.DomainFromTxts(domainName=\'{name}_corr\', folder={str(zones_dir)}{os.path.sep}corrected)\n'
+                f'\tdomain2 = aisdb.DomainFromTxts(domainName=\'{name}_west\', folder={str(zones_dir)}{os.path.sep}west))\n'
+                f'\tdomain3 = aisdb.DomainFromTxts(domainName=\'{name}_east\', folder={str(zones_dir)}{os.path.sep}east))\n'
+            )
+
+        assert self.minX < self.maxX
+        assert self.minY < self.maxY
+
+        self.boundary = {
+            'xmin': self.minX,
+            'xmax': self.maxX,
+            'ymin': self.minY,
+            'ymax': self.maxY
+        }
+
+    def nearest_polygons_to_point(self, x, y):
+        ''' compute great circle distance for this point to each polygon
+            centroid, subtracting the maximum polygon radius.
+            returns all zones with distances less than zero meters, sorted by
+            nearest first
+        '''
+        assert float(x) or x == 0.0, f'{type(x)} {x=}{y=}'
+        assert float(y) or y == 0.0, f'{type(y)} {x=}{y=}'
+        assert isinstance(self.zones, dict)
+        dist_to_centroids = {}
+        for name, z in self.zones.items():
+            dist_to_centroids.update({
+                name:
+                haversine(
+                    x,
+                    y,
+                    z['geometry'].centroid.x,
+                    z['geometry'].centroid.y,
+                ) - z['maxradius']
+            })
+        return dist_to_centroids
+
+    def point_in_polygon(self, x, y):
+        ''' Returns the zone containing the given coordinates.
+            if there are multiple zones containing the coordinates,
+            the zone with the nearest centroid will be selected.
+
+            args:
+                x (float)
+                    longitude value
+                y (float)
+                    latitude value
+        '''
+        assert float(x) or x == 0.0, f'{type(x)} {x=}{y=}'
+        assert float(y) or y == 0.0, f'{type(y)} {x=}{y=}'
+        assert len(self.zones) > 0
+        # first pass filter using distance to centroid, subtracting max radius.
+        # discard all geometry with a distance over zero
+        nearest = {
+            k: v
+            for k, v in sorted(self.nearest_polygons_to_point(x, y).items(),
+                               key=lambda item: item[1]) if v < 0
+        }
+        # check for zone containment, starting with the nearest centroid
+        for key, value in nearest.items():
+            if self.zones[key]['geometry'].contains(Point(x, y)):
+                return key
+        return 'Z0'
+
+    def split_geom(self, zone):
+        ''' Ensure that the zone doesn't intersect longitude 180 or -180.
+            If it does, divide it into two zones.
+        '''
+        merged = shapely.ops.linemerge(
+            [zone['geometry'].boundary, self._meridian])
+        border = shapely.ops.unary_union(merged)
+        decomp = shapely.ops.polygonize(border)
+        return decomp
+
+
+class DomainFromTxts(Domain):
+    ''' subclass of :class:`aisdb.gis.Domain`. used for convenience to load
+        zone geometry from .txt files directly
+    '''
+
+    def __init__(self, domainName, folder, ext='txt'):
+
+        files = glob_files(folder, ext=ext)
+        zones = []
+        for txt in files:
+            filename = txt.rsplit(os.path.sep, 1)[1].split('.')[0]
+            with open(txt, 'r') as f:
+                pts = f.read()
+            xy = list(
+                map(float,
+                    pts.replace('\n\n', '').replace('\n',
+                                                    ',').split(',')[:-1]))
+            x, y = np.array(xy[::2]), np.array(xy[1::2])
+            geom = Polygon(zip(x, y))
+            zones.append({'name': filename, 'geometry': geom})
+        super().__init__(domainName, zones, setattrs=False)
+
+
+class DomainFromPoints(Domain):
+    ''' Subclass of :class:`aisdb.gis.Domain`. Used for convenience to generate
+        bounding box polygons from longitude/latitude pairs and radial
+        distances, where the minimum radius is specified in meters.
+    '''
+
+    def __init__(self,
+                 points,
+                 radial_distances,
+                 names=[],
+                 domainName='domain'):
+        ''' Creates bounding-box polygons having a minimum radius atleast
+            approximately ``radial_distances`` in metres, centered on
+            ``points``.
+
+            args:
+                points (list)
+                    coordinate XY pairs
+                radial_distances (list)
+                    approximate distance in meters to extend the bounding box.
+                    the distance given will be used as the minimum distance to
+                    box boundaries
+                names (list)
+                    optionally assign a zone name for each point
+
+
+        '''
+        if names == []:
+            names = [f'{i:02d}' for i in range(len(points))]
+        zones = []
+        for xy, d, i in zip(points, radial_distances, names):
+            bounds = radial_coordinate_boundary(*xy, d)
+            geom = {
+                'name':
+                i,
+                'geometry':
+                Polygon([
+                    (bounds['xmin'], bounds['ymin']),
+                    (bounds['xmin'], bounds['ymax']),
+                    (bounds['xmax'], bounds['ymax']),
+                    (bounds['xmax'], bounds['ymin']),
+                    (bounds['xmin'], bounds['ymin']),
+                ]),
+            }
+            zones.append(geom)
+        super().__init__(name=domainName, zones=zones)
```

## aisdb/interp.py

 * *Ordering differences only*

```diff
@@ -1,56 +1,56 @@
-''' linear interpolation of track segments on temporal axis '''
-
-from datetime import timedelta
-
-import numpy as np
-import warnings
-
-
-def np_interp_linear(track, key, intervals):
-    assert len(track['time']) == len(track[key])
-    return np.interp(x=intervals.astype(int),
-                     xp=track['time'].astype(int),
-                     fp=track[key].astype(float))
-
-
-def interp_time(tracks, step=timedelta(minutes=10)):
-    ''' linear interpolation on vessel trajectory
-
-        args:
-            tracks (dict)
-                messages sorted by mmsi then time.
-                uses mmsi as key with columns: time lon lat cog sog name .. etc
-            step (datetime.timedelta)
-                interpolation interval
-
-        returns:
-            dictionary of interpolated tracks
-    '''
-    for track in tracks:
-        if track['time'].size <= 1:
-            # yield track
-            warnings.warn('cannot interpolate track of length 1, skipping...')
-            continue
-
-        intervals = np.arange(
-            start=track['time'][0],
-            stop=track['time'][-1] + int(step.total_seconds()),
-            step=int(step.total_seconds()),
-        ).astype(int)
-
-        assert len(intervals) >= 1
-
-        itr = dict(
-            **{k: track[k]
-               for k in track['static']},
-            time=intervals,
-            static=track['static'],
-            dynamic=track['dynamic'],
-            **{
-                k: np_interp_linear(track, k, intervals)
-                for k in track['dynamic'] if k != 'time'
-            },
-        )
-        yield itr
-
-    return
+''' linear interpolation of track segments on temporal axis '''
+
+from datetime import timedelta
+
+import numpy as np
+import warnings
+
+
+def np_interp_linear(track, key, intervals):
+    assert len(track['time']) == len(track[key])
+    return np.interp(x=intervals.astype(int),
+                     xp=track['time'].astype(int),
+                     fp=track[key].astype(float))
+
+
+def interp_time(tracks, step=timedelta(minutes=10)):
+    ''' linear interpolation on vessel trajectory
+
+        args:
+            tracks (dict)
+                messages sorted by mmsi then time.
+                uses mmsi as key with columns: time lon lat cog sog name .. etc
+            step (datetime.timedelta)
+                interpolation interval
+
+        returns:
+            dictionary of interpolated tracks
+    '''
+    for track in tracks:
+        if track['time'].size <= 1:
+            # yield track
+            warnings.warn('cannot interpolate track of length 1, skipping...')
+            continue
+
+        intervals = np.arange(
+            start=track['time'][0],
+            stop=track['time'][-1] + int(step.total_seconds()),
+            step=int(step.total_seconds()),
+        ).astype(int)
+
+        assert len(intervals) >= 1
+
+        itr = dict(
+            **{k: track[k]
+               for k in track['static']},
+            time=intervals,
+            static=track['static'],
+            dynamic=track['dynamic'],
+            **{
+                k: np_interp_linear(track, k, intervals)
+                for k in track['dynamic'] if k != 'time'
+            },
+        )
+        yield itr
+
+    return
```

## aisdb/network_graph.py

 * *Ordering differences only*

```diff
@@ -1,487 +1,487 @@
-'''
-    collect vessel transits between domain zones (graph nodes), and aggregate
-    trajectory statistics within the overall domain
-'''
-
-import os
-import pickle
-import re
-import tempfile
-import types
-from datetime import timedelta
-from functools import partial, reduce
-
-import numpy as np
-import warnings
-
-import aisdb
-from aisdb.database import sqlfcn
-from aisdb.gis import (
-    delta_knots,
-    delta_meters,
-    epoch_2_dt,
-)
-from aisdb.track_gen import (
-    TrackGen,
-    fence_tracks,
-    split_timedelta,
-)
-from aisdb.denoising_encoder import encode_greatcircledistance
-from aisdb.database.dbconn import ConnectionType
-from aisdb.interp import interp_time
-from aisdb.proc_util import _sanitize
-from aisdb.proc_util import _segment_rng
-from aisdb.webdata.bathymetry import Gebco
-from aisdb.webdata.marinetraffic import vessel_info, VesselInfo
-from aisdb.webdata.shore_dist import ShoreDist, PortDist
-from aisdb.wsa import wetted_surface_area
-
-
-def _fstr(s):
-    return f'{float(s):.2f}'
-
-
-def _depth_nonnegative(track, zoneset):
-    ''' returns absolute value of bathymetric depths with topographic heights
-        converted to 0
-    '''
-    return np.array(
-        [d if d >= 0 else 0 for d in track['depth_metres'][zoneset]])
-
-
-def _time_in_shoredist_rng(track, subset, dist0=0.01, dist1=5):
-    ''' returns minutes spent within kilometers range from shore '''
-    return sum(t for t in map(
-        len,
-        _segment_rng(
-            {
-                'time':
-                track['time'][subset]
-                [[dist0 <= d <= dist1 for d in track['km_from_shore'][subset]]]
-            },
-            maxdelta=timedelta(minutes=1),
-            key='time'),
-    ))
-
-
-def _staticinfo(track, domain):
-    ''' collect categorical vessel data as a dictionary '''
-    static = {'mmsi': track['mmsi']}
-    for key in track['marinetraffic_info'].keys():
-        if key in static.keys() or key not in track['marinetraffic_info'].keys(
-        ):
-            continue
-        static.update({key: _sanitize(track['marinetraffic_info'][key])})
-    for key in ['label', 'hull_submerged_m^2']:
-        if key in static.keys() or key not in track.keys():
-            continue
-        static.update({key: _sanitize(f'{track[key]:.0f}')})
-    return static
-
-
-def _transitinfo(track, zoneset, interp_resolution=timedelta(hours=1)):
-    ''' aggregate statistics on vessel network graph connectivity '''
-
-    dynamic = {}
-
-    # geofencing
-    dynamic.update(
-        dict(
-            src_zone=int(re.sub('[^0-9]', '', track['in_zone'][zoneset][0])),
-            rcv_zone=int(re.sub('[^0-9]', '', track['in_zone'][zoneset][-1])),
-            transit_nodes=
-            f"{track['in_zone'][zoneset][0]}_{track['in_zone'][zoneset][-1]}"))
-
-    # timestamp info
-    dynamic.update(
-        dict(first_seen_in_zone=epoch_2_dt(
-            track['time'][zoneset][0]).strftime('%Y-%m-%d %H:%M UTC'),
-             last_seen_in_zone=epoch_2_dt(
-                 track['time'][zoneset][-1]).strftime('%Y-%m-%d %H:%M UTC'),
-             year=epoch_2_dt(track['time'][zoneset][0]).year,
-             month=epoch_2_dt(track['time'][zoneset][0]).month,
-             day=epoch_2_dt(track['time'][zoneset][0]).day))
-
-    # distance travelled
-    dynamic.update(
-        dict(total_distance_meters=np.sum(delta_meters(
-            track, zoneset[[0, -1]])).astype(int),
-             cumulative_distance_meters=np.sum(delta_meters(
-                 track, zoneset)).astype(int)))
-    # shore dist
-    if 'km_from_shore' in track.keys():
-        dynamic.update(
-            dict(
-                min_shore_dist=f"{np.min(track['km_from_shore'][zoneset]):.2f}",
-                avg_shore_dist=
-                f"{np.average(track['km_from_shore'][zoneset]):.2f}"
-                if 'km_from_shore' in track.keys() else None,
-                max_shore_dist=f"{np.max(track['km_from_shore'][zoneset]):.2f}"
-                if 'km_from_shore' in track.keys() else None,
-            ))
-        # elapsed time in distance from shore
-        dynamic.update(
-            dict(
-                minutes_within_10m_5km_shoredist=_time_in_shoredist_rng(
-                    track, zoneset, 0.01, 5),
-                minutes_within_30m_20km_shoredist=_time_in_shoredist_rng(
-                    track, zoneset, 0.03, 20),
-                minutes_within_100m_50km_shoredist=_time_in_shoredist_rng(
-                    track, zoneset, 0.1, 50),
-            ))
-
-    # port dist
-    if 'km_from_port' in track.keys():
-        dynamic.update(
-            dict(
-                min_port_dist=_fstr(np.min(track['km_from_port'][zoneset])),
-                avg_port_dist=_fstr(np.average(track['km_from_port'][zoneset]))
-                if 'km_from_port' in track.keys() else None,
-                max_port_dist=_fstr(np.max(track['km_from_port'][zoneset]))
-                if 'km_from_port' in track.keys() else None,
-            ))
-
-    # depth charts
-    if 'depth_metres' in track.keys():
-        dynamic.update(
-            dict(
-                min_depth=_fstr(np.min(_depth_nonnegative(track, zoneset)))
-                if 'depth_metres' in track.keys() else None,
-                avg_depth=_fstr(np.average(_depth_nonnegative(track, zoneset)))
-                if 'depth_metres' in track.keys() else None,
-                max_depth=_fstr(np.max(_depth_nonnegative(track, zoneset)))
-                if 'depth_metres' in track.keys() else None,
-            ))
-
-    # computed velocity (knots)
-    dynamic.update(
-        dict(
-            velocity_knots_min=f"{np.min(delta_knots(track, zoneset)):.2f}"
-            if len(zoneset) > 1 else 'NULL',
-            velocity_knots_avg=f"{np.average(delta_knots(track, zoneset)):.2f}"
-            if len(zoneset) > 1 else 'NULL',
-            velocity_knots_max=f"{np.max(delta_knots(track, zoneset)):.2f}"
-            if len(zoneset) > 1 else 'NULL',
-        ))
-
-    # elapsed time spent in zones
-    dynamic.update(
-        dict(minutes_spent_in_zone=_fstr(
-            (epoch_2_dt(track['time'][zoneset][-1]) -
-             epoch_2_dt(track['time'][zoneset][0])).total_seconds() /
-            60) if len(zoneset) > 1 else 'NULL', ))
-
-    return dynamic
-
-
-def _serialize_network_edge(tracks, domain, tmp_dir):
-    ''' at each track position where the zone changes, a transit
-        index is recorded, and trajectory statistics are aggregated for this
-        index range using _staticinfo() and _transitinfo()
-
-        results will be serialized as binary files labelled by mmsi into the
-        'tmp_dir' directory, as defined in the config file. see graph() for
-        deserialization and concatenation of results
-
-        args:
-            tracks: dict
-                dictionary of vessel trajectory data, as output by
-                ais.track_gen.TrackGen() or its wrapper functions
-
-        returns: None
-    '''
-    for track in tracks:
-        assert isinstance(track, dict)
-        assert len(track['time']) > 0
-        filepath = os.path.join(tmp_dir, str(track['mmsi']).zfill(9))
-        assert 'in_zone' in track.keys(
-        ), 'need to append zone info from fence_tracks'
-
-        with open(filepath, 'ab') as f:
-            transits = np.where(
-                track['in_zone'][:-1] != track['in_zone'][1:])[0] + 1
-
-            for i in range(len(transits) - 1):
-                rng = np.array(range(transits[i], transits[i + 1] + 1))
-                track_stats = _staticinfo(track, domain)
-                track_stats.update(_transitinfo(track, rng))
-                pickle.dump(track_stats, f)
-
-            i0 = transits[-1] if len(transits) >= 1 else 0
-            rng = np.array(range(i0, len(track['in_zone'])))
-            track_stats = _staticinfo(track, domain)
-            track_stats.update(_transitinfo(track, rng))
-            track_stats['rcv_zone'] = 'NULL'
-            track_stats['transit_nodes'] = track_stats['src_zone']
-            pickle.dump(track_stats, f)
-        yield
-
-
-def _aggregate_output(outputfile, tmp_dir, filters=[lambda row: False]):
-    ''' concatenate serialized output from geofence()
-
-        args:
-            outputfile (string)
-                filepath location to output CSV data
-            tmp_dir (string)
-                files will temporarily be placed here while processing
-            filters (list)
-                list of callback functions. each callable function should
-                accept a dictionary describing a network edge as input. if any
-                return True, the edge will be filtered from the output rows.
-                see _staticinfo() and _transitinfo() for more info on
-                network edge dict keys
-
-                for example, to filter all rows where the max speed exceeds 50
-                knots, and filter non-transiting vessels from zone Z0:
-
-        >>> filters = [
-        ...     lambda r: float(r['velocity_knots_max']) > 50,
-        ...     lambda r: r['src_zone'] == '0' and r['rcv_zone'] == 'NULL'
-        ...     ]
-    '''
-    assert os.path.isdir(
-        os.path.dirname(outputfile)), f'no directory for {outputfile}!'
-
-    picklefiles = [
-        os.path.join(tmp_dir, fname) for fname in sorted(os.listdir(tmp_dir))
-        if '_' not in fname
-    ]
-    assert len(picklefiles) > 0, 'failed to geofence any data...'
-
-    with open(outputfile, 'w') as output:
-        with open(picklefiles[0], 'rb') as f0:
-            getrow = pickle.load(f0)
-            output.write(','.join(map(str, getrow.keys())) + '\n')
-
-        for picklefile in picklefiles:
-            results = []
-            with open(picklefile, 'rb') as f:
-                while True:
-                    try:
-                        getrow = pickle.load(f)
-                    except EOFError:
-                        break
-                    except Exception as e:
-                        raise e
-                    if not reduce(np.logical_or,
-                                  [f(getrow)
-                                   for f in filters]):  # pragma: no cover
-                        results.append(','.join(map(str, getrow.values())))
-
-            if len(results) == 0:
-                warnings.warn(f'no results for {outputfile}')
-            else:
-                output.write('\n'.join(results) + '\n')
-
-            os.remove(picklefile)
-
-
-def graph(
-        qry,
-        *,
-        outputfile,
-        domain,
-        dbconn: ConnectionType,
-        data_dir: str,
-        #dbpath: str = None,
-        trafficDBpath: str or None,  # none if using PostgresDBConn
-        maxdelta: timedelta = timedelta(weeks=1),
-        speed_threshold: float = 50,
-        distance_threshold: float = 200000,
-        interp_delta: float = timedelta(minutes=10),
-        minscore: float = 0,
-        qryfcn=sqlfcn.crawl_dynamic_static,
-        bathy_dir: str = None,
-        shoredist_raster: str = None,
-        portdist_raster: str = None,
-        decimate: float = 0.0001,
-        verbose: bool = False):
-    ''' Compute network graph of vessel movements within domain zones.
-        Zone polygons will be used as network nodes, with graph edges
-        represented by movements between zones.
-
-        args:
-            qry (:py:class:`aisdb.database.dbqry.DBQuery`)
-                database query generator
-            domain (:py:class:`aisdb.gis.Domain`)
-                collection of zones defined as polygons, these will
-                be used as nodes in the network graph
-            dbconn (ConnectionType)
-                Either a :class:`aisdb.database.dbconn.SQLiteDBConn` or
-                :class:`aisdb.database.dbconn.PostgresDBConn` database
-                connection objects
-            data_dir (string)
-                location of raster data
-            trafficDBpath (string)
-                path to marinetraffic database file
-            outpufile (string)
-                filepath for resulting CSV output
-            maxdelta (datetime.timedelta)
-                maximum time between vessel messages before considering
-                it to be part of a new trajectory. See
-                :func:`aisdb.track_gen.split_timedelta` for more info
-            speed_threshold (int, float)
-                maximum speed in knots for encoder segmentation. See
-                :func:`aisdb.denoising_encoder.encode_greatcircledistance` for
-                more info
-            distance_threshold (int, float)
-                maximum distance in meters for encoder segmentation. See
-                :func:`aisdb.denoising_encoder.encode_greatcircledistance` for
-                more info
-            interp_delta (timedelta)
-                track positions will be interpolated to the given sample rate
-            minscore (float)
-                minimum score for segments to be considered sequential. See
-                :func:`aisdb.denoising_encoder.encode_greatcircledistance` for
-                more info
-
-        Network graph activity is computed following these steps:
-
-            - Create database query with
-              :meth:`aisdb.database.dbqry.DBQuery.gen_qry`, and supply
-              resulting generator as rowgen arg. Define a domain
-              (:class:`aisdb.gis.Domain`) in which to compute movements
-            - Vectorize tracks using :py:func:`aisdb.track_gen.TrackGen`
-            - Append vessel metadata to track vessels with
-              :func:`aisdb.webdata.marinetraffic.vessel_info`
-            - Segment track vectors where time between messages exceeds
-              maxdelta using :func:`aisdb.track_gen.split_timedelta`
-            - Segment track vectors as encoded by
-              :py:func:`aisdb.denoising_encoder.encode_greatcircledistance`
-            - Perform geofencing on track segments using
-              :py:func:`aisdb.track_gen.fence_tracks` to determine zone
-              containment
-            - Check where zone boundaries are transited and serialize results
-              to ``outputfile``. Additional metrics per zone activity is also
-              aggregated at this step.
-
-        Example usage:
-
-        >>> import os
-        >>> import shapely
-        >>> from datetime import datetime
-        >>> from aisdb import DBConn, DBQuery, Domain, graph, decode_msgs
-        >>> from aisdb.database.sqlfcn_callbacks import in_bbox_time
-
-        >>> # create example database file
-        >>> dbpath = './example.sqlitedb'
-        >>> filepaths = ['./aisdb/tests/testdata/test_data_20210701.csv',
-        ...              './aisdb/tests/testdata/test_data_20211101.nm4']
-        >>> with DBConn() as dbconn:
-        ...     decode_msgs(filepaths=filepaths, dbconn=dbconn, dbpath=dbpath,
-        ...     source='TESTING')
-
-        Next, configure query area using Domain to compute region boundary
-
-        >>> zones = [{
-        ...     'name': 'Zone1',
-        ...     'geometry': shapely.geometry.Polygon(zip(
-        ...             [-170.24, -170.24, -38.5, -38.5, -170.24],
-        ...             [29.0, 75.2, 75.2, 29.0, 29.0],
-        ...         ))
-        ...     }]
-        >>> domain = Domain(name='new_domain', zones=zones)
-        >>> trafficDBpath = './testdata/marinetraffic_test.db'
-        >>> data_dir = os.environ.get('AISDBDATADIR', '/tmp/ais/')
-
-        Then, query db for points in domain
-
-        >>> with DBConn() as dbconn:
-        ...     qry = DBQuery(
-        ...             dbconn=dbconn,
-        ...             dbpath=dbpath,
-        ...             callback=in_bbox_time,
-        ...             start=datetime(2021, 7, 1),
-        ...             end=datetime(2021, 7, 3),
-        ...             **domain.boundary,
-        ...         )
-        ...     graph(qry,
-        ...           outputfile=os.path.join('testdata', 'test_graph.csv'),
-        ...           dbconn=dbconn,
-        ...           domain=domain,
-        ...           data_dir=data_dir,
-        ...           trafficDBpath=trafficDBpath)
-
-        Afterwards, delete the example database file
-
-        >>> os.remove(dbpath)
-        >>> os.remove(os.path.join('testdata', 'test_graph.csv'))
-
-        process the vessel movement graph edges.
-        caution: this may consume a large amount of memory
-    '''
-    assert not isinstance(qry, types.GeneratorType),\
-            'Got a generator for "qry" arg instead of DBQuery'
-
-    assert isinstance(qry, aisdb.database.dbqry.DBQuery),\
-            f'Not a DBQuery object! Got {qry}'
-
-    if not isinstance(dbconn, (
-            ConnectionType.SQLITE.value,
-            ConnectionType.POSTGRES.value,
-    )):
-        raise ValueError("Invalid dbconn connection type")
-    if isinstance(dbconn, ConnectionType.SQLITE.value):
-        assert trafficDBpath is not None
-        assert isinstance(trafficDBpath, str)
-        vinfoDB = VesselInfo(trafficDBpath).trafficDB
-    else:
-        vinfoDB = dbconn
-
-    rowgen = qry.gen_qry(fcn=qryfcn, verbose=verbose)
-    tracks = TrackGen(rowgen, decimate)
-
-    if portdist_raster is not None:
-        pdist = PortDist(portdist_raster)
-        with pdist:
-            tracks = list(pdist.get_distance(tracks))
-
-    if shoredist_raster is not None:
-        sdist_dir, sdist_name = shoredist_raster.rsplit(os.path.sep, 1)
-        sdist = ShoreDist(sdist_dir, sdist_name)
-        with sdist:
-            tracks = list(sdist.get_distance(tracks))
-
-    if bathy_dir is not None:
-        bathy = Gebco(data_dir=bathy_dir)
-        with bathy:
-            tracks = list(bathy.merge_tracks(tracks))
-
-    # initialize raster data sources
-    if not os.path.isdir('/tmp'):  # pragma: no cover
-        os.mkdir('/tmp')
-    with tempfile.TemporaryDirectory() as tmp_dir:
-        if os.environ.get('DEBUG'):
-            print(f'network graph {tmp_dir = }')
-            print(f'\n{domain.name=} {domain.boundary=}')
-
-        # configure processing pipeline
-        serialize_CSV = partial(_serialize_network_edge,
-                                domain=domain,
-                                tmp_dir=tmp_dir)
-        geofence = partial(fence_tracks, domain=domain)
-        interp = partial(interp_time, step=interp_delta)
-        encode_tracks = partial(encode_greatcircledistance,
-                                distance_threshold=distance_threshold,
-                                minscore=minscore,
-                                speed_threshold=speed_threshold)
-        timesplit = partial(split_timedelta, maxdelta=maxdelta)
-        vinfo = partial(vessel_info, dbconn=vinfoDB)
-
-        # pipeline execution order
-        tracks = vinfo(tracks)
-        tracks = wetted_surface_area(tracks)
-        tracks = timesplit(tracks)
-        tracks = encode_tracks(tracks)
-        tracks = interp(tracks)
-        tracks = geofence(tracks)
-        result = serialize_CSV(tracks)
-
-        for res in result:
-            assert res is None
-
-        if os.listdir(tmp_dir) == []:
-            warnings.warn(f'no data for {outputfile}, skipping...\n')
-        else:
-            _aggregate_output(outputfile=outputfile, tmp_dir=tmp_dir)
+'''
+    collect vessel transits between domain zones (graph nodes), and aggregate
+    trajectory statistics within the overall domain
+'''
+
+import os
+import pickle
+import re
+import tempfile
+import types
+from datetime import timedelta
+from functools import partial, reduce
+
+import numpy as np
+import warnings
+
+import aisdb
+from aisdb.database import sqlfcn
+from aisdb.gis import (
+    delta_knots,
+    delta_meters,
+    epoch_2_dt,
+)
+from aisdb.track_gen import (
+    TrackGen,
+    fence_tracks,
+    split_timedelta,
+)
+from aisdb.denoising_encoder import encode_greatcircledistance
+from aisdb.database.dbconn import ConnectionType
+from aisdb.interp import interp_time
+from aisdb.proc_util import _sanitize
+from aisdb.proc_util import _segment_rng
+from aisdb.webdata.bathymetry import Gebco
+from aisdb.webdata.marinetraffic import vessel_info, VesselInfo
+from aisdb.webdata.shore_dist import ShoreDist, PortDist
+from aisdb.wsa import wetted_surface_area
+
+
+def _fstr(s):
+    return f'{float(s):.2f}'
+
+
+def _depth_nonnegative(track, zoneset):
+    ''' returns absolute value of bathymetric depths with topographic heights
+        converted to 0
+    '''
+    return np.array(
+        [d if d >= 0 else 0 for d in track['depth_metres'][zoneset]])
+
+
+def _time_in_shoredist_rng(track, subset, dist0=0.01, dist1=5):
+    ''' returns minutes spent within kilometers range from shore '''
+    return sum(t for t in map(
+        len,
+        _segment_rng(
+            {
+                'time':
+                track['time'][subset]
+                [[dist0 <= d <= dist1 for d in track['km_from_shore'][subset]]]
+            },
+            maxdelta=timedelta(minutes=1),
+            key='time'),
+    ))
+
+
+def _staticinfo(track, domain):
+    ''' collect categorical vessel data as a dictionary '''
+    static = {'mmsi': track['mmsi']}
+    for key in track['marinetraffic_info'].keys():
+        if key in static.keys() or key not in track['marinetraffic_info'].keys(
+        ):
+            continue
+        static.update({key: _sanitize(track['marinetraffic_info'][key])})
+    for key in ['label', 'hull_submerged_m^2']:
+        if key in static.keys() or key not in track.keys():
+            continue
+        static.update({key: _sanitize(f'{track[key]:.0f}')})
+    return static
+
+
+def _transitinfo(track, zoneset, interp_resolution=timedelta(hours=1)):
+    ''' aggregate statistics on vessel network graph connectivity '''
+
+    dynamic = {}
+
+    # geofencing
+    dynamic.update(
+        dict(
+            src_zone=int(re.sub('[^0-9]', '', track['in_zone'][zoneset][0])),
+            rcv_zone=int(re.sub('[^0-9]', '', track['in_zone'][zoneset][-1])),
+            transit_nodes=
+            f"{track['in_zone'][zoneset][0]}_{track['in_zone'][zoneset][-1]}"))
+
+    # timestamp info
+    dynamic.update(
+        dict(first_seen_in_zone=epoch_2_dt(
+            track['time'][zoneset][0]).strftime('%Y-%m-%d %H:%M UTC'),
+             last_seen_in_zone=epoch_2_dt(
+                 track['time'][zoneset][-1]).strftime('%Y-%m-%d %H:%M UTC'),
+             year=epoch_2_dt(track['time'][zoneset][0]).year,
+             month=epoch_2_dt(track['time'][zoneset][0]).month,
+             day=epoch_2_dt(track['time'][zoneset][0]).day))
+
+    # distance travelled
+    dynamic.update(
+        dict(total_distance_meters=np.sum(delta_meters(
+            track, zoneset[[0, -1]])).astype(int),
+             cumulative_distance_meters=np.sum(delta_meters(
+                 track, zoneset)).astype(int)))
+    # shore dist
+    if 'km_from_shore' in track.keys():
+        dynamic.update(
+            dict(
+                min_shore_dist=f"{np.min(track['km_from_shore'][zoneset]):.2f}",
+                avg_shore_dist=
+                f"{np.average(track['km_from_shore'][zoneset]):.2f}"
+                if 'km_from_shore' in track.keys() else None,
+                max_shore_dist=f"{np.max(track['km_from_shore'][zoneset]):.2f}"
+                if 'km_from_shore' in track.keys() else None,
+            ))
+        # elapsed time in distance from shore
+        dynamic.update(
+            dict(
+                minutes_within_10m_5km_shoredist=_time_in_shoredist_rng(
+                    track, zoneset, 0.01, 5),
+                minutes_within_30m_20km_shoredist=_time_in_shoredist_rng(
+                    track, zoneset, 0.03, 20),
+                minutes_within_100m_50km_shoredist=_time_in_shoredist_rng(
+                    track, zoneset, 0.1, 50),
+            ))
+
+    # port dist
+    if 'km_from_port' in track.keys():
+        dynamic.update(
+            dict(
+                min_port_dist=_fstr(np.min(track['km_from_port'][zoneset])),
+                avg_port_dist=_fstr(np.average(track['km_from_port'][zoneset]))
+                if 'km_from_port' in track.keys() else None,
+                max_port_dist=_fstr(np.max(track['km_from_port'][zoneset]))
+                if 'km_from_port' in track.keys() else None,
+            ))
+
+    # depth charts
+    if 'depth_metres' in track.keys():
+        dynamic.update(
+            dict(
+                min_depth=_fstr(np.min(_depth_nonnegative(track, zoneset)))
+                if 'depth_metres' in track.keys() else None,
+                avg_depth=_fstr(np.average(_depth_nonnegative(track, zoneset)))
+                if 'depth_metres' in track.keys() else None,
+                max_depth=_fstr(np.max(_depth_nonnegative(track, zoneset)))
+                if 'depth_metres' in track.keys() else None,
+            ))
+
+    # computed velocity (knots)
+    dynamic.update(
+        dict(
+            velocity_knots_min=f"{np.min(delta_knots(track, zoneset)):.2f}"
+            if len(zoneset) > 1 else 'NULL',
+            velocity_knots_avg=f"{np.average(delta_knots(track, zoneset)):.2f}"
+            if len(zoneset) > 1 else 'NULL',
+            velocity_knots_max=f"{np.max(delta_knots(track, zoneset)):.2f}"
+            if len(zoneset) > 1 else 'NULL',
+        ))
+
+    # elapsed time spent in zones
+    dynamic.update(
+        dict(minutes_spent_in_zone=_fstr(
+            (epoch_2_dt(track['time'][zoneset][-1]) -
+             epoch_2_dt(track['time'][zoneset][0])).total_seconds() /
+            60) if len(zoneset) > 1 else 'NULL', ))
+
+    return dynamic
+
+
+def _serialize_network_edge(tracks, domain, tmp_dir):
+    ''' at each track position where the zone changes, a transit
+        index is recorded, and trajectory statistics are aggregated for this
+        index range using _staticinfo() and _transitinfo()
+
+        results will be serialized as binary files labelled by mmsi into the
+        'tmp_dir' directory, as defined in the config file. see graph() for
+        deserialization and concatenation of results
+
+        args:
+            tracks: dict
+                dictionary of vessel trajectory data, as output by
+                ais.track_gen.TrackGen() or its wrapper functions
+
+        returns: None
+    '''
+    for track in tracks:
+        assert isinstance(track, dict)
+        assert len(track['time']) > 0
+        filepath = os.path.join(tmp_dir, str(track['mmsi']).zfill(9))
+        assert 'in_zone' in track.keys(
+        ), 'need to append zone info from fence_tracks'
+
+        with open(filepath, 'ab') as f:
+            transits = np.where(
+                track['in_zone'][:-1] != track['in_zone'][1:])[0] + 1
+
+            for i in range(len(transits) - 1):
+                rng = np.array(range(transits[i], transits[i + 1] + 1))
+                track_stats = _staticinfo(track, domain)
+                track_stats.update(_transitinfo(track, rng))
+                pickle.dump(track_stats, f)
+
+            i0 = transits[-1] if len(transits) >= 1 else 0
+            rng = np.array(range(i0, len(track['in_zone'])))
+            track_stats = _staticinfo(track, domain)
+            track_stats.update(_transitinfo(track, rng))
+            track_stats['rcv_zone'] = 'NULL'
+            track_stats['transit_nodes'] = track_stats['src_zone']
+            pickle.dump(track_stats, f)
+        yield
+
+
+def _aggregate_output(outputfile, tmp_dir, filters=[lambda row: False]):
+    ''' concatenate serialized output from geofence()
+
+        args:
+            outputfile (string)
+                filepath location to output CSV data
+            tmp_dir (string)
+                files will temporarily be placed here while processing
+            filters (list)
+                list of callback functions. each callable function should
+                accept a dictionary describing a network edge as input. if any
+                return True, the edge will be filtered from the output rows.
+                see _staticinfo() and _transitinfo() for more info on
+                network edge dict keys
+
+                for example, to filter all rows where the max speed exceeds 50
+                knots, and filter non-transiting vessels from zone Z0:
+
+        >>> filters = [
+        ...     lambda r: float(r['velocity_knots_max']) > 50,
+        ...     lambda r: r['src_zone'] == '0' and r['rcv_zone'] == 'NULL'
+        ...     ]
+    '''
+    assert os.path.isdir(
+        os.path.dirname(outputfile)), f'no directory for {outputfile}!'
+
+    picklefiles = [
+        os.path.join(tmp_dir, fname) for fname in sorted(os.listdir(tmp_dir))
+        if '_' not in fname
+    ]
+    assert len(picklefiles) > 0, 'failed to geofence any data...'
+
+    with open(outputfile, 'w') as output:
+        with open(picklefiles[0], 'rb') as f0:
+            getrow = pickle.load(f0)
+            output.write(','.join(map(str, getrow.keys())) + '\n')
+
+        for picklefile in picklefiles:
+            results = []
+            with open(picklefile, 'rb') as f:
+                while True:
+                    try:
+                        getrow = pickle.load(f)
+                    except EOFError:
+                        break
+                    except Exception as e:
+                        raise e
+                    if not reduce(np.logical_or,
+                                  [f(getrow)
+                                   for f in filters]):  # pragma: no cover
+                        results.append(','.join(map(str, getrow.values())))
+
+            if len(results) == 0:
+                warnings.warn(f'no results for {outputfile}')
+            else:
+                output.write('\n'.join(results) + '\n')
+
+            os.remove(picklefile)
+
+
+def graph(
+        qry,
+        *,
+        outputfile,
+        domain,
+        dbconn: ConnectionType,
+        data_dir: str,
+        #dbpath: str = None,
+        trafficDBpath: str or None,  # none if using PostgresDBConn
+        maxdelta: timedelta = timedelta(weeks=1),
+        speed_threshold: float = 50,
+        distance_threshold: float = 200000,
+        interp_delta: float = timedelta(minutes=10),
+        minscore: float = 0,
+        qryfcn=sqlfcn.crawl_dynamic_static,
+        bathy_dir: str = None,
+        shoredist_raster: str = None,
+        portdist_raster: str = None,
+        decimate: float = 0.0001,
+        verbose: bool = False):
+    ''' Compute network graph of vessel movements within domain zones.
+        Zone polygons will be used as network nodes, with graph edges
+        represented by movements between zones.
+
+        args:
+            qry (:py:class:`aisdb.database.dbqry.DBQuery`)
+                database query generator
+            domain (:py:class:`aisdb.gis.Domain`)
+                collection of zones defined as polygons, these will
+                be used as nodes in the network graph
+            dbconn (ConnectionType)
+                Either a :class:`aisdb.database.dbconn.SQLiteDBConn` or
+                :class:`aisdb.database.dbconn.PostgresDBConn` database
+                connection objects
+            data_dir (string)
+                location of raster data
+            trafficDBpath (string)
+                path to marinetraffic database file
+            outpufile (string)
+                filepath for resulting CSV output
+            maxdelta (datetime.timedelta)
+                maximum time between vessel messages before considering
+                it to be part of a new trajectory. See
+                :func:`aisdb.track_gen.split_timedelta` for more info
+            speed_threshold (int, float)
+                maximum speed in knots for encoder segmentation. See
+                :func:`aisdb.denoising_encoder.encode_greatcircledistance` for
+                more info
+            distance_threshold (int, float)
+                maximum distance in meters for encoder segmentation. See
+                :func:`aisdb.denoising_encoder.encode_greatcircledistance` for
+                more info
+            interp_delta (timedelta)
+                track positions will be interpolated to the given sample rate
+            minscore (float)
+                minimum score for segments to be considered sequential. See
+                :func:`aisdb.denoising_encoder.encode_greatcircledistance` for
+                more info
+
+        Network graph activity is computed following these steps:
+
+            - Create database query with
+              :meth:`aisdb.database.dbqry.DBQuery.gen_qry`, and supply
+              resulting generator as rowgen arg. Define a domain
+              (:class:`aisdb.gis.Domain`) in which to compute movements
+            - Vectorize tracks using :py:func:`aisdb.track_gen.TrackGen`
+            - Append vessel metadata to track vessels with
+              :func:`aisdb.webdata.marinetraffic.vessel_info`
+            - Segment track vectors where time between messages exceeds
+              maxdelta using :func:`aisdb.track_gen.split_timedelta`
+            - Segment track vectors as encoded by
+              :py:func:`aisdb.denoising_encoder.encode_greatcircledistance`
+            - Perform geofencing on track segments using
+              :py:func:`aisdb.track_gen.fence_tracks` to determine zone
+              containment
+            - Check where zone boundaries are transited and serialize results
+              to ``outputfile``. Additional metrics per zone activity is also
+              aggregated at this step.
+
+        Example usage:
+
+        >>> import os
+        >>> import shapely
+        >>> from datetime import datetime
+        >>> from aisdb import DBConn, DBQuery, Domain, graph, decode_msgs
+        >>> from aisdb.database.sqlfcn_callbacks import in_bbox_time
+
+        >>> # create example database file
+        >>> dbpath = './example.sqlitedb'
+        >>> filepaths = ['./aisdb/tests/testdata/test_data_20210701.csv',
+        ...              './aisdb/tests/testdata/test_data_20211101.nm4']
+        >>> with DBConn() as dbconn:
+        ...     decode_msgs(filepaths=filepaths, dbconn=dbconn, dbpath=dbpath,
+        ...     source='TESTING')
+
+        Next, configure query area using Domain to compute region boundary
+
+        >>> zones = [{
+        ...     'name': 'Zone1',
+        ...     'geometry': shapely.geometry.Polygon(zip(
+        ...             [-170.24, -170.24, -38.5, -38.5, -170.24],
+        ...             [29.0, 75.2, 75.2, 29.0, 29.0],
+        ...         ))
+        ...     }]
+        >>> domain = Domain(name='new_domain', zones=zones)
+        >>> trafficDBpath = './testdata/marinetraffic_test.db'
+        >>> data_dir = os.environ.get('AISDBDATADIR', '/tmp/ais/')
+
+        Then, query db for points in domain
+
+        >>> with DBConn() as dbconn:
+        ...     qry = DBQuery(
+        ...             dbconn=dbconn,
+        ...             dbpath=dbpath,
+        ...             callback=in_bbox_time,
+        ...             start=datetime(2021, 7, 1),
+        ...             end=datetime(2021, 7, 3),
+        ...             **domain.boundary,
+        ...         )
+        ...     graph(qry,
+        ...           outputfile=os.path.join('testdata', 'test_graph.csv'),
+        ...           dbconn=dbconn,
+        ...           domain=domain,
+        ...           data_dir=data_dir,
+        ...           trafficDBpath=trafficDBpath)
+
+        Afterwards, delete the example database file
+
+        >>> os.remove(dbpath)
+        >>> os.remove(os.path.join('testdata', 'test_graph.csv'))
+
+        process the vessel movement graph edges.
+        caution: this may consume a large amount of memory
+    '''
+    assert not isinstance(qry, types.GeneratorType),\
+            'Got a generator for "qry" arg instead of DBQuery'
+
+    assert isinstance(qry, aisdb.database.dbqry.DBQuery),\
+            f'Not a DBQuery object! Got {qry}'
+
+    if not isinstance(dbconn, (
+            ConnectionType.SQLITE.value,
+            ConnectionType.POSTGRES.value,
+    )):
+        raise ValueError("Invalid dbconn connection type")
+    if isinstance(dbconn, ConnectionType.SQLITE.value):
+        assert trafficDBpath is not None
+        assert isinstance(trafficDBpath, str)
+        vinfoDB = VesselInfo(trafficDBpath).trafficDB
+    else:
+        vinfoDB = dbconn
+
+    rowgen = qry.gen_qry(fcn=qryfcn, verbose=verbose)
+    tracks = TrackGen(rowgen, decimate)
+
+    if portdist_raster is not None:
+        pdist = PortDist(portdist_raster)
+        with pdist:
+            tracks = list(pdist.get_distance(tracks))
+
+    if shoredist_raster is not None:
+        sdist_dir, sdist_name = shoredist_raster.rsplit(os.path.sep, 1)
+        sdist = ShoreDist(sdist_dir, sdist_name)
+        with sdist:
+            tracks = list(sdist.get_distance(tracks))
+
+    if bathy_dir is not None:
+        bathy = Gebco(data_dir=bathy_dir)
+        with bathy:
+            tracks = list(bathy.merge_tracks(tracks))
+
+    # initialize raster data sources
+    if not os.path.isdir('/tmp'):  # pragma: no cover
+        os.mkdir('/tmp')
+    with tempfile.TemporaryDirectory() as tmp_dir:
+        if os.environ.get('DEBUG'):
+            print(f'network graph {tmp_dir = }')
+            print(f'\n{domain.name=} {domain.boundary=}')
+
+        # configure processing pipeline
+        serialize_CSV = partial(_serialize_network_edge,
+                                domain=domain,
+                                tmp_dir=tmp_dir)
+        geofence = partial(fence_tracks, domain=domain)
+        interp = partial(interp_time, step=interp_delta)
+        encode_tracks = partial(encode_greatcircledistance,
+                                distance_threshold=distance_threshold,
+                                minscore=minscore,
+                                speed_threshold=speed_threshold)
+        timesplit = partial(split_timedelta, maxdelta=maxdelta)
+        vinfo = partial(vessel_info, dbconn=vinfoDB)
+
+        # pipeline execution order
+        tracks = vinfo(tracks)
+        tracks = wetted_surface_area(tracks)
+        tracks = timesplit(tracks)
+        tracks = encode_tracks(tracks)
+        tracks = interp(tracks)
+        tracks = geofence(tracks)
+        result = serialize_CSV(tracks)
+
+        for res in result:
+            assert res is None
+
+        if os.listdir(tmp_dir) == []:
+            warnings.warn(f'no data for {outputfile}, skipping...\n')
+        else:
+            _aggregate_output(outputfile=outputfile, tmp_dir=tmp_dir)
```

## aisdb/proc_util.py

 * *Ordering differences only*

```diff
@@ -1,246 +1,246 @@
-import os
-from functools import partial, reduce
-from datetime import datetime, timedelta
-import re
-import csv
-
-import numpy as np
-
-
-def _sanitize(s):
-    # note: the first comma uses ASCII code 44,
-    # second comma uses ASCII decimal 130 !!
-    # not the same char!
-    if s is None:
-        return ''
-    elif s == '-':
-        return ''
-    else:
-        return str(s).replace(',', '').replace(chr(130), '').replace(
-            '#', '').replace('"', '').replace("'", '').replace('\n', '')
-
-
-def _epoch_2_dt(ep_arr, t0=datetime(1970, 1, 1, 0, 0, 0), unit='seconds'):
-    ''' convert epoch minutes to datetime.datetime.
-        redefinition of function in aisdb.gis to avoid circular import
-    '''
-
-    delta = lambda ep, unit: t0 + timedelta(**{unit: ep})
-
-    if isinstance(ep_arr, (list, np.ndarray)):
-        return np.array(list(map(partial(delta, unit=unit), map(int, ep_arr))))
-
-    elif isinstance(ep_arr, (float, int, np.uint32)):
-        return delta(int(ep_arr), unit=unit)
-
-    else:  # pragma: no cover
-        raise ValueError(
-            f'input must be integer or array of integers. got {ep_arr=}{type(ep_arr)}'
-        )
-
-
-def _splits_idx(vector: np.ndarray, d: timedelta) -> np.ndarray:
-    assert isinstance(d, timedelta)
-    vector = np.array(vector, dtype=int)
-    splits = np.nonzero(vector[1:] - vector[:-1] >= d.total_seconds())[0] + 1
-    #else:
-    #    splits = np.nonzero(vector[1:] - vector[:-1] >= d)[0] + 1
-    idx = np.append(np.append([0], splits), [vector.size])
-    return idx
-
-
-def _segment_rng(track, maxdelta, key='time') -> filter:
-    ''' index time segments '''
-    for rng in map(
-            range,
-            _splits_idx(track[key], maxdelta)[:-1],
-            _splits_idx(track[key], maxdelta)[1:],
-    ):
-        yield rng
-
-
-def write_csv_rows(rows,
-                   pathname='/data/smith6/ais/scripts/output.csv',
-                   mode='a'):
-    with open(pathname, mode) as f:
-        f.write('\n'.join(
-            map(
-                lambda r: ','.join(
-                    map(lambda r: r.replace(',', '').replace('#', ''),
-                        map(str.rstrip, map(str, r)))), rows)) + '\n')
-
-
-def _datetime_column(tracks):
-    for track in tracks:
-        assert isinstance(track, dict), f'got {track=}'
-        track['datetime'] = np.array(
-            _epoch_2_dt(track['time'].astype(int)),
-            dtype=object,
-        )
-        track['dynamic'] = track['dynamic'].union(set(['datetime']))
-        yield track
-
-
-_columns_order = [
-    'mmsi', 'imo', 'vessel_name', 'name', 'datetime', 'time', 'lon', 'lat',
-    'cog', 'sog', 'dim_bow', 'dim_stern', 'dim_star', 'dim_port',
-    'coarse_type_txt', 'vesseltype_generic', 'vesseltype_detailed', 'callsign',
-    'flag', 'gross_tonnage', 'summer_dwt', 'length_breadth', 'year_built',
-    'home_port', 'error404'
-]
-
-
-def write_csv(
-    tracks,
-    fpath,
-    skipcols=['label', 'in_zone'],
-):
-    ''' write track vector dictionaries as CSV file
-
-        args:
-            tracks (iter)
-                track generator such as returned by
-                :func:`aisdb.track_gen.TrackGen`
-            fpath (string)
-                output CSV filepath
-            skipcols (list)
-                columns to be omitted from results
-    '''
-    tracks_dt = _datetime_column(tracks)
-    tr1 = next(tracks_dt)
-    colnames = [
-        c for c in _columns_order + list(
-            set(tr1['static'].union(tr1['dynamic'])) -
-            set(_columns_order).union(set(['marinetraffic_info'])))
-        if c in list(tr1['static']) + list(tr1['dynamic'])
-    ]
-    colnames = [col for col in colnames if col not in skipcols]
-
-    if 'marinetraffic_info' in tr1.keys():
-        colnames += tuple(tr1['marinetraffic_info'].keys())
-        colnames.remove('error404')
-        colnames.remove('dim_bow')
-        colnames.remove('dim_stern')
-        colnames.remove('dim_star')
-        colnames.remove('dim_port')
-        if 'coarse_type_txt' in colnames:  # pragma: no cover
-            colnames.remove('coarse_type_txt')
-        if 'vessel_name' in colnames:  # pragma: no cover
-            colnames.remove('vessel_name')
-        colnames = list(dict.fromkeys(colnames))
-
-    decimals = {
-        'lon': 5,
-        'lat': 5,
-        'depth_metres': 2,
-        'distance_metres': 2,
-        'submerged_hull_m^2': 0,
-    }
-
-    def _append(track, writer, colnames=colnames, decimals=decimals):
-        if 'marinetraffic_info' in track.keys():
-            for key, val in dict(track['marinetraffic_info']).items():
-                if key in ('error404', 'mmsi', 'imo'):
-                    continue
-                track[key] = val
-            del track['marinetraffic_info']
-
-        for i in range(0, track['time'].size):
-            row = [(track[c][i] if c in track['dynamic'] else
-                    (_sanitize(track[c]) if track[c] != 0 else ''))
-                   for c in colnames]
-            for ci, r in zip(range(len(colnames)), row):
-                if colnames[ci] in decimals.keys() and r != '':
-                    row[ci] = f'{float(r):.{decimals[colnames[ci]]}f}'
-
-            writer.writerow(row)
-
-    with open(fpath, 'w', newline='') as f:
-        f.write(','.join(colnames) + '\n')
-        writer = csv.writer(f,
-                            delimiter=',',
-                            quotechar="'",
-                            quoting=csv.QUOTE_NONE,
-                            dialect='unix')
-        _append(tr1, writer, colnames, decimals)
-        for track in tracks_dt:
-            _append(track, writer, colnames, decimals)
-
-    return
-
-
-def glob_files(dirpath, ext='.txt', keyorder=lambda key: key):
-    ''' walk a directory to glob txt files. can be used with ZoneGeomFromTxt()
-
-        zones_dir: string
-            directory to walk
-        keyorder:
-            anonymous function for custom sort ordering
-
-        example keyorder:
-
-        .. code-block::
-
-            # numeric sort on zone names with strsplit on 'Z' char
-            keyorder=lambda key: int(key.rsplit(os.path.sep, 1)[1].split('.')[0].split('Z')[1])
-
-        returns:
-            .txt shapefile paths
-
-    '''
-    paths = list(os.walk(dirpath))
-
-    extfiles = [[
-        p[0],
-        sorted([f for f in p[2] if f[-len(ext):] == ext], key=keyorder)
-    ] for p in paths if len(p[2]) > 0]
-
-    extpaths = reduce(np.append, [
-        list(map(os.path.join, (path[0] for p in path[1]), path[1]))
-        for path in extfiles
-    ], np.array([], dtype=object))
-
-    return sorted(extpaths, key=keyorder)
-
-
-def getfiledate(filename):
-    ''' attempt to parse the first valid epoch timestamp from .nm4 data file.
-        timestamp will be returned as :class:`datetime.date` if successful,
-        otherwise will return False if no date could be found
-
-        args:
-            filename (string)
-                raw AIS data file in .nm4 format
-    '''
-    filesize = os.path.getsize(filename)
-    if filesize == 0:  # pragma: no cover
-        return False
-    with open(filename, 'r') as f:
-        if 'csv' in filename:
-            reader = csv.reader(f)
-            head = next(reader)
-            row1 = next(reader)
-            rowdict = {a: b for a, b in zip(head, row1)}
-            fdate = datetime.strptime(rowdict['Time'], '%Y%m%d_%H%M%S').date()
-            return fdate
-        else:
-            line = f.readline()
-            head = line.rsplit('\\', 1)[0]
-            n = 0
-            while 'c:' not in head:  # pragma: no cover
-                n += 1
-                line = f.readline()
-                head = line.rsplit('\\', 1)[0]
-                #if n > 10000:
-                #    print(f'bad! {filename}')
-                #    return False
-                assert n <= 10000
-            split0 = re.split('c:', head)[1]
-            try:
-                epoch = int(re.split('[^0-9]', split0)[0])
-            except ValueError:  # pragma: no cover
-                return False
-            except Exception as err:  # pragma: no cover
-                raise err
-        fdate = datetime.fromtimestamp(epoch).date()
-        return fdate
+import os
+from functools import partial, reduce
+from datetime import datetime, timedelta
+import re
+import csv
+
+import numpy as np
+
+
+def _sanitize(s):
+    # note: the first comma uses ASCII code 44,
+    # second comma uses ASCII decimal 130 !!
+    # not the same char!
+    if s is None:
+        return ''
+    elif s == '-':
+        return ''
+    else:
+        return str(s).replace(',', '').replace(chr(130), '').replace(
+            '#', '').replace('"', '').replace("'", '').replace('\n', '')
+
+
+def _epoch_2_dt(ep_arr, t0=datetime(1970, 1, 1, 0, 0, 0), unit='seconds'):
+    ''' convert epoch minutes to datetime.datetime.
+        redefinition of function in aisdb.gis to avoid circular import
+    '''
+
+    delta = lambda ep, unit: t0 + timedelta(**{unit: ep})
+
+    if isinstance(ep_arr, (list, np.ndarray)):
+        return np.array(list(map(partial(delta, unit=unit), map(int, ep_arr))))
+
+    elif isinstance(ep_arr, (float, int, np.uint32)):
+        return delta(int(ep_arr), unit=unit)
+
+    else:  # pragma: no cover
+        raise ValueError(
+            f'input must be integer or array of integers. got {ep_arr=}{type(ep_arr)}'
+        )
+
+
+def _splits_idx(vector: np.ndarray, d: timedelta) -> np.ndarray:
+    assert isinstance(d, timedelta)
+    vector = np.array(vector, dtype=int)
+    splits = np.nonzero(vector[1:] - vector[:-1] >= d.total_seconds())[0] + 1
+    #else:
+    #    splits = np.nonzero(vector[1:] - vector[:-1] >= d)[0] + 1
+    idx = np.append(np.append([0], splits), [vector.size])
+    return idx
+
+
+def _segment_rng(track, maxdelta, key='time') -> filter:
+    ''' index time segments '''
+    for rng in map(
+            range,
+            _splits_idx(track[key], maxdelta)[:-1],
+            _splits_idx(track[key], maxdelta)[1:],
+    ):
+        yield rng
+
+
+def write_csv_rows(rows,
+                   pathname='/data/smith6/ais/scripts/output.csv',
+                   mode='a'):
+    with open(pathname, mode) as f:
+        f.write('\n'.join(
+            map(
+                lambda r: ','.join(
+                    map(lambda r: r.replace(',', '').replace('#', ''),
+                        map(str.rstrip, map(str, r)))), rows)) + '\n')
+
+
+def _datetime_column(tracks):
+    for track in tracks:
+        assert isinstance(track, dict), f'got {track=}'
+        track['datetime'] = np.array(
+            _epoch_2_dt(track['time'].astype(int)),
+            dtype=object,
+        )
+        track['dynamic'] = track['dynamic'].union(set(['datetime']))
+        yield track
+
+
+_columns_order = [
+    'mmsi', 'imo', 'vessel_name', 'name', 'datetime', 'time', 'lon', 'lat',
+    'cog', 'sog', 'dim_bow', 'dim_stern', 'dim_star', 'dim_port',
+    'coarse_type_txt', 'vesseltype_generic', 'vesseltype_detailed', 'callsign',
+    'flag', 'gross_tonnage', 'summer_dwt', 'length_breadth', 'year_built',
+    'home_port', 'error404'
+]
+
+
+def write_csv(
+    tracks,
+    fpath,
+    skipcols=['label', 'in_zone'],
+):
+    ''' write track vector dictionaries as CSV file
+
+        args:
+            tracks (iter)
+                track generator such as returned by
+                :func:`aisdb.track_gen.TrackGen`
+            fpath (string)
+                output CSV filepath
+            skipcols (list)
+                columns to be omitted from results
+    '''
+    tracks_dt = _datetime_column(tracks)
+    tr1 = next(tracks_dt)
+    colnames = [
+        c for c in _columns_order + list(
+            set(tr1['static'].union(tr1['dynamic'])) -
+            set(_columns_order).union(set(['marinetraffic_info'])))
+        if c in list(tr1['static']) + list(tr1['dynamic'])
+    ]
+    colnames = [col for col in colnames if col not in skipcols]
+
+    if 'marinetraffic_info' in tr1.keys():
+        colnames += tuple(tr1['marinetraffic_info'].keys())
+        colnames.remove('error404')
+        colnames.remove('dim_bow')
+        colnames.remove('dim_stern')
+        colnames.remove('dim_star')
+        colnames.remove('dim_port')
+        if 'coarse_type_txt' in colnames:  # pragma: no cover
+            colnames.remove('coarse_type_txt')
+        if 'vessel_name' in colnames:  # pragma: no cover
+            colnames.remove('vessel_name')
+        colnames = list(dict.fromkeys(colnames))
+
+    decimals = {
+        'lon': 5,
+        'lat': 5,
+        'depth_metres': 2,
+        'distance_metres': 2,
+        'submerged_hull_m^2': 0,
+    }
+
+    def _append(track, writer, colnames=colnames, decimals=decimals):
+        if 'marinetraffic_info' in track.keys():
+            for key, val in dict(track['marinetraffic_info']).items():
+                if key in ('error404', 'mmsi', 'imo'):
+                    continue
+                track[key] = val
+            del track['marinetraffic_info']
+
+        for i in range(0, track['time'].size):
+            row = [(track[c][i] if c in track['dynamic'] else
+                    (_sanitize(track[c]) if track[c] != 0 else ''))
+                   for c in colnames]
+            for ci, r in zip(range(len(colnames)), row):
+                if colnames[ci] in decimals.keys() and r != '':
+                    row[ci] = f'{float(r):.{decimals[colnames[ci]]}f}'
+
+            writer.writerow(row)
+
+    with open(fpath, 'w', newline='') as f:
+        f.write(','.join(colnames) + '\n')
+        writer = csv.writer(f,
+                            delimiter=',',
+                            quotechar="'",
+                            quoting=csv.QUOTE_NONE,
+                            dialect='unix')
+        _append(tr1, writer, colnames, decimals)
+        for track in tracks_dt:
+            _append(track, writer, colnames, decimals)
+
+    return
+
+
+def glob_files(dirpath, ext='.txt', keyorder=lambda key: key):
+    ''' walk a directory to glob txt files. can be used with ZoneGeomFromTxt()
+
+        zones_dir: string
+            directory to walk
+        keyorder:
+            anonymous function for custom sort ordering
+
+        example keyorder:
+
+        .. code-block::
+
+            # numeric sort on zone names with strsplit on 'Z' char
+            keyorder=lambda key: int(key.rsplit(os.path.sep, 1)[1].split('.')[0].split('Z')[1])
+
+        returns:
+            .txt shapefile paths
+
+    '''
+    paths = list(os.walk(dirpath))
+
+    extfiles = [[
+        p[0],
+        sorted([f for f in p[2] if f[-len(ext):] == ext], key=keyorder)
+    ] for p in paths if len(p[2]) > 0]
+
+    extpaths = reduce(np.append, [
+        list(map(os.path.join, (path[0] for p in path[1]), path[1]))
+        for path in extfiles
+    ], np.array([], dtype=object))
+
+    return sorted(extpaths, key=keyorder)
+
+
+def getfiledate(filename):
+    ''' attempt to parse the first valid epoch timestamp from .nm4 data file.
+        timestamp will be returned as :class:`datetime.date` if successful,
+        otherwise will return False if no date could be found
+
+        args:
+            filename (string)
+                raw AIS data file in .nm4 format
+    '''
+    filesize = os.path.getsize(filename)
+    if filesize == 0:  # pragma: no cover
+        return False
+    with open(filename, 'r') as f:
+        if 'csv' in filename:
+            reader = csv.reader(f)
+            head = next(reader)
+            row1 = next(reader)
+            rowdict = {a: b for a, b in zip(head, row1)}
+            fdate = datetime.strptime(rowdict['Time'], '%Y%m%d_%H%M%S').date()
+            return fdate
+        else:
+            line = f.readline()
+            head = line.rsplit('\\', 1)[0]
+            n = 0
+            while 'c:' not in head:  # pragma: no cover
+                n += 1
+                line = f.readline()
+                head = line.rsplit('\\', 1)[0]
+                #if n > 10000:
+                #    print(f'bad! {filename}')
+                #    return False
+                assert n <= 10000
+            split0 = re.split('c:', head)[1]
+            try:
+                epoch = int(re.split('[^0-9]', split0)[0])
+            except ValueError:  # pragma: no cover
+                return False
+            except Exception as err:  # pragma: no cover
+                raise err
+        fdate = datetime.fromtimestamp(epoch).date()
+        return fdate
```

## aisdb/receiver.py

```diff
@@ -1,56 +1,56 @@
-import os
-from aisdb.aisdb import receiver as _receiver
-
-
-def start_receiver(sqlite_dbpath=os.path.abspath("./ais_rx.db"),
-                   postgres_connection_string=None,
-                   connect_addr="aisdb.meridian.cs.dal.ca:9920",
-                   tcp_listen_addr=None,
-                   udp_listen_addr="[::0]:9921",
-                   multicast_addr=None,
-                   multicast_rebroadcast=None,
-                   tcp_output_addr=None,
-                   udp_output_addr=None,
-                   stdout=False):
-    '''
-        Receive raw AIS data from an upstream UDP data source, parse the data into
-        JSON format, and create a websocket listener to send parsed results downstream.
-        If dbpath is given, parsed data will be stored in an SQLite database.
-
-
-        args:
-            sqlite_dbpath (Option<str>)
-                If given, raw messages will be parsed and stored in an SQLite database at this location
-            postgres_connection_string (Option<String>)
-                Postgres database connection string
-            connect_addr (Option<str>)
-                Optionally forward upstream TCP/TLS host to udp_listen_addr
-            tcp_listen_addr (str)
-                if not None, a thread will be spawned to forward TCP connections to
-                incoming UDP port ``udp_listen_addr``
-            udp_listen_addr (str)
-                UDP port to listen for incoming AIS data streams e.g. "0.0.0.0:9921" or "[::]:9921"
-            multicast_addr (str)
-                Raw UDP messages will be parsed and then routed to TCP socket listeners via this channel.
-            multicast_rebroadcast (Option<str>)
-                Optionally pass a UDP rebroadcast address where raw data will be filtered
-                and rebroadcasted to this channel for e.g. forwarding to downstream
-                networks
-            tcp_output_addr (str)
-                TCP port to listen for websocket clients to send parsed data in JSON format
-            stdout (bool)
-                If True, raw input will be copied to stdout
-    '''
-
-    _receiver(sqlite_dbpath,
-              postgres_connection_string,
-              connect_addr,
-              tcp_listen_addr,
-              udp_listen_addr,
-              multicast_addr,
-              multicast_rebroadcast,
-              tcp_output_addr,
-              udp_output_addr,
-              dynamic_msg_bufsize=128,
-              static_msg_bufsize=64,
-              tee=stdout)
+import os
+from aisdb.aisdb import receiver as _receiver
+
+
+def start_receiver(sqlite_dbpath=os.path.abspath("./ais_rx.db"),
+                   postgres_connection_string=None,
+                   connect_addr="aisdb.meridian.cs.dal.ca:9920",
+                   tcp_listen_addr=None,
+                   udp_listen_addr=None,
+                   multicast_addr=None,
+                   multicast_rebroadcast=None,
+                   tcp_output_addr=None,
+                   udp_output_addr=None,
+                   stdout=False):
+    '''
+        Receive raw AIS data from an upstream UDP data source, parse the data into
+        JSON format, and create a websocket listener to send parsed results downstream.
+        If dbpath is given, parsed data will be stored in an SQLite database.
+
+
+        args:
+            sqlite_dbpath (Option<str>)
+                If given, raw messages will be parsed and stored in an SQLite database at this location
+            postgres_connection_string (Option<String>)
+                Postgres database connection string
+            connect_addr (Option<str>)
+                Optionally forward upstream TCP/TLS host to udp_listen_addr
+            tcp_listen_addr (str)
+                if not None, a thread will be spawned to forward TCP connections to
+                incoming UDP port ``udp_listen_addr``
+            udp_listen_addr (str)
+                UDP port to listen for incoming AIS data streams e.g. "0.0.0.0:9921" or "[::]:9921"
+            multicast_addr (str)
+                Raw UDP messages will be parsed and then routed to TCP socket listeners via this channel.
+            multicast_rebroadcast (Option<str>)
+                Optionally pass a UDP rebroadcast address where raw data will be filtered
+                and rebroadcasted to this channel for e.g. forwarding to downstream
+                networks
+            tcp_output_addr (str)
+                TCP port to listen for websocket clients to send parsed data in JSON format
+            stdout (bool)
+                If True, raw input will be copied to stdout
+    '''
+
+    _receiver(sqlite_dbpath,
+              postgres_connection_string,
+              connect_addr,
+              tcp_listen_addr,
+              udp_listen_addr,
+              multicast_addr,
+              multicast_rebroadcast,
+              tcp_output_addr,
+              udp_output_addr,
+              dynamic_msg_bufsize=128,
+              static_msg_bufsize=64,
+              tee=stdout)
```

## aisdb/tests/create_testing_data.py

 * *Ordering differences only*

```diff
@@ -1,90 +1,90 @@
-import os
-
-import numpy as np
-from shapely.geometry import Polygon
-
-from aisdb.gis import Domain
-from aisdb.database.create_tables import (
-    sqlite_createtable_dynamicreport,
-    sqlite_createtable_staticreport,
-)
-from aisdb import decode_msgs, DBConn, aggregate_static_msgs
-
-
-def sample_dynamictable_insertdata(*, dbconn, dbpath):
-    #db = DBConn()
-    assert isinstance(dbconn, DBConn)
-    sqlite_createtable_staticreport(dbconn, month="200001", dbpath=dbpath)
-    sqlite_createtable_dynamicreport(dbconn, month="200001", dbpath=dbpath)
-    dbconn.execute(
-        'INSERT OR IGNORE INTO ais_200001_dynamic (mmsi, time, longitude, latitude, cog, sog) VALUES (000000001, 946702800, -60.994833, 47.434647238127695, -1, -1)'
-    )
-    dbconn.execute(
-        'INSERT OR IGNORE INTO ais_200001_dynamic (mmsi, time, longitude, latitude, cog, sog) VALUES (000000001, 946702820, -60.994833, 47.434647238127695, -1, -1)'
-    )
-    dbconn.execute(
-        'INSERT OR IGNORE INTO ais_200001_dynamic (mmsi, time, longitude, latitude, cog, sog) VALUES (000000001, 946702840, -60.994833, 47.434647238127695, -1, -1)'
-    )
-    dbconn.commit()
-
-
-def sample_random_polygon(xscale=50, yscale=50):
-    vertices = 5
-
-    x, y = [0, 0, 0], [0, 0, 0]
-    while not Polygon(zip(x, y)).is_valid:
-        x = np.random.random(vertices) * xscale
-        x += np.random.randint(360 - xscale)
-        x -= 180
-        y = np.random.random(vertices) * yscale
-        y += np.random.randint(180 - yscale)
-        y -= 90
-        assert min(x) >= -180, min(x)
-        assert max(x) <= 180, max(x)
-        assert min(y) >= -90, min(y)
-        assert max(y) <= 90, max(y)
-
-    return x, y
-
-
-def sample_gulfstlawrence_bbox():
-    gulfstlawrence_bbox_xy = np.array([
-        (-71.64440346704974, 43.18445256159233),
-        (-71.2966623933639, 52.344721551389526),
-        (-51.2146153880073, 51.68484191466307),
-        (-50.345262703792734, 42.95158299927571),
-        (-71.64440346704974, 43.18445256159233),
-    ])
-    return gulfstlawrence_bbox_xy.T
-
-
-def random_polygons_domain(count=10):
-    return Domain('testdomain',
-                  [{
-                      'name': f'random_{i:03}',
-                      'geometry': Polygon(zip(*sample_random_polygon()))
-                  } for i in range(count)])
-
-
-def sample_database_file(dbpath):
-    ''' test data for date 2021-11-01 '''
-    assert os.path.isdir(os.path.join(os.path.dirname(__file__), 'testdata'))
-    datapath_csv = os.path.join(os.path.dirname(__file__), 'testdata',
-                                'test_data_20210701.csv')
-    # no static data in nm4
-    datapath_nm4 = os.path.join(os.path.dirname(__file__), 'testdata',
-                                'test_data_20211101.nm4')
-    months = ["202107", "202111"]
-    with DBConn() as dbconn:
-        dbconn._attach(dbpath)
-        decode_msgs(
-            dbconn=dbconn,
-            filepaths=[datapath_csv, datapath_nm4],
-            dbpath=dbpath,
-            source='TESTING',
-            vacuum=False,
-            skip_checksum=True,
-        )
-        aggregate_static_msgs(dbconn, months[:1])
-        dbconn.commit()
-    return months
+import os
+
+import numpy as np
+from shapely.geometry import Polygon
+
+from aisdb.gis import Domain
+from aisdb.database.create_tables import (
+    sqlite_createtable_dynamicreport,
+    sqlite_createtable_staticreport,
+)
+from aisdb import decode_msgs, DBConn, aggregate_static_msgs
+
+
+def sample_dynamictable_insertdata(*, dbconn, dbpath):
+    #db = DBConn()
+    assert isinstance(dbconn, DBConn)
+    sqlite_createtable_staticreport(dbconn, month="200001", dbpath=dbpath)
+    sqlite_createtable_dynamicreport(dbconn, month="200001", dbpath=dbpath)
+    dbconn.execute(
+        'INSERT OR IGNORE INTO ais_200001_dynamic (mmsi, time, longitude, latitude, cog, sog) VALUES (000000001, 946702800, -60.994833, 47.434647238127695, -1, -1)'
+    )
+    dbconn.execute(
+        'INSERT OR IGNORE INTO ais_200001_dynamic (mmsi, time, longitude, latitude, cog, sog) VALUES (000000001, 946702820, -60.994833, 47.434647238127695, -1, -1)'
+    )
+    dbconn.execute(
+        'INSERT OR IGNORE INTO ais_200001_dynamic (mmsi, time, longitude, latitude, cog, sog) VALUES (000000001, 946702840, -60.994833, 47.434647238127695, -1, -1)'
+    )
+    dbconn.commit()
+
+
+def sample_random_polygon(xscale=50, yscale=50):
+    vertices = 5
+
+    x, y = [0, 0, 0], [0, 0, 0]
+    while not Polygon(zip(x, y)).is_valid:
+        x = np.random.random(vertices) * xscale
+        x += np.random.randint(360 - xscale)
+        x -= 180
+        y = np.random.random(vertices) * yscale
+        y += np.random.randint(180 - yscale)
+        y -= 90
+        assert min(x) >= -180, min(x)
+        assert max(x) <= 180, max(x)
+        assert min(y) >= -90, min(y)
+        assert max(y) <= 90, max(y)
+
+    return x, y
+
+
+def sample_gulfstlawrence_bbox():
+    gulfstlawrence_bbox_xy = np.array([
+        (-71.64440346704974, 43.18445256159233),
+        (-71.2966623933639, 52.344721551389526),
+        (-51.2146153880073, 51.68484191466307),
+        (-50.345262703792734, 42.95158299927571),
+        (-71.64440346704974, 43.18445256159233),
+    ])
+    return gulfstlawrence_bbox_xy.T
+
+
+def random_polygons_domain(count=10):
+    return Domain('testdomain',
+                  [{
+                      'name': f'random_{i:03}',
+                      'geometry': Polygon(zip(*sample_random_polygon()))
+                  } for i in range(count)])
+
+
+def sample_database_file(dbpath):
+    ''' test data for date 2021-11-01 '''
+    assert os.path.isdir(os.path.join(os.path.dirname(__file__), 'testdata'))
+    datapath_csv = os.path.join(os.path.dirname(__file__), 'testdata',
+                                'test_data_20210701.csv')
+    # no static data in nm4
+    datapath_nm4 = os.path.join(os.path.dirname(__file__), 'testdata',
+                                'test_data_20211101.nm4')
+    months = ["202107", "202111"]
+    with DBConn() as dbconn:
+        dbconn._attach(dbpath)
+        decode_msgs(
+            dbconn=dbconn,
+            filepaths=[datapath_csv, datapath_nm4],
+            dbpath=dbpath,
+            source='TESTING',
+            vacuum=False,
+            skip_checksum=True,
+        )
+        aggregate_static_msgs(dbconn, months[:1])
+        dbconn.commit()
+    return months
```

## aisdb/tests/test_00_decode.py

 * *Ordering differences only*

```diff
@@ -1,34 +1,34 @@
-import os
-from datetime import datetime
-
-from aisdb.database.dbconn import DBConn
-from aisdb.database.decoder import decode_msgs
-
-
-def test_decode_1day(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_decode_1day.db')
-    testingdata_nm4 = os.path.join(os.path.dirname(__file__), 'testdata',
-                                   'test_data_20211101.nm4')
-    testingdata_csv = os.path.join(os.path.dirname(__file__), 'testdata',
-                                   'test_data_20210701.csv')
-    testingdata_gz = os.path.join(os.path.dirname(__file__), 'testdata',
-                                  'test_data_20211101.nm4.gz')
-    testingdata_zip = os.path.join(os.path.dirname(__file__), 'testdata',
-                                   'test_data_20211101.nm4.zip')
-    with DBConn() as dbconn:
-        filepaths = [
-            testingdata_nm4, testingdata_csv, testingdata_gz, testingdata_zip
-        ]
-        dt = datetime.now()
-        decode_msgs(filepaths=filepaths,
-                    dbconn=dbconn,
-                    dbpath=dbpath,
-                    source='TESTING',
-                    vacuum=True)
-        decode_msgs(filepaths=filepaths,
-                    dbconn=dbconn,
-                    dbpath=dbpath,
-                    source='TESTING',
-                    vacuum=dbpath + '.vacuum')
-        delta = datetime.now() - dt
-        print(f'total parse and insert time: {delta.total_seconds():.2f}s')
+import os
+from datetime import datetime
+
+from aisdb.database.dbconn import DBConn
+from aisdb.database.decoder import decode_msgs
+
+
+def test_decode_1day(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_decode_1day.db')
+    testingdata_nm4 = os.path.join(os.path.dirname(__file__), 'testdata',
+                                   'test_data_20211101.nm4')
+    testingdata_csv = os.path.join(os.path.dirname(__file__), 'testdata',
+                                   'test_data_20210701.csv')
+    testingdata_gz = os.path.join(os.path.dirname(__file__), 'testdata',
+                                  'test_data_20211101.nm4.gz')
+    testingdata_zip = os.path.join(os.path.dirname(__file__), 'testdata',
+                                   'test_data_20211101.nm4.zip')
+    with DBConn() as dbconn:
+        filepaths = [
+            testingdata_nm4, testingdata_csv, testingdata_gz, testingdata_zip
+        ]
+        dt = datetime.now()
+        decode_msgs(filepaths=filepaths,
+                    dbconn=dbconn,
+                    dbpath=dbpath,
+                    source='TESTING',
+                    vacuum=True)
+        decode_msgs(filepaths=filepaths,
+                    dbconn=dbconn,
+                    dbpath=dbpath,
+                    source='TESTING',
+                    vacuum=dbpath + '.vacuum')
+        delta = datetime.now() - dt
+        print(f'total parse and insert time: {delta.total_seconds():.2f}s')
```

## aisdb/tests/test_01_createtables.py

 * *Ordering differences only*

```diff
@@ -1,78 +1,78 @@
-import os
-import warnings
-import sqlite3
-
-from aisdb.database.dbconn import DBConn
-from aisdb.database.decoder import decode_msgs
-from aisdb.database.create_tables import (
-    aggregate_static_msgs,
-    sqlite_createtable_dynamicreport,
-    sqlite_createtable_staticreport,
-)
-
-
-def test_create_static_table(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_create_static_table.db')
-    with DBConn() as dbconn:
-        sqlite_createtable_staticreport(dbconn, month="202009", dbpath=dbpath)
-
-
-def test_create_dynamic_table(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_create_dynamic_table.db')
-    with DBConn() as dbconn:
-        sqlite_createtable_dynamicreport(dbconn, month="202009", dbpath=dbpath)
-
-
-def test_create_static_aggregate_table(tmpdir):
-    warnings.filterwarnings('error')
-    dbpath = os.path.join(tmpdir, 'test_create_static_aggregate_table.db')
-    testingdata_csv = os.path.join(os.path.dirname(__file__), 'testdata',
-                                   'test_data_20210701.csv')
-    with DBConn() as dbconn:
-        decode_msgs([testingdata_csv],
-                    dbconn=dbconn,
-                    dbpath=dbpath,
-                    source='TESTING')
-        aggregate_static_msgs(dbconn, ["202107"])
-
-
-def test_create_from_CSV(tmpdir):
-    testingdata_csv = os.path.join(os.path.dirname(__file__), 'testdata',
-                                   'test_data_20210701.csv')
-    dbpath = os.path.join(tmpdir, 'test_create_from_CSV.db')
-    with DBConn() as dbconn:
-        decode_msgs(
-            dbconn=dbconn,
-            filepaths=[testingdata_csv],
-            dbpath=dbpath,
-            source='TESTING',
-            vacuum=False,
-        )
-
-        # new tables will be created by the decode_msgs function
-        # sqlite_createtable_dynamicreport(dbconn, month="202107", dbpath=dbpath)
-        # aggregate_static_msgs(dbconn, ["202107"])
-
-        # executes SQL statement: ATTACH database AS dbname
-        dbconn._attach(dbpath)
-
-        curr = dbconn.cursor()
-        curr.execute(
-            # need to specify datbabase name in SQL statement
-            "SELECT name FROM test_create_from_CSV.sqlite_schema "
-            "WHERE type='table' ORDER BY name;")
-        rows = curr.fetchall()
-        temp = [row['name'] for row in rows]
-        print(temp)
-        assert len(temp) == 3
-
-    # alternatively, open a new connection to the database:
-    new_dbconn = sqlite3.Connection(dbpath)
-    new_dbconn.row_factory = sqlite3.Row
-    new_cursor = new_dbconn.cursor()
-    new_cursor.execute("SELECT name FROM sqlite_schema "
-                       "WHERE type='table' ORDER BY name;")
-    rows = new_cursor.fetchall()
-    temp = [row['name'] for row in rows]
-    print(temp)
-    assert len(temp) == 3
+import os
+import warnings
+import sqlite3
+
+from aisdb.database.dbconn import DBConn
+from aisdb.database.decoder import decode_msgs
+from aisdb.database.create_tables import (
+    aggregate_static_msgs,
+    sqlite_createtable_dynamicreport,
+    sqlite_createtable_staticreport,
+)
+
+
+def test_create_static_table(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_create_static_table.db')
+    with DBConn() as dbconn:
+        sqlite_createtable_staticreport(dbconn, month="202009", dbpath=dbpath)
+
+
+def test_create_dynamic_table(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_create_dynamic_table.db')
+    with DBConn() as dbconn:
+        sqlite_createtable_dynamicreport(dbconn, month="202009", dbpath=dbpath)
+
+
+def test_create_static_aggregate_table(tmpdir):
+    warnings.filterwarnings('error')
+    dbpath = os.path.join(tmpdir, 'test_create_static_aggregate_table.db')
+    testingdata_csv = os.path.join(os.path.dirname(__file__), 'testdata',
+                                   'test_data_20210701.csv')
+    with DBConn() as dbconn:
+        decode_msgs([testingdata_csv],
+                    dbconn=dbconn,
+                    dbpath=dbpath,
+                    source='TESTING')
+        aggregate_static_msgs(dbconn, ["202107"])
+
+
+def test_create_from_CSV(tmpdir):
+    testingdata_csv = os.path.join(os.path.dirname(__file__), 'testdata',
+                                   'test_data_20210701.csv')
+    dbpath = os.path.join(tmpdir, 'test_create_from_CSV.db')
+    with DBConn() as dbconn:
+        decode_msgs(
+            dbconn=dbconn,
+            filepaths=[testingdata_csv],
+            dbpath=dbpath,
+            source='TESTING',
+            vacuum=False,
+        )
+
+        # new tables will be created by the decode_msgs function
+        # sqlite_createtable_dynamicreport(dbconn, month="202107", dbpath=dbpath)
+        # aggregate_static_msgs(dbconn, ["202107"])
+
+        # executes SQL statement: ATTACH database AS dbname
+        dbconn._attach(dbpath)
+
+        curr = dbconn.cursor()
+        curr.execute(
+            # need to specify datbabase name in SQL statement
+            "SELECT name FROM test_create_from_CSV.sqlite_schema "
+            "WHERE type='table' ORDER BY name;")
+        rows = curr.fetchall()
+        temp = [row['name'] for row in rows]
+        print(temp)
+        assert len(temp) == 3
+
+    # alternatively, open a new connection to the database:
+    new_dbconn = sqlite3.Connection(dbpath)
+    new_dbconn.row_factory = sqlite3.Row
+    new_cursor = new_dbconn.cursor()
+    new_cursor.execute("SELECT name FROM sqlite_schema "
+                       "WHERE type='table' ORDER BY name;")
+    rows = new_cursor.fetchall()
+    temp = [row['name'] for row in rows]
+    print(temp)
+    assert len(temp) == 3
```

## aisdb/tests/test_02_dbqry.py

 * *Ordering differences only*

```diff
@@ -1,79 +1,79 @@
-import os
-import warnings
-from datetime import datetime, timedelta
-
-from shapely.geometry import Polygon
-
-from aisdb import DBConn, DBQuery, sqlfcn_callbacks, Domain, sqlfcn
-
-from aisdb.database.create_tables import sqlite_createtable_dynamicreport
-from aisdb.tests.create_testing_data import (
-    sample_database_file,
-    sample_gulfstlawrence_bbox,
-)
-
-
-def test_query_emptytable(tmpdir):
-    warnings.filterwarnings('error')
-    dbpath = os.path.join(tmpdir, 'test_query_emptytable.db')
-    with DBConn() as dbconn:
-        q = DBQuery(
-            dbconn=dbconn,
-            dbpath=dbpath,
-            start=datetime(2021, 1, 1),
-            end=datetime(2021, 1, 7),
-            callback=sqlfcn_callbacks.in_timerange_validmmsi,
-        )
-        sqlite_createtable_dynamicreport(dbconn, month='202101', dbpath=dbpath)
-        rows = q.gen_qry(reaggregate_static=True)
-        assert list(rows) == []
-
-
-def test_prepare_qry_domain(tmpdir):
-
-    testdbpath = os.path.join(tmpdir, 'test_prepare_qry_domain.db')
-    months = sample_database_file(testdbpath)
-    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
-    end = start + timedelta(weeks=4)
-    z1 = Polygon(zip(*sample_gulfstlawrence_bbox()))
-    domain = Domain('gulf domain', zones=[{'name': 'z1', 'geometry': z1}])
-    with DBConn() as aisdatabase:
-        rowgen = DBQuery(
-            dbconn=aisdatabase,
-            dbpath=testdbpath,
-            start=start,
-            end=end,
-            **domain.boundary,
-            callback=sqlfcn_callbacks.in_timerange,
-        ).gen_qry(reaggregate_static=True)
-        next(rowgen)
-
-
-def test_sql_query_strings(tmpdir):
-    testdbpath = os.path.join(tmpdir, 'test_sql_query_strings.db')
-    months = sample_database_file(testdbpath)
-    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
-    end = start + timedelta(weeks=4)
-    z1 = Polygon(zip(*sample_gulfstlawrence_bbox()))
-    domain = Domain('gulf domain', zones=[{'name': 'z1', 'geometry': z1}])
-    with DBConn() as aisdatabase:
-        for callback in [
-                sqlfcn_callbacks.in_bbox,
-                sqlfcn_callbacks.in_bbox_time,
-                sqlfcn_callbacks.in_bbox_time_validmmsi,
-                sqlfcn_callbacks.in_time_bbox_inmmsi,
-                sqlfcn_callbacks.in_timerange,
-                sqlfcn_callbacks.in_timerange_hasmmsi,
-                sqlfcn_callbacks.in_timerange_validmmsi,
-        ]:
-            rowgen = DBQuery(
-                dbconn=aisdatabase,
-                dbpath=testdbpath,
-                start=start,
-                end=end,
-                **domain.boundary,
-                callback=callback,
-                mmsi=316000000,
-                mmsis=[316000000, 316000001],
-            ).gen_qry(fcn=sqlfcn.crawl_dynamic_static)
-            next(rowgen)
+import os
+import warnings
+from datetime import datetime, timedelta
+
+from shapely.geometry import Polygon
+
+from aisdb import DBConn, DBQuery, sqlfcn_callbacks, Domain, sqlfcn
+
+from aisdb.database.create_tables import sqlite_createtable_dynamicreport
+from aisdb.tests.create_testing_data import (
+    sample_database_file,
+    sample_gulfstlawrence_bbox,
+)
+
+
+def test_query_emptytable(tmpdir):
+    warnings.filterwarnings('error')
+    dbpath = os.path.join(tmpdir, 'test_query_emptytable.db')
+    with DBConn() as dbconn:
+        q = DBQuery(
+            dbconn=dbconn,
+            dbpath=dbpath,
+            start=datetime(2021, 1, 1),
+            end=datetime(2021, 1, 7),
+            callback=sqlfcn_callbacks.in_timerange_validmmsi,
+        )
+        sqlite_createtable_dynamicreport(dbconn, month='202101', dbpath=dbpath)
+        rows = q.gen_qry(reaggregate_static=True)
+        assert list(rows) == []
+
+
+def test_prepare_qry_domain(tmpdir):
+
+    testdbpath = os.path.join(tmpdir, 'test_prepare_qry_domain.db')
+    months = sample_database_file(testdbpath)
+    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
+    end = start + timedelta(weeks=4)
+    z1 = Polygon(zip(*sample_gulfstlawrence_bbox()))
+    domain = Domain('gulf domain', zones=[{'name': 'z1', 'geometry': z1}])
+    with DBConn() as aisdatabase:
+        rowgen = DBQuery(
+            dbconn=aisdatabase,
+            dbpath=testdbpath,
+            start=start,
+            end=end,
+            **domain.boundary,
+            callback=sqlfcn_callbacks.in_timerange,
+        ).gen_qry(reaggregate_static=True)
+        next(rowgen)
+
+
+def test_sql_query_strings(tmpdir):
+    testdbpath = os.path.join(tmpdir, 'test_sql_query_strings.db')
+    months = sample_database_file(testdbpath)
+    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
+    end = start + timedelta(weeks=4)
+    z1 = Polygon(zip(*sample_gulfstlawrence_bbox()))
+    domain = Domain('gulf domain', zones=[{'name': 'z1', 'geometry': z1}])
+    with DBConn() as aisdatabase:
+        for callback in [
+                sqlfcn_callbacks.in_bbox,
+                sqlfcn_callbacks.in_bbox_time,
+                sqlfcn_callbacks.in_bbox_time_validmmsi,
+                sqlfcn_callbacks.in_time_bbox_inmmsi,
+                sqlfcn_callbacks.in_timerange,
+                sqlfcn_callbacks.in_timerange_hasmmsi,
+                sqlfcn_callbacks.in_timerange_validmmsi,
+        ]:
+            rowgen = DBQuery(
+                dbconn=aisdatabase,
+                dbpath=testdbpath,
+                start=start,
+                end=end,
+                **domain.boundary,
+                callback=callback,
+                mmsi=316000000,
+                mmsis=[316000000, 316000001],
+            ).gen_qry(fcn=sqlfcn.crawl_dynamic_static)
+            next(rowgen)
```

## aisdb/tests/test_02_sqlfcn.py

 * *Ordering differences only*

```diff
@@ -1,94 +1,94 @@
-import os
-from datetime import datetime, timedelta
-
-import numpy as np
-
-from aisdb import sqlfcn, sqlfcn_callbacks
-
-y, x = 44., -63.
-start = datetime(2021, 5, 1)
-kwargs = dict(
-    start=start,
-    end=start + timedelta(days=7),
-    xmin=x - 5,
-    xmax=x + 5,
-    ymin=y - 5,
-    ymax=y + 5,
-)
-
-
-def test_dynamic(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_sqlfcn_dynamic.db')
-    month = "202105"
-    callback = sqlfcn_callbacks.in_time_bbox_validmmsi
-    txt = sqlfcn._dynamic(dbpath=dbpath,
-                          month=month,
-                          callback=callback,
-                          **kwargs)
-    print(txt)
-
-
-def test_static(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_sqlfcn_static.db')
-    month = "202105"
-    txt = sqlfcn._static(dbpath=dbpath, month=month)
-    print(txt)
-
-
-def test_leftjoin():
-    month = "202105"
-    txt = sqlfcn._leftjoin(month=month)
-    print(txt)
-
-
-def test_crawl(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_sqlfcn_crawl.db')
-    months = ['202105']
-    callback = sqlfcn_callbacks.in_time_bbox_validmmsi
-    txt = sqlfcn.crawl_dynamic_static(dbpath=dbpath,
-                                      months=months,
-                                      callback=callback,
-                                      **kwargs)
-    print(txt)
-    txt = sqlfcn.crawl_dynamic(dbpath=dbpath,
-                               months=months,
-                               callback=callback,
-                               **kwargs)
-    print(txt)
-
-
-def test_callbacks(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_sqlfcn_callbacks.db')
-    months = ['202105']
-    callback = sqlfcn_callbacks.in_time_bbox_validmmsi
-    for callback in [
-            sqlfcn_callbacks.in_bbox,
-            sqlfcn_callbacks.in_bbox_time,
-            sqlfcn_callbacks.in_bbox_time_validmmsi,
-            sqlfcn_callbacks.in_time_bbox,
-            sqlfcn_callbacks.in_time_bbox_hasmmsi,
-            sqlfcn_callbacks.in_time_bbox_inmmsi,
-            sqlfcn_callbacks.in_time_bbox_validmmsi,
-            sqlfcn_callbacks.in_time_mmsi,
-            sqlfcn_callbacks.in_timerange,
-            sqlfcn_callbacks.in_timerange_hasmmsi,
-            sqlfcn_callbacks.in_timerange_inmmsi,
-            sqlfcn_callbacks.in_timerange_validmmsi,
-    ]:
-        box_x = sorted(np.random.random(2) * 360 - 180)
-        box_y = sorted(np.random.random(2) * 180 - 90)
-        kwargs = dict(
-            start=start,
-            end=start + timedelta(days=7),
-            xmin=box_x[0],
-            xmax=box_x[1],
-            ymin=min(box_y),
-            ymax=max(box_y),
-        )
-        txt = sqlfcn.crawl_dynamic_static(dbpath=dbpath,
-                                          months=months,
-                                          callback=callback,
-                                          mmsi=316000000,
-                                          mmsis=[316000000],
-                                          **kwargs)
-        print(txt)
+import os
+from datetime import datetime, timedelta
+
+import numpy as np
+
+from aisdb import sqlfcn, sqlfcn_callbacks
+
+y, x = 44., -63.
+start = datetime(2021, 5, 1)
+kwargs = dict(
+    start=start,
+    end=start + timedelta(days=7),
+    xmin=x - 5,
+    xmax=x + 5,
+    ymin=y - 5,
+    ymax=y + 5,
+)
+
+
+def test_dynamic(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_sqlfcn_dynamic.db')
+    month = "202105"
+    callback = sqlfcn_callbacks.in_time_bbox_validmmsi
+    txt = sqlfcn._dynamic(dbpath=dbpath,
+                          month=month,
+                          callback=callback,
+                          **kwargs)
+    print(txt)
+
+
+def test_static(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_sqlfcn_static.db')
+    month = "202105"
+    txt = sqlfcn._static(dbpath=dbpath, month=month)
+    print(txt)
+
+
+def test_leftjoin():
+    month = "202105"
+    txt = sqlfcn._leftjoin(month=month)
+    print(txt)
+
+
+def test_crawl(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_sqlfcn_crawl.db')
+    months = ['202105']
+    callback = sqlfcn_callbacks.in_time_bbox_validmmsi
+    txt = sqlfcn.crawl_dynamic_static(dbpath=dbpath,
+                                      months=months,
+                                      callback=callback,
+                                      **kwargs)
+    print(txt)
+    txt = sqlfcn.crawl_dynamic(dbpath=dbpath,
+                               months=months,
+                               callback=callback,
+                               **kwargs)
+    print(txt)
+
+
+def test_callbacks(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_sqlfcn_callbacks.db')
+    months = ['202105']
+    callback = sqlfcn_callbacks.in_time_bbox_validmmsi
+    for callback in [
+            sqlfcn_callbacks.in_bbox,
+            sqlfcn_callbacks.in_bbox_time,
+            sqlfcn_callbacks.in_bbox_time_validmmsi,
+            sqlfcn_callbacks.in_time_bbox,
+            sqlfcn_callbacks.in_time_bbox_hasmmsi,
+            sqlfcn_callbacks.in_time_bbox_inmmsi,
+            sqlfcn_callbacks.in_time_bbox_validmmsi,
+            sqlfcn_callbacks.in_time_mmsi,
+            sqlfcn_callbacks.in_timerange,
+            sqlfcn_callbacks.in_timerange_hasmmsi,
+            sqlfcn_callbacks.in_timerange_inmmsi,
+            sqlfcn_callbacks.in_timerange_validmmsi,
+    ]:
+        box_x = sorted(np.random.random(2) * 360 - 180)
+        box_y = sorted(np.random.random(2) * 180 - 90)
+        kwargs = dict(
+            start=start,
+            end=start + timedelta(days=7),
+            xmin=box_x[0],
+            xmax=box_x[1],
+            ymin=min(box_y),
+            ymax=max(box_y),
+        )
+        txt = sqlfcn.crawl_dynamic_static(dbpath=dbpath,
+                                          months=months,
+                                          callback=callback,
+                                          mmsi=316000000,
+                                          mmsis=[316000000],
+                                          **kwargs)
+        print(txt)
```

## aisdb/tests/test_03_gis.py

 * *Ordering differences only*

```diff
@@ -1,105 +1,105 @@
-import os
-
-from shapely.geometry import Polygon
-import numpy as np
-import zipfile
-
-from aisdb.gis import (
-    Domain,
-    DomainFromPoints,
-    DomainFromTxts,
-    distance3D,
-    shiftcoord,
-)
-from aisdb.tests.create_testing_data import random_polygons_domain
-from aisdb.tests.create_testing_data import sample_gulfstlawrence_bbox
-
-
-def test_invalid_domain():
-    try:
-        Domain('errordomain', [{
-            'name':
-            'outofbounds0',
-            'geometry':
-            Polygon(zip([-200, -170, -170, -200, -200], [90, 90, 0, 0, 90]))
-        }, {
-            'name':
-            'outofbounds1',
-            'geometry':
-            Polygon(zip([200, 170, 170, 200, 200], [-90, -90, 0, 0, -90]))
-        }])
-    except ValueError:
-        return
-    except Exception as e:
-        raise (e)
-
-    raise RuntimeError('This test should fail with a ValueError')
-
-
-def test_domain():
-    domain = random_polygons_domain(count=10)
-    dist_to_centroids = domain.nearest_polygons_to_point(-64, 45)
-
-    print(dist_to_centroids)
-
-    for name, zone in domain.zones.items():
-        poly = zone['geometry']
-        print(poly.geom_type, end='|')
-    print()
-
-    zoneID = domain.point_in_polygon(zone['geometry'].centroid.x,
-                                     zone['geometry'].centroid.y)
-    print(f'{zoneID = }')
-
-    print(f'{domain.minX=}\n{domain.maxX=}\n{domain.minY=}\n{domain.maxY=}')
-
-
-def test_DomainFromTxts():
-    folder = os.path.join(os.path.dirname(__file__), 'test_zones')
-    zipf = os.path.join(folder, 'test_zones.zip')
-
-    with zipfile.ZipFile(zipf, 'r') as zip_ref:
-        members = list(
-            set(zip_ref.namelist()) - set(sorted(os.listdir(folder))))
-        zip_ref.extractall(path=folder, members=members)
-
-    domain = DomainFromTxts(domainName='test', folder=folder)
-    assert domain
-
-
-def test_DomainFromPoints():
-
-    domain = DomainFromPoints([(-45, 50), (-50, 35), (-40, 55)],
-                              [10000, 1000, 100000])
-    assert domain
-
-
-def test_domain_points_in_polygon():
-    lon, lat = sample_gulfstlawrence_bbox()
-    z1 = Polygon(zip(lon, lat))
-    z2 = Polygon(zip(lon - 145, lat))
-    z3 = Polygon(zip(lon, lat - 45))
-    domain1 = Domain('gulf domain', zones=[{'name': 'z1', 'geometry': z1}])
-
-    xx = [z1.centroid.x, z2.centroid.x, z3.centroid.x]
-    yy = [z1.centroid.y, z2.centroid.y, z3.centroid.y]
-    test = [domain1.point_in_polygon(x, y) for x, y in zip(xx, yy)]
-    assert test[0] == 'z1'
-    assert test[1] == 'Z0'
-    assert test[2] == 'Z0'
-
-
-def test_shiftcoord():
-    x = np.array([-360, -270, -180, -90, 0, 90, 180, 270, 360])
-    xshift = shiftcoord(x)
-    assert sum(xshift == np.array([0, 90, 180, -90, 0, 90, -180, -90, 0])) == 9
-
-    x2 = np.array([-200, -190, -181, -180, -179, -170, -160])
-    xshift2 = shiftcoord(x2)
-
-
-def test_distance3D():
-    x1, y1 = -45, 50
-    x2, y2 = -40, 50
-    depth_metres = -500
-    dist = distance3D(x1, y1, x2, y2, depth_metres)
+import os
+
+from shapely.geometry import Polygon
+import numpy as np
+import zipfile
+
+from aisdb.gis import (
+    Domain,
+    DomainFromPoints,
+    DomainFromTxts,
+    distance3D,
+    shiftcoord,
+)
+from aisdb.tests.create_testing_data import random_polygons_domain
+from aisdb.tests.create_testing_data import sample_gulfstlawrence_bbox
+
+
+def test_invalid_domain():
+    try:
+        Domain('errordomain', [{
+            'name':
+            'outofbounds0',
+            'geometry':
+            Polygon(zip([-200, -170, -170, -200, -200], [90, 90, 0, 0, 90]))
+        }, {
+            'name':
+            'outofbounds1',
+            'geometry':
+            Polygon(zip([200, 170, 170, 200, 200], [-90, -90, 0, 0, -90]))
+        }])
+    except ValueError:
+        return
+    except Exception as e:
+        raise (e)
+
+    raise RuntimeError('This test should fail with a ValueError')
+
+
+def test_domain():
+    domain = random_polygons_domain(count=10)
+    dist_to_centroids = domain.nearest_polygons_to_point(-64, 45)
+
+    print(dist_to_centroids)
+
+    for name, zone in domain.zones.items():
+        poly = zone['geometry']
+        print(poly.geom_type, end='|')
+    print()
+
+    zoneID = domain.point_in_polygon(zone['geometry'].centroid.x,
+                                     zone['geometry'].centroid.y)
+    print(f'{zoneID = }')
+
+    print(f'{domain.minX=}\n{domain.maxX=}\n{domain.minY=}\n{domain.maxY=}')
+
+
+def test_DomainFromTxts():
+    folder = os.path.join(os.path.dirname(__file__), 'test_zones')
+    zipf = os.path.join(folder, 'test_zones.zip')
+
+    with zipfile.ZipFile(zipf, 'r') as zip_ref:
+        members = list(
+            set(zip_ref.namelist()) - set(sorted(os.listdir(folder))))
+        zip_ref.extractall(path=folder, members=members)
+
+    domain = DomainFromTxts(domainName='test', folder=folder)
+    assert domain
+
+
+def test_DomainFromPoints():
+
+    domain = DomainFromPoints([(-45, 50), (-50, 35), (-40, 55)],
+                              [10000, 1000, 100000])
+    assert domain
+
+
+def test_domain_points_in_polygon():
+    lon, lat = sample_gulfstlawrence_bbox()
+    z1 = Polygon(zip(lon, lat))
+    z2 = Polygon(zip(lon - 145, lat))
+    z3 = Polygon(zip(lon, lat - 45))
+    domain1 = Domain('gulf domain', zones=[{'name': 'z1', 'geometry': z1}])
+
+    xx = [z1.centroid.x, z2.centroid.x, z3.centroid.x]
+    yy = [z1.centroid.y, z2.centroid.y, z3.centroid.y]
+    test = [domain1.point_in_polygon(x, y) for x, y in zip(xx, yy)]
+    assert test[0] == 'z1'
+    assert test[1] == 'Z0'
+    assert test[2] == 'Z0'
+
+
+def test_shiftcoord():
+    x = np.array([-360, -270, -180, -90, 0, 90, 180, 270, 360])
+    xshift = shiftcoord(x)
+    assert sum(xshift == np.array([0, 90, 180, -90, 0, 90, -180, -90, 0])) == 9
+
+    x2 = np.array([-200, -190, -181, -180, -179, -170, -160])
+    xshift2 = shiftcoord(x2)
+
+
+def test_distance3D():
+    x1, y1 = -45, 50
+    x2, y2 = -40, 50
+    depth_metres = -500
+    dist = distance3D(x1, y1, x2, y2, depth_metres)
```

## aisdb/tests/test_04_trackgen.py

 * *Ordering differences only*

```diff
@@ -1,67 +1,67 @@
-import os
-from datetime import datetime, timedelta
-
-import numpy as np
-
-from aisdb import track_gen, sqlfcn_callbacks
-from aisdb.gis import vesseltrack_3D_dist, mask_in_radius_2D
-from aisdb.database.dbconn import DBConn
-from aisdb.database.dbqry import DBQuery
-from aisdb import encode_greatcircledistance
-from aisdb.track_gen import min_speed_filter
-from aisdb.tests.create_testing_data import sample_database_file
-
-
-def test_TrackGen(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_trackgen.db')
-    months = sample_database_file(dbpath)
-    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
-    end = start + timedelta(weeks=4)
-
-    with DBConn() as dbconn:
-        qry = DBQuery(
-            dbconn=dbconn,
-            dbpath=dbpath,
-            start=start,
-            end=end,
-            callback=sqlfcn_callbacks.valid_mmsi,
-        )
-        rowgen = qry.gen_qry(verbose=True)
-        tracks = track_gen.TrackGen(rowgen, decimate=True)
-
-        for track in tracks:
-            assert 'time' in track.keys()
-            if len(track['time']) >= 3:
-                print(track)
-            assert isinstance(track['lon'], np.ndarray)
-            assert isinstance(track['lat'], np.ndarray)
-            assert isinstance(track['time'], np.ndarray)
-
-
-def test_min_speed_filter(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_trackgen_min_speed_filter_encode.db')
-    months = sample_database_file(dbpath)
-    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
-    end = start + timedelta(weeks=4)
-
-    target_xy = [44.51204273779117, -63.47468122107318][::-1]
-
-    with DBConn() as dbconn:
-        qry = DBQuery(
-            dbconn=dbconn,
-            dbpath=dbpath,
-            start=start,
-            end=end,
-            callback=sqlfcn_callbacks.in_timerange_validmmsi,
-        )
-        rowgen = qry.gen_qry(verbose=True)
-        tracks = vesseltrack_3D_dist(
-            mask_in_radius_2D(min_speed_filter(encode_greatcircledistance(
-                track_gen.TrackGen(rowgen, decimate=True),
-                distance_threshold=250000,
-            ),
-                                               minspeed=5),
-                              target_xy,
-                              distance_meters=100000), *target_xy, 0)
-        for track in tracks:
-            assert 'time' in track.keys()
+import os
+from datetime import datetime, timedelta
+
+import numpy as np
+
+from aisdb import track_gen, sqlfcn_callbacks
+from aisdb.gis import vesseltrack_3D_dist, mask_in_radius_2D
+from aisdb.database.dbconn import DBConn
+from aisdb.database.dbqry import DBQuery
+from aisdb import encode_greatcircledistance
+from aisdb.track_gen import min_speed_filter
+from aisdb.tests.create_testing_data import sample_database_file
+
+
+def test_TrackGen(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_trackgen.db')
+    months = sample_database_file(dbpath)
+    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
+    end = start + timedelta(weeks=4)
+
+    with DBConn() as dbconn:
+        qry = DBQuery(
+            dbconn=dbconn,
+            dbpath=dbpath,
+            start=start,
+            end=end,
+            callback=sqlfcn_callbacks.valid_mmsi,
+        )
+        rowgen = qry.gen_qry(verbose=True)
+        tracks = track_gen.TrackGen(rowgen, decimate=True)
+
+        for track in tracks:
+            assert 'time' in track.keys()
+            if len(track['time']) >= 3:
+                print(track)
+            assert isinstance(track['lon'], np.ndarray)
+            assert isinstance(track['lat'], np.ndarray)
+            assert isinstance(track['time'], np.ndarray)
+
+
+def test_min_speed_filter(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_trackgen_min_speed_filter_encode.db')
+    months = sample_database_file(dbpath)
+    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
+    end = start + timedelta(weeks=4)
+
+    target_xy = [44.51204273779117, -63.47468122107318][::-1]
+
+    with DBConn() as dbconn:
+        qry = DBQuery(
+            dbconn=dbconn,
+            dbpath=dbpath,
+            start=start,
+            end=end,
+            callback=sqlfcn_callbacks.in_timerange_validmmsi,
+        )
+        rowgen = qry.gen_qry(verbose=True)
+        tracks = vesseltrack_3D_dist(
+            mask_in_radius_2D(min_speed_filter(encode_greatcircledistance(
+                track_gen.TrackGen(rowgen, decimate=True),
+                distance_threshold=250000,
+            ),
+                                               minspeed=5),
+                              target_xy,
+                              distance_meters=100000), *target_xy, 0)
+        for track in tracks:
+            assert 'time' in track.keys()
```

## aisdb/tests/test_05_proc_util.py

 * *Ordering differences only*

```diff
@@ -1,132 +1,132 @@
-import aisdb
-import os
-from datetime import datetime, timedelta
-
-import numpy as np
-
-from aisdb import track_gen, sqlfcn_callbacks
-from aisdb.database.dbconn import DBConn
-from aisdb.database.dbqry import DBQuery
-from aisdb.database import sqlfcn
-from aisdb.tests.create_testing_data import sample_database_file
-from aisdb.webdata.marinetraffic import vessel_info, VesselInfo
-
-testdir = os.environ.get(
-    'AISDBTESTDIR',
-    os.path.join(
-        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
-        'testdata',
-    ),
-)
-if not os.path.isdir(testdir):
-    os.mkdir(testdir)
-
-trafficDBpath = os.path.join(testdir, 'marinetraffic_test.db')
-
-
-def test_epoch_dt_convert():
-    aisdb.proc_util._epoch_2_dt(1600000000)
-    aisdb.proc_util._epoch_2_dt([1600000000])
-
-
-def test_write_csv_rows(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_write_csv.db')
-    months = sample_database_file(dbpath)
-    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
-    end = start + timedelta(weeks=4)
-
-    with DBConn() as dbconn:
-        qry = DBQuery(
-            dbconn=dbconn,
-            dbpath=dbpath,
-            start=start,
-            end=end,
-            callback=sqlfcn_callbacks.in_timerange_validmmsi,
-        )
-        rowgen = qry.gen_qry(verbose=True)
-        aisdb.proc_util.write_csv_rows(
-            rowgen,
-            pathname=os.path.join(
-                tmpdir,
-                'test_write_csv_rows.csv',
-            ),
-        )
-
-
-def test_write_csv_fromdict(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_write_csv.db')
-    months = sample_database_file(dbpath)
-    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
-    end = start + timedelta(weeks=4)
-
-    with DBConn() as dbconn:
-        qry = DBQuery(
-            dbconn=dbconn,
-            dbpath=dbpath,
-            start=start,
-            end=end,
-            callback=sqlfcn_callbacks.in_timerange_validmmsi,
-        )
-
-        rowgen = qry.gen_qry(fcn=sqlfcn.crawl_dynamic, verbose=True)
-        tracks = track_gen.TrackGen(rowgen, decimate=True)
-        aisdb.proc_util.write_csv(tracks,
-                                  fpath=os.path.join(tmpdir,
-                                                     'test_write_csv.csv'))
-
-
-def test_write_csv_fromdict_marinetraffic(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_write_csv.db')
-    months = sample_database_file(dbpath)
-    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
-    end = start + timedelta(weeks=4)
-
-    vinfo_db = VesselInfo(trafficDBpath).trafficDB
-
-    with DBConn() as dbconn, vinfo_db as trafficDB:
-        qry = DBQuery(
-            dbconn=dbconn,
-            dbpath=dbpath,
-            start=start,
-            end=end,
-            callback=sqlfcn_callbacks.in_timerange_validmmsi,
-        )
-        qry.check_marinetraffic(dbpath,
-                                trafficDBpath,
-                                boundary={
-                                    'xmin': -45,
-                                    'xmax': -25,
-                                    'ymin': 30,
-                                    'ymax': 50,
-                                })
-
-        rowgen = qry.gen_qry(fcn=sqlfcn.crawl_dynamic_static, verbose=True)
-        tracks = vessel_info(track_gen.TrackGen(rowgen, decimate=True),
-                             trafficDB)
-        aisdb.proc_util.write_csv(tracks,
-                                  fpath=os.path.join(tmpdir,
-                                                     'test_write_csv.csv'))
-
-
-def test_glob_files():
-    aisdb.proc_util.glob_files(os.path.dirname(__file__), '.nm4')
-
-
-def test_getfiledate():
-    aisdb.proc_util.getfiledate(
-        os.path.join(os.path.dirname(__file__), 'testdata',
-                     'test_data_20211101.nm4'))
-    aisdb.proc_util.getfiledate(
-        os.path.join(os.path.dirname(__file__), 'testdata',
-                     'test_data_20210701.csv'))
-
-
-def test_binarysearch():
-    arr = np.array([1, 2, 3])
-    arr_desc = arr[::-1]
-    assert aisdb.aisdb.binarysearch_vector(arr, [2])[0] == 1
-    assert aisdb.aisdb.binarysearch_vector(arr, [5])[0] == 2
-    assert aisdb.aisdb.binarysearch_vector(arr, [-10])[0] == 0
-    assert aisdb.aisdb.binarysearch_vector(arr_desc, [10])[0] == 0
-    assert aisdb.aisdb.binarysearch_vector(arr_desc, [-5])[0] == 2
-    assert aisdb.aisdb.binarysearch_vector(arr_desc, [2])[0] == 1
+import aisdb
+import os
+from datetime import datetime, timedelta
+
+import numpy as np
+
+from aisdb import track_gen, sqlfcn_callbacks
+from aisdb.database.dbconn import DBConn
+from aisdb.database.dbqry import DBQuery
+from aisdb.database import sqlfcn
+from aisdb.tests.create_testing_data import sample_database_file
+from aisdb.webdata.marinetraffic import vessel_info, VesselInfo
+
+testdir = os.environ.get(
+    'AISDBTESTDIR',
+    os.path.join(
+        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
+        'testdata',
+    ),
+)
+if not os.path.isdir(testdir):
+    os.mkdir(testdir)
+
+trafficDBpath = os.path.join(testdir, 'marinetraffic_test.db')
+
+
+def test_epoch_dt_convert():
+    aisdb.proc_util._epoch_2_dt(1600000000)
+    aisdb.proc_util._epoch_2_dt([1600000000])
+
+
+def test_write_csv_rows(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_write_csv.db')
+    months = sample_database_file(dbpath)
+    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
+    end = start + timedelta(weeks=4)
+
+    with DBConn() as dbconn:
+        qry = DBQuery(
+            dbconn=dbconn,
+            dbpath=dbpath,
+            start=start,
+            end=end,
+            callback=sqlfcn_callbacks.in_timerange_validmmsi,
+        )
+        rowgen = qry.gen_qry(verbose=True)
+        aisdb.proc_util.write_csv_rows(
+            rowgen,
+            pathname=os.path.join(
+                tmpdir,
+                'test_write_csv_rows.csv',
+            ),
+        )
+
+
+def test_write_csv_fromdict(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_write_csv.db')
+    months = sample_database_file(dbpath)
+    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
+    end = start + timedelta(weeks=4)
+
+    with DBConn() as dbconn:
+        qry = DBQuery(
+            dbconn=dbconn,
+            dbpath=dbpath,
+            start=start,
+            end=end,
+            callback=sqlfcn_callbacks.in_timerange_validmmsi,
+        )
+
+        rowgen = qry.gen_qry(fcn=sqlfcn.crawl_dynamic, verbose=True)
+        tracks = track_gen.TrackGen(rowgen, decimate=True)
+        aisdb.proc_util.write_csv(tracks,
+                                  fpath=os.path.join(tmpdir,
+                                                     'test_write_csv.csv'))
+
+
+def test_write_csv_fromdict_marinetraffic(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_write_csv.db')
+    months = sample_database_file(dbpath)
+    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
+    end = start + timedelta(weeks=4)
+
+    vinfo_db = VesselInfo(trafficDBpath).trafficDB
+
+    with DBConn() as dbconn, vinfo_db as trafficDB:
+        qry = DBQuery(
+            dbconn=dbconn,
+            dbpath=dbpath,
+            start=start,
+            end=end,
+            callback=sqlfcn_callbacks.in_timerange_validmmsi,
+        )
+        qry.check_marinetraffic(dbpath,
+                                trafficDBpath,
+                                boundary={
+                                    'xmin': -45,
+                                    'xmax': -25,
+                                    'ymin': 30,
+                                    'ymax': 50,
+                                })
+
+        rowgen = qry.gen_qry(fcn=sqlfcn.crawl_dynamic_static, verbose=True)
+        tracks = vessel_info(track_gen.TrackGen(rowgen, decimate=True),
+                             trafficDB)
+        aisdb.proc_util.write_csv(tracks,
+                                  fpath=os.path.join(tmpdir,
+                                                     'test_write_csv.csv'))
+
+
+def test_glob_files():
+    aisdb.proc_util.glob_files(os.path.dirname(__file__), '.nm4')
+
+
+def test_getfiledate():
+    aisdb.proc_util.getfiledate(
+        os.path.join(os.path.dirname(__file__), 'testdata',
+                     'test_data_20211101.nm4'))
+    aisdb.proc_util.getfiledate(
+        os.path.join(os.path.dirname(__file__), 'testdata',
+                     'test_data_20210701.csv'))
+
+
+def test_binarysearch():
+    arr = np.array([1, 2, 3])
+    arr_desc = arr[::-1]
+    assert aisdb.aisdb.binarysearch_vector(arr, [2])[0] == 1
+    assert aisdb.aisdb.binarysearch_vector(arr, [5])[0] == 2
+    assert aisdb.aisdb.binarysearch_vector(arr, [-10])[0] == 0
+    assert aisdb.aisdb.binarysearch_vector(arr_desc, [10])[0] == 0
+    assert aisdb.aisdb.binarysearch_vector(arr_desc, [-5])[0] == 2
+    assert aisdb.aisdb.binarysearch_vector(arr_desc, [2])[0] == 1
```

## aisdb/tests/test_06_interp.py

 * *Ordering differences only*

```diff
@@ -1,34 +1,34 @@
-import os
-from datetime import datetime, timedelta
-
-from aisdb import track_gen, sqlfcn, sqlfcn_callbacks
-from aisdb.database.dbconn import DBConn
-from aisdb.database.dbqry import DBQuery
-from aisdb.tests.create_testing_data import sample_database_file
-from aisdb.interp import interp_time
-
-
-def test_interp(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_interp.db')
-    months = sample_database_file(dbpath)
-    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
-    end = start + timedelta(weeks=4)
-
-    with DBConn() as dbconn:
-        qry = DBQuery(
-            dbconn=dbconn,
-            dbpath=dbpath,
-            start=start,
-            end=end,
-            callback=sqlfcn_callbacks.in_timerange_validmmsi,
-        )
-        rowgen = qry.gen_qry(fcn=sqlfcn.crawl_dynamic_static, verbose=True)
-        tracks = interp_time(
-            track_gen.TrackGen(rowgen, decimate=True),
-            step=timedelta(hours=0.5),
-        )
-
-        for track in tracks:
-            assert 'time' in track.keys()
-            if len(track['time']) >= 3:
-                print(track)
+import os
+from datetime import datetime, timedelta
+
+from aisdb import track_gen, sqlfcn, sqlfcn_callbacks
+from aisdb.database.dbconn import DBConn
+from aisdb.database.dbqry import DBQuery
+from aisdb.tests.create_testing_data import sample_database_file
+from aisdb.interp import interp_time
+
+
+def test_interp(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_interp.db')
+    months = sample_database_file(dbpath)
+    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
+    end = start + timedelta(weeks=4)
+
+    with DBConn() as dbconn:
+        qry = DBQuery(
+            dbconn=dbconn,
+            dbpath=dbpath,
+            start=start,
+            end=end,
+            callback=sqlfcn_callbacks.in_timerange_validmmsi,
+        )
+        rowgen = qry.gen_qry(fcn=sqlfcn.crawl_dynamic_static, verbose=True)
+        tracks = interp_time(
+            track_gen.TrackGen(rowgen, decimate=True),
+            step=timedelta(hours=0.5),
+        )
+
+        for track in tracks:
+            assert 'time' in track.keys()
+            if len(track['time']) >= 3:
+                print(track)
```

## aisdb/tests/test_07_bathymetry.py

 * *Ordering differences only*

```diff
@@ -1,51 +1,51 @@
-import os
-import numpy as np
-
-from aisdb.webdata.bathymetry import Gebco
-
-data_dir = os.environ.get(
-    'AISDBDATADIR',
-    os.path.join(
-        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
-        'testdata',
-    ),
-)
-
-y1, x1 = 48.271185186388735, -61.10595523571155
-tracks_single = [
-    dict(
-        lon=np.array([x1]),
-        lat=np.array([y1]),
-        time=[0],
-        dynamic=set(['time']),
-    )
-]
-track1K = [
-    dict(
-        lon=(np.random.random(1000) * 90) - 90,
-        lat=(np.random.random(1000) * 90) + 0,
-        time=range(1000),
-        dynamic=set(['time']),
-    )
-]
-
-
-def test_fetch_bathygrid():
-    print(f'ENV: {os.getenv("AISDBDATADIR")=}')
-    print(f'checking bathymetry rasters: {data_dir=}')
-    bathy = Gebco(data_dir=data_dir)
-    assert bathy
-
-
-def test_bathymetry_single_pillow():
-    with Gebco(data_dir=data_dir) as bathy:
-        test = list(bathy.merge_tracks(tracks_single))
-        assert 'depth_metres' in test[0].keys()
-        assert 'depth_metres' in test[0]['dynamic']
-        print(test[0]['depth_metres'])
-
-
-def test_bathymetry_1K_pillow():
-    with Gebco(data_dir=data_dir) as bathy:
-        for updated in bathy.merge_tracks(track1K):
-            assert 'depth_metres' in updated.keys()
+import os
+import numpy as np
+
+from aisdb.webdata.bathymetry import Gebco
+
+data_dir = os.environ.get(
+    'AISDBDATADIR',
+    os.path.join(
+        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
+        'testdata',
+    ),
+)
+
+y1, x1 = 48.271185186388735, -61.10595523571155
+tracks_single = [
+    dict(
+        lon=np.array([x1]),
+        lat=np.array([y1]),
+        time=[0],
+        dynamic=set(['time']),
+    )
+]
+track1K = [
+    dict(
+        lon=(np.random.random(1000) * 90) - 90,
+        lat=(np.random.random(1000) * 90) + 0,
+        time=range(1000),
+        dynamic=set(['time']),
+    )
+]
+
+
+def test_fetch_bathygrid():
+    print(f'ENV: {os.getenv("AISDBDATADIR")=}')
+    print(f'checking bathymetry rasters: {data_dir=}')
+    bathy = Gebco(data_dir=data_dir)
+    assert bathy
+
+
+def test_bathymetry_single_pillow():
+    with Gebco(data_dir=data_dir) as bathy:
+        test = list(bathy.merge_tracks(tracks_single))
+        assert 'depth_metres' in test[0].keys()
+        assert 'depth_metres' in test[0]['dynamic']
+        print(test[0]['depth_metres'])
+
+
+def test_bathymetry_1K_pillow():
+    with Gebco(data_dir=data_dir) as bathy:
+        for updated in bathy.merge_tracks(track1K):
+            assert 'depth_metres' in updated.keys()
```

## aisdb/tests/test_07_shore_dist.py

 * *Ordering differences only*

```diff
@@ -1,42 +1,42 @@
-import os
-
-import numpy as np
-
-from aisdb.webdata.shore_dist import ShoreDist, PortDist
-
-data_dir = os.environ.get(
-    'AISDBDATADIR',
-    os.path.join(
-        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
-        'testdata',
-    ),
-)
-
-y1, x1 = 48.271185186388735, -61.10595523571155
-
-tracks_short = [
-    dict(
-        lon=np.array([x1]),
-        lat=np.array([y1]),
-        time=[0],
-        dynamic=set(['time']),
-    )
-]
-
-
-def test_ShoreDist():
-    imgpath = os.path.join(data_dir, 'distance-from-shore.tif')
-    assert os.path.isfile(imgpath)
-    with ShoreDist(data_dir=data_dir) as sdist:
-        for track in sdist.get_distance(tracks_short):
-            assert 'km_from_shore' in track.keys()
-            assert 'km_from_shore' in track['dynamic']
-
-
-def test_PortDist():
-    imgpath = os.path.join(data_dir, 'distance-from-port-v20201104.tiff')
-    with PortDist(imgpath=imgpath) as portdist:
-        #assert hasattr(portdist, 'get_distance')
-        for track in portdist.get_distance(tracks_short):
-            assert 'km_from_port' in track.keys()
-            assert 'km_from_port' in track['dynamic']
+import os
+
+import numpy as np
+
+from aisdb.webdata.shore_dist import ShoreDist, PortDist
+
+data_dir = os.environ.get(
+    'AISDBDATADIR',
+    os.path.join(
+        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
+        'testdata',
+    ),
+)
+
+y1, x1 = 48.271185186388735, -61.10595523571155
+
+tracks_short = [
+    dict(
+        lon=np.array([x1]),
+        lat=np.array([y1]),
+        time=[0],
+        dynamic=set(['time']),
+    )
+]
+
+
+def test_ShoreDist():
+    imgpath = os.path.join(data_dir, 'distance-from-shore.tif')
+    assert os.path.isfile(imgpath)
+    with ShoreDist(data_dir=data_dir) as sdist:
+        for track in sdist.get_distance(tracks_short):
+            assert 'km_from_shore' in track.keys()
+            assert 'km_from_shore' in track['dynamic']
+
+
+def test_PortDist():
+    imgpath = os.path.join(data_dir, 'distance-from-port-v20201104.tiff')
+    with PortDist(imgpath=imgpath) as portdist:
+        #assert hasattr(portdist, 'get_distance')
+        for track in portdist.get_distance(tracks_short):
+            assert 'km_from_port' in track.keys()
+            assert 'km_from_port' in track['dynamic']
```

## aisdb/tests/test_08_marinetraffic.py

 * *Ordering differences only*

```diff
@@ -1,82 +1,82 @@
-import os
-from datetime import datetime
-
-from shapely.geometry import Polygon
-
-from aisdb import track_gen, decode_msgs, DBQuery, sqlfcn_callbacks, Domain
-from aisdb.webdata.marinetraffic import vessel_info, _vessel_info_dict, VesselInfo
-from aisdb.tests.create_testing_data import sample_gulfstlawrence_bbox
-from aisdb import DBConn
-
-start = datetime(2021, 11, 1)
-end = datetime(2021, 11, 2)
-
-testdir = os.environ.get(
-    'AISDBTESTDIR',
-    os.path.join(
-        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
-        'testdata',
-    ),
-)
-if not os.path.isdir(testdir):
-    os.mkdir(testdir)
-
-trafficDBpath = os.path.join(testdir, 'marinetraffic_test.db')
-
-
-def test_init_scraper():
-    from aisdb.webdata._scraper import _scraper
-    _driver = _scraper()
-    _driver.close()
-    _driver.quit()
-
-
-def test_retrieve_marinetraffic_data(tmpdir):
-    #domain = random_polygons_domain(count=10)
-    coords = sample_gulfstlawrence_bbox()
-    poly = Polygon(zip(*coords))
-    domain = Domain(name='test_marinetraffic',
-                    zones=[{
-                        'name': 'gulfstlawrence',
-                        'geometry': poly
-                    }])
-
-    datapath = os.path.join(os.path.dirname(__file__), 'testdata',
-                            'test_data_20211101.nm4')
-    dbpath = os.path.join(tmpdir, 'test_retrieve_marinetraffic_data.db')
-
-    vinfoDB = VesselInfo(trafficDBpath).trafficDB
-
-    with DBConn() as dbconn, vinfoDB as trafficDB:
-        decode_msgs(filepaths=[datapath],
-                    dbconn=dbconn,
-                    dbpath=dbpath,
-                    source='TESTING')
-
-        qry = DBQuery(dbconn=dbconn,
-                      dbpath=dbpath,
-                      start=start,
-                      end=end,
-                      callback=sqlfcn_callbacks.in_timerange_validmmsi)
-        qry.check_marinetraffic(dbpath=dbpath,
-                                trafficDBpath=trafficDBpath,
-                                boundary=domain.boundary,
-                                retry_404=False)
-        rowgen = qry.gen_qry(verbose=True)
-        trackgen = track_gen.TrackGen(rowgen, decimate=True)
-        tracks = [next(trackgen), next(trackgen)]
-
-        try:
-
-            for track in vessel_info(tracks, trafficDB):
-                assert 'marinetraffic_info' in track.keys()
-        except UserWarning:
-            pass
-        except Exception as err:
-            raise err
-
-
-def test_marinetraffic_metadict():
-    trafficDB = VesselInfo(trafficDBpath).trafficDB
-    meta = _vessel_info_dict(trafficDB)
-    assert meta
+import os
+from datetime import datetime
+
+from shapely.geometry import Polygon
+
+from aisdb import track_gen, decode_msgs, DBQuery, sqlfcn_callbacks, Domain
+from aisdb.webdata.marinetraffic import vessel_info, _vessel_info_dict, VesselInfo
+from aisdb.tests.create_testing_data import sample_gulfstlawrence_bbox
+from aisdb import DBConn
+
+start = datetime(2021, 11, 1)
+end = datetime(2021, 11, 2)
+
+testdir = os.environ.get(
+    'AISDBTESTDIR',
+    os.path.join(
+        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
+        'testdata',
+    ),
+)
+if not os.path.isdir(testdir):
+    os.mkdir(testdir)
+
+trafficDBpath = os.path.join(testdir, 'marinetraffic_test.db')
+
+
+def test_init_scraper():
+    from aisdb.webdata._scraper import _scraper
+    _driver = _scraper()
+    _driver.close()
+    _driver.quit()
+
+
+def test_retrieve_marinetraffic_data(tmpdir):
+    #domain = random_polygons_domain(count=10)
+    coords = sample_gulfstlawrence_bbox()
+    poly = Polygon(zip(*coords))
+    domain = Domain(name='test_marinetraffic',
+                    zones=[{
+                        'name': 'gulfstlawrence',
+                        'geometry': poly
+                    }])
+
+    datapath = os.path.join(os.path.dirname(__file__), 'testdata',
+                            'test_data_20211101.nm4')
+    dbpath = os.path.join(tmpdir, 'test_retrieve_marinetraffic_data.db')
+
+    vinfoDB = VesselInfo(trafficDBpath).trafficDB
+
+    with DBConn() as dbconn, vinfoDB as trafficDB:
+        decode_msgs(filepaths=[datapath],
+                    dbconn=dbconn,
+                    dbpath=dbpath,
+                    source='TESTING')
+
+        qry = DBQuery(dbconn=dbconn,
+                      dbpath=dbpath,
+                      start=start,
+                      end=end,
+                      callback=sqlfcn_callbacks.in_timerange_validmmsi)
+        qry.check_marinetraffic(dbpath=dbpath,
+                                trafficDBpath=trafficDBpath,
+                                boundary=domain.boundary,
+                                retry_404=False)
+        rowgen = qry.gen_qry(verbose=True)
+        trackgen = track_gen.TrackGen(rowgen, decimate=True)
+        tracks = [next(trackgen), next(trackgen)]
+
+        try:
+
+            for track in vessel_info(tracks, trafficDB):
+                assert 'marinetraffic_info' in track.keys()
+        except UserWarning:
+            pass
+        except Exception as err:
+            raise err
+
+
+def test_marinetraffic_metadict():
+    trafficDB = VesselInfo(trafficDBpath).trafficDB
+    meta = _vessel_info_dict(trafficDB)
+    assert meta
```

## aisdb/tests/test_08_wsa.py

 * *Ordering differences only*

```diff
@@ -1,53 +1,53 @@
-import os
-from datetime import datetime, timedelta
-
-import warnings
-
-from aisdb import track_gen, DBQuery, sqlfcn_callbacks, DBConn
-from aisdb import encode_greatcircledistance
-from aisdb.wsa import wetted_surface_area
-from aisdb.database import sqlfcn
-from aisdb.webdata.marinetraffic import vessel_info, VesselInfo
-
-from aisdb.tests.create_testing_data import sample_database_file
-
-testdir = os.environ.get(
-    'AISDBTESTDIR',
-    os.path.join(
-        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
-        'testdata',
-    ),
-)
-if not os.path.isdir(testdir):
-    os.mkdir(testdir)
-
-trafficDBpath = os.path.join(testdir, 'marinetraffic_test.db')
-
-
-def test_wetted_surface_area_regression_marinetraffic(tmpdir):
-    dbpath = os.path.join(tmpdir, 'test_trackgen.db')
-    months = sample_database_file(dbpath)
-    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
-    end = start + timedelta(weeks=4)
-    vinfoDB = VesselInfo(trafficDBpath).trafficDB
-    with DBConn() as dbconn, warnings.catch_warnings(), vinfoDB as trafficDB:
-        warnings.simplefilter('ignore')
-
-        qry = DBQuery(
-            dbconn=dbconn,
-            dbpath=dbpath,
-            start=start,
-            end=end,
-            callback=sqlfcn_callbacks.in_timerange_validmmsi,
-        )
-        rowgen = qry.gen_qry(fcn=sqlfcn.crawl_dynamic_static, verbose=True)
-        tracks = vessel_info(
-            encode_greatcircledistance(
-                track_gen.TrackGen(rowgen, decimate=True),
-                distance_threshold=250000,
-            ),
-            dbconn=trafficDB,
-        )
-
-        for track in tracks:
-            track = next(wetted_surface_area([track]))
+import os
+from datetime import datetime, timedelta
+
+import warnings
+
+from aisdb import track_gen, DBQuery, sqlfcn_callbacks, DBConn
+from aisdb import encode_greatcircledistance
+from aisdb.wsa import wetted_surface_area
+from aisdb.database import sqlfcn
+from aisdb.webdata.marinetraffic import vessel_info, VesselInfo
+
+from aisdb.tests.create_testing_data import sample_database_file
+
+testdir = os.environ.get(
+    'AISDBTESTDIR',
+    os.path.join(
+        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
+        'testdata',
+    ),
+)
+if not os.path.isdir(testdir):
+    os.mkdir(testdir)
+
+trafficDBpath = os.path.join(testdir, 'marinetraffic_test.db')
+
+
+def test_wetted_surface_area_regression_marinetraffic(tmpdir):
+    dbpath = os.path.join(tmpdir, 'test_trackgen.db')
+    months = sample_database_file(dbpath)
+    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
+    end = start + timedelta(weeks=4)
+    vinfoDB = VesselInfo(trafficDBpath).trafficDB
+    with DBConn() as dbconn, warnings.catch_warnings(), vinfoDB as trafficDB:
+        warnings.simplefilter('ignore')
+
+        qry = DBQuery(
+            dbconn=dbconn,
+            dbpath=dbpath,
+            start=start,
+            end=end,
+            callback=sqlfcn_callbacks.in_timerange_validmmsi,
+        )
+        rowgen = qry.gen_qry(fcn=sqlfcn.crawl_dynamic_static, verbose=True)
+        tracks = vessel_info(
+            encode_greatcircledistance(
+                track_gen.TrackGen(rowgen, decimate=True),
+                distance_threshold=250000,
+            ),
+            dbconn=trafficDB,
+        )
+
+        for track in tracks:
+            track = next(wetted_surface_area([track]))
```

## aisdb/tests/test_09_network_graph.py

 * *Ordering differences only*

```diff
@@ -1,126 +1,126 @@
-'''
-from multiprocessing import set_start_method
-set_start_method('forkserver')
-from multiprocessing import Pool, Queue
-'''
-import os
-from datetime import datetime, timedelta
-
-from shapely.geometry import Polygon
-import warnings
-
-from aisdb.database import sqlfcn, sqlfcn_callbacks
-from aisdb.database.dbqry import DBQuery
-from aisdb.database.dbconn import DBConn
-from aisdb.gis import Domain
-from aisdb.network_graph import graph
-from aisdb.tests.create_testing_data import (
-    sample_database_file,
-    sample_gulfstlawrence_bbox,
-)
-
-trafficDBpath = os.environ.get(
-    'AISDBMARINETRAFFIC',
-    os.path.join(
-        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
-        'testdata',
-        'marinetraffic_test.db',
-    ))
-
-data_dir = os.environ.get(
-    'AISDBDATADIR',
-    os.path.join(
-        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
-        'testdata',
-    ),
-)
-
-lon, lat = sample_gulfstlawrence_bbox()
-z1 = Polygon(zip(lon, lat))
-z2 = Polygon(zip(lon - 45, lat))
-z3 = Polygon(zip(lon, lat - 45))
-
-
-def test_graph_minimal(tmpdir):
-    domain = Domain('gulf domain',
-                    zones=[
-                        {
-                            'name': 'z1',
-                            'geometry': z1
-                        },
-                        {
-                            'name': 'z2',
-                            'geometry': z2
-                        },
-                        {
-                            'name': 'z3',
-                            'geometry': z3
-                        },
-                    ])
-
-    testdbpath = os.path.join(tmpdir, 'test_graph_minimal.db')
-
-    months = sample_database_file(testdbpath)
-    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
-    end = start + timedelta(weeks=1)
-
-    with DBConn() as aisdatabase:
-        qry = DBQuery(
-            dbconn=aisdatabase,
-            dbpath=testdbpath,
-            start=start,
-            end=end,
-            callback=sqlfcn_callbacks.in_bbox,
-            fcn=sqlfcn.crawl_dynamic_static,
-            **domain.boundary,
-        )
-
-        outputfile = os.path.join(tmpdir, "output.csv")
-
-        bathy_dir = None
-        if os.path.isfile(os.path.join(data_dir, 'gebco_2022_geotiff.zip')):
-            bathy_dir = data_dir
-
-        shoredist_raster = None
-        if os.path.isfile((p := os.path.join(data_dir,
-                                             'distance-from-shore.tif'))):
-            shoredist_raster = p
-
-        portdist_raster = None
-        if os.path.isfile((p :=
-                           os.path.join(data_dir,
-                                        'distance-from-port-v20201104.tiff'))):
-            portdist_raster = p
-
-        print(f'raw count: {len(list(qry.gen_qry()))}')
-
-        graph(
-            qry,
-            outputfile=outputfile,
-            data_dir=data_dir,
-            dbconn=aisdatabase,
-            domain=domain,
-            trafficDBpath=trafficDBpath,
-            bathy_dir=bathy_dir,
-            portdist_raster=portdist_raster,
-            shoredist_raster=shoredist_raster,
-        )
-
-    if os.path.isfile(outputfile):
-        os.remove(outputfile)
-    else:
-        warnings.warn("no output file generated for test graph")
-    os.remove(testdbpath)
-
-
-'''
-    import tempfile
-    import cProfile
-
-    data_dir = '/RAID0/ais/'
-    trafficDBpath = './testdata/marinetraffic_test.db'
-
-    with tempfile.TemporaryDirectory() as tmpdir:
-        cProfile.run("test_graph_pipeline_timing(tmpdir)", sort="tottime")
-        #cProfile.run("test_network_graph_CSV(tmpdir)", sort="tottime")
-'''
+'''
+from multiprocessing import set_start_method
+set_start_method('forkserver')
+from multiprocessing import Pool, Queue
+'''
+import os
+from datetime import datetime, timedelta
+
+from shapely.geometry import Polygon
+import warnings
+
+from aisdb.database import sqlfcn, sqlfcn_callbacks
+from aisdb.database.dbqry import DBQuery
+from aisdb.database.dbconn import DBConn
+from aisdb.gis import Domain
+from aisdb.network_graph import graph
+from aisdb.tests.create_testing_data import (
+    sample_database_file,
+    sample_gulfstlawrence_bbox,
+)
+
+trafficDBpath = os.environ.get(
+    'AISDBMARINETRAFFIC',
+    os.path.join(
+        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
+        'testdata',
+        'marinetraffic_test.db',
+    ))
+
+data_dir = os.environ.get(
+    'AISDBDATADIR',
+    os.path.join(
+        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
+        'testdata',
+    ),
+)
+
+lon, lat = sample_gulfstlawrence_bbox()
+z1 = Polygon(zip(lon, lat))
+z2 = Polygon(zip(lon - 45, lat))
+z3 = Polygon(zip(lon, lat - 45))
+
+
+def test_graph_minimal(tmpdir):
+    domain = Domain('gulf domain',
+                    zones=[
+                        {
+                            'name': 'z1',
+                            'geometry': z1
+                        },
+                        {
+                            'name': 'z2',
+                            'geometry': z2
+                        },
+                        {
+                            'name': 'z3',
+                            'geometry': z3
+                        },
+                    ])
+
+    testdbpath = os.path.join(tmpdir, 'test_graph_minimal.db')
+
+    months = sample_database_file(testdbpath)
+    start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
+    end = start + timedelta(weeks=1)
+
+    with DBConn() as aisdatabase:
+        qry = DBQuery(
+            dbconn=aisdatabase,
+            dbpath=testdbpath,
+            start=start,
+            end=end,
+            callback=sqlfcn_callbacks.in_bbox,
+            fcn=sqlfcn.crawl_dynamic_static,
+            **domain.boundary,
+        )
+
+        outputfile = os.path.join(tmpdir, "output.csv")
+
+        bathy_dir = None
+        if os.path.isfile(os.path.join(data_dir, 'gebco_2022_geotiff.zip')):
+            bathy_dir = data_dir
+
+        shoredist_raster = None
+        if os.path.isfile((p := os.path.join(data_dir,
+                                             'distance-from-shore.tif'))):
+            shoredist_raster = p
+
+        portdist_raster = None
+        if os.path.isfile((p :=
+                           os.path.join(data_dir,
+                                        'distance-from-port-v20201104.tiff'))):
+            portdist_raster = p
+
+        print(f'raw count: {len(list(qry.gen_qry()))}')
+
+        graph(
+            qry,
+            outputfile=outputfile,
+            data_dir=data_dir,
+            dbconn=aisdatabase,
+            domain=domain,
+            trafficDBpath=trafficDBpath,
+            bathy_dir=bathy_dir,
+            portdist_raster=portdist_raster,
+            shoredist_raster=shoredist_raster,
+        )
+
+    if os.path.isfile(outputfile):
+        os.remove(outputfile)
+    else:
+        warnings.warn("no output file generated for test graph")
+    os.remove(testdbpath)
+
+
+'''
+    import tempfile
+    import cProfile
+
+    data_dir = '/RAID0/ais/'
+    trafficDBpath = './testdata/marinetraffic_test.db'
+
+    with tempfile.TemporaryDirectory() as tmpdir:
+        cProfile.run("test_graph_pipeline_timing(tmpdir)", sort="tottime")
+        #cProfile.run("test_network_graph_CSV(tmpdir)", sort="tottime")
+'''
```

## aisdb/tests/test_11_postgres.py

 * *Ordering differences only*

```diff
@@ -1,32 +1,32 @@
-import os
-from aisdb.database.dbconn import PostgresDBConn
-
-#import dotenv
-#dotenv.load_dotenv()
-
-
-def test_postgres():
-
-    # keyword arguments
-    with PostgresDBConn(
-            #host='db',
-            #hostaddr='127.0.0.1/postgres',
-            hostaddr='fc00::9',
-            user='postgres',
-            port=5432,
-            password=os.environ.get('POSTGRES_PASSWORD', 'devel'),
-    ) as dbconn:
-        cur = dbconn.cursor()
-        cur.execute('select * from coarsetype_ref;')
-        res = cur.fetchall()
-        print(res)
-
-
-# libpq connection string
-'''
-with PostgresDBConn('postgresql://127.0.0.1:443/postgres?') as dbconn:
-    with dbconn.cursor() as cur:
-        cur.execute('select * from coarsetype_ref;')
-        res = cur.fetchall()
-        print(res)
-'''
+import os
+from aisdb.database.dbconn import PostgresDBConn
+
+#import dotenv
+#dotenv.load_dotenv()
+
+
+def test_postgres():
+
+    # keyword arguments
+    with PostgresDBConn(
+            #host='db',
+            #hostaddr='127.0.0.1/postgres',
+            hostaddr='fc00::9',
+            user='postgres',
+            port=5432,
+            password=os.environ.get('POSTGRES_PASSWORD', 'devel'),
+    ) as dbconn:
+        cur = dbconn.cursor()
+        cur.execute('select * from coarsetype_ref;')
+        res = cur.fetchall()
+        print(res)
+
+
+# libpq connection string
+'''
+with PostgresDBConn('postgresql://127.0.0.1:443/postgres?') as dbconn:
+    with dbconn.cursor() as cur:
+        cur.execute('select * from coarsetype_ref;')
+        res = cur.fetchall()
+        print(res)
+'''
```

## aisdb/tests/test_rx.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-def test_import_receiver():
-    from aisdb.receiver import start_receiver
+def test_import_receiver():
+    from aisdb.receiver import start_receiver
```

## aisdb/track_gen.py

 * *Ordering differences only*

```diff
@@ -1,224 +1,224 @@
-''' generation, segmentation, and filtering of vessel trajectories '''
-
-from functools import reduce
-from datetime import timedelta
-import sqlite3
-import types
-
-import numpy as np
-
-from aisdb.aisdb import simplify_linestring_idx
-from aisdb.gis import delta_knots
-from aisdb.proc_util import _segment_rng
-from aisdb import Domain
-
-staticcols = set([
-    'mmsi', 'vessel_name', 'ship_type', 'ship_type_txt', 'dim_bow',
-    'dim_stern', 'dim_port', 'dim_star', 'imo', 'draught'
-])
-
-
-def _segment_longitude(track, tolerance=300):
-    ''' segment track vectors where difference in longitude exceeds 300 degrees
-    '''
-
-    if len(track['time']) == 1:
-        yield track
-        return
-
-    diff = np.nonzero(
-        np.abs(track['lon'][1:] - track['lon'][:-1]) > tolerance)[0] + 1
-
-    if diff.size == 0:
-        assert 'time' in track.keys()
-        yield track
-        return
-
-    segments_idx = reduce(np.append, ([0], diff, [track['time'].size]))
-    for i in range(segments_idx.size - 1):
-        tracksplit = dict(
-            **{k: track[k]
-               for k in track['static']},
-            **{
-                k: track[k][segments_idx[i]:segments_idx[i + 1]]
-                for k in track['dynamic']
-            },
-            static=track['static'],
-            dynamic=track['dynamic'],
-        )
-        assert 'time' in tracksplit.keys()
-        yield tracksplit
-
-
-def _yieldsegments(rows, staticcols, dynamiccols, decimate=0.0001):
-    if decimate is True:
-        decimate = 0.0001
-    lon = np.array([r['longitude'] for r in rows], dtype=float)
-    lat = np.array([r['latitude'] for r in rows], dtype=float)
-    time = np.array([r['time'] for r in rows], dtype=np.uint32)
-    if decimate is not False:
-        idx = simplify_linestring_idx(lon, lat, precision=decimate)
-    else:
-        idx = np.array(range(len(lon)))
-    trackdict = dict(
-        **{col: rows[0][col]
-           for col in staticcols},
-        lon=lon[idx].astype(np.float32),
-        lat=lat[idx].astype(np.float32),
-        time=time[idx],
-        sog=np.array([r['sog'] for r in rows], dtype=np.float32)[idx],
-        cog=np.array([r['cog'] for r in rows], dtype=np.uint32)[idx],
-        static=staticcols,
-        dynamic=dynamiccols,
-    )
-    assert 'time' in trackdict.keys()
-
-    for segment in _segment_longitude(trackdict):
-        for key in segment['dynamic']:
-            assert len(segment[key]) == len(segment['time'])
-        yield segment
-
-
-def TrackGen(rowgen: iter, decimate: False) -> dict:
-    ''' generator converting sets of rows sorted by MMSI to a
-        dictionary containing track column vectors.
-        each row contains columns from database: mmsi time lon lat name ...
-        rows must be sorted by first by mmsi, then time
-
-        args:
-            rowgen (aisdb.database.dbqry.DBQuery.gen_qry())
-                DBQuery rows generator. Yields rows returned
-                by a database query
-            decimate (bool)
-                if True, linear curve decimation will be applied to reduce
-                the number of unnecessary datapoints
-
-        yields:
-            dictionary containing track column vectors.
-            static data (e.g. mmsi, name, geometry) will be stored as
-            scalar values
-
-        >>> import os
-        >>> from datetime import datetime
-        >>> from aisdb import DBConn, DBQuery, TrackGen, decode_msgs
-        >>> from aisdb.database import sqlfcn_callbacks
-        >>> # create example database file
-        >>> dbpath = 'track_gen_test.db'
-        >>> filepaths = ['aisdb/tests/testdata/test_data_20210701.csv',
-        ...              'aisdb/tests/testdata/test_data_20211101.nm4']
-        >>> with DBConn() as dbconn:
-        ...     decode_msgs(filepaths=filepaths, dbconn=dbconn, dbpath=dbpath,
-        ...     source='TESTING')
-        ...     q = DBQuery(callback=sqlfcn_callbacks.in_timerange_validmmsi,
-        ...             dbconn=dbconn,
-        ...             dbpath=dbpath,
-        ...             start=datetime(2021, 7, 1),
-        ...             end=datetime(2021, 7, 7))
-        ...     rowgen = q.gen_qry()
-        ...     for track in TrackGen(rowgen, decimate=True):
-        ...         print(track['mmsi'], track['lon'], track['lat'], track['time'])
-        ...         break
-        204242000 [-8.931666] [41.45] [1625176725]
-        >>> os.remove(dbpath)
-    '''
-    firstrow = True
-    assert isinstance(rowgen, types.GeneratorType)
-    for rows in rowgen:
-        assert not (rows is None or len(rows) == 0), 'rows cannot be empty'
-        assert isinstance(rows[0], (sqlite3.Row, dict))
-        if firstrow:
-            keys = set(rows[0].keys())
-            static = keys.intersection(set(staticcols))
-            dynamiccols = keys ^ static
-            dynamiccols = dynamiccols.difference(set(['longitude',
-                                                      'latitude']))
-            dynamiccols = dynamiccols.union(set(['lon', 'lat']))
-            firstrow = False
-        for track in _yieldsegments(rows, static, dynamiccols, decimate):
-            yield track
-
-
-def split_timedelta(tracks, maxdelta=timedelta(weeks=2)):
-    ''' partitions tracks where delta time exceeds maxdelta
-
-        args:
-            tracks (aisdb.track_gen.TrackGen)
-                track vectors generator
-            maxdelta (datetime.timedelta)
-                threshold at which tracks should be
-                partitioned
-    '''
-    for track in tracks:
-        for rng in _segment_rng(track, maxdelta):
-            assert len(rng) > 0
-            yield dict(
-                **{k: track[k]
-                   for k in track['static']},
-                **{
-                    k: np.array(track[k], dtype=type(track[k][0]))[rng]
-                    for k in track['dynamic']
-                },
-                static=track['static'],
-                dynamic=track['dynamic'],
-            )
-
-
-def fence_tracks(tracks, domain):
-    ''' compute points-in-polygons for vessel positions within domain polygons
-
-        yields track dictionaries
-
-        Also see zone_mask()
-    '''
-    assert isinstance(domain, Domain), 'Not a domain object'
-
-    for track in tracks:
-        assert isinstance(track, dict)
-        if 'in_zone' not in track.keys():
-            track['in_zone'] = np.array(
-                [
-                    domain.point_in_polygon(x, y)
-                    for x, y in zip(track['lon'], track['lat'])
-                ],
-                dtype=object,
-            )
-            track['dynamic'] = set(track['dynamic']).union(set(['in_zone']))
-        yield track
-
-
-def zone_mask(tracks, domain):
-    ''' compute points-in-polygons for track positions, and filter results to
-        positions within domain.
-
-        yields track dictionaries.
-
-        also see fence_tracks()
-    '''
-    for track in fence_tracks(tracks, domain):
-        mask = track['in_zone'] != 'Z0'
-        yield dict(
-            **{k: track[k]
-               for k in track['static']},
-            **{k: track[k][mask]
-               for k in track['dynamic']},
-            static=track['static'],
-            dynamic=track['dynamic'],
-        )
-
-
-def min_speed_filter(tracks, minspeed):
-    for track in tracks:
-        if len(track['time']) == 1:
-            yield track
-            continue
-        deltas = delta_knots(track)
-        deltas = np.append(deltas, [deltas[-1]])
-        mask = deltas >= minspeed
-        yield dict(
-            **{k: track[k]
-               for k in track['static']},
-            **{k: track[k][mask]
-               for k in track['dynamic']},
-            static=track['static'],
-            dynamic=track['dynamic'],
-        )
+''' generation, segmentation, and filtering of vessel trajectories '''
+
+from functools import reduce
+from datetime import timedelta
+import sqlite3
+import types
+
+import numpy as np
+
+from aisdb.aisdb import simplify_linestring_idx
+from aisdb.gis import delta_knots
+from aisdb.proc_util import _segment_rng
+from aisdb import Domain
+
+staticcols = set([
+    'mmsi', 'vessel_name', 'ship_type', 'ship_type_txt', 'dim_bow',
+    'dim_stern', 'dim_port', 'dim_star', 'imo', 'draught'
+])
+
+
+def _segment_longitude(track, tolerance=300):
+    ''' segment track vectors where difference in longitude exceeds 300 degrees
+    '''
+
+    if len(track['time']) == 1:
+        yield track
+        return
+
+    diff = np.nonzero(
+        np.abs(track['lon'][1:] - track['lon'][:-1]) > tolerance)[0] + 1
+
+    if diff.size == 0:
+        assert 'time' in track.keys()
+        yield track
+        return
+
+    segments_idx = reduce(np.append, ([0], diff, [track['time'].size]))
+    for i in range(segments_idx.size - 1):
+        tracksplit = dict(
+            **{k: track[k]
+               for k in track['static']},
+            **{
+                k: track[k][segments_idx[i]:segments_idx[i + 1]]
+                for k in track['dynamic']
+            },
+            static=track['static'],
+            dynamic=track['dynamic'],
+        )
+        assert 'time' in tracksplit.keys()
+        yield tracksplit
+
+
+def _yieldsegments(rows, staticcols, dynamiccols, decimate=0.0001):
+    if decimate is True:
+        decimate = 0.0001
+    lon = np.array([r['longitude'] for r in rows], dtype=float)
+    lat = np.array([r['latitude'] for r in rows], dtype=float)
+    time = np.array([r['time'] for r in rows], dtype=np.uint32)
+    if decimate is not False:
+        idx = simplify_linestring_idx(lon, lat, precision=decimate)
+    else:
+        idx = np.array(range(len(lon)))
+    trackdict = dict(
+        **{col: rows[0][col]
+           for col in staticcols},
+        lon=lon[idx].astype(np.float32),
+        lat=lat[idx].astype(np.float32),
+        time=time[idx],
+        sog=np.array([r['sog'] for r in rows], dtype=np.float32)[idx],
+        cog=np.array([r['cog'] for r in rows], dtype=np.uint32)[idx],
+        static=staticcols,
+        dynamic=dynamiccols,
+    )
+    assert 'time' in trackdict.keys()
+
+    for segment in _segment_longitude(trackdict):
+        for key in segment['dynamic']:
+            assert len(segment[key]) == len(segment['time'])
+        yield segment
+
+
+def TrackGen(rowgen: iter, decimate: False) -> dict:
+    ''' generator converting sets of rows sorted by MMSI to a
+        dictionary containing track column vectors.
+        each row contains columns from database: mmsi time lon lat name ...
+        rows must be sorted by first by mmsi, then time
+
+        args:
+            rowgen (aisdb.database.dbqry.DBQuery.gen_qry())
+                DBQuery rows generator. Yields rows returned
+                by a database query
+            decimate (bool)
+                if True, linear curve decimation will be applied to reduce
+                the number of unnecessary datapoints
+
+        yields:
+            dictionary containing track column vectors.
+            static data (e.g. mmsi, name, geometry) will be stored as
+            scalar values
+
+        >>> import os
+        >>> from datetime import datetime
+        >>> from aisdb import DBConn, DBQuery, TrackGen, decode_msgs
+        >>> from aisdb.database import sqlfcn_callbacks
+        >>> # create example database file
+        >>> dbpath = 'track_gen_test.db'
+        >>> filepaths = ['aisdb/tests/testdata/test_data_20210701.csv',
+        ...              'aisdb/tests/testdata/test_data_20211101.nm4']
+        >>> with DBConn() as dbconn:
+        ...     decode_msgs(filepaths=filepaths, dbconn=dbconn, dbpath=dbpath,
+        ...     source='TESTING')
+        ...     q = DBQuery(callback=sqlfcn_callbacks.in_timerange_validmmsi,
+        ...             dbconn=dbconn,
+        ...             dbpath=dbpath,
+        ...             start=datetime(2021, 7, 1),
+        ...             end=datetime(2021, 7, 7))
+        ...     rowgen = q.gen_qry()
+        ...     for track in TrackGen(rowgen, decimate=True):
+        ...         print(track['mmsi'], track['lon'], track['lat'], track['time'])
+        ...         break
+        204242000 [-8.931666] [41.45] [1625176725]
+        >>> os.remove(dbpath)
+    '''
+    firstrow = True
+    assert isinstance(rowgen, types.GeneratorType)
+    for rows in rowgen:
+        assert not (rows is None or len(rows) == 0), 'rows cannot be empty'
+        assert isinstance(rows[0], (sqlite3.Row, dict))
+        if firstrow:
+            keys = set(rows[0].keys())
+            static = keys.intersection(set(staticcols))
+            dynamiccols = keys ^ static
+            dynamiccols = dynamiccols.difference(set(['longitude',
+                                                      'latitude']))
+            dynamiccols = dynamiccols.union(set(['lon', 'lat']))
+            firstrow = False
+        for track in _yieldsegments(rows, static, dynamiccols, decimate):
+            yield track
+
+
+def split_timedelta(tracks, maxdelta=timedelta(weeks=2)):
+    ''' partitions tracks where delta time exceeds maxdelta
+
+        args:
+            tracks (aisdb.track_gen.TrackGen)
+                track vectors generator
+            maxdelta (datetime.timedelta)
+                threshold at which tracks should be
+                partitioned
+    '''
+    for track in tracks:
+        for rng in _segment_rng(track, maxdelta):
+            assert len(rng) > 0
+            yield dict(
+                **{k: track[k]
+                   for k in track['static']},
+                **{
+                    k: np.array(track[k], dtype=type(track[k][0]))[rng]
+                    for k in track['dynamic']
+                },
+                static=track['static'],
+                dynamic=track['dynamic'],
+            )
+
+
+def fence_tracks(tracks, domain):
+    ''' compute points-in-polygons for vessel positions within domain polygons
+
+        yields track dictionaries
+
+        Also see zone_mask()
+    '''
+    assert isinstance(domain, Domain), 'Not a domain object'
+
+    for track in tracks:
+        assert isinstance(track, dict)
+        if 'in_zone' not in track.keys():
+            track['in_zone'] = np.array(
+                [
+                    domain.point_in_polygon(x, y)
+                    for x, y in zip(track['lon'], track['lat'])
+                ],
+                dtype=object,
+            )
+            track['dynamic'] = set(track['dynamic']).union(set(['in_zone']))
+        yield track
+
+
+def zone_mask(tracks, domain):
+    ''' compute points-in-polygons for track positions, and filter results to
+        positions within domain.
+
+        yields track dictionaries.
+
+        also see fence_tracks()
+    '''
+    for track in fence_tracks(tracks, domain):
+        mask = track['in_zone'] != 'Z0'
+        yield dict(
+            **{k: track[k]
+               for k in track['static']},
+            **{k: track[k][mask]
+               for k in track['dynamic']},
+            static=track['static'],
+            dynamic=track['dynamic'],
+        )
+
+
+def min_speed_filter(tracks, minspeed):
+    for track in tracks:
+        if len(track['time']) == 1:
+            yield track
+            continue
+        deltas = delta_knots(track)
+        deltas = np.append(deltas, [deltas[-1]])
+        mask = deltas >= minspeed
+        yield dict(
+            **{k: track[k]
+               for k in track['static']},
+            **{k: track[k][mask]
+               for k in track['dynamic']},
+            static=track['static'],
+            dynamic=track['dynamic'],
+        )
```

## aisdb/webdata/bathymetry.py

 * *Ordering differences only*

```diff
@@ -1,150 +1,150 @@
-''' load bathymetry data from GEBCO raster files '''
-
-import hashlib
-import os
-import zipfile
-from functools import reduce
-
-import numpy as np
-import requests
-import warnings
-from tqdm import tqdm
-
-from aisdb.gis import shiftcoord
-from aisdb.webdata.load_raster import RasterFile
-
-url = 'https://www.bodc.ac.uk/data/open_download/gebco/gebco_2022/geotiff/'
-
-
-def _filebounds(fpath):
-    return {
-        f[0]: float(f[1:])
-        for f in fpath.split('gebco_2022_', 1)[1].rsplit('.tif', 1)[0].split(
-            '_')
-    }
-
-
-class Gebco():
-
-    def __init__(self, data_dir):
-        '''
-            args:
-                data_dir (string)
-                    folder where rasters should be stored
-        '''
-        self.data_dir = data_dir
-        assert os.path.isdir(data_dir)
-        self.__enter__()
-
-    def __enter__(self):
-        self.rasterfiles = {
-            f: _filebounds(f)
-            for f in {
-                k: None
-                for k in sorted([
-                    f for f in os.listdir(self.data_dir)
-                    if f[-4:] == '.tif' and 'gebco_2022' in f
-                ])
-            }
-        }
-
-        # download bathymetry rasters if missing
-        self.fetch_bathymetry_grid()
-
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self._close_all()
-
-    def fetch_bathymetry_grid(self):  # pragma: no cover
-        """ download geotiff zip archive and extract it """
-
-        zipf = os.path.join(self.data_dir, "gebco_2022_geotiff.zip")
-        try:
-
-            # download the file if necessary
-            if not os.path.isfile(zipf):
-                print('downloading gebco bathymetry...')
-                with requests.get(url, stream=True) as payload:
-                    assert payload.status_code == 200, 'error fetching file'
-                    with open(zipf, 'wb') as f:
-                        with tqdm(total=4011413504,
-                                  desc=zipf,
-                                  unit='B',
-                                  unit_scale=True) as t:
-                            for chunk in payload.iter_content(chunk_size=8192):
-                                _ = t.update(f.write(chunk))
-
-                with open(zipf, 'rb') as z:
-                    sha256sum = hashlib.sha256(z.read()).hexdigest()
-                print('verifying checksum...')
-                assert sha256sum == '5ade15083909fcd6003409df678bdc6537b8691df996f8d806b48de962470cc3',\
-                        'checksum failed!'
-                with zipfile.ZipFile(zipf, 'r') as zip_ref:
-                    members = list(
-                        set(zip_ref.namelist()) -
-                        set(sorted(os.listdir(self.data_dir))))
-                    print('extracting bathymetry data...')
-                    zip_ref.extractall(path=self.data_dir, members=members)
-        except (Exception, KeyboardInterrupt) as err:
-            os.remove(os.path.join(self.data_dir, "gebco_2022_geotiff.zip"))
-            raise (err)
-        return
-
-    def _load_raster(self, key):
-        self.rasterfiles[key]['raster'] = RasterFile(
-            imgpath=os.path.join(self.data_dir, key))
-
-    def _check_in_bounds(self, track):
-        for lon, lat in zip(track['lon'], track['lat']):
-            if not (-180 <= lon <= 180) or not (-90 <= lat <=
-                                                90):  # pragma: no cover
-                warnings.warn('coordinates out of range!')
-                lon = shiftcoord([lon])[0]
-                lat = shiftcoord([lat], rng=90)[0]
-
-            if os.environ.get('DEBUG'):
-                tracer = False
-            for key, bounds in self.rasterfiles.items():
-                if (bounds['w'] <= lon <= bounds['e']
-                        and bounds['s'] <= lat <= bounds['n']):
-                    tracer = True
-                    if 'raster' not in bounds.keys():
-                        self._load_raster(key)
-                    yield key
-                    break
-            if os.environ.get('DEBUG') and not tracer:
-                print(f'{lon = } {lat = }')
-                assert tracer
-        return
-
-    def _close_all(self):
-        for filepath, bounds in self.rasterfiles.items():
-            if 'raster' in bounds.keys():
-                bounds['raster'].img.close()
-
-    def merge_tracks(self, tracks):
-        ''' append `depth_metres` column to track dictionaries '''
-        for track in tracks:
-            # mapping of filepaths to the corresponding boundary region
-            raster_keys = np.array(list(self._check_in_bounds(track)),
-                                   dtype=object)
-
-            # ensure that each vector time slice has a value
-            if len(raster_keys) != len(track['time']):
-                raise ValueError('no rasters found for track')
-            bathy_segments = np.append(
-                np.append([0],
-                          np.where(raster_keys[:-1] != raster_keys[:1])[0]),
-                [len(raster_keys)],
-            )
-            track['depth_metres'] = reduce(np.append, [
-                self.rasterfiles[raster_keys[i]]
-                ['raster']._track_coordinate_values(
-                    track, rng=range(bathy_segments[i], bathy_segments[i + 1]))
-                for i in range(len(bathy_segments) - 1)
-            ]) * -1
-
-            track['dynamic'] = set(track['dynamic']).union(
-                set(['depth_metres']))
-            yield track
+''' load bathymetry data from GEBCO raster files '''
+
+import hashlib
+import os
+import zipfile
+from functools import reduce
+
+import numpy as np
+import requests
+import warnings
+from tqdm import tqdm
+
+from aisdb.gis import shiftcoord
+from aisdb.webdata.load_raster import RasterFile
+
+url = 'https://www.bodc.ac.uk/data/open_download/gebco/gebco_2022/geotiff/'
+
+
+def _filebounds(fpath):
+    return {
+        f[0]: float(f[1:])
+        for f in fpath.split('gebco_2022_', 1)[1].rsplit('.tif', 1)[0].split(
+            '_')
+    }
+
+
+class Gebco():
+
+    def __init__(self, data_dir):
+        '''
+            args:
+                data_dir (string)
+                    folder where rasters should be stored
+        '''
+        self.data_dir = data_dir
+        assert os.path.isdir(data_dir)
+        self.__enter__()
+
+    def __enter__(self):
+        self.rasterfiles = {
+            f: _filebounds(f)
+            for f in {
+                k: None
+                for k in sorted([
+                    f for f in os.listdir(self.data_dir)
+                    if f[-4:] == '.tif' and 'gebco_2022' in f
+                ])
+            }
+        }
+
+        # download bathymetry rasters if missing
+        self.fetch_bathymetry_grid()
+
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self._close_all()
+
+    def fetch_bathymetry_grid(self):  # pragma: no cover
+        """ download geotiff zip archive and extract it """
+
+        zipf = os.path.join(self.data_dir, "gebco_2022_geotiff.zip")
+        try:
+
+            # download the file if necessary
+            if not os.path.isfile(zipf):
+                print('downloading gebco bathymetry...')
+                with requests.get(url, stream=True) as payload:
+                    assert payload.status_code == 200, 'error fetching file'
+                    with open(zipf, 'wb') as f:
+                        with tqdm(total=4011413504,
+                                  desc=zipf,
+                                  unit='B',
+                                  unit_scale=True) as t:
+                            for chunk in payload.iter_content(chunk_size=8192):
+                                _ = t.update(f.write(chunk))
+
+                with open(zipf, 'rb') as z:
+                    sha256sum = hashlib.sha256(z.read()).hexdigest()
+                print('verifying checksum...')
+                assert sha256sum == '5ade15083909fcd6003409df678bdc6537b8691df996f8d806b48de962470cc3',\
+                        'checksum failed!'
+                with zipfile.ZipFile(zipf, 'r') as zip_ref:
+                    members = list(
+                        set(zip_ref.namelist()) -
+                        set(sorted(os.listdir(self.data_dir))))
+                    print('extracting bathymetry data...')
+                    zip_ref.extractall(path=self.data_dir, members=members)
+        except (Exception, KeyboardInterrupt) as err:
+            os.remove(os.path.join(self.data_dir, "gebco_2022_geotiff.zip"))
+            raise (err)
+        return
+
+    def _load_raster(self, key):
+        self.rasterfiles[key]['raster'] = RasterFile(
+            imgpath=os.path.join(self.data_dir, key))
+
+    def _check_in_bounds(self, track):
+        for lon, lat in zip(track['lon'], track['lat']):
+            if not (-180 <= lon <= 180) or not (-90 <= lat <=
+                                                90):  # pragma: no cover
+                warnings.warn('coordinates out of range!')
+                lon = shiftcoord([lon])[0]
+                lat = shiftcoord([lat], rng=90)[0]
+
+            if os.environ.get('DEBUG'):
+                tracer = False
+            for key, bounds in self.rasterfiles.items():
+                if (bounds['w'] <= lon <= bounds['e']
+                        and bounds['s'] <= lat <= bounds['n']):
+                    tracer = True
+                    if 'raster' not in bounds.keys():
+                        self._load_raster(key)
+                    yield key
+                    break
+            if os.environ.get('DEBUG') and not tracer:
+                print(f'{lon = } {lat = }')
+                assert tracer
+        return
+
+    def _close_all(self):
+        for filepath, bounds in self.rasterfiles.items():
+            if 'raster' in bounds.keys():
+                bounds['raster'].img.close()
+
+    def merge_tracks(self, tracks):
+        ''' append `depth_metres` column to track dictionaries '''
+        for track in tracks:
+            # mapping of filepaths to the corresponding boundary region
+            raster_keys = np.array(list(self._check_in_bounds(track)),
+                                   dtype=object)
+
+            # ensure that each vector time slice has a value
+            if len(raster_keys) != len(track['time']):
+                raise ValueError('no rasters found for track')
+            bathy_segments = np.append(
+                np.append([0],
+                          np.where(raster_keys[:-1] != raster_keys[:1])[0]),
+                [len(raster_keys)],
+            )
+            track['depth_metres'] = reduce(np.append, [
+                self.rasterfiles[raster_keys[i]]
+                ['raster']._track_coordinate_values(
+                    track, rng=range(bathy_segments[i], bathy_segments[i + 1]))
+                for i in range(len(bathy_segments) - 1)
+            ]) * -1
+
+            track['dynamic'] = set(track['dynamic']).union(
+                set(['depth_metres']))
+            yield track
```

## aisdb/webdata/load_raster.py

 * *Ordering differences only*

```diff
@@ -1,72 +1,72 @@
-import os
-
-import numpy as np
-from PIL import Image
-
-from aisdb.aisdb import binarysearch_vector
-
-Image.MAX_IMAGE_PIXELS = 650000000  # suppress DecompressionBombError warning
-
-
-class _RasterFile_generic():
-
-    def __enter__(self):
-        assert hasattr(self, 'img')
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        ''' close raster files upon exit from context '''
-        self.img.close()
-
-    def merge_tracks(self, tracks, new_track_key: str):
-        for track in tracks:
-            track['dynamic'] = set(track['dynamic']).union(set([new_track_key
-                                                                ]))
-            track[new_track_key] = self._track_coordinate_values(track)
-            yield track
-
-
-class RasterFile(_RasterFile_generic):
-
-    def _get_img_grids(self, im):
-        if 33922 in im.tag.tagdata.keys():
-            # GDAL tags
-            i, j, k, x, y, z = im.tag_v2[33922]  # ModelTiepointTag
-            dx, dy, dz = im.tag_v2[33550]  # ModelPixelScaleTag
-            lat = np.arange(y + dy, y + (dy * im.size[1]) + dy, dy)[::-1] - 90
-            if np.sum(lat > 91):
-                lat -= 90
-
-        elif 34264 in im.tag.tagdata.keys():  # pragma: no cover
-            # NASA JPL tags
-            dx, _, _, x, _, dy, _, y, _, _, dz, z, _, _, _, _ = im.tag_v2[
-                34264]  # ModelTransformationTag
-            lat = np.arange(y + dy, y + (dy * im.size[1]) + dy, dy)
-
-        else:
-            raise ValueError('error: unknown metadata tag encoding')
-
-        lon = np.arange(x + dx, x + (dx * im.size[0]) + dx, dx)
-
-        return lon, lat
-
-    def __init__(self, imgpath):
-        self.imgpath = imgpath
-        assert not hasattr(self, 'img')
-        assert os.path.isfile(
-            self.imgpath), f'raster file {self.imgpath} not found!'
-        self.img = Image.open(self.imgpath)
-        self.xy = self._get_img_grids(self.img)
-
-    def _get_coordinate_values(self, track, rng=None):
-        if rng is None:
-            rng = range(len(track['time']))
-        idx_lons = np.array(binarysearch_vector(self.xy[0], track['lon'][rng]))
-        idx_lats = np.array(binarysearch_vector(self.xy[1], track['lat'][rng]))
-        return np.array(list(map(
-            self.img.getpixel,
-            zip(idx_lons, idx_lats),
-        )))
-
-    def _track_coordinate_values(self, track, *, rng: range = None):
-        return self._get_coordinate_values(track, rng=rng)
+import os
+
+import numpy as np
+from PIL import Image
+
+from aisdb.aisdb import binarysearch_vector
+
+Image.MAX_IMAGE_PIXELS = 650000000  # suppress DecompressionBombError warning
+
+
+class _RasterFile_generic():
+
+    def __enter__(self):
+        assert hasattr(self, 'img')
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        ''' close raster files upon exit from context '''
+        self.img.close()
+
+    def merge_tracks(self, tracks, new_track_key: str):
+        for track in tracks:
+            track['dynamic'] = set(track['dynamic']).union(set([new_track_key
+                                                                ]))
+            track[new_track_key] = self._track_coordinate_values(track)
+            yield track
+
+
+class RasterFile(_RasterFile_generic):
+
+    def _get_img_grids(self, im):
+        if 33922 in im.tag.tagdata.keys():
+            # GDAL tags
+            i, j, k, x, y, z = im.tag_v2[33922]  # ModelTiepointTag
+            dx, dy, dz = im.tag_v2[33550]  # ModelPixelScaleTag
+            lat = np.arange(y + dy, y + (dy * im.size[1]) + dy, dy)[::-1] - 90
+            if np.sum(lat > 91):
+                lat -= 90
+
+        elif 34264 in im.tag.tagdata.keys():  # pragma: no cover
+            # NASA JPL tags
+            dx, _, _, x, _, dy, _, y, _, _, dz, z, _, _, _, _ = im.tag_v2[
+                34264]  # ModelTransformationTag
+            lat = np.arange(y + dy, y + (dy * im.size[1]) + dy, dy)
+
+        else:
+            raise ValueError('error: unknown metadata tag encoding')
+
+        lon = np.arange(x + dx, x + (dx * im.size[0]) + dx, dx)
+
+        return lon, lat
+
+    def __init__(self, imgpath):
+        self.imgpath = imgpath
+        assert not hasattr(self, 'img')
+        assert os.path.isfile(
+            self.imgpath), f'raster file {self.imgpath} not found!'
+        self.img = Image.open(self.imgpath)
+        self.xy = self._get_img_grids(self.img)
+
+    def _get_coordinate_values(self, track, rng=None):
+        if rng is None:
+            rng = range(len(track['time']))
+        idx_lons = np.array(binarysearch_vector(self.xy[0], track['lon'][rng]))
+        idx_lats = np.array(binarysearch_vector(self.xy[1], track['lat'][rng]))
+        return np.array(list(map(
+            self.img.getpixel,
+            zip(idx_lons, idx_lats),
+        )))
+
+    def _track_coordinate_values(self, track, *, rng: range = None):
+        return self._get_coordinate_values(track, rng=rng)
```

## aisdb/webdata/marinetraffic.py

 * *Ordering differences only*

```diff
@@ -1,324 +1,324 @@
-''' scrape vessel information such as deadweight tonnage from marinetraffic.com '''
-
-import os
-
-import numpy as np
-from selenium.webdriver.firefox.webdriver import WebDriver
-from selenium.webdriver.support.ui import WebDriverWait
-from selenium.webdriver.common.by import By
-from selenium.common.exceptions import TimeoutException
-
-from aisdb import sqlpath
-from aisdb.database.dbconn import ConnectionType
-from aisdb.webdata._scraper import _scraper
-import sqlite3
-
-baseurl = 'https://www.marinetraffic.com/'
-
-_err404 = 'INSERT INTO webdata_marinetraffic(mmsi, error404) '
-_err404 += 'VALUES (CAST(? as INT), 1)'
-
-_createtable_sqlfile = os.path.join(sqlpath,
-                                    'createtable_webdata_marinetraffic.sql')
-with open(_createtable_sqlfile, 'r') as f:
-    _createtable_sql = f.read()
-
-_insert_sqlfile = os.path.join(sqlpath, 'insert_webdata_marinetraffic.sql')
-with open(_insert_sqlfile, 'r') as f:
-    _insert_sql = f.read()
-
-
-def _nullinfo(track):
-    return {
-        'mmsi':
-        track['mmsi'],
-        'imo':
-        track['imo'] if 'imo' in track.keys() else 0,
-        'name': (track['vessel_name'] if 'vessel_name' in track.keys()
-                 and track['vessel_name'] is not None else ''),
-        'vesseltype_generic':
-        None,
-        'vesseltype_detailed':
-        None,
-        'callsign':
-        None,
-        'flag':
-        None,
-        'gross_tonnage':
-        None,
-        'summer_dwt':
-        None,
-        'length_breadth':
-        None,
-        'year_built':
-        None,
-        'home_port':
-        None,
-        'error404':
-        1
-    }
-
-
-def _loaded(drv: WebDriver) -> bool:  # pragma: no cover
-    asset_type = 'asset_type' in drv.current_url
-    e404 = '404' == drv.title[0:3]
-    exists = drv.find_elements(
-        by='id',
-        value='vesselDetails_voyageInfoSection',
-    )
-    return (exists or e404 or asset_type)
-
-
-def _updateinfo(info: str, vessel: dict) -> None:  # pragma: no cover
-    i = info.split(': ')
-    if len(i) < 2:
-        return
-    vessel[i[0]] = i[1]
-
-
-def _getrow(vessel: dict) -> tuple:  # pragma: no cover
-    if 'MMSI' not in vessel.keys() or vessel['MMSI'] == '-':
-        vessel['MMSI'] = 0
-    if 'IMO' not in vessel.keys() or vessel['IMO'] == '-':
-        vessel['IMO'] = 0
-    if 'Name' not in vessel.keys():
-        vessel['Name'] = ''
-    if 'Call Sign' not in vessel.keys():
-        vessel['Call Sign'] = ''
-    if 'Gross Tonnage' not in vessel.keys() or vessel['Gross Tonnage'] == '-':
-        vessel['Gross Tonnage'] = 0
-    elif ('Gross Tonnage' in vessel.keys()
-          and isinstance(vessel['Gross Tonnage'], str)):
-        vessel['Gross Tonnage'] = int(vessel['Gross Tonnage'].split()[0])
-    if 'Summer DWT' not in vessel.keys() or vessel['Summer DWT'] == '-':
-        vessel['Summer DWT'] = 0
-    elif ('Summer DWT' in vessel.keys()
-          and isinstance(vessel['Summer DWT'], str)):
-        vessel['Summer DWT'] = int(vessel['Summer DWT'].split()[0])
-    if 'Year Built' not in vessel.keys() or vessel['Year Built'] == '-':
-        vessel['Year Built'] = 0
-    return (
-        int(vessel['MMSI']),
-        int(vessel['IMO']),
-        vessel['Name'],
-        vessel['Vessel Type - Generic'],
-        vessel['Vessel Type - Detailed'],
-        vessel['Call Sign'],
-        vessel['Flag'],
-        int(vessel['Gross Tonnage']),
-        int(vessel['Summer DWT']),
-        vessel['Length Overall x Breadth Extreme'],
-        int(vessel['Year Built']),
-        vessel['Home Port'],
-    )
-
-
-def _insertvesselrow(elem, mmsi, trafficDB):  # pragma: no cover
-    vessel = {}
-    for info in elem.text.split('\n'):
-        _updateinfo(info, vessel)
-    if len(vessel.keys()) < 11:
-        return
-    insertrow = _getrow(vessel)
-
-    print(insertrow)
-
-    with trafficDB as conn:
-        conn.execute(_insert_sql, insertrow).fetchall()
-
-
-def _vessel_info_dict(dbconn) -> dict:
-    if isinstance(dbconn, ConnectionType.SQLITE.value):
-        # raise ValueError(f"Invalid database connection type: {dbconn}")
-        if not hasattr(dbconn, 'trafficdb'):
-            raise ValueError(
-                'Database connection does not have an attached traffic database!'
-            )
-        dbname = dbconn._get_dbname(dbconn.trafficdb)
-        cur = dbconn.cursor()
-        cur.execute(
-            f'SELECT * FROM {dbname}.sqlite_master '
-            'WHERE type="table" AND name LIKE "ais\\_%\\_dynamic" ESCAPE "\\" '
-        )
-        alias = dbconn._get_dbname(dbconn.trafficdb) + '.'
-    elif isinstance(dbconn, sqlite3.Connection):
-        alias = ''
-    elif isinstance(dbconn, ConnectionType.POSTGRES.value):
-        alias = ''
-    else:
-        raise ValueError(f"Invalid connection type: {dbconn}")
-    cur = dbconn.cursor()
-    res = cur.execute(
-        f'SELECT * FROM {alias}webdata_marinetraffic WHERE error404 != 1'
-    ).fetchall()
-    info_dict = {r['mmsi']: r for r in res}
-    return info_dict
-
-
-def vessel_info(tracks: iter, dbconn: sqlite3.Connection):
-    ''' append metadata scraped from marinetraffic.com to track dictionaries.
-
-        See :meth:`aisdb.database.dbqry.DBQuery.check_marinetraffic` for a
-        high-level method to retrieve metadata for all vessels observed within
-        a specific query time and region, or alternatively see
-        :meth:`aisdb.webdata.marinetraffic.VesselInfo.vessel_info_callback`
-        for scraping metadata for a given list of MMSIs
-
-        args:
-            tracks (iter)
-                collection of track dictionaries
-            dbconn (ConnectionType)
-                Either a :class:`aisdb.database.dbconn.SQLiteDBConn` or
-                :class:`aisdb.database.dbconn.PostgresDBConn` database
-                connection objects
-    '''
-    if not isinstance(dbconn, sqlite3.Connection):
-        raise ValueError(
-            f"Invalid database connection type: {dbconn}. Requires: {sqlite3.Connection}"
-        )
-    meta = _vessel_info_dict(dbconn)
-    for track in tracks:
-        assert isinstance(track, dict)
-        track['static'] = set(track['static']).union({'marinetraffic_info'})
-        if track['mmsi'] in meta.keys():
-            track['marinetraffic_info'] = meta[track['mmsi']]
-        else:
-            track['marinetraffic_info'] = _nullinfo(track)
-        yield track
-
-
-class VesselInfo():  # pragma: no cover
-    ''' scrape vessel metadata from marinetraffic.com
-
-        args:
-            trafficDBpath (string)
-                path where vessel traffic metadata should be stored
-
-        See :meth:`aisdb.database.dbqry.DBQuery.check_marinetraffic` for a
-        high-level method to retrieve metadata for all vessels observed within
-        a specific query time and region, or alternatively see
-        :meth:`aisdb.webdata.marinetraffic.VesselInfo.vessel_info_callback`
-        for scraping metadata for a given list of MMSIs
-    '''
-
-    def __init__(self, trafficDBpath, verbose=False):
-        self.driver = None
-        wd = os.path.dirname(trafficDBpath)
-        if not os.path.isdir(wd):  # pragma: no cover
-            if verbose: print(f'creating directory: {wd}')
-            os.makedirs(wd)
-        self.trafficDB = sqlite3.Connection(trafficDBpath)
-        self.trafficDB.row_factory = sqlite3.Row
-
-        # create a new info table if it doesnt exist yet
-        with self.trafficDB as conn:
-            conn.execute(_createtable_sql)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_value, tb):
-        if self.driver is not None:
-            self.driver.close()
-            self.driver.quit()
-
-    def _getinfo(self, *, url, searchmmsi, infotxt=''):
-        if self.driver is None:
-            self.driver = _scraper()
-
-        print(infotxt + url, end='\t')
-        try:
-            self.driver.get(url)
-            WebDriverWait(self.driver, 15).until(_loaded)
-        except TimeoutException:
-            print(f'timed out, skipping {searchmmsi=}')
-
-            # if timeout occurs, mark as error 404
-            with self.trafficDB as conn:
-                conn.execute(_err404, (str(searchmmsi), ))
-            return
-        except Exception as err:
-            self.driver.close()
-            self.driver.quit()
-            raise err
-
-        # recurse through vessel listings if multiple vessels appear
-        if 'asset_type' in self.driver.current_url:
-            print('recursing...')
-
-            urls = []
-            for elem in self.driver.find_elements(
-                    By.CLASS_NAME,
-                    value='ag-cell-content-link',
-            ):
-                urls.append(elem.get_attribute('href'))
-
-            for url in urls:
-                self._getinfo(url=url, searchmmsi=searchmmsi)
-
-            with self.trafficDB as conn:
-                insert404 = conn.execute(
-                    'SELECT COUNT(*) FROM webdata_marinetraffic WHERE mmsi=?',
-                    (str(searchmmsi), )).fetchone()[0] == 0
-                if insert404:
-                    conn.execute(_err404, (str(searchmmsi), ))
-
-        elif 'hc-en' in self.driver.current_url:
-            raise RuntimeError('bad url??')
-
-        elif self.driver.title[0:3] == '404':
-            print(f'404 error! {searchmmsi=}')
-            with self.trafficDB as conn:
-                conn.execute(_err404, (str(searchmmsi), ))
-
-        value = 'vesselDetails_vesselInfoSection'
-        for elem in self.driver.find_elements(value=value):
-            _ = _insertvesselrow(elem, searchmmsi, self.trafficDB)
-
-    def vessel_info_callback(self, mmsis, retry_404=False, infotxt=''):
-        ''' search for metadata for given mmsis
-
-            args:
-                mmsis (list)
-                    list of MMSI identifiers (integers)
-        '''
-        # only check unique mmsis
-        mmsis = np.unique(mmsis).astype(int)
-        print('.', end='')  # second dot (first in dbqry.py)
-
-        # check existing
-        sqlcount = 'SELECT mmsi FROM webdata_marinetraffic \t'
-        sqlcount += f'WHERE mmsi IN ({",".join(["?" for _ in mmsis])})\n'
-        if retry_404:
-            sqlcount += 'AND error404 != 1 \n'
-        sqlcount += 'ORDER BY mmsi'
-        with self.trafficDB as conn:
-            existing = conn.execute(sqlcount, tuple(map(str,
-                                                        mmsis))).fetchall()
-        print('.')  # third dot
-
-        # skip existing mmsis
-        ex_mmsis = np.array(existing).flatten()
-        xor_mmsis = np.setdiff1d(mmsis, ex_mmsis, assume_unique=True)
-        if xor_mmsis.size == 0:
-            return
-
-        for mmsi in xor_mmsis:
-            if not 200000000 <= mmsi <= 780000000:
-                continue
-            url = f'{baseurl}en/ais/details/ships/mmsi:{mmsi}'
-            self._getinfo(url=url, searchmmsi=mmsi, infotxt=infotxt)
-
-        return
-
-
-'''
-# validate IMO
-if searchimo != 0:
-    checksum = str(
-            np.sum(
-                np.array(list(map(int, list(str(searchimo)[:-1])))) *
-                np.array([7, 6, 5, 4, 3, 2])))[-1]
-else:
-    checksum = '0'
-'''
+''' scrape vessel information such as deadweight tonnage from marinetraffic.com '''
+
+import os
+
+import numpy as np
+from selenium.webdriver.firefox.webdriver import WebDriver
+from selenium.webdriver.support.ui import WebDriverWait
+from selenium.webdriver.common.by import By
+from selenium.common.exceptions import TimeoutException
+
+from aisdb import sqlpath
+from aisdb.database.dbconn import ConnectionType
+from aisdb.webdata._scraper import _scraper
+import sqlite3
+
+baseurl = 'https://www.marinetraffic.com/'
+
+_err404 = 'INSERT INTO webdata_marinetraffic(mmsi, error404) '
+_err404 += 'VALUES (CAST(? as INT), 1)'
+
+_createtable_sqlfile = os.path.join(sqlpath,
+                                    'createtable_webdata_marinetraffic.sql')
+with open(_createtable_sqlfile, 'r') as f:
+    _createtable_sql = f.read()
+
+_insert_sqlfile = os.path.join(sqlpath, 'insert_webdata_marinetraffic.sql')
+with open(_insert_sqlfile, 'r') as f:
+    _insert_sql = f.read()
+
+
+def _nullinfo(track):
+    return {
+        'mmsi':
+        track['mmsi'],
+        'imo':
+        track['imo'] if 'imo' in track.keys() else 0,
+        'name': (track['vessel_name'] if 'vessel_name' in track.keys()
+                 and track['vessel_name'] is not None else ''),
+        'vesseltype_generic':
+        None,
+        'vesseltype_detailed':
+        None,
+        'callsign':
+        None,
+        'flag':
+        None,
+        'gross_tonnage':
+        None,
+        'summer_dwt':
+        None,
+        'length_breadth':
+        None,
+        'year_built':
+        None,
+        'home_port':
+        None,
+        'error404':
+        1
+    }
+
+
+def _loaded(drv: WebDriver) -> bool:  # pragma: no cover
+    asset_type = 'asset_type' in drv.current_url
+    e404 = '404' == drv.title[0:3]
+    exists = drv.find_elements(
+        by='id',
+        value='vesselDetails_voyageInfoSection',
+    )
+    return (exists or e404 or asset_type)
+
+
+def _updateinfo(info: str, vessel: dict) -> None:  # pragma: no cover
+    i = info.split(': ')
+    if len(i) < 2:
+        return
+    vessel[i[0]] = i[1]
+
+
+def _getrow(vessel: dict) -> tuple:  # pragma: no cover
+    if 'MMSI' not in vessel.keys() or vessel['MMSI'] == '-':
+        vessel['MMSI'] = 0
+    if 'IMO' not in vessel.keys() or vessel['IMO'] == '-':
+        vessel['IMO'] = 0
+    if 'Name' not in vessel.keys():
+        vessel['Name'] = ''
+    if 'Call Sign' not in vessel.keys():
+        vessel['Call Sign'] = ''
+    if 'Gross Tonnage' not in vessel.keys() or vessel['Gross Tonnage'] == '-':
+        vessel['Gross Tonnage'] = 0
+    elif ('Gross Tonnage' in vessel.keys()
+          and isinstance(vessel['Gross Tonnage'], str)):
+        vessel['Gross Tonnage'] = int(vessel['Gross Tonnage'].split()[0])
+    if 'Summer DWT' not in vessel.keys() or vessel['Summer DWT'] == '-':
+        vessel['Summer DWT'] = 0
+    elif ('Summer DWT' in vessel.keys()
+          and isinstance(vessel['Summer DWT'], str)):
+        vessel['Summer DWT'] = int(vessel['Summer DWT'].split()[0])
+    if 'Year Built' not in vessel.keys() or vessel['Year Built'] == '-':
+        vessel['Year Built'] = 0
+    return (
+        int(vessel['MMSI']),
+        int(vessel['IMO']),
+        vessel['Name'],
+        vessel['Vessel Type - Generic'],
+        vessel['Vessel Type - Detailed'],
+        vessel['Call Sign'],
+        vessel['Flag'],
+        int(vessel['Gross Tonnage']),
+        int(vessel['Summer DWT']),
+        vessel['Length Overall x Breadth Extreme'],
+        int(vessel['Year Built']),
+        vessel['Home Port'],
+    )
+
+
+def _insertvesselrow(elem, mmsi, trafficDB):  # pragma: no cover
+    vessel = {}
+    for info in elem.text.split('\n'):
+        _updateinfo(info, vessel)
+    if len(vessel.keys()) < 11:
+        return
+    insertrow = _getrow(vessel)
+
+    print(insertrow)
+
+    with trafficDB as conn:
+        conn.execute(_insert_sql, insertrow).fetchall()
+
+
+def _vessel_info_dict(dbconn) -> dict:
+    if isinstance(dbconn, ConnectionType.SQLITE.value):
+        # raise ValueError(f"Invalid database connection type: {dbconn}")
+        if not hasattr(dbconn, 'trafficdb'):
+            raise ValueError(
+                'Database connection does not have an attached traffic database!'
+            )
+        dbname = dbconn._get_dbname(dbconn.trafficdb)
+        cur = dbconn.cursor()
+        cur.execute(
+            f'SELECT * FROM {dbname}.sqlite_master '
+            'WHERE type="table" AND name LIKE "ais\\_%\\_dynamic" ESCAPE "\\" '
+        )
+        alias = dbconn._get_dbname(dbconn.trafficdb) + '.'
+    elif isinstance(dbconn, sqlite3.Connection):
+        alias = ''
+    elif isinstance(dbconn, ConnectionType.POSTGRES.value):
+        alias = ''
+    else:
+        raise ValueError(f"Invalid connection type: {dbconn}")
+    cur = dbconn.cursor()
+    res = cur.execute(
+        f'SELECT * FROM {alias}webdata_marinetraffic WHERE error404 != 1'
+    ).fetchall()
+    info_dict = {r['mmsi']: r for r in res}
+    return info_dict
+
+
+def vessel_info(tracks: iter, dbconn: sqlite3.Connection):
+    ''' append metadata scraped from marinetraffic.com to track dictionaries.
+
+        See :meth:`aisdb.database.dbqry.DBQuery.check_marinetraffic` for a
+        high-level method to retrieve metadata for all vessels observed within
+        a specific query time and region, or alternatively see
+        :meth:`aisdb.webdata.marinetraffic.VesselInfo.vessel_info_callback`
+        for scraping metadata for a given list of MMSIs
+
+        args:
+            tracks (iter)
+                collection of track dictionaries
+            dbconn (ConnectionType)
+                Either a :class:`aisdb.database.dbconn.SQLiteDBConn` or
+                :class:`aisdb.database.dbconn.PostgresDBConn` database
+                connection objects
+    '''
+    if not isinstance(dbconn, sqlite3.Connection):
+        raise ValueError(
+            f"Invalid database connection type: {dbconn}. Requires: {sqlite3.Connection}"
+        )
+    meta = _vessel_info_dict(dbconn)
+    for track in tracks:
+        assert isinstance(track, dict)
+        track['static'] = set(track['static']).union({'marinetraffic_info'})
+        if track['mmsi'] in meta.keys():
+            track['marinetraffic_info'] = meta[track['mmsi']]
+        else:
+            track['marinetraffic_info'] = _nullinfo(track)
+        yield track
+
+
+class VesselInfo():  # pragma: no cover
+    ''' scrape vessel metadata from marinetraffic.com
+
+        args:
+            trafficDBpath (string)
+                path where vessel traffic metadata should be stored
+
+        See :meth:`aisdb.database.dbqry.DBQuery.check_marinetraffic` for a
+        high-level method to retrieve metadata for all vessels observed within
+        a specific query time and region, or alternatively see
+        :meth:`aisdb.webdata.marinetraffic.VesselInfo.vessel_info_callback`
+        for scraping metadata for a given list of MMSIs
+    '''
+
+    def __init__(self, trafficDBpath, verbose=False):
+        self.driver = None
+        wd = os.path.dirname(trafficDBpath)
+        if not os.path.isdir(wd):  # pragma: no cover
+            if verbose: print(f'creating directory: {wd}')
+            os.makedirs(wd)
+        self.trafficDB = sqlite3.Connection(trafficDBpath)
+        self.trafficDB.row_factory = sqlite3.Row
+
+        # create a new info table if it doesnt exist yet
+        with self.trafficDB as conn:
+            conn.execute(_createtable_sql)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, tb):
+        if self.driver is not None:
+            self.driver.close()
+            self.driver.quit()
+
+    def _getinfo(self, *, url, searchmmsi, infotxt=''):
+        if self.driver is None:
+            self.driver = _scraper()
+
+        print(infotxt + url, end='\t')
+        try:
+            self.driver.get(url)
+            WebDriverWait(self.driver, 15).until(_loaded)
+        except TimeoutException:
+            print(f'timed out, skipping {searchmmsi=}')
+
+            # if timeout occurs, mark as error 404
+            with self.trafficDB as conn:
+                conn.execute(_err404, (str(searchmmsi), ))
+            return
+        except Exception as err:
+            self.driver.close()
+            self.driver.quit()
+            raise err
+
+        # recurse through vessel listings if multiple vessels appear
+        if 'asset_type' in self.driver.current_url:
+            print('recursing...')
+
+            urls = []
+            for elem in self.driver.find_elements(
+                    By.CLASS_NAME,
+                    value='ag-cell-content-link',
+            ):
+                urls.append(elem.get_attribute('href'))
+
+            for url in urls:
+                self._getinfo(url=url, searchmmsi=searchmmsi)
+
+            with self.trafficDB as conn:
+                insert404 = conn.execute(
+                    'SELECT COUNT(*) FROM webdata_marinetraffic WHERE mmsi=?',
+                    (str(searchmmsi), )).fetchone()[0] == 0
+                if insert404:
+                    conn.execute(_err404, (str(searchmmsi), ))
+
+        elif 'hc-en' in self.driver.current_url:
+            raise RuntimeError('bad url??')
+
+        elif self.driver.title[0:3] == '404':
+            print(f'404 error! {searchmmsi=}')
+            with self.trafficDB as conn:
+                conn.execute(_err404, (str(searchmmsi), ))
+
+        value = 'vesselDetails_vesselInfoSection'
+        for elem in self.driver.find_elements(value=value):
+            _ = _insertvesselrow(elem, searchmmsi, self.trafficDB)
+
+    def vessel_info_callback(self, mmsis, retry_404=False, infotxt=''):
+        ''' search for metadata for given mmsis
+
+            args:
+                mmsis (list)
+                    list of MMSI identifiers (integers)
+        '''
+        # only check unique mmsis
+        mmsis = np.unique(mmsis).astype(int)
+        print('.', end='')  # second dot (first in dbqry.py)
+
+        # check existing
+        sqlcount = 'SELECT mmsi FROM webdata_marinetraffic \t'
+        sqlcount += f'WHERE mmsi IN ({",".join(["?" for _ in mmsis])})\n'
+        if retry_404:
+            sqlcount += 'AND error404 != 1 \n'
+        sqlcount += 'ORDER BY mmsi'
+        with self.trafficDB as conn:
+            existing = conn.execute(sqlcount, tuple(map(str,
+                                                        mmsis))).fetchall()
+        print('.')  # third dot
+
+        # skip existing mmsis
+        ex_mmsis = np.array(existing).flatten()
+        xor_mmsis = np.setdiff1d(mmsis, ex_mmsis, assume_unique=True)
+        if xor_mmsis.size == 0:
+            return
+
+        for mmsi in xor_mmsis:
+            if not 200000000 <= mmsi <= 780000000:
+                continue
+            url = f'{baseurl}en/ais/details/ships/mmsi:{mmsi}'
+            self._getinfo(url=url, searchmmsi=mmsi, infotxt=infotxt)
+
+        return
+
+
+'''
+# validate IMO
+if searchimo != 0:
+    checksum = str(
+            np.sum(
+                np.array(list(map(int, list(str(searchimo)[:-1])))) *
+                np.array([7, 6, 5, 4, 3, 2])))[-1]
+else:
+    checksum = '0'
+'''
```

## aisdb/webdata/shore_dist.py

 * *Ordering differences only*

```diff
@@ -1,68 +1,68 @@
-''' Collect shore/port distances at given coordinates using NASA and Global
-    Fishing Watch raster files.
-    A (free) login is required to download Global Fishing Watch rasters,
-    so these files must be manually downloaded and extracted into ``data_dir``.
-
-    Raster data can be downloaded from:
-
-    .. code-block::
-
-        https://oceancolor.gsfc.nasa.gov/docs/distfromcoast/GMT_intermediate_coast_distance_01d.zip
-        https://globalfishingwatch.org/data-download/datasets/public-distance-from-shore-v1
-        https://globalfishingwatch.org/data-download/datasets/public-distance-from-port-v1
-
-    once downloaded, place the unzipped geotiff files in `data_dir`
-'''
-
-import os
-import zipfile
-
-import requests
-from tqdm import tqdm
-
-from aisdb.webdata.load_raster import RasterFile
-
-def download_unzip(data_url, data_dir, bytesize=0):
-    assert os.path.isdir(data_dir), f'not a directory: {data_dir=}'
-    zipf = os.path.join(data_dir, data_url.rsplit('/',1)[1])
-    if not os.path.isfile(zipf):
-        try:
-            with requests.get(data_url, stream=True) as payload:
-                assert payload.status_code == 200, 'error fetching file'
-                with open(zipf, 'wb') as f:
-                    with tqdm(total=bytesize,
-                              desc=zipf,
-                              unit='B',
-                              unit_scale=True) as t:
-                        for chunk in payload.iter_content(chunk_size=8192):
-                            _ = t.update(f.write(chunk))
-        except Exception as err:
-            os.remove(zipf)
-            raise err
-    with zipfile.ZipFile(zipf, 'r') as zip_ref:
-        members = list( fpath for fpath in
-                       set(zip_ref.namelist()) -
-                       set(sorted(os.listdir(data_dir))) if '.tif' in fpath)
-        if len(members) > 0:
-            zip_ref.extractall(path=data_dir, members=members)
-
-class ShoreDist(RasterFile):
-
-    data_url = "https://oceancolor.gsfc.nasa.gov/docs/distfromcoast/GMT_intermediate_coast_distance_01d.zip"
-
-    def __init__(self, data_dir, tif_filename='GMT_intermediate_coast_distance_01d.tif'):
-        download_unzip(self.data_url, data_dir, bytesize=657280)
-        imgpath = os.path.join(data_dir, tif_filename)
-        #imgpath = os.path.join(data_dir, 'distance-from-shore.tif')
-        assert os.path.isfile(imgpath)
-        super().__init__(imgpath)
-
-    def get_distance(self, tracks):
-        assert hasattr(self, 'imgpath')
-        return self.merge_tracks(tracks, new_track_key='km_from_shore')
-
-
-class PortDist(RasterFile):
-
-    def get_distance(self, tracks):
-        return self.merge_tracks(tracks, new_track_key='km_from_port')
+''' Collect shore/port distances at given coordinates using NASA and Global
+    Fishing Watch raster files.
+    A (free) login is required to download Global Fishing Watch rasters,
+    so these files must be manually downloaded and extracted into ``data_dir``.
+
+    Raster data can be downloaded from:
+
+    .. code-block::
+
+        https://oceancolor.gsfc.nasa.gov/docs/distfromcoast/GMT_intermediate_coast_distance_01d.zip
+        https://globalfishingwatch.org/data-download/datasets/public-distance-from-shore-v1
+        https://globalfishingwatch.org/data-download/datasets/public-distance-from-port-v1
+
+    once downloaded, place the unzipped geotiff files in `data_dir`
+'''
+
+import os
+import zipfile
+
+import requests
+from tqdm import tqdm
+
+from aisdb.webdata.load_raster import RasterFile
+
+def download_unzip(data_url, data_dir, bytesize=0):
+    assert os.path.isdir(data_dir), f'not a directory: {data_dir=}'
+    zipf = os.path.join(data_dir, data_url.rsplit('/',1)[1])
+    if not os.path.isfile(zipf):
+        try:
+            with requests.get(data_url, stream=True) as payload:
+                assert payload.status_code == 200, 'error fetching file'
+                with open(zipf, 'wb') as f:
+                    with tqdm(total=bytesize,
+                              desc=zipf,
+                              unit='B',
+                              unit_scale=True) as t:
+                        for chunk in payload.iter_content(chunk_size=8192):
+                            _ = t.update(f.write(chunk))
+        except Exception as err:
+            os.remove(zipf)
+            raise err
+    with zipfile.ZipFile(zipf, 'r') as zip_ref:
+        members = list( fpath for fpath in
+                       set(zip_ref.namelist()) -
+                       set(sorted(os.listdir(data_dir))) if '.tif' in fpath)
+        if len(members) > 0:
+            zip_ref.extractall(path=data_dir, members=members)
+
+class ShoreDist(RasterFile):
+
+    data_url = "https://oceancolor.gsfc.nasa.gov/docs/distfromcoast/GMT_intermediate_coast_distance_01d.zip"
+
+    def __init__(self, data_dir, tif_filename='GMT_intermediate_coast_distance_01d.tif'):
+        download_unzip(self.data_url, data_dir, bytesize=657280)
+        imgpath = os.path.join(data_dir, tif_filename)
+        #imgpath = os.path.join(data_dir, 'distance-from-shore.tif')
+        assert os.path.isfile(imgpath)
+        super().__init__(imgpath)
+
+    def get_distance(self, tracks):
+        assert hasattr(self, 'imgpath')
+        return self.merge_tracks(tracks, new_track_key='km_from_shore')
+
+
+class PortDist(RasterFile):
+
+    def get_distance(self, tracks):
+        return self.merge_tracks(tracks, new_track_key='km_from_port')
```

## aisdb/webdata/_scraper.py

 * *Ordering differences only*

```diff
@@ -1,60 +1,60 @@
-''' webscraper using selenium, firefox, and mozilla geckodriver '''
-
-import os
-import shutil
-
-
-def _scraper():
-    ''' selenium web scraper ``selenium.webdriver``
-
-        to open a browser window while debugging, export DEBUG=1
-    '''
-    from selenium import webdriver
-    from selenium.webdriver.firefox.options import Options
-    from selenium.webdriver.firefox.service import Service
-    from webdriver_manager.firefox import GeckoDriverManager
-    # from selenium.webdriver.chrome.options import Options
-    # from selenium.webdriver.chrome.service import Service
-    # from webdriver_manager.chrome import ChromeDriverManager
-    # assert shutil.which('firefox') is not None, f'Firefox is required for this feature. {shutil.which("firefox")=}'
-
-    # configs
-    opt = Options()
-    opt.headless = True if not os.environ.get('DEBUG') else False
-    opt.set_preference('permissions.default.image', 2)
-    opt.set_preference('extensions.contentblocker.enabled', True)
-    opt.set_preference('media.autoplay.default', 2)
-    opt.set_preference('media.autoplay.allow-muted', False)
-    opt.set_preference('media.autoplay.block-event.enabled', True)
-    opt.set_preference('media.autoplay.block-webaudio', True)
-    opt.set_preference('services.sync.prefs.sync.media.autoplay.default',
-                       False)
-    opt.set_preference('ui.context_menus.after_mouseup', False)
-    opt.set_preference('privacy.sanitize.sanitizeOnShutdown', True)
-    opt.set_preference('dom.disable_beforeunload', True)
-    """ chrome args
-    opt.add_argument('--headless')
-    opt.add_argument(f'user-data-dir={data_dir}')
-    opt.add_argument('permissions.default.image=2')
-    opt.add_argument('extensions.contentblocker.enabled=True')
-    opt.add_argument('media.autoplay.default=2')
-    opt.add_argument('media.autoplay.allow-muted=False')
-    opt.add_argument('media.autoplay.block-event.enabled=True')
-    opt.add_argument('media.autoplay.block-webaudio=True')
-    opt.add_argument(
-        'services.sync.prefs.sync.media.autoplay.default=False')
-    opt.add_argument('ui.context_menus.after_mouseup=False')
-    opt.add_argument('privacy.sanitize.sanitizeOnShutdown=True')
-    opt.add_argument('dom.disable_beforeunload=True')
-    """
-
-    driver = webdriver.Firefox(
-            service=Service(executable_path=GeckoDriverManager().install()),
-            options=opt)
-
-    if os.environ.get('DEBUG'):
-        driver.maximize_window()
-    else:
-        driver.set_window_size(9999, 9999)
-
-    return driver
+''' webscraper using selenium, firefox, and mozilla geckodriver '''
+
+import os
+import shutil
+
+
+def _scraper():
+    ''' selenium web scraper ``selenium.webdriver``
+
+        to open a browser window while debugging, export DEBUG=1
+    '''
+    from selenium import webdriver
+    from selenium.webdriver.firefox.options import Options
+    from selenium.webdriver.firefox.service import Service
+    from webdriver_manager.firefox import GeckoDriverManager
+    # from selenium.webdriver.chrome.options import Options
+    # from selenium.webdriver.chrome.service import Service
+    # from webdriver_manager.chrome import ChromeDriverManager
+    # assert shutil.which('firefox') is not None, f'Firefox is required for this feature. {shutil.which("firefox")=}'
+
+    # configs
+    opt = Options()
+    opt.headless = True if not os.environ.get('DEBUG') else False
+    opt.set_preference('permissions.default.image', 2)
+    opt.set_preference('extensions.contentblocker.enabled', True)
+    opt.set_preference('media.autoplay.default', 2)
+    opt.set_preference('media.autoplay.allow-muted', False)
+    opt.set_preference('media.autoplay.block-event.enabled', True)
+    opt.set_preference('media.autoplay.block-webaudio', True)
+    opt.set_preference('services.sync.prefs.sync.media.autoplay.default',
+                       False)
+    opt.set_preference('ui.context_menus.after_mouseup', False)
+    opt.set_preference('privacy.sanitize.sanitizeOnShutdown', True)
+    opt.set_preference('dom.disable_beforeunload', True)
+    """ chrome args
+    opt.add_argument('--headless')
+    opt.add_argument(f'user-data-dir={data_dir}')
+    opt.add_argument('permissions.default.image=2')
+    opt.add_argument('extensions.contentblocker.enabled=True')
+    opt.add_argument('media.autoplay.default=2')
+    opt.add_argument('media.autoplay.allow-muted=False')
+    opt.add_argument('media.autoplay.block-event.enabled=True')
+    opt.add_argument('media.autoplay.block-webaudio=True')
+    opt.add_argument(
+        'services.sync.prefs.sync.media.autoplay.default=False')
+    opt.add_argument('ui.context_menus.after_mouseup=False')
+    opt.add_argument('privacy.sanitize.sanitizeOnShutdown=True')
+    opt.add_argument('dom.disable_beforeunload=True')
+    """
+
+    driver = webdriver.Firefox(
+            service=Service(executable_path=GeckoDriverManager().install()),
+            options=opt)
+
+    if os.environ.get('DEBUG'):
+        driver.maximize_window()
+    else:
+        driver.set_window_size(9999, 9999)
+
+    return driver
```

## aisdb/web_interface.py

 * *Ordering differences only*

```diff
@@ -1,206 +1,206 @@
-import asyncio
-import http.server
-import logging
-import multiprocessing
-import os
-import socketserver
-import webbrowser
-from datetime import datetime
-from functools import partial
-from tempfile import SpooledTemporaryFile
-
-import orjson
-import websockets.server
-
-logging.getLogger("websockets").setLevel(logging.WARNING)
-logging.getLogger("shapely").setLevel(logging.WARNING)
-
-wwwpath = os.path.abspath(
-    os.path.join(os.path.dirname(os.path.dirname(__file__)), 'aisdb_web',
-                 'dist_map'))
-
-wwwpath_visualearth = os.path.abspath(
-    os.path.join(os.path.dirname(os.path.dirname(__file__)), 'aisdb_web',
-                 'dist_map_bingmaps'))
-
-
-def _start_webclient(visualearth=False):
-    if not visualearth:
-        path = wwwpath
-    else:
-        path = wwwpath_visualearth
-
-    class AISDB_HTML(http.server.SimpleHTTPRequestHandler):
-
-        extensions_map = {
-            '': 'application/octet-stream',
-            '.css': 'text/css',
-            '.html': 'text/html',
-            '.jpg': 'image/jpg',
-            '.js': 'application/x-javascript',
-            '.json': 'application/json',
-            '.png': 'image/png',
-            '.wasm': 'application/wasm',
-        }
-
-        def __init__(self, *args, **kwargs):
-            super().__init__(*args, directory=path, **kwargs)
-
-    socketserver.TCPServer.allow_reuse_address = True
-    with socketserver.TCPServer(("localhost", 3000), AISDB_HTML) as httpd:
-        try:
-            print('Serving HTTP assets on localhost:3000')
-            httpd.serve_forever()
-        except KeyboardInterrupt:
-            httpd.server_close()
-            httpd.shutdown()
-        except Exception as e:
-            httpd.server_close()
-            httpd.shutdown()
-            raise e
-
-
-def serialize_zone_json(name, zone):
-    zone_dict = {
-        'msgtype': 'zone',
-        'meta': {
-            'name': name
-        },
-        'x': tuple(zone['geometry'].boundary.xy[0]),
-        'y': tuple(zone['geometry'].boundary.xy[1]),
-        't': [],
-    }
-    return orjson.dumps(zone_dict)
-
-
-def serialize_track_json(track) -> bytes:
-    ''' serializes a single track dictionary to JSON format encoded as UTF8 '''
-    vector = {
-        'msgtype': 'track_vector',
-        # currently, database_server sends all metadata as strings
-        # reproduce this behaviour by coercion to string type, even for int
-        'meta': {
-            'mmsi': str(track['mmsi'])
-        },
-        't': track['time'],
-        'x': track['lon'],
-        'y': track['lat'],
-    }
-
-    meta = {k: track[k] for k in track['static'] if k != 'marinetraffic_info'}
-    meta['msgtype'] = 'vesselinfo'
-
-    if 'marinetraffic_info' in track.keys():
-        meta.update({
-            k: track['marinetraffic_info'][k]
-            for k in track['marinetraffic_info'].keys()
-        })
-
-    vector_json = orjson.dumps(vector, option=orjson.OPT_SERIALIZE_NUMPY)
-    meta_json = orjson.dumps(meta)
-    return (vector_json, meta_json)
-
-
-async def _send_tracks(websocket, tmp_vectors, tmp_meta, domain=None):
-    ''' send tracks serialized as JSON to the connected websocket client '''
-    done = {}
-    async for message_json in websocket:
-        message = orjson.loads(message_json)
-        print(
-            f'{websocket.remote_address[0]}:{websocket.remote_address[1]} - received: {message}'
-        )
-
-        if message == {"msgtype": "validrange"}:
-            now = datetime.now().timestamp()
-            validrange = {"msgtype": "validrange", "start": now, "end": now}
-            await websocket.send(orjson.dumps(validrange))
-            done['validrange'] = True
-
-        elif message == {"msgtype": "zones"}:
-            await websocket.send(b'{"msgtype": "doneZones"}')
-            done['zones'] = True
-        elif message == {"msgtype": "meta"}:
-            done['meta'] = True
-        else:
-            raise RuntimeError(f'unknown request {message_json}')
-
-        if 'validrange' in done.keys() and 'zones' in done.keys():
-            assert len(done.keys()) == 2
-
-            if domain is not None:
-                for name, zone in domain.zones.items():
-                    zone_json = serialize_zone_json(name, zone)
-                    await websocket.send(zone_json)
-
-            tmp_vectors.seek(0)
-            for vector_json in tmp_vectors:
-                await websocket.send(vector_json)
-
-        elif 'meta' in done.keys():
-            assert len(done.keys()) == 1
-            tmp_meta.seek(0)
-            for meta_json in tmp_meta:
-                await websocket.send(meta_json)
-
-
-async def _start_webserver(tracks,
-                           domain=None,
-                           visualearth=False,
-                           open_browser=True):
-    ''' Display tracks in the web interface. Serves data to the web client '''
-    print('Querying database...', end='\t')
-    with SpooledTemporaryFile(max_size=1024 * 1e6, newline=b'\n') as vectors, \
-            SpooledTemporaryFile(max_size=256 * 1e6, newline=b'\n') as meta:
-        for vector, info in map(serialize_track_json, tracks):
-            vectors.write(vector)
-            vectors.write(b'\n')
-            meta.write(info)
-            meta.write(b'\n')
-
-        print('done query')
-
-        if open_browser:
-            print('Opening a new browser window to display track data. '
-                  'Press Ctrl-C to stop the server and close the webpage')
-            tag = 1 if not visualearth else 2
-            url = f'http://localhost:3000/index.html?python={tag}&z=2'
-            if not webbrowser.open_new_tab(url):
-                print(f'Failed to open webbrowser, instead use URL: {url}')
-
-        fcn = partial(_send_tracks,
-                      tmp_vectors=vectors,
-                      tmp_meta=meta,
-                      domain=domain)
-        async with websockets.server.serve(fcn, 'localhost', 9924) as server:
-            stop = asyncio.Future()
-            await stop
-            await server
-
-
-def visualize(tracks, domain=None, visualearth=False, open_browser=True):
-    ''' Display tracks using the web interface.
-
-        Starts the web client HTTP server in a separate process, and
-        serves track data via websocket on port 9924.
-
-        If a domain object is given, zone polygons will be drawn on the map
-        from domain zone geometries.
-
-        If visualearth is True, microsoft visual earth map tiles will be used
-        for the map background.
-
-        If open_browser is True, python will attempt to open the web application
-        in a new tab using the default browser.
-    '''
-    proc = multiprocessing.Process(target=_start_webclient, args=[visualearth])
-    proc.start()
-    try:
-        asyncio.run(_start_webserver(tracks, domain, visualearth,
-                                     open_browser))
-        proc.join()
-    except KeyboardInterrupt:
-        print('Received KeyboardInterrupt, stopping server...')
-        proc.terminate()
-    except Exception as err:
-        proc.terminate()
-        raise err
+import asyncio
+import http.server
+import logging
+import multiprocessing
+import os
+import socketserver
+import webbrowser
+from datetime import datetime
+from functools import partial
+from tempfile import SpooledTemporaryFile
+
+import orjson
+import websockets.server
+
+logging.getLogger("websockets").setLevel(logging.WARNING)
+logging.getLogger("shapely").setLevel(logging.WARNING)
+
+wwwpath = os.path.abspath(
+    os.path.join(os.path.dirname(os.path.dirname(__file__)), 'aisdb_web',
+                 'dist_map'))
+
+wwwpath_visualearth = os.path.abspath(
+    os.path.join(os.path.dirname(os.path.dirname(__file__)), 'aisdb_web',
+                 'dist_map_bingmaps'))
+
+
+def _start_webclient(visualearth=False):
+    if not visualearth:
+        path = wwwpath
+    else:
+        path = wwwpath_visualearth
+
+    class AISDB_HTML(http.server.SimpleHTTPRequestHandler):
+
+        extensions_map = {
+            '': 'application/octet-stream',
+            '.css': 'text/css',
+            '.html': 'text/html',
+            '.jpg': 'image/jpg',
+            '.js': 'application/x-javascript',
+            '.json': 'application/json',
+            '.png': 'image/png',
+            '.wasm': 'application/wasm',
+        }
+
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, directory=path, **kwargs)
+
+    socketserver.TCPServer.allow_reuse_address = True
+    with socketserver.TCPServer(("localhost", 3000), AISDB_HTML) as httpd:
+        try:
+            print('Serving HTTP assets on localhost:3000')
+            httpd.serve_forever()
+        except KeyboardInterrupt:
+            httpd.server_close()
+            httpd.shutdown()
+        except Exception as e:
+            httpd.server_close()
+            httpd.shutdown()
+            raise e
+
+
+def serialize_zone_json(name, zone):
+    zone_dict = {
+        'msgtype': 'zone',
+        'meta': {
+            'name': name
+        },
+        'x': tuple(zone['geometry'].boundary.xy[0]),
+        'y': tuple(zone['geometry'].boundary.xy[1]),
+        't': [],
+    }
+    return orjson.dumps(zone_dict)
+
+
+def serialize_track_json(track) -> bytes:
+    ''' serializes a single track dictionary to JSON format encoded as UTF8 '''
+    vector = {
+        'msgtype': 'track_vector',
+        # currently, database_server sends all metadata as strings
+        # reproduce this behaviour by coercion to string type, even for int
+        'meta': {
+            'mmsi': str(track['mmsi'])
+        },
+        't': track['time'],
+        'x': track['lon'],
+        'y': track['lat'],
+    }
+
+    meta = {k: track[k] for k in track['static'] if k != 'marinetraffic_info'}
+    meta['msgtype'] = 'vesselinfo'
+
+    if 'marinetraffic_info' in track.keys():
+        meta.update({
+            k: track['marinetraffic_info'][k]
+            for k in track['marinetraffic_info'].keys()
+        })
+
+    vector_json = orjson.dumps(vector, option=orjson.OPT_SERIALIZE_NUMPY)
+    meta_json = orjson.dumps(meta)
+    return (vector_json, meta_json)
+
+
+async def _send_tracks(websocket, tmp_vectors, tmp_meta, domain=None):
+    ''' send tracks serialized as JSON to the connected websocket client '''
+    done = {}
+    async for message_json in websocket:
+        message = orjson.loads(message_json)
+        print(
+            f'{websocket.remote_address[0]}:{websocket.remote_address[1]} - received: {message}'
+        )
+
+        if message == {"msgtype": "validrange"}:
+            now = datetime.now().timestamp()
+            validrange = {"msgtype": "validrange", "start": now, "end": now}
+            await websocket.send(orjson.dumps(validrange))
+            done['validrange'] = True
+
+        elif message == {"msgtype": "zones"}:
+            await websocket.send(b'{"msgtype": "doneZones"}')
+            done['zones'] = True
+        elif message == {"msgtype": "meta"}:
+            done['meta'] = True
+        else:
+            raise RuntimeError(f'unknown request {message_json}')
+
+        if 'validrange' in done.keys() and 'zones' in done.keys():
+            assert len(done.keys()) == 2
+
+            if domain is not None:
+                for name, zone in domain.zones.items():
+                    zone_json = serialize_zone_json(name, zone)
+                    await websocket.send(zone_json)
+
+            tmp_vectors.seek(0)
+            for vector_json in tmp_vectors:
+                await websocket.send(vector_json)
+
+        elif 'meta' in done.keys():
+            assert len(done.keys()) == 1
+            tmp_meta.seek(0)
+            for meta_json in tmp_meta:
+                await websocket.send(meta_json)
+
+
+async def _start_webserver(tracks,
+                           domain=None,
+                           visualearth=False,
+                           open_browser=True):
+    ''' Display tracks in the web interface. Serves data to the web client '''
+    print('Querying database...', end='\t')
+    with SpooledTemporaryFile(max_size=1024 * 1e6, newline=b'\n') as vectors, \
+            SpooledTemporaryFile(max_size=256 * 1e6, newline=b'\n') as meta:
+        for vector, info in map(serialize_track_json, tracks):
+            vectors.write(vector)
+            vectors.write(b'\n')
+            meta.write(info)
+            meta.write(b'\n')
+
+        print('done query')
+
+        if open_browser:
+            print('Opening a new browser window to display track data. '
+                  'Press Ctrl-C to stop the server and close the webpage')
+            tag = 1 if not visualearth else 2
+            url = f'http://localhost:3000/index.html?python={tag}&z=2'
+            if not webbrowser.open_new_tab(url):
+                print(f'Failed to open webbrowser, instead use URL: {url}')
+
+        fcn = partial(_send_tracks,
+                      tmp_vectors=vectors,
+                      tmp_meta=meta,
+                      domain=domain)
+        async with websockets.server.serve(fcn, 'localhost', 9924) as server:
+            stop = asyncio.Future()
+            await stop
+            await server
+
+
+def visualize(tracks, domain=None, visualearth=False, open_browser=True):
+    ''' Display tracks using the web interface.
+
+        Starts the web client HTTP server in a separate process, and
+        serves track data via websocket on port 9924.
+
+        If a domain object is given, zone polygons will be drawn on the map
+        from domain zone geometries.
+
+        If visualearth is True, microsoft visual earth map tiles will be used
+        for the map background.
+
+        If open_browser is True, python will attempt to open the web application
+        in a new tab using the default browser.
+    '''
+    proc = multiprocessing.Process(target=_start_webclient, args=[visualearth])
+    proc.start()
+    try:
+        asyncio.run(_start_webserver(tracks, domain, visualearth,
+                                     open_browser))
+        proc.join()
+    except KeyboardInterrupt:
+        print('Received KeyboardInterrupt, stopping server...')
+        proc.terminate()
+    except Exception as err:
+        proc.terminate()
+        raise err
```

## aisdb/wsa.py

 * *Ordering differences only*

```diff
@@ -1,114 +1,114 @@
-'''
-Compute wetted surface area using denny-mumford regression on vessel summer
-deadweight tonnage
-
-See table 2 in below paper for coefficient and exponent by ship type
-
-Reference:
-Moser, Cameron S., et al. "Quantifying the total wetted surface area of the world fleet: a first step in determining the potential extent of ships’ biofouling." Biological Invasions 18.1 (2016): 265-277.
-
-'''
-
-
-def _wsa(dwt, ship_type, ship_type_detailed='', **_):
-    ''' regression of Denny-Mumford WSA formula using ship type '''
-
-    # None, wing in ground craft, other
-    if (isinstance(ship_type, int)
-            and ship_type < 30) or ship_type == 'Wing In Grnd':
-        return 0
-
-    # fishing
-    elif (isinstance(ship_type, int)
-          and ship_type == 30) or ship_type == 'Fishing':
-        coef = 15.58
-        exp = 0.602
-
-    # tugs and port tenders
-    elif (isinstance(ship_type, int)
-          and 52 <= ship_type <= 53) or ship_type == 'Tug':
-        coef = 19.36
-        exp = 0.553
-
-    # passenger
-    elif (isinstance(ship_type, int)
-          and 60 <= ship_type < 70) or ship_type == 'Passenger':
-        coef = 14.64
-        exp = 0.671
-
-    # container ships
-    elif 'Container' in ship_type_detailed:
-        coef = 5.39
-        exp = 0.698
-
-    # bulk carriers
-    # note: cement classified as bulk carrier
-    elif 'Bulk' in ship_type_detailed or 'Cement' in ship_type_detailed:
-        coef = 9.57
-        exp = 0.63
-
-    # NOTE: no distinction for container ships or bulk carriers when using
-    # numeric ship type
-    # general cargo ship regression is used for these categories
-    elif (isinstance(ship_type, int)
-          and 70 <= ship_type < 80) or (isinstance(ship_type, str)
-                                        and 'Cargo' in ship_type):  # cargo
-        coef = 14.24
-        exp = 0.596
-
-    # tankers (LNG / LPG)
-    elif (isinstance(ship_type, int) and ship_type == 84) or (
-        (isinstance(ship_type, str) and
-         ('Tanker' in ship_type and
-          ('Oil' in ship_type_detailed or 'LNG' in ship_type_detailed
-           or 'LPG' in ship_type_detailed)))):
-        coef = 5.41
-        exp = 0.699
-
-    # tankers (general)
-    elif (isinstance(ship_type, int)
-          and 80 <= ship_type < 90) or (isinstance(ship_type, str)
-                                        and 'Tanker' in ship_type):
-        coef = 9.56
-        exp = 0.63
-
-    # SAR, law enforcement, towing, dredging, diving, military, sailing,
-    # pleasure craft, etc
-    else:
-        coef = 26.2
-        exp = 0.551
-
-    return coef * pow(base=dwt, exp=exp)
-
-
-def wetted_surface_area(tracks):
-    ''' regression of Denny-Mumford WSA formula using ship type
-
-        args:
-            tracks (:func:`aisdb.webdata.marinetraffic.vessel_info`)
-                track generator with vessel_info appended
-
-        yields:
-            track dicts with submerged surface area in square meters appended
-            to key 'submerged_hull_m^2'
-    '''
-    for track in tracks:
-        dwt = track['marinetraffic_info']['summer_dwt'] or 0
-        if 'marinetraffic_info' in track.keys(
-        ) and track['marinetraffic_info']['vesseltype_generic'] is not None:
-            hull = _wsa(dwt, track['marinetraffic_info']['vesseltype_generic'],
-                        track['marinetraffic_info']['vesseltype_detailed'])
-        else:
-            if 'ship_type' not in track.keys():
-                raise KeyError(
-                    "'ship_type' not in track: try using "
-                    "aisdb.database.sqlfcn.crawl_dynamic_static as 'fcn' arg "
-                    "for DBQuery.gen_qry()")
-            hull = _wsa(dwt, track['ship_type'] or 0)
-
-        track['submerged_hull_m^2'] = hull
-        track['static'] = set(track['static']).union(
-            set([
-                'submerged_hull_m^2',
-            ]))
-        yield track
+'''
+Compute wetted surface area using denny-mumford regression on vessel summer
+deadweight tonnage
+
+See table 2 in below paper for coefficient and exponent by ship type
+
+Reference:
+Moser, Cameron S., et al. "Quantifying the total wetted surface area of the world fleet: a first step in determining the potential extent of ships’ biofouling." Biological Invasions 18.1 (2016): 265-277.
+
+'''
+
+
+def _wsa(dwt, ship_type, ship_type_detailed='', **_):
+    ''' regression of Denny-Mumford WSA formula using ship type '''
+
+    # None, wing in ground craft, other
+    if (isinstance(ship_type, int)
+            and ship_type < 30) or ship_type == 'Wing In Grnd':
+        return 0
+
+    # fishing
+    elif (isinstance(ship_type, int)
+          and ship_type == 30) or ship_type == 'Fishing':
+        coef = 15.58
+        exp = 0.602
+
+    # tugs and port tenders
+    elif (isinstance(ship_type, int)
+          and 52 <= ship_type <= 53) or ship_type == 'Tug':
+        coef = 19.36
+        exp = 0.553
+
+    # passenger
+    elif (isinstance(ship_type, int)
+          and 60 <= ship_type < 70) or ship_type == 'Passenger':
+        coef = 14.64
+        exp = 0.671
+
+    # container ships
+    elif 'Container' in ship_type_detailed:
+        coef = 5.39
+        exp = 0.698
+
+    # bulk carriers
+    # note: cement classified as bulk carrier
+    elif 'Bulk' in ship_type_detailed or 'Cement' in ship_type_detailed:
+        coef = 9.57
+        exp = 0.63
+
+    # NOTE: no distinction for container ships or bulk carriers when using
+    # numeric ship type
+    # general cargo ship regression is used for these categories
+    elif (isinstance(ship_type, int)
+          and 70 <= ship_type < 80) or (isinstance(ship_type, str)
+                                        and 'Cargo' in ship_type):  # cargo
+        coef = 14.24
+        exp = 0.596
+
+    # tankers (LNG / LPG)
+    elif (isinstance(ship_type, int) and ship_type == 84) or (
+        (isinstance(ship_type, str) and
+         ('Tanker' in ship_type and
+          ('Oil' in ship_type_detailed or 'LNG' in ship_type_detailed
+           or 'LPG' in ship_type_detailed)))):
+        coef = 5.41
+        exp = 0.699
+
+    # tankers (general)
+    elif (isinstance(ship_type, int)
+          and 80 <= ship_type < 90) or (isinstance(ship_type, str)
+                                        and 'Tanker' in ship_type):
+        coef = 9.56
+        exp = 0.63
+
+    # SAR, law enforcement, towing, dredging, diving, military, sailing,
+    # pleasure craft, etc
+    else:
+        coef = 26.2
+        exp = 0.551
+
+    return coef * pow(base=dwt, exp=exp)
+
+
+def wetted_surface_area(tracks):
+    ''' regression of Denny-Mumford WSA formula using ship type
+
+        args:
+            tracks (:func:`aisdb.webdata.marinetraffic.vessel_info`)
+                track generator with vessel_info appended
+
+        yields:
+            track dicts with submerged surface area in square meters appended
+            to key 'submerged_hull_m^2'
+    '''
+    for track in tracks:
+        dwt = track['marinetraffic_info']['summer_dwt'] or 0
+        if 'marinetraffic_info' in track.keys(
+        ) and track['marinetraffic_info']['vesseltype_generic'] is not None:
+            hull = _wsa(dwt, track['marinetraffic_info']['vesseltype_generic'],
+                        track['marinetraffic_info']['vesseltype_detailed'])
+        else:
+            if 'ship_type' not in track.keys():
+                raise KeyError(
+                    "'ship_type' not in track: try using "
+                    "aisdb.database.sqlfcn.crawl_dynamic_static as 'fcn' arg "
+                    "for DBQuery.gen_qry()")
+            hull = _wsa(dwt, track['ship_type'] or 0)
+
+        track['submerged_hull_m^2'] = hull
+        track['static'] = set(track['static']).union(
+            set([
+                'submerged_hull_m^2',
+            ]))
+        yield track
```

## aisdb/__init__.py

 * *Ordering differences only*

```diff
@@ -1,75 +1,75 @@
-import os
-import logging
-import warnings
-
-import sqlite3
-if (sqlite3.sqlite_version_info[0] < 3
-        or (sqlite3.sqlite_version_info[0] <= 3
-            and sqlite3.sqlite_version_info[1] < 8)):
-    warnings.warn(
-        f"An outdated version of SQLite was found ({sqlite3.sqlite_version})")
-
-sqlpath = os.path.abspath(os.path.join(os.path.dirname(__file__), 'aisdb_sql'))
-
-import aisdb.web_interface
-
-from .database.create_tables import (
-    aggregate_static_msgs,
-    sqlite_createtable_dynamicreport,
-    sqlite_createtable_staticreport,
-)
-
-from .database.dbconn import DBConn, SQLiteDBConn, PostgresDBConn
-
-from .database.decoder import decode_msgs
-
-from .database.dbqry import DBQuery
-
-from .database import sqlfcn
-
-from .database import sqlfcn_callbacks
-
-from .webdata.bathymetry import Gebco
-
-from .webdata.shore_dist import ShoreDist, PortDist
-
-from .gis import (
-    Domain,
-    DomainFromTxts,
-    DomainFromPoints,
-    delta_knots,
-    delta_meters,
-    delta_seconds,
-    distance3D,
-    dt_2_epoch,
-    epoch_2_dt,
-    radial_coordinate_boundary,
-    vesseltrack_3D_dist,
-)
-
-from .interp import (
-    interp_time, )
-
-from .network_graph import graph
-
-from .receiver import start_receiver
-
-from .proc_util import (
-    glob_files,
-    write_csv,
-)
-
-from .track_gen import (
-    TrackGen,
-    split_timedelta,
-    fence_tracks,
-)
-from .denoising_encoder import (
-    encode_score,
-    encode_greatcircledistance,
-)
-
-LOGLEVEL = os.environ.get('LOGLEVEL', 'INFO')
-logging.basicConfig(format='%(message)s',
-                    level=LOGLEVEL,
-                    datefmt='%Y-%m-%d %I:%M:%S')
+import os
+import logging
+import warnings
+
+import sqlite3
+if (sqlite3.sqlite_version_info[0] < 3
+        or (sqlite3.sqlite_version_info[0] <= 3
+            and sqlite3.sqlite_version_info[1] < 8)):
+    warnings.warn(
+        f"An outdated version of SQLite was found ({sqlite3.sqlite_version})")
+
+sqlpath = os.path.abspath(os.path.join(os.path.dirname(__file__), 'aisdb_sql'))
+
+import aisdb.web_interface
+
+from .database.create_tables import (
+    aggregate_static_msgs,
+    sqlite_createtable_dynamicreport,
+    sqlite_createtable_staticreport,
+)
+
+from .database.dbconn import DBConn, SQLiteDBConn, PostgresDBConn
+
+from .database.decoder import decode_msgs
+
+from .database.dbqry import DBQuery
+
+from .database import sqlfcn
+
+from .database import sqlfcn_callbacks
+
+from .webdata.bathymetry import Gebco
+
+from .webdata.shore_dist import ShoreDist, PortDist
+
+from .gis import (
+    Domain,
+    DomainFromTxts,
+    DomainFromPoints,
+    delta_knots,
+    delta_meters,
+    delta_seconds,
+    distance3D,
+    dt_2_epoch,
+    epoch_2_dt,
+    radial_coordinate_boundary,
+    vesseltrack_3D_dist,
+)
+
+from .interp import (
+    interp_time, )
+
+from .network_graph import graph
+
+from .receiver import start_receiver
+
+from .proc_util import (
+    glob_files,
+    write_csv,
+)
+
+from .track_gen import (
+    TrackGen,
+    split_timedelta,
+    fence_tracks,
+)
+from .denoising_encoder import (
+    encode_score,
+    encode_greatcircledistance,
+)
+
+LOGLEVEL = os.environ.get('LOGLEVEL', 'INFO')
+logging.basicConfig(format='%(message)s',
+                    level=LOGLEVEL,
+                    datefmt='%Y-%m-%d %I:%M:%S')
```

## Comparing `aisdb-1.6.0.dist-info/METADATA` & `aisdb-1.6.3.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdb
-Version: 1.6.0
+Version: 1.6.3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,118 +25,120 @@
 Requires-Dist: tqdm
 Requires-Dist: numpy
 Requires-Dist: webdriver-manager
 Requires-Dist: psycopg
 Requires-Dist: psycopg[binary]
 Requires-Dist: orjson
 Requires-Dist: websockets
-Requires-Dist: sphinx; extra == 'docs'
-Requires-Dist: sphinx-rtd-theme; extra == 'docs'
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-dotenv; extra == 'test'
-Provides-Extra: docs
-Provides-Extra: test
+Requires-Dist: sphinx; extra == 'docs'
+Requires-Dist: sphinx-rtd-theme; extra == 'docs'
 Provides-Extra: devel
+Provides-Extra: test
+Provides-Extra: docs
 Summary: AIS Database and Processing Utils
 Author-email: Matthew Smith <matthew.smith@dal.ca>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
-Project-URL: documentation, https://aisdb.meridian.cs.dal.ca/doc/readme.html
 Project-URL: repository, https://git-dev.cs.dal.ca/meridian/aisdb
+Project-URL: documentation, https://aisdb.meridian.cs.dal.ca/doc/readme.html
 Project-URL: homepage, https://aisdb.meridian.cs.dal.ca/
 
-Readme
-======
-
-.. image:: https://git-dev.cs.dal.ca/meridian/aisdb/badges/master/pipeline.svg
-
-.. image:: https://img.shields.io/gitlab/coverage/meridian/aisdb/master?gitlab_url=https%3A%2F%2Fgit-dev.cs.dal.ca&job_name=python-test
-
-.. image:: https://img.shields.io/gitlab/v/release/meridian/aisdb?gitlab_url=https%3A%2F%2Fgit-dev.cs.dal.ca&include_prereleases&sort=semver
-
-.. description:
-
-Description
------------
-
-Package features:
-  + SQL database for storing AIS position reports and vessel metadata
-  + Vessel position cleaning and trajectory modeling
-  + Utilities for streaming and decoding AIS data in the NMEA binary string format (See `Base Station Deployment <AIS_base_station.html>`__)
-  + Integration with external datasources including depth charts, distances from shore, vessel geometry, etc.
-  + Network graph analysis, MMSI deduplication, interpolation, and other processing utilities
-  + Data visualization
-
-
-.. image:: https://aisdb.meridian.cs.dal.ca/readme_example.png
-
-
-| Web Interface:
-  https://aisdb.meridian.cs.dal.ca/
-| Docs:
-  https://aisdb.meridian.cs.dal.ca/doc/readme.html
-| Source Code: 
-  https://git-dev.cs.dal.ca/meridian/aisdb
-
-.. whatisais:
-
-What is AIS?
-------------
-
-| Wikipedia:
-  https://en.wikipedia.org/wiki/Automatic_identification_system
-| Description of message types:
-  https://arundaleais.github.io/docs/ais/ais_message_types.html
-
-
-
-Install
--------
-
-.. _install-pip:
-  
-Requires Python version 3.9 or newer installed on the system.
-Optionally requires SQLite (included by default in most versions of Python).
-The AISDB Python package can be installed with pip in a virtual Python environment from the command line:
-
-.. code-block:: sh
-
-   python -m venv env_ais && source ./env_ais/*/activate
-   pip install aisdb
-
-.. _install-src:
-
-For information on installing AISDB from source code, see `Installing from Source <https://aisdb.meridian.cs.dal.ca/doc/install_from_source.html>`__
-
-.. _readme-docs:
-
-
-Documentation
--------------
-
-An introduction to AISDB can be found here: `Introduction <https://aisdb.meridian.cs.dal.ca/doc/intro.html>`__.
-
-Additional API documentation: `API Docs <https://aisdb.meridian.cs.dal.ca/doc/api/aisdb.html>`__.
-
-.. _readme-examples:
-
-Code examples
--------------
-
-1. `Parsing raw format messages into a
-   database <https://aisdb.meridian.cs.dal.ca/doc/api/aisdb.database.decoder.html#aisdb.database.decoder.decode_msgs>`__
-
-2. `Automatically generate SQL database
-   queries <https://aisdb.meridian.cs.dal.ca/doc/api/aisdb.database.dbqry.html#aisdb.database.dbqry.DBQuery>`__
-
-3. `Compute trajectories from database rows <https://aisdb.meridian.cs.dal.ca/doc/api/aisdb.track_gen.html#aisdb.track_gen.TrackGen>`__
-
-4. `Vessel trajectory cleaning and MMSI deduplication <https://aisdb.meridian.cs.dal.ca/doc/api/aisdb.track_gen.html#aisdb.track_gen.encode_greatcircledistance>`__
-
-5. `Compute network graph of vessel movements between
-   polygons <https://aisdb.meridian.cs.dal.ca/doc/api/aisdb.network_graph.html#aisdb.network_graph.graph>`__
-
-6. Integrating data from web sources, such as depth charts, shore distance, etc.
-
+Readme
+======
+
+.. image:: https://git-dev.cs.dal.ca/meridian/aisdb/badges/master/pipeline.svg
+
+.. image:: https://img.shields.io/gitlab/coverage/meridian/aisdb/master?gitlab_url=https%3A%2F%2Fgit-dev.cs.dal.ca&job_name=python-test
+
+.. image:: https://img.shields.io/gitlab/v/release/meridian/aisdb?gitlab_url=https%3A%2F%2Fgit-dev.cs.dal.ca&include_prereleases&sort=semver
+
+.. description:
+
+Description
+-----------
+
+Package features:
+  + SQL database for storing AIS position reports and vessel metadata
+  + Vessel position cleaning and trajectory modeling
+  + Utilities for streaming and decoding AIS data in the NMEA binary string format (See `Base Station Deployment <AIS_base_station.html>`__)
+  + Integration with external datasources including depth charts, distances from shore, vessel geometry, etc.
+  + Network graph analysis, MMSI deduplication, interpolation, and other processing utilities
+  + Data visualization
+
+
+.. image:: https://aisdb.meridian.cs.dal.ca/readme_example.png
+
+
+| Web Interface:
+  https://aisdb.meridian.cs.dal.ca/
+| Docs:
+  https://aisdb.meridian.cs.dal.ca/doc/readme.html
+| Source Code: 
+  https://git-dev.cs.dal.ca/meridian/aisdb
+
+.. whatisais:
+
+What is AIS?
+------------
+
+| Wikipedia:
+  https://en.wikipedia.org/wiki/Automatic_identification_system
+| Description of message types:
+  https://arundaleais.github.io/docs/ais/ais_message_types.html
+
+
+
+Install
+-------
+
+.. _install-pip:
+  
+Requires Python version 3.8 or newer.
+Optionally requires SQLite (included in Python) or PostgresQL server (installed separately).
+The AISDB Python package can be installed using pip.
+It is recommended to install the package in a virtual Python environment such as ``venv``.
+
+.. code-block:: sh
+
+   python -m venv env_ais 
+   source ./env_ais/*/activate
+   pip install aisdb
+
+.. _install-src:
+
+For information on installing AISDB from source code, see `Installing from Source <https://aisdb.meridian.cs.dal.ca/doc/install_from_source.html>`__
+
+.. _readme-docs:
+
+
+Documentation
+-------------
+
+An introduction to AISDB can be found here: `Introduction <https://aisdb.meridian.cs.dal.ca/doc/intro.html>`__.
+
+Additional API documentation: `API Docs <https://aisdb.meridian.cs.dal.ca/doc/api/aisdb.html>`__.
+
+.. _readme-examples:
+
+Code examples
+-------------
+
+1. `Parsing raw format messages into a
+   database <https://aisdb.meridian.cs.dal.ca/doc/api/aisdb.database.decoder.html#aisdb.database.decoder.decode_msgs>`__
+
+2. `Automatically generate SQL database
+   queries <https://aisdb.meridian.cs.dal.ca/doc/api/aisdb.database.dbqry.html#aisdb.database.dbqry.DBQuery>`__
+
+3. `Compute trajectories from database rows <https://aisdb.meridian.cs.dal.ca/doc/api/aisdb.track_gen.html#aisdb.track_gen.TrackGen>`__
+
+4. `Vessel trajectory cleaning and MMSI deduplication <https://aisdb.meridian.cs.dal.ca/doc/api/aisdb.track_gen.html#aisdb.track_gen.encode_greatcircledistance>`__
+
+5. `Compute network graph of vessel movements between
+   polygons <https://aisdb.meridian.cs.dal.ca/doc/api/aisdb.network_graph.html#aisdb.network_graph.graph>`__
+
+6. Integrating data from web sources, such as depth charts, shore distance, etc.
+
```

