# Features

This document keeps the main SharpMTKClient feature list outside the README so the repository front page stays focused.

Feature availability depends on chipset, selected DA, boot mode, firmware package, security state and licensed package scope.

## Main Features

* MediaTek port detection by VID / PID and USB plug / unplug events.
* Device type support for LEGACY, XFLASH and XML workflows.
* UFS, NAND and EMMC support where DA and protocol allow it.
* Auto SLA / DAA handling paths where supported.
* Preloader crash / boot preparation paths where supported.
* MTKV5 and MTKV6 firmware flashing through scatter and `flash.xml`.
* Native XML firmware write paths: download, firmware upgrade and download-only.
* Flash by partition name.
* Raw firmware flash and raw / sparse image handling.
* Read Oxygen Forensics Detective dump paths where supported.
* GPT read, flash and rebuild.
* Dump, backup, write and erase partitions.
* Read and flash preloader.
* Safe format, manual format and FRP erase workflows.
* NV partition backup, write and erase paths.
* Bootloader unlock / relock and permanent unlock paths where supported.
* Fix read / orange state after bootloader unlock.
* RPMB read / write / erase and RPMB key read paths where supported.
* Hardware key read paths.
* DA / Preloader parser.
* Android `build.prop` extraction.
* File-system explorer for EXT4, EROFS and F2FS partitions.
* Native C# EXT4 stream reader / writer paths.
* Logical partition and `super.img` browsing paths.
* File browse, extract, rename, replace, delete and copy-to-local workflows where supported.
* Patch cert, account, MDM, OTA, Payjoy, Vbmeta and advanced patch workflows where supported.

## Advanced Patch / Service Features

* Patch cert.
* IMEI Repair for selected Vivo, Xiaomi, OPPO, Infinix, Tecno and Itel targets.
* Read IMEI information from `nvdata` and `ld0b`.
* Decrypt NV items.
* FlashMode IMEI repair for universal and Samsung MT67xx paths where supported.
* Remove Payjoy.
* Reset Huawei ID and OPPO ID.
* Disable Mi Account through system, APK and hosts methods where supported.
* Mi Account + Global using `cust` / `opcust` paths where supported.
* Mi Account Remove + Convert Global V2.
* OTA Remove for OPPO, Realme, OnePlus and Xiaomi.
* MDM + OTA Remove.
* MDM / Walock Remove for Walton.
* SIM Lock / MDM Remove for Nothing / CMF.
* Xiaomi anti-relock modem patch.
* Persist Patch and Demo Remove.
* Payjoy Remove through selected `oeminfo` paths.
* IT Admin / Network / Payjoy Unlock.
* Restore Vbmeta for Security ON paths.
* Vbmeta Patch V1 / V2 / V3 for Security OFF paths.
* Fix no efuse state, fix DM corrupted and remove security plugin.

## Security / Research Paths

* SLA / DAA handling paths where supported.
* Kamakiri workflow paths.
* HeapBait workflow paths.
* Carbonara workflow paths.
* New SLA key handling for selected Motorola, Xiaomi and AOT paths.
* Infinix DA + exploit paths for selected MT6789, MT6835, MT6855, MT6878, MT6886, MT6893, MT6895, MT6896, MT6897, MT6983, MT6985, MT6989 and MT6993 targets.
