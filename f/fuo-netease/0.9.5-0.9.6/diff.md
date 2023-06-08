# Comparing `tmp/fuo_netease-0.9.5.tar.gz` & `tmp/fuo_netease-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuo_netease-0.9.5.tar", last modified: Thu Apr 27 07:21:30 2023, max compression
+gzip compressed data, was "fuo_netease-0.9.6.tar", last modified: Thu Jun  8 05:22:53 2023, max compression
```

## Comparing `fuo_netease-0.9.5.tar` & `fuo_netease-0.9.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/fuo_netease/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23986 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/fuo_netease/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/assets/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/fuo_netease/cloud_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/cloud_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/cloud_helpers/cloud_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/cloud_helpers/security.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/excs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/login_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/nem.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/page_daily_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/page_explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/page_fav.py
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/fuo_netease/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/fuo_netease.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 07:21:30.000000 fuo_netease-0.9.5/fuo_netease.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-27 07:21:30.000000 fuo_netease-0.9.5/fuo_netease.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:21:30.000000 fuo_netease-0.9.5/fuo_netease.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 07:21:30.000000 fuo_netease-0.9.5/fuo_netease.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 07:21:30.000000 fuo_netease-0.9.5/fuo_netease.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 07:21:30.000000 fuo_netease-0.9.5/fuo_netease.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 07:21:30.689865 fuo_netease-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 07:21:28.000000 fuo_netease-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/fuo_netease/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/fuo_netease/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/assets/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/fuo_netease/cloud_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/cloud_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/cloud_helpers/cloud_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/cloud_helpers/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/excs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/login_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/nem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/page_daily_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/page_explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/page_fav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/fuo_netease.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-08 05:22:53.000000 fuo_netease-0.9.6/fuo_netease.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-08 05:22:53.000000 fuo_netease-0.9.6/fuo_netease.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:22:53.000000 fuo_netease-0.9.6/fuo_netease.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 05:22:53.000000 fuo_netease-0.9.6/fuo_netease.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-08 05:22:53.000000 fuo_netease-0.9.6/fuo_netease.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 05:22:53.000000 fuo_netease-0.9.6/fuo_netease.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/setup.py
```

### Comparing `fuo_netease-0.9.5/PKG-INFO` & `fuo_netease-0.9.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuo_netease
-Version: 0.9.5
+Version: 0.9.6
 Summary: feeluown netease plugin
 Home-page: https://github.com/feeluown/feeluown-netease
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: feeluown,plugin,netease
```

### Comparing `fuo_netease-0.9.5/README.md` & `fuo_netease-0.9.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 ## 安装
 
 ```sh
 pip3 install fuo-netease
 ```
 
 ## changelog
+
+### 0.9.6 (2023-06-08)
+- 移除对 feeluown.models 的依赖
+
 ### 0.9.5 (2023-04-27)
 - 提供双语歌词
 
 ### 0.9.4 (2023-03-27)
 - 提供专辑发布日期数据
 - 优化登陆时错误处理
```

### Comparing `fuo_netease-0.9.5/fuo_netease/__init__.py` & `fuo_netease-0.9.6/fuo_netease/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.5/fuo_netease/api.py` & `fuo_netease-0.9.6/fuo_netease/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,15 +384,14 @@
         data_add = {
             'tracks': str(mid),  # music id
             'pid': str(pid),    # playlist id
             'trackIds': trackIds,  # music id str
             'op': op   # opation
         }
         data = self.request('POST', url_add, data_add)
-        print(data)
         code = data.get('code')
 
         # 从歌单中成功的移除歌曲时，code 是 200
         # 当从歌单中移除一首不存在的歌曲时，code 也是 200
         # 当向歌单添加歌曲时，如果歌曲已经在列表当中，返回 code 为 502
         # code 为 521 时，可能是因为：绑定手机号后才可操作哦
         if code == 200:
@@ -460,15 +459,14 @@
             return data['songs']
         raise CodeShouldBe200(data)
 
     def get_recommend_songs(self):
         url = uri_v3 + '/discovery/recommend/songs'
         payload = self.encrypt_request({})
         res_data = self.request('POST', url, payload)
