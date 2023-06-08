# Comparing `tmp/fuo-ytmusic-0.1.1.tar.gz` & `tmp/fuo-ytmusic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuo-ytmusic-0.1.1.tar", max compression
+gzip compressed data, was "fuo-ytmusic-0.2.0.tar", last modified: Thu Jun  8 06:28:13 2023, max compression
```

## Comparing `fuo-ytmusic-0.1.1.tar` & `fuo-ytmusic-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,33 @@
--rw-r--r--   0        0        0    35149 2021-12-17 05:40:08.193105 fuo-ytmusic-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      907 2021-12-20 07:13:42.507095 fuo-ytmusic-0.1.1/README.md
--rw-r--r--   0        0        0      562 2021-12-20 07:27:27.893146 fuo-ytmusic-0.1.1/fuo_ytmusic/__init__.py
--rw-r--r--   0        0        0     1549 2021-12-01 05:52:09.231780 fuo-ytmusic-0.1.1/fuo_ytmusic/assets/icon.svg
--rw-r--r--   0        0        0      307 2021-12-02 02:49:13.523928 fuo-ytmusic-0.1.1/fuo_ytmusic/consts.py
--rw-r--r--   0        0        0      239 2021-12-03 03:15:55.642886 fuo-ytmusic-0.1.1/fuo_ytmusic/helpers.py
--rw-r--r--   0        0        0    18526 2021-12-22 10:29:10.286221 fuo-ytmusic-0.1.1/fuo_ytmusic/models.py
--rw-r--r--   0        0        0     3605 2021-12-15 08:22:37.379887 fuo-ytmusic-0.1.1/fuo_ytmusic/page_explore_qml.py
--rw-r--r--   0        0        0     1901 2021-12-02 13:34:00.967442 fuo-ytmusic-0.1.1/fuo_ytmusic/page_fav.py
--rw-r--r--   0        0        0     8441 2022-03-25 06:16:29.802646 fuo-ytmusic-0.1.1/fuo_ytmusic/page_more.py
--rw-r--r--   0        0        0     7579 2021-12-22 11:13:31.531359 fuo-ytmusic-0.1.1/fuo_ytmusic/provider.py
--rw-r--r--   0        0        0      650 2021-12-14 01:26:02.298167 fuo-ytmusic-0.1.1/fuo_ytmusic/qml/dummydata/explore_backend.qml
--rw-r--r--   0        0        0     3940 2021-12-15 08:20:12.257019 fuo-ytmusic-0.1.1/fuo_ytmusic/qml/page_explore.qml
--rw-r--r--   0        0        0     3028 2022-03-25 06:16:29.802646 fuo-ytmusic-0.1.1/fuo_ytmusic/qml/uploader.qml
--rw-r--r--   0        0        0    13911 2022-03-25 06:16:29.802646 fuo-ytmusic-0.1.1/fuo_ytmusic/service.py
--rw-r--r--   0        0        0     6572 2021-12-06 08:08:59.622860 fuo-ytmusic-0.1.1/fuo_ytmusic/timeparse.py
--rw-r--r--   0        0        0     5568 2021-12-22 09:32:34.547734 fuo-ytmusic-0.1.1/fuo_ytmusic/ui.py
--rw-r--r--   0        0        0      841 2022-03-25 06:16:29.804646 fuo-ytmusic-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1805 2022-03-25 06:16:44.368176 fuo-ytmusic-0.1.1/setup.py
--rw-r--r--   0        0        0     1602 2022-03-25 06:16:44.368393 fuo-ytmusic-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:28:13.258767 fuo-ytmusic-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-08 06:28:13.258767 fuo-ytmusic-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:28:13.258767 fuo-ytmusic-0.2.0/fuo_ytmusic/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:28:13.258767 fuo-ytmusic-0.2.0/fuo_ytmusic/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/assets/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18244 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/page_explore_qml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/page_fav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/page_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:28:13.258767 fuo-ytmusic-0.2.0/fuo_ytmusic/qml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:28:13.258767 fuo-ytmusic-0.2.0/fuo_ytmusic/qml/dummydata/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/qml/dummydata/explore_backend.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/qml/page_explore.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/qml/uploader.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    13978 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/timeparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/fuo_ytmusic/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:28:13.258767 fuo-ytmusic-0.2.0/fuo_ytmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-08 06:28:13.000000 fuo-ytmusic-0.2.0/fuo_ytmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-08 06:28:13.000000 fuo-ytmusic-0.2.0/fuo_ytmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:28:13.000000 fuo-ytmusic-0.2.0/fuo_ytmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 06:28:13.000000 fuo-ytmusic-0.2.0/fuo_ytmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 06:28:13.000000 fuo-ytmusic-0.2.0/fuo_ytmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 06:28:13.000000 fuo-ytmusic-0.2.0/fuo_ytmusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 06:28:13.258767 fuo-ytmusic-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-08 06:28:11.000000 fuo-ytmusic-0.2.0/setup.py
```

### Comparing `fuo-ytmusic-0.1.1/LICENSE.txt` & `fuo-ytmusic-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.1.1/fuo_ytmusic/assets/icon.svg` & `fuo-ytmusic-0.2.0/fuo_ytmusic/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.1.1/fuo_ytmusic/models.py` & `fuo-ytmusic-0.2.0/fuo_ytmusic/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,21 @@
 from feeluown.utils.reader import SequentialReader
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.fields import Field
 # noinspection PyProtectedMember
 from pydantic.main import ModelMetaclass
 
 from feeluown.media import Quality
-from feeluown.library import SongModel, VideoModel, ModelState, BriefArtistModel
-from feeluown.models import AlbumModel, AlbumType, ArtistModel, PlaylistModel
+from feeluown.library import (
+    VideoModel, ModelState, BriefArtistModel, BriefUserModel,
+    AlbumModel as AlbumModelV2, BriefSongModel, SongModel as SongModelV2,
+    BriefAlbumModel, ArtistModel as ArtistModelV2, PlaylistModel,
+    BriefPlaylistModel,
+)
+from feeluown.library import AlbumType
 
 from fuo_ytmusic.timeparse import timeparse
 
 
 class AllowOptional(ModelMetaclass):
     def __new__(mcs, name, bases, namespaces, **kwargs):
         annotations = namespaces.get('__annotations__', {})
@@ -34,34 +39,30 @@
         return 'ytmusic'
 
 
 class SearchNestedArtist(BaseModel):
     id: str
     name: str
 
-    def model(self) -> 'YtmusicArtistModel':
-        return YtmusicArtistModel(identifier=self.id or '', source=self.source, name=self.name or '')
-
-    def brief_model(self) -> BriefArtistModel:
+    def v2_brief_model(self) -> BriefArtistModel:
         return BriefArtistModel(identifier=self.id or '', source=self.source, name=self.name or '')
 
 
 class YtmusicArtistsMixin:
     artists: List[SearchNestedArtist]  # 歌手信息
 
-    @property
-    def artists_model(self) -> Optional[List['YtmusicArtistModel']]:
-        if self.artists is not None:
-            return [artist.model() for artist in self.artists]
-        return None
+    def v2_brief_artist_models(self) -> List[BriefArtistModel]:
+        return [artist.v2_brief_model() for artist in (self.artists or [])
+                if artist.id is not None]
 
