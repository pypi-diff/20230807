# Comparing `tmp/python-facebook-api-0.9.5.tar.gz` & `tmp/python-facebook-api-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-facebook-api-0.9.5.tar", max compression
+gzip compressed data, was "python-facebook-api-0.9.6.tar", max compression
```

## Comparing `python-facebook-api-0.9.5.tar` & `python-facebook-api-0.9.6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0    11357 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/LICENSE
--rw-r--r--   0        0        0    30051 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/README.rst
--rw-r--r--   0        0        0      165 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/__init__.py
--rw-r--r--   0        0        0      274 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/_compat.py
--rw-r--r--   0        0        0      200 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/api/__init__.py
--rw-r--r--   0        0        0    17956 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/api/base.py
--rw-r--r--   0        0        0    49868 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/api/facebook.py
--rw-r--r--   0        0        0    58619 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/api/instagram.py
--rw-r--r--   0        0        0    12183 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/api/instagram_basic.py
--rw-r--r--   0        0        0     2295 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/error.py
--rw-r--r--   0        0        0     1233 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/__init__.py
--rw-r--r--   0        0        0     2794 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/access_token.py
--rw-r--r--   0        0        0     1747 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/album.py
--rw-r--r--   0        0        0      430 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/base.py
--rw-r--r--   0        0        0     1395 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/comment.py
--rw-r--r--   0        0        0     4159 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/common.py
--rw-r--r--   0        0        0     2337 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/ig_basic_models.py
--rw-r--r--   0        0        0     8411 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/ig_pro_models.py
--rw-r--r--   0        0        0      513 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/likes.py
--rw-r--r--   0        0        0     3036 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/live.py
--rw-r--r--   0        0        0     1419 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/mixins.py
--rw-r--r--   0        0        0     6019 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/page.py
--rw-r--r--   0        0        0     2457 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/photo.py
--rw-r--r--   0        0        0     1542 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/picture.py
--rw-r--r--   0        0        0     4147 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/post.py
--rw-r--r--   0        0        0     3863 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/models/video.py
--rw-r--r--   0        0        0     5528 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/ratelimit.py
--rw-r--r--   0        0        0        0 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/utils/__init__.py
--rw-r--r--   0        0        0     5688 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/utils/constant.py
--rw-r--r--   0        0        0     1619 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyfacebook/utils/param_validation.py
--rw-r--r--   0        0        0     1569 2021-09-02 13:35:23.695813 python-facebook-api-0.9.5/pyproject.toml
--rw-r--r--   0        0        0        0 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/__init__.py
--rw-r--r--   0        0        0        0 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/__init__.py
--rw-r--r--   0        0        0        0 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/apis/__init__.py
--rw-r--r--   0        0        0     3284 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/apis/test_albums.py
--rw-r--r--   0        0        0     3656 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/apis/test_comments.py
--rw-r--r--   0        0        0     5461 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/apis/test_live_videos.py
--rw-r--r--   0        0        0     2895 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/apis/test_page.py
--rw-r--r--   0        0        0     3194 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/apis/test_photos.py
--rw-r--r--   0        0        0     2453 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/apis/test_pictures.py
--rw-r--r--   0        0        0     5626 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/apis/test_posts.py
--rw-r--r--   0        0        0     5679 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/apis/test_videos.py
--rw-r--r--   0        0        0        0 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/models/__init__.py
--rw-r--r--   0        0        0      510 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/models/test_album.py
--rw-r--r--   0        0        0      547 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/models/test_comment.py
--rw-r--r--   0        0        0      672 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/models/test_live.py
--rw-r--r--   0        0        0     1442 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/models/test_page.py
--rw-r--r--   0        0        0      561 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/models/test_photo.py
--rw-r--r--   0        0        0     1023 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/models/test_post.py
--rw-r--r--   0        0        0     1798 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/models/test_token.py
--rw-r--r--   0        0        0     1265 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/facebook/models/test_video.py
--rw-r--r--   0        0        0        0 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/__init__.py
--rw-r--r--   0        0        0        0 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/basic_apis/__init__.py
--rw-r--r--   0        0        0     2126 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/basic_apis/test_init_api.py
--rw-r--r--   0        0        0     2974 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/basic_apis/test_media.py
--rw-r--r--   0        0        0     1238 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/basic_apis/test_user.py
--rw-r--r--   0        0        0     4798 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/pro_apis/test_comment.py
--rw-r--r--   0        0        0     4084 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/pro_apis/test_discovery.py
--rw-r--r--   0        0        0     6704 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/pro_apis/test_hashtags.py
--rw-r--r--   0        0        0     3653 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/pro_apis/test_insights.py
--rw-r--r--   0        0        0     6431 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/pro_apis/test_media.py
--rw-r--r--   0        0        0     3990 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/pro_apis/test_mentions.py
--rw-r--r--   0        0        0     4451 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/pro_apis/test_publish.py
--rw-r--r--   0        0        0     4146 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/pro_apis/test_reply.py
--rw-r--r--   0        0        0     3383 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/pro_apis/test_stories.py
--rw-r--r--   0        0        0     1640 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/pro_apis/test_user.py
--rw-r--r--   0        0        0      961 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/test_basic_models.py
--rw-r--r--   0        0        0     3083 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/instagram/test_pro_models.py
--rw-r--r--   0        0        0     7808 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/test_base_api.py
--rw-r--r--   0        0        0     1114 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/test_exception.py
--rw-r--r--   0        0        0     1017 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/test_ratelimit.py
--rw-r--r--   0        0        0        0 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/utils/__init__.py
--rw-r--r--   0        0        0      780 2021-09-02 13:35:23.703814 python-facebook-api-0.9.5/tests/utils/test_param_validation.py
--rw-r--r--   0        0        0    32626 2021-09-02 13:36:14.881063 python-facebook-api-0.9.5/setup.py
--rw-r--r--   0        0        0    31488 2021-09-02 13:36:14.883232 python-facebook-api-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-11-02 14:06:30.084696 python-facebook-api-0.9.6/LICENSE
+-rw-r--r--   0        0        0    30051 2021-11-02 14:06:30.084696 python-facebook-api-0.9.6/README.rst
+-rw-r--r--   0        0        0      165 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/__init__.py
+-rw-r--r--   0        0        0      274 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/_compat.py
+-rw-r--r--   0        0        0      200 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/api/__init__.py
+-rw-r--r--   0        0        0    17957 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/api/base.py
+-rw-r--r--   0        0        0    49868 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/api/facebook.py
+-rw-r--r--   0        0        0    58619 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/api/instagram.py
+-rw-r--r--   0        0        0    12183 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/api/instagram_basic.py
+-rw-r--r--   0        0        0     2295 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/error.py
+-rw-r--r--   0        0        0     1233 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/__init__.py
+-rw-r--r--   0        0        0     2794 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/access_token.py
+-rw-r--r--   0        0        0     1747 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/album.py
+-rw-r--r--   0        0        0      430 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/base.py
+-rw-r--r--   0        0        0     1395 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/comment.py
+-rw-r--r--   0        0        0     4159 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/common.py
+-rw-r--r--   0        0        0     2337 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/ig_basic_models.py
+-rw-r--r--   0        0        0     8411 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/ig_pro_models.py
+-rw-r--r--   0        0        0      513 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/likes.py
+-rw-r--r--   0        0        0     3036 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/live.py
+-rw-r--r--   0        0        0     1419 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/mixins.py
+-rw-r--r--   0        0        0     6019 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/page.py
+-rw-r--r--   0        0        0     2457 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/photo.py
+-rw-r--r--   0        0        0     1542 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/picture.py
+-rw-r--r--   0        0        0     4147 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/post.py
+-rw-r--r--   0        0        0     3863 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/models/video.py
+-rw-r--r--   0        0        0     5528 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/ratelimit.py
+-rw-r--r--   0        0        0        0 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/utils/__init__.py
+-rw-r--r--   0        0        0     5688 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/utils/constant.py
+-rw-r--r--   0        0        0     1619 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyfacebook/utils/param_validation.py
+-rw-r--r--   0        0        0     1569 2021-11-02 14:06:30.088696 python-facebook-api-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/apis/__init__.py
+-rw-r--r--   0        0        0     3284 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/apis/test_albums.py
+-rw-r--r--   0        0        0     3656 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/apis/test_comments.py
+-rw-r--r--   0        0        0     5461 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/apis/test_live_videos.py
+-rw-r--r--   0        0        0     2895 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/apis/test_page.py
+-rw-r--r--   0        0        0     3194 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/apis/test_photos.py
+-rw-r--r--   0        0        0     2453 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/apis/test_pictures.py
+-rw-r--r--   0        0        0     5626 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/apis/test_posts.py
+-rw-r--r--   0        0        0     5679 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/apis/test_videos.py
+-rw-r--r--   0        0        0        0 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/models/__init__.py
+-rw-r--r--   0        0        0      510 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/models/test_album.py
+-rw-r--r--   0        0        0      547 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/models/test_comment.py
+-rw-r--r--   0        0        0      672 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/models/test_live.py
+-rw-r--r--   0        0        0     1442 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/models/test_page.py
+-rw-r--r--   0        0        0      561 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/models/test_photo.py
+-rw-r--r--   0        0        0     1023 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/models/test_post.py
+-rw-r--r--   0        0        0     1798 2021-11-02 14:06:30.096696 python-facebook-api-0.9.6/tests/facebook/models/test_token.py
+-rw-r--r--   0        0        0     1265 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/facebook/models/test_video.py
+-rw-r--r--   0        0        0        0 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/basic_apis/__init__.py
+-rw-r--r--   0        0        0     2126 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/basic_apis/test_init_api.py
+-rw-r--r--   0        0        0     2974 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/basic_apis/test_media.py
+-rw-r--r--   0        0        0     1238 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/basic_apis/test_user.py
+-rw-r--r--   0        0        0     4798 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/pro_apis/test_comment.py
+-rw-r--r--   0        0        0     4084 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/pro_apis/test_discovery.py
+-rw-r--r--   0        0        0     6704 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/pro_apis/test_hashtags.py
+-rw-r--r--   0        0        0     3653 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/pro_apis/test_insights.py
+-rw-r--r--   0        0        0     6431 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/pro_apis/test_media.py
+-rw-r--r--   0        0        0     3990 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/pro_apis/test_mentions.py
+-rw-r--r--   0        0        0     4451 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/pro_apis/test_publish.py
+-rw-r--r--   0        0        0     4146 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/pro_apis/test_reply.py
+-rw-r--r--   0        0        0     3383 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/pro_apis/test_stories.py
+-rw-r--r--   0        0        0     1640 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/pro_apis/test_user.py
+-rw-r--r--   0        0        0      961 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/test_basic_models.py
+-rw-r--r--   0        0        0     3083 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/instagram/test_pro_models.py
+-rw-r--r--   0        0        0     7698 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/test_base_api.py
+-rw-r--r--   0        0        0     1114 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/test_exception.py
+-rw-r--r--   0        0        0     1017 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/test_ratelimit.py
+-rw-r--r--   0        0        0        0 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/utils/__init__.py
+-rw-r--r--   0        0        0      780 2021-11-02 14:06:30.100696 python-facebook-api-0.9.6/tests/utils/test_param_validation.py
+-rw-r--r--   0        0        0    32626 2021-11-02 14:07:26.083600 python-facebook-api-0.9.6/setup.py
+-rw-r--r--   0        0        0    31539 2021-11-02 14:07:26.085540 python-facebook-api-0.9.6/PKG-INFO
```

### Comparing `python-facebook-api-0.9.5/LICENSE` & `python-facebook-api-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/README.rst` & `python-facebook-api-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/api/base.py` & `python-facebook-api-0.9.6/pyfacebook/api/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from pyfacebook.error import PyFacebookException, ErrorMessage, ErrorCode, PyFacebookDeprecationWaring
 from pyfacebook.models import AccessToken, AuthAccessToken
 from pyfacebook.ratelimit import RateLimit, PercentSecond
 
 
 class BaseApi(object):
