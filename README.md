# h296025733-sys

我主要做影像创作工具、经营数据系统和浏览器扩展。项目通常从具体工作开始：一段素材要怎么交付，一份报表能不能核对，重复操作怎样变成顺手的工具。

我喜欢把界面一直做到背后的流程：数据怎么来、任务怎么排、失败后留下什么、别人从哪里接着用。下面几项可以先看。

## 镜序 · AI 影像创作台

[项目与源码](https://github.com/h296025733-sys/jingxu-director-workbench) · Next.js / TypeScript / SQLite / Python

把需求、参考素材、创作规划、自动剪辑和交付版本收进同一个任务。后台处理同用户串行、不同用户轮转、分资源容量、上传取消与恢复；剪辑计划还记录原片覆盖和质量检查。这个项目让我把创作流程和多人使用时的工程问题一起处理。

从 [任务调度器](https://github.com/h296025733-sys/jingxu-director-workbench/blob/main/lib/work-scheduler.ts) 和 [上传会话](https://github.com/h296025733-sys/jingxu-director-workbench/blob/main/lib/video-upload-sessions.ts) 看实现。

## 飞书经营数据助手

[项目与源码](https://github.com/h296025733-sys/feishu-data-assistant) · TypeScript / 飞书多维表格 / 多租户

群聊里提问，由代码执行筛选、去重、求和和排名；群聊路由、表格与凭证按店铺分开。更新先形成计划并备份，执行后读回核对；回滚比较当前值与本次写入值，跳过后来被修改的记录。

可以一起看 [查询引擎](https://github.com/h296025733-sys/feishu-data-assistant/blob/main/src/query/engine.ts) 和 [更新 / 回滚](https://github.com/h296025733-sys/feishu-data-assistant/blob/main/src/realtime/feishu-video-sync.ts)。模型理解自然语言，统计口径和数据改动留在可检查的实现里。

## TikTok 达人助手

[项目与源码](https://github.com/h296025733-sys/tiktok-daren-assistant) · Chrome MV3 / TypeScript / 浏览器语音识别

围绕达人主页和当前视频做筛选、批量下载、评论翻译与字幕。动态页面会复用节点，异步请求也可能在切换视频后返回，因此活动视频、字幕缓存和下载队列各自管理状态。

[活动视频会话](https://github.com/h296025733-sys/tiktok-daren-assistant/blob/main/extension/src/content/session.ts) 很短，可以先从这里看结果归属；更长的侧栏流程与当前测试问题写在仓库里。

## 内容分析与媒体处理

| 项目 | 设计重点 |
| --- | --- |
| [TikTok 达人商业内容分析](https://github.com/h296025733-sys/tiktok-creator-intelligence) | 商业披露、挂链与推断分开；播放量与账号自身基线比较；两阶段复核绑定到本轮视频证据。 |
| [Auto Video Lab](https://github.com/h296025733-sys/codex-auto-video-lab) | JSON 剪辑单先校验，再渲染；成片解码、音视频指标和抽帧形成质量报告，也是镜序的媒体处理基础。 |
| [Seedance 视频导演工作台](https://github.com/h296025733-sys/seedance-director-workbench) | 参考片的动作、镜头、声音与时间轴证据，整理成分镜约束、素材职责和执行包。 |

## 数据与日常工具

| 项目 | 解决的问题 |
| --- | --- |
| [TikTok Shop 数据管线](https://github.com/h296025733-sys/tiktok-shop-data-pipeline) | 报表与只读 API 标准化；精确端点白名单、快照哈希、分页与能力状态。 |
| [FastMoss 本地数据目录](https://github.com/h296025733-sys/fastmoss-local-catalog) | 原始页、SQLite 索引、图片与导出之间的对应关系和缺口。 |
| [渠道内容运营台](https://github.com/h296025733-sys/channel-ops-workbench) | 店铺、账号、内容标识、制作阶段与排期的一套数据关系和矩阵界面。 |
| [商品素材助手](https://github.com/h296025733-sys/amazon-tiktok-shop-media-downloader) | 识别当前商品与 SKU，排除评论和推荐图，归并图片版本并分类下载。 |
| [轻存 · TikTok 下载器](https://github.com/h296025733-sys/qingcun-tiktok-downloader) | Windows 下载队列、文件整理、系统代理与逐项失败处理。 |
| [抖音下载与口播字幕](https://github.com/h296025733-sys/douyin-download-subtitles) | 当前视频绑定、平台字幕预览与带时间戳的 SRT 导出。 |
| [微信 ↔ Codex 文字聊天桥](https://github.com/h296025733-sys/wechat-codex-bridge) | 独立运行目录与可分享的安装、授权、网络诊断和维护模板。 |

## 前端实验

- [EM/20](https://github.com/h296025733-sys/em20-web-design-gallery)：二十套主题页面，比较侘寂、报刊、工业蓝图与数据驾驶舱等风格的信息组织。
- [Terminal UI Playground](https://github.com/h296025733-sys/terminal-ui-playground)：预设命令的输入节奏、逐行输出、键盘控制与状态层级。

## 更早的项目

- [telecom-bid-scout-lite](https://github.com/h296025733-sys/telecom-bid-scout-lite)：通信招采线索接入、规则评分、可解释报告与飞书通知。
- [openclaw-local-bootstrap-lite](https://github.com/h296025733-sys/openclaw-local-bootstrap-lite)：Windows 下的 OpenClaw 环境诊断与启动辅助。
- [ai-xhs-video-workflow-mvp](https://github.com/h296025733-sys/ai-xhs-video-workflow-mvp)：短视频采集、BGM 替换与自动化调度工作流 MVP。
- [my-crypto-tool](https://github.com/h296025733-sys/my-crypto-tool)：早期网页小工具。

近期整理的仓库保留了运行入口、设计说明、代码链接与检查记录。需要账号、企业表格、模型或平台的路径，分别说明实际测过什么与尚未验证什么；演示数据也有明确标注。