-    def brief_artists_model(self) -> Optional[List[BriefArtistModel]]:
-        if self.artists is not None:
-            return [artist.brief_model() for artist in self.artists]
-        return None
+    @property
+    def artists_name(self):
+        if self.artists is None:
+            return ''
+        return ' / '.join([a.name for a in self.artists])
 
 
 class SearchNestedThumbnail(BaseModel):
     url: str  # 图片地址
     width: int
     height: int
 
@@ -88,67 +89,109 @@
     @property
     def duration_ms(self) -> int:
         if self.duration is None:
             return 0
         return int(timeparse(self.duration) * 1000)
 
 
+class YtmusicAlbumSong(BaseModel, YtmusicArtistsMixin, YtmusicDurationMixin):
+    title: str
+    album: str
+    videoId: str
+
+    def v2_brief_model(self) -> BriefSongModel:
+        return BriefSongModel(
+            identifier=self.videoId,
+            source=self.source,
+            title=self.title,
+            artists_name=self.artists_name,
+            album_name=self.album,
+            duration_ms=self.duration
+        )
+
+    def v2_model_with_brief_album(self, album: BriefAlbumModel) -> SongModelV2:
+        return SongModelV2(
+            identifier=self.videoId,
+            source=self.source,
+            title=self.title,
+            album=album,
+            artists=self.v2_brief_artist_models(),
+            duration=self.duration_ms,
+        )
+
+
 class YtmusicSearchBase(BaseModel):
     category: str
     resultType: str
 
 
 class YtmusicSearchSong(YtmusicSearchBase, YtmusicCoverMixin, YtmusicArtistsMixin, YtmusicDurationMixin):
     class Album(BaseModel):
         id: str
         name: str
 
-        def model(self) -> 'YtmusicAlbumModel':
-            album = YtmusicAlbumModel(identifier=self.id or '', source=self.source, name=self.name)
+        def model(self) -> BriefAlbumModel:
+            album = BriefAlbumModel(identifier=self.id or '', source=self.source, name=self.name)
             if self.id is None:
                 album.state = ModelState.not_exists
             return album
 
     title: str  # 歌名
     album: Album  # 专辑信息
     feedbackTokens: dict
     videoId: str  # 歌曲ID
     isAvailable: bool
     isExplicit: bool
 
-    def model(self, album: 'AlbumInfo' = None, artists=None) -> 'YtmusicSongModel':
-        artists_ = self.brief_artists_model()
-        if artists_ is None and artists is not None:
-            artists_ = artists
-        song = YtmusicSongModel(identifier=self.videoId or '', source=self.source, title=self.title,
-                                artists=artists_ or [], duration=self.duration_ms)
-        if self.album is not None:
-            song.album = self.album.model()
+    def v2_brief_model(self) -> BriefSongModel:
+        song = BriefSongModel(
+            identifier=self.videoId or '',
+            source=self.source,
+            title=self.title,
+            artists_name=self.artists_name,
+            album_name=self.album.name if self.album else '',
+            duration_ms=self.duration
+        )
+        if not song.identifier:
+            song.state = ModelState.not_exists
+        return song
+
+    def v2_model(self) -> SongModelV2:
+        if self.album:
+            album = self.album.model()
         else:
-            if album is not None:
-                # noinspection PyProtectedMember
-                song.album = album._model()
-            else:
-                song.album = YtmusicAlbumModel(identifier='', source=self.source, name='', state=ModelState.not_exists)
-        if self.videoId is None:
+            album = None
+        song = SongModelV2(
+            identifier=self.videoId or '',
+            source=self.source,
+            title=self.title,
+            artists=self.v2_brief_artist_models(),
+            album=album,
+            duration=self.duration_ms,
+            pic_url=self.cover or '',
+        )
+        if not song.identifier:
             song.state = ModelState.not_exists
         return song
 
 
+class YtmusicWatchPlaylistSong(YtmusicSearchSong):
+    year: str  # This field exists in get_watch_playlist API.
+
+    def v2_model(self) -> SongModelV2:
+        song = super().v2_model()
+        song.date = self.year or ''
+        return song
+
+
 class YtmusicLibrarySong(YtmusicSearchSong):
     likeStatus: str  # LIKE
     setVideoId: str
     entityId: str
 
-    def model(self, album: 'AlbumInfo' = None, artists=None) -> 'YtmusicSongModel':
-        song = super().model(album, artists)
-        song.setVideoId = self.setVideoId
-        song.entityId = self.entityId
-        return song
-
 
 class YtmusicHistorySong(YtmusicLibrarySong):
     played: str  # 上次播放 eg November 2021
 
 
 class YtmusicSearchAlbum(YtmusicSearchBase, YtmusicCoverMixin, YtmusicArtistsMixin):
     title: str  # 专辑名
@@ -159,53 +202,67 @@
 
     @property
     def album_type(self) -> AlbumType:
         if self.type == 'Single':
             return AlbumType.single
         return AlbumType.standard
 
-    def model(self) -> 'YtmusicAlbumModel':
-        return YtmusicAlbumModel(identifier=self.browseId, source=self.source, name=self.title, type=self.album_type,
-                                 cover=self.cover, artists=self.artists_model)
+    def v2_brief_model(self) -> BriefAlbumModel:
+        return BriefAlbumModel(
+            identifier=self.browseId,
+            source=self.source,
+            name=self.title,
+            artists_name=self.artists_name,
+        )
 
 
 class YtmusicSearchArtist(YtmusicSearchBase, YtmusicCoverMixin):
     artist: str  # 歌手名
     shuffleId: str
     radioId: str
     browseId: str  # 查询ID
 
-    def model(self) -> 'YtmusicArtistModel':
-        return YtmusicArtistModel(identifier=self.browseId, source=self.source, name=self.artist,
-                                  cover=self.cover or '')
+    def v2_brief_model(self) -> BriefArtistModel:
+        return BriefArtistModel(identifier=self.browseId, source=self.source, name=self.artist)
 
 
 class YtmusicLibraryArtist(YtmusicSearchArtist):
     subscribers: str  # 歌曲数量
 
 
 class YtmusicSearchPlaylist(YtmusicSearchBase, YtmusicCoverMixin):
     title: str  # 歌单名
-    itemCount: int  # 歌曲数量
+    itemCount: Optional[int]  # 歌曲数量
     author: str  # 歌单作者
     browseId: str  # 查询ID
 
-    def model(self) -> 'YtmusicPlaylistModel':
-        return YtmusicPlaylistModel(identifier=self.browseId, source=self.source, name=self.title, cover=self.cover)
+    def v2_brief_model(self) -> BriefPlaylistModel:
+        return BriefPlaylistModel(
+            identifier=self.browseId,
+            source=self.source,
+            name=self.title,
+            creator_name=self.author or '',
+        )
 
 
 class YtmusicSearchVideo(YtmusicSearchBase, YtmusicCoverMixin, YtmusicArtistsMixin, YtmusicDurationMixin):
     title: str  # 视频标题
     views: str  # 播放量 eg:13K
     videoId: str  # 视频ID
     playlistId: str
 
