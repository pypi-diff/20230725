# Comparing `tmp/SoloPy-3.1.1.tar.gz` & `tmp/SoloPy-v1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SoloPy-3.1.1.tar", last modified: Tue Jul 25 14:50:23 2023, max compression
+gzip compressed data, was "SoloPy-v1.0.tar", last modified: Sun Aug 22 16:21:13 2021, max compression
```

## Comparing `SoloPy-3.1.1.tar` & `SoloPy-v1.0.tar`

### file list

```diff
@@ -1,90 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:50:23.704943 SoloPy-3.1.1/
--rw-rw-rw-   0        0        0     1573 2022-02-02 20:44:49.000000 SoloPy-3.1.1/.gitignore
--rw-rw-rw-   0        0        0    35804 2022-02-02 20:44:49.000000 SoloPy-3.1.1/COPYING
--rw-rw-rw-   0        0        0    34614 2022-02-02 20:44:49.000000 SoloPy-3.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      318 2023-01-05 13:22:08.000000 SoloPy-3.1.1/MANIFEST
--rw-rw-rw-   0        0        0       76 2023-01-05 13:18:08.000000 SoloPy-3.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      984 2023-07-25 14:50:23.705894 SoloPy-3.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3885 2023-02-08 09:34:00.000000 SoloPy-3.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-25 14:50:23.615438 SoloPy-3.1.1/SoloPy/
--rw-rw-rw-   0        0        0     3207 2023-05-12 16:41:00.000000 SoloPy-3.1.1/SoloPy/ConstantCanopen.py
--rw-rw-rw-   0        0        0      572 2023-05-12 15:40:09.000000 SoloPy-3.1.1/SoloPy/ConstantCommon.py
--rw-rw-rw-   0        0        0     5001 2023-05-12 16:43:24.000000 SoloPy-3.1.1/SoloPy/ConstantUart.py
--rw-rw-rw-   0        0        0    12031 2023-07-25 14:21:29.000000 SoloPy-3.1.1/SoloPy/SOLOMotorControllers.py
--rw-rw-rw-   0        0        0   106810 2023-07-25 14:23:38.000000 SoloPy-3.1.1/SoloPy/SOLOMotorControllersCanopen.py
--rw-rw-rw-   0        0        0    92926 2023-07-24 11:35:30.000000 SoloPy-3.1.1/SoloPy/SOLOMotorControllersUart.py
--rw-rw-rw-   0        0        0    16610 2023-07-25 14:24:17.000000 SoloPy-3.1.1/SoloPy/SOLOMotorControllersUtils.py
--rw-rw-rw-   0        0        0       85 2023-05-12 16:43:55.000000 SoloPy-3.1.1/SoloPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:50:23.627284 SoloPy-3.1.1/SoloPy.egg-info/
--rw-rw-rw-   0        0        0      984 2023-07-25 14:50:23.000000 SoloPy-3.1.1/SoloPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3483 2023-07-25 14:50:23.000000 SoloPy-3.1.1/SoloPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:50:23.000000 SoloPy-3.1.1/SoloPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-25 14:50:23.000000 SoloPy-3.1.1/SoloPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-25 14:50:23.000000 SoloPy-3.1.1/SoloPy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 14:50:23.554549 SoloPy-3.1.1/examples/
-drwxrwxrwx   0        0        0        0 2023-07-25 14:50:23.552554 SoloPy-3.1.1/examples/raspberry_pi/
-drwxrwxrwx   0        0        0        0 2023-07-25 14:50:23.645090 SoloPy-3.1.1/examples/raspberry_pi/canopen/
--rw-rw-rw-   0        0        0     3550 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/BLDC_Drone_RC_Car_Sensorless.py
--rw-rw-rw-   0        0        0     4191 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/BLDC_Position_Control_HALL_based.py
--rw-rw-rw-   0        0        0     3808 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/BLDC_Speed_Control_HALL_based.py
--rw-rw-rw-   0        0        0     3611 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/BLDC_Torque_Control_HALL_based.py
--rw-rw-rw-   0        0        0     4552 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/PMSM_Position_Control_Encoder_based.py
--rw-rw-rw-   0        0        0     3630 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/PMSM_Speed_Control_Encoder_based.py
--rw-rw-rw-   0        0        0     3972 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/PMSM_Torque_Control_Encoder_based.py
--rw-rw-rw-   0        0        0     2161 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/multiple_writeAndRead.py
--rw-rw-rw-   0        0        0     1003 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/reading_busVoltage.py
--rw-rw-rw-   0        0        0     1008 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/reading_temperature.py
--rw-rw-rw-   0        0        0     3680 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/sensorless_brushless_speed_control.py
--rw-rw-rw-   0        0        0     3040 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/toggle_commandMode.py
--rw-rw-rw-   0        0        0     1144 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/canopen/writing_reading_numberOfPoles.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:50:23.662010 SoloPy-3.1.1/examples/raspberry_pi/uart/
--rw-rw-rw-   0        0        0     3458 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/BLDC_Drone_RC_Car_Sensorless.py
--rw-rw-rw-   0        0        0     4099 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/BLDC_Position_Control_HALL_based.py
--rw-rw-rw-   0        0        0     3716 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/BLDC_Speed_Control_HALL_based.py
--rw-rw-rw-   0        0        0     3519 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/BLDC_Torque_Control_HALL_based.py
--rw-rw-rw-   0        0        0     4460 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/PMSM_Position_Control_Encoder_based.py
--rw-rw-rw-   0        0        0     3538 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/PMSM_Speed_Control_Encoder_based.py
--rw-rw-rw-   0        0        0     3880 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/PMSM_Torque_Control_Encoder_based.py
--rw-rw-rw-   0        0        0     2069 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/multiple_writeAndRead.py
--rw-rw-rw-   0        0        0      911 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/reading_busVoltage.py
--rw-rw-rw-   0        0        0      916 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/reading_temperature.py
--rw-rw-rw-   0        0        0     3588 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/sensorless_brushless_speed_control.py
--rw-rw-rw-   0        0        0     2948 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/toggle_commandMode.py
--rw-rw-rw-   0        0        0     1052 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/raspberry_pi/uart/writing_reading_numberOfPoles.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:50:23.553552 SoloPy-3.1.1/examples/ubuntu/
-drwxrwxrwx   0        0        0        0 2023-07-25 14:50:23.679962 SoloPy-3.1.1/examples/ubuntu/usb/
--rw-rw-rw-   0        0        0     3599 2023-02-08 09:43:17.000000 SoloPy-3.1.1/examples/ubuntu/usb/BLDC_Drone_RC_Car_Sensorless.py
--rw-rw-rw-   0        0        0     4240 2023-02-08 09:43:20.000000 SoloPy-3.1.1/examples/ubuntu/usb/BLDC_Position_Control_HALL_based.py
--rw-rw-rw-   0        0        0     3857 2023-02-08 09:43:23.000000 SoloPy-3.1.1/examples/ubuntu/usb/BLDC_Speed_Control_HALL_based.py
--rw-rw-rw-   0        0        0     3660 2023-02-08 09:43:27.000000 SoloPy-3.1.1/examples/ubuntu/usb/BLDC_Torque_Control_HALL_based.py
--rw-rw-rw-   0        0        0     4601 2023-02-08 09:43:35.000000 SoloPy-3.1.1/examples/ubuntu/usb/PMSM_Position_Control_Encoder_based.py
--rw-rw-rw-   0        0        0     3679 2023-02-08 09:43:38.000000 SoloPy-3.1.1/examples/ubuntu/usb/PMSM_Speed_Control_Encoder_based.py
--rw-rw-rw-   0        0        0     4021 2023-02-08 09:43:41.000000 SoloPy-3.1.1/examples/ubuntu/usb/PMSM_Torque_Control_Encoder_based.py
--rw-rw-rw-   0        0        0     2210 2023-02-08 09:43:32.000000 SoloPy-3.1.1/examples/ubuntu/usb/multiple_writeAndRead.py
--rw-rw-rw-   0        0        0     1052 2023-02-08 09:43:44.000000 SoloPy-3.1.1/examples/ubuntu/usb/reading_busVoltage.py
--rw-rw-rw-   0        0        0     1057 2023-02-08 09:43:46.000000 SoloPy-3.1.1/examples/ubuntu/usb/reading_temperature.py
--rw-rw-rw-   0        0        0     3729 2023-02-08 09:43:49.000000 SoloPy-3.1.1/examples/ubuntu/usb/sensorless_brushless_speed_control.py
--rw-rw-rw-   0        0        0     3089 2023-02-08 09:43:54.000000 SoloPy-3.1.1/examples/ubuntu/usb/toggle_commandMode.py
--rw-rw-rw-   0        0        0     1193 2023-02-08 09:43:57.000000 SoloPy-3.1.1/examples/ubuntu/usb/writing_reading_numberOfPoles.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:50:23.554549 SoloPy-3.1.1/examples/windows/
-drwxrwxrwx   0        0        0        0 2023-07-25 14:50:23.696917 SoloPy-3.1.1/examples/windows/usb/
--rw-rw-rw-   0        0        0     3452 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/windows/usb/BLDC_Drone_RC_Car_Sensorless.py
--rw-rw-rw-   0        0        0     4093 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/windows/usb/BLDC_Position_Control_HALL_based.py
--rw-rw-rw-   0        0        0     3710 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/windows/usb/BLDC_Speed_Control_HALL_based.py
--rw-rw-rw-   0        0        0     3513 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/windows/usb/BLDC_Torque_Control_HALL_based.py
--rw-rw-rw-   0        0        0     4454 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/windows/usb/PMSM_Position_Control_Encoder_based.py
--rw-rw-rw-   0        0        0     3532 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/windows/usb/PMSM_Speed_Control_Encoder_based.py
--rw-rw-rw-   0        0        0     3874 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/windows/usb/PMSM_Torque_Control_Encoder_based.py
--rw-rw-rw-   0        0        0     2063 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/windows/usb/multiple_writeAndRead.py
--rw-rw-rw-   0        0        0      905 2023-07-21 10:25:32.000000 SoloPy-3.1.1/examples/windows/usb/reading_busVoltage.py
--rw-rw-rw-   0        0        0      910 2023-07-21 10:25:32.000000 SoloPy-3.1.1/examples/windows/usb/reading_temperature.py
--rw-rw-rw-   0        0        0     3582 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/windows/usb/sensorless_brushless_speed_control.py
--rw-rw-rw-   0        0        0     2942 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/windows/usb/toggle_commandMode.py
--rw-rw-rw-   0        0        0     1046 2023-02-08 09:42:51.000000 SoloPy-3.1.1/examples/windows/usb/writing_reading_numberOfPoles.py
--rw-rw-rw-   0        0        0      116 2023-07-24 09:32:00.000000 SoloPy-3.1.1/requirements.txt
--rw-rw-rw-   0        0        0       87 2023-07-25 14:50:23.718859 SoloPy-3.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1227 2023-07-24 09:32:04.000000 SoloPy-3.1.1/setup.py
--rw-rw-rw-   0        0        0      730 2023-07-21 10:25:32.000000 SoloPy-3.1.1/test.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:50:23.701903 SoloPy-3.1.1/tests/
--rw-rw-rw-   0        0        0     7355 2023-05-13 16:43:51.000000 SoloPy-3.1.1/tests/test_SOLOMotorControllersCanopen.py
--rw-rw-rw-   0        0        0     7209 2023-07-24 09:25:16.000000 SoloPy-3.1.1/tests/test_SOLOMotorControllersUart.py
+drwxrwxrwx   0        0        0        0 2021-08-22 16:21:13.985564 SoloPy-v1.0/
+-rw-rw-rw-   0        0        0      972 2021-08-22 16:21:13.985564 SoloPy-v1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2518 2021-08-22 16:03:47.071998 SoloPy-v1.0/README.rst
+drwxrwxrwx   0        0        0        0 2021-08-22 16:21:13.985221 SoloPy-v1.0/SoloPy/
+-rw-rw-rw-   0        0        0       87 2021-08-22 16:03:47.072330 SoloPy-v1.0/SoloPy/__init__.py
+-rw-rw-rw-   0        0        0     3594 2021-08-22 16:03:47.073406 SoloPy-v1.0/SoloPy/constant.py
+-rw-rw-rw-   0        0        0    29850 2021-08-22 16:03:47.075222 SoloPy-v1.0/SoloPy/solo_motor_controller.py
+-rw-rw-rw-   0        0        0       41 2021-08-22 16:03:47.086342 SoloPy-v1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1837 2021-08-22 16:21:08.230116 SoloPy-v1.0/setup.py
```

### Comparing `SoloPy-3.1.1/PKG-INFO` & `SoloPy-v1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: SoloPy
-Version: 3.1.1
+Version: v1.0
 Summary: PYTHON Library for Control Solo Motor
 Home-page: https://github.com/Solo-FL/SoloPy
