# Comparing `tmp/py-eodms-rapi-1.5.4.tar.gz` & `tmp/py-eodms-rapi-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-eodms-rapi-1.5.4.tar", last modified: Tue May 23 19:05:36 2023, max compression
+gzip compressed data, was "py-eodms-rapi-1.5.5.tar", last modified: Thu Jun  8 18:39:06 2023, max compression
```

## Comparing `py-eodms-rapi-1.5.4.tar` & `py-eodms-rapi-1.5.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 19:05:36.478029 py-eodms-rapi-1.5.4/
--rw-rw-rw-   0        0        0     1180 2023-02-17 19:07:52.000000 py-eodms-rapi-1.5.4/LICENSE
--rw-rw-rw-   0        0        0     2841 2023-05-23 19:05:36.478029 py-eodms-rapi-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     2034 2022-06-16 17:33:17.000000 py-eodms-rapi-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 19:05:36.411837 py-eodms-rapi-1.5.4/eodms_rapi/
--rw-rw-rw-   0        0        0      535 2023-03-06 20:45:07.000000 py-eodms-rapi-1.5.4/eodms_rapi/__init__.py
--rw-rw-rw-   0        0        0   130009 2023-05-23 18:55:00.000000 py-eodms-rapi-1.5.4/eodms_rapi/eodms.py
--rw-rw-rw-   0        0        0    24662 2022-10-13 17:59:38.000000 py-eodms-rapi-1.5.4/eodms_rapi/geo.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:05:36.446720 py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/
--rw-rw-rw-   0        0        0     2841 2023-05-23 19:05:35.000000 py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-05-23 19:05:35.000000 py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 19:05:35.000000 py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-23 19:05:35.000000 py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-23 19:05:35.000000 py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      827 2023-05-23 19:05:36.481042 py-eodms-rapi-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1151 2023-03-06 21:00:57.000000 py-eodms-rapi-1.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:05:36.474722 py-eodms-rapi-1.5.4/test/
--rw-rw-rw-   0        0        0     6987 2022-10-13 18:00:49.000000 py-eodms-rapi-1.5.4/test/test_pyeodmsrapi.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:39:06.658344 py-eodms-rapi-1.5.5/
+-rw-rw-rw-   0        0        0     1180 2023-02-17 19:07:52.000000 py-eodms-rapi-1.5.5/LICENSE
+-rw-rw-rw-   0        0        0     2841 2023-06-08 18:39:06.658344 py-eodms-rapi-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2034 2022-06-16 17:33:17.000000 py-eodms-rapi-1.5.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 18:39:06.604276 py-eodms-rapi-1.5.5/eodms_rapi/
+-rw-rw-rw-   0        0        0      535 2023-06-08 18:27:53.000000 py-eodms-rapi-1.5.5/eodms_rapi/__init__.py
+-rw-rw-rw-   0        0        0   130078 2023-06-08 18:28:00.000000 py-eodms-rapi-1.5.5/eodms_rapi/eodms.py
+-rw-rw-rw-   0        0        0    23780 2023-06-08 18:28:02.000000 py-eodms-rapi-1.5.5/eodms_rapi/geo.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:39:06.641346 py-eodms-rapi-1.5.5/py_eodms_rapi.egg-info/
+-rw-rw-rw-   0        0        0     2841 2023-06-08 18:39:05.000000 py-eodms-rapi-1.5.5/py_eodms_rapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-08 18:39:06.000000 py-eodms-rapi-1.5.5/py_eodms_rapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 18:39:05.000000 py-eodms-rapi-1.5.5/py_eodms_rapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-08 18:39:05.000000 py-eodms-rapi-1.5.5/py_eodms_rapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-08 18:39:05.000000 py-eodms-rapi-1.5.5/py_eodms_rapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      827 2023-06-08 18:39:06.661309 py-eodms-rapi-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1151 2023-06-08 18:27:50.000000 py-eodms-rapi-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:39:06.655345 py-eodms-rapi-1.5.5/test/
+-rw-rw-rw-   0        0        0     6987 2022-10-13 18:00:49.000000 py-eodms-rapi-1.5.5/test/test_pyeodmsrapi.py
```

### Comparing `py-eodms-rapi-1.5.4/LICENSE` & `py-eodms-rapi-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-eodms-rapi-1.5.4/PKG-INFO` & `py-eodms-rapi-1.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-eodms-rapi
-Version: 1.5.4
+Version: 1.5.5
 Summary: EODMS RAPI Client is a Python3 package used to access the REST API service provided by the Earth Observation Data Management System (EODMS) from Natural Resources Canada.
 Home-page: https://py-eodms-rapi.readthedocs.io/en/latest/
 Author: Kevin Ballantyne (Natural Resources Canada)
 Author-email: kevin.ballantyne@nrcan-rncan.gc.ca
 License: LICENSE
 Project-URL: Source, https://github.com/eodms-sgdot/py-eodms-rapi
 Project-URL: Bug Tracker, https://github.com/eodms-sgdot/py-eodms-rapi/issues