-    def model(self) -> VideoModel:
-        return VideoModel(identifier=self.videoId, source=self.source, title=self.title, cover=self.cover,
-                          artists=self.artists_model, duration=self.duration_ms)
+    def v2_model(self) -> VideoModel:
+        return VideoModel(
+            identifier=self.videoId,
+            source=self.source,
+            title=self.title,
+            cover=self.cover,
+            artists=self.v2_brief_artist_models(),
+            duration=self.duration_ms
+        )
 
 
 class YtmusicDispatcher:
     RESULT_TYPE_MAP = {
         'video': YtmusicSearchVideo,
         'song': YtmusicSearchSong,
         'artist': YtmusicSearchArtist,
@@ -213,15 +270,15 @@
         'playlist': YtmusicSearchPlaylist,
     }
 
     @classmethod
     def search_result_dispatcher(cls, **data) \
             -> Union[YtmusicSearchBase, YtmusicSearchVideo, YtmusicSearchSong, YtmusicSearchArtist, YtmusicSearchAlbum,
                      YtmusicSearchPlaylist]:
-        clazz = cls.RESULT_TYPE_MAP.get(data.get('resultType'))
+        clazz = cls.RESULT_TYPE_MAP.get(data.get('resultType') or '')
         return clazz(**data) if clazz is not None else YtmusicSearchBase(**data)
 
 
 class ArtistInfo(BaseModel):
     class Songs(BaseModel):
         browseId: str  # 查询ID
         results: List[YtmusicSearchSong]  # 歌曲列表（部分）
@@ -249,44 +306,67 @@
     thumbnails: List[SearchNestedThumbnail]  # 封面信息
     songs: Songs
     albums: Albums  # 专辑
     singles: Albums  # 单曲专辑
     videos: Videos
     related: RelatedArtists
 
+    def v2_model(self, identifier) -> ArtistModelV2:
+        # Note that the channelId is different from the identifier.
+        # Though the channelId also refers to the artist,
+        # it's songs is a empty list.
+        return ArtistModelV2(
+            identifier=identifier,
+            source=self.source,
+            name=self.name,
+            pic_url=(self.thumbnails[0].url if self.thumbnails else ''),
+            aliases=[],
+            hot_songs=[],
+            description=self.description or '',
+        )
+
 
 class AlbumInfo(BaseModel, YtmusicArtistsMixin, YtmusicCoverMixin):
     title: str  # 专辑名
     type: str
     year: str
     trackCount: int
     duration: str  # eg.5 minutes, 14 seconds
     audioPlaylistId: str
-    tracks: List[YtmusicSearchSong]  # 专辑歌曲
-
-    def _model(self, id_: str = None):
-        return YtmusicAlbumModel(identifier=id_, source=self.source, name=self.title, type=self.type, cover=self.cover)
-
-    def model(self, id_: str = None) -> 'YtmusicAlbumModel':
-        result = self._model(id_)
-        artists = self.artists_model
-        result.songs = [track.model(album=self, artists=artists) for track in self.tracks]
-        result.artists = self.artists_model
-        return result
+    tracks: List[YtmusicAlbumSong]  # 专辑歌曲
+    # ytmusicapi.get_album has this field. Not sure if other api has this field.
+    description: str = ''
+
+    def v2_model_with_identifier(self, identifier) -> AlbumModelV2:
+        brief_album = BriefAlbumModel(
+            identifier=identifier,
+            source=self.source,
+            name=self.title,
+            artists_name=self.artists_name,
+        )
+        return AlbumModelV2(
+            identifier=identifier,
+            source=self.source,
+            name=self.title,
+            cover=self.cover,
+            songs=[t.v2_model_with_brief_album(brief_album) for t in self.tracks],
+            artists=self.v2_brief_artist_models(),
+            description=self.description,
+            released=self.year,
+        )
 
 
 class SongInfo(BaseModel):
     class VideoDetails(BaseModel):
         class Thumbnails(BaseModel, YtmusicCoverMixin):
             pass
 
         videoId: str
         title: str
         lengthSeconds: int
-        lengthSeconds: int
         channelId: str
         isOwnerViewing: bool
         isCrawlable: bool
         thumbnail: Thumbnails
         averageRating: float
         allowRatings: bool
         viewCount: int
@@ -374,16 +454,21 @@
         return None
 
 
 class PlaylistNestedResult(BaseModel, YtmusicCoverMixin):
     title: str
     playlistId: str
 
-    def model(self) -> 'YtmusicPlaylistModel':
-        return YtmusicPlaylistModel(identifier=self.playlistId, source=self.source, name=self.title, cover=self.cover)
+    def v2_brief_model(self) -> BriefPlaylistModel:
+        return BriefPlaylistModel(
+            identifier=self.playlistId,
+            source=self.source,
+            name=self.title,
+            creator_name='',
+        )
 
 
 class UserInfo(BaseModel):
     class Playlists(BaseModel):
         browseId: str
         results: List[PlaylistNestedResult]
         params: str
@@ -430,27 +515,40 @@
     class Author(BaseModel):
         id: str
         name: str
 
     id: str
     privacy: str  # PUBLIC
     title: str  # 歌单名
-    description: str
+    description: Optional[str]
     author: Author
     year: int
     duration: str
     trackCount: int
     tracks: List[YtmusicLibrarySong]
     fetched_tracks: set = Field(default_factory=set)
 
-    def model(self) -> 'YtmusicPlaylistModel':
-        return YtmusicPlaylistModel(identifier=self.id, source=self.source, name=self.title, cover=self.cover,
-                                    desc=self.description or '')
+    def v2_model(self):
+        creator = None
+        if self.author is not None and self.author.id is not None:
+            creator = BriefUserModel(
+                identifier=self.author.id,
+                source=self.source,
+                name=self.author.name or '',
+            )
+        return PlaylistModel(
+            identifier=self.id,
+            source=self.source,
+            name=self.title,
+            cover=self.cover,
+            description=self.description or '',
+            creator=creator
+        )
 
-    def reader(self, provider, playlist=None) -> SequentialReader:
+    def reader(self, provider) -> SequentialReader:
         total_count = self.trackCount
         self.fetched_tracks = set()
 
         def g():
             counter = 0
             offset = 0
             per = 50
@@ -458,20 +556,16 @@
                 end = min(offset + per, total_count)
                 data: PlaylistInfo = provider.service.playlist_info(self.id, limit=end)
                 tracks_data = data.tracks
                 for track_data in tracks_data:
                     if track_data.videoId is not None and track_data.videoId in self.fetched_tracks:
                         continue
                     self.fetched_tracks.add(track_data.videoId)
-                    if playlist is not None and track_data.setVideoId is not None:
-                        if playlist.set_id_map is None:
-                            playlist.set_id_map = dict()
-                        playlist.set_id_map[track_data.videoId] = track_data.setVideoId
                     counter += 1
-                    yield track_data.model()
+                    yield track_data.v2_brief_model()
                 if counter >= total_count:
                     break
                 offset += per
             self.fetched_tracks.clear()
 
         return SequentialReader(g(), total_count)
 
