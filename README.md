# SharpMTKClient

> Professional C# source code project for MediaTek / MTK protocol development on Windows.

## Overview

**SharpMTKClient** is a developer-focused C# / .NET source code project for building MediaTek / MTK software on Windows.

This repository is a public product showcase. It does not contain the commercial source code package. The full project is available through private licensing for developers, software owners, research teams and companies that want to build, customize or extend their own MTK service software.

The project focuses on MTK protocol workflows including device initialization, BROM / Preloader communication, Download Agent handling, flash operations, partition management, file-system access, NV / IMEI logic, RPMB paths and advanced research-oriented modules.

Official product page:

<https://alephgsm.com/2022/01/13/csharp-mtkclient/>

Contact:

<https://t.me/GsmCoder>

## Important Positioning

SharpMTKClient is **not** a simple compiled end-user repair tool.

It is a **source code product** for:

* C# / .NET developers who need a MediaTek protocol codebase.
* Software owners building a private MTK service product.
* Research teams studying MTK protocol behavior.
* Companies that need internal Windows tooling around MTK workflows.
* Developers who want branding, customization, licensing and private workflow control.

If your goal is to own and develop your own MTK software instead of depending on a closed binary, this project is designed for that use case.

## Documentation

* [Feature Matrix](docs/FEATURE_MATRIX.md)
* [Buyer Guide](docs/BUYER_GUIDE.md)
* [Compile and Debug Guide](docs/COMPILE_AND_DEBUG_GUIDE.md)
* [Support Policy](docs/SUPPORT_POLICY.md)
* [Media Kit](docs/MEDIA_KIT.md)
* [Links](docs/LINKS.md)

## Core Protocol Families

SharpMTKClient includes implementation paths for the major MediaTek workflow families:

| Protocol | Purpose |
| --- | --- |
| **LEGACY** | Classic MediaTek DA-based flow used on supported older and legacy devices. |
| **XFLASH** | Modern DA workflow with native partition-oriented operations and faster flash paths where supported. |
| **XML** | MTK V6 / XML command flow used by supported firmware packages and device modes. |

Protocol availability depends on chipset, selected DA, boot mode, security state and target operation.

## Main Feature Areas

### Device Connection and Initialization

* MediaTek port detection by VID / PID and USB plug / unplug events.
* BROM and Preloader communication workflow.
* Handshake and device information reading.
* Hardware code, hardware sub-code, hardware version, software version and security flag parsing.
* MEID / SOCID read paths where available.
* Watchdog handling where supported.
* DA selection logic.
* Stage-1 and Stage-2 DA upload flow.
* EMI receiving and sending workflow.
* Storage information detection for EMMC, UFS, NAND, NOR and SDMMC paths where supported.
* Windows native USB communication paths based on Windows APIs, with optional libusb usage for selected authorization paths.

### Download Agent and Stage Flow

* DA parser and loader metadata handling.
* Preloader parser and read / write logic.
* DA stage upload workflow.
* DA extension loading paths where available.
* Runtime configuration of flash type, page size, flash size and read size.
* Stage authentication related development paths where supported.
* Error handling around DA boot, reconnection and protocol mode changes.

### Firmware and Flash Operations

* Scatter firmware workflow.
* XML firmware workflow for supported MTK V6 packages.
* Native XFLASH / XML flash paths.
* Flash by partition name.
* Raw address-based read and write support.
* Raw and sparse image handling from device or file.
* Preloader read and write operations.
* GPT read, flash and rebuild paths.
* Download-only and firmware-upgrade style flows depending on protocol support.
* Progress reporting and logging integration.

### Partition and Storage Management

* GPT / partition table reading.
* Partition list parsing and display.
* Read selected partitions.
* Write selected partitions.
* Erase selected partitions.
* Full flash read path where supported.
* Partition lookup by name.
* Sector and size calculation helpers.
* Safe format and manual format workflows.
* FRP erase workflows.
* Support paths for EMMC, UFS and NAND targets where available.

### File Management and File-System Access

* Detect supported Android partitions.
* EXT4 stream read paths.
* EXT4 browse, extract, replace, delete and add file workflows where supported.
* Logical partition / `super` partition metadata handling.
* Dynamic partition browsing.
* EROFS detection and read paths where implemented.
* F2FS detection and read paths where implemented.
* Android `build.prop` extraction logic from supported partitions.
* File and directory extraction flows.

### NV, IMEI and Key-Related Modules

* NV partition backup, write and erase paths.
* NV item decode logic.
* LD0B / nvdata related IMEI development paths where supported.
* IMEI read and repair workflow source areas for selected modes and brands.
* Hardware key read paths where supported.
* DXCC / crypto-related integration points where available.
* AES and device crypto helper modules used by selected workflows.

### RPMB Development Paths

* RPMB read path where supported.
* RPMB write path where supported.
* RPMB erase path where supported.
* RPMB key read path where supported by mode and target.
* Protocol-specific RPMB integration points.

### Security, Patch and Research-Oriented Paths

* SLA / DAA related paths where supported.
* Kamakiri-style payload workflow where supported.
* HeapBait protocol path where supported.
* Carbonara stage authentication path where supported.
* Bootloader unlock and relock logic.
* Read / orange state fix paths after bootloader unlock where supported.
* Permanent unlock development paths for supported targets.
* FRP and format workflow code paths.
* Vbmeta / dm-verity patch logic where supported.
* Brand or model-specific patch workflow examples.

## Developer Value

SharpMTKClient is useful when you need more than a ready-made executable. The commercial package is intended to provide a foundation that can be studied, modified and integrated into your own business or research workflow.

Developers can use it to build:

* A branded MTK service software product.
* A private firmware flashing application.
* An internal device maintenance system.
* A research tool for MTK protocol analysis.
* A model-specific service workflow.
* A Windows C# application with custom UI and licensing.
* A commercial product based on private workflow requirements.

## Architecture Highlights

* C# / .NET Windows desktop codebase.
* WinForms-oriented GUI structure.
* Protocol-oriented module organization.
* Separate paths for LEGACY, XFLASH and XML workflows.
* DA parser and stage upload implementation.
* Native flash and partition command paths.
* MountCore-style file-system reader modules.
* File Management UI integration.
* Configurable UI and workflow logic.
* Suitable for private branding and commercial customization.

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

Default commercial usage rules are described in [LICENSE_TERMS.md](LICENSE_TERMS.md).

In short: licensed buyers may use the source code only in their own private/internal/commercial project. They may not resell it, exchange it with other teams, publish it for free, gift it to others, upload it publicly, or share it with third parties.

Support terms are described in [docs/SUPPORT_POLICY.md](docs/SUPPORT_POLICY.md). One year of minor updates and bug-fix support is included for licensed buyers by default, unless a separate written agreement says otherwise.

For pricing, licensing terms, technical questions or purchase requests, contact:

<https://t.me/GsmCoder>

Product page:

<https://alephgsm.com/2022/01/13/csharp-mtkclient/>

## Disclaimer

SharpMTKClient is intended for developers, research teams and authorized service software development. Device operations may depend on chipset, boot mode, selected DA, firmware package, security state and local regulations.

Use this project only for lawful development, research, maintenance and authorized service scenarios.