-    VALID_API_VERSIONS = ["v4.0", "v5.0", "v6.0", "v7.0", "v8.0", "v9.0", "v10.0", "v11.0"]
+    VALID_API_VERSIONS = ["v5.0", "v6.0", "v7.0", "v8.0", "v9.0", "v10.0", "v11.0", "v12.0"]
     GRAPH_URL = "https://graph.facebook.com/"
     DEFAULT_AUTHORIZATION_URL = 'https://www.facebook.com/dialog/oauth'
     DEFAULT_EXCHANGE_ACCESS_TOKEN_URL = 'https://graph.facebook.com/oauth/access_token'
     DEFAULT_REDIRECT_URI = 'https://localhost/'
     DEFAULT_SCOPE = []
     DEFAULT_STATE = 'PyFacebook'
```

### Comparing `python-facebook-api-0.9.5/pyfacebook/api/facebook.py` & `python-facebook-api-0.9.6/pyfacebook/api/facebook.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/api/instagram.py` & `python-facebook-api-0.9.6/pyfacebook/api/instagram.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/api/instagram_basic.py` & `python-facebook-api-0.9.6/pyfacebook/api/instagram_basic.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/error.py` & `python-facebook-api-0.9.6/pyfacebook/error.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/__init__.py` & `python-facebook-api-0.9.6/pyfacebook/models/__init__.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/access_token.py` & `python-facebook-api-0.9.6/pyfacebook/models/access_token.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/album.py` & `python-facebook-api-0.9.6/pyfacebook/models/album.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/comment.py` & `python-facebook-api-0.9.6/pyfacebook/models/comment.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/common.py` & `python-facebook-api-0.9.6/pyfacebook/models/common.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/ig_basic_models.py` & `python-facebook-api-0.9.6/pyfacebook/models/ig_basic_models.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/ig_pro_models.py` & `python-facebook-api-0.9.6/pyfacebook/models/ig_pro_models.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/likes.py` & `python-facebook-api-0.9.6/pyfacebook/models/likes.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/live.py` & `python-facebook-api-0.9.6/pyfacebook/models/live.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/mixins.py` & `python-facebook-api-0.9.6/pyfacebook/models/mixins.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/page.py` & `python-facebook-api-0.9.6/pyfacebook/models/page.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/photo.py` & `python-facebook-api-0.9.6/pyfacebook/models/photo.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/picture.py` & `python-facebook-api-0.9.6/pyfacebook/models/picture.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/post.py` & `python-facebook-api-0.9.6/pyfacebook/models/post.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/models/video.py` & `python-facebook-api-0.9.6/pyfacebook/models/video.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/ratelimit.py` & `python-facebook-api-0.9.6/pyfacebook/ratelimit.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/utils/constant.py` & `python-facebook-api-0.9.6/pyfacebook/utils/constant.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyfacebook/utils/param_validation.py` & `python-facebook-api-0.9.6/pyfacebook/utils/param_validation.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/pyproject.toml` & `python-facebook-api-0.9.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-facebook-api"
-version = "0.9.5"
+version = "0.9.6"
 description = "A simple Python wrapper around the Facebook Graph API"
 authors = ["Ikaros kun <merle.liukun@gmail.com>"]
 readme = "README.rst"
 license = "Apache-2.0"
 repository = 'https://github.com/sns-sdks/python-facebook'
 homepage = "https://github.com/sns-sdks/python-facebook"
 keywords = ["facebook-graph-api", "facebook-sdk", "instagram-api", "instagram-sdk", "facebook-api"]