```

### Comparing `py-eodms-rapi-1.5.4/README.md` & `py-eodms-rapi-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `py-eodms-rapi-1.5.4/eodms_rapi/__init__.py` & `py-eodms-rapi-1.5.5/eodms_rapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __title__ = 'py-eodms-rapi'
 __name__ = 'eodms_rapi'
 __author__ = 'Kevin Ballantyne'
 __copyright__ = 'Copyright (c) His Majesty the King in Right of Canada, ' \
                 'as represented by the Minister of Natural Resources, 2022'
 __license__ = 'MIT License'
 __description__ = 'A Python package to access the EODMS RAPI service.'
-__version__ = '1.5.4'
+__version__ = '1.5.5'
 __maintainer__ = 'Kevin Ballantyne'
 __email__ = 'eodms-sgdot@nrcan-rncan.gc.ca'
 
 from .eodms import EODMSRAPI
 from .eodms import QueryError
 from .geo import EODMSGeo
```

### Comparing `py-eodms-rapi-1.5.4/eodms_rapi/eodms.py` & `py-eodms-rapi-1.5.5/eodms_rapi/eodms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1210,18 +1210,19 @@
                     # Convert choice to value
                     choices = self.get_field_choices(self.collection, 
                                                      field_id, True)
                     valid_vals = []
                     for v in val:
                         new_val = None
                         for c in choices:
-                            if c.get('label') == v:
-                                new_val = c.get('value')
-                                valid_vals.append(new_val)
-                                break
+                            if isinstance(c, dict):
+                                if c.get('label') == v:
+                                    new_val = c.get('value')
+                                    valid_vals.append(new_val)
+                                    break
                         if not new_val:
                             valid_vals.append(v)
 
                     val = valid_vals
 
                     if len(val) > 1:
                         val_query = self._build_or(field_id, op, val, d_type)
```

### Comparing `py-eodms-rapi-1.5.4/eodms_rapi/geo.py` & `py-eodms-rapi-1.5.5/eodms_rapi/geo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ##############################################################################
 # MIT License
 # 
 # Copyright (c) His Majesty the King in Right of Canada, as
-# represented by the Minister of Natural Resources, 2022
+# represented by the Minister of Natural Resources, 2023
 # 
 # Permission is hereby granted, free of charge, to any person obtaining a 
 # copy of this software and associated documentation files (the "Software"), 
 # to deal in the Software without restriction, including without limitation 
 # the rights to use, copy, modify, merge, publish, distribute, sublicense, 
 # and/or sell copies of the Software, and to permit persons to whom the 
 # Software is furnished to do so, subject to the following conditions:
@@ -112,18 +112,18 @@
     def _check_ogr(self):
         """
         There is another ogr Python package. This will check if it was
             imported instead of the proper ogr.
         """
 
         if ogr.__doc__ is not None and \
