# Comparing `tmp/micrOSDevToolKit-1.21.5.tar.gz` & `tmp/micrOSDevToolKit-1.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.21.5.tar", last modified: Sun Aug  6 19:17:14 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.22.0.tar", last modified: Mon Aug  7 13:37:12 2023, max compression
```

## Comparing `micrOSDevToolKit-1.21.5.tar` & `micrOSDevToolKit-1.22.0.tar`

### file list

```diff
@@ -1,277 +1,277 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.535475 micrOSDevToolKit-1.21.5/
--rw-r--r--   0 bnm        (501) staff       (20)      358 2023-08-03 17:06:55.000000 micrOSDevToolKit-1.21.5/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    55058 2023-08-06 19:17:14.534935 micrOSDevToolKit-1.21.5/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    45495 2023-08-05 00:33:02.000000 micrOSDevToolKit-1.21.5/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.21.5/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.113460 micrOSDevToolKit-1.21.5/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.107223 micrOSDevToolKit-1.21.5/env/driver_cp210x/
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.155197 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/
--rw-r--r--   0 bnm        (501) staff       (20)  1049848 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x64.exe
--rw-r--r--   0 bnm        (501) staff       (20)   924408 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x86.exe
--rw-r--r--   0 bnm        (501) staff       (20)    25165 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210x_Universal_Windows_Driver_ReleaseNotes.txt
--rw-r--r--   0 bnm        (501) staff       (20)     8370 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/SLAB_License_Agreement_VCP_Windows.txt
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.157739 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/
--rw-r--r--   0 bnm        (501) staff       (20)    95408 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/silabser.sys
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.160306 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/
--rw-r--r--   0 bnm        (501) staff       (20)   111792 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/silabser.sys
--rw-r--r--   0 bnm        (501) staff       (20)    11569 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/dpinst.xml
--rw-r--r--   0 bnm        (501) staff       (20)    12624 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.cat
--rw-r--r--   0 bnm        (501) staff       (20)    10453 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.inf
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.162763 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/
--rw-r--r--   0 bnm        (501) staff       (20)   110768 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/silabser.sys
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.173232 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/
--rw-r--r--   0 bnm        (501) staff       (20)    98480 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/silabser.sys
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.192409 micrOSDevToolKit-1.21.5/env/driver_cp210x/macOS_VCP_Driver/
--rwxr-xr-x   0 bnm        (501) staff       (20)  2004490 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/macOS_VCP_Driver/SiLabsUSBDriverDisk.dmg
--rwxr-xr-x   0 bnm        (501) staff       (20)    10569 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/macOS_VCP_Driver/macOS_VCP_Driver_Release_Notes.txt
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.207922 micrOSDevToolKit-1.21.5/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.5/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.5/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.214175 micrOSDevToolKit-1.21.5/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.21.5/micrOS/SchedulerUT.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.246400 micrOSDevToolKit-1.21.5/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.21.5/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.21.5/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.311374 micrOSDevToolKit-1.21.5/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.21.5/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6218 2023-08-02 12:29:26.000000 micrOSDevToolKit-1.21.5/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.21.5/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6443 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.5/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.21.5/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.21.5/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-08-06 19:04:54.000000 micrOSDevToolKit-1.21.5/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.21.5/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     3786 2023-08-01 19:30:57.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_aht10.py
--rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     3559 2023-08-02 17:26:12.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_lmpacman.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    19504 2023-08-04 14:14:52.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11897 2023-08-04 10:52:35.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     1629 2023-08-04 11:24:20.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_rgbcct.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.21.5/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.21.5/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.21.5/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.21.5/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.21.5/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.21.5/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-29 10:25:26.000000 micrOSDevToolKit-1.21.5/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19349 2023-08-06 19:01:22.000000 micrOSDevToolKit-1.21.5/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.21.5/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/micrOS/source/TinyPLed.py
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.21.5/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.21.5/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.21.5/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.21.5/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.314783 micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    55058 2023-08-06 19:17:13.000000 micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     9934 2023-08-06 19:17:14.000000 micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-08-06 19:17:13.000000 micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-08-06 19:17:13.000000 micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-08-06 19:17:13.000000 micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-08-06 19:17:14.535640 micrOSDevToolKit-1.21.5/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-08-06 19:12:41.000000 micrOSDevToolKit-1.21.5/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.340715 micrOSDevToolKit-1.21.5/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.21.5/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.21.5/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.21.5/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.21.5/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.429294 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.434325 micrOSDevToolKit-1.21.5/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.21.5/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.21.5/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.21.5/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.21.5/toolkit/micrOSdashboard.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.454203 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/
--rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/LP_darwin.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.488318 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     7455 2023-08-02 12:44:06.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5415 2023-08-01 19:28:24.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/dotstar.py
--rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/ds18x20.py
--rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/framebuf.py
--rw-r--r--   0 bnm        (501) staff       (20)     4828 2023-08-02 12:43:56.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/machine.py
--rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/micropython.py
--rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/network.py
--rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/ntptime.py
--rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/onewire.py
--rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/sim_console.py
--rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/simgc.py
--rw-r--r--   0 bnm        (501) staff       (20)     6584 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/simulator.py
--rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/uasyncio.py
--rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/utime.py
--rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/webrepl.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.21.5/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.489151 micrOSDevToolKit-1.21.5/toolkit/user_data/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.21.5/toolkit/user_data/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.489530 micrOSDevToolKit-1.21.5/toolkit/user_data/node_config_archive/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/user_data/node_config_archive/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.489887 micrOSDevToolKit-1.21.5/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.533491 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/
--rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Common.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/ConfigHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1990 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Debug.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      759 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Hooks.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/InterConnect.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/InterpreterShell.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/InterruptHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      869 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     1297 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_aht10.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_bme280.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_buzzer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_cct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_co2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_dht11.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_dht22.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_dimmer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)      522 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_ds18.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_genIO.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)      616 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_intercon.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1193 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_light_sensor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_lmpacman.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_neoeffects.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_neopixel.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_oled.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     6207 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_oled_ui.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_presence.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)     3501 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_rgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      557 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_rgbcct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_roboarm.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_servo.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_stepper.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_switch.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_system.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      872 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_telegram.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_tinyrgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      550 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_esp32.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      563 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_esp32s2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      553 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_esp32s3.mpy
--rw-r--r--   0 bnm        (501) staff       (20)       54 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_rp2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      491 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_tinypico.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LogicalPins.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Network.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Notify.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Scheduler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/SocketServer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     5714 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/TaskManager.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Time.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      434 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/TinyPLed.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/micrOS.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/micrOSloader.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      198 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/reset.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/urequests.mpy
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:12.036529 micrOSDevToolKit-1.22.0/
+-rw-r--r--   0 bnm        (501) staff       (20)      358 2023-08-03 17:06:55.000000 micrOSDevToolKit-1.22.0/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    55058 2023-08-07 13:37:12.035950 micrOSDevToolKit-1.22.0/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    45495 2023-08-05 00:33:02.000000 micrOSDevToolKit-1.22.0/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.22.0/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.565608 micrOSDevToolKit-1.22.0/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.558807 micrOSDevToolKit-1.22.0/env/driver_cp210x/
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.596037 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/
+-rw-r--r--   0 bnm        (501) staff       (20)  1049848 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x64.exe
+-rw-r--r--   0 bnm        (501) staff       (20)   924408 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x86.exe
+-rw-r--r--   0 bnm        (501) staff       (20)    25165 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210x_Universal_Windows_Driver_ReleaseNotes.txt
+-rw-r--r--   0 bnm        (501) staff       (20)     8370 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/SLAB_License_Agreement_VCP_Windows.txt
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.597411 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/
+-rw-r--r--   0 bnm        (501) staff       (20)    95408 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/silabser.sys
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.599802 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/
+-rw-r--r--   0 bnm        (501) staff       (20)   111792 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/silabser.sys
+-rw-r--r--   0 bnm        (501) staff       (20)    11569 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/dpinst.xml
+-rw-r--r--   0 bnm        (501) staff       (20)    12624 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.cat
+-rw-r--r--   0 bnm        (501) staff       (20)    10453 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.inf
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.604957 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/
+-rw-r--r--   0 bnm        (501) staff       (20)   110768 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/silabser.sys
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.609332 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/
+-rw-r--r--   0 bnm        (501) staff       (20)    98480 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/silabser.sys
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.622319 micrOSDevToolKit-1.22.0/env/driver_cp210x/macOS_VCP_Driver/
+-rwxr-xr-x   0 bnm        (501) staff       (20)  2004490 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/macOS_VCP_Driver/SiLabsUSBDriverDisk.dmg
+-rwxr-xr-x   0 bnm        (501) staff       (20)    10569 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/env/driver_cp210x/macOS_VCP_Driver/macOS_VCP_Driver_Release_Notes.txt
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.636750 micrOSDevToolKit-1.22.0/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.22.0/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.22.0/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.640320 micrOSDevToolKit-1.22.0/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.22.0/micrOS/SchedulerUT.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.674437 micrOSDevToolKit-1.22.0/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.22.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.22.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.748224 micrOSDevToolKit-1.22.0/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.22.0/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6218 2023-08-02 12:29:26.000000 micrOSDevToolKit-1.22.0/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.22.0/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6443 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.22.0/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.22.0/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.22.0/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11532 2023-08-07 13:21:48.000000 micrOSDevToolKit-1.22.0/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.22.0/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3786 2023-08-01 19:30:57.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_aht10.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3559 2023-08-02 17:26:12.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_lmpacman.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19504 2023-08-04 14:14:52.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11897 2023-08-04 10:52:35.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1629 2023-08-04 11:24:20.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_rgbcct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.22.0/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.22.0/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.22.0/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.22.0/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.22.0/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.22.0/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.22.0/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11571 2023-08-07 13:21:48.000000 micrOSDevToolKit-1.22.0/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19349 2023-08-06 19:01:22.000000 micrOSDevToolKit-1.22.0/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.22.0/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/micrOS/source/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.22.0/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.22.0/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.22.0/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.22.0/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.22.0/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.753754 micrOSDevToolKit-1.22.0/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    55058 2023-08-07 13:37:11.000000 micrOSDevToolKit-1.22.0/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     9934 2023-08-07 13:37:11.000000 micrOSDevToolKit-1.22.0/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-08-07 13:37:11.000000 micrOSDevToolKit-1.22.0/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-08-07 13:37:11.000000 micrOSDevToolKit-1.22.0/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-08-07 13:37:11.000000 micrOSDevToolKit-1.22.0/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-08-07 13:37:12.036783 micrOSDevToolKit-1.22.0/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-08-07 13:34:42.000000 micrOSDevToolKit-1.22.0/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.765379 micrOSDevToolKit-1.22.0/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.22.0/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.22.0/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.22.0/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.22.0/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.798107 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.814068 micrOSDevToolKit-1.22.0/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.22.0/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.22.0/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.22.0/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.22.0/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.893850 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.947591 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7455 2023-08-02 12:44:06.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5415 2023-08-01 19:28:24.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4828 2023-08-02 12:43:56.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6584 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.22.0/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.948466 micrOSDevToolKit-1.22.0/toolkit/user_data/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.22.0/toolkit/user_data/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.949061 micrOSDevToolKit-1.22.0/toolkit/user_data/node_config_archive/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/user_data/node_config_archive/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:11.949427 micrOSDevToolKit-1.22.0/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-07 13:37:12.034351 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/
+-rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Common.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/ConfigHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1990 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Debug.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      759 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Hooks.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/InterConnect.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4147 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/InterpreterShell.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/InterruptHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      869 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1297 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_aht10.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_bme280.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_buzzer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_cct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_co2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_dht11.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_dht22.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_dimmer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)      522 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_ds18.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_genIO.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)      616 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_intercon.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1193 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_light_sensor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_lmpacman.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_neoeffects.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_neopixel.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_oled.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     6207 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_oled_ui.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_presence.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3501 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_rgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      557 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_rgbcct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_roboarm.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_servo.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_stepper.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_switch.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_system.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      872 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_telegram.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      550 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LP_esp32.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      563 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LP_esp32s2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      553 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LP_esp32s3.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)       54 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LP_rp2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      491 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LP_tinypico.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LogicalPins.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Network.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Notify.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Scheduler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3760 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/SocketServer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     5714 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/TaskManager.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Time.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      434 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/TinyPLed.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/micrOS.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/micrOSloader.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      198 2023-08-07 13:31:07.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/reset.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-08-07 13:31:08.000000 micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/urequests.mpy
```

### Comparing `micrOSDevToolKit-1.21.5/PKG-INFO` & `micrOSDevToolKit-1.22.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.21.5
+Version: 1.22.0
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.21.5/README.md` & `micrOSDevToolKit-1.22.0/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/devToolKit.py` & `micrOSDevToolKit-1.22.0/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x64.exe` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x64.exe`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x86.exe` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x86.exe`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210x_Universal_Windows_Driver_ReleaseNotes.txt` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210x_Universal_Windows_Driver_ReleaseNotes.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/SLAB_License_Agreement_VCP_Windows.txt` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/SLAB_License_Agreement_VCP_Windows.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/silabser.sys` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/silabser.sys`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/silabser.sys` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/silabser.sys`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/dpinst.xml` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/dpinst.xml`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.cat` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.cat`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.inf` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.inf`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/silabser.sys` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/silabser.sys`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/silabser.sys` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/silabser.sys`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/macOS_VCP_Driver/SiLabsUSBDriverDisk.dmg` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/macOS_VCP_Driver/SiLabsUSBDriverDisk.dmg`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/env/driver_cp210x/macOS_VCP_Driver/macOS_VCP_Driver_Release_Notes.txt` & `micrOSDevToolKit-1.22.0/env/driver_cp210x/macOS_VCP_Driver/macOS_VCP_Driver_Release_Notes.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/media/dnd.png` & `micrOSDevToolKit-1.22.0/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/media/logo.png` & `micrOSDevToolKit-1.22.0/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/media/logo_mini.png` & `micrOSDevToolKit-1.22.0/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/SchedulerUT.py` & `micrOSDevToolKit-1.22.0/micrOS/SchedulerUT.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.22.0/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.22.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.22.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.22.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.22.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.22.0/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/Common.py` & `micrOSDevToolKit-1.22.0/micrOS/source/Common.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.22.0/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/Debug.py` & `micrOSDevToolKit-1.22.0/micrOS/source/Debug.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.22.0/micrOS/source/Hooks.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.22.0/micrOS/source/InterConnect.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.22.0/micrOS/source/InterpreterShell.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,52 +20,48 @@
 
 
 #################################################################
 #                  SHELL Interpreter FUNCTIONS                  #
 #################################################################
 
 class Shell:
-    MICROS_VERSION = '1.21.1-0'
+    MICROS_VERSION = '1.22.0-0'
 
-    def __init__(self, msg_obj=None):
+    def __init__(self):
         """
         comm_obj - communication object - send messages back
                  - comm_obj.reply('msg')
         """
