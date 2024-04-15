# Comparing `tmp/mpflash-0.5.0.tar.gz` & `tmp/mpflash-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpflash-0.5.0.tar", max compression
+gzip compressed data, was "mpflash-0.6.0.tar", max compression
```

## Comparing `mpflash-0.5.0.tar` & `mpflash-0.6.0.tar`

### file list

```diff
@@ -1,34 +1,39 @@
--rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.5.0/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.5.0/mpflash/__init__.py
--rw-r--r--   0        0        0     5248 2024-03-20 22:33:20.130001 mpflash-0.5.0/mpflash/ask_input.py
--rw-r--r--   0        0        0     2446 2024-03-20 21:36:30.723746 mpflash-0.5.0/mpflash/cli_download.py
--rw-r--r--   0        0        0     7341 2024-04-03 19:46:44.670186 mpflash-0.5.0/mpflash/cli_flash.py
--rw-r--r--   0        0        0     1946 2024-03-20 21:46:16.907966 mpflash-0.5.0/mpflash/cli_group.py
--rw-r--r--   0        0        0     2832 2024-03-27 18:14:45.280335 mpflash-0.5.0/mpflash/cli_list.py
--rw-r--r--   0        0        0      529 2024-03-20 21:44:59.429778 mpflash-0.5.0/mpflash/cli_main.py
--rw-r--r--   0        0        0     5066 2024-03-26 21:17:44.038751 mpflash-0.5.0/mpflash/common.py
--rw-r--r--   0        0        0      419 2024-03-19 23:55:54.108209 mpflash-0.5.0/mpflash/config.py
--rw-r--r--   0        0        0    10357 2024-03-20 21:15:24.579971 mpflash-0.5.0/mpflash/download.py
--rw-r--r--   0        0        0     5692 2024-03-20 21:18:04.789556 mpflash-0.5.0/mpflash/flash.py
--rw-r--r--   0        0        0     2396 2024-03-18 18:41:36.590406 mpflash-0.5.0/mpflash/flash_esp.py
--rw-r--r--   0        0        0      869 2024-03-15 14:55:22.828719 mpflash-0.5.0/mpflash/flash_stm32.py
--rw-r--r--   0        0        0     4010 2024-03-12 22:57:35.914158 mpflash-0.5.0/mpflash/flash_stm32_cube.py
--rw-r--r--   0        0        0     2509 2024-03-17 13:45:35.210978 mpflash-0.5.0/mpflash/flash_stm32_dfu.py
--rw-r--r--   0        0        0     2029 2024-03-15 15:46:23.966502 mpflash-0.5.0/mpflash/flash_uf2.py
--rw-r--r--   0        0        0      414 2024-03-05 22:17:23.940389 mpflash-0.5.0/mpflash/flash_uf2_boardid.py
--rw-r--r--   0        0        0     4298 2024-03-14 14:09:42.343080 mpflash-0.5.0/mpflash/flash_uf2_linux.py
--rw-r--r--   0        0        0     1072 2024-03-14 14:09:42.343080 mpflash-0.5.0/mpflash/flash_uf2_windows.py
--rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.5.0/mpflash/logger.py
--rw-r--r--   0        0        0     3143 2024-03-26 21:25:42.797035 mpflash-0.5.0/mpflash/mpboard_id/api.py
--rw-r--r--   0        0        0     1778 2024-03-12 12:49:58.741138 mpflash-0.5.0/mpflash/mpboard_id/board_id.py
--rw-r--r--   0        0        0    96983 2024-03-17 23:08:19.329031 mpflash-0.5.0/mpflash/mpboard_id/board_info.csv
--rw-r--r--   0        0        0   674442 2024-03-17 23:08:19.327031 mpflash-0.5.0/mpflash/mpboard_id/board_info.json
--rw-r--r--   0        0        0     4726 2024-03-13 16:28:38.858846 mpflash-0.5.0/mpflash/mpremoteboard/__init__.py
--rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.5.0/mpflash/mpremoteboard/mpy_fw_info.py
--rw-r--r--   0        0        0     4583 2024-03-13 16:26:49.937127 mpflash-0.5.0/mpflash/mpremoteboard/runner.py
--rw-r--r--   0        0        0     5739 2024-03-15 15:39:12.242892 mpflash-0.5.0/mpflash/vendored/dfu.py
--rw-r--r--   0        0        0    20542 2024-03-15 15:48:45.978919 mpflash-0.5.0/mpflash/vendored/pydfu.py
--rw-r--r--   0        0        0       86 2024-03-13 08:41:44.017018 mpflash-0.5.0/mpflash/vendored/readme.md
--rw-r--r--   0        0        0     1628 2024-04-05 08:35:21.948203 mpflash-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    12272 2024-03-12 12:49:58.724383 mpflash-0.5.0/README.md
--rw-r--r--   0        0        0    13797 1970-01-01 00:00:00.000000 mpflash-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.6.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.6.0/mpflash/__init__.py
+-rw-r--r--   0        0        0     7793 2024-04-12 12:06:31.002240 mpflash-0.6.0/mpflash/ask_input.py
+-rw-r--r--   0        0        0     3090 2024-04-12 12:06:31.002240 mpflash-0.6.0/mpflash/cli_download.py
+-rw-r--r--   0        0        0     5482 2024-04-12 12:06:31.002240 mpflash-0.6.0/mpflash/cli_flash.py
+-rw-r--r--   0        0        0     1946 2024-04-05 19:52:32.882426 mpflash-0.6.0/mpflash/cli_group.py
+-rw-r--r--   0        0        0     1005 2024-04-06 13:17:36.787587 mpflash-0.6.0/mpflash/cli_list.py
+-rw-r--r--   0        0        0      632 2024-04-11 20:40:17.002612 mpflash-0.6.0/mpflash/cli_main.py
+-rw-r--r--   0        0        0     1049 2024-04-12 12:22:07.242346 mpflash-0.6.0/mpflash/common.py
+-rw-r--r--   0        0        0      419 2024-04-05 19:52:32.888852 mpflash-0.6.0/mpflash/config.py
+-rw-r--r--   0        0        0    10765 2024-04-06 16:22:42.858056 mpflash-0.6.0/mpflash/download.py
+-rw-r--r--   0        0        0     3803 2024-04-09 22:57:44.547253 mpflash-0.6.0/mpflash/downloaded.py
+-rw-r--r--   0        0        0       96 2024-04-11 22:01:44.716103 mpflash-0.6.0/mpflash/errors.py
+-rw-r--r--   0        0        0     2490 2024-04-07 23:02:43.917516 mpflash-0.6.0/mpflash/flash.py
+-rw-r--r--   0        0        0     2316 2024-04-12 12:21:11.617847 mpflash-0.6.0/mpflash/flash_esp.py
+-rw-r--r--   0        0        0      823 2024-04-13 19:41:37.773737 mpflash-0.6.0/mpflash/flash_stm32.py
+-rw-r--r--   0        0        0     3970 2024-04-13 19:41:45.110360 mpflash-0.6.0/mpflash/flash_stm32_cube.py
+-rw-r--r--   0        0        0     2972 2024-04-11 22:23:28.005043 mpflash-0.6.0/mpflash/flash_stm32_dfu.py
+-rw-r--r--   0        0        0     2029 2024-04-05 19:52:32.892053 mpflash-0.6.0/mpflash/flash_uf2.py
+-rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.6.0/mpflash/flash_uf2_boardid.py
+-rw-r--r--   0        0        0     4298 2024-04-05 19:52:32.898069 mpflash-0.6.0/mpflash/flash_uf2_linux.py
+-rw-r--r--   0        0        0     1072 2024-04-05 19:52:32.900154 mpflash-0.6.0/mpflash/flash_uf2_windows.py
+-rw-r--r--   0        0        0     2248 2024-04-09 20:33:31.520438 mpflash-0.6.0/mpflash/list.py
+-rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.6.0/mpflash/logger.py
+-rw-r--r--   0        0        0     3509 2024-04-11 22:02:26.573574 mpflash-0.6.0/mpflash/mpboard_id/__init__.py
+-rw-r--r--   0        0        0     2230 2024-04-11 22:02:45.348676 mpflash-0.6.0/mpflash/mpboard_id/board_id.py
+-rw-r--r--   0        0        0    96983 2024-04-05 19:52:32.903789 mpflash-0.6.0/mpflash/mpboard_id/board_info.csv
+-rw-r--r--   0        0        0   674442 2024-04-05 19:52:32.903789 mpflash-0.6.0/mpflash/mpboard_id/board_info.json
+-rw-r--r--   0        0        0     6951 2024-04-12 12:21:47.875443 mpflash-0.6.0/mpflash/mpremoteboard/__init__.py
+-rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.6.0/mpflash/mpremoteboard/mpy_fw_info.py
+-rw-r--r--   0        0        0     4783 2024-04-15 16:01:00.749925 mpflash-0.6.0/mpflash/mpremoteboard/runner.py
+-rw-r--r--   0        0        0     5739 2024-04-05 19:52:32.916470 mpflash-0.6.0/mpflash/vendor/dfu.py
+-rw-r--r--   0        0        0    20542 2024-04-05 19:52:32.918984 mpflash-0.6.0/mpflash/vendor/pydfu.py
+-rw-r--r--   0        0        0       86 2024-04-05 19:52:32.919979 mpflash-0.6.0/mpflash/vendor/readme.md
+-rw-r--r--   0        0        0     3629 2024-04-12 10:48:05.417995 mpflash-0.6.0/mpflash/vendor/versions.py
+-rw-r--r--   0        0        0     5266 2024-04-12 12:06:31.002240 mpflash-0.6.0/mpflash/worklist.py
+-rw-r--r--   0        0        0     1628 2024-04-13 19:38:40.396476 mpflash-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    12253 2024-04-09 20:15:12.410633 mpflash-0.6.0/README.md
+-rw-r--r--   0        0        0    13778 1970-01-01 00:00:00.000000 mpflash-0.6.0/PKG-INFO
```

### Comparing `mpflash-0.5.0/LICENSE` & `mpflash-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpflash-0.5.0/mpflash/cli_download.py` & `mpflash-0.6.0/mpflash/cli_download.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 """CLI to Download MicroPython firmware for specific ports, boards and versions."""
 
 from pathlib import Path
 from typing import List, Tuple
 
 import rich_click as click