```

### Comparing `python-facebook-api-0.9.5/tests/facebook/apis/test_albums.py` & `python-facebook-api-0.9.6/tests/facebook/apis/test_albums.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/apis/test_comments.py` & `python-facebook-api-0.9.6/tests/facebook/apis/test_comments.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/apis/test_live_videos.py` & `python-facebook-api-0.9.6/tests/facebook/apis/test_live_videos.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/apis/test_page.py` & `python-facebook-api-0.9.6/tests/facebook/apis/test_page.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/apis/test_photos.py` & `python-facebook-api-0.9.6/tests/facebook/apis/test_photos.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/apis/test_pictures.py` & `python-facebook-api-0.9.6/tests/facebook/apis/test_pictures.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/apis/test_posts.py` & `python-facebook-api-0.9.6/tests/facebook/apis/test_posts.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/apis/test_videos.py` & `python-facebook-api-0.9.6/tests/facebook/apis/test_videos.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/models/test_comment.py` & `python-facebook-api-0.9.6/tests/facebook/models/test_comment.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/models/test_live.py` & `python-facebook-api-0.9.6/tests/facebook/models/test_live.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/models/test_page.py` & `python-facebook-api-0.9.6/tests/facebook/models/test_page.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/models/test_photo.py` & `python-facebook-api-0.9.6/tests/facebook/models/test_photo.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/models/test_post.py` & `python-facebook-api-0.9.6/tests/facebook/models/test_post.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/models/test_token.py` & `python-facebook-api-0.9.6/tests/facebook/models/test_token.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/facebook/models/test_video.py` & `python-facebook-api-0.9.6/tests/facebook/models/test_video.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/basic_apis/test_init_api.py` & `python-facebook-api-0.9.6/tests/instagram/basic_apis/test_init_api.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/basic_apis/test_media.py` & `python-facebook-api-0.9.6/tests/instagram/basic_apis/test_media.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/basic_apis/test_user.py` & `python-facebook-api-0.9.6/tests/instagram/basic_apis/test_user.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/pro_apis/test_comment.py` & `python-facebook-api-0.9.6/tests/instagram/pro_apis/test_comment.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/pro_apis/test_discovery.py` & `python-facebook-api-0.9.6/tests/instagram/pro_apis/test_discovery.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/pro_apis/test_hashtags.py` & `python-facebook-api-0.9.6/tests/instagram/pro_apis/test_hashtags.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/pro_apis/test_insights.py` & `python-facebook-api-0.9.6/tests/instagram/pro_apis/test_insights.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/pro_apis/test_media.py` & `python-facebook-api-0.9.6/tests/instagram/pro_apis/test_media.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/pro_apis/test_mentions.py` & `python-facebook-api-0.9.6/tests/instagram/pro_apis/test_mentions.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/pro_apis/test_publish.py` & `python-facebook-api-0.9.6/tests/instagram/pro_apis/test_publish.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/pro_apis/test_reply.py` & `python-facebook-api-0.9.6/tests/instagram/pro_apis/test_reply.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/pro_apis/test_stories.py` & `python-facebook-api-0.9.6/tests/instagram/pro_apis/test_stories.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/pro_apis/test_user.py` & `python-facebook-api-0.9.6/tests/instagram/pro_apis/test_user.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/test_basic_models.py` & `python-facebook-api-0.9.6/tests/instagram/test_basic_models.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/instagram/test_pro_models.py` & `python-facebook-api-0.9.6/tests/instagram/test_pro_models.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/test_base_api.py` & `python-facebook-api-0.9.6/tests/test_base_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,16 @@
 
         with self.assertRaises(pyfacebook.PyFacebookException):
             BaseApi(version="version")
 
         api = BaseApi(long_term_token="token", version=None)
         self.assertEqual(api.version, api.VALID_API_VERSIONS[-1])
 
-        api = BaseApi(long_term_token="token", version="3.3")
-        self.assertEqual(api.version, "v3.3")
-
-        api = BaseApi(long_term_token="token", version="v10.0")
-        self.assertEqual(api.version, "v10.0")
+        api = BaseApi(long_term_token="token", version="12.0")
+        self.assertEqual(api.version, "v12.0")
 
     @patch('time.sleep', return_value=None)
     def testApiToken(self, patched_time_sleep):
         with self.assertRaises(pyfacebook.PyFacebookException):
             BaseApi()
 
         api = BaseApi(long_term_token="token", debug_http=True)
