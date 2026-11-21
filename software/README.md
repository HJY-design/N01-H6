# N01 H6 软件参考

| 目录 | 内容 |
| --- | --- |
| [linux-mainline](linux-mainline/) | 基于 Linux 6.12.109 的 N01 设备树和通用调试配置。设备树引用同版本上游 H6 Orange Pi 公共描述。 |
| [u-boot](u-boot/) | U-Boot 2022.01 的板级设备树和 FEL 配置参考。720 MHz 配置的 `REPLACE_WITH_ROOT_PARTUUID` 需替换为自己的根分区标识。 |
| [openwrt](openwrt/) | OpenWrt 23.05.3 / Linux 5.15.150 的板级设备树、构建配置快照和 extlinux 示例。 |

这些文件用于理解 N01 的板级适配。完整构建还需要对应版本的上游源码、相应的 H6 DDR 初始化修改、启动固件和所用外设的固件。各系统的 U-Boot、内核、DTB 和根文件系统需要配套，按自己的分区调整启动配置。正文记录的实机结果对应当时的构建与样板。

FEL 启动实验从电脑把 SPL 和 U-Boot 装入内存，再由 U-Boot 从 USB 盘加载 `Image` 和 `/allwinner/sun50i-h6-n01.dtb`。Linux 调试配置曾将 RT5370 的 `rt2870.bin` 编入内核，重建该配置时从适用的上游固件包另行取得。

这里提供的是基于上游 Linux、U-Boot 和 OpenWrt 的板级材料，各设备树保留 SPDX 声明和上游署名。全志官方 Linux/Android BSP、基于 BSP 开展的修改和构建产物不在本仓库中。
