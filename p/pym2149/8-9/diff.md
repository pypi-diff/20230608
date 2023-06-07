# Comparing `tmp/pym2149-8.tar.gz` & `tmp/pym2149-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pym2149-8.tar", last modified: Sat Mar 21 18:22:49 2020, max compression
+gzip compressed data, was "dist/pym2149-9.tar", last modified: Sat May  9 22:36:21 2020, max compression
```

## Comparing `pym2149-8.tar` & `pym2149-9.tar`

### file list

```diff
@@ -1,136 +1,119 @@
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-03-21 18:22:49.000000 pym2149-8/
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-03-21 18:22:49.000000 pym2149-8/pym2149/
--rw-rw-r--   0 arc       (1000) arc       (1000)     4635 2020-03-01 19:39:29.000000 pym2149-8/pym2149/pitch.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2042 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_mix.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     7297 2020-03-21 17:26:41.000000 pym2149-8/pym2149/defaultconf.arid
--rw-rw-r--   0 arc       (1000) arc       (1000)     8494 2020-03-21 17:27:05.000000 pym2149-8/pym2149/midi.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2108 2020-03-01 19:39:29.000000 pym2149-8/pym2149/timerimpl.py
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-03-21 18:22:49.000000 pym2149-8/pym2149/native/
--rw-rw-r--   0 arc       (1000) arc       (1000)      132 2019-11-17 19:03:15.000000 pym2149-8/pym2149/native/calsa.pyxbld
--rw-rw-r--   0 arc       (1000) arc       (1000)     5522 2020-03-01 19:39:29.000000 pym2149-8/pym2149/native/calsa.pyx
--rw-rw-r--   0 arc       (1000) arc       (1000)     1264 2020-03-01 19:39:29.000000 pym2149-8/pym2149/native/resid.pyx
--rw-rw-r--   0 arc       (1000) arc       (1000)      966 2020-03-01 19:39:29.000000 pym2149-8/pym2149/native/ctime.pxd
--rw-rw-r--   0 arc       (1000) arc       (1000)      203 2020-03-01 19:39:29.000000 pym2149-8/pym2149/native/resid.pyxbld
--rw-rw-r--   0 arc       (1000) arc       (1000)      701 2020-03-01 19:39:29.000000 pym2149-8/pym2149/native/__init__.py
--rw-rw-r--   0 arc       (1000) arc       (1000)    19342 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_osc.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2626 2020-03-01 19:39:29.000000 pym2149-8/pym2149/mfp.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1201 2020-03-01 19:39:29.000000 pym2149-8/pym2149/txt.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1975 2020-03-21 17:27:10.000000 pym2149-8/pym2149/util.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2643 2020-03-01 19:39:29.000000 pym2149-8/pym2149/wav.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1340 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_lfsr.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      745 2020-03-01 19:39:29.000000 pym2149-8/pym2149/dsd.arid
--rw-rw-r--   0 arc       (1000) arc       (1000)     1145 2020-03-01 19:39:29.000000 pym2149-8/pym2149/lfsr.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     4075 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_reg.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      948 2020-03-01 19:39:29.000000 pym2149-8/pym2149/iface.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3284 2020-03-01 19:39:29.000000 pym2149-8/pym2149/budgie.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      820 2020-03-01 19:39:29.000000 pym2149-8/pym2149/txt.arid
--rw-rw-r--   0 arc       (1000) arc       (1000)     5377 2020-03-01 19:39:29.000000 pym2149-8/pym2149/program.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1780 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_channels.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     4180 2020-03-01 19:39:29.000000 pym2149-8/pym2149/mediation.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3205 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_pll.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3147 2020-03-01 19:39:29.000000 pym2149-8/pym2149/clock.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1729 2020-03-01 19:39:29.000000 pym2149-8/pym2149/boot.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     8442 2020-03-01 19:39:29.000000 pym2149-8/pym2149/channels.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      986 2020-03-01 19:39:29.000000 pym2149-8/pym2149/minblep.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     4002 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_lfo.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3444 2020-03-01 19:39:29.000000 pym2149-8/pym2149/pll.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     4962 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_pitch.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2507 2020-03-01 19:39:29.000000 pym2149-8/pym2149/dosound.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2279 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_clock.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2493 2020-03-01 19:39:29.000000 pym2149-8/pym2149/reg.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     6790 2020-03-01 19:39:29.000000 pym2149-8/pym2149/resid.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     4975 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_mediation.py
--rw-rw-r--   0 arc       (1000) arc       (1000)    10166 2020-03-07 12:14:32.000000 pym2149-8/pym2149/ymformat.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     4575 2020-03-01 19:39:29.000000 pym2149-8/pym2149/portaudio.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3609 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_timer.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      860 2020-03-01 19:39:29.000000 pym2149-8/pym2149/const.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1932 2020-03-01 19:39:29.000000 pym2149-8/pym2149/timer.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2866 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_out.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2952 2020-03-07 12:14:51.000000 pym2149-8/pym2149/test_expected.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     4889 2020-03-01 19:39:29.000000 pym2149-8/pym2149/lurlene.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3792 2020-03-01 19:39:29.000000 pym2149-8/pym2149/mix.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2044 2020-03-21 17:27:16.000000 pym2149-8/pym2149/ymplayer.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1236 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_dac.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2437 2020-03-01 19:39:29.000000 pym2149-8/pym2149/nod.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2327 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_speed.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2809 2020-03-01 19:39:29.000000 pym2149-8/pym2149/lfo.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2952 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_program.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2033 2020-03-01 19:39:29.000000 pym2149-8/pym2149/shapes.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1289 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_nod.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     5954 2020-03-01 19:39:29.000000 pym2149-8/pym2149/ym2149.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3778 2020-03-01 19:39:29.000000 pym2149-8/pym2149/dac.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3899 2020-03-01 19:39:29.000000 pym2149-8/pym2149/jackclient.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     8221 2020-03-01 19:39:29.000000 pym2149-8/pym2149/osc2.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1314 2020-03-17 19:10:08.000000 pym2149-8/pym2149/power.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     4629 2020-03-01 19:39:29.000000 pym2149-8/pym2149/buf.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     5499 2020-03-21 17:27:27.000000 pym2149-8/pym2149/config.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      761 2020-03-01 19:39:29.000000 pym2149-8/pym2149/realtime.arid
--rw-rw-r--   0 arc       (1000) arc       (1000)     1212 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_mfp.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      701 2020-03-01 19:39:29.000000 pym2149-8/pym2149/__init__.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     6992 2020-03-01 19:39:29.000000 pym2149-8/pym2149/out.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3220 2020-03-01 19:39:29.000000 pym2149-8/pym2149/test_ym2149.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     4074 2020-03-01 19:39:29.000000 pym2149-8/pym2149/vis.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3381 2020-03-01 19:39:29.000000 pym2149-8/pym2149/speed.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      800 2020-03-01 19:39:29.000000 pym2149-8/pym2149/initlogging.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1007 2020-03-01 19:39:29.000000 pym2149-8/bpmtool.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1512 2020-03-01 19:39:29.000000 pym2149-8/lc2txt.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1377 2020-03-01 19:39:29.000000 pym2149-8/ym2portaudio.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1497 2020-03-01 19:39:29.000000 pym2149-8/lc2wav.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1682 2020-03-01 19:39:29.000000 pym2149-8/dosound2jack.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1561 2020-03-01 19:39:29.000000 pym2149-8/midi2wav.py
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-03-21 18:22:49.000000 pym2149-8/spectrogram/
--rw-rw-r--   0 arc       (1000) arc       (1000)      978 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/noise5k+tone1.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      981 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/tone1k+noise5k.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      921 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/noise5k.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1095 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/tone1k+noise5k+tri1.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      979 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/tone1k,2k,3k,4k.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      920 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/tone250.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1188 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/pwm100.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      927 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/noise125k.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      919 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/tone1k.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      985 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/tone1-8.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      921 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/tone1k5.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      993 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/saw600.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      993 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/tri650.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      825 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/__init__.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1166 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/pwm250.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1294 2020-03-01 19:39:29.000000 pym2149-8/spectrogram/sin1k.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1370 2020-03-01 19:39:29.000000 pym2149-8/ym2wav.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1401 2020-03-01 19:39:29.000000 pym2149-8/dosound2wav.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1530 2020-03-21 18:22:48.000000 pym2149-8/setup.py
--rw-rw-r--   0 arc       (1000) arc       (1000)       67 2020-03-21 18:22:49.000000 pym2149-8/setup.cfg
--rw-rw-r--   0 arc       (1000) arc       (1000)     1373 2020-03-01 19:39:29.000000 pym2149-8/ym2txt.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1693 2020-03-01 19:39:29.000000 pym2149-8/dosound2txt.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1374 2020-03-01 19:39:29.000000 pym2149-8/ym2jack.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      634 2020-03-01 19:39:29.000000 pym2149-8/README.md
--rw-rw-r--   0 arc       (1000) arc       (1000)     1600 2020-03-01 19:39:29.000000 pym2149-8/midi2jack.py
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-03-21 18:22:49.000000 pym2149-8/ymtests/
--rw-rw-r--   0 arc       (1000) arc       (1000)      931 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qenvpzer.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3075 2020-03-01 19:39:29.000000 pym2149-8/ymtests/mkdsd.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      856 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qmtreset.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      881 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qtonpzer.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      912 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qbmixenv.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      879 2020-03-01 19:39:29.000000 pym2149-8/ymtests/dosound0.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1025 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qtonflip.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      891 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qtonpbuf.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      880 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qenvrbuf.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      848 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qnoipbuf.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      978 2020-03-01 19:39:29.000000 pym2149-8/ymtests/dosound1.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      850 2020-03-01 19:39:29.000000 pym2149-8/ymtests/dosound2.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1036 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qanlgmix.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      915 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qenvpbuf.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1026 2020-03-01 19:39:29.000000 pym2149-8/ymtests/test_mkdsd.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      823 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qnoispec.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      863 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qmnreset.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      701 2020-03-01 19:39:29.000000 pym2149-8/ymtests/__init__.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      999 2020-03-01 19:39:29.000000 pym2149-8/ymtests/qtinheri.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1695 2020-03-01 19:39:29.000000 pym2149-8/dsd2wav.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1093 2020-03-21 18:22:49.000000 pym2149-8/PKG-INFO
--rw-rw-r--   0 arc       (1000) arc       (1000)     1737 2020-03-01 19:39:29.000000 pym2149-8/lc2jack.py
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-03-21 18:22:49.000000 pym2149-8/pym2149.egg-info/
--rw-rw-r--   0 arc       (1000) arc       (1000)        1 2020-03-21 18:22:49.000000 pym2149-8/pym2149.egg-info/dependency_links.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)       83 2020-03-21 18:22:49.000000 pym2149-8/pym2149.egg-info/requires.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      537 2020-03-21 18:22:49.000000 pym2149-8/pym2149.egg-info/entry_points.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)     2546 2020-03-21 18:22:49.000000 pym2149-8/pym2149.egg-info/SOURCES.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      157 2020-03-21 18:22:49.000000 pym2149-8/pym2149.egg-info/top_level.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)     1093 2020-03-21 18:22:49.000000 pym2149-8/pym2149.egg-info/PKG-INFO
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-05-09 22:36:21.000000 pym2149-9/
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-05-09 22:36:21.000000 pym2149-9/pym2149/
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4642 2020-03-28 20:59:38.000000 pym2149-9/pym2149/pitch.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     7552 2020-04-13 18:10:16.000000 pym2149-9/pym2149/defaultconf.arid
+-rw-rw-r--   0 arc       (1000) arc       (1000)     8494 2020-03-21 17:27:05.000000 pym2149-9/pym2149/midi.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2108 2020-03-01 19:39:29.000000 pym2149-9/pym2149/timerimpl.py
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-05-09 22:36:21.000000 pym2149-9/pym2149/native/
+-rw-rw-r--   0 arc       (1000) arc       (1000)      132 2019-11-17 19:03:15.000000 pym2149-9/pym2149/native/calsa.pyxbld
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5522 2020-03-01 19:39:29.000000 pym2149-9/pym2149/native/calsa.pyx
+-rw-rw-r--   0 arc       (1000) arc       (1000)   339466 2020-05-09 22:36:20.000000 pym2149-9/pym2149/native/resid.cpp
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1264 2020-03-01 19:39:29.000000 pym2149-9/pym2149/native/resid.pyx
+-rw-rw-r--   0 arc       (1000) arc       (1000)      966 2020-03-01 19:39:29.000000 pym2149-9/pym2149/native/ctime.pxd
+-rw-rw-r--   0 arc       (1000) arc       (1000)      203 2020-03-01 19:39:29.000000 pym2149-9/pym2149/native/resid.pyxbld
+-rw-rw-r--   0 arc       (1000) arc       (1000)      701 2020-03-01 19:39:29.000000 pym2149-9/pym2149/native/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)   374340 2020-05-09 22:36:19.000000 pym2149-9/pym2149/native/calsa.c
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2626 2020-03-01 19:39:29.000000 pym2149-9/pym2149/mfp.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1201 2020-03-01 19:39:29.000000 pym2149-9/pym2149/txt.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1975 2020-03-21 17:27:10.000000 pym2149-9/pym2149/util.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2643 2020-03-01 19:39:29.000000 pym2149-9/pym2149/wav.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      745 2020-03-01 19:39:29.000000 pym2149-9/pym2149/dsd.arid
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1145 2020-03-01 19:39:29.000000 pym2149-9/pym2149/lfsr.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      948 2020-03-01 19:39:29.000000 pym2149-9/pym2149/iface.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3284 2020-03-01 19:39:29.000000 pym2149-9/pym2149/budgie.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      820 2020-03-01 19:39:29.000000 pym2149-9/pym2149/txt.arid
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5377 2020-03-01 19:39:29.000000 pym2149-9/pym2149/program.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4180 2020-03-01 19:39:29.000000 pym2149-9/pym2149/mediation.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3147 2020-03-01 19:39:29.000000 pym2149-9/pym2149/clock.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1729 2020-03-01 19:39:29.000000 pym2149-9/pym2149/boot.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     8442 2020-03-01 19:39:29.000000 pym2149-9/pym2149/channels.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      986 2020-03-01 19:39:29.000000 pym2149-9/pym2149/minblep.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3444 2020-03-01 19:39:29.000000 pym2149-9/pym2149/pll.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2507 2020-03-01 19:39:29.000000 pym2149-9/pym2149/dosound.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2493 2020-03-01 19:39:29.000000 pym2149-9/pym2149/reg.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     6790 2020-03-01 19:39:29.000000 pym2149-9/pym2149/resid.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)    10166 2020-03-07 12:14:32.000000 pym2149-9/pym2149/ymformat.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4575 2020-03-01 19:39:29.000000 pym2149-9/pym2149/portaudio.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      860 2020-03-01 19:39:29.000000 pym2149-9/pym2149/const.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1932 2020-03-01 19:39:29.000000 pym2149-9/pym2149/timer.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4889 2020-03-01 19:39:29.000000 pym2149-9/pym2149/lurlene.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3792 2020-03-01 19:39:29.000000 pym2149-9/pym2149/mix.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2044 2020-03-21 17:27:16.000000 pym2149-9/pym2149/ymplayer.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2437 2020-03-01 19:39:29.000000 pym2149-9/pym2149/nod.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2809 2020-03-01 19:39:29.000000 pym2149-9/pym2149/lfo.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2033 2020-03-01 19:39:29.000000 pym2149-9/pym2149/shapes.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5954 2020-03-01 19:39:29.000000 pym2149-9/pym2149/ym2149.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3778 2020-03-01 19:39:29.000000 pym2149-9/pym2149/dac.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3899 2020-03-01 19:39:29.000000 pym2149-9/pym2149/jackclient.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     8221 2020-03-01 19:39:29.000000 pym2149-9/pym2149/osc2.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1314 2020-03-17 19:10:08.000000 pym2149-9/pym2149/power.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4629 2020-03-01 19:39:29.000000 pym2149-9/pym2149/buf.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5559 2020-05-09 14:36:31.000000 pym2149-9/pym2149/config.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      761 2020-03-01 19:39:29.000000 pym2149-9/pym2149/realtime.arid
+-rw-rw-r--   0 arc       (1000) arc       (1000)      701 2020-03-01 19:39:29.000000 pym2149-9/pym2149/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     6992 2020-03-01 19:39:29.000000 pym2149-9/pym2149/out.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4074 2020-03-01 19:39:29.000000 pym2149-9/pym2149/vis.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3381 2020-03-01 19:39:29.000000 pym2149-9/pym2149/speed.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      800 2020-03-01 19:39:29.000000 pym2149-9/pym2149/initlogging.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1007 2020-03-01 19:39:29.000000 pym2149-9/bpmtool.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1512 2020-03-01 19:39:29.000000 pym2149-9/lc2txt.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1377 2020-03-01 19:39:29.000000 pym2149-9/ym2portaudio.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1497 2020-03-01 19:39:29.000000 pym2149-9/lc2wav.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1682 2020-03-01 19:39:29.000000 pym2149-9/dosound2jack.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1561 2020-03-01 19:39:29.000000 pym2149-9/midi2wav.py
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-05-09 22:36:21.000000 pym2149-9/spectrogram/
+-rw-rw-r--   0 arc       (1000) arc       (1000)      978 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/noise5k+tone1.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      981 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/tone1k+noise5k.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      921 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/noise5k.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1095 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/tone1k+noise5k+tri1.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      979 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/tone1k,2k,3k,4k.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      920 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/tone250.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1188 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/pwm100.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      927 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/noise125k.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      919 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/tone1k.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      985 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/tone1-8.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      921 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/tone1k5.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      993 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/saw600.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      993 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/tri650.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      825 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1166 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/pwm250.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1294 2020-03-01 19:39:29.000000 pym2149-9/spectrogram/sin1k.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1370 2020-03-01 19:39:29.000000 pym2149-9/ym2wav.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1401 2020-03-01 19:39:29.000000 pym2149-9/dosound2wav.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3998 2020-05-09 22:36:17.000000 pym2149-9/setup.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)       67 2020-05-09 22:36:21.000000 pym2149-9/setup.cfg
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1373 2020-03-01 19:39:29.000000 pym2149-9/ym2txt.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1693 2020-03-01 19:39:29.000000 pym2149-9/dosound2txt.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)       69 2020-05-09 22:36:17.000000 pym2149-9/pyproject.toml
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1374 2020-03-01 19:39:29.000000 pym2149-9/ym2jack.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      634 2020-03-01 19:39:29.000000 pym2149-9/README.md
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1600 2020-03-01 19:39:29.000000 pym2149-9/midi2jack.py
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-05-09 22:36:21.000000 pym2149-9/ymtests/
+-rw-rw-r--   0 arc       (1000) arc       (1000)      931 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qenvpzer.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3075 2020-03-01 19:39:29.000000 pym2149-9/ymtests/mkdsd.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      856 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qmtreset.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      881 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qtonpzer.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      912 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qbmixenv.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      879 2020-03-01 19:39:29.000000 pym2149-9/ymtests/dosound0.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1025 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qtonflip.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      891 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qtonpbuf.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      880 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qenvrbuf.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      848 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qnoipbuf.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      978 2020-03-01 19:39:29.000000 pym2149-9/ymtests/dosound1.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      850 2020-03-01 19:39:29.000000 pym2149-9/ymtests/dosound2.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1036 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qanlgmix.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      915 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qenvpbuf.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      823 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qnoispec.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      863 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qmnreset.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      701 2020-03-01 19:39:29.000000 pym2149-9/ymtests/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      999 2020-03-01 19:39:29.000000 pym2149-9/ymtests/qtinheri.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1695 2020-03-01 19:39:29.000000 pym2149-9/dsd2wav.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1093 2020-05-09 22:36:21.000000 pym2149-9/PKG-INFO
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1735 2020-03-28 22:25:07.000000 pym2149-9/lc2jack.py
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-05-09 22:36:21.000000 pym2149-9/pym2149.egg-info/
+-rw-rw-r--   0 arc       (1000) arc       (1000)        1 2020-05-09 22:36:20.000000 pym2149-9/pym2149.egg-info/dependency_links.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       83 2020-05-09 22:36:20.000000 pym2149-9/pym2149.egg-info/requires.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      537 2020-05-09 22:36:20.000000 pym2149-9/pym2149.egg-info/entry_points.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2175 2020-05-09 22:36:20.000000 pym2149-9/pym2149.egg-info/SOURCES.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      157 2020-05-09 22:36:20.000000 pym2149-9/pym2149.egg-info/top_level.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1093 2020-05-09 22:36:20.000000 pym2149-9/pym2149.egg-info/PKG-INFO
```

### Comparing `pym2149-8/pym2149/pitch.py` & `pym2149-9/pym2149/pitch.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     @types(Context, DI)
     def __init__(self, context, di):
         self.context = context
         self.di = di
 
     def __getattr__(self, name):
