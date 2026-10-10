# 小学语文 · 有声动画课件 作品集

> **Primary Chinese · Animated Audio Courseware Collection**

一套面向小学课堂的**有声动画课件**作品集：浏览器直接打开，无需安装、无需联网，内含课文朗读、旁白讲解、生字点读与实时音效。

An open collection of **animated audio courseware** for primary school classrooms. Opens straight in the browser — no install, no internet required — with textbook narration, teacher voiceover, vocabulary pronunciation and live sound effects.

[![GitHub Pages](https://img.shields.io/badge/%E5%9C%A8%E7%BA%BF%E9%A2%84%E8%A7%88-GitHub%20Pages-2ea44f?style=flat-square)](https://xiangsir4088.github.io/primary-courseware/)
[![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](./LICENSE)

---

## 🔗 在线预览 · Live Demo

| 入口 | 地址 | Entry |
| --- | --- | --- |
| 作品集首页 | <https://xiangsir4088.github.io/primary-courseware/> | Collection home |
| 《秋天的雨》课件 | <https://xiangsir4088.github.io/primary-courseware/autumn-rain/> | *The Rain of Autumn* |

> 打开后点击 **「🔊 点击开始上课」** 即可解锁浏览器声音（浏览器要求先有一次点击才允许播放音频）。
>
> Click **"🔊 点击开始上课"** on launch to unlock audio — browsers block sound until the first user click.

---

## 📚 收录课件 · Courseware

| # | 课件 | 学科 / 学段 | 页数 | 声音 | 在线打开 |
| --- | --- | --- | --- | --- | --- |
| 1 | **《秋天的雨》精品动画课件** | 语文 · 三年级上册（部编版） | 15 | 课文范读 5 段 + 旁白 15 条 + 生字点读 11 条 + 音效 | [▶ 打开](https://xiangsir4088.github.io/primary-courseware/autumn-rain/) |

| # | Courseware | Subject / Grade | Slides | Audio | Open |
| --- | --- | --- | --- | --- | --- |
| 1 | **The Rain of Autumn** | Chinese, Grade 3 (Vol. 1) | 15 | 5 passages + 15 narrations + 11 words + SFX | [▶ Open](https://xiangsir4088.github.io/primary-courseware/autumn-rain/) |

> 后续将持续新增课文课件（如《富饶的西沙群岛》《花的学校》等），本仓库即为系列作品官网。
>
> More textbook courseware will be added continuously; this repository doubles as the project's official gallery.

---

## ✨ 课件特性 · Features

**声音 Audio**

- 🎙️ **课文全文范读** —— 逐段真人级语音朗读，可反复播放，学生可跟读
- 🗣️ **每页旁白讲解** —— 老师口吻的知识点导学，翻页自动播报
- 🔊 **生字词点读** —— 点击"钥匙 / 五彩缤纷 / 喇叭"等词语即时发音
- 🎵 **实时音效** —— 翻页声、答对 / 答错提示音、雨声环境音（可按需开关）

**动画 Animation**

- 分层入场动画、飘落秋叶、光晕呼吸、场景插画（银杏、枫树、田野、小动物）
- 每页独立分镜，翻页重新播放出场动效

**互动 Interaction**

- 「连一连」点选配对练习，对错**即时反馈带音效**
- 拟人修辞单选题，作答后给出讲解
- 底部 **首页 / 上一页 / 页码 / 下一页 / 尾页 + 任意页跳转**，键盘 `←/→/空格/Home/End` 亦可翻页

**English (brief)**

- 🎙️ Full-text narration, 🗣️ per-slide teacher voiceover, 🔊 tap-to-pronounce vocabulary, 🎵 real-time sound effects (page turn, correct/wrong chime, rain ambience)
- Layered entrance animations, falling leaves, SVG-style scene illustrations
- Interactive matching exercise and a multiple-choice question with instant feedback
- Full navigation: first / prev / page indicator / next / last + jump-to-any-slide dropdown; keyboard `← → Space Home End` supported

---

## 🚀 使用方式 · How to use

**方式一：在线使用（推荐）**
直接打开 <https://xiangsir4088.github.io/primary-courseware/autumn-rain/>，点击「开始上课」即可。可投屏、可全屏（右下角 `⛶ 全屏`）。

**方式二：本地离线使用**
下载 `site/autumn-rain/index.html` 单个文件，双击即可打开。
**所有音频已内嵌进这一个 HTML 文件**（约 2.7 MB），不依赖网络、不依赖任何素材目录，拷贝到 U 盘也能在教室电脑上直接上课。

> **How to use** — Open the Pages link and click "开始上课". For offline classroom use, download the single `index.html` of a courseware: every audio clip is embedded as base64 inside that one file, so it works with no network and no assets folder — copy it to a USB stick and it just runs.

---

## 🗂️ 仓库结构 · Repository layout

```
primary-courseware/
├── site/                          # GitHub Pages 站点根目录 / Pages site root
│   ├── index.html                 # 作品集门户 / Collection home
│   └── autumn-rain/
│       └── index.html             # 《秋天的雨》课件（单文件，音频内嵌）
├── .github/workflows/pages.yml    # 自动部署到 GitHub Pages
├── LICENSE
└── README.md
```

---

## 🛠️ 技术说明 · Technical notes

- **纯静态**：零依赖、零构建、零后端，`site/` 目录即站点，GitHub Pages 直接托管
- **单文件课件**：HTML + CSS + JavaScript 全部内联；音频以 base64 data URI 内嵌，天然离线可用
- **音效合成**：翻页 / 对错 / 点击音效由 **Web Audio API 实时合成**，不占用任何音频文件
- **自适应**：`clamp()` + Grid/Flex 布局，从手机窄屏到投影大屏、全屏均可正常显示
- **无障碍提示**：播放语音时底部同步显示字幕条

> **Tech** — Pure static: no dependencies, no build step, no backend. Each courseware is a **single self-contained HTML file** with audio embedded as base64 data URIs. Sound effects are **synthesised at runtime with the Web Audio API**, so no extra audio assets are needed. Layout is fully responsive via `clamp()` + Grid/Flex, and a subtitle bar accompanies every voice clip.

---

## ➕ 新增一篇课件 · Adding a courseware

1. 在 `site/` 下新建目录，例如 `site/my-lesson/`，放入该课件的 `index.html`
2. 在 `site/index.html` 的作品集列表里加一张卡片
3. 提交到 `main` 分支 —— workflow 会自动重新部署到 Pages

> To add a new courseware: create `site/<slug>/index.html`, add a card to `site/index.html`, then push to `main` — the workflow redeploys automatically.

---

## 📄 许可 · License

本项目采用 [MIT License](./LICENSE)。
课件基于**部编版小学语文教材**编写，仅供课堂教学与学习交流使用，请勿用于商业售卖。

Released under the [MIT License](./LICENSE).
Courseware content is based on the **official primary Chinese textbook (部编版)** and is intended for classroom teaching and educational sharing only. Commercial resale is not permitted.

---

## 🙏 制作说明 · Credits

由 **WorkBuddy** 智能体辅助制作：课文配音与讲解语音由平台语音合成服务生成，动画、交互与音频引擎为原生 HTML / CSS / JavaScript 实现。

Made with **WorkBuddy**. Narration and voiceover are produced by the platform's text-to-speech service; all animation, interaction and the audio engine are hand-written in vanilla HTML / CSS / JavaScript.