@@ -483,80 +577,14 @@
 
     status: str  # STATUS_SUCCEEDED STATUS_FAILED
     playlistEditResults: List[PlaylistEditResult]
 
 
 # FeelUOwn models
 
-class YtmusicSongModel(SongModel):
+class YtmusicSongModel(SongModelV2):
     setVideoId: Optional[str]
     entityId: Optional[str]
 
 
-class YtmusicPlaylistModel(PlaylistModel):
-    provider = None
-
-    class Meta:
-        fields = ['source', 'set_id_map']
-        allow_create_songs_g = True
-
-    @classmethod
-    def get(cls, identifier: str) -> 'YtmusicPlaylistModel':
-        return cls.provider.playlist_info(identifier)
-
-    def create_songs_g(self):
-        playlist: PlaylistInfo = self.provider.service.playlist_info(self.identifier)
-        return playlist.reader(self.provider, self)
-
-    def add(self, song_id):
-        if self.identifier == 'LM':
-            return False
-        return self.provider.add_playlist_item(self.identifier, song_id)
-
-    def remove(self, song_id):
-        if self.identifier == 'LM':
-            return False
-        if self.set_id_map is None:
-            return False
-        set_id = self.set_id_map.get(song_id)
-        if set_id is None:
-            return False
-        return self.provider.remove_playlist_item(self.identifier, song_id, set_id)
-
-
-class YtmusicAlbumModel(AlbumModel):
-    provider = None
-
-    class Meta:
-        fields = ['source']
-
-    @classmethod
-    def get(cls, identifier: str) -> 'YtmusicAlbumModel':
-        return cls.provider.album_info(identifier)
-
-
-class YtmusicArtistModel(ArtistModel):
-    provider = None
-
-    class Meta:
-        fields = ['source']
-        allow_create_songs_g = True
-
-    @classmethod
-    def get(cls, identifier: str) -> 'YtmusicArtistModel':
-        return cls.provider.artist_info(identifier)
-
-    def create_songs_g(self):
-        artist: ArtistInfo = self.provider.service.artist_info(self.identifier)
-        playlist: PlaylistInfo = self.provider.service.playlist_info(artist.songs.browseId)
-        return playlist.reader(self.provider)
-
-    @property
-    def albums(self):
-        artist: ArtistInfo = self.provider.service.artist_info(self.identifier)
-        albums: List[YtmusicSearchAlbum] = self.provider.service.artist_albums(artist.albums.browseId,
-                                                                               artist.albums.params)
-        return [album.model() for album in albums]
-
-    @albums.setter
-    def albums(self, _):
-        pass
+class YtBriefUserModel(BriefUserModel):
+    cookies: dict = {}
```

### Comparing `fuo-ytmusic-0.1.1/fuo_ytmusic/page_explore_qml.py` & `fuo-ytmusic-0.2.0/fuo_ytmusic/page_explore_qml.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import os
 from pathlib import Path
 
 from PyQt5.QtCore import Qt, QUrl, QObject, pyqtProperty, pyqtSlot, pyqtSignal
 from PyQt5.QtQuick import QQuickView
 from PyQt5.QtWidgets import QWidget
 
+from feeluown.library import BriefPlaylistModel
 from feeluown.gui.base_renderer import TabBarRendererMixin
 from fuo_ytmusic import YtmusicProvider
-from fuo_ytmusic.models import YtmusicPlaylistModel
 
 
 class ExploreBackend(QObject):
     categoriesLoaded = pyqtSignal('QVariantList')
     playlistsLoaded = pyqtSignal('QVariantList')
 
     def __init__(self, provider: YtmusicProvider, app):
@@ -41,15 +41,15 @@
 
     @pyqtSlot(str)
     def load_playlists(self, params: str):
         asyncio.ensure_future(self.playlists(params))
 
     @pyqtSlot(str, str, str)
     def goto_playlist(self, playlist_id: str, name: str, cover: str):
-        model = YtmusicPlaylistModel(identifier=playlist_id, source='ytmusic', name=name, cover=cover)
+        model = BriefPlaylistModel(identifier=playlist_id, source='ytmusic', name=name)
         self._app.browser.goto(model=model)
 
     @pyqtProperty(bool, constant=True)
     def is_dark(self) -> bool:
         return self._app.theme_mgr.theme == 'dark'
```

### Comparing `fuo-ytmusic-0.1.1/fuo_ytmusic/page_fav.py` & `fuo-ytmusic-0.2.0/fuo_ytmusic/page_fav.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from feeluown.utils import aio
 from feeluown.gui.base_renderer import LibraryTabRendererMixin
 from feeluown.gui.page_containers.table import Renderer
 from feeluown.gui.widgets.tabbar import Tab
 
-from fuo_ytmusic import YtmusicProvider
+from fuo_ytmusic.provider import YtmusicProvider
 
 logger = logging.getLogger(__name__)
 
 
 async def render(req, **kwargs):
     app = req.ctx['app']
     app.ui.right_panel.set_body(app.ui.table_container)
```

### Comparing `fuo-ytmusic-0.1.1/fuo_ytmusic/page_more.py` & `fuo-ytmusic-0.2.0/fuo_ytmusic/page_more.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.1.1/fuo_ytmusic/provider.py` & `fuo-ytmusic-0.2.0/fuo_ytmusic/provider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 from typing import List, Optional
 
 from feeluown.excs import NoUserLoggedIn
-from feeluown.library import AbstractProvider, ProviderV2, ModelType, ProviderFlags as Pf, SongModel, BriefVideoModel, \
-    BriefUserModel
+from feeluown.library import (
+    AbstractProvider, ProviderV2, ProviderFlags as Pf,
+    SongModel, BriefVideoModel, BriefUserModel, ModelType,
+    BriefPlaylistModel, BriefArtistModel, PlaylistModel, ModelNotFound,
+)
 from feeluown.media import Quality, Media, VideoAudioManifest, MediaType
-from feeluown.models import SearchType, SearchModel, ArtistModel
+from feeluown.library import SearchType, SimpleSearchResult
 from feeluown.library.model_protocol import BriefSongProtocol
-from fuo_netease.models import NSearchModel
 from fuo_netease.provider import NeteaseProvider
 
 from fuo_ytmusic.consts import HEADER_FILE
-from fuo_ytmusic.models import YtmusicPlaylistModel, Categories, YtmusicAlbumModel, YtmusicArtistModel
+from fuo_ytmusic.models import Categories, YtBriefUserModel, YtmusicWatchPlaylistSong
 from fuo_ytmusic.service import YtmusicService, YtmusicType, YtmusicPrivacyStatus
 
 
 class YtmusicProvider(AbstractProvider, ProviderV2):
-    service: YtmusicService
 
-    def __init__(self, app=None):
+    def __init__(self):
         super(YtmusicProvider, self).__init__()
-        self.service: YtmusicService = YtmusicService(app.config if app is not None else None)
+        self.service: YtmusicService = YtmusicService()
         self._user = None
