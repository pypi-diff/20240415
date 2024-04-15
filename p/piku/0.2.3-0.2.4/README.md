# Comparing `tmp/piku-0.2.3.tar.gz` & `tmp/piku-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piku-0.2.3.tar", max compression
+gzip compressed data, was "piku-0.2.4.tar", max compression
```

## Comparing `piku-0.2.3.tar` & `piku-0.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1065 2022-04-24 03:12:02.559100 piku-0.2.3/LICENSE
--rw-r--r--   0        0        0    11805 2023-02-06 03:16:21.108167 piku-0.2.3/README.md
--rw-r--r--   0        0        0       22 2022-01-28 21:23:02.244141 piku-0.2.3/piku/__init__.py
--rw-r--r--   0        0        0      311 2022-03-24 02:11:21.681040 piku-0.2.3/piku/commands/__init__.py
--rw-r--r--   0        0        0     2217 2022-03-24 02:11:21.681040 piku-0.2.3/piku/commands/add.py
--rw-r--r--   0        0        0     2689 2022-03-24 02:11:29.428245 piku-0.2.3/piku/commands/create.py
--rw-r--r--   0        0        0     1725 2022-04-24 03:12:43.456750 piku-0.2.3/piku/commands/deploy.py
--rw-r--r--   0        0        0      610 2022-03-24 02:11:21.685040 piku-0.2.3/piku/commands/info.py
--rw-r--r--   0        0        0      761 2022-03-24 02:11:21.685040 piku-0.2.3/piku/commands/install.py
--rw-r--r--   0        0        0     1164 2022-03-24 02:11:21.685040 piku-0.2.3/piku/commands/remove.py
--rw-r--r--   0        0        0     1938 2022-03-17 19:48:11.961823 piku-0.2.3/piku/commands/serial.py
--rw-r--r--   0        0        0      725 2022-03-24 02:11:21.685040 piku-0.2.3/piku/commands/upgrade.py
--rw-r--r--   0        0        0      229 2022-02-13 07:35:58.832280 piku-0.2.3/piku/commands/version.py
--rw-r--r--   0        0        0     2469 2022-03-24 02:11:21.685040 piku-0.2.3/piku/core/config.py
--rw-r--r--   0        0        0     2546 2022-04-02 04:47:05.765308 piku-0.2.3/piku/core/device.py
--rw-r--r--   0        0        0      207 2022-03-24 02:11:21.685040 piku-0.2.3/piku/core/errors.py
--rw-r--r--   0        0        0     3464 2022-03-24 02:11:21.685040 piku-0.2.3/piku/core/locker.py
--rw-r--r--   0        0        0     3710 2022-03-24 02:11:21.685040 piku-0.2.3/piku/core/packages.py
--rw-r--r--   0        0        0       96 2022-04-24 03:12:43.456750 piku-0.2.3/piku/core/utils/__init__.py
--rw-r--r--   0        0        0      330 2022-03-24 02:11:21.685040 piku-0.2.3/piku/core/utils/cache.py
--rw-r--r--   0        0        0     1973 2022-04-24 03:12:43.456750 piku-0.2.3/piku/core/utils/sync.py
--rw-r--r--   0        0        0     3257 2022-03-24 02:11:21.689040 piku-0.2.3/piku/core/utils/utils.py
--rw-r--r--   0        0        0      931 2022-04-24 03:12:43.456750 piku-0.2.3/piku/core/utils/watcher.py
--rw-r--r--   0        0        0     3302 2022-04-24 03:12:43.456750 piku-0.2.3/piku/main.py
--rw-r--r--   0        0        0     1957 2022-02-04 04:27:06.684134 piku-0.2.3/piku/template/.gitignore
--rw-r--r--   0        0        0       14 2022-02-02 23:44:08.492690 piku-0.2.3/piku/template/README.md
--rw-r--r--   0        0        0        0 2022-02-02 23:41:14.755383 piku-0.2.3/piku/template/project/code.py
--rw-r--r--   0        0        0      165 2022-03-24 02:11:21.689040 piku-0.2.3/piku/template/pyproject.toml
--rw-r--r--   0        0        0      893 2023-02-06 03:17:42.066693 piku-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    13157 1970-01-01 00:00:00.000000 piku-0.2.3/setup.py
--rw-r--r--   0        0        0    12784 1970-01-01 00:00:00.000000 piku-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-04-24 03:12:02.559100 piku-0.2.4/LICENSE
+-rw-r--r--   0        0        0    11805 2023-02-06 03:16:21.108167 piku-0.2.4/README.md
+-rw-r--r--   0        0        0       22 2022-01-28 21:23:02.244141 piku-0.2.4/piku/__init__.py
+-rw-r--r--   0        0        0      311 2022-03-24 02:11:21.681040 piku-0.2.4/piku/commands/__init__.py
+-rw-r--r--   0        0        0     2217 2022-03-24 02:11:21.681040 piku-0.2.4/piku/commands/add.py
+-rw-r--r--   0        0        0     2689 2022-03-24 02:11:29.428245 piku-0.2.4/piku/commands/create.py
+-rw-r--r--   0        0        0     1726 2024-04-15 08:42:54.912404 piku-0.2.4/piku/commands/deploy.py
+-rw-r--r--   0        0        0      610 2022-03-24 02:11:21.685040 piku-0.2.4/piku/commands/info.py
+-rw-r--r--   0        0        0      761 2022-03-24 02:11:21.685040 piku-0.2.4/piku/commands/install.py
+-rw-r--r--   0        0        0     1164 2022-03-24 02:11:21.685040 piku-0.2.4/piku/commands/remove.py
+-rw-r--r--   0        0        0     1938 2022-03-17 19:48:11.961823 piku-0.2.4/piku/commands/serial.py
+-rw-r--r--   0        0        0      725 2022-03-24 02:11:21.685040 piku-0.2.4/piku/commands/upgrade.py
+-rw-r--r--   0        0        0      229 2022-02-13 07:35:58.832280 piku-0.2.4/piku/commands/version.py
+-rw-r--r--   0        0        0     2469 2022-03-24 02:11:21.685040 piku-0.2.4/piku/core/config.py
+-rw-r--r--   0        0        0     2547 2024-04-15 08:42:54.912404 piku-0.2.4/piku/core/device.py
+-rw-r--r--   0        0        0      207 2022-03-24 02:11:21.685040 piku-0.2.4/piku/core/errors.py
+-rw-r--r--   0        0        0     3464 2022-03-24 02:11:21.685040 piku-0.2.4/piku/core/locker.py
+-rw-r--r--   0        0        0     3710 2022-03-24 02:11:21.685040 piku-0.2.4/piku/core/packages.py
+-rw-r--r--   0        0        0       96 2022-04-24 03:12:43.456750 piku-0.2.4/piku/core/utils/__init__.py
+-rw-r--r--   0        0        0      330 2022-03-24 02:11:21.685040 piku-0.2.4/piku/core/utils/cache.py
+-rw-r--r--   0        0        0     1973 2022-04-24 03:12:43.456750 piku-0.2.4/piku/core/utils/sync.py
+-rw-r--r--   0        0        0     3257 2022-03-24 02:11:21.689040 piku-0.2.4/piku/core/utils/utils.py
+-rw-r--r--   0        0        0      931 2022-04-24 03:12:43.456750 piku-0.2.4/piku/core/utils/watcher.py
+-rw-r--r--   0        0        0     3302 2022-04-24 03:12:43.456750 piku-0.2.4/piku/main.py
+-rw-r--r--   0        0        0     1957 2022-02-04 04:27:06.684134 piku-0.2.4/piku/template/.gitignore
+-rw-r--r--   0        0        0       14 2022-02-02 23:44:08.492690 piku-0.2.4/piku/template/README.md
+-rw-r--r--   0        0        0        0 2022-02-02 23:41:14.755383 piku-0.2.4/piku/template/project/code.py
+-rw-r--r--   0        0        0      165 2022-03-24 02:11:21.689040 piku-0.2.4/piku/template/pyproject.toml
+-rw-r--r--   0        0        0      893 2024-04-15 08:43:21.158999 piku-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    13157 1970-01-01 00:00:00.000000 piku-0.2.4/setup.py
+-rw-r--r--   0        0        0    12784 1970-01-01 00:00:00.000000 piku-0.2.4/PKG-INFO
```

### Comparing `piku-0.2.3/LICENSE` & `piku-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/README.md` & `piku-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/commands/add.py` & `piku-0.2.4/piku/commands/add.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/commands/create.py` & `piku-0.2.4/piku/commands/create.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/commands/deploy.py` & `piku-0.2.4/piku/commands/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # check that we have a device found or specified
     if not drive:
         print('Unable find a device and deploy, please specify a device to deploy to.')
         return
 
     # check that device size and name are as expected to reduce chances of loading onto wrong device
     if not device.has_correct_size(drive):
