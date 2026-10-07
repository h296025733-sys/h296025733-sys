# h296025733-sys

我做的项目大多从具体工作里的重复操作开始：整理视频素材、查看店铺数据、连接聊天与本地工具，再把这些步骤做成别人能理解和使用的应用。

最近主要在做 AI 影像创作、跨境电商数据与浏览器工具，也继续保留通信行业信息筛选和 Windows 本地自动化方面的项目。

## 可以先看这些

| 项目 | 做了什么 | 主要技术 |
| --- | --- | --- |
| [镜序 · AI 影像创作台](https://github.com/h296025733-sys/jingxu-director-workbench) | 把素材、创作规划、自动剪辑和交付管理放进同一个工作台；处理多人任务队列、权限与失败恢复。 | TypeScript / Next.js / Python |
| [飞书经营数据助手](https://github.com/h296025733-sys/feishu-data-assistant) | 在群聊中查询与更新经营数据。模型理解问题，统计、去重和更新规则由代码执行。 | TypeScript / 飞书 / 多租户 |
| [TikTok 达人助手](https://github.com/h296025733-sys/tiktok-daren-assistant) | 在浏览器里查看达人与视频数据，处理下载、评论翻译、字幕和页面切换后的状态隔离。 | Chrome 扩展 / TypeScript |
| [TikTok 达人内容分析](https://github.com/h296025733-sys/tiktok-creator-intelligence) | 从公开视频与证据整理商业内容信号，保留评分理由、失败恢复和缺失信息。 | Python / CLI / Codex skill |
| [Auto Video Lab](https://github.com/h296025733-sys/codex-auto-video-lab) | 本地媒体分析、编辑计划、FFmpeg 渲染和质量检查，也是镜序的媒体处理基础。 | Python / FFmpeg |
| [商品素材助手](https://github.com/h296025733-sys/amazon-tiktok-shop-media-downloader) | 从商品页提取当前 SKU 图片、视频与规格信息，按分类预览和批量下载。 | JavaScript / Manifest V3 |

## 其他工具与应用

| 项目 | 用途 |
| --- | --- |
| [Seedance 视频导演工作台](https://github.com/h296025733-sys/seedance-director-workbench) | 参考视频证据、分镜、素材职责与平台执行包。 |
| [TikTok Shop 只读数据管线](https://github.com/h296025733-sys/tiktok-shop-data-pipeline) | 端点白名单、请求签名、数据接入、订单归因与能力状态。 |
| [渠道内容运营台](https://github.com/h296025733-sys/channel-ops-workbench) | 账号、内容阶段、排期与运营记录的 Web 工作台；公开版使用示例数据。 |
| [FastMoss 本地数据目录](https://github.com/h296025733-sys/fastmoss-local-catalog) | 原始采集、SQLite 索引、图片登记、查询与导出一致性检查。 |
| [轻存 · TikTok 下载器](https://github.com/h296025733-sys/qingcun-tiktok-downloader) | Windows 桌面下载队列、目录管理、代理与逐项失败处理。 |
| [抖音下载与口播字幕](https://github.com/h296025733-sys/douyin-download-subtitles) | 平台视频与字幕提取、预览及 SRT 导出。 |
| [微信 ↔ Codex 文字聊天桥](https://github.com/h296025733-sys/wechat-codex-bridge) | 可分享的安装、授权、启动和排错脚本模板。 |

## 页面与交互练习

- [EM/20 · 二十种网页视觉实验](https://github.com/h296025733-sys/em20-web-design-gallery)：围绕同一主题做二十套版式与视觉系统。
- [Terminal UI Playground](https://github.com/h296025733-sys/terminal-ui-playground)：前端终端界面、命令历史与逐行输出；使用预设演示场景。

## 更早的项目

- [telecom-bid-scout-lite](https://github.com/h296025733-sys/telecom-bid-scout-lite)：通信招采线索接入、规则评分、可解释报告与飞书通知。
- [openclaw-local-bootstrap-lite](https://github.com/h296025733-sys/openclaw-local-bootstrap-lite)：Windows 下的 OpenClaw 环境诊断与启动辅助。
- [ai-xhs-video-workflow-mvp](https://github.com/h296025733-sys/ai-xhs-video-workflow-mvp)：短视频采集、BGM 替换与自动化调度工作流 MVP。
- [my-crypto-tool](https://github.com/h296025733-sys/my-crypto-tool)：早期网页小工具。

## 我在意的事

我习惯先把业务步骤和失败条件理清楚，再决定哪里适合用模型，哪里应该交给确定的规则。处理多人、多账号或多店铺时，权限、数据范围和恢复过程也是功能的一部分。

近期公开整理的仓库分别写了运行入口和检查范围。需要账号、模型或企业配置的项目，使用者准备自己的环境；演示页面和模型输出各自有明确的使用范围。
