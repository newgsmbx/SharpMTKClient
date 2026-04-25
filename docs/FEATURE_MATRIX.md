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
| BROM handshake | Included where supported |
| Preloader communication | Included where supported |
| Hardware code and version parsing | Included where supported |
| Security flag parsing | Included where supported |
| MEID / SOCID reading | Device dependent |
| Watchdog handling | Device dependent |
| DA selection | Included where supported |
| Stage-1 / Stage-2 upload | Included where supported |
| EMI receive / send workflow | Device dependent |

## Flash and Partition Operations

| Feature | Status |
| --- | --- |
| Scatter firmware workflow | Included where supported |
| XML firmware workflow | Included where supported |
| Native XFLASH / XML flash | Included where supported |
| Raw partition read / write | Included where supported |
| Sparse image handling | Included where supported |
| GPT read | Included where supported |
| GPT flash | Included where supported |
| GPT rebuild | Included where supported |
| Partition dump / backup | Included where supported |
| Partition erase | Included where supported |
| Preloader read / write | Included where supported |
| Safe format | Device dependent |
| Manual format | Device dependent |
| FRP erase | Device dependent |

## File-System and Android Data

| Feature | Status |
| --- | --- |
| EXT4 partition detection | Included where supported |
| EXT4 browse and extraction | Included where supported |
| EXT4 file replace / delete / add | Package dependent |
| Logical partition / super parsing | Included where supported |
| EROFS detection and read paths | Included where supported |
| F2FS detection and read paths | Included where supported |
| Android build.prop extraction | Included where supported |
| File and directory extraction | Included where supported |

## NV, IMEI, RPMB and Keys

| Feature | Status |
| --- | --- |
| NV backup | Included where supported |
| NV write | Device dependent |
| NV erase | Device dependent |
| NV item decode logic | Package dependent |
| IMEI read / repair source areas | Brand and mode dependent |
| Hardware key read paths | Device dependent |
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
| Vbmeta / dm-verity patch paths | Device dependent |
| Brand-specific patch examples | Package dependent |

## Storage Targets

| Storage | Notes |
| --- | --- |
| EMMC | Supported where protocol and DA allow it. |
| UFS | Supported where protocol and DA allow it. |
| NAND | Supported where protocol and DA allow it. |
| NOR / SDMMC | Supported in selected paths where available. |
