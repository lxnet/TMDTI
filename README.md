
# TMDTI 人格测试 | Too Much Drama Type Indicator

[![GitHub stars](https://img.shields.io/github/stars/yourusername/tmdti-test?style=social)](https://github.com/yourusername/tmdti-test)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Made with](https://img.shields.io/badge/Made%20with-HTML%2FTailwind%2FJS-blue)](https://developer.mozilla.org/)

> **"MBTI 已经过时，TMDTI 来了。"**

在这个"那咋了"和"已读乱回"的时代，TMDTI 用量身定制的 30 道灵魂拷问，测出你究竟是 **"偷感很重"** 的隐形人，还是 **"Passion"** 拉满的显眼包。

🌐 **[在线体验](tmdti.suify.cn)**

---

## ✨ 项目特色

- 🎭 **16 种热梗人格类型** - 从"Passion 狂暴者"到"抽象隐身人"，每种都有独特的网络亚文化特征
- 📊 **五维度评分系统** - Passion 能量 / 松弛感 / 抽象力 / 偷感指数 / 逻辑值
- 📱 **完美移动端适配** - 支持手机端长按保存结果图片
- 🎨 **故障艺术视觉风格** - Glitch 效果 + 赛博朋克配色
- ⌨️ **键盘导航支持** - 数字键 1-4 快速作答，方向键切换题目

---

## 🧠 人格类型一览

| 代码 | 名称 | 特征描述 |
|:---:|:---|:---|
| **AAAA** | 🔥 Passion 狂暴者 | 古希腊掌管 Passion 的神 |
| **AAAP** | 🌟 显眼包 Pro Max | 水灵灵地成为焦点 |
| **AAPA** | 🚀 赛博激情家 | 数字游民的 Passion 版本 |
| **AAPP** | 🎭 预制显眼包 | 被社会预制的 Passion 人格 |
| **APAA** | 🎨 抽象 Passion 家 | 用抽象表达 Passion |
| **APAP** | 🤖 梗图制造机 | 24 小时不间断产出 meme |
| **APPA** | 🎸 赛博吟游诗人 | 在数字世界吟唱 Passion |
| **APPP** | 🔍 抽象观察家 | 冷静地搞抽象 |
| **PAAA** | 🧮 逻辑 Passion 家 | 理性地 Passion，Passion 地理性 |
| **PAAP** | 🧘 松弛感掌控者 | 从从容容游刃有余 |
| **PAPA** | 💻 赛博分析师 | 用数据解构一切热梗 |
| **PAPP** | 📊 预制理性人 | 被系统预制的逻辑怪 |
| **PPAA** | 🥷 偷感 Passion 者 | 偷偷 Passion，惊艳所有人 |
| **PPAP** | 👻 隐形显眼包 | 在人群中隐形，在角落里显眼 |
| **PPPA** | 🐱 终极偷感人 | 偷感很重地观察世界 |
| **PPPP** | 👤 抽象隐身人 | 存在但不可见，抽象但真实 |

---

## 📋 题目设计维度

测试基于四个核心维度设计：

| 维度 | 对立面 | 描述 |
|:---|:---|:---|
| **E/I** (外向/内向) | A/P (Active/Passive) | 社交能量获取方式 |
| **A/R** (抽象/现实) | A/P (Abstract/Realistic) | 信息处理与表达方式 |
| **P/V** (低调/显眼) | P/V (Private/Visible) | 自我展示与存在感策略 |
| **L/C** (逻辑/混沌) | A/P (Analytical/Chaotic) | 决策风格与思维模式 |

---

## 🛠️ 技术栈

- **HTML5** - 语义化结构
- **Tailwind CSS** - 原子化 CSS 框架（CDN 引入）
- **原生 JavaScript** - 无框架依赖，轻量高效
- **html2canvas** - 客户端截图生成
- **Google Fonts** - Noto Sans SC 中文字体

---

## 📸 截图功能说明

项目支持将测试结果保存为图片：

- **iOS 设备**：生成预览 → 长按图片 → 保存到相册
- **Android/PC**：自动生成下载，保存为 `TMDTI-{人格类型}-{时间戳}.png`

截图区域针对移动端优化，包含：
- 人格类型代码与名称
- 匹配度百分比
- 五维度雷达图风格的进度条
- 人格分析与代表语录
- 品牌水印与免责声明

---

## 🎨 自定义配置

### 修改题目
编辑 `index.html` 中的 `questions` 数组，每个题目包含：
```javascript
{
    id: 1,
    text: "题目描述",
    options: [
        { text: "选项A", scores: { E: 3, A: 1 } },  // 分值对应维度
        { text: "选项B", scores: { I: 3, R: 1 } },
        // ...
    ]
}