-                ogr.__doc__.find("Module providing one api for multiple git "
+                    ogr.__doc__.find("Module providing one api for multiple git "
                                  "services") > -1:
-            msg = "Another package named 'ogr' is installed."
             if self.eodmsrapi is not None:
+                msg = "Another package named 'ogr' is installed."
                 self.eodmsrapi.log_msg(msg, 'warning')
             return False
 
         return True
 
     def _convert_list(self, in_feat, out='wkt'):
         """
@@ -173,18 +173,15 @@
             wkt_val = wkt.loads(in_feat.upper())
         except (ValueError, TypeError) as e:
             if show_error:
                 if self.eodmsrapi is not None:
                     self.eodmsrapi.log_msg(str(e), 'warning')
             return False
 
-        if return_wkt:
-            return wkt_val
-        else:
-            return True
+        return wkt_val if return_wkt else True
 
     def _remove_zero_trail(self, in_wkt):
         """
         Removes the trailing zeros in coordinates after the decimal in a WKT.
         
         :param in_wkt: The input WKT.
         :type  in_wkt: str
@@ -314,15 +311,15 @@
                 return self.feats
 
         # If the source is a list of coordinates
         if not isinstance(in_src, list):
             try:
                 eval(in_src)
             except SyntaxError as err:
-                self.logger.warning("%s" % err)
+                self.logger.warning(f"{err}")
                 return err
 
     def convert_coords(self, coord_lst, geom_type):
         """
         Converts a list of points to GeoJSON format.
         
         :param coord_lst: A list of points.
@@ -335,34 +332,39 @@
         :rtype:  dict
         
         """
 
         pnts_array = []
         pnts = None
         for c in coord_lst:
-            pnts = [p.strip('\n').strip('\t').split(',') for p in
-                    c.split(' ') if not p.strip('\n').strip('\t') == '']
+            pnts = [
+                p.strip('\n').strip('\t').split(',')
+                for p in c.split(' ')
+                if p.strip('\n').strip('\t') != ''
+            ]
             pnts_array += pnts
 
         if pnts is None:
             return None
 
-        if geom_type == 'Point':
-            json_geom = {'type': 'Point', 'coordinates': [float(pnts[0][0]),
-                                                          float(pnts[0][1])]}
-        elif geom_type == 'LineString':
-            json_geom = {'type': 'LineString', 'coordinates': [[float(p[0]),
-                                                                float(p[1])]
-                                                               for p in pnts]}
+        if geom_type == 'LineString':
+            return {
+                'type': 'LineString',
+                'coordinates': [[float(p[0]), float(p[1])] for p in pnts],
+            }
+        elif geom_type == 'Point':
+            return {
+                'type': 'Point',
+                'coordinates': [float(pnts[0][0]), float(pnts[0][1])],
+            }
         else:
-            json_geom = {'type': 'Polygon', 'coordinates': [[[float(p[0]),
-                                                              float(p[1])]
-                                                             for p in pnts]]}
-
-        return json_geom
+            return {
+                'type': 'Polygon',
+                'coordinates': [[[float(p[0]), float(p[1])] for p in pnts]],
+            }
 
     def convert_image_geom(self, coords, output='array'):
         """
         Converts a list of coordinates from the RAPI to a polygon geometry,
         array of points or as WKT.
         
         :param coords: A list of coordinates from the RAPI results.
@@ -392,32 +394,31 @@
                     pnt_array = coords['coordinates']
             else:
                 self.logger.warning("No coordinates provided.")
                 return None
         else:
             pnt_array = coords[0]
 
-        # Get the points from the coordinates list
-        pnt1 = pnt_array[0]
-        pnt2 = pnt_array[1]
-        pnt3 = pnt_array[2]
-        pnt4 = pnt_array[3]
-
         if GDAL_INSTALLED:
             if not self._check_ogr():
-                msg = "Cannot convert geometry."
                 if self.eodmsrapi is not None:
-                    self.eodmsrapi.log_msg(msg, 'warning')
+                    self.eodmsrapi.log_msg("Cannot convert geometry.", 'warning')
                 return None
 
             # Create ring
             ring = ogr.Geometry(ogr.wkbLinearRing)
+            # Get the points from the coordinates list
+            pnt1 = pnt_array[0]
             ring.AddPoint(pnt1[0], pnt1[1])
+            pnt2 = pnt_array[1]
             ring.AddPoint(pnt2[0], pnt2[1])
+            pnt3 = pnt_array[2]
             ring.AddPoint(pnt3[0], pnt3[1])
+            pnt4 = pnt_array[3]
+
             ring.AddPoint(pnt4[0], pnt4[1])
             ring.AddPoint(pnt1[0], pnt1[1])
 
             # Create polygon
             poly = ogr.Geometry(ogr.wkbPolygon)
             poly.AddGeometry(ring)
 
@@ -425,23 +426,22 @@
             if output == 'wkt':
                 return poly.ExportToWkt()
             elif output == 'geom':
                 return poly
             else:
                 return pnt_array
 
-        else:
-            if output == 'wkt':
-                # Convert values in point array to strings
-                pnt_array = [[str(p[0]), str(p[1])] for p in pnt_array]
+        elif output == 'wkt':
+            # Convert values in point array to strings
+            pnt_array = [[str(p[0]), str(p[1])] for p in pnt_array]
 
-                return "POLYGON ((%s))" % ', '.join([' '.join(pnt)
-                                                     for pnt in pnt_array])
-            else:
-                return pnt_array
+            return "POLYGON ((%s))" % ', '.join([' '.join(pnt)
+                                                 for pnt in pnt_array])
+        else:
+            return pnt_array
 
     # def convert_fromWKT(self, in_feat):
     # """
     # Converts a WKT to a GDAL geometry.
 
     # :param in_feat: The WKT of the feature.
     # :type  in_feat: str
@@ -474,17 +474,15 @@
 
         out_wkt = None
         if in_type == 'json':
             out_wkt = wkt.dumps(in_feat)
         elif in_type == 'list':
             out_wkt = self._convert_list(in_feat)
         elif in_type == 'file':
-            out_wkts = self.get_features(in_feat)
-            return out_wkts
-
+            return self.get_features(in_feat)
         out_wkt = self._remove_zero_trail(out_wkt)
 
         return out_wkt
 
     def convert_to_geojson(self, results, output='FeatureCollection'):
         """
         Converts RAPI results to GeoJSON geometries.
@@ -512,38 +510,35 @@
             feat = {"type": "Feature", "geometry": geom, "properties": props}
 
             features.append(feat)
 
         if output == 'list':
             return features
 
-        feature_collection = {"type": "FeatureCollection",
-                              "features": features}
-
-        return feature_collection
+        return {"type": "FeatureCollection", "features": features}
 
     def process_polygon(self, geom, t_crs):
 
         # Convert the geometry to WGS84
         s_crs = geom.GetSpatialReference()
 
         if s_crs is None:
             s_crs = osr.SpatialReference()
             s_crs.ImportFromEPSG(4326)
 
         # Get the EPSG codes from the spatial references
         epsg_scrs = s_crs.GetAttrValue("AUTHORITY", 1)
         epsg_tcrs = t_crs.GetAttrValue("AUTHORITY", 1)
 
-        if not str(epsg_scrs) == '4326':
+        if str(epsg_scrs) != '4326':
             if epsg_tcrs is None:
                 print("\nCannot reproject AOI.")
                 return None
 
-            if not s_crs.IsSame(t_crs) and not epsg_scrs == epsg_tcrs:
+            if not s_crs.IsSame(t_crs) and epsg_scrs != epsg_tcrs:
                 # Create the CoordinateTransformation
                 print("\nReprojecting input AOI...")
                 coord_trans = osr.CoordinateTransformation(s_crs, t_crs)
                 geom.Transform(coord_trans)
 
                 # Reverse x and y of transformed geometry
                 ring = geom.GetGeometryRef(0)
@@ -586,16 +581,15 @@
             elif in_src.find('.kml') > -1:
                 ogr_driver = 'KML'
             elif in_src.find('.json') > -1 or in_src.find('.geojson') > -1:
                 ogr_driver = 'GeoJSON'
             elif in_src.find('.shp') > -1:
                 ogr_driver = 'ESRI Shapefile'
             else:
-                err_msg = "The AOI file type could not be determined."
-                self.logger.error(err_msg)
+                self.logger.error("The AOI file type could not be determined.")
                 return None
 
             # Open AOI file and extract AOI
             driver = ogr.GetDriverByName(ogr_driver)
             ds = driver.Open(in_src, 0)
 
             # Get the layer from the file
@@ -606,100 +600,92 @@
             t_crs.ImportFromEPSG(4326)
 
             for feat in lyr:
                 # Create the geometry
                 geom = feat.GetGeometryRef()
 
                 if geom.GetGeometryName() == 'MULTIPOLYGON':
-                    for geom_part in geom:
-                        # print("geom_part: %s" % geom_part)
-                        out_feats.append(self.process_polygon(geom_part, t_crs))
+                    out_feats.extend(self.process_polygon(geom_part, t_crs) for geom_part in geom)
                 else:
                     out_feats.append(self.process_polygon(geom, t_crs))
 
-        else:
+        elif in_src.find('.gml') > -1 or in_src.find('.kml') > -1:
+
+            with open(in_src, 'rt') as f:
+                tree = ElementTree.parse(f)
+                root = tree.getroot()
 
             geom_choices = ['Point', 'LineString', 'Polygon']
 
-            # Determine the OGR driver of the input AOI
-            if in_src.find('.gml') > -1 or in_src.find('.kml') > -1:
+            if in_src.find('.gml') > -1:
+                for feat in root.findall('.//{http://www.opengis.net/'
+                                             'gml}featureMember'):
 
-                with open(in_src, 'rt') as f:
-                    tree = ElementTree.parse(f)
-                    root = tree.getroot()
+                    # Get geometry type
+                    geom_type = 'Polygon'
+                    for elem in feat.findall('*'):
+                        tag = elem.tag.replace('{http://ogr.maptools.'
+                                               'org/}', '')
+                        if tag in geom_choices:
+                            geom_type = tag
+
+                    coord_lst = [
+                        coords.text
+                        for coords in root.findall(
+                            './/{http://www.opengis' '.net/gml}coordinates'
+                        )
+                    ]
+                    json_geom = self.convert_coords(coord_lst, geom_type)
 
-                if in_src.find('.gml') > -1:
-                    for feat in root.findall('.//{http://www.opengis.net/'
-                                             'gml}featureMember'):
+                    wkt_feat = self._split_multi(json_geom)
 
-                        # Get geometry type
-                        geom_type = 'Polygon'
-                        for elem in feat.findall('*'):
-                            tag = elem.tag.replace('{http://ogr.maptools.'
-                                                   'org/}', '')
-                            if tag in geom_choices:
-                                geom_type = tag
-
-                        coord_lst = []
-                        for coords in root.findall('.//{http://www.opengis'
-                                                   '.net/gml}coordinates'):
-                            coord_lst.append(coords.text)
-
-                        json_geom = self.convert_coords(coord_lst, geom_type)
-
-                        wkt_feat = self._split_multi(json_geom)
-
-                        if isinstance(wkt_feat, list):
-                            out_feats += wkt_feat
-                        else:
-                            out_feats.append(wkt_feat)
-                else:
-                    for plcmark in root.findall('.//{http://www.opengis.net/'
+                    if isinstance(wkt_feat, list):
+                        out_feats += wkt_feat
+                    else:
+                        out_feats.append(wkt_feat)
+            else:
+                for plcmark in root.findall('.//{http://www.opengis.net/'
                                                 'kml/2.2}Placemark'):
 
-                        # Get geometry type
-                        geom_type = 'Polygon'
-                        for elem in plcmark.findall('*'):
-                            tag = elem.tag.replace('{http://www.opengis.net/'
-                                                   'kml/2.2}', '')
-                            if tag in geom_choices:
-                                geom_type = tag
+                    # Get geometry type
+                    geom_type = 'Polygon'
+                    for elem in plcmark.findall('*'):
+                        tag = elem.tag.replace('{http://www.opengis.net/'
+                                               'kml/2.2}', '')
+                        if tag in geom_choices:
+                            geom_type = tag
 
-                        coord_lst = []
+                    coord_lst = [
+                        coords.text
                         for coords in plcmark.findall(
-                                './/{http://www.opengis.net/kml/2.2}'
-                                'coordinates'):
-                            coord_lst.append(coords.text)
-
-                        json_geom = self.convert_coords(coord_lst, geom_type)
-
-                        wkt_feat = self._split_multi(json_geom)
-
-                        if isinstance(wkt_feat, list):
-                            out_feats += wkt_feat
-                        else:
-                            out_feats.append(wkt_feat)
+                            './/{http://www.opengis.net/kml/2.2}' 'coordinates'
+                        )
+                    ]
+                    json_geom = self.convert_coords(coord_lst, geom_type)
 
-            elif in_src.find('.json') > -1 or in_src.find('.geojson') > -1:
-                with open(in_src) as f:
-                    data = json.load(f)
-
-                feats = data['features']
-                for f in feats:
-
-                    wkt_feat = self._split_multi(f['geometry'])
+                    wkt_feat = self._split_multi(json_geom)
 
                     if isinstance(wkt_feat, list):
                         out_feats += wkt_feat
                     else:
                         out_feats.append(wkt_feat)
 
-            elif in_src.find('.shp') > -1:
-                msg = "Could not open shapefile. The GDAL Python Package " \
-                      "must be installed to use shapefiles."
-                self.logger.warning(msg)
-                return None
-            # else:
-            #     self.logger.warning(msg)
-            #     return None
+        elif in_src.find('.json') > -1 or in_src.find('.geojson') > -1:
+            with open(in_src) as f:
+                data = json.load(f)
+
+            feats = data['features']
+            for f in feats:
 
+                wkt_feat = self._split_multi(f['geometry'])
+
+                if isinstance(wkt_feat, list):
+                    out_feats += wkt_feat
+                else:
+                    out_feats.append(wkt_feat)
+
+        elif in_src.find('.shp') > -1:
+            msg = "Could not open shapefile. The GDAL Python Package " \
+                      "must be installed to use shapefiles."
+            self.logger.warning(msg)
+            return None
         return out_feats
```

### Comparing `py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/PKG-INFO` & `py-eodms-rapi-1.5.5/py_eodms_rapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-eodms-rapi
-Version: 1.5.4
+Version: 1.5.5
 Summary: EODMS RAPI Client is a Python3 package used to access the REST API service provided by the Earth Observation Data Management System (EODMS) from Natural Resources Canada.
 Home-page: https://py-eodms-rapi.readthedocs.io/en/latest/
 Author: Kevin Ballantyne (Natural Resources Canada)
 Author-email: kevin.ballantyne@nrcan-rncan.gc.ca
 License: LICENSE
 Project-URL: Source, https://github.com/eodms-sgdot/py-eodms-rapi
 Project-URL: Bug Tracker, https://github.com/eodms-sgdot/py-eodms-rapi/issues
```

### Comparing `py-eodms-rapi-1.5.4/setup.cfg` & `py-eodms-rapi-1.5.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 792d 656f 646d 732d 7261 7069   = py-eodms-rapi
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 340d 0a61 7574 686f 7220 3d20 4b65 7669  4..author = Kevi
+00000030: 350d 0a61 7574 686f 7220 3d20 4b65 7669  5..author = Kevi
 00000040: 6e20 4261 6c6c 616e 7479 6e65 2028 4e61  n Ballantyne (Na
 00000050: 7475 7261 6c20 5265 736f 7572 6365 7320  tural Resources 
 00000060: 4361 6e61 6461 290d 0a61 7574 686f 725f  Canada)..author_
 00000070: 656d 6169 6c20 3d20 6b65 7669 6e2e 6261  email = kevin.ba
 00000080: 6c6c 616e 7479 6e65 406e 7263 616e 2d72  llantyne@nrcan-r
 00000090: 6e63 616e 2e67 632e 6361 0d0a 6465 7363  ncan.gc.ca..desc
 000000a0: 7269 7074 696f 6e20 3d20 454f 444d 5320  ription = EODMS
```

### Comparing `py-eodms-rapi-1.5.4/setup.py` & `py-eodms-rapi-1.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='py-eodms-rapi',
-    version='1.5.4', 
+    version='1.5.5', 
     author='Kevin Ballantyne (Natural Resources Canada)',
     author_email='kevin.ballantyne@nrcan-rncan.gc.ca',
     packages=find_packages(),
     include_package_data=True, 
     url='https://py-eodms-rapi.readthedocs.io/en/latest/',
     license='LICENSE',
     description='EODMS RAPI Client is a Python3 package used to access the REST API service provided by the Earth Observation Data Management System (EODMS) from Natural Resources Canada.',
```

### Comparing `py-eodms-rapi-1.5.4/test/test_pyeodmsrapi.py` & `py-eodms-rapi-1.5.5/test/test_pyeodmsrapi.py`

 * *Files identical despite different names*

