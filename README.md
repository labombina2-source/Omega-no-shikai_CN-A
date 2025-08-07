# Omega の視界 ～ミヨ オワレル シマイ トワ（●ｎｄ）～

<div align="center">

![Visual Novel](https://img.shields.io/badge/Type-Visual%20Novel-ff69b4)
![Engine](https://img.shields.io/badge/Engine-Kirikiri%2FTJS-blue)
![Language](https://img.shields.io/badge/Language-Japanese%20%7C%20Chinese-green)
![Status](https://img.shields.io/badge/Status-Localized-success)

*一个基于 Kirikiri/TJS 引擎的视觉小说游戏的中文本地化仓库*


</div>

## 📖 项目简介

「Omega の視界」是一款日式视觉小说游戏，本项目包含了中文本地化版本，目前采用AI翻译，人工校对的方式进行翻译。

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
| `*.trans` | 翻译对照文件 |



## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request 来改进项目：

1. Fork 本项目
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request


## 🙏 致谢

- 原作开发团队
- Kirikiri/TJS 引擎开发者

---

<div align="center">

**享受游戏体验！** 🎮

</div>