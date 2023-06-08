# Comparing `tmp/circuitpython-stubs-8.2.0b0.tar.gz` & `tmp/circuitpython-stubs-8.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-stubs-8.2.0b0.tar", last modified: Wed May 24 15:46:21 2023, max compression
+gzip compressed data, was "circuitpython-stubs-8.2.0b1.tar", last modified: Thu Jun  8 18:53:00 2023, max compression
```

## Comparing `circuitpython-stubs-8.2.0b0.tar` & `circuitpython-stubs-8.2.0b1.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.626046 circuitpython-stubs-8.2.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 15:46:21.626046 circuitpython-stubs-8.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.606045 circuitpython-stubs-8.2.0b0/_bleio/
--rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/_bleio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.606045 circuitpython-stubs-8.2.0b0/_eve/
--rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/_eve/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.606045 circuitpython-stubs-8.2.0b0/_pew/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/_pew/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.606045 circuitpython-stubs-8.2.0b0/_pixelmap/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/_pixelmap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.606045 circuitpython-stubs-8.2.0b0/_stage/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/_stage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.606045 circuitpython-stubs-8.2.0b0/adafruit_bus_device/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/adafruit_bus_device/i2c_device/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/adafruit_bus_device/i2c_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/adafruit_bus_device/spi_device/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/adafruit_bus_device/spi_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/adafruit_pixelbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/aesio/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/aesio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/alarm/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/alarm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/alarm/pin/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/alarm/pin/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/alarm/time/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/alarm/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/alarm/touch/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/alarm/touch/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/analogbufio/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/analogbufio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/analogio/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/analogio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/atexit/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/atexit/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/audiobusio/
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/audiobusio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/audiocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/audiocore/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/audioio/
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/audioio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/audiomixer/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/audiomixer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/audiomp3/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/audiomp3/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/audiopwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/audiopwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/bitbangio/
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/bitbangio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/bitmaptools/
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/bitmaptools/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/bitops/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/bitops/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/board/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/busio/
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/busio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/camera/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/camera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/canio/
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/canio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 15:46:20.000000 circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-24 15:46:21.000000 circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:46:20.000000 circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:46:20.000000 circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-24 15:46:20.000000 circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/countio/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/countio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/cyw43/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/cyw43/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/digitalio/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-24 15:46:09.000000 circuitpython-stubs-8.2.0b0/digitalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/displayio/
--rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/displayio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.610045 circuitpython-stubs-8.2.0b0/dualbank/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/dualbank/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/espcamera/
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/espcamera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/espidf/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/espidf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/espnow/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/espnow/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/espulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/espulp/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/floppyio/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/floppyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/fontio/
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/fontio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/framebufferio/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/framebufferio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/frequencyio/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/frequencyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/getpass/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/getpass/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/gifio/
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/gifio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/gnss/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/gnss/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/hashlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/hashlib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/i2ctarget/
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/i2ctarget/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/imagecapture/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/imagecapture/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/ipaddress/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/ipaddress/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/is31fl3741/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/is31fl3741/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/keypad/
--rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/keypad/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/math/
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/math/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/mdns/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/mdns/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/memorymap/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/memorymap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/memorymonitor/
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/memorymonitor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/microcontroller/
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/microcontroller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/msgpack/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/msgpack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/neopixel_write/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/neopixel_write/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/nvm/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/nvm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/onewireio/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/onewireio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/os/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/os/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/paralleldisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/picodvi/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/picodvi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/ps2io/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/ps2io/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.614045 circuitpython-stubs-8.2.0b0/pulseio/
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/pulseio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/pwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/pwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/qrio/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/qrio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/rainbowio/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/rainbowio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/random/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/random/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/rgbmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/rotaryio/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/rotaryio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/rp2pio/
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/rp2pio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/rtc/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/rtc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/samd/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/samd/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/sdcardio/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/sdcardio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/sdioio/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/sdioio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:46:21.626046 circuitpython-stubs-8.2.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-24 15:46:12.000000 circuitpython-stubs-8.2.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/sharpdisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/socketpool/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/socketpool/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/ssl/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/storage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/struct/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/struct/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/supervisor/
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/supervisor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/synthio/
--rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/synthio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/terminalio/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/terminalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/time/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/touchio/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/touchio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/traceback/
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/traceback/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/uheap/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-24 15:46:10.000000 circuitpython-stubs-8.2.0b0/uheap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/ulab/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/ulab/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/numpy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/ulab/numpy/carray/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/numpy/carray/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/ulab/numpy/fft/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/numpy/fft/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.618045 circuitpython-stubs-8.2.0b0/ulab/numpy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/numpy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/ulab/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/scipy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/ulab/scipy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/scipy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/ulab/scipy/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/scipy/optimize/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/ulab/user/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/user/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/ulab/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ulab/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/usb/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/usb/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/usb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/usb/core/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/usb_cdc/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/usb_cdc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/usb_hid/
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/usb_hid/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/usb_host/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/usb_host/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/usb_midi/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/usb_midi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/ustack/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/ustack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/vectorio/
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/vectorio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/watchdog/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/wifi/
--rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/wifi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:21.622046 circuitpython-stubs-8.2.0b0/zlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-24 15:46:11.000000 circuitpython-stubs-8.2.0b0/zlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.273276 circuitpython-stubs-8.2.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 18:52:52.000000 circuitpython-stubs-8.2.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-08 18:53:00.273276 circuitpython-stubs-8.2.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-08 18:52:52.000000 circuitpython-stubs-8.2.0b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.257275 circuitpython-stubs-8.2.0b1/_bleio/
+-rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/_bleio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.257275 circuitpython-stubs-8.2.0b1/_eve/
+-rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/_eve/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.257275 circuitpython-stubs-8.2.0b1/_pew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/_pew/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.257275 circuitpython-stubs-8.2.0b1/_pixelmap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/_pixelmap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.257275 circuitpython-stubs-8.2.0b1/_stage/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/_stage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/adafruit_bus_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/adafruit_bus_device/i2c_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/adafruit_bus_device/i2c_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/adafruit_bus_device/spi_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/adafruit_bus_device/spi_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/adafruit_pixelbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/aesio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/aesio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/alarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/alarm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/alarm/pin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/alarm/pin/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/alarm/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/alarm/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/alarm/touch/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/alarm/touch/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/analogbufio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/analogbufio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/analogio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/analogio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/atexit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/atexit/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/audiobusio/
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/audiobusio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/audiocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/audiocore/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/audioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/audioio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/audiomixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/audiomixer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/audiomp3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/audiomp3/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/audiopwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/audiopwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/bitbangio/
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/bitbangio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/bitmaptools/
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/bitmaptools/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/bitops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/bitops/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/board/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/busio/
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/busio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/camera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/canio/
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/canio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.273276 circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-08 18:52:59.000000 circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-08 18:53:00.000000 circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:52:59.000000 circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:52:59.000000 circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-08 18:52:59.000000 circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/countio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/countio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/cyw43/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-08 18:52:52.000000 circuitpython-stubs-8.2.0b1/cyw43/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/digitalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/digitalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/displayio/
+-rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/displayio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/dualbank/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/dualbank/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/espcamera/
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/espcamera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/espidf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/espidf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/espnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/espnow/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/espulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/espulp/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/floppyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/floppyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/fontio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/fontio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/framebufferio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/framebufferio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/frequencyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/frequencyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/getpass/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/getpass/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/gifio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/gifio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/gnss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/gnss/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/hashlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/hashlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/i2ctarget/
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/i2ctarget/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/imagecapture/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/imagecapture/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/ipaddress/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/ipaddress/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/is31fl3741/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/is31fl3741/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/keypad/
+-rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/keypad/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/math/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/mdns/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/mdns/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/memorymap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/memorymap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/memorymonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/memorymonitor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/microcontroller/
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/microcontroller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/msgpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/msgpack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/neopixel_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/neopixel_write/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/nvm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/nvm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/onewireio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/onewireio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/os/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/os/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/paralleldisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/picodvi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-08 18:52:52.000000 circuitpython-stubs-8.2.0b1/picodvi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/ps2io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/ps2io/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/pulseio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/pulseio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/pwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/pwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/qrio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/qrio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/rainbowio/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/rainbowio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/random/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/random/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/rgbmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/rotaryio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/rotaryio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/rp2pio/
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-06-08 18:52:52.000000 circuitpython-stubs-8.2.0b1/rp2pio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/rtc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/rtc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/samd/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/samd/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/sdcardio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/sdcardio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/sdioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/sdioio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:53:00.273276 circuitpython-stubs-8.2.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-08 18:52:52.000000 circuitpython-stubs-8.2.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/sharpdisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/socketpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/socketpool/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/ssl/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/storage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/struct/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/supervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/supervisor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/synthio/
+-rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/synthio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/terminalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/terminalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/touchio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/touchio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/traceback/
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/traceback/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/uheap/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/uheap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/numpy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/numpy/carray/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/numpy/carray/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/numpy/fft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/numpy/fft/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/numpy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/numpy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/scipy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/scipy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/scipy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/scipy/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/scipy/optimize/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/user/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/usb/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/usb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/usb/core/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/usb_cdc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/usb_cdc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/usb_hid/
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/usb_hid/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/usb_host/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/usb_host/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/usb_midi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/usb_midi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ustack/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/ustack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/vectorio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/vectorio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/watchdog/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/wifi/
+-rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/wifi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/zlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/zlib/__init__.pyi
```

### Comparing `circuitpython-stubs-8.2.0b0/README.rst` & `circuitpython-stubs-8.2.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/_bleio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/_eve/__init__.pyi` & `circuitpython-stubs-8.2.0b1/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/_pew/__init__.pyi` & `circuitpython-stubs-8.2.0b1/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/_pixelmap/__init__.pyi` & `circuitpython-stubs-8.2.0b1/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/_stage/__init__.pyi` & `circuitpython-stubs-8.2.0b1/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/adafruit_bus_device/i2c_device/__init__.pyi` & `circuitpython-stubs-8.2.0b1/adafruit_bus_device/i2c_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/adafruit_bus_device/spi_device/__init__.pyi` & `circuitpython-stubs-8.2.0b1/adafruit_bus_device/spi_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/adafruit_pixelbuf/__init__.pyi` & `circuitpython-stubs-8.2.0b1/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/aesio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/aesio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/alarm/__init__.pyi` & `circuitpython-stubs-8.2.0b1/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/alarm/pin/__init__.pyi` & `circuitpython-stubs-8.2.0b1/alarm/pin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/alarm/time/__init__.pyi` & `circuitpython-stubs-8.2.0b1/alarm/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/alarm/touch/__init__.pyi` & `circuitpython-stubs-8.2.0b1/alarm/touch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/analogbufio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/analogio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/atexit/__init__.pyi` & `circuitpython-stubs-8.2.0b1/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/audiobusio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/audiocore/__init__.pyi` & `circuitpython-stubs-8.2.0b1/audiocore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/audioio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/audiomixer/__init__.pyi` & `circuitpython-stubs-8.2.0b1/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/audiomp3/__init__.pyi` & `circuitpython-stubs-8.2.0b1/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/audiopwmio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/bitbangio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/bitbangio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/bitmaptools/__init__.pyi` & `circuitpython-stubs-8.2.0b1/bitmaptools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/bitops/__init__.pyi` & `circuitpython-stubs-8.2.0b1/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/board/__init__.pyi` & `circuitpython-stubs-8.2.0b1/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/busio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/busio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/camera/__init__.pyi` & `circuitpython-stubs-8.2.0b1/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/canio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/SOURCES.txt` & `circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/circuitpython_stubs.egg-info/top_level.txt` & `circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/countio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/countio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/cyw43/__init__.pyi` & `circuitpython-stubs-8.2.0b1/cyw43/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/digitalio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/displayio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/displayio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/dualbank/__init__.pyi` & `circuitpython-stubs-8.2.0b1/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/espcamera/__init__.pyi` & `circuitpython-stubs-8.2.0b1/espcamera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/espidf/__init__.pyi` & `circuitpython-stubs-8.2.0b1/espidf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/espnow/__init__.pyi` & `circuitpython-stubs-8.2.0b1/espnow/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/espulp/__init__.pyi` & `circuitpython-stubs-8.2.0b1/espulp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/floppyio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/fontio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/framebufferio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/framebufferio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/frequencyio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/getpass/__init__.pyi` & `circuitpython-stubs-8.2.0b1/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/gifio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/gifio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/gnss/__init__.pyi` & `circuitpython-stubs-8.2.0b1/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/hashlib/__init__.pyi` & `circuitpython-stubs-8.2.0b1/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/i2ctarget/__init__.pyi` & `circuitpython-stubs-8.2.0b1/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/imagecapture/__init__.pyi` & `circuitpython-stubs-8.2.0b1/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/ipaddress/__init__.pyi` & `circuitpython-stubs-8.2.0b1/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/is31fl3741/__init__.pyi` & `circuitpython-stubs-8.2.0b1/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/keypad/__init__.pyi` & `circuitpython-stubs-8.2.0b1/keypad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/math/__init__.pyi` & `circuitpython-stubs-8.2.0b1/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/mdns/__init__.pyi` & `circuitpython-stubs-8.2.0b1/mdns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/memorymap/__init__.pyi` & `circuitpython-stubs-8.2.0b1/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/memorymonitor/__init__.pyi` & `circuitpython-stubs-8.2.0b1/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/microcontroller/__init__.pyi` & `circuitpython-stubs-8.2.0b1/microcontroller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/msgpack/__init__.pyi` & `circuitpython-stubs-8.2.0b1/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/neopixel_write/__init__.pyi` & `circuitpython-stubs-8.2.0b1/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/nvm/__init__.pyi` & `circuitpython-stubs-8.2.0b1/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/onewireio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/onewireio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/os/__init__.pyi` & `circuitpython-stubs-8.2.0b1/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/paralleldisplay/__init__.pyi` & `circuitpython-stubs-8.2.0b1/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/picodvi/__init__.pyi` & `circuitpython-stubs-8.2.0b1/picodvi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/ps2io/__init__.pyi` & `circuitpython-stubs-8.2.0b1/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/pulseio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/pwmio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/qrio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/random/__init__.pyi` & `circuitpython-stubs-8.2.0b1/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/rgbmatrix/__init__.pyi` & `circuitpython-stubs-8.2.0b1/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/rotaryio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/rp2pio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/rp2pio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/rtc/__init__.pyi` & `circuitpython-stubs-8.2.0b1/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/samd/__init__.pyi` & `circuitpython-stubs-8.2.0b1/samd/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/sdcardio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/sdioio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/setup.py` & `circuitpython-stubs-8.2.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/sharpdisplay/__init__.pyi` & `circuitpython-stubs-8.2.0b1/sharpdisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/socketpool/__init__.pyi` & `circuitpython-stubs-8.2.0b1/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/ssl/__init__.pyi` & `circuitpython-stubs-8.2.0b1/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/storage/__init__.pyi` & `circuitpython-stubs-8.2.0b1/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/struct/__init__.pyi` & `circuitpython-stubs-8.2.0b1/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/supervisor/__init__.pyi` & `circuitpython-stubs-8.2.0b1/supervisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/synthio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/synthio/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,27 @@
     """Converts the given midi note (60 = middle C, 69 = concert A) to Hz"""
 
 def voct_to_hz(ctrl: float) -> float:
     """Converts a 1v/octave signal to Hz.
 
     24/12 (2.0) corresponds to middle C, 33/12 (2.75) is concert A."""
 