+from loguru import logger as log
 
-from mpflash.common import clean_version
+from mpflash.mpboard_id import find_stored_board
+from mpflash.vendor.versions import clean_version
 
 from .ask_input import DownloadParams, ask_missing_params
 from .cli_group import cli
 from .cli_list import list_mcus
 from .config import config
 from .download import download
 
 
-def connected_ports_boards() -> Tuple[List[str], List[str]]:
-    mpr_boards = list_mcus()
-    ports = list({b.port for b in mpr_boards})
-    boards = list({b.board for b in mpr_boards})
-    return ports, boards
-
-
 @cli.command(
     "download",
     help="Download MicroPython firmware for specific ports, boards and versions.",
 )
 @click.option(
     "--destination",
     "-d",
@@ -45,15 +40,15 @@
     metavar="SEMVER, 'stable', 'preview' or '?'",
 )
 @click.option(
     "--board",
     "-b",
     "boards",
     multiple=True,
-    default=["?"],
+    default=[],
     show_default=True,
     help="The board(s) to download the firmware for.",
     metavar="BOARD_ID or ?",
 )
 @click.option(
     "--clean/--no-clean",
     default=True,
@@ -67,25 +62,46 @@
     show_default=True,
     help="""Force download of firmware even if it already exists.""",
 )
 def cli_download(
     **kwargs,
 ):
     params = DownloadParams(**kwargs)
-
-    if not params.boards:
-        # nothing specified - detect connected boards
+    params.versions = list(params.versions)
+    params.boards = list(params.boards)
+    if params.boards:
+        pass
+        # TODO Clean board - same as in cli_flash.py
+    else:
+        # no boards specified - detect connected boards
         params.ports, params.boards = connected_ports_boards()
-    # ask for any remaining parameters
+
     params = ask_missing_params(params, action="download")
+    if not params:  # Cancelled by user
+        exit(1)
+    params.versions = [clean_version(v, drop_v=True) for v in params.versions]
     assert isinstance(params, DownloadParams)
 
-    params.versions = [clean_version(v, drop_v=True) for v in params.versions]  # remove leading v from version
-
     download(
         params.fw_folder,
         params.ports,
         params.boards,
         params.versions,
         params.force,
         params.clean,
     )
+
+
+def connected_ports_boards() -> Tuple[List[str], List[str]]:
+    """
+    Returns a tuple containing lists of unique ports and boards from the connected MCUs.
+    Boards that are physically connected, but give no tangible response are ignored.
+
+    Returns:
+        A tuple containing two lists:
+            - A list of unique ports where MCUs are connected.
+            - A list of unique board names of the connected MCUs.
+    """
+    mpr_boards = [b for b in list_mcus() if b.connected]
+    ports = list({b.port for b in mpr_boards})
+    boards = list({b.board for b in mpr_boards})
+    return ports, boards
```

### Comparing `mpflash-0.5.0/mpflash/cli_flash.py` & `mpflash-0.6.0/mpflash/ask_input.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,225 +1,234 @@
+"""
+Interactive input for mpflash.
+
+Note: The prompts can use "{version}" and "{action}" to insert the version and action in the prompt without needing an f-string.
+The values are provided from the answers dictionary.
+"""
+
+from dataclasses import dataclass, field
 from pathlib import Path
-from typing import List
+from typing import Dict, List, Sequence, Tuple, Union
 
-import rich_click as click
 from loguru import logger as log
 