-        return getattr(self.di(self.context.tuning), name)
+        return getattr(self.di(self.context.get('tuning')), name)
 
     def dispose(self):
         pass
 
 class EqualTemperament:
 
     @types(Config)
```

### Comparing `pym2149-8/pym2149/defaultconf.arid` & `pym2149-9/pym2149/defaultconf.arid`

 * *Files 3% similar despite different names*

```diff
@@ -179,7 +179,10 @@
 : If true, show periods in visualisation instead of MIDI notes.
 
 SID enabled = false
 : If true, integrate with reSID shared library.
 
 SID clock = $global(.resid.PAL)
 : The clock to use for reSID.
+
+Lurlene lazy = false
+: If true Lurlene will lookup objects in globals at runtime, so you don't have to update sections and everything in-between for your changes to be audible. This feature is currently experimental, it's usable but there are many bugs.
```

### Comparing `pym2149-8/pym2149/midi.py` & `pym2149-9/pym2149/midi.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/timerimpl.py` & `pym2149-9/pym2149/timerimpl.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/native/calsa.pyx` & `pym2149-9/pym2149/native/calsa.pyx`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/native/resid.pyx` & `pym2149-9/pym2149/native/resid.pyx`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/native/ctime.pxd` & `pym2149-9/pym2149/native/ctime.pxd`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/native/__init__.py` & `pym2149-9/pym2149/native/__init__.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/mfp.py` & `pym2149-9/pym2149/mfp.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/txt.py` & `pym2149-9/pym2149/txt.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/util.py` & `pym2149-9/pym2149/util.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/wav.py` & `pym2149-9/pym2149/wav.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/dsd.arid` & `pym2149-9/pym2149/dsd.arid`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/lfsr.py` & `pym2149-9/pym2149/lfsr.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/iface.py` & `pym2149-9/pym2149/iface.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/budgie.py` & `pym2149-9/pym2149/budgie.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/txt.arid` & `pym2149-9/pym2149/txt.arid`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/program.py` & `pym2149-9/pym2149/program.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/mediation.py` & `pym2149-9/pym2149/mediation.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/test_pll.py` & `pym2149-9/pym2149/pll.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,110 +11,89 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
-from .pll import PLL
-import unittest
-
-dp = 6
-
-class Event:
-
-    def __init__(self, eventtime):
-        self.eventtime = eventtime
-
-    def __repr__(self):
-        return "%s(%r)" % (type(self).__name__, round(self.eventtime, dp))
-
-class TestPLL(unittest.TestCase):
-
-    updaterate = 50
-    updateperiod = 1 / updaterate
-    plltargetpos = updateperiod / 2
-    pllalpha = .2
-
-    def doit(self, positionshift, *offsetlists):
-        pll = PLL(self)
-        pll.start()
-        eventlists = []
-        for u, offsets in enumerate(offsetlists):
-            updatetime = pll.mark + self.updateperiod * (u + .5)
-            eventlists.append([Event(updatetime + offset) for offset in offsets])
-        updates = []
-        for events in eventlists:
-            for event in events:
-                while pll.exclusivewindowend <= event.eventtime:
-                    updates.append(pll.takeupdateimpl(pll.exclusivewindowend).events)
-                pll.event(event.eventtime, event, True)
-        ewe = pll.exclusivewindowend
-        updates.append(pll.takeupdateimpl(ewe).events)
-        self.assertEqual(eventlists, updates)
-        self.assertEqual(positionshift, round(ewe - (pll.mark + self.updateperiod * len(eventlists)), dp))
-
-    def test_0perfecttiming(self):
-        self.doit(0,
-            [0],
-            [0],
-            [],
-            [0],
-            [0, 0],
-            [0],
-        )
-
-    def test_1consistentlylate(self):
-        self.doit(.002952,
-            [.005],
-            [.005],
-            [],
-            [.005],
-            [.005, .005],
-            [.005],
-        )
-
-    def test_2consistentlyearly(self):
-        self.doit(-.002952,
-            [-.005],
-            [-.005],
-            [],
-            [-.005],
-            [-.005, -.005],
-            [-.005],
-        )
-
-    def test_3hundredthgranularity(self):
-        self.doit(-.004959,
-            [0],
-            [-.01],
-            [0],
-            [-.01],
-            [-.01],
-            [0],
-            [-.01],
-            [0],
-        )
-
-    def test_4hundredthgranularityaltsync(self):
-        self.doit(.003701,
-            [0, .009],
-            [],
-            [0, .01],
-            [.01],
-            [],
-            [0, .01],
-            [],
-            [0],
-        )
-
-    def test_5hundredthgranularityaltshift(self):
-        self.doit(.002891,
-            [.009],
-            [0],
-            [.01],
-            [0],
-            [0],
-            [.01],
-            [0],
-            [.01],
-        )
+from .iface import Config
+from diapyr import types
+from .util import EMA
+import time, logging
+
+log = logging.getLogger(__name__)
+
+class Update:
+
+    def __init__(self, events, idealtaketime):
+        self.events = events
+        self.idealtaketime = idealtaketime
+
+class PLL:
+
+    @types(Config)
+    def __init__(self, config):
+        self.updateperiod = 1 / config.updaterate
+        self.targetpos = float(config.plltargetpos)
+        self.medianshiftema = EMA(float(config.pllalpha), None)
+
+    def start(self):
+        self.events = []
+        self.updates = []
+        self.medianshiftema.value = 0
+        self.mark = time.time()
+        self.windowindex = 0
+        self.nextwindow()
+
+    def stop(self):
+        pass
+
+    def nextwindow(self):
+        self.windowindex += 1
+        self.exclusivewindowend = self.mark + self.windowindex * self.updateperiod + self.medianshiftema.value
+
+    def event(self, eventtime, event, significant):
+        self.events.append((eventtime, event, significant))
+
+    def closeupdate(self):
+        inclusivewindowstart = self.exclusivewindowend - self.updateperiod
+        targettime = inclusivewindowstart + self.targetpos
+        shifts = []
+        i = 0
+        for eventtime, _, significant in self.events:
+            if eventtime >= self.exclusivewindowend:
+                break
+            if significant and eventtime >= inclusivewindowstart:
+                shifts.append(self.medianshiftema.value + eventtime - targettime)
+            # If eventtime < inclusivewindowstart we consume the event without harvesting its shift.
+            i += 1
+        update = []
+        for eventtime, event, _ in self.events[:i]:
+            event.offset = eventtime - inclusivewindowstart
+            update.append(event)
+        self.updates.append(update)
+        del self.events[:i]
+        if shifts:
+            n = len(shifts)
+            if n & 1: # Odd.
+                medianshift = shifts[(n - 1) // 2]
+            else:
+                midindex = n // 2
+                medianshift = (shifts[midindex - 1] + shifts[midindex]) / 2
+            self.medianshiftema(medianshift)
+        self.nextwindow()
+
+    def takeupdate(self):
+        return self.takeupdateimpl(time.time())
+
+    def takeupdateimpl(self, now):
+        while now >= self.exclusivewindowend: # No more events can qualify for this window.
+            self.closeupdate()
+        copy = self.updates[:]
+        n = len(copy)
+        del self.updates[:n] # Not actually necessary to use n, as only we call closeupdate.
+        if 1 == n:
+            update, = copy
+        else:
+            log.warning("Yielding %s updates as one.", n)
+            update = sum(copy, [])
+        return Update(update, self.exclusivewindowend)
```

