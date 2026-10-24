# OpenCreate Design

**OpenCreate Design 是一个面向产品、设计与创意工作的 AI 协作创作空间。** 你可以围绕一个项目与 AI 编码代理协作，把想法逐步变成可预览、可迭代的设计产物，而不必在多个工具之间反复切换。

本仓库用于发布 OpenCreate Design Community Edition（CE）的桌面安装包和使用说明；应用源码不在此仓库中提供。

## 你可以用它做什么

- **从想法开始制作交互式原型**：描述目标和需求，与 AI 代理一起创建 Web 体验，在工作区中预览并继续修改。
- **让设计遵循品牌规范**：使用设计系统、品牌资产与设计模板，为原型和创作内容提供一致的视觉基础。
- **制作演示文稿**：生成和迭代演示文稿，检查页面与讲稿，并按需要导出。
- **创作图像与视频内容**：在项目中生成、查看和整理图像素材；结合兼容的模型与工作流制作视频和动态视觉内容。
- **在同一项目中持续协作**：通过对话推进任务，查看预览与文件，并在已有成果上继续迭代。
- **连接你熟悉的 AI 工具**：OpenCreate Design 面向 AI 编码代理构建，可与受支持的代理及工作流协作。部分代理、模型或生成能力需要单独安装、登录或配置相应服务。

具体可用的代理、模型和生成服务取决于你的环境与服务商配置。

## 下载 v0.0.2

| 平台 | 安装包 | 支持设备 |
|---|---|---|
| macOS | [OpenCreate-Design-v0.0.2-mac-arm64.dmg](https://github.com/LIBERSEEK/OpenCreate-Design-CE/releases/download/v0.0.2/OpenCreate-Design-v0.0.2-mac-arm64.dmg) | Apple 芯片（arm64） |
| Windows | [OpenCreate-Design-v0.0.2-win-x64-setup.exe](https://github.com/LIBERSEEK/OpenCreate-Design-CE/releases/download/v0.0.2/OpenCreate-Design-v0.0.2-win-x64-setup.exe) | 64 位 Windows（x64） |

安装后的应用名称为 **OpenCreate Design**。Intel 芯片 Mac 和 Linux 暂无此版本的预编译安装包。

更多版本和本次更新内容见 [v0.0.2 Release](https://github.com/LIBERSEEK/OpenCreate-Design-CE/releases/tag/v0.0.2)。

## 安装

### macOS

1. 下载上方 `.dmg` 文件并打开。
2. 将 **OpenCreate Design** 拖入“应用程序”（Applications）文件夹。
3. 从“应用程序”文件夹启动应用。

此版本的 macOS 安装包未使用 Apple Developer ID 签名，也未经 Apple 公证。首次打开若被 macOS 拦截，可先尝试打开一次，再前往“系统设置 → 隐私与安全性”，在安全性提示中选择“仍要打开”。系统版本或设备管理策略可能影响该选项是否显示；可参考 [Apple 官方说明](https://support.apple.com/zh-cn/102445)。

### Windows

下载并运行上方的 `.exe` 安装程序，按安装向导完成安装，然后启动 **OpenCreate Design**。

## 校验下载文件

Release 提供 SHA-256 校验文件。下载安装包和对应的 `.sha256` 文件后，可在文件所在目录执行：

macOS：

```bash
shasum -a 256 -c OpenCreate-Design-v0.0.2-mac-arm64.dmg.sha256
```

Windows PowerShell：

```powershell
(Get-FileHash .\OpenCreate-Design-v0.0.2-win-x64-setup.exe -Algorithm SHA256).Hash.ToLower()
```

Windows 上将命令输出与 Release 中 `.exe.sha256` 文件里的哈希值比较。

## 更新

CE 当前未启用应用内自动更新。后续版本发布后，请从 [Releases 页面](https://github.com/LIBERSEEK/OpenCreate-Design-CE/releases) 手动下载并安装。