-        self._app = app
-        YtmusicPlaylistModel.provider = self
-        YtmusicAlbumModel.provider = self
-        YtmusicArtistModel.provider = self
+        self._http_proxy = ''
+
+    def setup_http_proxy(self, http_proxy):
+        self._http_proxy = http_proxy
+        self.service.setup_http_proxy(http_proxy)
 
     # noinspection PyPep8Naming
     class meta:
         identifier = 'ytmusic'
         name = 'YouTube Music'
-        flags = {
-            ModelType.song: (Pf.model_v2 | Pf.multi_quality | Pf.mv | Pf.lyric),
-            ModelType.video: Pf.multi_quality,
-            ModelType.album: Pf.get,
-            ModelType.artist: Pf.get,
-        }
 
     @property
     def identifier(self):
         return self.meta.identifier
 
     @property
     def name(self):
@@ -47,51 +43,59 @@
 
     @property
     def user(self):
         return self._user
 
     @user.setter
     def user(self, user):
-        self.service.setup()
+        self.service.reload()
         self._user = user
 
-    def library_songs(self):
-        songs = self.service.library_songs(100)
-        return [song.model() for song in songs]
+    def use_model_v2(self, mtype):
+        return mtype in (
+            ModelType.song,
+            ModelType.album,
+            ModelType.artist,
+            ModelType.playlist,
+        )
 
     def library_upload_songs(self):
         songs = self.service.library_upload_songs(100)
         return [song.model() for song in songs]
 
     def library_upload_artists(self):
         artists = self.service.library_upload_artists(100)
         return [artist.model() for artist in artists]
 
     def library_upload_albums(self):
         albums = self.service.library_upload_albums(100)
         return [album.model() for album in albums]
 
+    def library_songs(self):
+        songs = self.service.library_songs(100)
+        return [song.v2_model() for song in songs]
+
     def library_albums(self):
         albums = self.service.library_albums(100)
-        return [album.model() for album in albums]
+        return [album.v2_brief_model() for album in albums]
 
-    def library_artists(self) -> List[ArtistModel]:
+    def library_artists(self) -> List[BriefArtistModel]:
         artists = self.service.library_subscription_artists(100)
-        return [artist.model() for artist in artists]
+        return [artist.v2_brief_model() for artist in artists]
 
-    def library_playlists(self) -> List[YtmusicPlaylistModel]:
+    def library_playlists(self) -> List[BriefPlaylistModel]:
         playlists = self.service.library_playlists(100)
-        return [playlist.model() for playlist in playlists]
+        return [playlist.v2_brief_model() for playlist in playlists]
 
     def create_playlist(self, title: str, description: str, privacy_status: YtmusicPrivacyStatus,
                         video_ids: List[str] = None, source_playlist: str = None) -> bool:
         return self.service.create_playlist(title, description, privacy_status, video_ids, source_playlist)
 
-    def playlist_info(self, identifier) -> YtmusicPlaylistModel:
-        return self.service.playlist_info(identifier, limit=0).model()
+    def playlist_info(self, identifier) -> PlaylistModel:
+        return self.service.playlist_info(identifier, limit=0).v2_model()
 
     def add_playlist_item(self, identifier, song_id) -> bool:
         result = self.service.add_playlist_items(identifier, [song_id])
         return result.status == 'STATUS_SUCCEEDED'
 
     def remove_playlist_item(self, identifier, song_id, set_song_id) -> bool:
         return self.service.remove_playlist_items(identifier, [{
@@ -99,66 +103,141 @@
             'setVideoId': set_song_id,
         }]) == 'STATUS_SUCCEEDED'
 
     def category_playlists(self, params):
         playlists = self.service.category_playlists(params)
         return [p.model() for p in playlists]
 
-    def album_info(self, identifier) -> YtmusicAlbumModel:
-        return self.service.album_info(identifier).model(id_=identifier)
-
     def categories(self) -> List[Categories]:
         return self.service.categories()
 
-    def user_from_cookie(self, _):
-        return BriefUserModel(identifier='', source=self.meta.identifier, name='Me')
+    def user_from_cookie(self, cookies: dict):
+        return YtBriefUserModel(
+            identifier='', source=self.meta.identifier, name='Me',
+            cookies=cookies)
 
     def has_current_user(self) -> bool:
-        return HEADER_FILE.exists()
+        return self._user is not None
 
     def get_current_user(self):
-        if not HEADER_FILE.exists():
+        if not self._user:
             raise NoUserLoggedIn
-        return BriefUserModel(identifier='', source=self.meta.identifier, name='Me')
+        return self._user
 
     def user_get(self, identifier):
         if identifier is None:
             return None
         if identifier == '':
             return BriefUserModel(identifier='', source=self.meta.identifier, name='Me')
         user = self.service.user_info(identifier)
         return BriefUserModel(identifier=identifier, source=self.meta.identifier, name=user.name)
 
     def search(self, keyword, type_, *args, **kwargs):
         type_ = SearchType.parse(type_)
         ytmusic_type = YtmusicType.parse(type_)
         results = self.service.search(keyword, ytmusic_type)
-        model = SearchModel(q=keyword)
-        setattr(model, ytmusic_type.value, [r.model() for r in results])
+        model = SimpleSearchResult(q=keyword)
+        if results:
+            try:
+                results[0].v2_model
+            except AttributeError:
+                models = [r.v2_brief_model() for r in results]
+            else:
+                # Try to use SongModel instead of BriefSongModel,
+                # because there is no way to implement song_get.
+                models = [r.v2_model() for r in results]
+        else:
+            models = []
+        setattr(model, ytmusic_type.value, models)
         return model
 
     def song_list_quality(self, song) -> List[Quality.Audio]:
         id_ = song.identifier
         song_ = self.service.song_info(id_)
         return song_.list_formats() if song_ is not None else []
 
     def song_get_media(self, song: SongModel, quality: Quality.Audio) -> Optional[Media]:
         song_info = self.service.song_info(song.identifier)
         format_code, bitrate, format_str = song_info.get_media(quality)
         url = self.service.stream_url(song.identifier, format_code)
