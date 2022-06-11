# Hackintosh with OpenCore

Update: [OpenCore 0.8.1](https://github.com/acidanthera/OpenCorePkg)

## 0x00 Hardware

| Index | Name              | Model                                                                                                                                              |
|-------|-------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|
| 1     | CPU               | [i9-10850K](https://www.intel.cn/content/www/cn/zh/products/sku/205904/intel-core-i910850k-processor-20m-cache-up-to-5-20-ghz/specifications.html) |
| 2     | CPU Cooler        | [NZXT X63](https://nzxt.com/product/kraken-x63)                                                                                                    |
| 3     | Motherboard       | [MSI MEG Z490i Unify](https://cn.msi.com/Motherboard/MEG-Z490I-UNIFY/Specification)                                                                |
| 4     | RAM               | [Kingston Fury DDR4 3200 16GBx2](https://item.jd.com/100005089420.html)                                                                            |
| 5     | Solid State Drive | [SAMSUNG 970 EVO Plus 512G](https://item.jd.com/100003181110.html)                                                                                 |
| 6     | Power Supply      | [USCORSAIR SF600](https://www.corsair.com/us/en/Categories/Products/Power-Supply-Units/Power-Supply-Units-Advanced/SF-Series/p/CP-9020182-NA)      |
| 7     | Case              | [VECTOR-1 SE](https://item.taobao.com/item.htm?id=627430968966)                                                                                    |
| 8     | Monitor           | [DELL 2718QM](https://item.jd.com/4585499.html)                                                                                                    |
| 9     | Network Card      | [BCM943602CS](https://item.taobao.com/item.htm?id=608922155647)                                                                                    |

## 0x02 [Motherboard](https://cn.msi.com/Motherboard/MEG-Z490I-UNIFY/Specification)

### WIFI

Intel® AX201

- The Wireless module is pre-installed in the M.2 [Key-E] slot
- Supports MU-MIMO TX/RX, 2.4GHz/ 5GHz [160MHz] up to 2.4Gbps
- Supports 802.11ac
- WiFi 6
- Supports Bluetooth® 5.1, FIPS, FISMA

### LAN

Realtek® RTL8125B 2.5Gbps LAN controller

### AUDIO 

Realtek® ALC1220 Codec

- 7.1-Channel High Definition Audio
- Supports S/PDIF output

## 0x03 Status

目前用到的功能都完美。
- Monitor：4K，正常， HiDPI：正常
- WIFI：正常
- Bluetooth：正常
- AirDrop：可用
- Sleep/Resume：正常

## 0x03 BIOS Settings

TODO

## 0x04 Custom USB

|       | Index | USB2.0(USB1.1)   | USB3.0  |
|-------|:-----:|:----------------:|:-------:|
| 1     | a     | 12              |          |

![USB](USB.png)

## 0x04 Tools

### OpenCore

[OpenCore](https://github.com/acidanthera/OpenCorePkg)

### Drives

- [OpenCore](https://github.com/acidanthera/OpenCorePkg)
- [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- [Lilu](https://github.com/acidanthera/Lilu)
- [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
- [AppleALC](https://github.com/acidanthera/AppleALC)
- [LucyRTL8125Ethernet](https://github.com/Mieze/LucyRTL8125Ethernet)
- [USBInjectAll](https://github.com/RehabMan/OS-X-USB-Inject-All)

### Tools

- [HackintoshBuild](https://github.com/bugprogrammer/HackintoshBuild)
- [ProperTree](https://github.com/corpnewt/ProperTree)
- [MacInfoPkg](https://github.com/acidanthera/MacInfoPkg)
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
- [gibMacOS](https://github.com/corpnewt/gibMacOS)
- [MountEFI](https://github.com/corpnewt/MountEFI)
- [SSDTTime](https://github.com/corpnewt/SSDTTime)
- [balenaEtcher](https://github.com/balena-io/etcher/releases)
- [MaciASL](https://github.com/acidanthera/MaciASL/releases)

### Download

`python3 OC.py`


## 0x05 问题

水冷和网卡都需要用到USB2.0（9PIN），基于以上配置，可以把两个9PIN的接口保持线序列合二为一即可。当然也可以直接买内置USB2.0的HUB（主板USB2.0 9针转双9针一分二）。


## 0x06 感谢

1. [wjz304/Hackintosh-EFI-MSI-Z490i-Unify](https://github.com/wjz304/Hackintosh-EFI-MSI-Z490i-Unify)
1. [gngpp/MSI-MEG-Z490I-Unify-Hackintosh-OC-EFI](https://github.com/gngpp/MSI-MEG-Z490I-Unify-Hackintosh-OC-EFI)
1. [Hackintosh-MSI-MEG-z490i-UNIFY-OpenCore](https://github.com/H3C4T0M8/Hackintosh-MSI-MEG-z490i-UNIFY-OpenCore)


## 0xFF Reference

1. [MSI MEG Z490I Unify](https://cn.msi.com/Motherboard/MEG-Z490I-UNIFY/Specification)
1. [Comet Lake](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html)
1. [OpenCore Desktop Guide](https://dortania.github.io/OpenCore-Install-Guide/)