-Download-URL: https://github.com/Solo-FL/SoloPy/archive/refs/tags/v3.1.1.tar.gz
 Author: Solo
 Author-email: support@solomotorcontrollers.com
 License: gpl-3.0
+Download-URL: https://github.com/Solo-FL/SoloPy/archive/refs/tags/v1.0.tar.gz
+Description: UNKNOWN
 Keywords: Solo Motor controllers,Solo,SoloPy
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-License-File: LICENSE.txt
-License-File: COPYING
```

### Comparing `SoloPy-3.1.1/README.rst` & `SoloPy-v1.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,146 +1,65 @@
 |License|
 
 ==================================================
 SoloPy
 ==================================================
 
-SoloPy is a Python library published by SOLO Motor Controllers to control, command
-or read all the parameters that are stored or existing in the command set of SOLO devices.
-More information about SoloPy on `the SOLO website <https://www.solomotorcontrollers.com/>`_.
-For List of All the Available Methods Read the `DataSheet <https://www.solomotorcontrollers.com/resources/specs-datasheets/>`__
-
-SoloPy allows SOLO devices to be used in this conditions: 
-
-- USB Communication with Windows OS or Linux
-
-- UART protocol with RASPBERRY PI or any similar controller
-
-- CanOpen protocol with RASPBERRY PI or any similar controller
-
-
-Installation
-=============
-Please make sure you have installed **Python 3** and **pip**
+SoloPy is a library of SOLO Motor Controllers write in PYTHON compatible also with RASPBERRY PI.
+It can be used with UART line of RASPBERRY PI or any similar controller to control, command
+or read all the parameters that are stored or existing in command set of SOLO.
+More information about it on `the SOLO website <https://www.solomotorcontrollers.com/>`_.
 