-        print(res_data)
         if res_data['code'] == 200:
             return res_data['data']['dailySongs']
         raise CodeShouldBe200(res_data)
 
     def get_recommend_playlists(self):
         url = uri + '/discovery/recommend/resource'
         payload = self.encrypt_request({})
@@ -676,9 +674,10 @@
 
 api = API()
 
 
 if __name__ == '__main__':
     from fuo_netease.login_controller import LoginController
     user = LoginController.load()
-    api.load_cookies(user.cookies)
+    cookies, _ = user.cache_get('cookies')
+    api.load_cookies(cookies)
     print(api.djradio_song_detail(1883706033))
```

### Comparing `fuo_netease-0.9.5/fuo_netease/assets/icon.svg` & `fuo_netease-0.9.6/fuo_netease/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.5/fuo_netease/cloud_helpers/__init__.py` & `fuo_netease-0.9.6/fuo_netease/cloud_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.5/fuo_netease/cloud_helpers/cloud_api.py` & `fuo_netease-0.9.6/fuo_netease/cloud_helpers/cloud_api.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.5/fuo_netease/cloud_helpers/security.py` & `fuo_netease-0.9.6/fuo_netease/cloud_helpers/security.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.5/fuo_netease/downloader.py` & `fuo_netease-0.9.6/fuo_netease/downloader.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.5/fuo_netease/login_controller.py` & `fuo_netease-0.9.6/fuo_netease/login_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import json
 import logging
 import os
 
+from feeluown.library import BriefUserModel
 from .api import api
-from .schemas import NeteaseUserSchema
-from .models import _deserialize
 from .consts import USERS_INFO_FILE
 
 logger = logging.getLogger(__name__)
 
 
 def create_user(identifier, name, cookies):
-    user = _deserialize(dict(
-        id=int(identifier),
+    user = BriefUserModel(
+        source='netease',
+        identifier=identifier,
         name=name,
-        cookies=cookies,
-    ), NeteaseUserSchema)
+    )
+    user.cache_set('cookies', cookies)
     return user
 
 
 class LoginController(object):
     _api = api
 
     def __init__(self, username, uid, name, img):
@@ -73,15 +73,15 @@
     @classmethod
     def save(cls, user):
         with open(USERS_INFO_FILE, 'w+') as f:
             data = {
                 user.name: {
                     'uid': user.identifier,
                     'name': user.name,
-                    'cookies': user.cookies
+                    'cookies': user.cache_get('cookies')[0]
                 }
             }
             if f.read() != '':
                 data.update(json.load(f))
             json.dump(data, f, indent=4)
 
     @classmethod
```

### Comparing `fuo_netease-0.9.5/fuo_netease/nem.py` & `fuo_netease-0.9.6/fuo_netease/nem.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import logging
 
 from PyQt5.QtCore import QObject
 
+from feeluown.utils import aio
 from .excs import NeteaseIOError
 from .provider import provider
 from .login_controller import LoginController
 from .ui import LoginDialog
 
 
 logger = logging.getLogger(__name__)
@@ -41,15 +42,17 @@
     def ready_to_login(self):
         if self._user is not None:
             logger.debug('You have already logined in.')
             asyncio.ensure_future(self.login_as(self._user))
             return
         logger.debug('Trying to load last login user...')
         user = LoginController.load()
-        if user is None or 'MUSIC_U' not in user.cookies:
+        cookies, exists = user.cache_get('cookies')
+        assert exists
+        if user is None or 'MUSIC_U' not in cookies:
             logger.debug('Trying to load last login user...failed')
             self.login_dialog.show()
             self.login_dialog.load_user_pw()
             self.login_dialog.login_success.connect(
                 lambda user: asyncio.ensure_future(self.login_as(user)))
         else:
             logger.debug('Trying to load last login user...done')
@@ -75,22 +78,20 @@
             weak=False)
 
         self._app.mymusic_uimgr.clear()
         self._app.mymusic_uimgr.add_item(mymusic_explore_item)
         self._app.mymusic_uimgr.add_item(mymusic_fm_item)
         self._app.mymusic_uimgr.add_item(mymusic_fav_item)
 
-        loop = asyncio.get_event_loop()
-        playlists = await loop.run_in_executor(None, lambda: user.playlists)
+        playlists, fav_playlists = await aio.run_fn(provider.current_user_playlists)
         self._app.pl_uimgr.clear()
         self._app.pl_uimgr.add(playlists)