-        print('Refusing to deploy, specified CircuitPython drive is larger than expected (~2MB).')
+        print('Refusing to deploy, specified CircuitPython drive is larger than expected (~16MB).')
         return
     if not device.has_correct_label(drive):
         print('Refusing to deploy, expected device to have "circuitpy" in path.')
         return
 
     # confirm deploy
     if not args.yes:
```

### Comparing `piku-0.2.3/piku/commands/info.py` & `piku-0.2.4/piku/commands/info.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/commands/install.py` & `piku-0.2.4/piku/commands/install.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/commands/remove.py` & `piku-0.2.4/piku/commands/remove.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/commands/serial.py` & `piku-0.2.4/piku/commands/serial.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/commands/upgrade.py` & `piku-0.2.4/piku/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/core/config.py` & `piku-0.2.4/piku/core/config.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/core/device.py` & `piku-0.2.4/piku/core/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 def deploy(device):
     source = config.get('tool.piku.source')
     utils.sync(source, device, exclude=['boot_out.txt', '.*'], verbosity=1)
 
 def has_correct_size(path):
     total, used, free = shutil.disk_usage(path)
-    return 0 < total < 3E6
+    return 0 < total < 16E6
 
 def has_correct_label(path):
     if platform.system() == 'Windows':
         drive = path.split(':')[0]
         output = check_output(f'cmd /c vol {drive}:'.split()).decode()
         label = output.split('\r\n')[0].split(' ').pop()
         return 'circuitpy' in label.lower()