### Comparing `pym2149-8/pym2149/clock.py` & `pym2149-9/pym2149/clock.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/boot.py` & `pym2149-9/pym2149/boot.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/channels.py` & `pym2149-9/pym2149/channels.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/minblep.py` & `pym2149-9/pym2149/minblep.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/dosound.py` & `pym2149-9/pym2149/dosound.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/reg.py` & `pym2149-9/pym2149/reg.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/resid.py` & `pym2149-9/pym2149/resid.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/ymformat.py` & `pym2149-9/pym2149/ymformat.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/portaudio.py` & `pym2149-9/pym2149/portaudio.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/const.py` & `pym2149-9/pym2149/const.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/timer.py` & `pym2149-9/pym2149/timer.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/lurlene.py` & `pym2149-9/pym2149/lurlene.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/mix.py` & `pym2149-9/pym2149/mix.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/ymplayer.py` & `pym2149-9/pym2149/ymplayer.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/test_dac.py` & `pym2149-9/spectrogram/sin1k.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,28 +11,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
-import unittest
-from .dac import Dac
-from .nod import BufNode, Block
-from .shapes import signaldtype
+from . import E, V
+from pym2149.dac import SinusEffect
+from spectrogram import silence
+
+# TODO LATER: Find out why the result appears shifted a few samples to the right.
+class Sin1k:
+
+    level = V('75x15//,0')
+
+    def on(self, ym, frame):
+        ym.level = self.level[frame]
+        if frame < 1:
+            chan = ym[0]._chan
+            timer = ym._chip.timers[chan]
+            timer.effect.value = SinusEffect(ym._chip.fixedlevels[chan])
+            timer.freq.value = 1000 * 4 # FIXME: It should know wavelength from effect.
 
