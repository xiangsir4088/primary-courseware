# 小学课堂 · 动画课件作品集

> **Animated Courseware Collection for Primary Classrooms**

把小学课堂上的课文与数学难题，做成**浏览器一打开就能演示**的动画课件：语文有课文范读、老师旁白、生字点读；数学把抽象方法变成看得见的动作。

An open collection of **animated courseware** for primary school classrooms — textbook narration and vocabulary for Chinese, and step-by-step visual demonstrations for Math. Opens straight in the browser, no install required.

[![GitHub Pages](https://img.shields.io/badge/%E5%9C%A8%E7%BA%BF%E6%BC%94%E7%A4%BA-GitHub%20Pages-2ea44f?style=flat-square)](https://xiangsir4088.github.io/primary-courseware/)
[![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](./LICENSE)

---

## 🔗 访问地址导航 · Live Demo

| 入口 | 地址 | Entry |
| --- | --- | --- |
| **作品集主页** | <https://xiangsir4088.github.io/primary-courseware/> | Collection home |
| 语文 ·《秋天的雨》 | <https://xiangsir4088.github.io/primary-courseware/chinese/autumn-rain/> | *The Rain of Autumn* (Chinese) |
| 语文 · 古诗绘本课件 | <https://xiangsir4088.github.io/primary-courseware/chinese/picture-book/> | Classical-poem picture-book decks |
| 数学 ·《鸡兔同笼》 | <https://xiangsir4088.github.io/primary-courseware/math/chicken-rabbit/> | *Chickens & Rabbits* (Math) |
| 语文 · 离线单文件 | <https://xiangsir4088.github.io/primary-courseware/chinese/autumn-rain/offline.html> | Offline single-file build |

> 旧地址 `…/autumn-rain/` 与 `…/chicken-rabbit/` 已做**自动跳转**，之前分享出去的链接依然可用。
>
> The old paths redirect automatically, so previously shared links keep working.

---

## 📚 课件清单 · Courseware

### 语文 · Chinese

| # | 课件 | 学段 | 形式 | 打开 |
| --- | --- | --- | --- | --- |
| 1 | **《秋天的雨》精品动画课件** | 三年级上册（部编版） | 网页 · 15 页 · 31 条配音 | [▶ 在线演示](https://xiangsir4088.github.io/primary-courseware/chinese/autumn-rain/) |
| 2 | **四年级语文 · 古诗绘本课件（5 套）** | 四年级上册（部编版） | PPTX 下载 · 共约 38 MB | [📥 查看并下载](https://xiangsir4088.github.io/primary-courseware/chinese/picture-book/) |

《秋天的雨》：课文范读 5 段 + 每页旁白 15 条 + 生字点读 11 条 + 实时音效，含「连一连」与拟人单选题。
古诗绘本课件：《暮江吟》《望庐山瀑布》《雪梅》《题西林壁》《爬山虎的脚》——每首拆成「认识诗人 → 诵读全诗 → 逐句品析 → 轻声吟诵」。

### 数学 · Math

| # | 课件 | 学段 | 形式 | 打开 |
| --- | --- | --- | --- | --- |
| 1 | **鸡兔同笼 · 一步一步数腿** | 四年级下册 · 数学广角 | 网页 · 互动演示 | [▶ 在线演示](https://xiangsir4088.github.io/primary-courseware/math/chicken-rabbit/) |

点「下一步」，笼子里就有一只鸡长出 2 条腿变成兔，腿数从 16 一路涨到 26，脚丫柱状图实时对照目标——把「假设法」讲成看得见的动作，还支持拖滑块与自动播放。

> 后续持续新增，本仓库即系列作品官网。
>
> More courseware will be added continuously; this repository doubles as the project's official gallery.

---

## 🗂️ 仓库结构 · Repository layout

> ⚠️ 注意：GitHub Pages 的站点根目录是 **`site/`**，不是仓库根目录。
> 新增课件请放进 `site/<学科>/<课件名>/`，并在 `site/index.html` 加一张卡片。

```
primary-courseware/
├── site/                                  # ← GitHub Pages 站点根目录
│   ├── index.html                         # 作品集门户（语文 / 数学两个分区）
│   ├── chinese/                           # 语文
│   │   ├── autumn-rain/                   #   《秋天的雨》
│   │   │   ├── index.html                 #     在线版（页面 80 KB）
│   │   │   ├── offline.html               #     离线单文件版（音频内嵌，约 2.7 MB）
│   │   │   └── audio/*.mp3                #     31 条配音，按需加载
│   │   └── picture-book/                  #   四年级语文古诗绘本课件
│   │       ├── index.html                 #     画廊页（含诗作原文与教学步骤）
│   │       └── files/*.pptx               #     5 套 PPTX，共约 38 MB
│   ├── math/                              # 数学
│   │   └── chicken-rabbit/                #   《鸡兔同笼》
│   │       ├── index.html
│   │       └── vendor/echarts.min.js      #     图表库本地化，不依赖外部 CDN
│   └── autumn-rain/  chicken-rabbit/      #   旧地址 → 自动跳转页（保住已分享链接）
├── .github/workflows/pages.yml            # 自动部署到 GitHub Pages
├── README.md
└── LICENSE
```

---

## ✨ 课件特性 · Features

- 🎙️ **课文全文范读** —— 逐段真人级语音朗读，可反复播放，学生可跟读
- 🗣️ **每页旁白讲解** —— 老师口吻的知识点导学，翻页自动播报
- 🔊 **生字词点读** —— 点击"钥匙 / 五彩缤纷 / 喇叭"等词语即时发音
- 🎵 **实时音效** —— 翻页声、答对 / 答错提示音、雨声环境音（可按需开关）
- 🖐️ **互动练习** —— 「连一连」点选配对 + 单选拟人题，对错即时反馈并自动记录作答
- 🐔 **看得见的数学演示** —— 鸡一只只换成兔，腿数实时变化并与目标线对照
- 📥 **绘本课件下载** —— 古诗绘本 PPTX，PowerPoint / WPS 全屏放映
- 📶 **可离线使用** —— 语文课件另附单文件离线版，音频内嵌，拷 U 盘即可上课

**English (brief)** — Full-text narration · per-slide teacher voiceover · tap-to-pronounce vocabulary · live sound effects · interactive matching & quiz with instant feedback · step-by-step math demonstration (chicken-and-rabbit) · downloadable PPTX picture-book decks · offline single-file build for the Chinese courseware.

---

## 🚀 使用方式 · How to use

| 场景 | 怎么做 |
| --- | --- |
| 在线演示 | 直接打开上面的链接，投屏即可；按 `F11` 全屏 |
| 语文课件出声 | 进入后先点一下「🔊 点击开始上课」——浏览器要求先有用户点击才允许播放声音 |
| 数学课件 | 打开即可操作，无音频；点「下一步」、「自动播放」或拖滑块 |
| PPTX 绘本 | 点「下载 PPTX」保存，用 PowerPoint / WPS 打开，按 `F5` 全屏放映 |
| 教室无网 | 下载语文离线单文件版，双击打开，音频已全部内嵌 |

---

## ➕ 新增一个课件 · Adding a courseware

1. 把课件放进新目录，例如 `site/math/tree-planting/index.html`
2. 在 `site/index.html` 对应的学科分区里加一张卡片
3. 推送到 `main` 分支 —— workflow 会自动重新部署到 Pages

> To add a courseware: drop it into `site/<subject>/<slug>/index.html`, add a card to `site/index.html`, then push to `main`.

---

## 🛠️ 技术说明 · Technical notes

- **纯静态**：零构建、零后端，`site/` 目录即站点，GitHub Pages 直接托管
- **页面与音频分离**：语文课件页面仅 80 KB，31 条 mp3 按需加载——秒开，且单条损坏不影响整页
- **音效实时合成**：翻页 / 对错 / 点击音效由 **Web Audio API** 生成，不占任何音频文件
- **依赖本地化**：数学课件所用图表库（Apache ECharts）随仓库分发，**不依赖任何外部 CDN**
- **失败降级**：图表库若加载失败，讲解、数字与按钮仍全部可用；语文课件若配音数据未加载完整，会明确提示且不影响翻页
- **自适应**：`clamp()` + Grid/Flex，手机窄屏到投影大屏、全屏均可正常显示

> **Tech** — Pure static, no build step, no backend. Courseware pages and audio are split so pages stay tiny (80 KB) and a single bad clip never breaks the page. Sound effects are synthesised at runtime with the Web Audio API. Third-party chart library is vendored in-repo, so there is **no external CDN dependency**. If it ever fails to load, the lesson still works. Layout is fully responsive.

---

## 📄 许可 · License

本项目采用 [MIT License](./LICENSE)。
课件内容基于**部编版小学教材**编写，仅供课堂教学与学习交流，请勿用于商业售卖。

Released under the [MIT License](./LICENSE). Content is based on the **official primary textbook (部编版)** and is intended for classroom teaching and educational sharing only. Commercial resale is not permitted.

---

## 🙏 制作说明 · Credits

由 **WorkBuddy** 智能体辅助制作：配音由平台语音合成服务生成，动画、交互与音频引擎为原生 HTML / CSS / JavaScript。

Made with **WorkBuddy**. Narration is produced by the platform's text-to-speech service; all animation, interaction and the audio engine are hand-written in vanilla HTML / CSS / JavaScript.
