# 墨稿工作台 · 发布仓库

本仓库仅用于存放 **墨稿工作台桌面版（Windows x64）** 的安装包与自动更新清单，不保存创作源码与作品数据。

## Release 资产说明

每个版本 Release 包含：

- `墨稿工作台-Setup-<version>.exe`：NSIS 安装包（可手动下载安装）
- `latest.json`：自动更新清单，字段为 `version` / `file` / `url` / `sha256`

## 更新机制

桌面客户端启动后读取本仓库最新 Release 的 `latest.json`，对比本地版本；检测到新版本后可一键静默更新，安装前校验 SHA-256。
