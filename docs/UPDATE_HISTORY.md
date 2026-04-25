# Update History

Public SharpMTKClient update highlights are kept here so the README remains compact.

## 2026.02.21

* Added patch cert.
* Added IMEI Repair for selected Vivo, Xiaomi, OPPO, Infinix, Tecno and Itel targets.
* Added remove Payjoy.
* Added reset Huawei ID.
* Added reset OPPO ID.
* Added fix no efuse state.
* Added fix DM corrupted.
* Added remove security plugin.
* Added OTA Remove for OPPO, Realme and OnePlus.
* Added Xiaomi OTA Remove.
* Added MDM + OTA Remove.
* Added MDM / Walock Remove for Walton.
* Added SIM Lock / MDM Remove for Nothing / CMF.
* Added Xiaomi anti-relock modem patch.
* Added Persist Patch.
* Added Demo Remove.
* Added Payjoy Remove through selected `oeminfo` paths.
* Added IT Admin / Network / Payjoy Unlock.
* Added Restore Vbmeta for Security ON paths.
* Added Vbmeta Patch V1 / V2 / V3 for Security OFF paths.
* Added Mi Account + Global through `cust` / `opcust` paths.
* Added Mi Account Remove + Convert Global V2.
* Updated HeapBait protocol.
* Optimized protocol.

## 2026.02.13

* Added read IMEI info from device in all operations from `nvdata` and `ld0b`.
* Added decrypt NV items.
* Added IMEI repair for IMEI1 / IMEI2 in FlashMode.
* Added universal and Samsung MT67xx key paths where supported.
* Added Mi Account disable paths through system, APK and hosts methods.
* Added permanent bootloader unlock.

## 2026.02.10

* Added HeapBait exploit workflow.
* Added selected Infinix chipset support paths for DA + exploit workflows.
* Added new key paths for Motorola, Xiaomi and AOT.
* Optimized and fixed XML protocol issues.

## 2025.12.25

* Added partition explorer for EROFS, F2FS and EXT4FS.
* Updated EROFS algorithm.
* Added rename, replace, delete and copy-to-local workflows inside readable partitions.
* Updated other protocol areas.

## 2025.10.27

* Added EROFS partition support paths.
* Added F2FS partition support paths.
* Added raw and sparse image handling from device and file.
* Optimized and fixed protocol issues.

## 2025.10.23

* Added Carbonara exploit in universal mode for selected supported devices.
* Added new keys for `handle_sla` paths.
* Added `build.prop` information read in supported features.
* Updated MTKV6 protocol.
* Fixed and optimized protocol areas.

## 2025.09.23

* Added native C# EXT4 stream reader and writer paths.
* Added EXT4 partition mount and file / directory listing.
* Added logical partition and `super.img` browsing paths.
* Added EXT4 item extraction from logical partitions.
* Added replace, delete and add file workflows for EXT4.
* Added EXT4 partition detection.
* Added `build.prop` parser from system or super partition.

## 2025.06.07

* Updated RPMB erase and write paths.
* Added vendor selection tab.
* Added selected Samsung, Motorola, Infinix, Honor, Vivo, Redmi and TCL workflow examples.
* Updated MTKV6 commands.

## 2025.04.12

* Added read RPMB for V6 devices.
* Added write RPMB for V6 devices.
* Added native XML firmware write paths: download, firmware upgrade and download-only.
* Added flash partition by name for XML and XFLASH.
* Updated DA2 patch.
* Updated CPU list.
* Updated MTKV6 protocol.

## 2025.04.06

* Added native MTKV6 firmware flash through `flash.xml` and scatter.
* Updated legacy protocol.
* Fixed and optimized protocol areas.