-        self.msg_obj = msg_obj
         # Used node_config parameters
         self.__devfid = cfgget('devfid')
         self.__auth_mode = cfgget('auth')
         self.__hwuid = cfgget("hwuid")
         # State machine
         self.__auth_ok = False          # session authentication state (auth mode)
         self.__conf_mode = False        # session conf mode: on / off
         # Set proper micrOS version
         try:
             cfgput('version', Shell.MICROS_VERSION)
         except Exception as e:
             console_write(f"Export system version to config failed: {e}")
             errlog_add(f"[Shell][ERR] system version export error: {e}")
 
-    def msg(self, msg):
-        """Message stream method"""
-        try:
-            self.msg_obj(msg)
-        except:
-            print(msg)
+    def send(self, msg):
+        # Placeholder method, it will be overwritten by SocektServer.send
+        print(msg)
 
     def reset(self):
         """Reset shell state"""
         self.__auth_ok = False
         self.__conf_mode = False
 
     def reboot(self, hard=False):
         """Reboot micropython VM"""
-        self.msg(f"{'[HARD] ' if hard else ''}Reboot micrOS system.")
-        self.msg("Bye!")
+        self.send(f"{'[HARD] ' if hard else ''}Reboot micrOS system.")
+        self.send("Bye!")
         if hard:
             hard_reset()
         soft_reset()
 
     def prompt(self):
         """Generate prompt"""
         auth = "[password] " if self.__auth_mode and not self.__auth_ok else ""
@@ -76,27 +72,27 @@
         """Authorize user"""
         # Set user auth state
         if self.__auth_mode and not self.__auth_ok:
             # check password
             usrpwd = cfgget('appwd')
             if usrpwd == msg_list[0].strip():
                 self.__auth_ok = True
-                self.msg("AuthOk")
+                self.send("AuthOk")
                 return True, []
-            self.msg("AuthFailed\nBye!")
+            self.send("AuthFailed\nBye!")
             return False, []
         return True, msg_list
 
     def shell(self, msg):
         """
         micrOS Shell main - input string handling
         :param msg: incoming shell command (command or load module call)
         """
         state = self.__shell(msg)
-        self.msg(self.prompt())
+        self.send(self.prompt())
         return state
 
     def __shell(self, msg):
         """
         Socket server - interpreter shell
         :param msg: socket input string
         :return: execution status
@@ -116,90 +112,90 @@
         #   [1] Handle built-in shell commands   #
         # hello, *auth, version, reboot, webrepl #
         ##########################################
 
         # Hello message
         if msg_list[0] == 'hello':
             # For low level device identification - hello msg
-            self.msg(f"hello:{self.__devfid}:{self.__hwuid}")
+            self.send(f"hello:{self.__devfid}:{self.__hwuid}")
             return True
 
         state, msg_list = self.__authentication(msg_list)
         if not state:
             return False
         if len(msg_list) == 0:
             return True
 
         # Version handling
         if msg_list[0] == 'version':
             # For micrOS system version info
-            self.msg(str(Shell.MICROS_VERSION))
+            self.send(str(Shell.MICROS_VERSION))
             return True
 
         # Reboot micropython VM
         if msg_list[0] == 'reboot':
             hard = False
             if len(msg_list) >= 2 and "-h" in msg_list[1]:
                 # reboot / reboot -h
                 hard = True
             self.reboot(hard)
 
         if msg_list[0].startswith('webrepl'):
             if len(msg_list) == 2 and '-u' in msg_list[1]:
-                Shell.webrepl(msg_obj=self.msg, update=True)
-            Shell.webrepl(msg_obj=self.msg)
+                Shell.webrepl(msg_obj=self.send, update=True)
+            Shell.webrepl(msg_obj=self.send)
 
         # CONFIGURE MODE STATE: ACCESS FOR NODE_CONFIG.JSON
         if msg_list[0].startswith('conf'):
             self.__conf_mode = True
             return True
         elif msg_list[0].startswith('noconf'):
             self.__conf_mode = False
             return True
 
         # HELP MSG
         if msg_list[0] == "help":
-            self.msg("[MICROS]   - built-in shell commands")
-            self.msg("   hello   - hello msg - for device identification")
-            self.msg("   version - returns micrOS version")
-            self.msg("   exit    - exit from shell socket prompt")
-            self.msg("   reboot  - system soft reboot (vm), hard reboot (hw): reboot -h")
-            self.msg("   webrepl - start webrepl, for file transfers use with --update")
-            self.msg("[CONF] Configure mode - built-in shell commands")
-            self.msg("  conf       - Enter conf mode")
-            self.msg("    dump       - Dump all data")
-            self.msg("    key        - Get value")
-            self.msg("    key value  - Set value")
-            self.msg("  noconf     - Exit conf mode")
-            self.msg("[TASK] postfix: &x - one-time,  &&x - periodic, x: wait ms [x min: 20ms]")
-            self.msg("  task list         - list tasks with <tag>s")
-            self.msg("  task kill <tag>   - stop task")
-            self.msg("  task show <tag>   - show task output")
-            self.msg("[EXEC] Command mode (LMs):")
-            self.msg("   help lm  - list ALL LoadModules")
+            self.send("[MICROS]   - built-in shell commands")
+            self.send("   hello   - hello msg - for device identification")
+            self.send("   version - returns micrOS version")
+            self.send("   exit    - exit from shell socket prompt")
+            self.send("   reboot  - system soft reboot (vm), hard reboot (hw): reboot -h")
+            self.send("   webrepl - start webrepl, for file transfers use with --update")
+            self.send("[CONF] Configure mode - built-in shell commands")
+            self.send("  conf       - Enter conf mode")
+            self.send("    dump       - Dump all data")
+            self.send("    key        - Get value")
+            self.send("    key value  - Set value")
+            self.send("  noconf     - Exit conf mode")
+            self.send("[TASK] postfix: &x - one-time,  &&x - periodic, x: wait ms [x min: 20ms]")
+            self.send("  task list         - list tasks with <tag>s")
+            self.send("  task kill <tag>   - stop task")
+            self.send("  task show <tag>   - show task output")
+            self.send("[EXEC] Command mode (LMs):")
+            self.send("   help lm  - list ALL LoadModules")
             if "lm" in str(msg_list):
-                return Shell._show_lm_funcs(msg_obj=self.msg)
-            return Shell._show_lm_funcs(msg_obj=self.msg, active_only=True)
+                return Shell._show_lm_funcs(msg_obj=self.send)
+            return Shell._show_lm_funcs(msg_obj=self.send, active_only=True)
 
         # [2] EXECUTE:
         # @1 Configure mode
         if self.__conf_mode and len(msg_list) > 0:
             # Lock thread under config handling is threads available
-            return Shell._configure(self.msg, msg_list)
+            return Shell._configure(self.send, msg_list)
         # @2 Command mode
         """
         INPUT MSG STRUCTURE
         1. param. - LM name, i.e. LM_commands
         2. param. - function call with parameters, i.e. a()
         """
         try:
             # Execute command via InterpreterCore
-            return exec_lm_core(arg_list=msg_list, msgobj=self.msg)
+            return exec_lm_core(arg_list=msg_list, msgobj=self.send)
         except Exception as e:
-            self.msg(f"[ERROR] exec_lm_shell internal error: {e}")
+            self.send(f"[ERROR] exec_lm_shell internal error: {e}")
             return False
 
     #################################################################
     #                     CONFIGURE MODE HANDLER                    #
     #################################################################
     @staticmethod
     def _configure(msg_obj, attributes):
```

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.22.0/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_aht10.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_aht10.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_light_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_lmpacman.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_lmpacman.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_oled_ui.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_rgbcct.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_rgbcct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.22.0/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/Network.py` & `micrOSDevToolKit-1.22.0/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/Notify.py` & `micrOSDevToolKit-1.22.0/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.22.0/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.22.0/micrOS/source/SocketServer.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,29 +33,30 @@
         Debug.INDENT += 1 if Debug.INDENT < 50 else 0       # Auto indent
 
 
 #########################################################
 #          SOCKET SERVER-CLIENT HANDLER CLASS           #
 #########################################################
 
-class Client:
+class Client(Shell):
     ACTIVE_CLIS = {}
 
     def __init__(self, reader, writer):
         self.connected = True
         self.reader = reader
         self.writer = writer
         self.drain_event = asyncio.Event()
         self.drain_event.set()
 
         self.client_id = writer.get_extra_info('peername')
         Debug.console(f"[Client] new conn: {self.client_id}")
         client_tag = f"{'.'.join(self.client_id[0].split('.')[-2:])}:{str(self.client_id[1])}"
         self.client_id = client_tag
-        self.shell = Shell(self.send)
+        #self.shell = Shell(self.send)
+        super().__init__()
         self.last_msg_t = ticks_ms()
 
     async def read(self):
         """
         Implements client read function, reader size: 2048
         - set timeout counter
         - read input from client (run: return False)
@@ -79,15 +80,15 @@
         return False, request
 
     def send(self, response):
         """
         Send response to client with non-async function
         """
         if self.connected:
-            if self.shell.prompt() != response:
+            if self.prompt() != response:
                 # Add new line if not prompt (?)
                 response = f"{response}\n"
             # Debug.console("[Client] ----- SteamWrite: {}".format(response))
             # Store data in stream buffer
             try:
                 self.writer.write(response.encode('utf8'))
             except Exception as e:
@@ -120,15 +121,15 @@
         # set drain free
         self.drain_event.set()
 
     async def close(self):
         Debug.console(f"[Client] Close connection {self.client_id}")
         self.send("Bye!\n")
         # Reset shell state machine
-        self.shell.reset()
+        self.reset()
         await asyncio.sleep_ms(50)
         try:
             self.writer.close()
             await self.writer.wait_closed()
         except Exception as e:
             Debug.console(f"[Client] Close error {self.client_id}: {e}")
         self.connected = False
@@ -145,15 +146,15 @@
         # Update server task output (? test ?)
         Manager().server_task_msg(','.join(list(Client.ACTIVE_CLIS.keys())))
 
     async def __shell_cmd(self, request):
         # Run micrOS shell with request string
         try:
             Debug.console("[CLIENT] --- #Run shell")
-            state = self.shell.shell(request)
+            state = self.shell(request)
             if state:
                 return True
         except Exception as e:
             if "ECONNRESET" in e:
                 await self.close()
             Debug.console(f"[Client] Shell exception: {e}")
             return False
@@ -162,28 +163,28 @@
         return True
 
     async def run_shell(self):
         # Update server task output (? test ?)
         Manager().server_task_msg(','.join(list(Client.ACTIVE_CLIS.keys())))
 
         # Init prompt
-        self.send(self.shell.prompt())
+        self.send(self.prompt())
         # Run async connection handling
         while self.connected:
             try:
                 # Read request msg from client
                 state, request = await self.read()
                 if state:
                     break
 
                 state = await self.__shell_cmd(request)
                 if not state:
                     self.send("[HA] Critical error - disconnect & hard reset")
                     errlog_add("[ERR] Socket critical error - reboot")
-                    self.shell.reboot()
+                    self.reboot()
             except Exception as e:
                 errlog_add(f"[ERR] handle_client: {e}")
                 break
         # Close connection
         await self.close()
 
     def __del__(self):
```

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.22.0/micrOS/source/TaskManager.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/Time.py` & `micrOSDevToolKit-1.22.0/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.22.0/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.22.0/micrOS/source/micrOS.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.22.0/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOS/source/urequests.py` & `micrOSDevToolKit-1.22.0/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.22.0/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.21.5
+Version: 1.22.0
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.22.0/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/setup.py` & `micrOSDevToolKit-1.22.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.21.5',
+    version='1.22.0',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.21.5/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.22.0/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.22.0/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.22.0/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/Gateway.py` & `micrOSDevToolKit-1.22.0/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.22.0/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.22.0/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.22.0/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.22.0/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.22.0/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.22.0/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.22.0/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.22.0/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/LP_darwin.py` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/LP_darwin.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/machine.py` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/machine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/micropython.py` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/micropython.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/neopixel.py` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/network.py` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/sim_console.py` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/sim_console.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/simulator.py` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/simulator.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/uasyncio.py` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/utime.py` & `micrOSDevToolKit-1.22.0/toolkit/simulator_lib/utime.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/socketClient.py` & `micrOSDevToolKit-1.22.0/toolkit/socketClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Common.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Common.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/ConfigHandler.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/ConfigHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Debug.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Debug.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Hooks.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Hooks.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/InterConnect.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/InterConnect.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/InterpreterShell.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/InterpreterShell.mpy`

 * *Files 16% similar despite different names*

