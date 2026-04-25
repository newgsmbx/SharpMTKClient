# SharpMTKClient

![SharpMTKClient banner](assets/sharpmtkclient-hero-v2.svg)

> Professional C# source code project for MediaTek / MTK protocol development on Windows.

[![Product Type](https://img.shields.io/badge/product-source%20code-blue)](#)
[![Language](https://img.shields.io/badge/language-C%23-68217A)](#)
[![Platform](https://img.shields.io/badge/platform-Windows-0078D4)](#)
[![Protocols](https://img.shields.io/badge/protocols-LEGACY%20%7C%20XFLASH%20%7C%20XML-green)](#)
[![Audience](https://img.shields.io/badge/audience-developers%20%7C%20researchers%20%7C%20software%20owners-purple)](#)

## Overview

**SharpMTKClient** is a Windows GUI source-code project written in C# by Alephgsm for MediaTek chipset devices.

The project is designed for developers, researchers and software owners who want a private MTK service software foundation instead of a closed binary. The full commercial source code is provided privately to licensed buyers only.

SharpMTKClient supports MTK protocol workflows including BROM / Preloader communication, Download Agent handling, LEGACY, XFLASH and MTK V6 XML operations, firmware flashing, partition management, file-system access, NV / IMEI logic, RPMB paths and advanced patch/service modules.

USB communication is based on Windows APIs. It has no UsbDk dependency; libusb is used only for selected `ControlTransfer` paths.

Product page: <https://alephgsm.com/2022/01/13/csharp-mtkclient/>

Contact: <https://t.me/GsmCoder>

## Core Protocol Families

| Protocol | Purpose |
| --- | --- |
| **LEGACY** | Classic DA-based MediaTek workflow. |
| **XFLASH** | Modern DA workflow with native partition-oriented operations. |
| **XML** | MTK V6 / XML command flow for supported firmware packages and modes. |

Protocol availability depends on chipset, selected DA, boot mode, security state and target operation.

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

## Public Update Highlights

### 2026.02.21

* Added patch cert.
* Added IMEI Repair for selected Vivo, Xiaomi, OPPO, Infinix, Tecno and Itel targets.
* Added Payjoy, Huawei ID, OPPO ID, no efuse state, DM corrupted and security plugin workflows.
* Added OTA, MDM, Walock, SIM Lock / MDM, modem patch, persist patch, demo remove and Vbmeta patch workflows.
* Updated HeapBait protocol and optimized protocol.

### 2026.02.13

* Added read IMEI info from device in all operations from `nvdata` and `ld0b`.
* Added decrypt NV items.
* Added IMEI repair for IMEI1 / IMEI2 in FlashMode.
* Added Mi Account disable paths.
* Added permanent bootloader unlock.

### 2026.02.10

* Added HeapBait exploit workflow.
* Added selected Infinix chipset support paths.
* Added new keys for Motorola, Xiaomi and AOT paths.
* Optimized and fixed XML protocol issues.

![SharpMTKClient 2026 update screenshot](https://alephgsm.com/wp-content/uploads/2022/01/Screenshot-2026-02-10-174646.png)

### 2025.12.25

* Added partition explorer for EROFS, F2FS and EXT4FS.
* Updated EROFS algorithm.
* Added rename, replace, delete and copy-to-local file workflows inside readable partitions.
* Updated protocol areas.

Video: <https://youtu.be/a5HE8kyOKfU?si=aC3T7rvYiMM2NAQN>

### 2025.10.27

* Added EROFS partitions.
* Added F2FS partitions.
* Added raw and sparse image handling from device and file.
* Optimized and fixed protocol issues.

### 2025.09.23

* Added native C# EXT4 stream reader and writer.
* Added logical partition and `super.img` browsing.
* Added file and directory extraction from EXT4 partitions.
* Added replace, delete and add file workflows for EXT4.
* Added `build.prop` parser from system or super partition.

Video: <https://alephgsm.com/wp-content/uploads/2022/01/VID_20250923_055602_985.mp4>

### 2025.06.07

* Updated RPMB erase and write paths.
* Added vendor selection tab.
* Added selected Samsung, Motorola, Infinix, Honor, Vivo, Redmi and TCL workflow examples.
* Updated MTKV6 commands.

Video: <https://youtu.be/wMd3SnQVEt8>

### 2025.04.12

* Added read and write RPMB for V6 devices.
* Added native XML firmware write paths.
* Added flash partition by name for XML and XFLASH.
* Updated DA2 patch, CPU list and MTKV6 protocol.

Video: <https://www.youtube.com/watch?v=7Nz4s8QR5SM>

### 2025.04.06

* Added native MTKV6 firmware flash through `flash.xml` and scatter.
* Updated legacy protocol.
* Fixed and optimized protocol areas.

## Screenshots From Code

![SharpMTKClient code screenshot 1](https://alephgsm.com/wp-content/uploads/2022/01/2-1.jpg)

![SharpMTKClient code screenshot 2](https://alephgsm.com/wp-content/uploads/2022/01/4.jpg)

![SharpMTKClient code screenshot 3](https://alephgsm.com/wp-content/uploads/2022/01/5.jpg)

![SharpMTKClient code screenshot 4](https://alephgsm.com/wp-content/uploads/2022/01/6.jpg)

## Screenshots From Interface

![SharpMTKClient interface screenshot 1](https://alephgsm.com/wp-content/uploads/2022/01/Screenshot-2025-04-12-072352.png)

![SharpMTKClient interface screenshot 2](https://alephgsm.com/wp-content/uploads/2022/01/Screenshot-2025-04-12-072654.png)

![SharpMTKClient interface screenshot 3](https://alephgsm.com/wp-content/uploads/2022/01/Screenshot-2025-04-12-072713.png)

![SharpMTKClient interface screenshot 4](https://alephgsm.com/wp-content/uploads/2022/01/Screenshot-2025-04-12-072727.png)

![SharpMTKClient interface screenshot 5](https://alephgsm.com/wp-content/uploads/2022/01/Screenshot-2025-04-12-072739.png)

## Documentation

* [Feature Matrix](docs/FEATURE_MATRIX.md)
* [Advanced Service Features](docs/ADVANCED_SERVICE_FEATURES.md)
* [Architecture](docs/ARCHITECTURE.md)
* [Module Catalog](docs/MODULE_CATALOG.md)
* [Buyer Guide](docs/BUYER_GUIDE.md)
* [Support Policy](docs/SUPPORT_POLICY.md)

## Repository Notice

This public repository is for **product presentation only**.

It may include:

* README and product documentation.
* Feature descriptions.
* Demo links and media references.
* Contact and licensing information.

It does not include:

* Full commercial source code.
* Private protocol implementation.
* Payloads, loaders or protected assets.
* Sensitive security research files.
* Licensed customer-only material.

## Licensing and Purchase

The full SharpMTKClient source code is available by private licensing.

Commercial usage rules are described in [LICENSE_TERMS.md](LICENSE_TERMS.md).

For pricing, licensing terms, technical questions or purchase requests, contact:

<https://t.me/GsmCoder>

Product page:

<https://alephgsm.com/2022/01/13/csharp-mtkclient/>

## Disclaimer

SharpMTKClient is intended for developers, research teams and authorized service software development. Device operations may depend on chipset, boot mode, selected DA, firmware package, security state and local regulations.

Use this project only for lawful development, research, maintenance and authorized service scenarios.
