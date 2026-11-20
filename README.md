# ATScope releases

English | [中文](README.zh-CN.md)

Release packages of ATScope, a viewer for Apple ATS (Accessory Test System)
captures that can also capture Bluetooth and Wi-Fi traffic live from an
iPhone over USB.

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
