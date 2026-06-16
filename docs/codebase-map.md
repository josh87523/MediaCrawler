# MediaCrawler Codebase Map

> 用于人和 AI 快速定位产品逻辑、运行逻辑和对应代码入口。先读 `docs/business-product-logic.md`，再按下表跳到具体模块。

## Module Entrypoints

| Area | Entry | Notes |
|---|---|---|
| 业务逻辑 | `docs/business-product-logic.md` | 多平台自媒体采集框架边界 |
| 项目入口 | `README.md, README_en.md` | 框架能力、支持平台和运行方式 |
| 统一入口 | `main.py, cmd_arg/` | 命令行参数和采集启动入口 |
| 采集平台 | `media_platform/` | 小红书、抖音、快手、B站、微博、贴吧、知乎等平台实现 |
| API 服务 | `api/` | Web/API 封装、routers、schemas 和 services |
| 配置 | `config/` | 平台配置、数据库配置和运行参数 |
| 存储模型 | `store/, model/, database/` | 平台数据模型、存储适配和数据库层 |
| 代理/缓存 | `proxy/, cache/` | 代理池、缓存和网络辅助层 |
| 文档 | `docs/项目架构文档.md, docs/项目代码结构.md` | 架构、代码结构和使用说明 |

## Reading Contract

- 先用 `docs/business-product-logic.md` 判断这个仓库解决什么问题。
- 再按本页定位到代码或运行入口，避免从文件名猜产品逻辑。
- dated plan、archive、runtime data、generated output 只能当证据或历史参考，不能直接当当前运行合同。
- 涉及外部平台、账号、发布、支付、浏览器 profile 或凭证时，必须读真实运行面和权限边界，不能只读源码。

## Recommended First Read

1. `docs/business-product-logic.md`
2. `README.md`
3. `docs/项目架构文档.md`
4. `main.py`
5. `media_platform/`
