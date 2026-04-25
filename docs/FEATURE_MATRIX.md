# Feature Matrix

This matrix describes major SharpMTKClient source-code areas. Availability depends on chipset, boot mode, selected DA, firmware package, security state and licensed package scope.

## Protocol Families

| Area | Description |
| --- | --- |
| LEGACY | Classic DA-based MediaTek protocol flow for supported legacy devices. |
| XFLASH | Modern DA workflow with native partition operations and faster flash paths where supported. |
| XML | MTK V6 / XML command workflow for supported firmware packages and device modes. |

## Device and Boot Flow

| Feature | Status |
| --- | --- |
| VID / PID MediaTek port detection | Included where supported |
| USB plug / unplug event handling | Included where supported |
| BROM service detection | Included where supported |
| BROM handshake | Included where supported |
| Preloader communication | Included where supported |
| Hardware code and version parsing | Included where supported |
| Hardware sub-code parsing | Included where supported |
| Security flag parsing | Included where supported |
| MEID / SOCID reading | Device dependent |
| Watchdog handling | Device dependent |
| DA selection | Included where supported |
| Stage-1 / Stage-2 upload | Included where supported |
| EMI receive / send workflow | Device dependent |
| Connection status reporting | Included where supported |
| Operation log output | Included where supported |

## Flash and Partition Operations

| Feature | Status |
| --- | --- |
| Scatter firmware workflow | Included where supported |
| XML firmware workflow | Included where supported |
| Native XFLASH / XML flash | Included where supported |
| Raw partition read / write | Included where supported |
| Raw firmware flash | Included where supported |
| Sparse image handling | Included where supported |
| GPT read | Included where supported |
| GPT flash | Included where supported |
| GPT rebuild | Included where supported |
| Partition dump / backup | Included where supported |
| Partition erase | Included where supported |
| Full flash backup | Device dependent |
| Preloader read / write | Included where supported |
| Safe format | Device dependent |
| Manual format | Device dependent |
| FRP erase | Device dependent |
| Bootloader unlock / relock | Device dependent |
| Read / orange state fix | Device dependent |

## File-System and Android Data

| Feature | Status |
| --- | --- |
| EXT4 partition detection | Included where supported |
| EXT4 browse and extraction | Included where supported |
| EXT4 file replace / delete / add | Package dependent |
| Logical partition / super parsing | Included where supported |
| Dynamic partition browsing | Included where supported |
| EROFS detection and read paths | Included where supported |
| F2FS detection and read paths | Included where supported |
| Android build.prop extraction | Included where supported |
| File and directory extraction | Included where supported |
| Raw image source handling | Included where supported |

## NV, IMEI, RPMB and Keys

| Feature | Status |
| --- | --- |
| NV backup | Included where supported |
| NV write | Device dependent |
| NV erase | Device dependent |
| NV item decode logic | Package dependent |
| IMEI read / repair source areas | Brand and mode dependent |
| Hardware key read paths | Device dependent |
| DXCC helper integration | Device dependent |
| SEJ / GCPU helper integration | Device dependent |
| AES helper paths | Included where supported |
| RPMB read | Device dependent |
| RPMB write | Device dependent |
| RPMB erase | Device dependent |
| RPMB key read | Device dependent |

## Security and Research-Oriented Paths

| Feature | Status |
| --- | --- |
| SLA / DAA handling | Device dependent |
| Kamakiri workflow | Device dependent |
| HeapBait workflow | Device dependent |
| Carbonara workflow | Device dependent |
| Bootloader unlock / relock | Device dependent |
| Read / orange state fix | Device dependent |
| Permanent unlock development paths | Device dependent |
| FRP / format workflow code paths | Device dependent |
| Vbmeta / dm-verity patch paths | Device dependent |
| Brand-specific patch examples | Package dependent |

## Example Brand Workflow Areas

| Brand / Area | Notes |
| --- | --- |
| Samsung MTK | Selected service, NV, partition and authorization paths depending on model and package scope. |
| Motorola MTK | MTKV5 and MTKV6 workflow examples for supported chipsets and models. |
| Infinix MTK | MTKV5 and MTKV6 workflow examples where supported. |
| Honor / Vivo | Selected modern MTK workflow examples where supported. |
| Redmi / Xiaomi | Selected flash, partition, file-system and information read paths where supported. |
| TCL / Alcatel | Selected model-specific support paths where included. |

## Storage Targets

| Storage | Notes |
| --- | --- |
| EMMC | Supported where protocol and DA allow it. |
| UFS | Supported where protocol and DA allow it. |
| NAND | Supported where protocol and DA allow it. |
| NOR / SDMMC | Supported in selected paths where available. |