-class Ramps(BufNode):
-
-    dtype = signaldtype
-
-    def __init__(self):
-        super().__init__(self.dtype)
-
-    def callimpl(self):
-        for i in range(self.block.framecount):
-            self.blockbuf.fillpart(i, i + 1, self.dtype(i))
-
-class TestDac(unittest.TestCase):
-
-    def test_works(self):
-        d = Dac(Ramps(), 16, 1)
-        self.assertEqual([d.leveltopeaktopeak[v] for v in range(32)], d.call(Block(32)).tolist())
+sections = [[E(Sin1k, '2'), silence, silence]]
+speed = 50
```

### Comparing `pym2149-8/pym2149/nod.py` & `pym2149-9/pym2149/nod.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/lfo.py` & `pym2149-9/pym2149/lfo.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/shapes.py` & `pym2149-9/pym2149/shapes.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/test_nod.py` & `pym2149-9/spectrogram/saw600.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,33 +11,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
-import unittest
-from .nod import Node, Block
+from . import E
+from spectrogram import silence
 
-class MyNode(Node):
+class Saw600:
 
-    def __init__(self):
-        super().__init__()
-        self.x = 0
+    shape = 0x08
 
-    def callimpl(self):
-        x = self.block.framecount + self.x
-        self.x += 1
-        return x
+    def on(self, ym):
+        ym.envflag = True
+        if ym.envshape != self.shape:
+            ym.envshape = self.shape
+        ym.envfreq = 600
 
