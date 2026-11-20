# atscope releases

[English](#english) | [中文](#中文)

## English

Release packages of atscope (ATS Viewer). The app checks this repository
for updates; the source code is maintained elsewhere.

| Platform | Package |
|---|---|
| macOS | `ATS-Viewer-<version>-<arch>.dmg` (install), `atscope-<version>-macos-<arch>.zip` (in-app update) |
| Windows | `atscope-<version>-windows-<arch>.zip` (portable, unzip and run) |
| Linux | `ats-viewer-<version>-linux-<arch>.AppImage`, `.deb`, `.rpm`, `.tar.gz` |

Every release carries `SHA256SUMS` and its minisign signature
`SHA256SUMS.minisig`. The app verifies both before installing an update.
To check a download by hand:

```sh
minisign -Vm SHA256SUMS -P RWRPEkF8Vr6wEMusaKr3XZ9GD8HiS35spynF6sCcDcYZ5M8t9n2WVlnj
shasum -a 256 -c SHA256SUMS --ignore-missing
```

## 中文

atscope（ATS Viewer）的发布包。程序从这个仓库检查更新，源码在其他地方维护。

| 平台 | 安装包 |
|---|---|
| macOS | `ATS-Viewer-<版本>-<arch>.dmg`（安装用）、`atscope-<版本>-macos-<arch>.zip`（程序内更新用） |
| Windows | `atscope-<版本>-windows-<arch>.zip`（便携版，解压即可运行） |
| Linux | `ats-viewer-<版本>-linux-<arch>.AppImage`、`.deb`、`.rpm`、`.tar.gz` |

每个 Release 都附带 `SHA256SUMS` 和它的 minisign 签名 `SHA256SUMS.minisig`，
程序安装更新前会验证这两项。手动校验下载的文件：

```sh
minisign -Vm SHA256SUMS -P RWRPEkF8Vr6wEMusaKr3XZ9GD8HiS35spynF6sCcDcYZ5M8t9n2WVlnj
shasum -a 256 -c SHA256SUMS --ignore-missing
```