-from .ask_input import FlashParams, ask_missing_params
-from .cli_download import connected_ports_boards
-from .cli_group import cli
-from .cli_list import show_mcus
-from .common import clean_version
-from .config import config
-from .flash import WorkList, auto_update, enter_bootloader, find_firmware
-from .flash_esp import flash_esp
-from .flash_stm32 import flash_stm32
-from .flash_uf2 import flash_uf2
-from .mpboard_id.api import find_mp_board
-from .mpremoteboard import MPRemoteBoard
-
-# #########################################################################################################
-# CLI
-# #########################################################################################################
-
-
-@cli.command(
-    "flash",
-    short_help="Flash one or all connected MicroPython boards with a specific firmware and version.",
-)
-@click.option(
-    "--firmware",
-    "-f",
-    "fw_folder",
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, path_type=Path),
-    default=config.firmware_folder,
-    show_default=True,
-    help="The folder to retrieve the firmware from.",
-)
-@click.option(
-    "--version",
-    "-v",
-    "version",  # single version
-    default="stable",
-    multiple=False,
-    show_default=True,
-    help="The version of MicroPython to flash.",
-    metavar="SEMVER, 'stable', 'preview' or '?'",
-)
-@click.option(
-    "--serial",
-    "--serial-port",
-    "-s",
-    "serial",
-    default="auto",
-    show_default=True,
-    help="Which serial port(s) to flash",
-    metavar="SERIAL_PORT",
-)
-@click.option(
-    "--port",
-    "-p",
-    "ports",
-    help="The MicroPython port to flash",
-    metavar="PORT",
-    default=[],
-    multiple=True,
-)
-@click.option(
-    "--board",
-    "-b",
-    "boards",
-    multiple=False,
-    default=[],
-    help="The MicroPython board ID to flash. If not specified will try to read the BOARD_ID from the connected MCU.",
-    metavar="BOARD_ID or ?",
-)
-@click.option(
-    "--cpu",
-    "--chip",
-    "-c",
-    "cpu",
-    help="The CPU type to flash. If not specified will try to read the CPU from the connected MCU.",
-    metavar="CPU",
-)
-@click.option(
-    "--erase/--no-erase",
-    default=True,
-    show_default=True,
-    help="""Erase flash before writing new firmware. (Not supported on UF2 boards)""",
-)
-@click.option(
-    "--bootloader/--no-bootloader",
-    default=True,
-    is_flag=True,
-    show_default=True,
-    help="""Enter micropython bootloader mode before flashing.""",
-)
-def cli_flash_board(**kwargs):
-    todo: WorkList = []
-
-    # version to versions
-    if "version" in kwargs:
-        kwargs["versions"] = [kwargs.pop("version")]
-    params = FlashParams(**kwargs)
-    print(f"{params=}")
-    # print(f"{params.version=}")
-    print(f"{params.versions=}")
-    if not params.boards:
-        # nothing specified - detect connected boards
-        params.ports, params.boards = connected_ports_boards()
-    # Ask for missing input if needed
-    params = ask_missing_params(params, action="flash")
-    # TODO: Just in time Download of firmware
-
-    assert isinstance(params, FlashParams)
-
-    if len(params.versions) > 1:
-        print(repr(params.versions))
-        log.error(f"Only one version can be flashed at a time, not {params.versions}")
-        return
-    params.versions = [clean_version(v) for v in params.versions]
-    if params.versions[0] and params.boards[0] and params.serial:
-        # update a single board
-        todo = manual_worklist(
-            params.versions[0],
-            params.fw_folder,
-            params.serial,
-            params.boards[0],
-            # params.ports[0],
-        )
-    elif params.serial:
-        if params.serial == "auto":
-            # Update all micropython boards to the latest version
-            todo = auto_worklist(params.versions[0], params.fw_folder)
-        else:
-            # just this serial port on auto
-            todo = oneport_worklist(
-                params.versions[0],
-                params.fw_folder,
-                params.serial,
-            )
-
-    if flashed := flash_list(
-        todo,
-        params.fw_folder,
-        params.erase,
-        params.bootloader,
-    ):
-        log.info(f"Flashed {len(flashed)} boards")
-        show_mcus(flashed, title="Connected boards after flashing")
-
-
-def oneport_worklist(
-    version: str,
-    fw_folder: Path,
-    serial_port: str,
-    # preview: bool,
-) -> WorkList:
-    """Create a worklist for a single serial-port."""
-    conn_boards = [MPRemoteBoard(serial_port)]
-    todo = auto_update(conn_boards, version, fw_folder)  # type: ignore # List / list
-    show_mcus(conn_boards)  # type: ignore
-    return todo
-
-
-def auto_worklist(version: str, fw_folder: Path) -> WorkList:
-    conn_boards = [MPRemoteBoard(sp) for sp in MPRemoteBoard.connected_boards() if sp not in config.ignore_ports]
-    return auto_update(conn_boards, version, fw_folder)  # type: ignore
-
-
-def manual_worklist(
-    version: str,
-    fw_folder: Path,
-    serial_port: str,
-    board: str,
-    # port: str,
-) -> WorkList:
-    mcu = MPRemoteBoard(serial_port)
-    # TODO : Find a way to avoid needing to specify the port
-    # Lookup the matching port and cpu in board_info based in the board name
-    port = find_mp_board(board)["port"]
-    mcu.port = port
-    mcu.cpu = port if port.startswith("esp") else ""
-    mcu.board = board
-    firmwares = find_firmware(fw_folder=fw_folder, board=board, version=version, port=port)
-    if not firmwares:
-        log.error(f"No firmware found for {port} {board} version {version}")
-        return []
-        # use the most recent matching firmware
-    return [(mcu, firmwares[-1])]  # type: ignore
-
-
-def flash_list(
-    todo: WorkList,
-    fw_folder: Path,
-    erase: bool,
-    bootloader: bool,
-):
-    """Flash a list of boards with the specified firmware."""
-    flashed = []
-    for mcu, fw_info in todo:
-        fw_file = fw_folder / fw_info["filename"]  # type: ignore
-        if not fw_file.exists():
-            log.error(f"File {fw_file} does not exist, skipping {mcu.board} on {mcu.serialport}")
-            continue
-        log.info(f"Updating {mcu.board} on {mcu.serialport} to {fw_info['version']}")
-        updated = None
-        # try:
-        if mcu.port in ["samd", "rp2", "nrf"]:  #  [k for k, v in PORT_FWTYPES.items() if v == ".uf2"]:
-            if bootloader:
-                enter_bootloader(mcu)
-            updated = flash_uf2(mcu, fw_file=fw_file, erase=erase)
-        elif mcu.port in ["stm32"]:
-            if bootloader:
-                enter_bootloader(mcu)
-            updated = flash_stm32(mcu, fw_file, erase=erase)
-        elif mcu.port in ["esp32", "esp8266"]:
-            #  bootloader is handled by esptool for esp32/esp8266
-            updated = flash_esp(mcu, fw_file=fw_file, erase=erase)
+from mpflash.config import config
+from mpflash.mpboard_id import known_stored_boards, local_mp_ports
+from mpflash.mpremoteboard import MPRemoteBoard
+from mpflash.vendor.versions import micropython_versions
+
+
+@dataclass
+class Params:
+    ports: List[str] = field(default_factory=list)
+    boards: List[str] = field(default_factory=list)
+    versions: List[str] = field(default_factory=list)
+    fw_folder: Path = Path()
+
+
+@dataclass
+class DownloadParams(Params):
+    clean: bool = False
+    force: bool = False
+
+
+@dataclass
+class FlashParams(Params):
+    # TODO: Should Serial port be a list?
+    serial: str = ""
+    erase: bool = True
+    bootloader: bool = True
+    cpu: str = ""
+
+
+ParamType = Union[DownloadParams, FlashParams]
+
+
+def ask_missing_params(
+    params: ParamType,
+    action: str = "download",
+) -> ParamType:
+    """
+    Asks the user for parameters that have not been supplied on the commandline and returns the updated params.
+
+    Args:
+        params (ParamType): The parameters to be updated.
+        action (str, optional): The action to be performed. Defaults to "download".
+
+    Returns:
+        ParamType: The updated parameters.
+    """
+    if not config.interactive:
+        # no interactivity allowed
+        return params
+    # import only when needed to reduce load time
+    import inquirer
+
+    questions = []
+    answers = {"action": action}
+    if isinstance(params, FlashParams):
+        if not params.serial or "?" in params.serial:
+            ask_serialport(questions, action=action)
         else:
-            log.error(f"Don't (yet) know how to flash {mcu.port}-{mcu.board} on {mcu.serialport}")
+            answers["serial"] = params.serial
 