```diff
@@ -1,261 +1,260 @@
-00000000: 4d06 001f 6d26 2649 6e74 6572 7072 6574  M...m&&Interpret
+00000000: 4d06 001f 6e26 2649 6e74 6572 7072 6574  M...n&&Interpret
 00000010: 6572 5368 656c 6c2e 7079 000f 0e6c 6973  erShell.py...lis
 00000020: 7464 6972 0004 6f73 000e 6d6f 6475 6c65  tdir..os..module
 00000030: 7300 0673 7973 000c 6366 6767 6574 000c  s..sys..cfgget..
 00000040: 6366 6770 7574 001a 436f 6e66 6967 4861  cfgput..ConfigHa
 00000050: 6e64 6c65 7200 1865 7865 635f 6c6d 5f63  ndler..exec_lm_c
 00000060: 6f72 6500 1654 6173 6b4d 616e 6167 6572  ore..TaskManager
 00000070: 001a 636f 6e73 6f6c 655f 7772 6974 6500  ..console_write.
 00000080: 1465 7272 6c6f 675f 6164 6400 0a44 6562  .errlog_add..Deb
 00000090: 7567 000a 7265 7365 7400 1473 6f66 745f  ug..reset..soft_
 000000a0: 7265 7365 7400 0e6d 6163 6869 6e65 000a  reset..machine..
-000000b0: 5368 656c 6c00 1031 2e32 312e 312d 3000  Shell..1.21.1-0.
-000000c0: 230e 6d73 675f 6f62 6a00 0c64 6576 6669  #.msg_obj..devfi
-000000d0: 6400 105f 5f64 6576 6669 6400 0861 7574  d..__devfid..aut
-000000e0: 6800 165f 5f61 7574 685f 6d6f 6465 000a  h..__auth_mode..
-000000f0: 6877 7569 6400 0e5f 5f68 7775 6964 0012  hwuid..__hwuid..
-00000100: 5f5f 6175 7468 5f6f 6b00 165f 5f63 6f6e  __auth_ok..__con
-00000110: 665f 6d6f 6465 000e 7665 7273 696f 6e00  f_mode..version.
-00000120: 1c4d 4943 524f 535f 5645 5253 494f 4e00  .MICROS_VERSION.
-00000130: 8129 066d 7367 000c 7265 626f 6f74 000e  .).msg..reboot..
-00000140: 5b48 4152 445d 2000 0308 4279 6521 000c  [HARD] ...Bye!..
-00000150: 7072 6f6d 7074 0012 7b7d 7b7d 7b7d 2024  prompt..{}{}{} $
-00000160: 2000 205f 5f61 7574 6865 6e74 6963 6174   . __authenticat
-00000170: 696f 6e00 0a61 7070 7764 0082 310c 4175  ion..appwd..1.Au
-00000180: 7468 4f6b 000a 7368 656c 6c00 0e5f 5f73  thOk..shell..__s
-00000190: 6865 6c6c 0082 230a 6865 6c6c 6f00 042d  hell..#.hello..-
-000001a0: 6800 8227 0e77 6562 7265 706c 0004 2d75  h..'.webrepl..-u
-000001b0: 0082 3f08 636f 6e66 000c 6e6f 636f 6e66  ..?.conf..noconf
-000001c0: 0008 6865 6c70 0004 6c6d 001c 5f73 686f  ..help..lm.._sho
-000001d0: 775f 6c6d 5f66 756e 6373 0016 6163 7469  w_lm_funcs..acti
-000001e0: 7665 5f6f 6e6c 7900 145f 636f 6e66 6967  ve_only.._config
-000001f0: 7572 6500 1061 7267 5f6c 6973 7400 0c6d  ure..arg_list..m
-00000200: 7367 6f62 6a00 0864 756d 7000 814d 0981  sgobj..dump..M..
-00000210: 5114 7479 7065 5f63 6865 636b 000a 5361  Q.type_check..Sa
-00000220: 7665 6400 8155 1069 6663 6f6e 6669 6700  ved..U.ifconfig.
-00000230: 0e4e 6574 776f 726b 000a 2042 7965 2100  .Network.. Bye!.
-00000240: 102e 6966 5f6d 6f64 6500 0277 0082 4982  ..if_mode..w..I.
-00000250: 2510 7061 7373 776f 7264 001a 5f6f 6666  %.password.._off
-00000260: 6c69 6e65 5f68 656c 7000 8203 064c 4d5f  line_help....LM_
-00000270: 0002 2e00 0a20 2020 7b7d 0081 1f08 2e6d  .....   {}.....m
-00000280: 7079 0012 2020 207b 7d68 656c 7000 0272  py..   {}help..r
-00000290: 0081 7f06 6465 6600 1182 130e 2020 207b  ....def.....   {
-000002a0: 7d7b 7d00 0864 6566 2000 0228 0012 3c67  }{}..def ..(..<g
-000002b0: 656e 6578 7072 3e00 0470 7900 1468 6172  enexpr>..py..har
-000002c0: 645f 7265 7365 7400 2f2d 3582 2949 8177  d_reset./-5.)I.w
-000002d0: 0868 6172 6400 106d 7367 5f6c 6973 7400  .hard..msg_list.
-000002e0: 8157 822f 1461 7474 7269 6275 7465 7300  .W./.attributes.
-000002f0: 816d 0b16 6d6f 6475 6c65 5f6c 6973 7400  .m..module_list.
-00000300: 052a 4578 706f 7274 2073 7973 7465 6d20  .*Export system 
-00000310: 7665 7273 696f 6e20 746f 2063 6f6e 6669  version to confi
-00000320: 6720 6661 696c 6564 3a20 7b7d 0005 2c5b  g failed: {}..,[
-00000330: 5368 656c 6c5d 5b45 5252 5d20 7379 7374  Shell][ERR] syst
-00000340: 656d 2076 6572 7369 6f6e 2065 7870 6f72  em version expor
-00000350: 7420 6572 726f 723a 207b 7d00 0517 7b7d  t error: {}...{}
-00000360: 5265 626f 6f74 206d 6963 724f 5320 7379  Reboot micrOS sy
-00000370: 7374 656d 2e00 050b 5b70 6173 7377 6f72  stem....[passwor
-00000380: 645d 2000 050c 5b63 6f6e 6669 6775 7265  d] ...[configure
-00000390: 5d20 0005 0f41 7574 6846 6169 6c65 640a  ] ...AuthFailed.
-000003a0: 4279 6521 0005 0b68 656c 6c6f 3a7b 7d3a  Bye!...hello:{}:
-000003b0: 7b7d 0005 245b 4d49 4352 4f53 5d20 2020  {}..$[MICROS]   
-000003c0: 2d20 6275 696c 742d 696e 2073 6865 6c6c  - built-in shell
-000003d0: 2063 6f6d 6d61 6e64 7300 0532 2020 2068   commands..2   h
-000003e0: 656c 6c6f 2020 202d 2068 656c 6c6f 206d  ello   - hello m
-000003f0: 7367 202d 2066 6f72 2064 6576 6963 6520  sg - for device 
-00000400: 6964 656e 7469 6669 6361 7469 6f6e 0005  identification..
-00000410: 2320 2020 7665 7273 696f 6e20 2d20 7265  #   version - re
-00000420: 7475 726e 7320 6d69 6372 4f53 2076 6572  turns micrOS ver
-00000430: 7369 6f6e 0005 2a20 2020 6578 6974 2020  sion..*   exit  
-00000440: 2020 2d20 6578 6974 2066 726f 6d20 7368    - exit from sh
-00000450: 656c 6c20 736f 636b 6574 2070 726f 6d70  ell socket promp
-00000460: 7400 0541 2020 2072 6562 6f6f 7420 202d  t..A   reboot  -
-00000470: 2073 7973 7465 6d20 736f 6674 2072 6562   system soft reb
-00000480: 6f6f 7420 2876 6d29 2c20 6861 7264 2072  oot (vm), hard r
-00000490: 6562 6f6f 7420 2868 7729 3a20 7265 626f  eboot (hw): rebo
-000004a0: 6f74 202d 6800 0540 2020 2077 6562 7265  ot -h..@   webre
-000004b0: 706c 202d 2073 7461 7274 2077 6562 7265  pl - start webre
-000004c0: 706c 2c20 666f 7220 6669 6c65 2074 7261  pl, for file tra
-000004d0: 6e73 6665 7273 2075 7365 2077 6974 6820  nsfers use with 
-000004e0: 2d2d 7570 6461 7465 0005 2f5b 434f 4e46  --update../[CONF
-000004f0: 5d20 436f 6e66 6967 7572 6520 6d6f 6465  ] Configure mode
-00000500: 202d 2062 7569 6c74 2d69 6e20 7368 656c   - built-in shel
-00000510: 6c20 636f 6d6d 616e 6473 0005 1e20 2063  l commands...  c
-00000520: 6f6e 6620 2020 2020 2020 2d20 456e 7465  onf       - Ente
-00000530: 7220 636f 6e66 206d 6f64 6500 051e 2020  r conf mode...  
-00000540: 2020 6475 6d70 2020 2020 2020 202d 2044    dump       - D
-00000550: 756d 7020 616c 6c20 6461 7461 0005 1a20  ump all data... 
-00000560: 2020 206b 6579 2020 2020 2020 2020 2d20     key        - 
-00000570: 4765 7420 7661 6c75 6500 051a 2020 2020  Get value...    
-00000580: 6b65 7920 7661 6c75 6520 202d 2053 6574  key value  - Set
-00000590: 2076 616c 7565 0005 1d20 206e 6f63 6f6e   value...  nocon
-000005a0: 6620 2020 2020 2d20 4578 6974 2063 6f6e  f     - Exit con
-000005b0: 6620 6d6f 6465 0005 485b 5441 534b 5d20  f mode..H[TASK] 
-000005c0: 706f 7374 6669 783a 2026 7820 2d20 6f6e  postfix: &x - on
-000005d0: 652d 7469 6d65 2c20 2026 2678 202d 2070  e-time,  &&x - p
-000005e0: 6572 696f 6469 632c 2078 3a20 7761 6974  eriodic, x: wait
-000005f0: 206d 7320 5b78 206d 696e 3a20 3230 6d73   ms [x min: 20ms
-00000600: 5d00 052c 2020 7461 736b 206c 6973 7420  ]..,  task list 
-00000610: 2020 2020 2020 2020 2d20 6c69 7374 2074          - list t
-00000620: 6173 6b73 2077 6974 6820 3c74 6167 3e73  asks with <tag>s
-00000630: 0005 1f20 2074 6173 6b20 6b69 6c6c 203c  ...  task kill <
-00000640: 7461 673e 2020 202d 2073 746f 7020 7461  tag>   - stop ta
-00000650: 736b 0005 2620 2074 6173 6b20 7368 6f77  sk..&  task show
-00000660: 203c 7461 673e 2020 202d 2073 686f 7720   <tag>   - show 
-00000670: 7461 736b 206f 7574 7075 7400 051a 5b45  task output...[E
-00000680: 5845 435d 2043 6f6d 6d61 6e64 206d 6f64  XEC] Command mod
-00000690: 6520 284c 4d73 293a 0005 2220 2020 6865  e (LMs):.."   he
-000006a0: 6c70 206c 6d20 202d 206c 6973 7420 414c  lp lm  - list AL
-000006b0: 4c20 4c6f 6164 4d6f 6475 6c65 7300 0528  L LoadModules..(
-000006c0: 5b45 5252 4f52 5d20 6578 6563 5f6c 6d5f  [ERROR] exec_lm_
-000006d0: 7368 656c 6c20 696e 7465 726e 616c 2065  shell internal e
-000006e0: 7272 6f72 3a20 7b7d 0005 0c20 207b 7d7b  rror: {}...  {}{
-000006f0: 7d3a 7b7d 207b 7d00 051b 6e6f 6465 5f63  }:{} {}...node_c
-00000700: 6f6e 6669 6720 7772 6974 6520 6572 726f  onfig write erro
-00000710: 723a 207b 7d00 050b 496e 7661 6c69 6420  r: {}...Invalid 
-00000720: 6b65 7900 050e 4661 696c 6564 2074 6f20  key...Failed to 
-00000730: 7361 7665 0005 3820 5374 6172 7420 6d69  save..8 Start mi
-00000740: 6372 6f70 7974 686f 6e20 5745 4252 4550  cropython WEBREP
-00000750: 4c20 2d20 6669 6c65 2074 7261 6e73 6665  L - file transfe
-00000760: 7220 616e 6420 6465 6275 6767 696e 6700  r and debugging.
-00000770: 052c 2020 5b69 5d20 7265 7374 6172 7420  .,  [i] restart 
-00000780: 6d61 6368 696e 6520 7368 6f72 7463 7574  machine shortcut
-00000790: 3a20 696d 706f 7274 2072 6573 6574 0005  : import reset..
-000007a0: 3720 2043 6f6e 6e65 6374 206f 7665 7220  7  Connect over 
-000007b0: 6874 7470 3a2f 2f6d 6963 726f 7079 7468  http://micropyth
-000007c0: 6f6e 2e6f 7267 2f77 6562 7265 706c 2f23  on.org/webrepl/#
-000007d0: 7b7d 3a38 3236 362f 0005 1b20 2009 5b21  {}:8266/...  .[!
-000007e0: 5d20 7765 6272 6570 6c20 7061 7373 776f  ] webrepl passwo
-000007f0: 7264 3a20 7b7d 0005 2420 2052 6573 7461  rd: {}..$  Resta
-00000800: 7274 206e 6f64 6520 7468 656e 2073 7461  rt node then sta
-00000810: 7274 2077 6562 7265 706c 2e2e 2e00 0520  rt webrepl..... 
-00000820: 5b45 5252 5d20 7768 696c 6520 7374 6172  [ERR] while star
-00000830: 7469 6e67 2077 6562 7265 706c 3a20 7b7d  ting webrepl: {}
-00000840: 0005 0f6d 6963 724f 5369 7354 6865 4265  ...micrOSisTheBe
-00000850: 7374 0005 1f5b 7b7d 5d20 5348 4f57 204c  st...[{}] SHOW L
-00000860: 4d20 5041 5253 4552 2057 4152 4e49 4e47  M PARSER WARNING
-00000870: 3a20 7b7d 0087 1410 1601 800d 2c2c 322c  : {}........,,2,
-00000880: 3272 6020 8010 022a 011b 031c 0216 0259  2r` ...*.......Y
-00000890: 8010 042a 011b 051c 0416 0459 8010 0610  ...*.......Y....
-000008a0: 072a 021b 081c 0616 061c 0716 0759 8010  .*...........Y..
-000008b0: 092a 011b 0a1c 0916 0959 8010 0b10 0c2a  .*.......Y.....*
-000008c0: 021b 0d1c 0b16 0b1c 0c16 0c59 8010 0e10  ...........Y....
-000008d0: 0f2a 021b 101c 0e16 5e1c 0f16 0f59 5432  .*......^....YT2
-000008e0: 0010 1134 0216 1151 6301 8704 1030 1188  ...4...Qc....0..
-000008f0: 1a44 8814 8407 6440 8808 6460 840e 8409  .D....d@..d`....
-00000900: 846a 8825 8c21 115f 1660 1011 1661 1012  .j.%.!._.`...a..
-00000910: 161e 512a 0153 3300 1613 3201 1620 3202  ..Q*.S3...2.. 2.
-00000920: 160e 502a 0153 3303 1621 3204 1625 3205  ..P*.S3..!2..%2.
-00000930: 1627 3206 162b 3207 162c 1162 3208 3401  .'2..+2..,.b2.4.
-00000940: 163a 1162 502a 0153 3309 3401 1638 1162  .:.bP*.S3.4..8.b
-00000950: 502a 0153 330a 3401 1631 5163 0b87 28ca  P*.S3.4..1Qc..(.
-00000960: 0320 1358 1480 1d60 2044 2929 4924 4422  . .X...` D))I$D"
-00000970: 562c b1b0 1814 1206 1015 3401 b018 1612  V,........4.....
-00000980: 0610 1734 01b0 1818 1206 1019 3401 b018  ...4........4...
-00000990: 1a50 b018 1b50 b018 1c48 0d12 0710 1d12  .P...P...H......
-000009a0: 1113 1e34 0259 4a2a 5712 63df 4463 c249  ...4.YJ*W.c.Dc.I
-000009b0: 1912 0b23 0014 1fb2 3601 3401 5912 0c23  ...#....6.4.Y..#
-000009c0: 0114 1fb2 3601 3401 5951 51c2 2802 5d4a  ....6.4.YQQ.(.]J
-000009d0: 015d 5163 8208 3610 2058 2080 3120 224a  .]Qc..6. X .1 "J
-000009e0: 4809 b014 14b1 3601 594a 0a59 1264 b134  H.....6.YJ.Y.d.4
-000009f0: 0159 4a01 5d51 6381 1011 0c0e 5880 3820  .YJ.]Qc.....X.8 
-00000a00: 2450 b018 1b50 b018 1c51 6383 48b2 0114  $P...P...Qc.H...
-00000a10: 2158 6580 3d20 3528 2325 b014 2023 0214  !Xe.= 5(#%.. #..
-00000a20: 1fb1 4444 1022 4242 1023 3601 3601 59b0  ..DD."BB.#6.6.Y.
-00000a30: 1420 1024 3601 59b1 4445 125e 3400 5912  . .$6.Y.DE.^4.Y.
-00000a40: 0f34 0059 5163 8310 390e 2558 8045 2031  .4.YQc..9.%X.E 1
-00000a50: 2cb0 1318 4449 b013 1b43 4423 0342 4210  ,...DI...CD#.BB.
-00000a60: 23c1 b013 1c44 4423 0442 4210 23c2 1026  #....DD#.BB.#..&
-00000a70: 141f b1b2 b013 1636 0363 8508 2a1c 2758  .......6.c..*.'X
-00000a80: 6680 4b40 4a27 2b24 2826 2826 b013 1844  f.K@J'+$(&(&...D
-00000a90: 77b0 131b 4372 1206 1028 3401 c2b2 b180  w...Cr...(4.....
-00000aa0: 5514 2936 00d9 4452 52b0 181b b014 2010  U.)6..DRR..... .
-00000ab0: 2a36 0159 522b 002a 0263 b014 2023 0536  *6.YR+.*.c.. #.6
-00000ac0: 0159 502b 002a 0263 52b1 2a02 6381 7832  .YP+.*.cR.*.c.x2
-00000ad0: 122b 5820 8059 6020 272b b014 2cb1 3601  .+X .Y` '+..,.6.
-00000ae0: c2b0 1420 b014 2536 0036 0159 b263 a400  ... ..%6.6.Y.c..
-00000af0: ea02 8602 2c58 2080 6280 0b52 228a 0848  ....,X .b..R"..H
-00000b00: 3242 2a23 2229 6248 2e62 2822 5122 472b  2B*#")bH.b("Q"G+
-00000b10: 3130 6d2b 2422 2b24 6229 2828 2828 2828  10m+$"+$b)((((((
-00000b20: 2828 2828 2828 2828 2828 2828 2a2d 7020  ((((((((((((*-p 
-00000b30: 4e4b 6040 4259 2db1 51de 434d 1267 b114  NK`@BY-.Q.CM.g..
-00000b40: 2936 0034 0180 d944 4252 63b1 1429 3600  )6.4...DBRc..)6.
-00000b50: 142d 3600 c2b2 8055 102e d944 54b0 1420  .-6....U...DT.. 
-00000b60: 2306 141f b013 16b0 131a 3602 3601 5952  #.........6.6.YR
-00000b70: 63b0 1427 b236 0130 02c3 c2b3 4342 5063  c..'.6.0....CBPc
-00000b80: 1267 b234 0180 d944 4252 63b2 8055 101d  .g.4...DBRc..U..
-00000b90: d944 50b0 1420 1268 1211 131e 3401 3601  .DP.. .h....4.6.
-00000ba0: 5952 63b2 8055 1021 d944 5c50 c412 67b2  YRc..U.!.D\P..g.
-00000bb0: 3401 82db 444a 102f b281 55dd 4442 52c4  4...DJ./..U.DBR.
-00000bc0: b014 21b4 3601 59b2 8055 1430 1031 3601  ..!.6.Y..U.0.16.
-00000bd0: 446e 1267 b234 0182 d944 5810 32b2 8155  Dn.g.4...DX.2..U
-00000be0: dd44 5012 1114 3110 14b0 1320 1033 5236  .DP...1.... .3R6
-00000bf0: 8400 5912 1114 3110 14b0 1320 3682 0059  ..Y...1.... 6..Y
-00000c00: b280 5514 3010 3436 0144 4652 b018 1c52  ..U.0.46.DFR...R
-00000c10: 63b2 8055 1430 1035 3601 4446 50b0 181c  c..U.0.56.DFP...
-00000c20: 5263 b280 5510 36d9 44b7 81b0 1420 2307  Rc..U.6.D.... #.
-00000c30: 3601 59b0 1420 2308 3601 59b0 1420 2309  6.Y.. #.6.Y.. #.
-00000c40: 3601 59b0 1420 230a 3601 59b0 1420 230b  6.Y.. #.6.Y.. #.
-00000c50: 3601 59b0 1420 230c 3601 59b0 1420 230d  6.Y.. #.6.Y.. #.
-00000c60: 3601 59b0 1420 230e 3601 59b0 1420 230f  6.Y.. #.6.Y.. #.
-00000c70: 3601 59b0 1420 2310 3601 59b0 1420 2311  6.Y.. #.6.Y.. #.
-00000c80: 3601 59b0 1420 2312 3601 59b0 1420 2313  6.Y.. #.6.Y.. #.
-00000c90: 3601 59b0 1420 2314 3601 59b0 1420 2315  6.Y.. #.6.Y.. #.
-00000ca0: 3601 59b0 1420 2316 3601 59b0 1420 2317  6.Y.. #.6.Y.. #.
-00000cb0: 3601 59b0 1420 2318 3601 5910 3712 68b2  6.Y.. #.6.Y.7.h.
-00000cc0: 3401 dd44 4d12 1114 3810 14b0 1320 3682  4..DM...8.... 6.
-00000cd0: 0063 1211 1438 1014 b013 2010 3952 3684  .c...8.... .9R6.
-00000ce0: 0063 b013 1c44 5412 67b2 3401 80d8 444b  .c...DT.g.4...DK
-00000cf0: 1211 143a b013 20b2 3602 6348 1012 0910  ...:.. .6.cH....
-00000d00: 3bb2 103c b013 2034 8400 634a 2157 1263  ;..<.. 4..cJ!W.c
-00000d10: df44 5ac5 4910 b014 2023 1914 1fb5 3601  .DZ.I... #....6.
-00000d20: 3601 5950 6351 51c5 2805 5d4a 015d 5163  6.YPcQQ.(.]J.]Qc
-00000d30: 8d00 9212 303a 1469 80cd 6060 2a48 2f28  ....0:.i..``*H/(
-00000d40: 3642 2b42 4a24 4d22 562b 4b30 2c12 67b1  6B+BJ$M"V+K0,.g.
-00000d50: 3401 81d9 44c4 80b1 8055 103d d944 6f12  4...D....U.=.Do.
-00000d60: 0634 0014 3e36 005f 4b22 3002 c2c3 8a12  .4..>6._K"0.....
-00000d70: 67b2 3401 f3c4 b023 1a14 1fb2 103f b4f4  g.4....#.....?..
-00000d80: 103f 87f4 b336 0434 0159 421c 5263 b012  .?...6.4.YB.Rc..
-00000d90: 06b1 8055 3401 3401 5952 6312 67b1 3401  ...U4.4.YRc.g.4.
-00000da0: 82db 44db 80b1 8055 c210 3f14 40b1 8151  ..D....U..?.@..Q
-00000db0: 2e02 5536 01c3 480d 1207 b2b3 1041 5234  ..U6..H......AR4
-00000dc0: 8202 c54a 1f57 1263 df44 58c6 490e b023  ...J.W.c.DX.I..#
-00000dd0: 1b14 1fb6 3601 3401 5950 c551 51c6 2806  ....6.4.YP.QQ.(.
-00000de0: 5d4a 015d 1206 b234 0151 de44 4423 1c42  ]J.]...4.Q.DD#.B
-00000df0: 4223 1dc7 b0b5 4444 1042 4241 b734 0159  B#....DD.BBA.4.Y
-00000e00: 5263 8364 b201 9a01 3814 3980 f260 2085  Rc.d....8.9..` .
-00000e10: 1423 282c 4500 04b0 2000 01c2 b144 5912  .#(,E... ....DY.
-00000e20: 0414 4336 0027 04b4 2001 0112 0234 005e  ..C6.'.. ....4.^
-00000e30: 3401 c3b2 b334 0163 b212 0234 0034 0163  4....4.c...4.4.c
-00000e40: 028f 4ca2 122c 4c6b 6c80 f72b 3223 2c29  ..L..,Lkl..+2#,)
-00000e50: 1f24 242a 2323 263b 1f57 2d2e 3200 b15e  .$$*##&;.W-.2..^
-00000e60: 3401 5f4b d401 c2b2 144d 104e 1023 3602  4._K.....M.N.#6.
-00000e70: 142d 104f 3601 8055 c348 9a01 2500 1050  .-.O6..U.H..%..P
-00000e80: 141f b336 0134 0159 b214 5110 5236 0144  ...6.4.Y..Q.R6.D
-00000e90: 6725 0010 5314 1f10 3f12 67b2 144d 104e  g%..S...?.g..M.N
-00000ea0: 1023 3602 142d 104f 3601 8055 3401 f436  .#6..-.O6..U4..6
-00000eb0: 0134 0159 40ac 7f01 126a b210 5434 0247  .4.Y@....j..T4.G
-00000ec0: 51c4 2324 c542 c580 b414 5536 00c5 b514  Q.#$.B....U6....
-00000ed0: 2936 0014 3010 5636 0144 7210 57b5 ddd3  )6..0.V6.Dr.W...
-00000ee0: 446b 1058 b5dd d344 6425 0010 5914 1f10  Dk.X...Dd%..Y...
-00000ef0: 3f12 67b3 3401 f4b5 144d 105a 1023 3602  ?.g.4....M.Z.#6.
-00000f00: 142d 105b 3601 8055 3602 3401 59b5 43b7  .-.[6..U6.4.Y.C.
-00000f10: 7f51 5c5d 4a21 5712 63df 445a c649 1025  .Q\]J!W.c.DZ.I.%
-00000f20: 0023 2514 1fb2 b636 0234 0159 5063 5151  .#%....6.4.YPcQQ
-00000f30: c628 065d 4a01 5d42 a97e 5263 0182 38c1  .(.]J.]B.~Rc..8.
-00000f40: 4008 5c6b 80f7 53b0 5353 4b18 c1b1 1430  @.\k..S.SSK....0
-00000f50: 104e 3601 4434 b114 5110 5d36 0144 2bb1  .N6.D4..Q.]6.D+.
-00000f60: 6759 4226 5163 8220 ca40 0a5c 6b6b 900c  gYB&Qc. .@.\kk..
-00000f70: 53b1 5353 4b14 c2b2 142d 104f 3601 8055  S.SSK....-.O6..U
-00000f80: 2500 dd44 2fb2 6759 422a 5163 8c00 e203  %..D/.gYB*Qc....
-00000f90: 2c31 1433 9013 4b26 2631 3023 2626 432b  ,1.3..K&&10#&&C+
-00000fa0: 2b25 2225 5d28 2580 1044 2a01 1b45 1c44  +%"%](%..D*..E.D
-00000fb0: c259 b023 1e34 0159 b023 1f34 0159 b023  .Y.#.4.Y.#.4.Y.#
-00000fc0: 2014 1fb2 3400 8155 8055 3601 3401 59b0   ...4..U.U6.4.Y.
-00000fd0: 2321 141f 1206 1028 3401 3601 3401 59b1  #!.....(4.6.4.Y.
-00000fe0: 4446 b023 2234 0159 b010 4634 0159 b144  DF.#"4.Y..F4.Y.D
-00000ff0: 5b12 6a10 4710 4834 0247 0ac3 b314 4910  [.j.G.H4.G....I.
-00001000: 3136 0159 515c 5d12 5e34 0059 4819 8051  16.YQ\].^4.YH..Q
-00001010: 1b31 c4b0 b414 4a10 4b12 0610 2834 0136  .1....J.K...(4.6
-00001020: 8200 3401 594a 2557 1263 df44 5ec5 4914  ..4.YJ%W.c.D^.I.
-00001030: 2323 141f b536 01c6 b0b6 3401 5912 0cb6  ##...6....4.Y...
-00001040: 3401 5951 51c5 2805 5d4a 015d 5163       4.YQQ.(.]J.]Qc
+000000b0: 5368 656c 6c00 1031 2e32 322e 302d 3000  Shell..1.22.0-0.
+000000c0: 230c 6465 7666 6964 0010 5f5f 6465 7666  #.devfid..__devf
+000000d0: 6964 0008 6175 7468 0016 5f5f 6175 7468  id..auth..__auth
+000000e0: 5f6d 6f64 6500 0a68 7775 6964 000e 5f5f  _mode..hwuid..__
+000000f0: 6877 7569 6400 125f 5f61 7574 685f 6f6b  hwuid..__auth_ok
+00000100: 0016 5f5f 636f 6e66 5f6d 6f64 6500 0e76  ..__conf_mode..v
+00000110: 6572 7369 6f6e 001c 4d49 4352 4f53 5f56  ersion..MICROS_V
+00000120: 4552 5349 4f4e 0081 2982 150c 7265 626f  ERSION..)...rebo
+00000130: 6f74 000e 5b48 4152 445d 2000 0308 4279  ot..[HARD] ...By
+00000140: 6521 000c 7072 6f6d 7074 0012 7b7d 7b7d  e!..prompt..{}{}
+00000150: 7b7d 2024 2000 205f 5f61 7574 6865 6e74  {} $ . __authent
+00000160: 6963 6174 696f 6e00 0a61 7070 7764 0082  ication..appwd..
+00000170: 310c 4175 7468 4f6b 000a 7368 656c 6c00  1.AuthOk..shell.
+00000180: 0e5f 5f73 6865 6c6c 0082 230a 6865 6c6c  .__shell..#.hell
+00000190: 6f00 042d 6800 8227 0e77 6562 7265 706c  o..-h..'.webrepl
+000001a0: 0004 2d75 000e 6d73 675f 6f62 6a00 823f  ..-u..msg_obj..?
+000001b0: 0863 6f6e 6600 0c6e 6f63 6f6e 6600 0868  .conf..noconf..h
+000001c0: 656c 7000 046c 6d00 1c5f 7368 6f77 5f6c  elp..lm.._show_l
+000001d0: 6d5f 6675 6e63 7300 1661 6374 6976 655f  m_funcs..active_
+000001e0: 6f6e 6c79 0014 5f63 6f6e 6669 6775 7265  only.._configure
+000001f0: 0010 6172 675f 6c69 7374 000c 6d73 676f  ..arg_list..msgo
+00000200: 626a 0008 6475 6d70 0081 4d09 8151 1474  bj..dump..M..Q.t
+00000210: 7970 655f 6368 6563 6b00 0a53 6176 6564  ype_check..Saved
+00000220: 0081 5510 6966 636f 6e66 6967 000e 4e65  ..U.ifconfig..Ne
+00000230: 7477 6f72 6b00 0a20 4279 6521 0010 2e69  twork.. Bye!...i
+00000240: 665f 6d6f 6465 0002 7700 8249 8225 1070  f_mode..w..I.%.p
+00000250: 6173 7377 6f72 6400 1a5f 6f66 666c 696e  assword.._offlin
+00000260: 655f 6865 6c70 0082 0306 4c4d 5f00 022e  e_help....LM_...
+00000270: 000a 2020 207b 7d00 811f 082e 6d70 7900  ..   {}.....mpy.
+00000280: 1220 2020 7b7d 6865 6c70 0002 7200 817f  .   {}help..r...
+00000290: 0664 6566 0011 8213 0e20 2020 7b7d 7b7d  .def.....   {}{}
+000002a0: 0008 6465 6620 0002 2800 123c 6765 6e65  ..def ..(..<gene
+000002b0: 7870 723e 0004 7079 0014 6861 7264 5f72  xpr>..py..hard_r
+000002c0: 6573 6574 002f 2d35 8229 4906 6d73 6700  eset./-5.)I.msg.
+000002d0: 8177 0868 6172 6400 106d 7367 5f6c 6973  .w.hard..msg_lis
+000002e0: 7400 8157 822f 1461 7474 7269 6275 7465  t..W./.attribute
+000002f0: 7300 816d 0b16 6d6f 6475 6c65 5f6c 6973  s..m..module_lis
+00000300: 7400 052a 4578 706f 7274 2073 7973 7465  t..*Export syste
+00000310: 6d20 7665 7273 696f 6e20 746f 2063 6f6e  m version to con
+00000320: 6669 6720 6661 696c 6564 3a20 7b7d 0005  fig failed: {}..
+00000330: 2c5b 5368 656c 6c5d 5b45 5252 5d20 7379  ,[Shell][ERR] sy
+00000340: 7374 656d 2076 6572 7369 6f6e 2065 7870  stem version exp
+00000350: 6f72 7420 6572 726f 723a 207b 7d00 0517  ort error: {}...
+00000360: 7b7d 5265 626f 6f74 206d 6963 724f 5320  {}Reboot micrOS 
+00000370: 7379 7374 656d 2e00 050b 5b70 6173 7377  system....[passw
+00000380: 6f72 645d 2000 050c 5b63 6f6e 6669 6775  ord] ...[configu
+00000390: 7265 5d20 0005 0f41 7574 6846 6169 6c65  re] ...AuthFaile
+000003a0: 640a 4279 6521 0005 0b68 656c 6c6f 3a7b  d.Bye!...hello:{
+000003b0: 7d3a 7b7d 0005 245b 4d49 4352 4f53 5d20  }:{}..$[MICROS] 
+000003c0: 2020 2d20 6275 696c 742d 696e 2073 6865    - built-in she
+000003d0: 6c6c 2063 6f6d 6d61 6e64 7300 0532 2020  ll commands..2  
+000003e0: 2068 656c 6c6f 2020 202d 2068 656c 6c6f   hello   - hello
+000003f0: 206d 7367 202d 2066 6f72 2064 6576 6963   msg - for devic
+00000400: 6520 6964 656e 7469 6669 6361 7469 6f6e  e identification
+00000410: 0005 2320 2020 7665 7273 696f 6e20 2d20  ..#   version - 
+00000420: 7265 7475 726e 7320 6d69 6372 4f53 2076  returns micrOS v
+00000430: 6572 7369 6f6e 0005 2a20 2020 6578 6974  ersion..*   exit
+00000440: 2020 2020 2d20 6578 6974 2066 726f 6d20      - exit from 
+00000450: 7368 656c 6c20 736f 636b 6574 2070 726f  shell socket pro
+00000460: 6d70 7400 0541 2020 2072 6562 6f6f 7420  mpt..A   reboot 
+00000470: 202d 2073 7973 7465 6d20 736f 6674 2072   - system soft r
+00000480: 6562 6f6f 7420 2876 6d29 2c20 6861 7264  eboot (vm), hard
+00000490: 2072 6562 6f6f 7420 2868 7729 3a20 7265   reboot (hw): re
+000004a0: 626f 6f74 202d 6800 0540 2020 2077 6562  boot -h..@   web
+000004b0: 7265 706c 202d 2073 7461 7274 2077 6562  repl - start web
+000004c0: 7265 706c 2c20 666f 7220 6669 6c65 2074  repl, for file t
+000004d0: 7261 6e73 6665 7273 2075 7365 2077 6974  ransfers use wit
+000004e0: 6820 2d2d 7570 6461 7465 0005 2f5b 434f  h --update../[CO
+000004f0: 4e46 5d20 436f 6e66 6967 7572 6520 6d6f  NF] Configure mo
+00000500: 6465 202d 2062 7569 6c74 2d69 6e20 7368  de - built-in sh
+00000510: 656c 6c20 636f 6d6d 616e 6473 0005 1e20  ell commands... 
+00000520: 2063 6f6e 6620 2020 2020 2020 2d20 456e   conf       - En
+00000530: 7465 7220 636f 6e66 206d 6f64 6500 051e  ter conf mode...
+00000540: 2020 2020 6475 6d70 2020 2020 2020 202d      dump       -
+00000550: 2044 756d 7020 616c 6c20 6461 7461 0005   Dump all data..
+00000560: 1a20 2020 206b 6579 2020 2020 2020 2020  .    key        
+00000570: 2d20 4765 7420 7661 6c75 6500 051a 2020  - Get value...  
+00000580: 2020 6b65 7920 7661 6c75 6520 202d 2053    key value  - S
+00000590: 6574 2076 616c 7565 0005 1d20 206e 6f63  et value...  noc
+000005a0: 6f6e 6620 2020 2020 2d20 4578 6974 2063  onf     - Exit c
+000005b0: 6f6e 6620 6d6f 6465 0005 485b 5441 534b  onf mode..H[TASK
+000005c0: 5d20 706f 7374 6669 783a 2026 7820 2d20  ] postfix: &x - 
+000005d0: 6f6e 652d 7469 6d65 2c20 2026 2678 202d  one-time,  &&x -
+000005e0: 2070 6572 696f 6469 632c 2078 3a20 7761   periodic, x: wa
+000005f0: 6974 206d 7320 5b78 206d 696e 3a20 3230  it ms [x min: 20
+00000600: 6d73 5d00 052c 2020 7461 736b 206c 6973  ms]..,  task lis
+00000610: 7420 2020 2020 2020 2020 2d20 6c69 7374  t         - list
+00000620: 2074 6173 6b73 2077 6974 6820 3c74 6167   tasks with <tag
+00000630: 3e73 0005 1f20 2074 6173 6b20 6b69 6c6c  >s...  task kill
+00000640: 203c 7461 673e 2020 202d 2073 746f 7020   <tag>   - stop 
+00000650: 7461 736b 0005 2620 2074 6173 6b20 7368  task..&  task sh
+00000660: 6f77 203c 7461 673e 2020 202d 2073 686f  ow <tag>   - sho
+00000670: 7720 7461 736b 206f 7574 7075 7400 051a  w task output...
+00000680: 5b45 5845 435d 2043 6f6d 6d61 6e64 206d  [EXEC] Command m
+00000690: 6f64 6520 284c 4d73 293a 0005 2220 2020  ode (LMs):.."   
+000006a0: 6865 6c70 206c 6d20 202d 206c 6973 7420  help lm  - list 
+000006b0: 414c 4c20 4c6f 6164 4d6f 6475 6c65 7300  ALL LoadModules.
+000006c0: 0528 5b45 5252 4f52 5d20 6578 6563 5f6c  .([ERROR] exec_l
+000006d0: 6d5f 7368 656c 6c20 696e 7465 726e 616c  m_shell internal
+000006e0: 2065 7272 6f72 3a20 7b7d 0005 0c20 207b   error: {}...  {
+000006f0: 7d7b 7d3a 7b7d 207b 7d00 051b 6e6f 6465  }{}:{} {}...node
+00000700: 5f63 6f6e 6669 6720 7772 6974 6520 6572  _config write er
+00000710: 726f 723a 207b 7d00 050b 496e 7661 6c69  ror: {}...Invali
+00000720: 6420 6b65 7900 050e 4661 696c 6564 2074  d key...Failed t
+00000730: 6f20 7361 7665 0005 3820 5374 6172 7420  o save..8 Start 
+00000740: 6d69 6372 6f70 7974 686f 6e20 5745 4252  micropython WEBR
+00000750: 4550 4c20 2d20 6669 6c65 2074 7261 6e73  EPL - file trans
+00000760: 6665 7220 616e 6420 6465 6275 6767 696e  fer and debuggin
+00000770: 6700 052c 2020 5b69 5d20 7265 7374 6172  g..,  [i] restar
+00000780: 7420 6d61 6368 696e 6520 7368 6f72 7463  t machine shortc
+00000790: 7574 3a20 696d 706f 7274 2072 6573 6574  ut: import reset
+000007a0: 0005 3720 2043 6f6e 6e65 6374 206f 7665  ..7  Connect ove
+000007b0: 7220 6874 7470 3a2f 2f6d 6963 726f 7079  r http://micropy
+000007c0: 7468 6f6e 2e6f 7267 2f77 6562 7265 706c  thon.org/webrepl
+000007d0: 2f23 7b7d 3a38 3236 362f 0005 1b20 2009  /#{}:8266/...  .
+000007e0: 5b21 5d20 7765 6272 6570 6c20 7061 7373  [!] webrepl pass
+000007f0: 776f 7264 3a20 7b7d 0005 2420 2052 6573  word: {}..$  Res
+00000800: 7461 7274 206e 6f64 6520 7468 656e 2073  tart node then s
+00000810: 7461 7274 2077 6562 7265 706c 2e2e 2e00  tart webrepl....
+00000820: 0520 5b45 5252 5d20 7768 696c 6520 7374  . [ERR] while st
+00000830: 6172 7469 6e67 2077 6562 7265 706c 3a20  arting webrepl: 
+00000840: 7b7d 0005 0f6d 6963 724f 5369 7354 6865  {}...micrOSisThe
+00000850: 4265 7374 0005 1f5b 7b7d 5d20 5348 4f57  Best...[{}] SHOW
+00000860: 204c 4d20 5041 5253 4552 2057 4152 4e49   LM PARSER WARNI
+00000870: 4e47 3a20 7b7d 0087 1410 1601 800d 2c2c  NG: {}........,,
+00000880: 322c 3272 6020 8010 022a 011b 031c 0216  2,2r` ...*......
+00000890: 0259 8010 042a 011b 051c 0416 0459 8010  .Y...*.......Y..
+000008a0: 0610 072a 021b 081c 0616 061c 0716 0759  ...*...........Y
+000008b0: 8010 092a 011b 0a1c 0916 0959 8010 0b10  ...*.......Y....
+000008c0: 0c2a 021b 0d1c 0b16 0b1c 0c16 0c59 8010  .*...........Y..
+000008d0: 0e10 0f2a 021b 101c 0e16 5e1c 0f16 0f59  ...*......^....Y
+000008e0: 5432 0010 1134 0216 1151 6301 8664 1030  T2...4...Qc..d.0
+000008f0: 1188 1a44 8413 6420 6440 8808 6460 840e  ...D..d d@..d`..
+00000900: 8409 846a 8825 8c21 115f 1660 1011 1661  ...j.%.!._.`...a
+00000910: 1012 161d 3200 1613 3201 161f 3202 160e  ....2...2...2...
+00000920: 502a 0153 3303 1620 3204 1624 3205 1626  P*.S3.. 2..$2..&
+00000930: 3206 162a 3207 162b 1162 3208 3401 163a  2..*2..+.b2.4..:
+00000940: 1162 502a 0153 3309 3401 1638 1162 502a  .bP*.S3.4..8.bP*
+00000950: 0153 330a 3401 1630 5163 0b86 78c1 021c  .S3.4..0Qc..x...
+00000960: 1358 801d 6040 2929 4924 4422 562c 1206  .X..`@))I$D"V,..
+00000970: 1014 3401 b018 1512 0610 1634 01b0 1817  ..4........4....
+00000980: 1206 1018 3401 b018 1950 b018 1a50 b018  ....4....P...P..
+00000990: 1b48 0d12 0710 1c12 1113 1d34 0259 4a2a  .H.........4.YJ*
+000009a0: 5712 63df 4463 c149 1912 0b23 0014 1eb1  W.c.Dc.I...#....
+000009b0: 3601 3401 5912 0c23 0114 1eb1 3601 3401  6.4.Y..#....6.4.
+000009c0: 5951 51c1 2801 5d4a 015d 5163 781a 0a1f  YQQ.(.]J.]Qcx...
+000009d0: 5864 8031 1265 b134 0159 5163 8110 110c  Xd.1.e.4.YQc....
+000009e0: 0e58 8034 2024 50b0 181a 50b0 181b 5163  .X.4 $P...P...Qc
+000009f0: 8348 b201 1420 5866 8039 2035 2823 25b0  .H... Xf.9 5(#%.
+00000a00: 141f 2302 141e b144 4410 2142 4210 2236  ..#....DD.!BB."6
+00000a10: 0136 0159 b014 1f10 2336 0159 b144 4512  .6.Y....#6.Y.DE.
+00000a20: 5e34 0059 120f 3400 5951 6383 1039 0e24  ^4.Y..4.YQc..9.$
+00000a30: 5880 4120 312c b013 1744 49b0 131a 4344  X.A 1,...DI...CD
+00000a40: 2303 4242 1022 c1b0 131b 4444 2304 4242  #.BB."....DD#.BB
+00000a50: 1022 c210 2514 1eb1 b2b0 1315 3603 6385  ."..%.......6.c.
+00000a60: 082a 1c26 5867 8047 404a 272b 2428 2628  .*.&Xg.G@J'+$(&(
+00000a70: 26b0 1317 4477 b013 1a43 7212 0610 2734  &...Dw...Cr...'4
+00000a80: 01c2 b2b1 8055 1428 3600 d944 5252 b018  .....U.(6..DRR..
+00000a90: 1ab0 141f 1029 3601 5952 2b00 2a02 63b0  .....)6.YR+.*.c.
+00000aa0: 141f 2305 3601 5950 2b00 2a02 6352 b12a  ..#.6.YP+.*.cR.*
+00000ab0: 0263 8178 3212 2a58 6480 5560 2027 2bb0  .c.x2.*Xd.U` '+.
+00000ac0: 142b b136 01c2 b014 1fb0 1424 3600 3601  .+.6.......$6.6.
+00000ad0: 59b2 63a4 00ea 0286 022b 5864 805e 800b  Y.c......+Xd.^..
+00000ae0: 5222 8a08 4832 422a 2322 2962 482e 6228  R"..H2B*#")bH.b(
+00000af0: 2251 2247 2b31 306d 2b24 222b 2462 2928  "Q"G+10m+$"+$b)(
+00000b00: 2828 2828 2828 2828 2828 2828 2828 2828  ((((((((((((((((
+00000b10: 282a 2d70 204e 4b60 4042 592d b151 de43  (*-p NK`@BY-.Q.C
+00000b20: 4d12 68b1 1428 3600 3401 80d9 4442 5263  M.h..(6.4...DBRc
+00000b30: b114 2836 0014 2c36 00c2 b280 5510 2dd9  ..(6..,6....U.-.
+00000b40: 4454 b014 1f23 0614 1eb0 1315 b013 1936  DT...#.........6
+00000b50: 0236 0159 5263 b014 26b2 3601 3002 c3c2  .6.YRc..&.6.0...
+00000b60: b343 4250 6312 68b2 3401 80d9 4442 5263  .CBPc.h.4...DBRc
+00000b70: b280 5510 1cd9 4450 b014 1f12 6912 1113  ..U...DP....i...
+00000b80: 1d34 0136 0159 5263 b280 5510 20d9 445c  .4.6.YRc..U. .D\
+00000b90: 50c4 1268 b234 0182 db44 4a10 2eb2 8155  P..h.4...DJ....U
+00000ba0: dd44 4252 c4b0 1420 b436 0159 b280 5514  .DBR... .6.Y..U.
+00000bb0: 2f10 3036 0144 6e12 68b2 3401 82d9 4458  /.06.Dn.h.4...DX
+00000bc0: 1031 b281 55dd 4450 1211 1430 1032 b013  .1..U.DP...0.2..
+00000bd0: 1f10 3352 3684 0059 1211 1430 1032 b013  ..3R6..Y...0.2..
+00000be0: 1f36 8200 59b2 8055 142f 1034 3601 4446  .6..Y..U./.46.DF
+00000bf0: 52b0 181b 5263 b280 5514 2f10 3536 0144  R...Rc..U./.56.D
+00000c00: 4650 b018 1b52 63b2 8055 1036 d944 b781  FP...Rc..U.6.D..
+00000c10: b014 1f23 0736 0159 b014 1f23 0836 0159  ...#.6.Y...#.6.Y
+00000c20: b014 1f23 0936 0159 b014 1f23 0a36 0159  ...#.6.Y...#.6.Y
+00000c30: b014 1f23 0b36 0159 b014 1f23 0c36 0159  ...#.6.Y...#.6.Y
+00000c40: b014 1f23 0d36 0159 b014 1f23 0e36 0159  ...#.6.Y...#.6.Y
+00000c50: b014 1f23 0f36 0159 b014 1f23 1036 0159  ...#.6.Y...#.6.Y
+00000c60: b014 1f23 1136 0159 b014 1f23 1236 0159  ...#.6.Y...#.6.Y
+00000c70: b014 1f23 1336 0159 b014 1f23 1436 0159  ...#.6.Y...#.6.Y
+00000c80: b014 1f23 1536 0159 b014 1f23 1636 0159  ...#.6.Y...#.6.Y
+00000c90: b014 1f23 1736 0159 b014 1f23 1836 0159  ...#.6.Y...#.6.Y
+00000ca0: 1037 1269 b234 01dd 444d 1211 1438 1032  .7.i.4..DM...8.2
+00000cb0: b013 1f36 8200 6312 1114 3810 32b0 131f  ...6..c...8.2...
+00000cc0: 1039 5236 8400 63b0 131b 4454 1268 b234  .9R6..c...DT.h.4
+00000cd0: 0180 d844 4b12 1114 3ab0 131f b236 0263  ...DK...:....6.c
+00000ce0: 4810 1209 103b b210 3cb0 131f 3484 0063  H....;..<...4..c
+00000cf0: 4a21 5712 63df 445a c549 10b0 141f 2319  J!W.c.DZ.I....#.
+00000d00: 141e b536 0136 0159 5063 5151 c528 055d  ...6.6.YPcQQ.(.]
+00000d10: 4a01 5d51 638d 0092 1230 3a32 6a80 c960  J.]Qc....0:2j..`
+00000d20: 602a 482f 2836 422b 424a 244d 2256 2b4b  `*H/(6B+BJ$M"V+K
+00000d30: 302c 1268 b134 0181 d944 c480 b180 5510  0,.h.4...D....U.
+00000d40: 3dd9 446f 1206 3400 143e 3600 5f4b 2230  =.Do..4..>6._K"0
+00000d50: 02c2 c38a 1268 b234 01f3 c4b0 231a 141e  .....h.4....#...
+00000d60: b210 3fb4 f410 3f87 f4b3 3604 3401 5942  ..?...?...6.4.YB
+00000d70: 1c52 63b0 1206 b180 5534 0134 0159 5263  .Rc.....U4.4.YRc
+00000d80: 1268 b134 0182 db44 db80 b180 55c2 103f  .h.4...D....U..?
+00000d90: 1440 b181 512e 0255 3601 c348 0d12 07b2  .@..Q..U6..H....
+00000da0: b310 4152 3482 02c5 4a1f 5712 63df 4458  ..AR4...J.W.c.DX
+00000db0: c649 0eb0 231b 141e b636 0134 0159 50c5  .I..#....6.4.YP.
+00000dc0: 5151 c628 065d 4a01 5d12 06b2 3401 51de  QQ.(.]J.]...4.Q.
+00000dd0: 4444 231c 4242 231d c7b0 b544 4410 4242  DD#.BB#....DD.BB
+00000de0: 41b7 3401 5952 6383 64b2 019a 0138 3239  A.4.YRc.d....829
+00000df0: 80ee 6020 8514 2328 2c45 0004 b020 0001  ..` ..#(,E... ..
+00000e00: c2b1 4459 1204 1443 3600 2704 b420 0101  ..DY...C6.'.. ..
+00000e10: 1202 3400 5e34 01c3 b2b3 3401 63b2 1202  ..4.^4....4.c...
+00000e20: 3400 3401 6302 8f4c a212 2c4c 6c6d 80f3  4.4.c..L..,Llm..
+00000e30: 2b32 232c 291f 2424 2a23 2326 3b1f 572d  +2#,).$$*##&;.W-
+00000e40: 2e32 00b1 5e34 015f 4bd4 01c2 b214 4d10  .2..^4._K.....M.
+00000e50: 4e10 2236 0214 2c10 4f36 0180 55c3 489a  N."6..,.O6..U.H.
+00000e60: 0125 0010 5014 1eb3 3601 3401 59b2 1451  .%..P...6.4.Y..Q
+00000e70: 1052 3601 4467 2500 1053 141e 103f 1268  .R6.Dg%..S...?.h
+00000e80: b214 4d10 4e10 2236 0214 2c10 4f36 0180  ..M.N."6..,.O6..
+00000e90: 5534 01f4 3601 3401 5940 ac7f 0112 6bb2  U4..6.4.Y@....k.
+00000ea0: 1054 3402 4751 c423 24c5 42c5 80b4 1455  .T4.GQ.#$.B....U
+00000eb0: 3600 c5b5 1428 3600 142f 1056 3601 4472  6....(6../.V6.Dr
+00000ec0: 1057 b5dd d344 6b10 58b5 ddd3 4464 2500  .W...Dk.X...Dd%.
+00000ed0: 1059 141e 103f 1268 b334 01f4 b514 4d10  .Y...?.h.4....M.
+00000ee0: 5a10 2236 0214 2c10 5b36 0180 5536 0234  Z."6..,.[6..U6.4
+00000ef0: 0159 b543 b77f 515c 5d4a 2157 1263 df44  .Y.C..Q\]J!W.c.D
+00000f00: 5ac6 4910 2500 2325 141e b2b6 3602 3401  Z.I.%.#%....6.4.
+00000f10: 5950 6351 51c6 2806 5d4a 015d 42a9 7e52  YPcQQ.(.]J.]B.~R
+00000f20: 6301 8238 c140 085c 6c80 f353 b053 534b  c..8.@.\l..S.SSK
+00000f30: 18c1 b114 2f10 4e36 0144 34b1 1451 105d  ..../.N6.D4..Q.]
+00000f40: 3601 442b b167 5942 2651 6382 20ca 400a  6.D+.gYB&Qc. .@.
+00000f50: 5c6c 6c90 0853 b153 534b 14c2 b214 2c10  \ll..S.SSK....,.
+00000f60: 4f36 0180 5525 00dd 442f b267 5942 2a51  O6..U%..D/.gYB*Q
+00000f70: 638c 00e2 032c 3032 3390 0f4b 2626 3130  c....,023..K&&10
+00000f80: 2326 2643 2b2b 2522 255d 2825 8010 442a  #&&C++%"%](%..D*
+00000f90: 011b 451c 44c2 59b0 231e 3401 59b0 231f  ..E.D.Y.#.4.Y.#.
+00000fa0: 3401 59b0 2320 141e b234 0081 5580 5536  4.Y.# ...4..U.U6
+00000fb0: 0134 0159 b023 2114 1e12 0610 2734 0136  .4.Y.#!.....'4.6
+00000fc0: 0134 0159 b144 46b0 2322 3401 59b0 1046  .4.Y.DF.#"4.Y..F
+00000fd0: 3401 59b1 445b 126b 1047 1048 3402 470a  4.Y.D[.k.G.H4.G.
+00000fe0: c3b3 1449 1030 3601 5951 5c5d 125e 3400  ...I.06.YQ\].^4.
+00000ff0: 5948 1980 511b 30c4 b0b4 144a 104b 1206  YH..Q.0....J.K..
+00001000: 1027 3401 3682 0034 0159 4a25 5712 63df  .'4.6..4.YJ%W.c.
+00001010: 445e c549 1423 2314 1eb5 3601 c6b0 b634  D^.I.##...6....4
+00001020: 0159 120c b634 0159 5151 c528 055d 4a01  .Y...4.YQQ.(.]J.
+00001030: 5d51 63                                  ]Qc
```

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/InterruptHandler.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/InterruptHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_VL53L0X.py` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_aht10.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_aht10.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_bme280.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_bme280.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_buzzer.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_buzzer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_catgame.py` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_cct.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_cct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_co2.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_co2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_demo.py` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_dht11.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_dht11.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_dht22.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_dht22.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_dimmer.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_dimmer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_distance.py` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_ds18.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_ds18.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_esp32.py` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_genIO.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_genIO.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_i2c.py` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_intercon.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_intercon.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_light_sensor.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_light_sensor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_lmpacman.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_lmpacman.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_neoeffects.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_neoeffects.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_neopixel.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_neopixel.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_oled.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_oled.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_oled_sh1106.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_oled_ui.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_oled_ui.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_pet_feeder.py` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_ph_sensor.py` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_presence.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_presence.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_rencoder.py` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_rgb.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_rgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_rgbcct.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_rgbcct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_roboarm.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_roboarm.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_robustness.py` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_servo.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_servo.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_stepper.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_stepper.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_switch.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_switch.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_system.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_system.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_telegram.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_telegram.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_tinyrgb.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_esp32.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LP_esp32.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_esp32s2.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LP_esp32s2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_esp32s3.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LP_esp32s3.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LogicalPins.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/LogicalPins.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Network.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Network.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Notify.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Notify.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Scheduler.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Scheduler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/SocketServer.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/SocketServer.mpy`

 * *Files 13% similar despite different names*

```diff
@@ -16,46 +16,46 @@
 000000f0: 6f6e 736f 6c65 0002 7c00 022d 000c 494e  onsole..|..-..IN
 00000100: 4445 4e54 0023 1263 6f6e 6e65 6374 6564  DENT.#.connected
 00000110: 000c 7265 6164 6572 000c 7772 6974 6572  ..reader..writer
 00000120: 000a 4576 656e 7400 1664 7261 696e 5f65  ..Event..drain_e
 00000130: 7665 6e74 0082 191c 6765 745f 6578 7472  vent....get_extr
 00000140: 615f 696e 666f 0010 7065 6572 6e61 6d65  a_info..peername
 00000150: 0012 636c 6965 6e74 5f69 6400 8129 0a7b  ..client_id..).{
-00000160: 7d3a 7b7d 0002 2e00 8151 8223 8215 0a73  }:{}.....Q.#...s
-00000170: 6865 6c6c 0014 6c61 7374 5f6d 7367 5f74  hell..last_msg_t
-00000180: 0081 7b0c 6465 636f 6465 0008 7574 6638  ..{.decode..utf8
-00000190: 0082 3108 6578 6974 0003 0c70 726f 6d70  ..1.exit...promp
-000001a0: 7400 067b 7d0a 0082 490c 656e 636f 6465  t..{}...I.encode
-000001b0: 0016 6472 6f70 5f63 6c69 656e 7400 1c67  ..drop_client..g
-000001c0: 6574 5f65 7665 6e74 5f6c 6f6f 7000 1663  et_event_loop..c
-000001d0: 7265 6174 655f 7461 736b 0020 5f5f 7761  reate_task. __wa
-000001e0: 6974 5f66 6f72 5f64 7261 696e 0008 7761  it_for_drain..wa
-000001f0: 6974 0081 0d0a 6472 6169 6e00 810f 0a42  it....drain....B
-00000200: 7965 210a 000a 7265 7365 7400 1073 6c65  ye!...reset..sle
-00000210: 6570 5f6d 7300 1677 6169 745f 636c 6f73  ep_ms..wait_clos
-00000220: 6564 0016 4143 5449 5645 5f43 4c49 5300  ed..ACTIVE_CLIS.
-00000230: 812d 8171 1e73 6572 7665 725f 7461 736b  .-.q.server_task
-00000240: 5f6d 7367 0002 2c00 8155 165f 5f73 6865  _msg..,..U.__she
-00000250: 6c6c 5f63 6d64 0014 4543 4f4e 4e52 4553  ll_cmd..ECONNRES
+00000160: 7d3a 7b7d 0002 2e00 8151 8223 146c 6173  }:{}.....Q.#.las
+00000170: 745f 6d73 675f 7400 817b 0c64 6563 6f64  t_msg_t..{.decod
+00000180: 6500 0875 7466 3800 8231 0865 7869 7400  e..utf8..1.exit.
+00000190: 0382 150c 7072 6f6d 7074 0006 7b7d 0a00  ....prompt..{}..
+000001a0: 8249 0c65 6e63 6f64 6500 1664 726f 705f  .I.encode..drop_
+000001b0: 636c 6965 6e74 001c 6765 745f 6576 656e  client..get_even
+000001c0: 745f 6c6f 6f70 0016 6372 6561 7465 5f74  t_loop..create_t
+000001d0: 6173 6b00 205f 5f77 6169 745f 666f 725f  ask. __wait_for_
+000001e0: 6472 6169 6e00 0877 6169 7400 810d 0a64  drain..wait....d
+000001f0: 7261 696e 0081 0f0a 4279 6521 0a00 0a72  rain....Bye!...r
+00000200: 6573 6574 0010 736c 6565 705f 6d73 0016  eset..sleep_ms..
+00000210: 7761 6974 5f63 6c6f 7365 6400 1641 4354  wait_closed..ACT
+00000220: 4956 455f 434c 4953 0081 2d81 711e 7365  IVE_CLIS..-.q.se
+00000230: 7276 6572 5f74 6173 6b5f 6d73 6700 022c  rver_task_msg..,
+00000240: 0081 5516 5f5f 7368 656c 6c5f 636d 6400  ..U.__shell_cmd.
+00000250: 0a73 6865 6c6c 0014 4543 4f4e 4e52 4553  .shell..ECONNRES
 00000260: 4554 0012 7275 6e5f 7368 656c 6c00 0c72  ET..run_shell..r
 00000270: 6562 6f6f 7400 0e5f 5f64 656c 5f5f 0031  eboot..__del__.1
 00000280: 145f 5f69 6e73 7461 6e63 6500 0c5f 5f68  .__instance..__h
 00000290: 6f73 7400 0c73 6572 7665 7200 185f 5f63  ost..server..__c
 000002a0: 6f6e 6e5f 7175 6575 6500 0e73 6f63 706f  onn_queue..socpo
 000002b0: 7274 000c 5f5f 706f 7274 000e 736f 6374  rt..__port..soct
 000002c0: 6f75 7400 1673 6f63 5f74 696d 656f 7574  out..soc_timeout
 000002d0: 001a 6163 6365 7074 5f63 6c69 656e 7400  ..accept_client.
 000002e0: 814d 1a68 616e 646c 655f 636c 6965 6e74  .M.handle_client
 000002f0: 0014 7275 6e5f 7365 7276 6572 0018 7374  ..run_server..st
 00000300: 6172 745f 7365 7276 6572 000e 6261 636b  art_server..back
 00000310: 6c6f 6700 0a72 6570 6c79 000e 6173 796e  log..reply..asyn
-00000320: 6369 6f00 2f2d 3582 2906 6d73 6700 8213  cio./-5.).msg...
-00000330: 822f 4910 7265 7370 6f6e 7365 0081 7781  ./I.response..w.
-00000340: 590e 7265 7175 6573 7400 0b06 636c 7300  Y.request...cls.
-00000350: 8235 813d 146e 6577 5f63 6c69 656e 7400  .5.=.new_client.
+00000320: 6369 6f00 2f2d 3582 2906 6d73 6700 0b82  cio./-5.).msg...
+00000330: 1382 2f82 3549 1072 6573 706f 6e73 6500  ../.5I.response.
+00000340: 8177 8159 0e72 6571 7565 7374 0006 636c  .w.Y.request..cl
+00000350: 7300 813d 146e 6577 5f63 6c69 656e 7400  s..=.new_client.
 00000360: 8157 051a 5b53 494d 554c 4154 4f52 204d  .W..[SIMULATOR M
 00000370: 4f44 4520 4743 2049 4d50 4f52 545d 0005  ODE GC IMPORT]..
 00000380: 155b 436c 6965 6e74 5d20 6e65 7720 636f  .[Client] new co
 00000390: 6e6e 3a20 7b7d 0005 105b 436c 6965 6e74  nn: {}...[Client
 000003a0: 5d20 7265 6164 207b 7d00 0523 5b43 6c69  ] read {}..#[Cli
 000003b0: 656e 745d 2053 7472 6561 6d20 7265 6164  ent] Stream read
 000003c0: 2065 7272 6f72 2028 7b7d 293a 207b 7d00   error ({}): {}.
@@ -101,136 +101,135 @@
 00000640: 5b20 736f 636b 6574 2073 6572 7665 7220  [ socket server 
 00000650: 5d20 5374 6172 7420 736f 636b 6574 2073  ] Start socket s
 00000660: 6572 7665 7220 6f6e 207b 7d3a 7b7d 0005  erver on {}:{}..
 00000670: 292d 2054 4350 2073 6572 7665 7220 7265  )- TCP server re
 00000680: 6164 792c 2063 6f6e 6e65 6374 3a20 7465  ady, connect: te
 00000690: 6c6e 6574 207b 7d20 7b7d 0005 205b 2073  lnet {} {}.. [ s
 000006a0: 6f63 6b65 7420 7365 7276 6572 205d 203c  ocket server ] <
-000006b0: 3c64 6573 7472 7563 746f 723e 3e00 8b74  <destructor>>..t
+000006b0: 3c64 6573 7472 7563 746f 723e 3e00 8c04  <destructor>>...
 000006c0: 2c24 0180 0c2c 322c 2c26 2c32 2255 2775  ,$...,2,,&,2"U'u
-000006d0: 890d 899e 8010 022a 011b 031c 0216 0259  .......*.......Y
+000006d0: 890d 8b9f 8010 022a 011b 031c 0216 0259  .......*.......Y
 000006e0: 8010 0410 052a 021b 061c 0416 041c 0516  .....*..........
 000006f0: 0559 8010 072a 011b 081c 0716 0759 8010  .Y...*.......Y..
 00000700: 092a 011b 0a1c 0916 0959 8051 1b0b 165e  .*.......Y.Q...^
 00000710: 8010 0c2a 011b 0d1c 0c16 0c59 8010 0e10  ...*.......Y....
 00000720: 0f2a 021b 101c 0e16 0e1c 0f16 0f59 4814  .*...........YH.
 00000730: 8010 1110 122a 021b 131c 1116 111c 1216  .....*..........
 00000740: 1259 4a1d 5911 0423 0034 0159 8010 1110  .YJ.Y..#.4.Y....
 00000750: 122a 021b 141c 1116 111c 1216 1259 4a01  .*...........YJ.
-00000760: 5d54 3200 1006 3402 1606 5432 0110 1534  ]T2...4...T2...4
-00000770: 0216 1554 3202 1016 3402 1616 5163 0381  ...T2...4...Qc..
-00000780: 5c08 0806 881b 4311 5f16 6010 0616 6180  \.....C._.`...a.
-00000790: 161a 1162 3200 3401 1617 5163 0183 0021  ...b2.4...Qc...!
-000007a0: 0a17 6380 1f31 1204 1018 1019 1206 131a  ..c..1..........
-000007b0: f4f2 b0f2 3401 5912 0657 131a 1206 131a  ....4.Y..W......
-000007c0: 2232 d744 4381 4241 80e5 5a18 1a51 6384  "2.DC.BA..Z..Qc.
-000007d0: 6408 2815 8828 4484 0e84 1884 1584 1584  d.(..(D.........
-000007e0: 1288 0784 1084 1911 5f16 6010 1516 612c  ........_.`...a,
-000007f0: 0016 4332 0016 1b32 0116 2d32 0216 2a32  ..C2...2..-2..*2
-00000800: 0316 3a32 0416 3e11 6232 0534 0116 3732  ..:2..>.b2.4..72
-00000810: 0616 4932 0716 4b32 0816 4d51 6309 8838  ..I2..K2..MQc..8
-00000820: 5322 1b64 1d1e 802b 2424 2429 482a 301f  S".d...+$$$)H*0.
-00000830: 2724 2a52 b018 1cb1 b018 1db2 b018 1e12  '$*R............
-00000840: 5e14 1f36 00b0 1820 b013 2014 2136 0059  ^..6... .. .!6.Y
-00000850: b214 2210 2336 01b0 1824 1206 1417 2301  ..".#6...$....#.
-00000860: 1425 b013 2436 0136 0159 1026 1425 1027  .%..$6.6.Y.&.%.'
-00000870: 1428 b013 2480 5514 2910 2736 017e 512e  .(..$.U.).'6.~Q.
-00000880: 0255 3601 1265 b013 2481 5534 0136 02c3  .U6..e..$.U4.6..
-00000890: b3b0 1824 1207 b013 2a34 01b0 182b 120e  ...$....*4...+..
-000008a0: 3400 b018 2c51 6389 58d9 4222 2d64 8039  4...,Qc.X.B"-d.9
-000008b0: 8007 3027 222e 5731 256c 312c 2512 0614  ..0'".W1%l1,%...
-000008c0: 1723 0214 25b0 1324 3601 3601 5912 0e34  .#..%..$6.6.Y..4
-000008d0: 00b0 182c 481c b013 1d14 2d22 9000 3601  ...,H.....-"..6.
-000008e0: 5e51 68c1 b114 2e10 2f36 0114 3036 00c1  ^Qh...../6..06..
-000008f0: 4a2b 5712 66df 4464 c249 1a12 0614 1723  J+W.f.Dd.I.....#
-00000900: 0314 25b0 1324 b236 0236 0159 1211 3400  ..%..$.6.6.Y..4.
-00000910: 5923 0463 5151 c228 025d 4a01 5d12 0614  Y#.cQQ.(.]J.]...
-00000920: 1723 0514 25b0 1324 b136 0236 0159 b110  .#..%..$.6.6.Y..
-00000930: 31d9 4346 b110 32d9 4445 52b1 2a02 6350  1.CF..2.DER.*.cP
-00000940: b12a 0263 8810 d202 1c2a 6467 8051 6026  .*.c.....*dg.Q`&
-00000950: 4b68 227a 2a58 52b0 131c 44e3 80b0 132b  Kh"z*XR...D....+
-00000960: 1433 3600 b1dc 4448 1034 1425 b136 01c1  .36...DH.4.%.6..
-00000970: 4811 b013 1e14 35b1 1436 102f 3601 3601  H.....5..6./6.6.
-00000980: 594a 2b57 1266 df44 64c2 491a 1215 1437  YJ+W.f.Dd.I....7
-00000990: b013 2436 0159 1205 2306 1425 b013 24b2  ..$6.Y..#..%..$.
-000009a0: 3602 3401 5951 51c2 2802 5d4a 015d 125e  6.4.YQQ.(.]J.].^
-000009b0: 1438 3600 1439 b014 3a36 0036 0159 4246  .86..9..:6.6.YBF
-000009c0: 1268 b134 0159 5163 8620 c942 183a 6480  .h.4.YQc. .B.:d.
-000009d0: 6660 406b 2862 762e 52b0 1320 143b 3600  f`@k(bv.R.. .;6.
-000009e0: 5e51 6859 b013 2014 3c36 0059 480d b013  ^QhY.. .<6.YH...
-000009f0: 1e14 3d36 005e 5168 594a 2957 1266 df44  ..=6.^QhYJ)W.f.D
-00000a00: 62c1 4918 1206 1417 2307 1425 b136 0136  b.I.....#..%.6.6
-00000a10: 0159 b014 3e36 005e 5168 5951 51c1 2801  .Y..>6.^QhYQQ.(.
-00000a20: 5d4a 015d b013 2014 2136 0059 5163 8910  ]J.].. .!6.YQc..
-00000a30: d142 1e3e 6480 7b30 4828 2c22 2856 3a24  .B.>d.{0H(,"(V:$
-00000a40: 454a 1206 1417 2308 1425 b013 2436 0136  EJ....#..%..$6.6
-00000a50: 0159 b014 2a10 3f36 0159 b013 2b14 4036  .Y..*.?6.Y..+.@6
-00000a60: 0059 125e 1441 2232 3601 5e51 6859 4815  .Y.^.A"26.^QhYH.
-00000a70: b013 1e14 3e36 0059 b013 1e14 4236 005e  ....>6.Y....B6.^
-00000a80: 5168 594a 2357 1266 df44 5cc1 4912 1206  QhYJ#W.f.D\.I...
-00000a90: 1417 2309 1425 b013 24b1 3602 3601 5951  ..#..%..$.6.6.YQ
-00000aa0: 51c1 2801 5d4a 015d 50b0 181c 8012 0618  Q.(.]J.]P.......
-00000ab0: 1a12 1514 37b0 1324 3601 5912 1134 0059  ....7..$6.Y..4.Y
-00000ac0: 5163 8370 390c 3724 808e 2f4a 1215 1343  Qc.p9.7$../J...C
-00000ad0: 1444 b051 3602 51de d344 4a12 1513 4314  .D.Q6.Q..DJ...C.
-00000ae0: 45b0 3601 5912 0c34 0014 4610 4714 2812  E.6.Y..4..F.G.(.
-00000af0: 6912 1513 4314 4836 0034 0136 0136 0159  i...C.H6.4.6.6.Y
-00000b00: 5163 8730 da42 2049 646a 8095 2229 2923  Qc.0.B Idj.."))#
-00000b10: 4d26 292e 2b25 3048 1912 0614 1723 0a36  M&).+%0H.....#.6
-00000b20: 0159 b013 2b14 2bb1 3601 c2b2 4442 5263  .Y..+.+.6...DBRc
-00000b30: 4a31 5712 66df 446a c349 2010 4ab3 dd44  J1W.f.Dj.I .J..D
-00000b40: 49b0 143e 3600 5e51 6859 1206 1417 230b  I..>6.^QhY....#.
-00000b50: 1425 b336 0136 0159 5063 5151 c328 035d  .%.6.6.YPcQQ.(.]
-00000b60: 4a01 5d12 1134 0059 b014 2a23 0c14 2512  J.]..4.Y..*#..%.
-00000b70: 1234 0036 0136 0159 5263 8a68 d142 244b  .4.6.6.YRc.h.B$K
-00000b80: 6480 a57b 4d23 422c 2344 2a23 2827 532c  d..{M#B,#D*#('S,
-00000b90: 5212 0c34 0014 4610 4714 2812 6912 1513  R..4..F.G.(.i...
-00000ba0: 4314 4836 0034 0136 0136 0159 b014 2ab0  C.H6.4.6.6.Y..*.
-00000bb0: 132b 1433 3600 3601 5942 dc80 4839 b014  .+.36.6.YB..H9..
-00000bc0: 2d36 005e 5168 3002 c1c2 b144 4440 ce80  -6.^Qh0....DD@..
-00000bd0: 01b0 1449 b236 015e 5168 c1b1 4357 b014  ...I.6.^Qh..CW..
-00000be0: 2a23 0d36 0159 1205 230e 3401 59b0 132b  *#.6.Y..#.4.Y..+
-00000bf0: 144c 3600 594a 2157 1266 df44 5ac3 4910  .L6.YJ!W.f.DZ.I.
-00000c00: 1205 230f 1425 b336 0134 0159 4050 0251  ..#..%.6.4.Y@P.Q
-00000c10: 51c3 2803 5d4a 015d b013 1c43 9e7f b014  Q.(.]J.]...C....
-00000c20: 3e36 005e 5168 5951 6381 7029 0a4d 6480  >6.^QhYQc.p).Md.
-00000c30: bd25 1211 3400 5912 0614 1723 1014 25b0  .%..4.Y....#..%.
-00000c40: 1324 3601 3601 5951 6383 7410 2116 88c6  .$6.6.YQc.t.!...
-00000c50: 8007 4386 1b84 2884 1384 0a88 0a00 115f  ..C...(........_
-00000c60: 1660 1016 1661 5116 4fb0 2000 0116 4e32  .`...aQ.O. ...N2
-00000c70: 0116 5732 0216 5932 0316 5a11 6232 0434  ..W2..Y2..Z.b2.4
-00000c80: 0116 5d32 0516 4db0 6306 8718 2a20 4e6b  ..]2..M.c...* Nk
-00000c90: 6c80 d060 4049 4e28 2767 4c2b 4f29 1216  l..`@IN('gL+O)..
-00000ca0: 134f 51de 44d3 8012 6d25 00b1 154e b136  .OQ.D...m%...N.6
-00000cb0: 0112 1618 4f10 3212 1613 4f18 5051 1216  ....O.2...O.PQ..
-00000cc0: 134f 1851 8212 1613 4f18 5212 0210 5334  .O.Q....O.R...S4
-00000cd0: 0112 1613 4f18 5412 6e12 0210 5534 0134  ....O.T.n...U4.4
-00000ce0: 01c2 b285 d744 4385 4241 b212 1613 4f18  .....DC.BA....O.
-00000cf0: 5612 0614 1723 1136 0159 1216 134f 638d  V....#.6.Y...Oc.
-00000d00: 6092 5036 576c 6f80 eb80 0764 5627 652e  `.P6Wlo....dV'e.
-00000d10: 222f 3334 4c29 2922 6923 4549 2829 22b1  "/34L))"i#EI()".
-00000d20: 1324 c212 7012 6912 1513 4314 4836 0034  .$..p.i...C.H6.4
-00000d30: 0134 01b0 1352 d744 4cb1 1215 1343 b256  .4...R.DL....C.V
-00000d40: 52b2 2a02 6312 0614 1723 1214 25b2 3601  R.*.c....#..%.6.
-00000d50: 3601 5950 c312 1513 4314 5836 005f 4b54  6.YP....C.X6._KT
-00000d60: 3002 c4c5 126e 120f 120e 3400 b513 2c34  0....n....4...,4
-00000d70: 0223 13f4 3401 c612 0614 1723 1414 25b2  .#..4......#..%.
-00000d80: b4b0 1356 b6f3 3603 3601 59b5 131c 4447  ...V..6.6.Y...DG
-00000d90: b6b0 1356 d844 5a12 0614 1723 1536 0159  ...V.DZ....#.6.Y
-00000da0: b514 3e36 005e 5168 5952 c359 5959 5942  ..>6.^QhYR.YYYYB
-00000db0: 4342 aa7f b344 4552 b22a 0263 1206 1417  CB...DER.*.c....
-00000dc0: 2316 3601 59b1 142a 2317 3601 59b1 143e  #.6.Y..*#.6.Y..>
-00000dd0: 3600 5e51 6859 2801 50b2 2a02 6383 18c3  6.^QhY(.P.*.c...
-00000de0: 4018 596c 1d1e 9013 6060 672d 6362 1215  @.Yl....``g-cb..
-00000df0: b1b2 3402 c3b0 1457 b336 015e 5168 3002  ..4....W.6.^Qh0.
-00000e00: c4c5 b443 4251 63b3 144b 3600 5e51 6859  ...CBQc..K6.^QhY
-00000e10: 5163 8540 c140 125a 6c90 2660 2931 3827  Qc.@.@.Zl.&`)18'
-00000e20: 1209 3400 8155 8055 c112 0614 1723 1814  ..4..U.U.....#..
-00000e30: 25b1 b013 5436 0236 0159 125e 145b b013  %...T6.6.Y.^.[..
-00000e40: 59b0 1350 b013 5410 5cb0 1352 3682 03b0  Y..P..T.\..R6...
-00000e50: 1851 b013 515e 5168 5912 0614 1723 1914  .Q..Q^QhY....#..
-00000e60: 25b1 b013 5436 0236 0159 5163 8248 4910  %...T6.6.YQc.HI.
-00000e70: 5d63 9031 6020 2f25 1215 1343 1458 3600  ]c.1` /%...C.X6.
-00000e80: 5f4b 1230 02c1 c2b2 131c 4447 b214 2ab0  _K.0......DG..*.
-00000e90: 3601 5942 2c51 6381 5019 0a4d 6c90 3a29  6.YB,Qc.P..Ml.:)
-00000ea0: 1206 1417 231a 3601 59b0 1351 143e 3600  ....#.6.Y..Q.>6.
-00000eb0: 5951 63                                  YQc
+00000760: 5d54 3200 1006 3402 1606 5432 0110 1511  ]T2...4...T2....
+00000770: 0734 0316 1554 3202 1016 3402 1616 5163  .4...T2...4...Qc
+00000780: 0381 5c08 0806 881b 4311 5f16 6010 0616  ..\.....C._.`...
+00000790: 6180 161a 1162 3200 3401 1617 5163 0183  a....b2.4...Qc..
+000007a0: 0021 0a17 6380 1f31 1204 1018 1019 1206  .!..c..1........
+000007b0: 131a f4f2 b0f2 3401 5912 0657 131a 1206  ......4.Y..W....
+000007c0: 131a 2232 d744 4381 4241 80e5 5a18 1a51  .."2.DC.BA..Z..Q
+000007d0: 6384 7c10 2915 8828 4486 0f84 1884 1584  c.|.)..(D.......
+000007e0: 1584 1288 0784 1084 1900 115f 1660 1015  ..........._.`..
+000007f0: 1661 2c00 1642 b020 0001 161b 3201 162b  .a,..B. ....2..+
+00000800: 3202 1631 3203 1639 3204 163d 1162 3205  2..12..92..=.b2.
+00000810: 3401 1636 3206 1648 3207 164b 3208 164d  4..62..H2..K2..M
+00000820: b063 0988 48d8 0424 1b64 651d 1e80 2b24  .c..H..$.de...+$
+00000830: 2424 2948 2a30 1f27 442a 52b1 181c b2b1  $$)H*0.'D*R.....
+00000840: 181d b3b1 181e 125e 141f 3600 b118 20b1  .......^..6... .
+00000850: 1320 1421 3600 59b3 1422 1023 3601 b118  . .!6.Y..".#6...
+00000860: 2412 0614 1723 0114 25b1 1324 3601 3601  $....#..%..$6.6.
+00000870: 5910 2614 2510 2714 28b1 1324 8055 1429  Y.&.%.'.(..$.U.)
+00000880: 1027 3601 7e51 2e02 5536 0112 66b1 1324  .'6.~Q..U6..f..$
+00000890: 8155 3401 3602 c4b4 b118 2412 6725 00b1  .U4.6.....$.g%..
+000008a0: 151b 3600 5912 0e34 00b1 182a 5163 8958  ..6.Y..4...*Qc.X
+000008b0: d942 222b 6580 3a80 0730 2722 2e57 3125  .B"+e.:..0'".W1%
+000008c0: 6c31 2c25 1206 1417 2302 1425 b013 2436  l1,%....#..%..$6
+000008d0: 0136 0159 120e 3400 b018 2a48 1cb0 131d  .6.Y..4...*H....
+000008e0: 142b 2290 0036 015e 5168 c1b1 142c 102d  .+"..6.^Qh...,.-
+000008f0: 3601 142e 3600 c14a 2b57 1268 df44 64c2  6...6..J+W.h.Dd.
+00000900: 491a 1206 1417 2303 1425 b013 24b2 3602  I.....#..%..$.6.
+00000910: 3601 5912 1134 0059 2304 6351 51c2 2802  6.Y..4.Y#.cQQ.(.
+00000920: 5d4a 015d 1206 1417 2305 1425 b013 24b1  ]J.]....#..%..$.
+00000930: 3602 3601 59b1 102f d943 46b1 1030 d944  6.6.Y../.CF..0.D
+00000940: 4552 b12a 0263 50b1 2a02 6388 00d2 021c  ER.*.cP.*.c.....
+00000950: 3165 6980 5260 2649 6822 7a2a 5852 b013  1ei.R`&Ih"z*XR..
+00000960: 1c44 e180 b014 3236 00b1 dc44 4810 3314  .D....26...DH.3.
+00000970: 25b1 3601 c148 11b0 131e 1434 b114 3510  %.6..H.....4..5.
+00000980: 2d36 0136 0159 4a2b 5712 68df 4464 c249  -6.6.YJ+W.h.Dd.I
+00000990: 1a12 1514 36b0 1324 3601 5912 0523 0614  ....6..$6.Y..#..
+000009a0: 25b0 1324 b236 0234 0159 5151 c228 025d  %..$.6.4.YQQ.(.]
+000009b0: 4a01 5d12 5e14 3736 0014 38b0 1439 3600  J.].^.76..8..96.
+000009c0: 3601 5942 4612 6ab1 3401 5951 6386 20c9  6.YBF.j.4.YQc. .
+000009d0: 4218 3965 8067 6040 6b28 6276 2e52 b013  B.9e.g`@k(bv.R..
+000009e0: 2014 3a36 005e 5168 59b0 1320 143b 3600   .:6.^QhY.. .;6.
+000009f0: 5948 0db0 131e 143c 3600 5e51 6859 4a29  YH.....<6.^QhYJ)
+00000a00: 5712 68df 4462 c149 1812 0614 1723 0714  W.h.Db.I.....#..
+00000a10: 25b1 3601 3601 59b0 143d 3600 5e51 6859  %.6.6.Y..=6.^QhY
+00000a20: 5151 c128 015d 4a01 5db0 1320 1421 3600  QQ.(.]J.].. .!6.
+00000a30: 5951 6389 00d1 421e 3d65 807c 3048 262c  YQc...B.=e.|0H&,
+00000a40: 2228 563a 2445 4a12 0614 1723 0814 25b0  "(V:$EJ....#..%.
+00000a50: 1324 3601 3601 59b0 1431 103e 3601 59b0  .$6.6.Y..1.>6.Y.
+00000a60: 143f 3600 5912 5e14 4022 3236 015e 5168  .?6.Y.^.@"26.^Qh
+00000a70: 5948 15b0 131e 143d 3600 59b0 131e 1441  YH.....=6.Y....A
+00000a80: 3600 5e51 6859 4a23 5712 68df 445c c149  6.^QhYJ#W.h.D\.I
+00000a90: 1212 0614 1723 0914 25b0 1324 b136 0236  .....#..%..$.6.6
+00000aa0: 0159 5151 c128 015d 4a01 5d50 b018 1c80  .YQQ.(.]J.]P....
+00000ab0: 1206 181a 1215 1436 b013 2436 0159 1211  .......6..$6.Y..
+00000ac0: 3400 5951 6383 7039 0c36 2480 8f2f 4a12  4.YQc.p9.6$../J.
+00000ad0: 1513 4214 43b0 5136 0251 ded3 444a 1215  ..B.C.Q6.Q..DJ..
+00000ae0: 1342 1444 b036 0159 120c 3400 1445 1046  .B.D.6.Y..4..E.F
+00000af0: 1428 126b 1215 1342 1447 3600 3401 3601  .(.k...B.G6.4.6.
+00000b00: 3601 5951 6387 20da 4220 4865 6c80 9622  6.YQc. .B Hel.."
+00000b10: 2927 234d 2629 2e2b 2530 4817 1206 1417  )'#M&).+%0H.....
+00000b20: 230a 3601 59b0 1449 b136 01c2 b244 4252  #.6.Y..I.6...DBR
+00000b30: 634a 3157 1268 df44 6ac3 4920 104a b3dd  cJ1W.h.Dj.I .J..
+00000b40: 4449 b014 3d36 005e 5168 5912 0614 1723  DI..=6.^QhY....#
+00000b50: 0b14 25b3 3601 3601 5950 6351 51c3 2803  ..%.6.6.YPcQQ.(.
+00000b60: 5d4a 015d 1211 3400 59b0 1431 230c 1425  ]J.]..4.Y..1#..%
+00000b70: 1212 3400 3601 3601 5952 638a 48d1 4224  ..4.6.6.YRc.H.B$
+00000b80: 4b65 80a6 7b4b 2342 2c23 442a 2328 2751  Ke..{K#B,#D*#('Q
+00000b90: 2c52 120c 3400 1445 1046 1428 126b 1215  ,R..4..E.F.(.k..
+00000ba0: 1342 1447 3600 3401 3601 3601 59b0 1431  .B.G6.4.6.6.Y..1
+00000bb0: b014 3236 0036 0159 42da 8048 37b0 142b  ..26.6.YB..H7..+
+00000bc0: 3600 5e51 6830 02c1 c2b1 4444 40cc 8001  6.^Qh0....DD@...
+00000bd0: b014 48b2 3601 5e51 68c1 b143 55b0 1431  ..H.6.^Qh..CU..1
+00000be0: 230d 3601 5912 0523 0e34 0159 b014 4c36  #.6.Y..#.4.Y..L6
+00000bf0: 0059 4a21 5712 68df 445a c349 1012 0523  .YJ!W.h.DZ.I...#
+00000c00: 0f14 25b3 3601 3401 5940 5002 5151 c328  ..%.6.4.Y@P.QQ.(
+00000c10: 035d 4a01 5db0 131c 43a0 7fb0 143d 3600  .]J.]...C....=6.
+00000c20: 5e51 6859 5163 8170 290a 4d65 80be 2512  ^QhYQc.p).Me..%.
+00000c30: 1134 0059 1206 1417 2310 1425 b013 2436  .4.Y....#..%..$6
+00000c40: 0136 0159 5163 8374 1021 1688 c780 0743  .6.YQc.t.!.....C
+00000c50: 861b 8428 8413 840a 880a 0011 5f16 6010  ...(........_.`.
+00000c60: 1616 6151 164f b020 0001 164e 3201 1657  ..aQ.O. ...N2..W
+00000c70: 3202 1659 3203 165a 1162 3204 3401 165d  2..Y2..Z.b2.4..]
+00000c80: 3205 164d b063 0687 182a 204e 646d 80d1  2..M.c...* Ndm..
+00000c90: 6040 494e 2827 674c 2b4f 2912 1613 4f51  `@IN('gL+O)...OQ
+00000ca0: de44 d380 1267 2500 b115 4eb1 3601 1216  .D...g%...N.6...
+00000cb0: 184f 1030 1216 134f 1850 5112 1613 4f18  .O.0...O.PQ...O.
+00000cc0: 5182 1216 134f 1852 1202 1053 3401 1216  Q....O.R...S4...
+00000cd0: 134f 1854 126e 1202 1055 3401 3401 c2b2  .O.T.n...U4.4...
+00000ce0: 85d7 4443 8542 41b2 1216 134f 1856 1206  ..DC.BA....O.V..
+00000cf0: 1417 2311 3601 5912 1613 4f63 8d60 9250  ..#.6.Y...Oc.`.P
+00000d00: 3657 6d6f 80ec 8007 6456 2765 2e22 2f33  6Wmo....dV'e."/3
+00000d10: 344c 2929 2269 2345 4928 2922 b113 24c2  4L))"i#EI()"..$.
+00000d20: 1270 126b 1215 1342 1447 3600 3401 3401  .p.k...B.G6.4.4.
+00000d30: b013 52d7 444c b112 1513 42b2 5652 b22a  ..R.DL....B.VR.*
+00000d40: 0263 1206 1417 2312 1425 b236 0136 0159  .c....#..%.6.6.Y
+00000d50: 50c3 1215 1342 1458 3600 5f4b 5430 02c4  P....B.X6._KT0..
+00000d60: c512 6e12 0f12 0e34 00b5 132a 3402 2313  ..n....4...*4.#.
+00000d70: f434 01c6 1206 1417 2314 1425 b2b4 b013  .4......#..%....
+00000d80: 56b6 f336 0336 0159 b513 1c44 47b6 b013  V..6.6.Y...DG...
+00000d90: 56d8 445a 1206 1417 2315 3601 59b5 143d  V.DZ....#.6.Y..=
+00000da0: 3600 5e51 6859 52c3 5959 5959 4243 42aa  6.^QhYR.YYYYBCB.
+00000db0: 7fb3 4445 52b2 2a02 6312 0614 1723 1636  ..DER.*.c....#.6
+00000dc0: 0159 b114 3123 1736 0159 b114 3d36 005e  .Y..1#.6.Y..=6.^
+00000dd0: 5168 5928 0150 b22a 0263 8318 c340 1859  QhY(.P.*.c...@.Y
+00000de0: 6d1d 1e90 1460 6067 2d63 6212 15b1 b234  m....``g-cb....4
+00000df0: 02c3 b014 57b3 3601 5e51 6830 02c4 c5b4  ....W.6.^Qh0....
+00000e00: 4342 5163 b314 4b36 005e 5168 5951 6385  CBQc..K6.^QhYQc.
+00000e10: 40c1 4012 5a6d 9027 6029 3138 2712 0934  @.@.Zm.'`)18'..4
+00000e20: 0081 5580 55c1 1206 1417 2318 1425 b1b0  ..U.U.....#..%..
+00000e30: 1354 3602 3601 5912 5e14 5bb0 1359 b013  .T6.6.Y.^.[..Y..
+00000e40: 50b0 1354 105c b013 5236 8203 b018 51b0  P..T.\..R6....Q.
+00000e50: 1351 5e51 6859 1206 1417 2319 1425 b1b0  .Q^QhY....#..%..
+00000e60: 1354 3602 3601 5951 6382 4849 105d 6390  .T6.6.YQc.HI.]c.
+00000e70: 3260 202f 2512 1513 4214 5836 005f 4b12  2` /%...B.X6._K.
+00000e80: 3002 c1c2 b213 1c44 47b2 1431 b036 0159  0......DG..1.6.Y
+00000e90: 422c 5163 8150 190a 4d6d 903b 2912 0614  B,Qc.P..Mm.;)...
+00000ea0: 1723 1a36 0159 b013 5114 3d36 0059 5163  .#.6.Y..Q.=6.YQc
```

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/TaskManager.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/TaskManager.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Time.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/Time.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/micrOS.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/micrOS.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/micrOSloader.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/micrOSloader.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/urequests.mpy` & `micrOSDevToolKit-1.22.0/toolkit/workspace/precompiled/urequests.mpy`

 * *Files identical despite different names*