-Install Solopy From Pip
-
-.. code-block::
-
-   $ pip install solopy
-
-
-Update
+How To Use
 =============
-If you have installed the library and you want to update it on Linux, RASPBERRY PI or Windows
+Please make sure you have installed Dependencies
 
+To download the full library with examples
 .. code-block::
 
-   $ pip install --upgrade SoloPy 
-   
-
-
-USB Communication with Windows OS or Linux Note
-==========================
-1. Connect Solo to Raspberry Pi or Pc
-
-2. Open terminal in linux(cmd in windows) and enter the following command
-
-.. code-block::
+   $ git clone https://github.com/Solo-FL/SoloPy.git SoloMotorControllers
 
-   $ python -m serial.tools.list_ports -v
 
-3. this will show you the port name that SOLO is connected to (in linux it's sth like '/dev/ttyAMC0' and in windows it's sth like 'COM8'
+For List of All the Available Methods Read the `DataSheet <https://www.solomotorcontrollers.com/resources/specs-datasheets/>`__
 
 
-UART protocol with RASPBERRY PI Note
+Configuring UART on Raspberry Pi
 =============
-In order to enable UART Protocol on Raspberry Pi you need to follow this one time process. 
-
-1. In Raspberry Pi, enter following command in Terminal to enable UART
 
+In Raspberry Pi, enter following command in Terminal window to enable UART::
 .. code-block::
 
    $ sudo raspi-config
 
-2. Select -> Interfacing Options
-
-3. After selecting Interfacing option, select Serial option to enable UART
-
-4. Then it will ask for the login shell to be accessible over Serial, select No shown as follows.
-
-5. At the end, it will ask for enabling Hardware Serial port, select Yes,
-
-6. Finally, our UART is enabled for Serial Communication on RX and TX pins of Raspberry Pi 3.
-
-7. Then, reboot the Raspberry Pi.
-
-
-CanOpen protocol with RASPBERRY PI Note
-=============
-In order to enable CanOpen Protocol on Raspberry Pi you need to follow this process one time
-
-1. turn SPI on in raspberry pi: 
-
-.. code-block::
-
-   $ sudo raspi-config   
-
-then go to interfaces 
-
-then go to SPI and turn on 
-
-then go to reboot
-
-2. type in terminal
-
-.. code-block::
-
-   $ sudo apt-get update
-
-3. then type this command:
-
-.. code-block::
-
-   $ sudo nano /boot/config.txt
-
-4- scroll down and add these lines:
-
-.. code-block::
-
-   dtoverlay=mcp2515-can0,oscillator=16000000,interrupt=25
-
-5- then reboot RASPBERRY PI
-
-
-**Every time** you reboot RASPBERRY PI you need to follow this process
-
-1- type this command 
-
-.. code-block::
-
-   $ sudo ip link set can0 up type can bitrate 1000000
-
-**Notes** 
-
-- The bit-rate has to be the same as the one used in the code
-
-- The following CAN transceiver module  `"PiCAN2" <https://copperhilltech.com/pican-2-can-bus-interface-for-raspberry-pi/>`__ has been used to test the library 
+#. Select -> Interfacing Options
+#. After selecting Interfacing option, select Serial option to enable UART
+#. Then it will ask for login shell to be accessible over Serial, select No shown as follows.
+#. At the end, it will ask for enabling Hardware Serial port, select Yes,
+#. Finally, our UART is enabled for Serial Communication on RX and TX pin of Raspberry Pi 3.
+#. Then, reboot the Raspberry Pi.
 
+Communication within USB
+==========================
+#. Connect Solo to Raspberry Pi or Pc
+#. Open terminal in linux(cmd in windows) & enter the following command
+#. python -m serial.tools.list_ports -v
+#. get the port name that solo is connected to (in linux it's sth like '/dev/ttyAMC0' and in windows it's sth like 'COM8'
 
 Dependencies
 =============
 `Python 3 <https://www.python.org/downloads/>`__
+`pyserial <https://github.com/pyserial/pyserial>`__
 
-`python-interface <https://github.com/ssanderson/python-interface>`__
-
-for UART `pyserial <https://github.com/pyserial/pyserial>`__
-
-for CanOpen `Python-Can <https://pypi.org/project/python-can/>`__
+Testing Examples
+=============
+To test the examples in Raspberry Pi you might need to put the example files within the "src" folder to be able to compile them
+The installation of "pyserial" is mandatory, to install that
+.. code-block::
 
+   $ sudo apt-get install python-serial
 
 Authors
 =============
 
 SoloPy is created by SOLO Motor Controllers team
```