-        if updated:
-            flashed.append(updated)
-        else:
-            log.error(f"Failed to flash {mcu.board} on {mcu.serialport}")
+    if not params.versions or "?" in params.versions:
+        ask_versions(questions, action=action)
+    else:
+        # versions is used to show only the boards for the selected versions
+        answers["versions"] = params.versions  # type: ignore
+
+    if not params.boards or "?" in params.boards:
+        ask_port_board(questions, action=action)
+
+    answers = inquirer.prompt(questions, answers=answers)
+    if not answers:
+        # input cancelled by user
+        return []  # type: ignore
+    # print(repr(answers))
+    if isinstance(params, FlashParams) and "serial" in answers:
+        params.serial = answers["serial"]
+    if "port" in answers:
+        params.ports = [answers["port"]]
+    if "boards" in answers:
+        params.boards = answers["boards"] if isinstance(answers["boards"], list) else [answers["boards"]]
+    if "versions" in answers:
+        # make sure it is a list
+        params.versions = answers["versions"] if isinstance(answers["versions"], list) else [answers["versions"]]
+
+    log.debug(repr(params))
+
+    return params
+
+
+def filter_matching_boards(answers: dict) -> Sequence[Tuple[str, str]]:
+    """
+    Filters the known boards based on the selected versions and returns the filtered boards.
+
+    Args:
+        answers (dict): The user's answers.
+
+    Returns:
+        Sequence[Tuple[str, str]]: The filtered boards.
+    """
+    # if version is not asked ; then need to get the version from the inputs
+    if "versions" in answers:
+        _versions = list(answers["versions"])
+        if "stable" in _versions:
+            _versions.remove("stable")
+            _versions.append(micropython_versions()[-2])  # latest stable
+        if "preview" in _versions:
+            _versions.remove("preview")
+            _versions.extend((micropython_versions()[-1], micropython_versions()[-2]))  # latest preview and stable
+
+        some_boards = known_stored_boards(answers["port"], _versions)  #    or known_mp_boards(answers["port"])
+    else:
+        some_boards = known_stored_boards(answers["port"])
+
+    if some_boards:
+        # Create a dictionary where the keys are the second elements of the tuples
+        # This will automatically remove duplicates because dictionaries cannot have duplicate keys
+        unique_dict = {item[1]: item for item in some_boards}
+        # Get the values of the dictionary, which are the unique items from the original list
+        some_boards = list(unique_dict.values())
+    else:
+        some_boards = [("No boards found", "")]
+    return some_boards
+
+
+def ask_port_board(questions: list, *, action: str):
+    """
+    Asks the user for the port and board selection.
+
+    Args:
+        questions (list): The list of questions to be asked.
+        action (str): The action to be performed.
+
+    Returns:
+        None
+    """
+    # import only when needed to reduce load time
+    import inquirer
+
+    # TODO: if action = flash, Use Inquirer.List for boards
+    inquirer_ux = inquirer.Checkbox if action == "download" else inquirer.List
+    questions.extend(
+        (
+            inquirer.List(
+                "port",
+                message="Which port do you want to {action} " + "to {serial} ?" if action == "flash" else "?",
+                choices=local_mp_ports(),
+                autocomplete=True,
+            ),
+            inquirer_ux(
+                "boards",
+                message=(
+                    "Which {port} board firmware do you want to {action} " + "to {serial} ?"
+                    if action == "flash"
+                    else "?"
+                ),
+                choices=filter_matching_boards,
+                validate=lambda _, x: True if x else "Please select at least one board",  # type: ignore
+            ),
+        )
+    )
+
+
+def ask_versions(questions: list, *, action: str):
+    """
+    Asks the user for the version selection.
+
+    Args:
+        questions (list): The list of questions to be asked.
+        action (str): The action to be performed.
+
+    Returns:
+        None
+    """
+    # import only when needed to reduce load time
+    import inquirer
+
+    input_ux = inquirer.Checkbox if action == "download" else inquirer.List
+    mp_versions: List[str] = micropython_versions()
+    mp_versions = [v for v in mp_versions if "preview" not in v]
+    mp_versions.append("preview")
+    mp_versions.reverse()  # newest first
+    questions.append(
+        input_ux(
+            # inquirer.List(
+            "versions",
+            message="Which version(s) do you want to {action} " + ("to {serial} ?" if action == "flash" else "?"),
+            # Hints would be nice , but needs a hint for each and every option
+            # hints=["Use space to select multiple options"],
+            choices=mp_versions,
+            autocomplete=True,
+            validate=lambda _, x: True if x else "Please select at least one version",  # type: ignore
+        )
+    )
+
+
+def ask_serialport(questions: list, *, action: str):
+    """
+    Asks the user for the serial port selection.
+
+    Args:
+        questions (list): The list of questions to be asked.
+        action (str): The action to be performed.
+
+    Returns:
+        None
+    """
+    # import only when needed to reduce load time
+    import inquirer
+
+    serialports = MPRemoteBoard.connected_boards()
+    questions.append(
+        inquirer.List(
+            "serial",
+            message="Which serial port do you want to {action} ?",
+            choices=serialports,
+            other=True,
+            validate=lambda _, x: True if x else "Please select or enter a serial port",  # type: ignore
+        )
+    )
+
+    return questions
```

### Comparing `mpflash-0.5.0/mpflash/cli_group.py` & `mpflash-0.6.0/mpflash/cli_group.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.5.0/mpflash/cli_list.py` & `mpflash-0.6.0/mpflash/list.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,29 @@
-import json
 from typing import List
 
-import rich_click as click
 from rich import print
 from rich.progress import track
 from rich.table import Table
 
 from mpflash.mpremoteboard import MPRemoteBoard
 
-from .cli_group import cli
 from .config import config
-from .logger import console, make_quiet
+from .logger import console
 
 
-@cli.command("list", help="List the connected MCU boards.")
-@click.option(
-    "--json",
-    "-j",
-    "as_json",
-    is_flag=True,
-    default=False,
-    show_default=True,
-    help="""Output in json format""",
-)
-@click.option(
-    "--progress/--no-progress",
-    "progress",
-    is_flag=True,
-    default=True,
-    show_default=True,
-    help="""Show progress""",
-)
-def cli_list_mcus(as_json: bool, progress: bool = True):
-    """List the connected MCU boards, and output in a nice table or json."""
-    if as_json:
-        # avoid noise in json output
-        make_quiet()
-
-    conn_mcus = list_mcus()
-    if as_json:
-        print(json.dumps([mcu.__dict__ for mcu in conn_mcus], indent=4))
-        progress = False
-    if progress:
-        show_mcus(conn_mcus, refresh=False)
-    return conn_mcus
-
-
-def list_mcus():
-    conn_mcus = [MPRemoteBoard(sp) for sp in MPRemoteBoard.connected_boards() if sp not in config.ignore_ports]
+def list_mcus(bluetooth: bool = False):
+    """
+    Retrieves information about connected microcontroller boards.
+
+    Returns:
+        List[MPRemoteBoard]: A list of MPRemoteBoard instances with board information.
+    Raises:
+        ConnectionError: If there is an error connecting to a board.
+    """
+    conn_mcus = [MPRemoteBoard(sp) for sp in MPRemoteBoard.connected_boards(bluetooth) if sp not in config.ignore_ports]
 
     for mcu in track(conn_mcus, description="Getting board info", transient=True, update_period=0.1):
         try:
             mcu.get_mcu_info()
         except ConnectionError as e:
             print(f"Error: {e}")
             continue
@@ -62,14 +34,15 @@
     conn_mcus: List[MPRemoteBoard],
     title: str = "Connected boards",
     refresh: bool = True,
 ):  # sourcery skip: extract-duplicate-method
     """Show the list of connected boards in a nice table"""
     table = Table(
         title=title,
+        title_style="bold",
         header_style="bold blue",
         collapse_padding=True,
         width=110,
         row_styles=["blue", "yellow"],
     )
     table.add_column("Serial", overflow="fold")
     table.add_column("Family")
```

### Comparing `mpflash-0.5.0/mpflash/cli_main.py` & `mpflash-0.6.0/mpflash/cli_main.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,12 +11,16 @@
 
 
 def mpflash():
     cli.add_command(cli_flash_board)
     cli.add_command(cli_list_mcus)
     cli.add_command(cli_download)
     # cli(auto_envvar_prefix="MPFLASH")