-class TestNode(unittest.TestCase):
-
-    def test_works(self):
-        n = MyNode()
-        b1 = Block(10)
-        b2 = Block(20)
-        for _ in range(2):
-            self.assertEqual(10, n.call(b1))
-        for _ in range(2):
-            self.assertEqual(21, n.call(b2))
-        for _ in range(2):
-            self.assertEqual(12, n.call(b1))
+sections = [[E(Saw600, '1.5'), silence, silence]]
+speed = 50
```

### Comparing `pym2149-8/pym2149/ym2149.py` & `pym2149-9/pym2149/ym2149.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/dac.py` & `pym2149-9/pym2149/dac.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/jackclient.py` & `pym2149-9/pym2149/jackclient.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/osc2.py` & `pym2149-9/pym2149/osc2.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/power.py` & `pym2149-9/pym2149/power.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/buf.py` & `pym2149-9/pym2149/buf.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/config.py` & `pym2149-9/pym2149/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,13 +149,13 @@
 class ConfigImpl(Config, lurlene.iface.Config):
 
     def __init__(self, context):
         self.pRiVaTe = context
 
     def __getattr__(self, name):
         try:
-            return self[(name,)].unravel()
+            return self[(name,)].unravel() # TODO: Refactor to allow arbitrarily deep dotted notation.
         except NoSuchPathException:
             raise AttributeError(name)
 
     def __getitem__(self, path):
         return self.pRiVaTe.resolved(*(namespace,) + path)
