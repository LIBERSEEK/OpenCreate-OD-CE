# OpenCreate OD Community Edition

从 [GitHub Releases](https://github.com/LIBERSEEK/OpenCreate-OD-CE/releases) 下载最新的 macOS 安装包。本仓库用于提供安装包和使用说明。

## 下载与安装

当前版本为 [v0.0.1](https://github.com/LIBERSEEK/OpenCreate-OD-CE/releases/tag/v0.0.1)，适用于 Apple 芯片 Mac（arm64）。Intel Mac 暂不支持。

1. 下载 Release 中的 `.dmg` 文件。
2. 打开 DMG，将应用拖入“应用程序”（Applications）文件夹。
3. 从“应用程序”文件夹打开应用。

## 首次打开被 macOS 拦截

**当前版本没有 Developer ID 签名，也未经 Apple 公证，macOS 可能在首次打开时拦截应用。**

确认安装包来自本仓库的官方 Release 后，可按以下步骤操作：

1. 先尝试打开一次应用。
2. 打开“系统设置 → 隐私与安全性”。
3. 在安全性区域找到该应用的拦截提示，点击“仍要打开”（Open Anyway，如有显示）。
4. 按系统提示确认，必要时输入 Mac 登录密码或使用 Touch ID。

不同 macOS 版本或设备管理策略下，可用选项可能不同。若没有“仍要打开”，请参阅 [Apple 官方说明](https://support.apple.com/zh-cn/102445)。

## 文件校验与更新

Release 同时提供 `.dmg.sha256` 校验文件。在两个文件所在目录运行以下命令，可检查下载文件是否完整：

```bash
shasum -a 256 -c open-create-od-ce-0.0.1-mac-arm64.dmg.sha256
```

`v0.0.1` 暂未启用自动更新，请从本仓库的 Releases 下载后续版本。