```

### Comparing `piku-0.2.3/piku/core/locker.py` & `piku-0.2.4/piku/core/locker.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/core/packages.py` & `piku-0.2.4/piku/core/packages.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/core/utils/sync.py` & `piku-0.2.4/piku/core/utils/sync.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/core/utils/utils.py` & `piku-0.2.4/piku/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/core/utils/watcher.py` & `piku-0.2.4/piku/core/utils/watcher.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/main.py` & `piku-0.2.4/piku/main.py`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/piku/template/.gitignore` & `piku-0.2.4/piku/template/.gitignore`

 * *Files identical despite different names*

### Comparing `piku-0.2.3/pyproject.toml` & `piku-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "piku"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = [
   "Mark Raleson <markraleson@outlook.com>",
   "Tammy Cravit <tammy@tammymakesthings.com>"
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `piku-0.2.3/setup.py` & `piku-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'watchdog>=2.1.7,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['piku = piku.main:main']}
 
 setup_kwargs = {
     'name': 'piku',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': '',
     'long_description': '# Piku\nPiku is small command line utility for managing CircuitPython projects\n\nThe purpose of this project is to make creating a CircuitPython project, installing packages, deploying, and connecting to a CircuitPython device easy to do from the command line.\n\n### Warning\nThis tool is in early development please be careful when deploying and confirm before deploying that you are only deploying your CircuitPython device, not another drive or device.\n\n\n---\n\n\n# Quick Start\n\n### Installation\nPiku is a command line tool that can be installed on Windows, macOS, and Linux using pip3 or pipx.\n\n```\npipx install piku\n```\n\n### Usage\nAfter piku is installed you can now create, deploy, add packages, and upgrade CircuitPython projects.  You can also use piku to connect to and debug your devices.\n\n```\nusage: piku [-h] {create,add,remove,install,upgrade,serial,deploy,version,info} ...\n    create              create new CircuitPython project\n    add                 download and add package to project\n    remove              remove package from project\n    install             install project dependencies\n    upgrade             upgrade all project dependencies to latest\n    serial              connect usb serial port of device\n    deploy              deploy project to device\n    version             show piku version\n    info                show additional piku information\n\n```\n\n\n---\n\n\n# Documentation\n\n\n### Installation\nPiku can be installed on Windows, macOS, or Linux.  This documentation is a work in progress, is you find issues please feel free to update them and make a pull request. To install Piku please ensure that you have at least **Python 3.8** and **pipx** or **pip3** installed, then run.  Installing via **pipx** is preferred when there are\ndependency conflicts with other tools on your system.\n\n```\npipx install piku\n```\n\nOr alternatively:\n\n```\npython3 -m pip install --user piku\n```\n\nAfter Piku is installed you should be able to run Piku from the command line.  You can test this by executing:\n\n```\npiku version\n```\n\n##### Additional Steps for Linux\n\nSome linux computers do not have the default pip user bin directory included in the PATH.  If installing via pip you may add this directory to your PATH or install without the `--user` argument.\n\nhttps://unix.stackexchange.com/questions/612779/warning-not-on-path-when-i-tried-to-install-python-extensions-im-new-to-linu\n\nAfter installation if your user does not have permissions to use the serial port, you may need to add your user to the `dialout` group.\nhttps://askubuntu.com/questions/58119/changing-permissions-on-serial-port#answer-58122\n\n### Preparing your Device\n\nBefore creating a project you must have CircuitPython installed on your device, and have your device serial and USB drivers installed.  Please check the CircuitPython website for instructions or the documentation of the board you have purchased.  When your done you should be able to see your drive mounted as a USB drive named `CIRCUITPY`.\n\nhttps://learn.adafruit.com/welcome-to-circuitpython/installing-circuitpython\n\n\n### Creating a Project\n\nTo create a new Piku project from the command line type:\n\n```\npiku create example\n```\n\nThis will create a new directory with the name of your project and a few folders and files inside. After you have created a project to use Piku, enter the directory of the project you just created to use Piku:\n\n```\ncd example\n```\n\n\n### Deploying your Project\nAfter you have created a project and modified the main `code.py` file you can deploy your project to a connected CircuitPython device.  To deploy your project find the path of your `CIRCUITPY` UDB drive.  Then type:\n\n```\npiku deploy -d <path of your device>\n```\n\n***WARNING!!***  \nDeploying will remove other files from your device.  Piku attempts to check that the device is actually a CircuitPython device, and backup your old files, but you still need to be very careful.\n\nYou can also let Piku find your device by running deploy with no device argument:\n\n```\npiku deploy\n```\n\nAfter you have confirmed multiple times that you are deploying to the correct device you can also live on the wild side and skip the confirmation dialog using the `-y` command line argument.  Please be careful.\n\nIf changes have been made in your project code, the CircuitPython device should automatically detect and change files and reload.\n\n\n### Connecting to your Device\n\nYou can also connect to your CircuitPython device\'s serial port using Piku.  To do this just use the serial command from your Piku project directory:\n\n```\npiku serial\n```\n\nIf you are unable to connect, please confirm that you have the serial drivers for your device installed and you have permission to use the serial port (see installation instructions).  If you know the serial port, or Piku is connecting to the wront port you can also try specifying it directly via the `-s` command line flag.\n\nOnce connected you can exit by typing `ctrl-x`, enter the CircuitPython REPL by hitting `ctrl-c` and `ctrl-d` to exit the CircuitPython REPL.\n\n\n### Adding CircuitPython Packages/Libraries\n\nYou can easily download and add CircuitPython packages from the official Bundle or Community bundle using the command.  For example to download and add the `neopixel` package you would type:\n\n```\npiku add neopixel\n```\n\nThe specified package and its dependencies will be downloaded and added to your `lib` folder and your `pyproject.toml` file. You can also remove this package by typing:\n\n```\npiku remove neopixel\n```\n\nYou can also install specific versions of packages by specifying in a similar way to other package manages:\n\n```\npiku add neopixel@~6\n```\n\nor\n\n```\npiku add neopixel@~6.1.2\n```\n\nYou can also specify the target CircuitPython version (6 or 7) in your pyproject.toml file.  One word of warning: package dependencies are often not broadly specified and may clash if you are not installing the latest versions of packages.\n\n### Upgrading Packages\n\nYou can upgrade all packages by running the upgrade command.\n```\npiku upgrade\n```\n\nYou can also upgrade a single package by adding the latest version.\n```\npiku add neopixel\n```\n\n### A Complete Example with Adafruit Feather Sense\n\n##### Creating the Example Project\nAssuming you have successfully installed Piku, here is a complete example on how to create and deploy a Piku project to the [Adafruit Feather Sense](https://www.adafruit.com/product/4516) board using a Linux computer.\n\nFirst setup the board to user CircuitPython following the instructions found here:  \nhttps://learn.adafruit.com/adafruit-feather-sense/circuitpython-on-feather-sense\n\nAfter your board is setup and mounts as a `CIRCUITPY` USB drive create a new Piku project and enter the project directory.\n```\npiku create example\ncd example\n```\n\n##### Adding Main Example Program\nAfter you have created a project you will need to edit `project/code.py` which is the main file for your project (this is a CircuitPython convention). Open `project/code.py` and paste the following [Demo Code from AdaFruit](https://learn.adafruit.com/adafruit-feather-sense/circuitpython-sense-demo).\n\n```py\n# SPDX-FileCopyrightText: 2020 Kattni Rembor for Adafruit Industries\n#\n# SPDX-License-Identifier: MIT\n#\n"""Sensor demo for Adafruit Feather Sense. Prints data from each of the sensors."""\nimport time\nimport array\nimport math\nimport board\nimport audiobusio\nimport adafruit_apds9960.apds9960\nimport adafruit_bmp280\nimport adafruit_lis3mdl\nimport adafruit_lsm6ds.lsm6ds33\nimport adafruit_sht31d\n\ni2c = board.I2C()\n\napds9960 = adafruit_apds9960.apds9960.APDS9960(i2c)\nbmp280 = adafruit_bmp280.Adafruit_BMP280_I2C(i2c)\nlis3mdl = adafruit_lis3mdl.LIS3MDL(i2c)\nlsm6ds33 = adafruit_lsm6ds.lsm6ds33.LSM6DS33(i2c)\nsht31d = adafruit_sht31d.SHT31D(i2c)\nmicrophone = audiobusio.PDMIn(board.MICROPHONE_CLOCK, board.MICROPHONE_DATA,\n                              sample_rate=16000, bit_depth=16)\n\ndef normalized_rms(values):\n    minbuf = int(sum(values) / len(values))\n    return int(math.sqrt(sum(float(sample - minbuf) *\n                             (sample - minbuf) for sample in values) / len(values)))\n\napds9960.enable_proximity = True\napds9960.enable_color = True\n\n# Set this to sea level pressure in hectoPascals at your location for accurate altitude reading.\nbmp280.sea_level_pressure = 1013.25\n\nwhile True:\n    samples = array.array(\'H\', [0] * 160)\n    microphone.record(samples, len(samples))\n\n    print("\\nFeather Sense Sensor Demo")\n    print("---------------------------------------------")\n    print("Proximity:", apds9960.proximity)\n    print("Red: {}, Green: {}, Blue: {}, Clear: {}".format(*apds9960.color_data))\n    print("Temperature: {:.1f} C".format(bmp280.temperature))\n    print("Barometric pressure:", bmp280.pressure)\n    print("Altitude: {:.1f} m".format(bmp280.altitude))\n    print("Magnetic: {:.3f} {:.3f} {:.3f} uTesla".format(*lis3mdl.magnetic))\n    print("Acceleration: {:.2f} {:.2f} {:.2f} m/s^2".format(*lsm6ds33.acceleration))\n    print("Gyro: {:.2f} {:.2f} {:.2f} dps".format(*lsm6ds33.gyro))\n    print("Humidity: {:.1f} %".format(sht31d.relative_humidity))\n    print("Sound level:", normalized_rms(samples))\n    time.sleep(0.3)\n```\n\n##### Installing Packages\nNext install the required libraries for the AdaFruit Feather Sense example:\n```\npiku add adafruit_apds9960\npiku add adafruit_bmp280\npiku add adafruit_lis3mdl\npiku add adafruit_lsm6ds\npiku add adafruit_sht31d\npiku add neopixel\n```\n\nThese packages should now found to your project `lib` folder, and your `pyproject.toml` file.  Confirm this by listing the files in your `lib` directory using `ls project/lib`. The ls command should return something the following if all packages were installed properly:\n```\nadafruit_apds9960\nadafruit_bus_device\nadafruit_lsm6ds\nadafruit_register\nneopixel.mpy\nadafruit_bmp280.mpy\nadafruit_lis3mdl.mpy\nadafruit_pixelbuf.mpy\nadafruit_sht31d.mpy\n```\n\nYour pyproject.toml file should now look something like this:\n```\n[tool.piku]\nproject = "example"\npiku = "0.1.8"\ncircuit-python = "7"\n\n[tool.piku.dependencies]\nneopixel = "latest"\nadafruit_bmp280 = "latest"\nadafruit_apds9960 = "latest"\nadafruit_lis3mdl = "latest"\nadafruit_lsm6ds = "latest"\nadafruit_sht31d = "latest"\n```\n\n##### Deploying to the Device\nNow make sure your device is mounted as a USB drive and find the device\'s mount point.  This should be something like `/media/username/CIRCUITPY/` or a drive letter on windows. ***Make note of this!***\n\nAfter your device is connected and mounted, you can deploy your code using the deploy command:\n```\npiku deploy -d <your device path here>\n```\n\nNext before deploying confirm that the device selected is the correct device. When Piku deploys it first attempts to validate its a CircuitPython device and then tries to backup the contents of the device in a temporary location. After validation and backup it loads your files onto the device and removes almost all other files\n\nYou can also forego the `-d <your device path here>` argument and let Piku attempt to find your device, but please confirm that you are deploying to the correct device so you don\'t lost any data.\n\n##### Connecting to the Serial Port\nAfter your code is deployed you can connect to the serial port to see your code in action. It make take a minute for the device to reload. To connect to the serial port run:\n\n```\npiku serial\n```\n\nPiku will attempt to connect to the first available serial port and reach your device, if you have more than one serial port you may need to specify which port via the command like arguments.  Hit `ctrl-x` to exit or `ctrl-c`/`ctrl-d` to enter/exit the CircuitPython REPL.\n\nThanks it! Happy hacking!\n\n\n# Contributing\n\nContributions are very welcome, my time to work on the project is limited.  Please post issues and pull requests on Github if you would like to help forward the project.\n',
     'author': 'Mark Raleson',
     'author_email': 'markraleson@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mraleson/piku.git',
```

### Comparing `piku-0.2.3/PKG-INFO` & `piku-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piku
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Home-page: https://github.com/mraleson/piku.git
 License: MIT
 Author: Mark Raleson
 Author-email: markraleson@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