-    cli()
+    try:
+        exit(cli())
+    except AttributeError as e:
+        print(f"Error: {e}")
+        exit(-1)
 
 
-# if __name__ == "__main__":
-mpflash()
+if __name__ == "__main__":
+    mpflash()
```

### Comparing `mpflash-0.5.0/mpflash/download.py` & `mpflash-0.6.0/mpflash/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,27 +42,39 @@
 
 
 @functools.lru_cache(maxsize=500)
 def get_board_urls(page_url: str) -> List[Dict[str, str]]:
     """
     Get the urls to all the board pages listed on this page.
     Assumes that all links to firmware  have "class": "board-card"
+
+    Args:
+        page_url (str): The url of the page to get the board urls from.
     """
     downloads_html = get_page(page_url)
     soup = BeautifulSoup(downloads_html, "html.parser")
     tags = soup.findAll("a", recursive=True, attrs={"class": "board-card"})
     # assumes that all links are relative to the page url
     boards = [tag.get("href") for tag in tags]
     if "?" in page_url:
         page_url = page_url.split("?")[0]
     return [{"board": board, "url": page_url + board} for board in boards]
 
 
-def firmware_list(board_url: str, base_url: str, ext: str) -> List[str]:
-    """Get the urls to all the firmware files for a board."""
+def board_firmware_urls(board_url: str, base_url: str, ext: str) -> List[str]:
+    """
+    Get the urls to all the firmware files for a board.
+    Args:
+        page_url (str): The url of the page to get the board urls from.
+    ??? base_url (str): The base url to join the relative urls to.
+        ext (str): The extension of the firmware files to get. (with or withouth leading .)
+
+    the urls are relative urls to the site root
+
+    """
     html = get_page(board_url)
     soup = BeautifulSoup(html, "html.parser")
     # get all the a tags:
     #  1. that have a url that starts with `/resources/firmware/`
     #  2. end with a matching extension for this port.
     tags = soup.findAll(
         "a",
@@ -105,15 +117,15 @@
         for board in _urls:
             board["port"] = port
 
         for board in track(_urls, description=f"Checking {port} download pages", transient=True):
             # add a board to the list for each firmware found
             firmwares = []
             for ext in PORT_FWTYPES[port]:
-                firmwares += firmware_list(board["url"], MICROPYTHON_ORG_URL, ext)
+                firmwares += board_firmware_urls(board["url"], MICROPYTHON_ORG_URL, ext)
 
             for _url in firmwares:
                 board["firmware"] = _url
                 board["preview"] = "preview" in _url  # type: ignore
                 if ver_match := re.search(RE_VERSION_PREVIEW, _url):
                     board["version"] = ver_match[1]
                 else:
```

### Comparing `mpflash-0.5.0/mpflash/flash.py` & `mpflash-0.6.0/mpflash/worklist.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,138 +1,56 @@
-import time
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
-import jsonlines
 from loguru import logger as log
 
-from mpflash.mpremoteboard import MPRemoteBoard
+from mpflash.common import FWInfo
+from mpflash.errors import MPFlashError
 
-from .common import FWInfo, clean_version
 from .config import config
+from .downloaded import find_downloaded_firmware
+from .list import show_mcus
+from .mpboard_id import find_stored_board
+from .mpremoteboard import MPRemoteBoard
 
 # #########################################################################################################
 WorkList = List[Tuple[MPRemoteBoard, FWInfo]]
-
-
-# #########################################################################################################
-def local_firmwares(fw_folder: Path) -> List[FWInfo]:
-    """Load a list of locally available  firmwares from the jsonl file"""
-    firmwares: List[FWInfo] = []
-    try:
-        with jsonlines.open(fw_folder / "firmware.jsonl") as reader:
-            firmwares.extend(iter(reader))
-    except FileNotFoundError:
-        log.error(f"No firmware.jsonl found in {fw_folder}")
-    # sort by filename
-    firmwares.sort(key=lambda x: x["filename"])
-    return firmwares
-
-
-def find_firmware(
-    *,
-    board: str,
-    version: str = "",
-    port: str = "",
-    variants: bool = False,
-    fw_folder: Optional[Path] = None,
-    trie: int = 1,
-    selector: Optional[Dict[str, str]] = None,
-) -> List[FWInfo]:
-    if selector is None:
-        selector = {}
-    fw_folder = fw_folder or config.firmware_folder
-    # Use the information in firmwares.jsonl to find the firmware file
-    fw_list = local_firmwares(fw_folder)
-    if not fw_list:
-        log.error("No firmware files found. Please download the firmware first.")
-        return []
-    # filter by version
-    version = clean_version(version, drop_v=True)
-    fw_list = filter_fwlist(fw_list, board, version, port, variants, selector)
-
-    if not fw_list and trie < 2:
-        board_id = board.replace("_", "-")
-        # ESP board naming conventions have changed by adding a PORT refix
-        if port.startswith("esp") and not board_id.startswith(port.upper()):
-            board_id = f"{port.upper()}_{board_id}"
-        # RP2 board naming conventions have changed by adding a _RPIprefix
-        if port == "rp2" and not board_id.startswith("RPI_"):
-            board_id = f"RPI_{board_id}"
-
-        log.info(f"Try ({trie}) to find a firmware for the board {board_id}")
-        fw_list = find_firmware(
-            fw_folder=fw_folder,
-            board=board_id,
-            version=version,
-            port=port,
-            trie=trie + 1,
-            selector=selector,
-        )
-        # hope we have a match now for the board
-    # sort by filename
-    fw_list.sort(key=lambda x: x["filename"])
-    return fw_list
-
-
-def filter_fwlist(
-    fw_list: List[FWInfo],
-    board: str,
-    version: str,
-    port: str,
-    # preview: bool,
-    variants: bool,
-    selector: dict,
-) -> List[FWInfo]:
-    """Filter the firmware list based on the provided parameters"""
-    if "preview" in version:
-        # never get a preview for an older version
-        fw_list = [fw for fw in fw_list if fw["preview"]]
-    else:
-        fw_list = [fw for fw in fw_list if fw["version"] == version]
-
-    # filter by port
-    if port:
-        fw_list = [fw for fw in fw_list if fw["port"] == port]
-
-    if board:
-        if variants:
-            fw_list = [fw for fw in fw_list if fw["board"] == board]
-        else:
-            # the variant should match exactly the board name
-            fw_list = [fw for fw in fw_list if fw["variant"] == board]
-    if selector and port in selector:
-        fw_list = [fw for fw in fw_list if fw["filename"].endswith(selector[port])]
-    return fw_list
-
-
 # #########################################################################################################
-#
 
 
 def auto_update(
     conn_boards: List[MPRemoteBoard],
     target_version: str,
     fw_folder: Path,
     *,
     selector: Optional[Dict[str, str]] = None,
 ) -> WorkList:
-    """Builds a list of boards to update based on the connected boards and the firmware available"""
+    """Builds a list of boards to update based on the connected boards and the firmware available
+
+    Args:
+        conn_boards (List[MPRemoteBoard]): List of connected boards
+        target_version (str): Target firmware version
+        fw_folder (Path): Path to the firmware folder
+        selector (Optional[Dict[str, str]], optional): Selector for filtering firmware. Defaults to None.
+
+    Returns:
+        WorkList: List of boards and firmware information to update
+    """
     if selector is None:
         selector = {}
     wl: WorkList = []
     for mcu in conn_boards:
-        if mcu.family != "micropython":
+        if mcu.family not in ("micropython", "unknown"):
             log.warning(
-                f"Skipping {mcu.family} {mcu.port} {mcu.board} on {mcu.serialport} as it is a MicroPython firmware"
+                f"Skipping flashing {mcu.family} {mcu.port} {mcu.board} on {mcu.serialport} as it is not a MicroPython firmware"
             )
             continue
-        board_firmwares = find_firmware(
+        board_firmwares = find_downloaded_firmware(
             fw_folder=fw_folder,
-            board=mcu.board,
+            board_id=mcu.board,
             version=target_version,
             port=mcu.port,
             selector=selector,
         )
 
         if not board_firmwares:
             log.error(f"No {target_version} firmware found for {mcu.board} on {mcu.serialport}.")
@@ -143,22 +61,87 @@
         # just use the last firmware
         fw_info = board_firmwares[-1]
         log.info(f"Found {target_version} firmware {fw_info['filename']} for {mcu.board} on {mcu.serialport}.")
         wl.append((mcu, fw_info))
     return wl
 
 
-def enter_bootloader(mcu: MPRemoteBoard, timeout: int = 10, wait_after: int = 2):
-    """Enter the bootloader mode for the board"""
-    log.info(f"Entering bootloader on {mcu.board} on {mcu.serialport}")
-    mcu.run_command("bootloader", timeout=timeout)
-    time.sleep(wait_after)
+def single_auto_worklist(
+    *,
+    serial_port: str,
+    version: str,
+    fw_folder: Path,
+) -> WorkList:
+    """Create a worklist for a single serial-port.
 
+    Args:
+        serial_port (str): Serial port of the board
+        version (str): Firmware version
+        fw_folder (Path): Path to the firmware folder
+
+    Returns:
+        WorkList: List of boards and firmware information to update
+    """
+    conn_boards = [MPRemoteBoard(serial_port)]
+    todo = auto_update(conn_boards, version, fw_folder)  # type: ignore # List / list
+    show_mcus(conn_boards)  # type: ignore
+    return todo
+
+
+def full_auto_worklist(*, version: str, fw_folder: Path) -> WorkList:
+    """
+    Create a worklist for all connected micropython boards based on the information retrieved from the board.
+    This allows the firmware version of one or moae boards to be changed without needing to specify the port or board_id manually.
+
+    Args:
+        version (str): Firmware version
+        fw_folder (Path): Path to the firmware folder
+
+    Returns:
+        WorkList: List of boards and firmware information to update
+    """
+    try:
+        conn_boards = [
+            MPRemoteBoard(sp, update=True) for sp in MPRemoteBoard.connected_boards() if sp not in config.ignore_ports
+        ]
+    except ConnectionError as e:
+        log.error(f"Error connecting to boards: {e}")
+        return []
+    return auto_update(conn_boards, version, fw_folder)  # type: ignore
 
-# TODO:
-# flash from some sort of queue to allow different images to be flashed to the same board
-#  - flash variant 1
-#  - stub variant 1
-#  - flash variant 2
-#  - stub variant 2
-#
-# JIT download / download any missing firmwares based on the detected boards
+
+def manual_worklist(
+    version: str,
+    fw_folder: Path,
+    serial_port: str,
+    board: str,
+    # port: str,
+) -> WorkList:
+    """Create a worklist for a single board specified manually.
+
+    Args:
+        version (str): Firmware version
+        fw_folder (Path): Path to the firmware folder
+        serial_port (str): Serial port of the board
+        board (str): Board name
+
+    Returns:
+        WorkList: List of boards and firmware information to update
+    """
+    mcu = MPRemoteBoard(serial_port)
+    # TODO : Find a way to avoid needing to specify the port
+    # Lookup the matching port and cpu in board_info based in the board name
+    try:
+        info = find_stored_board(board)
+        mcu.port = info["port"]
+        # need the CPU type for the esptool
+        mcu.cpu = info["cpu"]
+    except (LookupError, MPFlashError) as e:
+        log.error(f"Board {board} not found in board_info.json")
+        return []
+    mcu.board = board
+    firmwares = find_downloaded_firmware(fw_folder=fw_folder, board_id=board, version=version, port=mcu.port)
+    if not firmwares:
+        log.error(f"No firmware found for {mcu.port} {board} version {version}")
+        return []
+        # use the most recent matching firmware
+    return [(mcu, firmwares[-1])]  # type: ignore
```

### Comparing `mpflash-0.5.0/mpflash/flash_esp.py` & `mpflash-0.6.0/mpflash/flash_esp.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,59 +6,54 @@
 
 from pathlib import Path
 from typing import List, Optional
 
 import esptool
 from loguru import logger as log
 
-from mpflash.mpboard_id.api import find_mp_board
+from mpflash.mpboard_id import find_stored_board
 from mpflash.mpremoteboard import MPRemoteBoard
 
-from .common import wait_for_restart
-
 
 def flash_esp(mcu: MPRemoteBoard, fw_file: Path, *, erase: bool = True) -> Optional[MPRemoteBoard]:
     if mcu.port not in ["esp32", "esp8266"] or mcu.board in ["ARDUINO_NANO_ESP32"]:
         log.error(f"esptool not supported for {mcu.port} {mcu.board} on {mcu.serialport}")
         return None
 
     log.info(f"Flashing {fw_file} on {mcu.board} on {mcu.serialport}")
     if not mcu.cpu:
         # Lookup CPU based on the board name
-        mcu.cpu = find_mp_board(mcu.board)["cpu"]
+        mcu.cpu = find_stored_board(mcu.board)["cpu"]
 
-    if mcu.port == "esp8266":
-        baud_rate = str(460_800)
-    else:
-        baud_rate = str(512_000)
-        # baud_rate = str(115_200)
     cmds: List[List[str]] = []
     if erase:
         cmds.append(f"esptool --chip {mcu.cpu} --port {mcu.serialport} erase_flash".split())
 
-    if mcu.cpu.upper() in ("ESP32", "ESP32S2"):
-        start_addr = "0x1000"
-    elif mcu.cpu.upper() in ("ESP32S3", "ESP32C3"):
-        start_addr = "0x0"
     if mcu.cpu.upper().startswith("ESP32"):
+        baud_rate = str(921_600)
+        if mcu.cpu.upper() in ("ESP32", "ESP32S2"):
+            start_addr = "0x1000"
+        elif mcu.cpu.upper() in ("ESP32S3", "ESP32C3"):
+            start_addr = "0x0"
         cmds.append(
             f"esptool --chip {mcu.cpu} --port {mcu.serialport} -b {baud_rate} write_flash --compress {start_addr}".split()
             + [str(fw_file)]
         )
     elif mcu.cpu.upper() == "ESP8266":
+        baud_rate = str(460_800)
         start_addr = "0x0"
         cmds.append(
             f"esptool --chip {mcu.cpu} --port {mcu.serialport} -b {baud_rate} write_flash --flash_size=detect {start_addr}".split()
             + [str(fw_file)]
         )
     try:
         for cmd in cmds:
             log.info(f"Running {' '.join(cmd)} ")
             esptool.main(cmd[1:])
     except Exception as e:
         log.error(f"Failed to flash {mcu.board} on {mcu.serialport} : {e}")
         return None
 
     log.info("Done flashing, resetting the board and wait for it to restart")
-    wait_for_restart(mcu)
-    log.success(f"Flashed {mcu.version} to {mcu.board}")
+    mcu.wait_for_restart()
+    log.success(f"Flashed {mcu.serialport} to {mcu.board} {mcu.version}")
     return mcu
```

### Comparing `mpflash-0.5.0/mpflash/flash_stm32.py` & `mpflash-0.6.0/mpflash/flash_stm32.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Flash STM32 boards using either STM32CubeProgrammer CLI or dfu-util"""
 
 from pathlib import Path
 
 from loguru import logger as log
 
-from mpflash.common import wait_for_restart
-
 # from .flash_stm32_cube import flash_stm32_cubecli
 from .flash_stm32_dfu import dfu_init, flash_stm32_dfu
 from mpflash.mpremoteboard import MPRemoteBoard
 
 
 def flash_stm32(mcu: MPRemoteBoard, fw_file: Path, *, erase: bool, stm32_dfu: bool = True):
     # sourcery skip: lift-return-into-if
@@ -17,10 +15,10 @@
     dfu_init()
     updated = flash_stm32_dfu(mcu, fw_file=fw_file, erase=erase)
     # if stm32_dfu:
     # else:
     #     log.info("Using STM32CubeProgrammer CLI")
     #     updated = flash_stm32_cubecli(mcu, fw_file=fw_file, erase=erase)
 
-    wait_for_restart(mcu)
+    mcu.wait_for_restart()
     log.success(f"Flashed {mcu.version} to {mcu.board}")
     return updated
```

### Comparing `mpflash-0.5.0/mpflash/flash_stm32_cube.py` & `mpflash-0.6.0/mpflash/flash_stm32_cube.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # from typing import Optional
 
 # import bincopy
 # from loguru import logger as log
 # from rich.progress import track
 # from strip_ansi import strip_ansi
 
-# from .common import wait_for_restart
 # from .mpremoteboard.mpremoteboard import MPRemoteBoard
 
 # STM32_CLI_WIN = "C:\\Program Files\\STMicroelectronics\\STM32Cube\\STM32CubeProgrammer\\bin\\STM32_Programmer_CLI.exe"
 # STM32_CLI_LINUX = "~/STMicroelectronics/STM32Cube/STM32CubeProgrammer/bin/STM32_Programmer_CLI"
 
 
 # def get_stm32_start_address(fw_file: Path):
```

### Comparing `mpflash-0.5.0/mpflash/flash_stm32_dfu.py` & `mpflash-0.6.0/mpflash/flash_stm32_dfu.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,51 +4,65 @@
 
 from loguru import logger as log
 
 from mpflash.mpremoteboard import MPRemoteBoard
 
 
 def init_libusb_windows() -> bool:
-    # on windows we need to initialze the libusb backend with the correct dll
+    """
+    Initializes the libusb backend on Windows.
+
+    Returns:
+        bool: True if the initialization is successful, False otherwise.
+    """
     import libusb  # type: ignore
     import usb.backend.libusb1 as libusb1
 
     arch = "x64" if platform.architecture()[0] == "64bit" else "x86"
     libusb1_dll = Path(libusb.__file__).parent / f"_platform\\_windows\\{arch}\\libusb-1.0.dll"
     if not libusb1_dll.exists():
         raise FileNotFoundError(f"libusb1.dll not found at {libusb1_dll}")
     backend = libusb1.get_backend(find_library=lambda x: libusb1_dll.as_posix())
     return backend is not None
 
 
 try:
-    from .vendored import pydfu as pydfu
+    from .vendor import pydfu as pydfu
 except ImportError:
     pydfu = None
 
 
 def dfu_init():
+    """
+    Initializes the DFU (Device Firmware Upgrade) process.
+    """
     if not pydfu:
         log.error("pydfu not found")
         return None
     if platform.system() == "Windows":
         init_libusb_windows()
 
 
 def flash_stm32_dfu(
     mcu: MPRemoteBoard,
     fw_file: Path,
     *,
     erase: bool = True,
 ) -> Optional[MPRemoteBoard]:
+    """
+    Flashes the STM32 microcontroller using DFU (Device Firmware Upgrade).
 
-    # if sys.platform == "win32":
-    #     log.error(f"OS {sys.platform} not supported")
-    #     return None
-
+    Args:
+        mcu (MPRemoteBoard): The remote board to flash.
+        fw_file (Path): The path to the firmware file (.dfu).
+        erase (bool, optional): Whether to erase the memory before flashing. Defaults to True.
+
+    Returns:
+        Optional[MPRemoteBoard]: The flashed remote board if successful, None otherwise.
+    """
     if not pydfu:
         log.error("pydfu not found, please install it with 'pip install pydfu' if supported")
         return None
 
     if not fw_file.exists():
         log.error(f"File {fw_file} not found")
         return None
```

### Comparing `mpflash-0.5.0/mpflash/flash_uf2.py` & `mpflash-0.6.0/mpflash/flash_uf2.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.5.0/mpflash/flash_uf2_linux.py` & `mpflash-0.6.0/mpflash/flash_uf2_linux.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.5.0/mpflash/flash_uf2_windows.py` & `mpflash-0.6.0/mpflash/flash_uf2_windows.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.5.0/mpflash/logger.py` & `mpflash-0.6.0/mpflash/logger.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.5.0/mpflash/mpboard_id/api.py` & `mpflash-0.6.0/mpflash/mpboard_id/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,21 @@
+"""
+Access to the micropython port and board information that is stored in the board_info.json file 
+that is included in the module.
+
+"""
+
 import json
 from functools import lru_cache
 from pathlib import Path
 from typing import List, Optional, Tuple, TypedDict, Union
 
-from mpflash.common import PORT_FWTYPES, clean_version
+from mpflash.errors import MPFlashError
+from mpflash.common import PORT_FWTYPES
+from mpflash.vendor.versions import clean_version
 
 
 # Board  based on the dataclass Board but changed to TypedDict
 # - source : get_boardnames.py
 class Board(TypedDict):
     """MicroPython Board definition"""
 
@@ -18,35 +26,35 @@
     mcu_name: str
     path: Union[Path, str]
     version: str
     cpu: str
 
 
 @lru_cache(maxsize=None)
-def read_boardinfo() -> List[Board]:
+def read_stored_boardinfo() -> List[Board]:
     """Reads the board_info.json file and returns the data as a list of Board objects"""
     with open(Path(__file__).parent / "board_info.json", "r") as file:
         return json.load(file)
 
 
-def known_mp_ports() -> List[str]:
+def local_mp_ports() -> List[str]:
     # TODO: Filter for Version
-    mp_boards = read_boardinfo()
+    mp_boards = read_stored_boardinfo()
     # select the unique ports from info
     ports = set({board["port"] for board in mp_boards if board["port"] in PORT_FWTYPES.keys()})
     return sorted(list(ports))
 
 
-def get_mp_boards_for_port(port: str, versions: Optional[List[str]] = None):
+def get_stored_boards_for_port(port: str, versions: Optional[List[str]] = None):
     """
     Returns a list of boards for the given port and version(s)
 
     port : str : The Micropython port to filter for
     versions : List[str] : The Micropython versions to filter for (actual versions required)"""
-    mp_boards = read_boardinfo()
+    mp_boards = read_stored_boardinfo()
 
     # filter for 'preview' as they are not in the board_info.json
     # instead use stable version
     versions = versions or []
     if "preview" in versions:
         versions.remove("preview")
         versions.append("stable")
@@ -56,34 +64,33 @@
         # filter for the version(s)
         mp_boards = [board for board in mp_boards if board["version"] in versions]
     # filter for the port
     mp_boards = [board for board in mp_boards if board["port"] == port]
     return mp_boards
 
 
-def known_mp_boards(port: str, versions: Optional[List[str]] = None) -> List[Tuple[str, str]]:
+def known_stored_boards(port: str, versions: Optional[List[str]] = None) -> List[Tuple[str, str]]:
     """
     Returns a list of tuples with the description and board name for the given port and version
 
     port : str : The Micropython port to filter for
     versions : List[str] : The Micropython versions to filter for (actual versions required)
     """
-    mp_boards = get_mp_boards_for_port(port, versions)
+    mp_boards = get_stored_boards_for_port(port, versions)
 
-    boards = set(
-        {(f'{board["description"]} [board["board"]] {board["version"]}', board["board"]) for board in mp_boards}
-    )
+    boards = set({(f'{board["version"]} {board["description"]}', board["board"]) for board in mp_boards})
     return sorted(list(boards))
 
 
-def find_mp_board(board: str) -> Board:
-    """Find the board for the given board"""
-    info = read_boardinfo()
+@lru_cache(maxsize=20)
+def find_stored_board(board_id: str) -> Board:
+    """Find the board for the given board_ID or 'board description' and return the board info as a Board object"""
+    info = read_stored_boardinfo()
     for board_info in info:
-        if board_info["board"] == board:
+        if board_id in (board_info["board"], board_info["description"]):
             if "cpu" not in board_info or not board_info["cpu"]:
                 if " with " in board_info["description"]:
                     board_info["cpu"] = board_info["description"].split(" with ")[-1]
                 else:
                     board_info["cpu"] = board_info["port"]
             return board_info
-    raise LookupError(f"Board {board} not found")
+    raise MPFlashError(f"Board {board_id} not found")
```

### Comparing `mpflash-0.5.0/mpflash/mpboard_id/board_info.csv` & `mpflash-0.6.0/mpflash/mpboard_id/board_info.csv`

 * *Files identical despite different names*

### Comparing `mpflash-0.5.0/mpflash/mpboard_id/board_info.json` & `mpflash-0.6.0/mpflash/mpboard_id/board_info.json`

 * *Files identical despite different names*

### Comparing `mpflash-0.5.0/mpflash/mpremoteboard/mpy_fw_info.py` & `mpflash-0.6.0/mpflash/mpremoteboard/mpy_fw_info.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.5.0/mpflash/mpremoteboard/runner.py` & `mpflash-0.6.0/mpflash/mpremoteboard/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 def run(
     cmd: List[str],
     timeout: int = 60,
     log_errors: bool = True,
     no_info: bool = False,
     *,
+    log_warnings: bool = False,
     reset_tags: Optional[LogTagList] = None,
     error_tags: Optional[LogTagList] = None,
     warning_tags: Optional[LogTagList] = None,
     success_tags: Optional[LogTagList] = None,
     ignore_tags: Optional[LogTagList] = None,
 ) -> Tuple[int, List[str]]:
     # sourcery skip: no-long-functions
@@ -89,15 +90,16 @@
             encoding="utf-8",
         )
     except FileNotFoundError as e:
         raise FileNotFoundError(f"Failed to start {cmd[0]}") from e
 
     def timed_out():
         proc.kill()
-        log.warning(f"Command {cmd} timed out after {timeout} seconds")
+        if log_warnings:
+            log.warning(f"Command {cmd} timed out after {timeout} seconds")
 
     timer = Timer(timeout, timed_out)
     try:
         timer.start()
         # stdout has most of the output, assign log categories based on text tags
         if proc.stdout:
             for line in proc.stdout:
@@ -119,14 +121,16 @@
                     log.warning(line)
                 elif any(tag in line for tag in success_tags):
                     log.success(line)
                 elif any(tag in line for tag in ignore_tags):
                     continue
                 else:
                     if not no_info:
+                        if line.startswith(("INFO  : ", "WARN  : ", "ERROR : ")):
+                            line = line[8:].lstrip()
                         log.info(line)
         if proc.stderr and log_errors:
             for line in proc.stderr:
                 log.warning(line)
     except UnicodeDecodeError as e:
         log.error(f"Failed to decode output: {e}")
     finally:
```

### Comparing `mpflash-0.5.0/mpflash/vendored/dfu.py` & `mpflash-0.6.0/mpflash/vendor/dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.5.0/mpflash/vendored/pydfu.py` & `mpflash-0.6.0/mpflash/vendor/pydfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.5.0/pyproject.toml` & `mpflash-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpflash"
-version = "0.5.0"
+version = "0.6.0"
 description = "Flash and download tool for MicroPython firmwares"
 authors = ["Jos Verlinde <jos_verlinde@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["MicroPython", "firmware", "flash", "download", "UF2", "esptool"]
 homepage = "https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md"
 repository = "https://github.com/Josverl/micropython-stubber"
```

### Comparing `mpflash-0.5.0/README.md` & `mpflash-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 
 mpflash has been tested on Windows x64, Linux X64 and ARM64, but not (yet) macOS.
 
 ## Features
  1. List the connected boards including their firmware details, in a tabular or json format
  2. Download MicroPython firmware for specific boards and versions.
  3. Flash one or all connected MicroPython boards with a specific firmware or version.
-    Tested ports: rp2, samd, esp32, esp32s3, esp8266 and stm32 (requires cubeprogrammer)
+    Tested ports: rp2, samd, esp32, esp32s3, esp8266 and stm32
  
 ## Installation
 To install mpflash, you can use pip: `pip install mpflash`
 
 ## Basic usage
 You can use mpflash to perform various operations on your MicroPython boards. Here is an example of basic usage:
 
 | Command | Description |
 |---------|-------------|
 | `mpflash list` | List the connected board(s) including their firmware details |
 | `mpflash download` | Download the MicroPython firmware(s) for the connected board(s) |
 | `mpflash flash` | Flash the latest stable firmware to the connected board(s) |
 
 
-## Linux permissions for usb devices 
+## Linux permissions to access usb devices 
 In order to flash the firmware to the board, you need to have the correct permissions to access the USB devices.
 On Windows this will not be an issue, but on Linux you can use  udev rules to give non-root users access to the USB devices.
-[See thestm32_permissions documentation](./stm32_udev_rules.md) for more information.
+[See the stm32_permissions documentation](./stm32_udev_rules.md) for more information.
 
 
 ## Advanced use
 You can list the connected boards using the following command:
 ```bash
 $ mpflash list
 D:\MyPython\micropython-stubber> mpflash list
```

### Comparing `mpflash-0.5.0/PKG-INFO` & `mpflash-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpflash
-Version: 0.5.0
+Version: 0.6.0
 Summary: Flash and download tool for MicroPython firmwares
 Home-page: https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md
 License: MIT
 Keywords: MicroPython,firmware,flash,download,UF2,esptool
 Author: Jos Verlinde
 Author-email: jos_verlinde@hotmail.com
 Requires-Python: >=3.8.1,<4.0
@@ -44,33 +44,33 @@
 
 mpflash has been tested on Windows x64, Linux X64 and ARM64, but not (yet) macOS.
 
 ## Features
  1. List the connected boards including their firmware details, in a tabular or json format
  2. Download MicroPython firmware for specific boards and versions.
  3. Flash one or all connected MicroPython boards with a specific firmware or version.
-    Tested ports: rp2, samd, esp32, esp32s3, esp8266 and stm32 (requires cubeprogrammer)
+    Tested ports: rp2, samd, esp32, esp32s3, esp8266 and stm32
  
 ## Installation
 To install mpflash, you can use pip: `pip install mpflash`
 
 ## Basic usage
 You can use mpflash to perform various operations on your MicroPython boards. Here is an example of basic usage:
 
 | Command | Description |
 |---------|-------------|
 | `mpflash list` | List the connected board(s) including their firmware details |
 | `mpflash download` | Download the MicroPython firmware(s) for the connected board(s) |
 | `mpflash flash` | Flash the latest stable firmware to the connected board(s) |
 
 
-## Linux permissions for usb devices 
+## Linux permissions to access usb devices 
 In order to flash the firmware to the board, you need to have the correct permissions to access the USB devices.
 On Windows this will not be an issue, but on Linux you can use  udev rules to give non-root users access to the USB devices.
-[See thestm32_permissions documentation](./stm32_udev_rules.md) for more information.
+[See the stm32_permissions documentation](./stm32_udev_rules.md) for more information.
 
 
 ## Advanced use
 You can list the connected boards using the following command:
 ```bash
 $ mpflash list
 D:\MyPython\micropython-stubber> mpflash list
```