```

### Comparing `pym2149-8/pym2149/realtime.arid` & `pym2149-9/pym2149/realtime.arid`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/test_mfp.py` & `pym2149-9/spectrogram/tone1k,2k,3k,4k.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,24 +11,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
-import unittest
-from .mfp import MFPTimer
+from . import E, V
+from spectrogram import silence
 
-class TestMFPTimer(unittest.TestCase):
+class T:
 
-    def test_setfreq(self):
-        timer = MFPTimer()
-        timer.freq.value = 1000
-        self.assertEqual(2460, timer.getnormperiod()) # Close.
-        timer.freq.value = 100
-        self.assertEqual(24576, timer.getnormperiod()) # Exact.
+    def on(self, ym, freq, frame):
+        ym.toneflag = True
+        ym.level = 15
+        ym.tonefreq = freq[frame]
 
-    def test_zerotdr(self):
-        t = MFPTimer()
-        t.control_data.value = 3, 0
-        self.assertEqual(300, t.getfreq())
-        self.assertEqual((3, 0), t.findtcrtdr(300))
+sections = [[E(T, '.25', freq = V('1000 2000 3000 4000').of(.25)), silence, silence]]
+speed = 50
```

### Comparing `pym2149-8/pym2149/__init__.py` & `pym2149-9/pym2149/__init__.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/out.py` & `pym2149-9/pym2149/out.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/vis.py` & `pym2149-9/pym2149/vis.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/speed.py` & `pym2149-9/pym2149/speed.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149/initlogging.py` & `pym2149-9/pym2149/initlogging.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/bpmtool.py` & `pym2149-9/bpmtool.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/lc2txt.py` & `pym2149-9/lc2txt.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ym2portaudio.py` & `pym2149-9/ym2portaudio.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/lc2wav.py` & `pym2149-9/lc2wav.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/dosound2jack.py` & `pym2149-9/dosound2jack.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/midi2wav.py` & `pym2149-9/midi2wav.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/spectrogram/noise5k+tone1.py` & `pym2149-9/spectrogram/noise5k+tone1.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/spectrogram/tone1k+noise5k.py` & `pym2149-9/spectrogram/tone1k+noise5k.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/spectrogram/noise5k.py` & `pym2149-9/spectrogram/noise5k.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/spectrogram/tone1k+noise5k+tri1.py` & `pym2149-9/spectrogram/tone1k+noise5k+tri1.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/spectrogram/tone1k,2k,3k,4k.py` & `pym2149-9/spectrogram/tri650.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
-from . import E, V
+from . import E
 from spectrogram import silence
 