+class Biquad:
+    def __init__(self, b0: float, b1: float, b2: float, a1: float, a2: float) -> None:
+        """Construct a normalized biquad filter object.
+
+        This implements the "direct form 1" biquad filter, where each coefficient
+        has been pre-divided by a0.
+
+        Biquad objects are usually constructed via one of the related methods on a `Synthesizer` object
+        rather than directly from coefficients.
+
+        https://github.com/WebAudio/Audio-EQ-Cookbook/blob/main/Audio-EQ-Cookbook.txt
+        """
+
 class LFO:
     """A low-frequency oscillator block
 
     Every `rate` seconds, the output of the LFO cycles through its `waveform`.
     The output at any particular moment is ``waveform[idx] * scale + offset``.
 
     If `waveform` is None, a triangle waveform is used.
@@ -305,28 +318,33 @@
         *,
         frequency: float,
         panning: BlockInput = 0.0,
         waveform: Optional[ReadableBuffer] = None,
         envelope: Optional[Envelope] = None,
         amplitude: BlockInput = 0.0,
         bend: BlockInput = 0.0,
+        filter: Optional[Biquad] = None,
         ring_frequency: float = 0.0,
         ring_bend: float = 0.0,
         ring_waveform: Optional[ReadableBuffer] = 0.0,
     ) -> None:
         """Construct a Note object, with a frequency in Hz, and optional panning, waveform, envelope, tremolo (volume change) and bend (frequency change).
 
         If waveform or envelope are `None` the synthesizer object's default waveform or envelope are used.
 
         If the same Note object is played on multiple Synthesizer objects, the result is undefined.
         """
     frequency: float
     """The base frequency of the note, in Hz."""
-    filter: bool
-    """True if the note should be processed via the synthesizer's FIR filter."""
+    filter: Optional[Biquad]
+    """If not None, the output of this Note is filtered according to the provided coefficients.
+
+    Construct an appropriate filter by calling a filter-making method on the
+    `Synthesizer` object where you plan to play the note, as filter coefficients depend
+    on the sample rate"""
     panning: BlockInput
     """Defines the channel(s) in which the note appears.
 
     -1 is left channel only, 0 is both channels, and 1 is right channel.
     For fractional values, the note plays at full amplitude in one channel
     and partial amplitude in the other channel. For instance -.5 plays at full
     amplitude in the left channel and 1/2 amplitude in the right channel."""
