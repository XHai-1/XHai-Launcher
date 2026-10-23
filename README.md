# XHai Launcher

<div align="center">
  <img src="logo.png" width="160" alt="XHai Launcher">
</div>

<p align="center">一个轻量的 Minecraft: Java Edition 启动器 · 单个 exe · 免安装 · 开源（GPL-3.0）</p>

---

## 简介

XHai Launcher 是 Windows 上的第三方 Minecraft: Java Edition 启动器，以单个 `.exe` 分发，
放进任意文件夹双击即可使用，不写注册表、不安装任何组件。

本项目基于开源项目 [OpenLauncher](https://github.com/OpenLauncher-MC/OpenLauncher)（GPL-3.0）改编，
保留了其去中心化的设计思路：游戏本体、加载器（Forge / NeoForge / Fabric / Quilt）与 Mod
全部直接从官方源和公益镜像获取，启动器本身不内置任何版本号，也不收集任何用户数据。

## 功能

- **启动**：一键启动、自动补全缺失文件、自动选择或下载合适的 Java、自动分配内存、版本隔离、自定义窗口标题与大小、启动后自动进服、实时游戏日志
- **账号**：离线账号、微软正版登录（需自备 Azure Client ID，见下）、外置登录（authlib-injector，如 LittleSkin / Blessing Skin）
- **下载游戏**：正式版 / 快照 / 远古版 / 愚人节版；Forge、NeoForge、Fabric（可同时装 Fabric API）、Quilt、OptiFine
- **社区资源**：Modrinth + CurseForge 双源搜索 Mod / 整合包 / 资源包 / 光影包 / 数据包，自动补齐前置 Mod
- **整合包**：导入 Modrinth（`.mrpack`）与 CurseForge（`.zip`），导出为 `.mrpack`
- **管理**：多游戏目录、版本重命名 / 删除、Mod 启停与批量更新、资源包 / 光影 / 存档 / 截图管理
- **崩溃分析**：识别内存不足、Java 版本不符、缺失前置、重复 Mod、Mixin 冲突、显卡驱动等常见原因并给出建议

## 下载与使用

1. 下载 `XHai启动器.exe`，放进一个**空文件夹**
2. 双击运行（Windows 10 / 11 自带 .NET Framework 4.8，无需另装）
3. 配置与账号保存在 exe 旁的 `XHai` 文件夹，游戏文件默认在 `.minecraft`
4. 已有游戏文件可用「版本选择 → 添加已有的游戏目录」直接导入官方启动器 / PCL / HMCL 的 `.minecraft`

> 若 Windows 弹出「已保护你的电脑」，点 **更多信息 → 仍要运行** 即可（程序未购买代码签名证书）。

### 微软正版登录

启动器不内置 Azure Client ID（避免所有用户共用一个 ID 而集体失效）。
需要微软正版登录时，请自行在 Azure 注册应用，并将 **应用程序(客户端) ID**
填入「设置 → 账户 → 微软登录 Client ID」，且该 ID 需通过 Mojang 的
Java Edition Game Service API 审核。

在此之前，可使用**离线账号**或**外置登录**（皮肤站）游玩。

## 开源协议

本项目基于 [OpenLauncher](https://github.com/OpenLauncher-MC/OpenLauncher) 改编，
遵循 **GPL-3.0** 协议发布，完整条款见 [LICENSE.txt](LICENSE.txt)。

Minecraft 是 Mojang AB 的商标，本项目与 Mojang、Microsoft 无关。
镜像服务由 BMCLAPI（bangbang93）、MCIM 等社区成员公益提供，请合理使用。