-class T:
+class Tri650:
 
-    def on(self, ym, freq, frame):
-        ym.toneflag = True
-        ym.level = 15
-        ym.tonefreq = freq[frame]
+    shape = 0x0a
 
-sections = [[E(T, '.25', freq = V('1000 2000 3000 4000').of(.25)), silence, silence]]
+    def on(self, ym):
+        ym.envflag = True
+        if ym.envshape != self.shape:
+            ym.envshape = self.shape
+        ym.envfreq = 650
+
+sections = [[E(Tri650, '1.5'), silence, silence]]
 speed = 50
```

### Comparing `pym2149-8/spectrogram/tone250.py` & `pym2149-9/spectrogram/tone250.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/spectrogram/pwm100.py` & `pym2149-9/spectrogram/pwm100.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/spectrogram/noise125k.py` & `pym2149-9/spectrogram/noise125k.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/spectrogram/tone1k.py` & `pym2149-9/spectrogram/tone1k.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/spectrogram/tone1-8.py` & `pym2149-9/spectrogram/tone1-8.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/spectrogram/tone1k5.py` & `pym2149-9/spectrogram/tone1k5.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/spectrogram/saw600.py` & `pym2149-9/spectrogram/pwm250.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
 from . import E
+from pym2149.dac import PWMEffect
 from spectrogram import silence
 
-class Saw600:
+class PWM250:
 
-    shape = 0x08
+    def on(self, ym, frame):
+        ym.toneflag = True
+        ym.level = 15
+        ym.tonefreq = 250
+        if frame < 1:
+            chan = ym[0]._chan
+            timer = ym._chip.timers[chan]
+            timer.effect.value = PWMEffect(ym._chip.fixedlevels[chan])
+            timer.freq.value = 250
 
-    def on(self, ym):
-        ym.envflag = True
-        if ym.envshape != self.shape:
-            ym.envshape = self.shape
-        ym.envfreq = 600
-
-sections = [[E(Saw600, '1.5'), silence, silence]]
+sections = [[E(PWM250, '1.5'), silence, silence]]
 speed = 50
```

### Comparing `pym2149-8/spectrogram/tri650.py` & `pym2149-9/ymtests/qenvrbuf.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,22 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
-from . import E
-from spectrogram import silence
-
-class Tri650:
-
-    shape = 0x0a
-
-    def on(self, ym):
-        ym.envflag = True
-        if ym.envshape != self.shape:
-            ym.envshape = self.shape
-        ym.envfreq = 650
-
-sections = [[E(Tri650, '1.5'), silence, silence]]
-speed = 50
+mixer.put() # All off.
+A_level.put(0x10) # Variable level.
+E_fine.put(0x77)
+E_rough.put(0x0e)
+for i in range(10):
+  E_shape.put(0x0a) # Triangle.
+  sleep(2 + i)
+A_level.put(0x00)
```

### Comparing `pym2149-8/spectrogram/__init__.py` & `pym2149-9/spectrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/spectrogram/pwm250.py` & `pym2149-9/ymtests/qmtreset.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,25 +11,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
-from . import E
-from pym2149.dac import PWMEffect
-from spectrogram import silence
-
-class PWM250:
-
-    def on(self, ym, frame):
-        ym.toneflag = True
-        ym.level = 15
-        ym.tonefreq = 250
-        if frame < 1:
-            chan = ym[0]._chan
-            timer = ym._chip.timers[chan]
-            timer.effect.value = PWMEffect(ym._chip.fixedlevels[chan])
-            timer.freq.value = 250
-
-sections = [[E(PWM250, '1.5'), silence, silence]]
-speed = 50
+A_fine.put(0x00)
+A_rough.put(0x07)
+A_level.put(0x0f)
+for i in range(10):
+  mixer.put()
+  sleep(2 + i)
+  mixer.put(A_tone)
+  sleep(2 + i)
+A_level.put(0x00)
```

### Comparing `pym2149-8/ym2wav.py` & `pym2149-9/ym2wav.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/dosound2wav.py` & `pym2149-9/dosound2wav.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ym2txt.py` & `pym2149-9/ym2txt.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/dosound2txt.py` & `pym2149-9/dosound2txt.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ym2jack.py` & `pym2149-9/ym2jack.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/README.md` & `pym2149-9/README.md`

 * *Files identical despite different names*

### Comparing `pym2149-8/midi2jack.py` & `pym2149-9/midi2jack.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ymtests/qenvpzer.py` & `pym2149-9/ymtests/qenvpzer.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ymtests/mkdsd.py` & `pym2149-9/ymtests/mkdsd.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ymtests/qmtreset.py` & `pym2149-9/ymtests/qmnreset.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
-A_fine.put(0x00)
-A_rough.put(0x07)
-A_level.put(0x0f)
+N_period.put(0x1f)
 for i in range(10):
   mixer.put()
+  A_level.put(0x0d)
   sleep(2 + i)
-  mixer.put(A_tone)
+  A_level.put(0x0f)
+  mixer.put(A_noise)
   sleep(2 + i)
 A_level.put(0x00)
```

### Comparing `pym2149-8/ymtests/qtonpzer.py` & `pym2149-9/ymtests/qtonpzer.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ymtests/qbmixenv.py` & `pym2149-9/ymtests/qbmixenv.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ymtests/dosound0.py` & `pym2149-9/ymtests/dosound0.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ymtests/qtonflip.py` & `pym2149-9/ymtests/qtonflip.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ymtests/qtonpbuf.py` & `pym2149-9/ymtests/qtonpbuf.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ymtests/qenvrbuf.py` & `pym2149-9/ymtests/qanlgmix.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
 mixer.put() # All off.
