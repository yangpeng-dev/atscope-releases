# ATScope releases

[English](README.md) | 中文

ATScope 的发布包。ATScope 用来查看 Apple ATS（Accessory Test System）抓包，
也可以通过 USB 从 iPhone 实时抓取蓝牙和 Wi-Fi 流量。

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