-        return Media(url, type_=MediaType.audio, bitrate=bitrate, format=format_str) if url is not None else None
+        if url is not None:
+            return Media(url, type_=MediaType.audio, bitrate=bitrate,
+                         format=format_str, http_proxy=self._http_proxy)
+        return None
+
+    def song_get(self, identifier):
+        # ytmusicapi has not api to get song detail.
+        # hack(cosven): we use get_watch_playlist to try to get song detail.
+        # It works for song like '如愿-王菲'.
+        result = self.service.api.get_watch_playlist(identifier)
+        songs = [YtmusicWatchPlaylistSong(**track).v2_model()
+                 for track in result['tracks']]
+        for song in songs:
+            if song.identifier == identifier:
+                return song
+        # I think this branch should not be reached (in most cases).
+        return ModelNotFound(f'song:{identifier} not found')
+
+    def album_get(self, identifier):
+        album_info = self.service.album_info(identifier)
+        return album_info.v2_model_with_identifier(identifier)
+
+    def artist_get(self, identifier):
+        return self.service.artist_info(identifier).v2_model(identifier)
+
+    def playlist_get(self, identifier):
+        return self.service.playlist_info(identifier).v2_model()
+
+    def playlist_create_songs_rd(self, playlist):
+        playlist_info = self.service.playlist_info(playlist.identifier)
+        return playlist_info.reader(self)
+
+    def playlist_add_song(self, playlist, song):
+        if playlist.identifier == 'LM':
+            return False
+        return self.add_playlist_item(playlist.identifier, song.identifier)
+
+    # playlist.set_id_map is not currently maintained.
+    #
+    # def playlist_remove_song(self, playlist, song):
+    #     song_id = song.identifier
+    #     if playlist.identifier == 'LM':
+    #         return False
+    #     set_id = playlist.set_id_map.get(song_id)
+    #     if set_id is None:
+    #         return False
+    #     return self.remove_playlist_item(self.identifier, song_id, set_id)
+
+    def artist_create_songs_rd(self, artist):
+        artist_info = self.service.artist_info(artist.identifier)
+        if artist_info.songs.browseId is None:
+            # results may also be none.
+            # for example: channelId=UCGSXa1Ve1FswQxtwarGi-Vg
+            return [song.v2_model() for song in artist_info.songs.results or []]
+        playlist_info = self.service.playlist_info(artist_info.songs.browseId)
+        return playlist_info.reader(self)
+
+    def artist_create_albums_rd(self, artist):
+        artist_info = self.service.artist_info(artist.identifier)
+        # Sometimes, the artist only has few albums, read them from results.
+        if artist_info.albums.browseId is None:
+            albums = artist_info.albums.results
+        else:
+            albums = self.service.artist_albums(artist_info.albums.browseId,
+                                                artist_info.albums.params)
+        return [album.v2_brief_model() for album in albums]
 
-    def song_get_lyric(self, song):
+    def deprecated_song_get_lyric(self, song):
         # 歌词获取报错的 workaround
         if self._app is None:
             return None
         provider: NeteaseProvider = self._app.library.get('netease')
         if provider is None:
             return None
-        result: NSearchModel = provider.search(f'{song.title} {song.artists_name}', type_=SearchType.so)
+        result = provider.search(f'{song.title} {song.artists_name}', type_=SearchType.so)
         songs = result.songs
         if len(songs) < 1:
             return None
         return provider.song_get_lyric(songs[0])
 
     def video_list_quality(self, video) -> List[Quality.Video]:
         id_ = video.identifier
@@ -170,18 +249,21 @@
         format_code = song_info.get_mv(quality)
         audio_formats = song_info.list_formats()
         audio_code, _, __ = song_info.get_media(audio_formats[0])
         url = self.service.stream_url(video.identifier, format_code)
         audio_url = self.service.stream_url(video.identifier, audio_code)
         if url is None or audio_url is None:
             return None
-        return Media(VideoAudioManifest(url, audio_url))
+        return Media(VideoAudioManifest(url, audio_url), http_proxy=self._http_proxy)
 
     def song_get_mv(self, song: BriefSongProtocol) -> BriefVideoModel:
         return BriefVideoModel(identifier=song.identifier, source=song.source, title=song.title,
                                artists_name=song.artists_name, duration_ms=song.duration_ms)
 
     def upload_song(self, path: str) -> bool:
         return self.service.upload_song(path) == 'STATUS_SUCCEEDED'
 
     def delete_uploaded_song(self, entity_id: str) -> bool:
         return self.service.delete_upload_song(entity_id) == 'STATUS_SUCCEEDED'
+
+
+provider = YtmusicProvider()
```

### Comparing `fuo-ytmusic-0.1.1/fuo_ytmusic/qml/dummydata/explore_backend.qml` & `fuo-ytmusic-0.2.0/fuo_ytmusic/qml/dummydata/explore_backend.qml`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.1.1/fuo_ytmusic/qml/page_explore.qml` & `fuo-ytmusic-0.2.0/fuo_ytmusic/qml/page_explore.qml`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.1.1/fuo_ytmusic/qml/uploader.qml` & `fuo-ytmusic-0.2.0/fuo_ytmusic/qml/uploader.qml`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.1.1/fuo_ytmusic/service.py` & `fuo-ytmusic-0.2.0/fuo_ytmusic/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 import ntpath
+import json
 import os
 import sys
 from datetime import timedelta
 from enum import Enum
 from functools import partial
 from typing import Optional, Union, List
 from urllib.parse import unquote
 
 import cachetools.keys
 import requests
 
-from feeluown.models import SearchType
+from feeluown.library import SearchType
 from pytube.cipher import Cipher
 from requests import Response
 from pytube import extract
 
 from fuo_ytmusic.consts import HEADER_FILE
 from fuo_ytmusic.helpers import Singleton
 from fuo_ytmusic.models import YtmusicSearchSong, YtmusicSearchAlbum, YtmusicSearchArtist, YtmusicSearchVideo, \
@@ -130,59 +131,65 @@
         if response.status_code == 200:
             return 'STATUS_SUCCEEDED'
         else:
             return response
 
 
 class YtmusicService(metaclass=Singleton):
-    def __init__(self, config=None):
-        self._session: Optional[requests.Session] = None
+    def __init__(self):
+        self._session = requests.Session()
         self._api: Optional[YTMusic] = None
         self._js = ""
         self._cipher = None
         self._signature_timestamp = 0
-        self.setup(config)
+        self._session.hooks['response'].append(self._do_logging)
 
     @staticmethod
     def _do_logging(r: Response, *_, **__):
         logger.debug(f'[ytmusic] Requesting: [{r.request.method.upper()}] {r.url}; '
                      f'Response: [{r.status_code}] {len(r.content)} bytes.')
 
     @property
-    def api(self):
+    def api(self) -> YTMusic:
         if self._api is None:
-            logger.info('initializing ytmusic')
-            if HEADER_FILE.exists():
-                self._api = YTMusic(HEADER_FILE, requests_session=self._session, language='zh_CN')
-            else:
-                self._api = YTMusic(requests_session=self._session, language='zh_CN')
-            self._signature_timestamp = self._api.get_signatureTimestamp()
+            self._initialize_by_headerfile()
         return self._api
 
-    def setup(self, config=None):
-        del self._session
-        self._session = requests.Session()
-        if config is not None and hasattr(config, 'YTM_HTTP_PROXY') and config.YTM_HTTP_PROXY != '':
-            self._session.proxies = {
-                'http': 'http://' + config.YTM_HTTP_PROXY,
-                'https': 'http://' + config.YTM_HTTP_PROXY
-            }
-        self._session.hooks['response'].append(self._do_logging)
+    def _initialize_by_headerfile(self):
+        options = dict(requests_session=self._session, language='zh_CN')
+        if HEADER_FILE.exists():
+            logger.info('Initializing ytmusic api with headerfile.')
+            self._api = YTMusic(HEADER_FILE, **options)
+        else:
+            logger.info('Initializing ytmusic api with no headerfile.')
+            # Actually, YTMusic does not work if no auth file is provided.
+            self._api = YTMusic(**options)
+        self._signature_timestamp = self._api.get_signatureTimestamp()
+
+    def reload(self):
+        self._initialize_by_headerfile()
+
+    def setup_http_proxy(self, http_proxy):
+        self._session.proxies = {
+            'http': http_proxy,
+            'https': http_proxy,
+        }
 
     def search(self, keywords: str, t: Optional[YtmusicType], scope: YtmusicScope = None,
                page_size: int = GLOBAL_LIMIT) \
             -> List[Union[YtmusicSearchSong, YtmusicSearchAlbum, YtmusicSearchArtist, YtmusicSearchVideo,
                           YtmusicSearchPlaylist, YtmusicSearchBase]]:
         response = self.api.search(keywords, None if t is None else t.value, None if scope is None else scope.value,
                                    page_size)
         return [YtmusicDispatcher.search_result_dispatcher(**data) for data in response]
 
     @ttl_cache(maxsize=CACHE_SIZE, ttl=CACHE_TTL)
     def artist_info(self, channel_id: str) -> ArtistInfo:
-        return ArtistInfo(**self.api.get_artist(channel_id))
+        data = self.api.get_artist(channel_id)
+        return ArtistInfo(**data)
 
     @ttl_cache(maxsize=CACHE_SIZE, ttl=CACHE_TTL)
     def artist_albums(self, channel_id: str, params: str) -> List[YtmusicSearchAlbum]:
         response = self.api.get_artist_albums(channel_id, params)
         return [YtmusicSearchAlbum(**data) for data in response]
 
     @ttl_cache(maxsize=CACHE_SIZE, ttl=CACHE_TTL)
@@ -190,15 +197,16 @@
         return UserInfo(**self.api.get_user(channel_id))
 
     def user_playlists(self, channel_id: str, params: str):
         return self.api.get_user_playlists(channel_id, params)
 
     @ttl_cache(maxsize=CACHE_SIZE, ttl=CACHE_TTL)
     def album_info(self, browse_id: str) -> AlbumInfo:
-        return AlbumInfo(**self.api.get_album(browse_id))
+        data = self.api.get_album(browse_id)
+        return AlbumInfo(**data)
 
     @ttl_cache(maxsize=CACHE_SIZE, ttl=CACHE_TTL)
     def song_info(self, video_id: str) -> SongInfo:
         return SongInfo(**self.api.get_song(video_id, self._signature_timestamp))
 
     @ttl_cache(maxsize=CACHE_SIZE, ttl=CACHE_TTL)
     def categories(self) -> List[Categories]:
@@ -322,12 +330,11 @@
         js_url = extract.js_url(embed_html)
         self._js = self._session.get(js_url).text
         self._cipher = Cipher(js=self._js)
 
 
 if __name__ == '__main__':
     # noinspection PyUnresolvedReferences
-    import json
 
     service = YtmusicService()
     # print(service.upload_song('/home/bruce/Music/阿梓 - 呼吸决定.mp3'))
     print(service.api.delete_upload_entity('t_po_CJT896eTt_a5swEQwrmdzf7_____AQ'))
```