-        self._app.pl_uimgr.add(user.fav_playlists, is_fav=True)
-        # self._app.pl_uimgr.add(user.rec_playlists)
+        self._app.pl_uimgr.add(fav_playlists, is_fav=True)
 
     def activate_fm(self):
         self._app.fm.activate(self.fetch_fm_songs)
 
     def fetch_fm_songs(self, *args, **kwargs):
-        songs = provider._user.get_radio()  # noqa
+        songs = provider.current_user_get_radio_songs()  # noqa
         if songs is None:
             raise NeteaseIOError('unknown error: get no radio songs')
         return songs
```

### Comparing `fuo_netease-0.9.5/fuo_netease/page_daily_recommendation.py` & `fuo_netease-0.9.6/fuo_netease/page_daily_recommendation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from feeluown.utils import aio
 from feeluown.gui.page_containers.table import Renderer
 
+from fuo_netease import provider
+
 
 async def render(req, **kwargs):
     app = req.ctx['app']
-    provider = app.library.get('netease')
     user = provider._user
 
     app.ui.right_panel.set_body(app.ui.right_panel.table_container)
     renderer = DailyRecommendationRenderer(user)
     await app.ui.right_panel.table_container.set_renderer(renderer)
 
 
@@ -16,8 +17,8 @@
     def __init__(self, user):
         self._user = user
 
     async def render(self):
         self.meta_widget.title = '每日推荐'
         self.meta_widget.show()
 
-        self.show_songs(await aio.run_fn(lambda: self._user.rec_songs))
+        self.show_songs(await aio.run_fn(lambda: provider.current_user_rec_songs_p))
```

### Comparing `fuo_netease-0.9.5/fuo_netease/page_explore.py` & `fuo_netease-0.9.6/fuo_netease/page_explore.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 from feeluown.utils.reader import wrap
 from feeluown.gui.widgets.playlist import PlaylistListView, PlaylistListModel, \
     PlaylistFilterProxyModel
 from feeluown.gui.widgets.textbtn import TextButton
 from feeluown.gui.helpers import fetch_cover_wrapper, BgTransparentMixin
 
+from fuo_netease import provider
+
 
 async def render(req, **kwargs):
     app = req.ctx['app']
-    provider = app.library.get('netease')
 
-    playlists = provider._user.rec_playlists
+    playlists = provider.current_user_rec_playlists_p
     view = ExploreView()
     view.daily_rec_btn.clicked.connect(
         lambda: app.browser.goto(page='/providers/netease/daily_recommendation'))
     model = PlaylistListModel(wrap(playlists),
                               fetch_cover_wrapper(app),
                               {p.identifier: p.name for p in app.library.list()})
     filter_model = PlaylistFilterProxyModel()
```

### Comparing `fuo_netease-0.9.5/fuo_netease/page_fav.py` & `fuo_netease-0.9.6/fuo_netease/page_fav.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,57 +5,60 @@
 from PyQt5.QtWidgets import QFileDialog, QMessageBox
 from feeluown.gui.widgets import TextButton
 from feeluown.utils import aio
 from feeluown.gui.base_renderer import LibraryTabRendererMixin
 from feeluown.gui.page_containers.table import Renderer
 from feeluown.gui.widgets.tabbar import Tab
 
+from fuo_netease import provider
 
 logger = logging.getLogger(__name__)
 
 
 async def render(req, **kwargs):
     app = req.ctx['app']
     app.ui.right_panel.set_body(app.ui.table_container)
 
-    provider = app.library.get('netease')
     tab_id = Tab(int(req.query.get('tab_id', Tab.songs.value)))
     # FIXM
-    renderer = FavRenderer(tab_id, provider._user)
+    renderer = FavRenderer(tab_id)
     await app.ui.table_container.set_renderer(renderer)
 
 
 class FavRenderer(Renderer, LibraryTabRendererMixin):
-    def __init__(self, tab_id, user):
+    def __init__(self, tab_id):
+        global provider
+
         self.tab_id = tab_id
-        self._user = user
+        self._user = provider._user
 
     async def render(self):
         self.render_tabbar()
         self.meta_widget.show()
         self.meta_widget.title = '收藏与关注'
 
         if self.tab_id == Tab.songs:
-            self.show_songs(await aio.run_fn(lambda: self._user.cloud_songs))
+            self.show_songs(await aio.run_fn(provider.current_user_cloud_songs))
             dir_upload_btn = TextButton('上传目录', self.toolbar)
             dir_upload_btn.clicked.connect(
                 lambda: aio.run_afn(self._upload_cloud_songs_bydir))
             self.toolbar.add_tmp_button(dir_upload_btn)
             upload_btn = TextButton('上传音乐', self.toolbar)
             upload_btn.clicked.connect(lambda: aio.run_afn(self._upload_cloud_songs))
             self.toolbar.add_tmp_button(upload_btn)
             refresh_btn = TextButton('刷新音乐', self.toolbar)
             refresh_btn.clicked.connect(self._refresh_cloud_songs)
             self.toolbar.add_tmp_button(refresh_btn)
         elif self.tab_id == Tab.albums:
-            self.show_albums(await aio.run_fn(lambda: self._user.fav_albums))
+            self.show_albums(await aio.run_fn(provider.current_user_fav_albums))
         elif self.tab_id == Tab.artists:
-            self.show_artists(await aio.run_fn(lambda: self._user.fav_artists))
+            self.show_artists(await aio.run_fn(provider.current_user_fav_artists))
         elif self.tab_id == Tab.playlists:
-            self.show_playlists(await aio.run_fn(lambda: self._user.fav_djradio))
+            playlists = await aio.run_fn(provider.current_user_fav_djradios)
+            self.show_playlists(playlists)
 
     async def _upload_cloud_songs_bydir(self):
         # FIXME: 目前无法根据当前页面进行自动刷新, 只能手动刷新
         # FIXME: 本地音乐还没扫描完成或歌曲播放时, 可能线程错误提示
         root = QFileDialog.getExistingDirectory(
             self.toolbar, '选择文件夹', Path.home().as_posix())
         if root == '':
@@ -91,15 +94,14 @@
             if ok:
                 logger.warning(f'[{idx + 1}/{len(paths)}]{path} 上传成功!')
             else:
                 logger.warning(f'[{idx + 1}/{len(paths)}]{path} 上传失败!')
         QMessageBox.information(self.toolbar, '上传音乐', '上传完成！')
 
     def _refresh_cloud_songs(self):
-        self._user.cloud_songs = None
         self.show_by_tab_id(Tab.songs)
 
     def show_by_tab_id(self, tab_id):
         query = {'tab_id': tab_id.value}
         self._app.browser.goto(page='/providers/netease/fav', query=query)
 
     def render_tabbar(self):
```

### Comparing `fuo_netease-0.9.5/fuo_netease/provider.py` & `fuo_netease-0.9.6/fuo_netease/provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import logging
 
 from feeluown.library import AbstractProvider, ProviderV2, ProviderFlags as PF, \
     CommentModel, BriefCommentModel, BriefUserModel, UserModel, \
     NoUserLoggedIn, LyricModel, ModelNotFound
 from feeluown.media import Quality, Media
-from feeluown.models import ModelType, SearchType
+from feeluown.library import ModelType, SearchType
+from feeluown.utils.cache import cached_field
 from feeluown.utils.reader import create_reader, SequentialReader
 from .api import API
 
 
 logger = logging.getLogger(__name__)
 SOURCE = 'netease'
 
 
 class NeteaseProvider(AbstractProvider, ProviderV2):
     class meta:
         identifier = SOURCE
         name = '网易云音乐'
