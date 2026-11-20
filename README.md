# ATScope releases

[English](#english) | [中文](#中文)

## English

Release packages of ATScope, a viewer for Apple ATS (Accessory Test System)
captures that can also capture Bluetooth and Wi-Fi traffic live from an
iPhone over USB. The app checks this repository for updates; the source
code is maintained elsewhere.

| Platform | Package |
|---|---|
| macOS | `atscope-<version>-macos-<arch>.dmg` (install), `atscope-<version>-macos-<arch>.zip` (in-app update) |
| Windows | `atscope-<version>-windows-<arch>.zip` (portable, unzip and run) |
| Linux | `atscope-<version>-linux-<arch>.AppImage`, `atscope_<version>_<arch>.deb`, `atscope-<version>-1.<arch>.rpm`, `atscope-<version>-linux-<arch>.tar.gz` |

Every release carries `SHA256SUMS` and its minisign signature
`SHA256SUMS.minisig`. The app verifies both before installing an update.
To check a download by hand:

```sh
minisign -Vm SHA256SUMS -P RWRPEkF8Vr6wEMusaKr3XZ9GD8HiS35spynF6sCcDcYZ5M8t9n2WVlnj
shasum -a 256 -c SHA256SUMS --ignore-missing
```

## 中文

ATScope 的发布包。ATScope 用来查看 Apple ATS（Accessory Test System）抓包，
也可以通过 USB 从 iPhone 实时抓取蓝牙和 Wi-Fi 流量。程序从这个仓库检查更新，
源码在其他地方维护。

| 平台 | 安装包 |
|---|---|
| macOS | `atscope-<版本>-macos-<arch>.dmg`（安装用）、`atscope-<版本>-macos-<arch>.zip`（程序内更新用） |
| Windows | `atscope-<版本>-windows-<arch>.zip`（便携版，解压即可运行） |
| Linux | `atscope-<版本>-linux-<arch>.AppImage`、`atscope_<版本>_<arch>.deb`、`atscope-<版本>-1.<arch>.rpm`、`atscope-<版本>-linux-<arch>.tar.gz` |

每个 Release 都附带 `SHA256SUMS` 和它的 minisign 签名 `SHA256SUMS.minisig`，
程序安装更新前会验证这两项。手动校验下载的文件：

```sh
minisign -Vm SHA256SUMS -P RWRPEkF8Vr6wEMusaKr3XZ9GD8HiS35spynF6sCcDcYZ5M8t9n2WVlnj
shasum -a 256 -c SHA256SUMS --ignore-missing
```