### Comparing `fuo-ytmusic-0.1.1/fuo_ytmusic/timeparse.py` & `fuo-ytmusic-0.2.0/fuo_ytmusic/timeparse.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.1.1/fuo_ytmusic/ui.py` & `fuo-ytmusic-0.2.0/fuo_ytmusic/ui.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 import asyncio
+import logging
 import json
-import os
 from pathlib import Path
 
 from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import QLabel, QAction, QInputDialog, QMessageBox
+from PyQt5.QtWidgets import QLabel, QAction, QInputDialog, QMessageBox, QTextEdit
+from feeluown.utils import aio
 from feeluown.gui.widgets.login import CookiesLoginDialog
 from feeluown.uimodels.my_music import MyMusicUiManager
 from feeluown.uimodels.playlist import PlaylistUiManager
 from feeluown.uimodels.provider import ProviderUiManager
 
 from fuo_ytmusic.consts import HEADER_FILE, REQUIRED_COOKIE_FIELDS
 
-from .page_explore_qml import render as explore_render
+# QML page has two problems
+# 1. they may block the whole UI.
+# 2. they consumes much memory.
+# from .page_explore_qml import render as explore_render
+# from .page_more import render as more_render
 from .page_fav import render as fav_render
-from .page_more import render as more_render
 from .service import YtmusicPrivacyStatus
 
 
+logger = logging.getLogger(__name__)
+
+
 class YtmusicUiManager:
     def __init__(self, app):
         self._app = app
         self._provider = app.library.get('ytmusic')
         self._pvd_uimgr: ProviderUiManager = app.pvd_uimgr
         self._pvd_item = self._pvd_uimgr.create_item(
             name=self._provider.identifier,
             text=self._provider.name,
             desc=self._provider.name,
             colorful_svg=(Path(__file__).parent / 'assets' / 'icon.svg').as_posix()
         )
         self._pvd_item.clicked.connect(self.login_or_show)
         self._pvd_uimgr.add_item(self._pvd_item)
         self._app.browser.route('/providers/ytmusic/fav')(fav_render)
-        self._app.browser.route('/providers/ytmusic/explore')(explore_render)
-        self._app.browser.route('/providers/ytmusic/more')(more_render)
+        # self._app.browser.route('/providers/ytmusic/explore')(explore_render)
+        # self._app.browser.route('/providers/ytmusic/more')(more_render)
 
     def login_or_show(self):
         if self._provider.user is None:
             dialog = LoginDialog(self._provider)
             dialog.login_succeed.connect(lambda: asyncio.ensure_future(self.load_user()))
-            dialog.show()
+            dialog.open()
             dialog.autologin()
         else:
             asyncio.ensure_future(self.load_user())
 
     def new_playlist(self):
         name, o1 = QInputDialog.getText(self._app.ui.left_panel.playlists_header, '新建歌单', '请输入歌单名称:')
         if not o1:
@@ -74,24 +81,24 @@
         new_pl_action = QAction('新建歌单', pl_header)
         pl_header.addAction(new_pl_action)
         new_pl_action.triggered.connect(self.new_playlist)
 
         mymusic_mgr: MyMusicUiManager = self._app.mymusic_uimgr
         playlists_mgr: PlaylistUiManager = self._app.pl_uimgr
 
-        explore_item = mymusic_mgr.create_item('🔮 发现音乐')
+        # explore_item = mymusic_mgr.create_item('🔮 发现音乐')
         my_fav_item = mymusic_mgr.create_item('⭐️ 收藏与关注')
-        more_item = mymusic_mgr.create_item('☁️ 上传的音乐')
-        explore_item.clicked.connect(lambda: self._app.browser.goto(page='/providers/ytmusic/explore'), weak=False)
+        # more_item = mymusic_mgr.create_item('☁️ 上传的音乐')
+        # explore_item.clicked.connect(lambda: self._app.browser.goto(page='/providers/ytmusic/explore'), weak=False)
         my_fav_item.clicked.connect(lambda: self._app.browser.goto(page='/providers/ytmusic/fav'), weak=False)
-        more_item.clicked.connect(lambda: self._app.browser.goto(page='/providers/ytmusic/more'), weak=False)
+        # more_item.clicked.connect(lambda: self._app.browser.goto(page='/providers/ytmusic/more'), weak=False)
         mymusic_mgr.clear()
