# Omega の視界 中文本地化仓库

<div align="center">

![Visual Novel](https://img.shields.io/badge/Type-Visual%20Novel-ff69b4)
![Engine](https://img.shields.io/badge/Engine-Kirikiri%2FTJS-blue)
![Language](https://img.shields.io/badge/Language-Japanese%20%7C%20Chinese-green)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)

*一个基于 Kirikiri/TJS 引擎的视觉小说游戏的中文本地化仓库*

![游戏主视觉图](https://img.dlsite.jp/modpub/images2/work/doujin/RJ102000/RJ101805_img_main.webp)

</div>

## 📖 项目简介

「Omega の視界」是一款日式视觉小说游戏，本项目包含了中文本地化版本，目前采用AI翻译，人工校对的方式进行翻译。

### 🎮 游戏介绍

这是一部以书库之城发生的事件为舞台，以猫为主题创作的传奇系视觉小说。

閂夜明（はり よあけ）独自包揽原画与剧本，打造出独一无二的世界观。

除了由 onoken 先生、三泽秋女士担任主题曲的豪华阵容外，本次新作中，还收录了由负责背景音乐的 Manack 先生作曲、mitose noriko（みとせのりこ）女士作词并演唱的插入歌（短篇版本）！

#### 📚 章节构成

- 第一幕『Omegaの視界 シキのはじまり/未解封のハコニハ』（已翻译）

- 第二幕『Omegaの視界 アキかけたシキのアイ』
- 第三幕『Omegaの視界 アキかけたシキのアイ:残(ザン)』
- 最終幕『Omegaの視界 〜ミヨ　オワレル　シマイ　トワ(●nd)〜』

#### 🌟 故事梗概

愿 Omega 之瞳的祝福降临于你。

自称美少女古书店长的宫冈门王水（かどみ），与主人公饭洼真言（まこと）一同前往北方乡村 "玄之森"。

在当地，真言接到门王水的命令，调查疑似与神秘资料集《月狂跳（げっきょうちょう）》相关的神体，以及当地的祭祀活动。

调查途中，真言遇到了自称是他青梅竹马的贵奴（きぬ），以及独眼少女冬夏（とうか），并与她们一同展开调查。

被饭洼本家的意图裹挟着，真言等三人在冬夏的老家 —— 三春家的仓库中，究竟看到了什么？

碎片化的信息。
逐渐扭曲的视野。

『彼は雫だ。
濁ったみどろをさざめかせ、停止した時間を動かす針だ』

嗚呼、

猫が──

### 翻译进度

- 剧本翻译：进行中
- 系统文件翻译：完成
- 翻译对照文件：Omegaの視界 ～ミヨ オワレル シマイ トワ（●ｎｄ）～／ねこバナナ.trans

## 🗂️ 项目结构

```
Omega-no-shikai_CN/
├── Chinese/                    # 中文版本
│   └── data/
│       ├── scenario/           # 剧本文件
│       ├── system/             # 系统文件
│       └── startup.tjs         # 启动脚本
├── Japanese/                   # 日文版本
│   └── data/
│       ├── scenario/           # 剧本文件
│       ├── system/             # 系统文件
│       ├── startup.tjs         # 启动脚本
│       └── 1.py               # 编码转换工具
└── Omegaの視界 ～ミヨ オワレル シマイ トワ（●ｎｄ）～／ねこバナナ.trans  # 翻译文件
```

## 🚀 快速开始

## 🔧 开发说明

### 常见问题修复

#### @r 标签格式问题

使用 Translator++ 导出 ks 文件后，打开游戏可能会遇到因为 `@r` 没有独占一行导致的报错。可以使用以下正则表达式进行批量修复：

- **查找**：`@r(?!\s*$)`
- **替换为**：`@r\n`

这个正则表达式会找到所有不在行末的 `@r` 标签，并在其后添加换行符，确保 `@r` 标签独占一行。



### 编码转换（仅日文版本）

如果遇到编码问题，可以使用提供的转换工具：

```bash
cd Japanese/data/
python 1.py
```

该脚本会自动将 Shift-JIS 编码的 `.ks` 和 `.tjs` 文件转换为 UTF-8 编码。


## 📁 文件说明

| 文件/目录 | 描述 |
|-----------|------|
| `startup.tjs` | 游戏启动脚本，负责初始化系统 |
| `scenario/` | 存放游戏剧本和场景文件 |
| `system/` | 系统相关文件和配置 |
| `1.py` | 编码转换工具（仅日文版本） |
| `*.trans` | 翻译对照文件，需要使用 Translator++ 打开 |



## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request 来改进项目：

1. Fork 本项目
2. 创建新分支 (`git checkout -b test`)
3. 提交更改 (`git commit -m 'Add some changes'`)
4. 推送到分支 (`git push origin test`)
5. 开启 Pull Request


## 🙏 致谢

- 原作开发团队ねこバナナ
- Kirikiri/TJS 引擎开发者

---

<div align="center">

**享受游戏体验！** 🎮

</div>