+        # TODO: remove
         flags = {
             ModelType.song: (PF.model_v2 | PF.similar | PF.multi_quality |
                              PF.get | PF.hot_comments | PF.web_url |
                              PF.lyric | PF.mv),
             ModelType.album: (PF.model_v2 | PF.get),
             ModelType.artist: (PF.model_v2 | PF.get | PF.songs_rd | PF.albums_rd),
             ModelType.video: (PF.model_v2 | PF.get | PF.multi_quality),
@@ -38,17 +40,18 @@
         return SOURCE
 
     @property
     def name(self):
         return '网易云音乐'
 
     def auth(self, user):
-        assert user.cookies is not None
+        cookies, exists = user.cache_get('cookies')
+        assert exists and cookies is not None
         self._user = user
-        self.api.load_cookies(user.cookies)
+        self.api.load_cookies(cookies)
 
     def has_current_user(self):
         return self._user is not None
 
     def get_current_user(self):
         if self._user is None:
             raise NoUserLoggedIn
@@ -59,14 +62,73 @@
         data = self.api.user_profile(identifier)
         user = UserModel(identifier=str(identifier),
                          source=SOURCE,
                          name=data['nickname'],
                          avatar_url=data['avatarImg'])
         return user
 
+    def current_user_fav_djradios(self):
+        return create_g(self.api.subscribed_djradio, NeteaseDjradioSchema, 'djRadios')
+
+    def current_user_fav_artists(self):
+        return create_g(self.api.user_favorite_artists, V2BriefArtistSchema)
+
+    def current_user_fav_albums(self):
+        return create_g(self.api.user_favorite_albums, V2BriefAlbumSchema)
+
+    def current_user_cloud_songs(self):
+        return create_cloud_songs_g(
+            self.api.cloud_songs,
+            self.api.cloud_songs_detail,
+            V2SongSchemaForV3,
+            NCloudSchema,
+            data_key='simpleSong'
+        )
+
+    def current_user_playlists(self):
+        user_id = str(self._user.identifier)
+        data_playlists = self.api.user_playlists(user_id)
+        playlists = []
+        fav_playlists = []
+        for pl in data_playlists:
+            if str(pl['userId']) == user_id:
+                playlists.append(pl)
+            else:
+                fav_playlists.append(pl)
+        return [_deserialize(e, V2PlaylistSchema) for e in playlists], \
+            [_deserialize(e, V2PlaylistSchema) for e in fav_playlists]
+
+    def current_user_get_radio_songs(self):
+        songs_data = self.api.get_radio_music()
+        if songs_data is None:
+            logger.error('data should not be None')
+            return None
+        return [_deserialize(song_data, V2SongSchema)
+                for song_data in songs_data]
+
+    @cached_field()
+    def current_user_rec_playlists_p(self):
+        playlists_data = self.api.get_recommend_playlists()
+        rec_playlists = []
+        for playlist_data in playlists_data:
+            # FIXME: GUI模式下无法显示歌单描述
+            playlist_data['coverImgUrl'] = playlist_data['picUrl']
+            playlist_data['description'] = None
+            playlist = _deserialize(playlist_data, V2PlaylistSchema)
+            rec_playlists.append(playlist)
+        return rec_playlists
+
+    # 根据过去经验，每日推荐歌曲在每天早上 6:00 刷新，
+    # ttl 设置为 60s 是为了能够比较即时的获取今天推荐。
+    @cached_field(ttl=60)
+    def current_user_rec_songs_p(self):
+        songs_data = self.api.get_recommend_songs()
+        return [_deserialize(song_data, V2SongSchemaForV3)
+                for song_data in songs_data]
+
     def song_get(self, identifier):
         data = self.api.song_detail(int(identifier))
         return _deserialize(data, V2SongSchema)
 
     def song_list_similar(self, song):
         songs = self.api.get_similar_song(song.identifier)
         return [_deserialize(song, V2SongSchema) for song in songs]
@@ -240,14 +302,18 @@
         if album_data is None:
             raise ModelNotFound
         description = self.api.album_desc(identifier)
         album_data['description'] = description
         album = _deserialize(album_data, V2AlbumSchema)
         return album
 
+    def album_create_songs_rd(self, album):
+        album_with_songs = self.album_get(album.identifier)
+        return create_reader(album_with_songs.songs)
+
     def artist_get(self, identifier):
         artist_data = self.api.artist_infos(identifier)
         artist = artist_data['artist']
         artist['songs'] = artist_data['hotSongs'] or []
         description = self.api.artist_desc(identifier)
         artist['description'] = description
         artist['aliases'] = []
@@ -284,29 +350,47 @@
             else:
                 cur = 1
                 while True:
                     for album in data['hotAlbums']:
                         # the songs field will always be an empty list,
                         # we set it to None
                         album['songs'] = None
-                        yield _deserialize(album, V2BriefAlbumSchema)
+                        yield _deserialize(album, V2AlbumSchema)
                         cur += 1
                     if data['more']:
                         data = self.api.artist_albums(artist.identifier, offset=cur)
                     else:
                         break
 
         return create_reader(g())
 
     def playlist_get(self, identifier):
         data = self.api.playlist_detail_v3(identifier, limit=0)
         playlist = _deserialize(data, V2PlaylistSchema)
         return playlist
 
+    def djradio_create_songs_rd(self, djradio_id):
+        data = self.api.djradio_list(djradio_id, limit=1, offset=0)
+        count = data.get('count', 0)
+
+        def g():
+            offset = 0
+            per = 50  # speed up first request
+            while offset < count:
+                tracks_data = self.api.djradio_list(
+                    djradio_id, limit=per, offset=offset)
+                for track_data in tracks_data.get('programs', []):
+                    yield _deserialize(track_data, NDjradioSchema)
+                offset += per
+        return create_reader(g())
+
     def playlist_create_songs_rd(self, playlist):
+        if playlist.identifier.startswith(DjradioPrefix):
+            return self.djradio_create_songs_rd(playlist.identifier[len(DjradioPrefix):])
+
         data = self.api.playlist_detail_v3(playlist.identifier, limit=0)
         track_ids = data['trackIds']  # [{'id': 1, 'v': 1}, ...]
         count = len(track_ids)
 
         def g():
             offset = 0
             # 第一次请求应该尽可能快一点，所以这里只获取少量的歌曲。
@@ -354,26 +438,31 @@
         type_type_map = {
             SearchType.so: 1,
             SearchType.al: 10,
             SearchType.ar: 100,
             SearchType.pl: 1000,
         }
         data = provider.api.search(keyword, stype=type_type_map[type_])
+        data['q'] = keyword
         result = _deserialize(data, NeteaseSearchSchema)
-        result.q = keyword
         return result
 
 
 provider = NeteaseProvider()
 
 
-from .models import _deserialize  # noqa
+from .models import _deserialize, create_g, create_cloud_songs_g  # noqa
 from .schemas import (  # noqa
     V2SongSchema,
     V2SongSchemaForV3,
     V2MvSchema,
     V2AlbumSchema,
     V2ArtistSchema,
+    V2BriefArtistSchema,
     V2BriefAlbumSchema,
     V2PlaylistSchema,
+    NeteaseDjradioSchema,
     NeteaseSearchSchema,
+    NDjradioSchema,
+    NCloudSchema,
+    DjradioPrefix,
 )
```

### Comparing `fuo_netease-0.9.5/fuo_netease/schemas.py` & `fuo_netease-0.9.6/fuo_netease/schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from datetime import datetime
 
 from marshmallow import Schema, post_load, fields, EXCLUDE
 
 from feeluown.library import (
     SongModel, BriefAlbumModel, BriefArtistModel, ModelState, BriefSongModel,
     VideoModel, AlbumModel, ArtistModel, PlaylistModel, BriefUserModel,
+    SimpleSearchResult,
 )
 from feeluown.media import Quality, MediaType, Media
 
 logger = logging.getLogger(__name__)
 
 
 class BaseSchema(Schema):
@@ -27,14 +28,15 @@
 
     class Meta:
         unknown = EXCLUDE
 
 
 Schema = BaseSchema
 Unknown = 'Unknown'
+DjradioPrefix = 'djradio_'
 
 
 def create_model(model_cls, data, fields_to_cache=None):
     """
     maybe this function should be provided by feeluown
 
     :param fields_to_cache: list of fields name to be cached
@@ -150,26 +152,28 @@
 class V2AlbumSchema(Schema):
     identifier = fields.Int(required=True, data_key='id')
     name = fields.Str(required=True)
     cover = fields.Str(data_key='picUrl', allow_none=True)
     artists = fields.List(fields.Nested('V2BriefArtistSchema'))
     # 收藏和搜索接口返回的 album 数据中的 songs 为 None
     songs = fields.List(fields.Nested('V2SongSchema'), allow_none=True)
+    song_count = fields.Int(data_key='size')
 
     # Description is fetched seperatelly by `album_desc` API.
     description = fields.Str(missing='')
     released = fields.Int(data_key='publishTime', missing=0)
 
     @post_load
     def create_v2_model(self, data, **kwargs):
         released = data['released']
         if released:
             released_date = datetime.fromtimestamp(released / 1000)
             released_str = released_date.strftime('%Y-%m-%d')
             data['released'] = released_str
+        data['songs'] = data['songs'] or []
         return AlbumModel(**data)
 
 
 class V2ArtistSchema(Schema):
     identifier = fields.Int(required=True, data_key='id')
     name = fields.Str()
     pic_url = fields.Str(data_key='picUrl', allow_none=True)
@@ -200,20 +204,23 @@
             album.name = ''
         return album
 
 
 class NeteaseDjradioSchema(Schema):
     identifier = fields.Int(required=True, data_key='id')
     name = fields.Str(required=True)
-    desc = fields.Str(required=False)
+    description = fields.Str(data_key='desc', required=False)
     cover = fields.Str(required=False, data_key='picUrl')
 
     @post_load
     def create_model(self, data, **kwargs):
-        return NRadioModel(**data)
+        identifier = data['identifier']
+        data['identifier'] = f'{DjradioPrefix}{identifier}'
+        # TODO: set creator properly.
+        return PlaylistModel(**data, creator=None)
 
 
 class NDjradioSchema(Schema):
     # identifier = fields.Int(required=True, data_key='id')
     # title = fields.Str(required=True, data_key='name')
     main_song = fields.Dict(required=True, data_key='mainSong')
     # cover = fields.Str(required=False, data_key='coverUrl')
@@ -282,36 +289,19 @@
     @post_load
     def create_v2_model(self, data, **kwargs):
         if data.get('description') is None:
             data['description'] = ''
         return PlaylistModel(**data)
 
 
-class NeteaseUserSchema(Schema):
-    identifier = fields.Int(required=True, data_key='id')
-    name = fields.Str(required=True)
-    playlists = fields.List(fields.Nested(V2PlaylistSchema))
-    fav_playlists = fields.List(fields.Nested(V2PlaylistSchema))
-    cookies = fields.Dict()
-
-    @post_load
-    def create_model(self, data, **kwargs):
-        return NUserModel(**data)
-
-
 class NeteaseSearchSchema(Schema):
     """搜索结果 Schema"""
+    q = fields.Str()
     songs = fields.List(fields.Nested(V2SongSchema))
-    albums = fields.List(fields.Nested(V2BriefAlbumSchema))
+    albums = fields.List(fields.Nested(V2AlbumSchema))
     artists = fields.List(fields.Nested(V2BriefArtistSchema))
     playlists = fields.List(fields.Nested(V2PlaylistSchema))
 
     @post_load
     def create_model(self, data, **kwargs):
-        return NSearchModel(**data)
-
-
-from .models import (  # noqa
-    NUserModel,
-    NSearchModel,
-    NRadioModel,
-)  # noqa
+        data.pop('source')
+        return SimpleSearchResult(**data)
```

### Comparing `fuo_netease-0.9.5/fuo_netease/ui.py` & `fuo_netease-0.9.6/fuo_netease/ui.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.5/fuo_netease.egg-info/PKG-INFO` & `fuo_netease-0.9.6/fuo_netease.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuo-netease
-Version: 0.9.5
+Version: 0.9.6
 Summary: feeluown netease plugin
 Home-page: https://github.com/feeluown/feeluown-netease
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: feeluown,plugin,netease
```

### Comparing `fuo_netease-0.9.5/fuo_netease.egg-info/SOURCES.txt` & `fuo_netease-0.9.6/fuo_netease.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.5/setup.py` & `fuo_netease-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='fuo_netease',
-    version='0.9.5',
+    version='0.9.6',
     description='feeluown netease plugin',
     author='Cosven',
     author_email='yinshaowen241@gmail.com',
     packages=find_packages(exclude=('tests*',)),
     package_data={
         '': ['assets/*.svg',
              ]
@@ -20,15 +20,15 @@
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3 :: Only',
     ],
     install_requires=[
-        'feeluown>=3.8.10',
+        'feeluown>=3.8.12',
         'beautifulsoup4',
         'pycryptodome',
         'marshmallow>=3.0',
         'requests',
         'mutagen>=1.37',
     ],
     extras_require={
```