-        mymusic_mgr.add_item(explore_item)
+        # mymusic_mgr.add_item(explore_item)
         mymusic_mgr.add_item(my_fav_item)
-        mymusic_mgr.add_item(more_item)
+        # mymusic_mgr.add_item(more_item)
 
         playlists_mgr.clear()
         self._pvd_item.text = f'{user.name} - 已登录'
 
         loop = asyncio.get_event_loop()
         pls = await loop.run_in_executor(None, self._provider.library_playlists)
         playlists_mgr.add(pls)
@@ -99,29 +106,80 @@
 
 class LoginDialog(CookiesLoginDialog):
     def __init__(self, provider):
         super(LoginDialog, self).__init__(uri='https://music.youtube.com/',
                                           required_cookies_fields=REQUIRED_COOKIE_FIELDS)
         self._provider = provider
 
+        self.auth_text_edit = QTextEdit(self)
+        self.auth_text_edit.setAcceptRichText(False)
+        self.auth_text_edit.setPlaceholderText(
+            '请打开 music.youtube.com 并登陆，'
+            '然后从浏览器中复制 HTTP 请求 header 中的 Authorization 字段：\n\n'
+            '它类似这样：SAPISIDHASH 123333333_abfasdfs12fadcdfa2d'
+        )
+        self.__hint_label = QLabel(
+            '还有另外一种登陆方式，你可以参考 ytmusicapi 的使用文档，使用'
+            ' ytmusicapi oauth 命令来生成登陆所需信息。你如果登陆成功，'
+            '它会生成一个 oauth.json 文件，你把 oauth.json 文件移动到'
+            ' ~/.FeelUOwn/data/ytmusic_header.json ，然后重新点击图标登陆即可。'
+        )
+        self.__hint_label.setWordWrap(True)
+        # weblogin can't fetch the authorization field, so diable it.
+        self.weblogin_btn.hide()
+        self._layout.insertWidget(0, self.auth_text_edit)
+        self._layout.addWidget(self.__hint_label)
+        self.setWindowFlags(self.windowFlags() | Qt.Dialog)
+
     def setup_user(self, user):
         self._provider.user = user
 
+    def get_cookies(self):
+        cookie = self.cookies_text_edit.toPlainText()
+        auth = self.auth_text_edit.toPlainText()
+        if not auth or not cookie:
+            self.show_hint(f'authorization is empty, you must fill it', color='orange')
+            return None
+
+        agent = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:88.0) Gecko/20100101 Firefox/88.0'
+        # Note ytmusicapi needs the entire header, not only the authorization and cookie parts.
+        header = {
+            "user-agent": agent,
+            "accept": "*/*",
+            "accept-encoding": "gzip, deflate",
+            "content-type": "application/json",
+            "content-encoding": "gzip",
+            "origin": 'https://music.youtube.com',
+            'authorization': auth,
+            'cookie': cookie,
+        }
+        return header
+
     async def user_from_cookies(self, cookies):
         return self._provider.user_from_cookie(cookies)
 
     def load_user_cookies(self):
+        self.load_header_file()
+
+    def load_header_file(self):
         if HEADER_FILE.exists():
             with HEADER_FILE.open('r') as f:
-                return self._parse_text_cookies(json.load(f).get('Cookie', ''))
+                data = json.load(f)
+                return data
+
+    def autologin(self):
+        """Overload super.autologin."""
+        header_or_oauth = self.load_header_file()
+        if header_or_oauth is not None:
+            self.show_hint('正在尝试加载已有用户...', color='green')
+            if 'cookie' in header_or_oauth:  # It is a header.
+                cookie = header_or_oauth['cookie']
+                auth = header_or_oauth['authorization']
+                self.cookies_text_edit.setText(cookie)
+                self.auth_text_edit.setText(auth)
+            else:
+                logger.debug('The header file is a oauth.json, will not load it to UI')
+            aio.create_task(self.login_with_cookies(header_or_oauth))
 
     def dump_user_cookies(self, user, cookies):
-        js = {
-            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:72.0) Gecko/20100101 Firefox/72.0',
-            'Accept-Language': 'zh-CN,zh;q=0.9,zh-TW;q=0.8,en;q=0.7',
-            'Content-Type': 'application/json',
-            'X-Goog-AuthUser': '0',
-            'x-origin': 'https://music.youtube.com',
-            'Cookie': ';'.join([f'{k}={v}' for k, v in cookies.items()])
-        }
         with HEADER_FILE.open('w') as f:
-            json.dump(js, f, indent=2)
+            json.dump(cookies, f, indent=2)
```

### Comparing `fuo-ytmusic-0.1.1/pyproject.toml` & `fuo-ytmusic-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "fuo-ytmusic"
-version = "0.1.1"
+version = "0.2.0"
 description = "feeluown Youtube Music plugin"
 authors = ["Bruce Zhang <zttt183525594@gmail.com>"]
 keywords = ["feeluown", "ytmusic", "youtube"]
 homepage = "https://github.com/feeluown/feeluown-ytmusic"
 readme = "README.md"
 include = ["fuo_ytmusic/assets/*.svg", "fuo_ytmusic/qml/*.qml"]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
-feeluown = ">=3.7.13"
+feeluown = ">=3.8.12"
 ytmusicapi = "*"
 pydantic = "*"
 cachetools = "*"
 pytube = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
```

### Comparing `fuo-ytmusic-0.1.1/setup.py` & `fuo-ytmusic-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['cachetools', 'feeluown>=3.7.13', 'pydantic', 'pytube', 'ytmusicapi']
 
 entry_points = \
 {'fuo.plugins_v1': ['ytmusic = fuo_ytmusic']}
 
 setup_kwargs = {
     'name': 'fuo-ytmusic',
-    'version': '0.1.1',
+    'version': '0.2.0',
     'description': 'feeluown Youtube Music plugin',
     'long_description': "# YouTube Music plugin for FeelUOwn player\n\n## Prerequisites\n\nInstall [FeelUOwn](https://github.com/feeluown/FeelUOwn) before installing this plugin.\nSees: [Documentation](https://feeluown.readthedocs.io/)\n\n## Installation\n\n```shell\npip install fuo-ytmusic  # Lastest stable release\npip install https://github.com/feeluown/feeluown-ytmusic.git  # master branch\npoetry install  # Local development\n```\n\n## Configuration\n\n### Proxies\n\n```python\n# In ~/.fuorc\nconfig.deffield('YTM_HTTP_PROXY', type_=str, default='', desc='YouTube Music 代理设置')\nconfig.YTM_HTTP_PROXY='127.0.0.1:10809'\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please create a new issue first to discuss what you'd like to change.\n\nPlease make sure to compatible with [FeelUOwn](https://github.com/feeluown/FeelUOwn) lastest stable release.\n\n## License\n\nThis project is licensed under the [GPLv3](LICENSE.txt).\n",
     'author': 'Bruce Zhang',
     'author_email': 'zttt183525594@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/feeluown/feeluown-ytmusic',
@@ -28,7 +28,8 @@
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
+
```