```

### Comparing `python-facebook-api-0.9.5/tests/test_exception.py` & `python-facebook-api-0.9.6/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/test_ratelimit.py` & `python-facebook-api-0.9.6/tests/test_ratelimit.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/tests/utils/test_param_validation.py` & `python-facebook-api-0.9.6/tests/utils/test_param_validation.py`

 * *Files identical despite different names*

### Comparing `python-facebook-api-0.9.5/setup.py` & `python-facebook-api-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 extras_require = \
 {':python_version >= "2.7" and python_version < "2.8" or python_version >= "3.6" and python_version < "3.7"': ['cattrs==1.0.0'],
  ':python_version >= "3.7" and python_version < "4.0"': ['cattrs==1.6.0']}
 
 setup_kwargs = {
     'name': 'python-facebook-api',
-    'version': '0.9.5',
+    'version': '0.9.6',
     'description': 'A simple Python wrapper around the Facebook Graph API',
     'long_description': 'Python Facebook\n\nA Python wrapper for the Facebook Common API.\n\n.. image:: https://github.com/sns-sdks/python-facebook/workflows/Test/badge.svg\n    :target: https://github.com/sns-sdks/python-facebook/actions\n    :alt: Build Status\n\n.. image:: https://img.shields.io/badge/Docs-passing-brightgreen\n    :target: https://sns-sdks.github.io/python-facebook/\n    :alt: Documentation Status\n\n.. image:: https://codecov.io/gh/sns-sdks/python-facebook/branch/master/graph/badge.svg\n    :target: https://codecov.io/gh/sns-sdks/python-facebook\n    :alt: Codecov\n\n.. image:: https://img.shields.io/pypi/v/python-facebook-api.svg\n    :target: https://pypi.org/project/python-facebook-api\n    :alt: PyPI\n\n\nREADME: `English <README.rst>`_ | `中文 <README-zh.rst>`_\n\n======\nTHANKS\n======\n\nInspired by `Python-Twitter <https://github.com/bear/python-twitter>`_.\n\n============\nIntroduction\n============\n\nLibrary provides a service to easily use Facebook Graph API.\n\nIt currently includes the use of ``Facebook``,  ``Instagram Business``, and ``Instagram Basic Display`` product data.\n\n==========\nInstalling\n==========\n\nYou can install this library from ``pypi``::\n\n    $pip install --upgrade python-facebook-api\n    ✨🍰✨\n\n\n=============\nDocumentation\n=============\n\nYou can view the latest ``python-facebook`` documentation at: https://sns-sdks.github.io/python-facebook/\n\nAlso view the full ``Facebook Graph API`` docs at: https://developers.facebook.com/docs/graph-api/\n\nAnd full ``Instagram Graph API`` docs at: https://developers.facebook.com/docs/instagram-api/\n\nAnd full ``Instagram Basic Display API`` docs at: https://developers.facebook.com/docs/instagram-basic-display-api/\n\n=============================\nBase-Usage-Facebook Graph API\n=============================\n\nThe API is exposed via the ``pyfacebook.Api`` class.\n\nTo get data, you need to have a facebook app first.\nYou can get more information about create, apply permissions for app at `App docs <https://developers.facebook.com/docs/apps>`_.\n\nAlso, you can get some examples for this library at `Example folder <examples>`_.\n\n-----------\nInitial Api\n-----------\n\nFacebook has different types of access tokens. You can use different access tokens to get different data.\n\n1. User Access Token\n#. App Access Token\n#. Page Access Token\n#. Client Token (library not support)\n\nYou can see the docs `access-token`_ to get more information.\n\nIf you want to get user access token by authorize. You can follow the docs `authorization-manually`_ to initial the api.\n\nIf you just want to use app access token to get some public data. You can initial an api as follows::\n\n    In [2]: api = Api(app_id="your app id", app_secret="your app secret", application_only_auth=True)\n    In [3]: api.get_token_info()\n    Out[3]: AccessToken(app_id=\'id\', application=\'app name\', user_id=None)\n\nIf you have a short-lived token you can initial an api as follows::\n\n    In [4]: api = Api(app_id="your app id", app_secret="your app secret", short_token="short-lived token")\n    In [5]: api.get_token_info()\n    Out[5]: AccessToken(app_id=\'id\', application=\'app name\', user_id=\'token user id\')\n\nIf you have a long term token you can initial an api as follows (Just provide only ``long_term_token`` parameter enough. but for security need provide with app credentials)::\n\n    In [6]: api = Api(app_id="your app id", app_secret="your app secret", long_term_token="long-term token")\n    In [7]: api.get_token_info()\n    Out[7]: AccessToken(app_id=\'id\', application=\'app name\', user_id=\'token user id\')\n\n    # this need token have additional manage_pages permission.\n    In [8]: api = Api(long_term_token="long-term token")\n\nthe difference between initialize with parameter ``short_token`` or ``long_term_token`` is that short token will auto exchange a long term token inside.\n\nFacebook rate limit is very vague, it is related to the number of users of your app. So the library provides the custom sleep times in requests.\nYou can only set parameter ``sleep_on_rate_limit`` with ``True`` to let api sleep two seconds between two requests.\nOr you can set parameter ``sleep_seconds_mapping`` with a dict that contains your custom data. ex::\n\n    In [9]: mapping = {10: 2, 20: 5, 50: 20, 70: 30}  # key is api limit reached percent and value is seconds to sleep.\n    In [10]: api = Api(\n        ...:     app_id="your app id", app_secret="your app secret", long_term_token="long-term token",\n        ...:     sleep_on_rate_limit=True, sleep_seconds_mapping=mapping\n        ...:)\n\n\n--------\nGet Data\n--------\n\nYou can get a facebook page information by the following methods.\n\nTo fetch one facebook page\'s public data::\n\n    In [3]: api.get_page_info(username=\'facebookapp\')\n    Out[3]: Page(id=\'20531316728\', name=\'Facebook\', username=\'facebookapp\')\n\n\nTo fetch multi page by one request, you can pass the page username list or page id list with the ``ids`` parameter as follows::\n\n    In [4]: api.get_pages_info(ids=["20531316728", "nba"])\n    Out[4]:\n    {\'20531316728\': Page(id=\'20531316728\', name=\'Facebook\', username=\'facebookapp\'),\n     \'nba\': Page(id=\'8245623462\', name=\'NBA\', username=\'nba\')}\n\nThere are multiple methods to retrieve one page\'s posts data.\n\n>>> api.get_page_feeds()\n>>> api.get_page_posts()\n>>> api.get_page_published_posts()\n>>> api.get_page_tagged_posts()\n\nPage feeds can get feed of posts (including status updates) and links published by this page, or by others on this page. You can call with the following::\n\n    In [5]: api.get_page_feeds(page_id="20531316728",count=2)\n    Out[5]:\n    [Post(id=\'20531316728_587455038708591\', permalink_url=\'https://www.facebook.com/facebookapp/videos/587455038708591/\'),\n     Post(id=\'20531316728_10159023836696729\', permalink_url=\'https://www.facebook.com/20531316728/posts/10159023836696729/\')]\n\nPage posts can only get the posts that were published by this page::\n\n    In [6]: api.get_page_posts(page_id="20531316728",count=2)\n    Out[6]:\n    [Post(id=\'20531316728_587455038708591\', permalink_url=\'https://www.facebook.com/facebookapp/videos/587455038708591/\'),\n     Post(id=\'20531316728_10159023836696729\', permalink_url=\'https://www.facebook.com/20531316728/posts/10159023836696729/\')]\n\n\nBecause of facebook graph api limit `Page Feed <https://developers.facebook.com/docs/graph-api/reference/v5.0/page/feed>`_.\nUsing public token can only get approximately 600 ranked, published posts per year.\n\nSo if you want to get all of a page\'s posts or posts which tagged the page. you need use method ``get_page_published_posts``, and this needs a page\'s access token with permission ``manage_pages``.\n\nYou can use authorization to get that page access token. Just follows docs `authorization-manually`_.\nThen you can get all published posts::\n\n    In [7]: api.get_published_posts(username=\'facebookapp\', access_token=\'page access token\')\n    Out[7]: [Post...]\n\nYou can get tagged posts::\n\n    In [8]: api.get_tagged_posts(username=\'facebookapp\', access_token=\'page access token\')\n    Out[8]: [Post...]\n\n\nIf you also have the post id, you can get post detail info by the following methods.\n\nTo fetch a post info::\n\n    In [9]: api.get_post_info(post_id="20531316728_587455038708591")\n    Out[9]: Post(id=\'20531316728_587455038708591\', permalink_url=\'https://www.facebook.com/facebookapp/videos/587455038708591/\')\n\nTo fetch multi posts by one requests::\n\n    In [10]: api.get_posts_info(ids=["20531316728_587455038708591", "20531316728_10159023836696729"])\n    Out[10]:\n    {\'20531316728_587455038708591\': Post(id=\'20531316728_587455038708591\', permalink_url=\'https://www.facebook.com/facebookapp/videos/587455038708591/\'),\n     \'20531316728_10159023836696729\': Post(id=\'20531316728_10159023836696729\', permalink_url=\'https://www.facebook.com/20531316728/posts/10159023836696729/\')}\n\nYou can get comments data by the object(post, page and so on) id::\n\n    In [11]: api.get_comments_by_object(object_id="20531316728_587455038708591", count=2)\n    Out[11]:\n    ([Comment(id=\'587455038708591_587460942041334\', can_like=True, can_comment=True, comment_count=2, like_count=1),\n      Comment(id=\'587455038708591_587464298707665\', can_like=True, can_comment=True, comment_count=2, like_count=14)],\n     CommentSummary(total_count=392, can_comment=True))\n\nIf you already have the comment id, you can get comment details info with the following methods.\n\nTo fetch one comment info::\n\n    In [12]: api.get_comment_info(comment_id="587455038708591_587460942041334")\n    Out[12]: Comment(id=\'587455038708591_587460942041334\', comment_count=2, like_count=1)\n\nTo fetch multi comment info by one request::\n\n    In [13]: api.get_comments_info(ids=["587455038708591_587460942041334", "587455038708591_587464298707665"])\n    Out[13]:\n    {\'587455038708591_587460942041334\': Comment(id=\'587455038708591_587460942041334\', comment_count=2, like_count=1),\n     \'587455038708591_587464298707665\': Comment(id=\'587455038708591_587464298707665\', comment_count=2, like_count=14)}\n\n\n\nYou can get the page\'s profile picture by the following methods.\n\nTo fetch one page picture::\n\n    In [14]: api.get_picture(page_id="20531316728")\n    Out[14]: ProfilePictureSource(url=\'https://scontent.xx.fbcdn.net/v/t1.0-1/p100x100/58978526_10158354585751729_7411073224387067904_o.png?_nc_cat=1&_nc_oc=AQmaFO7eND-DVRoArrQLUZVDpmemw8nMPmHJWvoCyXId_MKLLHQdsS8UbTOX4oaEfeQ&_nc_ht=scontent.xx&oh=128f57c4dc65608993af62b562d92d84&oe=5E942420\', height=100, width=100)\n\n\nTo fetch multi page picture::\n\n    In [15]: api.get_pictures(ids=["20531316728", "nba"])\n    Out[15]:\n    {\'20531316728\': ProfilePictureSource(url=\'https://scontent.xx.fbcdn.net/v/t1.0-1/p100x100/58978526_10158354585751729_7411073224387067904_o.png?_nc_cat=1&_nc_oc=AQmaFO7eND-DVRoArrQLUZVDpmemw8nMPmHJWvoCyXId_MKLLHQdsS8UbTOX4oaEfeQ&_nc_ht=scontent.xx&oh=128f57c4dc65608993af62b562d92d84&oe=5E942420\', height=100, width=100),\n     \'nba\': ProfilePictureSource(url=\'https://scontent.xx.fbcdn.net/v/t1.0-1/p100x100/81204460_10158199356848463_5727214464013434880_n.jpg?_nc_cat=1&_nc_oc=AQmcent57E-a-923C_VVpiX26nGqKDodImY1gsiu7h1czDmcpLHXR8D5hIh9g9Ao3wY&_nc_ht=scontent.xx&oh=1656771e6c11bd03147b69ee643238ba&oe=5E66450C\', height=100, width=100)}\n\nYou can get videos data by the object(page, user...) id::\n\n    In [16]: api.get_videos_by_object("ikaroskunlife", fields=["id", "title", "description"], count=None, limit=20)\n    Out[16]:\n    [Video(id=\'969222676905304\', created_time=None, description=\'冬日\'),\n     Video(id=\'210174653594254\', created_time=None, description=\'Snowing\'),\n     Video(id=\'674270653053120\', created_time=None, description=\'Visible\')]\n\nIf you already have the id of videos, you can get more info by the following methods::\n\n    In [17]: api.get_video_info("969222676905304")\n    Out[17]: Video(id=\'969222676905304\', created_time=\'2020-09-12T09:53:06+0000\', description=\'冬日\')\n\n    In [18]: api.get_videos(ids=["210174653594254", "674270653053120"])\n    Out[18]:\n    {\'210174653594254\': Video(id=\'210174653594254\', created_time=\'2020-03-31T08:13:14+0000\', description=\'Snowing\'),\n     \'674270653053120\': Video(id=\'674270653053120\', created_time=\'2019-09-02T06:13:17+0000\', description=\'Visible\')}\n\nYou can get albums data by the object(page, user...) id::\n\n    In[19]: api.get_albums_by_object("instagram", count=20, limit=15)\n    Out[19]:\n    [Album(id=\'372558296163354\', created_time=\'2012-10-29T19:46:35+0000\', name=\'时间线照片\'),\n     Album(id=\'623202484432266\', created_time=\'2014-04-12T15:28:26+0000\', name=\'手机上传\')...]\n\nIf you already have the id of album, you can get more info by the following methods::\n\n    In[20]: api.get_album_info("372558296163354")\n    Out[20]: Album(id=\'372558296163354\', created_time=\'2012-10-29T19:46:35+0000\', name=\'时间线照片\')\n\n    In[21]: api.get_albums(ids="372558296163354,623202484432266")\n    Out[21]:\n    {\'372558296163354\': Album(id=\'372558296163354\', created_time=\'2012-10-29T19:46:35+0000\', name=\'时间线照片\'),\n     \'623202484432266\': Album(id=\'623202484432266\', created_time=\'2014-04-12T15:28:26+0000\', name=\'手机上传\')}\n\nYou can get photos data by the object(page, album, user...) id::\n\n    In [22]: api.get_photos_by_object("372558296163354", count=10, limit=5)\n    Out[22]:\n    [Photo(id=\'3293405020745319\', created_time=\'2020-09-10T19:11:01+0000\', name=\'Roller skating = Black joy for Travis Reynolds. 🖤\\n\\nWatch our IGTV to catch some good vibes and see his 🔥🔥🔥 tricks. \\n\\n#ShareBlackStories\\n\\nhttps://www.instagram.com/tv/CE9xgF3jwS_/\'),\n     Photo(id=\'3279789248773563\', created_time=\'2020-09-06T16:23:17+0000\', name=\'#HelloFrom Los Glaciares National Park, Argentina 👏👏👏\\n\\nhttps://www.instagram.com/p/CEzSoQNMdfH/\'),\n     Photo(id=\'3276650595754095\', created_time=\'2020-09-05T16:52:54+0000\', name=None)...]\n\nIf you already have the id of photos, you can get more info by the following methods::\n\n    In [4]: api.get_photo_info("3293405020745319")\n    Out[4]: Photo(id=\'3293405020745319\', created_time=\'2020-09-10T19:11:01+0000\', name=\'Roller skating = Black joy for Travis Reynolds. 🖤\\n\\nWatch our IGTV to catch some good vibes and see his 🔥🔥🔥 tricks. \\n\\n#ShareBlackStories\\n\\nhttps://www.instagram.com/tv/CE9xgF3jwS_/\')\n\n    In [5]: api.get_photos(ids=["3279789248773563", "3276650595754095"])\n    Out[5]:\n    {\'3279789248773563\': Photo(id=\'3279789248773563\', created_time=\'2020-09-06T16:23:17+0000\', name=\'#HelloFrom Los Glaciares National Park, Argentina 👏👏👏\\n\\nhttps://www.instagram.com/p/CEzSoQNMdfH/\'),\n     \'3276650595754095\': Photo(id=\'3276650595754095\', created_time=\'2020-09-05T16:52:54+0000\', name=None)}\n\n\nYou can get live videos data by the object(page, user...) id::\n\n    In [6]: api.get_live_videos_by_object(object_id="2121008874780932", limit=10, count=2)\n    Out[6]:\n    [LiveVideo(id=\'2814245952123884\', permalink_url=\'/IkaroskunLife/videos/710393869909608/\'),\n     LiveVideo(id=\'2809188389296307\', permalink_url=\'/IkaroskunLife/videos/706216360286730/\')]\n\nIf you already have the id of live videos, you can get more info by the following methods::\n\n    In [7]: api.get_live_video_info(live_video_id="2814245952123884")\n    Out[7]: LiveVideo(id=\'2814245952123884\', permalink_url=\'/IkaroskunLife/videos/710393869909608/\')\n\n    In [8]: api.get_live_videos(ids=["2814245952123884", "2809188389296307"])\n    Out[8]:\n    {\'2814245952123884\': LiveVideo(id=\'2814245952123884\', permalink_url=\'/IkaroskunLife/videos/710393869909608/\'),\n     \'2809188389296307\': LiveVideo(id=\'2809188389296307\', permalink_url=\'/IkaroskunLife/videos/706216360286730/\')}\n\nSame as get live video input stream data.\n\n==============================\nBase-Usage-Instagram Graph API\n==============================\n\nInstagram Graph API allows you to get `instagram Professional accounts <https://help.instagram.com/502981923235522>`_ data.\n\n-----------\nInitial Api\n-----------\n\nAs similar to facebook graph api. This api can be initialized by multiple methods. But can only use user access token, and needs your instagram business id.\n\nIf you want to get user access token by authorize. You can follows the docs `authorization-manually`_ to initialize the api.\n\nIf you have a short-lived token you can initialize an api as follows::\n\n    In [2]: api = IgProApi(app_id="your app id", app_secret="your app secret", short_token="short-lived token", instagram_business_id="17841406338772941")\n    In [3]: api.get_token_info()\n    Out[3]: AccessToken(app_id=\'id\', application=\'app name\', user_id="token user id")\n\nIf you have a long term token you can initialize an api as follows (Just providing only ``long_term_token`` parameter is enough, but for security you need to provide app credentials)::\n\n    In [4]: api = IgProApi(app_id="your app id", app_secret="your app secret", long_term_token="long-lived token")\n    In [5]: api.get_token_info()\n    Out[5]: AccessToken(app_id=\'id\', application=\'app name\', user_id=\'token user id\')\n\n--------\nGet Data\n--------\n\nIf you want to search other\'s business account basic info and medias.\nYou can use methods as follows::\n\n    - discovery_user: retrieve user basic data\n    - discovery_user_medias: retrieve user medias data\n\n.. note::\n   Use discovery only support search by instagram user name.\n\nRetrieve other user info by username::\n\n    In [6]: api.discovery_user(username="facebook")\n    Out[6]: IgProUser(id=\'17841400455970028\', name=\'Facebook\', username=\'facebook\')\n\nRetrieve other user medias by username::\n\n    In [7]: api.discovery_user_medias(username="facebook", count=2)\n    Out[7]:\n    [IgProMedia(comments=None, id=\'17859633232647524\', permalink=\'https://www.instagram.com/p/B6jje2UnoH8/\'),\n     IgProMedia(comments=None, id=\'18076151185161297\', permalink=\'https://www.instagram.com/p/B6ji-PZH2V1/\')]\n\n\nGet your account info::\n\n    In [10]: api.get_user_info(user_id="your instagram business id")\n    Out[10]: IgProUser(id=\'17841406338772941\', name=\'LiuKun\', username=\'ikroskun\')\n\n\nGet your medias::\n\n    In [11]: api.get_user_medias(user_id=api.instagram_business_id, count=2)\n    Out[11]:\n    [IgProMedia(comments=None, id=\'18075344632131157\', permalink=\'https://www.instagram.com/p/B38X8BzHsDi/\'),\n     IgProMedia(comments=None, id=\'18027939643230671\', permalink=\'https://www.instagram.com/p/B38Xyp6nqsS/\')]\n\n\nIf you already have some medias id, you can get media info by the following methods.\n\nTo fetch a post info::\n\n    In [12]: api.get_media_info(media_id="18075344632131157")\n    Out[12]: IgProMedia(comments=None, id=\'18075344632131157\', permalink=\'https://www.instagram.com/p/B38X8BzHsDi/\')\n\n\nTo fetch multi medias by one requests::\n\n    In [13]: api.get_medias_info(media_ids=["18075344632131157", "18027939643230671"])\n    Out[13]:\n    {\'18075344632131157\': IgProMedia(comments=None, id=\'18075344632131157\', permalink=\'https://www.instagram.com/p/B38X8BzHsDi/\'),\n     \'18027939643230671\': IgProMedia(comments=None, id=\'18027939643230671\', permalink=\'https://www.instagram.com/p/B38Xyp6nqsS/\')}\n\nGet comments for media::\n\n    In [16]: api.get_comments_by_media(media_id="17955956875141196", count=2)\n    Out[16]:\n    [IgProComment(id=\'17862949873623188\', timestamp=\'2020-01-05T05:58:47+0000\'),\n     IgProComment(id=\'17844360649889631\', timestamp=\'2020-01-05T05:58:42+0000\')]\n\n\nIf you already have some comments id, you can get comment details info by the following methods.\n\nTo fetch a comment info::\n\n    In [17]: api.get_comment_info(comment_id="17862949873623188")\n    Out[17]: IgProComment(id=\'17862949873623188\', timestamp=\'2020-01-05T05:58:47+0000\')\n\nTo fetch multi comments by one requests::\n\n    In [18]: api.get_comments_info(comment_ids=["17862949873623188", "17844360649889631"\n    ...: ])\n    Out[18]:\n    {\'17862949873623188\': IgProComment(id=\'17862949873623188\', timestamp=\'2020-01-05T05:58:47+0000\'),\n     \'17844360649889631\': IgProComment(id=\'17844360649889631\', timestamp=\'2020-01-05T05:58:42+0000\')}\n\nGet replies for a comments::\n\n    In [19]: api.get_replies_by_comment("17984127178281340", count=2)\n    Out[19]:\n    [IgProReply(id=\'18107567341036926\', timestamp=\'2019-10-15T07:06:09+0000\'),\n     IgProReply(id=\'17846106427692294\', timestamp=\'2019-10-15T07:05:17+0000\')]\n\nIf you already have some replies id, you can get replies details info by the following methods.\n\nTo fetch a reply info::\n\n    In [20]: api.get_reply_info(reply_id="18107567341036926")\n    Out[20]: IgProReply(id=\'18107567341036926\', timestamp=\'2019-10-15T07:06:09+0000\')\n\nTo fetch multi replies info by one requests::\n\n    In [21]: api.get_replies_info(reply_ids=["18107567341036926", "17846106427692294"])\n    Out[21]:\n    {\'18107567341036926\': IgProReply(id=\'18107567341036926\', timestamp=\'2019-10-15T07:06:09+0000\'),\n     \'17846106427692294\': IgProReply(id=\'17846106427692294\', timestamp=\'2019-10-15T07:05:17+0000\')}\n\n\nUse ``get_user_insights`` method, you can get account insights data.\n\nIf you want get your account insights, just provide ``user_id`` with your id.\n\nIf you have other account\'s access token, you can provide with ``user_id`` and ``access_token``::\n\n    In [4]: api.get_user_insights(user_id=api.instagram_business_id, period="day", metrics=["impressions", "reach"])\n    Out[4]:\n    [IgProInsight(name=\'impressions\', period=\'day\'),\n     IgProInsight(name=\'reach\', period=\'day\')]\n\n\nThe same as ``get_user_insights``, you can custom provide ``media_id`` and ``access_token``.\n\nGet your media insights data::\n\n    In [6]: api.get_media_insights(media_id="media_id", metrics=["engagement","impressions"])\n    Out[6]:\n    [IgProInsight(name=\'engagement\', period=\'lifetime\'),\n     IgProInsight(name=\'impressions\', period=\'lifetime\')]\n\nGet hashtag id::\n\n    In [3]: api.search_hashtag(q="love")\n    Out[3]: [IgProHashtag(id=\'17843826142012701\', name=None)]\n\nGet hashtag info::\n\n    In [4]: api.get_hashtag_info(hashtag_id="17843826142012701")\n    Out[4]: IgProHashtag(id=\'17843826142012701\', name=\'love\')\n\nGet hashtag\'s top medias::\n\n    In [5]: r = api.get_hashtag_top_medias(hashtag_id="17843826142012701", count=5)\n\n    In [6]: r\n    Out[6]:\n    [IgProMedia(comments=None, id=\'18086291068155608\', permalink=\'https://www.instagram.com/p/B8ielBPpHaw/\'),\n     IgProMedia(comments=None, id=\'17935250359346228\', permalink=\'https://www.instagram.com/p/B8icUmwoF0Y/\'),\n     IgProMedia(comments=None, id=\'17847031435934181\', permalink=\'https://www.instagram.com/p/B8icycxKEn-/\'),\n     IgProMedia(comments=None, id=\'18000940699302502\', permalink=\'https://www.instagram.com/p/B8ieNN7Cv6S/\'),\n     IgProMedia(comments=None, id=\'18025516372248793\', permalink=\'https://www.instagram.com/p/B8iduQJgSyO/\')]\n\nGet hashtag\'s recent medias::\n\n    In [7]: r1 = api.get_hashtag_recent_medias(hashtag_id="17843826142012701", count=5)\n\n    In [8]: r1\n    Out[8]:\n    [IgProMedia(comments=None, id=\'18128248021002097\', permalink=\'https://www.instagram.com/p/B8ifnoWA5Ru/\'),\n     IgProMedia(comments=None, id=\'18104579776105272\', permalink=\'https://www.instagram.com/p/B8ifwfsgBw2/\'),\n     IgProMedia(comments=None, id=\'17898846532442427\', permalink=\'https://www.instagram.com/p/B8ifwZ4ltqP/\'),\n     IgProMedia(comments=None, id=\'17891698510462453\', permalink=\'https://www.instagram.com/p/B8ifwepgf_E/\'),\n     IgProMedia(comments=None, id=\'17883544606492965\', permalink=\'https://www.instagram.com/p/B8ifwabgiPf/\')]\n\nIf you have other account\'s access token, you can provide it with ``user_id`` and ``access_token`` to get its search hashtags.\nOr just get your account recent searched hashtags::\n\n    In [9]: api.get_user_recently_searched_hashtags(user_id="17841406338772941")\n    Out[9]:\n    [IgProHashtag(id=\'17843826142012701\', name=\'love\'),\n     IgProHashtag(id=\'17843421130029320\', name=\'liukun\'),\n     IgProHashtag(id=\'17841562447105233\', name=\'loveyou\'),\n     IgProHashtag(id=\'17843761288040806\', name=\'a\')]\n\n\nGet the media objects in which a Business or Creator Account has been tagged.\nIf you have another account authorized access token, you can provide it with ``user_id`` and ``access_token`` to get its data.\nOr only get your account\'s data::\n\n    In [10]: medias = api.get_tagged_user_medias(user_id=api.instagram_business_id, count=5, limit=5)\n    Out[10]:\n    [IgProMedia(id=\'18027939643230671\', permalink=\'https://www.instagram.com/p/B38Xyp6nqsS/\'),\n     IgProMedia(id=\'17846368219941692\', permalink=\'https://www.instagram.com/p/B8gQCApHMT-/\'),\n     IgProMedia(id=\'17913531439230186\', permalink=\'https://www.instagram.com/p/Bop3AGOASfY/\'),\n     IgProMedia(id=\'17978630677077508\', permalink=\'https://www.instagram.com/p/BotSABoAn8E/\'),\n     IgProMedia(id=\'17955956875141196\', permalink=\'https://www.instagram.com/p/Bn-35GGl7YM/\')]\n\nGet data about a comment that an Business or Creator Account has been @mentioned in comment text::\n\n    In [11]: api.get_mentioned_comment_info(user_id=api.instagram_business_id, comment_id="17892250648466172")\n    Out[11]: IgProComment(id=\'17892250648466172\', timestamp=\'2020-02-24T09:15:16+0000\')\n\n\nGet data about a media object on which a Business or Creator Account has been @mentioned in a caption::\n\n    In [12]: api.get_mentioned_media_info(user_id=api.instagram_business_id, media_id="18027939643230671")\n    Out[12]: IgProMedia(id=\'18027939643230671\', permalink=\'https://www.instagram.com/p/B38Xyp6nqsS/\')\n\nNow you can publish instagram content if your app have publish permission.\n\nfor publish, you need create a container first, the make the container publish.\n\n.. code-block:: python\n\n    # create photo\n    >>> api.create_photo(\n            image_url="https://www.example.com/images/gugges.jpg",\n            caption="publish test",\n            location_id="7640348500",\n            user_tags=\'[{"username": "somebody", "x": 0.5, "y": 0.8}]\'\n        )\n    # IgProContainer(id=\'17877174857201040\', status_code=None)\n\n    # create video\n    >>> api.create_video(\n            video_url="https://www.example.com/videos/hungry-fonzes.mov",\n            caption="video test",\n            location_id="",\n            thumb_offset=5,\n        )\n    # IgProContainer(id=\'17877174857201041\', status_code=None)\n\nThen you can get container status, if container is ready, You can make it published.\n\n.. code-block:: python\n\n    >>> api.get_container_info(container_id="17877174857201040")\n    # IgProContainer(id=\'17877174857201040\', status_code=\'FINISHED\')\n\nThen you can publish it.\n\n.. code-block:: python\n\n    >>> api.publish_container(creation_id="17877174857201040")\n    # {\'id\': \'17892354025952911\'}\n\nIf success, will return the media id.\n\n\nFor now, Instagram accounts are limited to 25 API-published posts within a 24 hour moving period.\n\nSo you can get current limit info.\n\n.. code-block:: python\n\n    >>> api.get_publish_limit()\n    # IgProPublishLimit(quota_usage=4)\n\n==============================\nBase-Usage-Instagram Basic API\n==============================\n\nInstagram Basic Display API can be used to access any type of Instagram account but only provides read-access to basic data.\n\nYou need do authorize first, and get access token which has permission to retrieve data.\n\nAll docs on `Basic Display APi <https://developers.facebook.com/docs/instagram-basic-display-api>`_.\n\n-----------\nInitial Api\n-----------\n\nNow provide three methods to init api.\n\nIf you have long-lived access token, can just initial by token::\n\n    In[1]: from pyfacebook import IgBasicApi\n    In[2]: api = IgBasicApi(long_term_token="token")\n\nIf you have short-lived access token, can provide with app credentials::\n\n    In[3]: api = IgBasicApi(app_id="app id", app_secret="app secret", short_token="token")\n\nIf you want to authorized by user on hand. You can use authorize flow::\n\n    In[4]: api = IgBasicApi(app_id="app id", app_secret="app secret", initial_access_token=False)\n    In[5]: api.get_authorization_url()\n    Out[5]:\n    (\'https://api.instagram.com/oauth/authorize?response_type=code&client_id=app+id&redirect_uri=https%3A%2F%2Flocalhost%2F&scope=user_profile+user_media&state=PyFacebook\',\n     \'PyFacebook\')\n    # give permission and copy the redirect full url.\n    In[6]: api.exchange_access_token(response="the full url")\n\n--------\nGet Data\n--------\n\nYou can get user basic info::\n\n    In[7]: api.get_user_info()\n    Out[7]: IgBasicUser(id=\'17841406338772941\', username=\'ikroskun\')\n\nYou can get user medias::\n\n    In[7]: r = api.get_user_medias()\n    In[8]: r\n    Out[8]:\n    [IgBasicMedia(id=\'17846368219941692\', media_type=\'IMAGE\', permalink=\'https://www.instagram.com/p/B8gQCApHMT-/\'),\n     IgBasicMedia(id=\'18091893643133286\', media_type=\'IMAGE\', permalink=\'https://www.instagram.com/p/B8gPx-UnsjA/\'),\n     IgBasicMedia(id=\'18075344632131157\', media_type=\'VIDEO\', permalink=\'https://www.instagram.com/p/B38X8BzHsDi/\'),\n     IgBasicMedia(id=\'18027939643230671\', media_type=\'CAROUSEL_ALBUM\', permalink=\'https://www.instagram.com/p/B38Xyp6nqsS/\'),\n     IgBasicMedia(id=\'17861821972334188\', media_type=\'IMAGE\', permalink=\'https://www.instagram.com/p/BuGD8NmF4KI/\'),\n     IgBasicMedia(id=\'17864312515295083\', media_type=\'IMAGE\', permalink=\'https://www.instagram.com/p/BporjsCF6mt/\'),\n     IgBasicMedia(id=\'17924095942208544\', media_type=\'IMAGE\', permalink=\'https://www.instagram.com/p/BoqBgsNl5qT/\'),\n     IgBasicMedia(id=\'17896189813249754\', media_type=\'IMAGE\', permalink=\'https://www.instagram.com/p/Bop_Hz5FzyL/\'),\n     IgBasicMedia(id=\'17955956875141196\', media_type=\'CAROUSEL_ALBUM\', permalink=\'https://www.instagram.com/p/Bn-35GGl7YM/\'),\n     IgBasicMedia(id=\'17970645226046242\', media_type=\'IMAGE\', permalink=\'https://www.instagram.com/p/Bme0cU1giOH/\')]\n\nYou can get just one media info::\n\n    In[9]: r = basic_api.get_media_info(media_id="18027939643230671")\n    In[9]: r\n    Out[10]: IgBasicMedia(id=\'18027939643230671\', media_type=\'CAROUSEL_ALBUM\', permalink=\'https://www.instagram.com/p/B38Xyp6nqsS/\')\n\n\n=======\nSUPPORT\n=======\n\n``python-facebook-api`` had been being developed with Pycharm under the free JetBrains Open Source license(s) granted by JetBrains s.r.o.,\nhence I would like to express my thanks here.\n\n.. image:: docs/imgs/jetbrains.svg\n    :target: https://www.jetbrains.com/?from=sns-sdks/python-facebook\n    :alt: Jetbrains\n\n====\nTODO\n====\n\n------------\nNow features\n------------\n\nFacebook Api:\n\n- Page Info.\n- Page Picture Info.\n- Feed Info (public posts, published posts, tagged posts).\n- Comment Info.\n- Video Info.\n- Album Info.\n- Photo Info.\n- Live Video Info.\n\nInstagram Professional Api:\n\n- Other business account info and media.\n- Authorized business account info\n- Authorized account medias\n- Authorized account comments\n- Authorized account replies\n- Authorized account insights and media insights\n- Search hashtag id\n- Get hashtag info\n- Get top medias with hashtag\n- Get recent medias with hashtag\n- Get Authorized account recent searched hashtags\n- Get medias which tagged account\n- Get comment info mentioned user.\n- Get media info mentioned user.\n- Publish Content\n\nInstagram Basic display api:\n\n- Get user info\n- Get user medias\n- Get media info\n\n----\nTODO\n----\n\n- publish\n\n.. _access-token: https://developers.facebook.com/docs/facebook-login/access-tokens\n.. _authorization-manually: https://developers.facebook.com/docs/facebook-login/manually-build-a-login-flow',
     'author': 'Ikaros kun',
     'author_email': 'merle.liukun@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/sns-sdks/python-facebook',
```

### Comparing `python-facebook-api-0.9.5/PKG-INFO` & `python-facebook-api-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: python-facebook-api
-Version: 0.9.5
+Version: 0.9.6
 Summary: A simple Python wrapper around the Facebook Graph API
 Home-page: https://github.com/sns-sdks/python-facebook
 License: Apache-2.0
 Keywords: facebook-graph-api,facebook-sdk,instagram-api,instagram-sdk,facebook-api
 Author: Ikaros kun
 Author-email: merle.liukun@gmail.com
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: attrs (>=20.1.0,<21.0.0)
 Requires-Dist: cattrs (==1.0.0); python_version >= "2.7" and python_version < "2.8" or python_version >= "3.6" and python_version < "3.7"
```