@@ -381,28 +399,26 @@
     def __init__(
         self,
         *,
         sample_rate: int = 11025,
         channel_count: int = 1,
         waveform: Optional[ReadableBuffer] = None,
         envelope: Optional[Envelope] = None,
-        filter: Optional[ReadableBuffer] = None,
     ) -> None:
         """Create a synthesizer object.
 
         This API is experimental.
 
         Integer notes use MIDI note numbering, with 60 being C4 or Middle C,
         approximately 262Hz. Integer notes use the given waveform & envelope,
         and do not support advanced features like tremolo or vibrato.
 
         :param int sample_rate: The desired playback sample rate; higher sample rate requires more memory
         :param int channel_count: The number of output channels (1=mono, 2=stereo)
         :param ReadableBuffer waveform: A single-cycle waveform. Default is a 50% duty cycle square wave. If specified, must be a ReadableBuffer of type 'h' (signed 16 bit)
-        :param ReadableBuffer filter: Coefficients of an FIR filter to apply to notes with ``filter=True``. If specified, must be a ReadableBuffer of type 'h' (signed 16 bit)
         :param Optional[Envelope] envelope: An object that defines the loudness of a note over time. The default envelope, `None` provides no ramping, voices turn instantly on and off.
         """
     def press(self, /, press: NoteOrNoteSequence = ()) -> None:
         """Turn some notes on.
 
         Pressing a note that was already pressed has no effect.
 
@@ -469,7 +485,40 @@
 
     This can be used to implement 'free-running' LFOs. LFOs associated with playing notes are advanced whether or not they are in this list.
 
     This property is read-only but its contents may be modified by e.g., calling ``synth.blocks.append()`` or ``synth.blocks.remove()``. It is initially an empty list."""
 
     max_polyphony: int
     """Maximum polyphony of the synthesizer (read-only class property)"""
