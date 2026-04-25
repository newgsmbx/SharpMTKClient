# Advanced Service Features

This document lists advanced service, patch and Patch [1] workflow areas described for SharpMTKClient. Exact availability depends on licensed package scope, target chipset, firmware, boot mode, security state, selected DA and operation requirements.

All workflows are intended for lawful development, authorized device maintenance, internal service tooling and research by qualified teams.

## Patch Certificate and Account Workflows

| Feature | Notes |
| --- | --- |
| Patch cert | Selected OPPO / Xiaomi workflows where supported. |
| Disable Mi Account | System, APK and hosts based paths where supported. |
| Mi Account + Global | Selected `cust` / `opcust` paths where supported. |
| Mi Account Remove + Convert Global V2 | Device and firmware dependent. |
| Reset Huawei ID | Device and firmware dependent. |
| Reset OPPO ID | Device and firmware dependent. |
| Remove security plugin | Device and firmware dependent. |

## OTA, MDM, Payjoy and Lock Workflows

| Feature | Notes |
| --- | --- |
| OTA Remove | Selected OPPO / Realme / OnePlus workflows where supported. |
| Xiaomi OTA Remove | Device and firmware dependent. |
| MDM + OTA Remove | Device and firmware dependent. |
| MDM Remove | Device and firmware dependent. |
| Walton MDM / Walock Remove | Selected Walton workflows where supported. |
| Nothing / CMF SIM Lock / MDM Remove | Selected Nothing / CMF workflows where supported. |
| Payjoy Remove | Device and firmware dependent. |
| Payjoy Remove through `oeminfo` | Selected paths where supported. |
| IT Admin / Network / Payjoy Unlock | Device and firmware dependent. |

## Patch and Repair Workflows

| Feature | Notes |
| --- | --- |
| Modem Patch | Xiaomi anti-relock paths where supported. |
| Persist Patch | Device and firmware dependent. |
| Demo Remove | Device and firmware dependent. |
| Restore Vbmeta | Security ON paths where supported. |
| Vbmeta Patch V1 / V2 / V3 | Security OFF paths where supported. |
| Fix no efuse state | Device and firmware dependent. |
| Fix DM corrupted | Device and firmware dependent. |
| Fix read / orange state | Device dependent after bootloader unlock. |

## IMEI, NV and Identity Workflows

| Feature | Notes |
| --- | --- |
| Read IMEI info | Supported paths can read from `nvdata`, `ld0b` or device-specific sources. |
| Decrypt NV items | Package and target dependent. |
| IMEI repair | Selected Vivo, Xiaomi, OPPO, Infinix, Tecno, Itel and Samsung MTK paths. |
| FlashMode IMEI repair | Universal and selected Samsung MT67xx paths where supported. |
| NV backup / write / erase | Device and operation dependent. |
| Hardware key read | Device and protocol dependent. |

## Exploit and Authorization Workflow Areas

| Feature | Notes |
| --- | --- |
| SLA / DAA handling | Device, security state and package dependent. |
| Kamakiri workflow | Device dependent. |
| HeapBait workflow | Device dependent. |
| Carbonara workflow | Device dependent. |
| SLA key handling | Brand and model dependent. |
| New chipset support paths | Package and target dependent. |

## Device Families Mentioned in Public Feature History

Public SharpMTKClient feature history mentions selected workflow areas for:

* Vivo.
* Xiaomi / Redmi.
* OPPO / Realme / OnePlus.
* Infinix.
* Tecno.
* Itel.
* Samsung MTK.
* Motorola.
* Honor.
* Huawei.
* TCL / Alcatel.
* Walton.
* Nothing / CMF.

Support for any specific model must be confirmed before purchase.