-A_level.put(0x10) # Variable level.
-E_fine.put(0x77)
-E_rough.put(0x0e)
-for i in range(10):
-  E_shape.put(0x0a) # Triangle.
-  sleep(2 + i)
-A_level.put(0x00)
+def reset():
+  for l in A_level, B_level, C_level:
+    l.put(0x0d) # Half amplitude.
+reset()
+sleep(50) # Allow it to settle at DC 0.
+for a in range(0x10):
+  for b in range(0x10):
+    for c in range(0x10):
+      A_level.put(a)
+      B_level.put(b)
+      C_level.put(c)
+      sleep(2)
+      reset()
+      sleep(2)
```

### Comparing `pym2149-8/ymtests/qnoipbuf.py` & `pym2149-9/ymtests/qnoipbuf.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ymtests/dosound1.py` & `pym2149-9/ymtests/dosound1.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ymtests/dosound2.py` & `pym2149-9/ymtests/dosound2.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/ymtests/qanlgmix.py` & `pym2149-9/ymtests/qenvpbuf.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,21 +12,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
 mixer.put() # All off.
-def reset():
-  for l in A_level, B_level, C_level:
-    l.put(0x0d) # Half amplitude.
-reset()
-sleep(50) # Allow it to settle at DC 0.
-for a in range(0x10):
-  for b in range(0x10):
-    for c in range(0x10):
-      A_level.put(a)
-      B_level.put(b)
-      C_level.put(c)
-      sleep(2)
-      reset()
-      sleep(2)
+A_level.put(0x10) # Variable level.
+E_shape.put(0x0a) # Triangle.
+E_fine.put(0x00)
+for i in range(20):
+  E_rough.put(0x05)
+  sleep(2 + i)
+  E_rough.put(0x02)
+  sleep(2 + i)
+A_level.put(0x00)
```

### Comparing `pym2149-8/ymtests/qenvpbuf.py` & `pym2149-9/ymtests/qnoispec.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
-mixer.put() # All off.
-A_level.put(0x10) # Variable level.
-E_shape.put(0x0a) # Triangle.
-E_fine.put(0x00)
-for i in range(20):
-  E_rough.put(0x05)
-  sleep(2 + i)
-  E_rough.put(0x02)
-  sleep(2 + i)
-A_level.put(0x00)
+mixer.put(A_noise)
+for p in range(0x20):
+  A_level.put(0x0f)
+  N_period.put(p)
+  sleep(48)
+  A_level.put(0x00)
+  sleep(2)
```

### Comparing `pym2149-8/ymtests/test_mkdsd.py` & `pym2149-9/ymtests/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,20 +11,7 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
-import unittest
-from .mkdsd import Data
-
-class TestReg(unittest.TestCase):
-
-    def test_anim(self):
-        d = Data()
-        r = d.reg()
-        d.setprev(0)
-        self.assertEqual(0, d.totalticks)
-        r.anim(2, 5)
-        # We did a whole cycle to decide it never stops:
-        self.assertEqual(128, d.totalticks)
```

### Comparing `pym2149-8/ymtests/qnoispec.py` & `pym2149-9/ymtests/qtinheri.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pym2149.  If not, see <http://www.gnu.org/licenses/>.
 
-mixer.put(A_noise)
-for p in range(0x20):
-  A_level.put(0x0f)
-  N_period.put(p)
-  sleep(48)
-  A_level.put(0x00)
-  sleep(2)
+mixer.put(A_tone)
+A_level.put(0x0f)
+B_level.put(0x00)
+def spike(): # Doesn't work, never mind.
+  B_level.put(0x0d)
+  B_level.put(0x00)
+A_fine.put(0x00)
+for i in range(20):
+  spike()
+  A_rough.put(0x0e)
+  sleep(2 + i)
+  spike()
+  A_rough.put(0x02)
+  sleep(2 + i)
+A_level.put(0x00)
+B_level.put(0x00)
```

### Comparing `pym2149-8/dsd2wav.py` & `pym2149-9/dsd2wav.py`

 * *Files identical despite different names*

### Comparing `pym2149-8/PKG-INFO` & `pym2149-9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pym2149
-Version: 8
+Version: 9
 Summary: YM2149 emulator supporting YM files, OSC, MIDI to JACK, PortAudio, WAV
 Home-page: https://github.com/combatopera/pym2149
 Author: Andrzej Cichocki
 License: UNKNOWN
 Description: # pym2149
         YM2149 emulator supporting YM files, OSC, MIDI to JACK, PortAudio, WAV.
```

### Comparing `pym2149-8/lc2jack.py` & `pym2149-9/lc2jack.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 import lurlene.osc
 
 log = logging.getLogger(__name__)
 
 @types(Config, Context, this = Started)
 def loadcontext(config, context):
     with open(config.inpath) as f:
-        context._update(f.read())
-    context._flip()
+        context.update(f.read())
+    context.flip()
 
 def main_lc2jack():
     config, di = boot(ConfigName('inpath', '--section'))
     try:
         di.add(loadcontext)
         di.add(LurleneBridge)
         lurlene.osc.configure(di)
```

### Comparing `pym2149-8/pym2149.egg-info/entry_points.txt` & `pym2149-9/pym2149.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pym2149-8/pym2149.egg-info/PKG-INFO` & `pym2149-9/pym2149.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pym2149
-Version: 8
+Version: 9
 Summary: YM2149 emulator supporting YM files, OSC, MIDI to JACK, PortAudio, WAV
 Home-page: https://github.com/combatopera/pym2149
 Author: Andrzej Cichocki
 License: UNKNOWN
 Description: # pym2149
         YM2149 emulator supporting YM files, OSC, MIDI to JACK, PortAudio, WAV.
```

