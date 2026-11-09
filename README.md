# 我的作品集 · run666888

> 插件、小软件和实验项目的索引。能公开的代码都单独开了仓库；涉及第三方素材、厂商 SDK 或个人数据的项目，只在这里给出说明，不上传代码。

## DSH 插件

| 项目 | 说明 | 状态 |
| --- | --- | --- |
| [dsh-peak-hours](https://github.com/run666888/dsh-peak-hours) | DeepSeek 高峰/空闲时段提示：输入框角标显示时段、北京时间与倒计时，设置页把用量拆成高峰/空闲并估算花费。已收录进 DSH 社区市场 | ✅ 已发布 |

## 桌面小工具

| 项目 | 说明 | 技术 |
| --- | --- | --- |
| [sysmon-float](https://github.com/run666888/sysmon-float) | Windows 11 系统状态悬浮窗：CPU、网络、GPU、内存、运行时间；横向/纵向、三密度、四配色、透明置顶 | Electron |
| [token-tracker](https://github.com/run666888/token-tracker) | 跨平台 AI Token 用量追踪：本地代理记录各服务商用量，按模型汇总并估算花费 | Electron + React + TS |
| [cliphistory](https://github.com/run666888/cliphistory) | Windows 剪贴板历史：后台记录复制过的文本，搜索、点击回填 | Python + tkinter |
| [screen-time-tracker](https://github.com/run666888/screen-time-tracker) | 屏幕使用时间：后台采集活动窗口，本地 Flask 面板按应用统计 | Python + Flask + SQLite |

## 网页 / PWA

| 项目 | 说明 | 技术 |
| --- | --- | --- |
| [sonicseal](https://github.com/run666888/sonicseal) | 声波加密机：文本 → AES-256-GCM → 7 位信道编码 → ggwave FSK 声波；麦克风收回解密。含 ESP32-C3 + HC-12 电台版固件 | 纯前端 PWA + MicroPython |

## AI / 自动化

| 项目 | 说明 | 技术 |
| --- | --- | --- |
| [personal-agent](https://github.com/run666888/personal-agent) | 个人 AI 助手：CLI + 桌面窗口，多轮对话、可切换推理档位、本地文件与 PowerShell 工具带审批 | OpenAI Python SDK（Responses API） |
| [face-detection](https://github.com/run666888/face-detection) | 实时多人脸检测与识别（不带模型、不带人脸数据） | OpenCV YuNet + InsightFace |
| [photo-slideshow](https://github.com/run666888/photo-slideshow) | 照片自动排版成拼图 / pptx 幻灯片 / mp4 视频 | Python + ffmpeg |
| [dl-starter](https://github.com/run666888/dl-starter) | 面向 Intel Arc XPU 的图像分类训练模板：AMP、断点续训、CLI 推理 | PyTorch |

## 硬件与嵌入式

| 项目 | 说明 |
| --- | --- |
| [sonicseal](https://github.com/run666888/sonicseal)（`firmware/`） | ESP32-C3 + HC-12 433MHz 加密电台：A 板输入，B 板 OLED 显示，空中走密文 |
| [stm32-vscode-starter](https://github.com/run666888/stm32-vscode-starter) | STM32 + VSCode 工程脚手架：CubeMX Makefile 工程、初始化脚本与模板 |

## Skills

| 项目 | 说明 |
| --- | --- |
| [dsh-skills](https://github.com/run666888/dsh-skills) | 三个自研 skill：一键 git 流程、技术视频动效规范、多智能体委派门槛与拆法 |

## 没有开源的项目（及原因）

- **课程 / 竞赛项目**（四旋翼 MPC、CUMCM、过程控制、PPO-FJSP 复现、智能车等）：涉及课程与竞赛规则，暂不公开，避免学术诚信争议。
- **硬件厂商 SDK 相关脚本**（WS63/Spark 烧录、部分板卡工具）：受厂商 SDK 许可约束。
- **视频生产流水线**：包含第三方配音、素材与工程文件，版权不清晰。
- **Zotero PDF 翻译服务**：核心是第三方的 [pdf2zh-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next)，只做了本地部署封装，不重复开源。

## 合规说明

- 本账号下所有仓库**不含**：API Key、私钥/证书、个人照片、屏幕使用记录、人脸数据库。
- 第三方组件遵循其原始许可：
  - `sonicseal` 使用 [ggwave](https://github.com/ggerganov/ggwave)（MIT）做 FSK 调制；
  - `face-detection` 需自行下载 YuNet（OpenCV Zoo）与 InsightFace `buffalo_s` 模型，InsightFace 模型**仅限非商业研究用途**；
  - `sysmon-float` 依赖 `@hicccc77/electron-liquid-glass` 与 `systeminformation`，遵循各自许可。
- 人脸识别类代码仅作技术演示，请勿用于未经同意的采集或识别他人。

## License

本仓库的文档与索引以 MIT 许可发布；各子项目见其仓库内的 LICENSE。