+
+    def low_pass_filter(
+        cls, frequency: float, q_factor: float = 0.7071067811865475
+    ) -> Biquad:
+        """Construct a low-pass filter with the given parameters.
+
+        ``frequency``, called f0 in the cookbook, is the corner frequency in Hz
+        of the filter.
+
+        ``q_factor``, called ``Q`` in the cookbook.  Controls how peaked the response will be at the cutoff frequency. A large value makes the response more peaked.
+        """
+    def high_pass_filter(
+        cls, frequency: float, q_factor: float = 0.7071067811865475
+    ) -> Biquad:
+        """Construct a high-pass filter with the given parameters.
+
+        ``frequency``, called f0 in the cookbook, is the corner frequency in Hz
+        of the filter.
+
+        ``q_factor``, called ``Q`` in the cookbook.  Controls how peaked the response will be at the cutoff frequency. A large value makes the response more peaked.
+        """
+    def band_pass_filter(
+        cls, frequency: float, q_factor: float = 0.7071067811865475
+    ) -> Biquad:
+        """Construct a band-pass filter with the given parameters.
+
+        ``frequency``, called f0 in the cookbook, is the center frequency in Hz
+        of the filter.
+
+        ``q_factor``, called ``Q`` in the cookbook.  Controls how peaked the response will be at the cutoff frequency. A large value makes the response more peaked.
+
+        The coefficients are scaled such that the filter has a 0dB peak gain.
+        """
```

### Comparing `circuitpython-stubs-8.2.0b0/terminalio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/time/__init__.pyi` & `circuitpython-stubs-8.2.0b1/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/touchio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/traceback/__init__.pyi` & `circuitpython-stubs-8.2.0b1/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/ulab/__init__.pyi` & `circuitpython-stubs-8.2.0b1/ulab/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/ulab/numpy/__init__.pyi` & `circuitpython-stubs-8.2.0b1/ulab/numpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/ulab/numpy/carray/__init__.pyi` & `circuitpython-stubs-8.2.0b1/ulab/numpy/carray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/ulab/numpy/fft/__init__.pyi` & `circuitpython-stubs-8.2.0b1/ulab/numpy/fft/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/ulab/numpy/linalg/__init__.pyi` & `circuitpython-stubs-8.2.0b1/ulab/numpy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/ulab/scipy/linalg/__init__.pyi` & `circuitpython-stubs-8.2.0b1/ulab/scipy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/ulab/scipy/optimize/__init__.pyi` & `circuitpython-stubs-8.2.0b1/ulab/scipy/optimize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/usb/core/__init__.pyi` & `circuitpython-stubs-8.2.0b1/usb/core/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/usb_cdc/__init__.pyi` & `circuitpython-stubs-8.2.0b1/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/usb_hid/__init__.pyi` & `circuitpython-stubs-8.2.0b1/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/usb_host/__init__.pyi` & `circuitpython-stubs-8.2.0b1/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/usb_midi/__init__.pyi` & `circuitpython-stubs-8.2.0b1/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/vectorio/__init__.pyi` & `circuitpython-stubs-8.2.0b1/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/watchdog/__init__.pyi` & `circuitpython-stubs-8.2.0b1/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/wifi/__init__.pyi` & `circuitpython-stubs-8.2.0b1/wifi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b0/zlib/__init__.pyi` & `circuitpython-stubs-8.2.0b1/zlib/__init__.pyi`

 * *Files identical despite different names*

