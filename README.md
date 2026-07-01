# Copywriter

<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-Skill%20Pack-blue" alt="Claude Code Skill Pack">
  <img src="https://img.shields.io/badge/文案风格-蒸馏包-orange" alt="文案风格蒸馏包">
  <img src="https://img.shields.io/badge/MIT-License-green" alt="MIT License">
</p>

<p align="center">
  <i>基于真实博主文章全量蒸馏的文案风格技能包</i>
</p>

---

## 项目简介

**Copywriter** 是一个 Claude Code 技能包集合，通过**全量分析真实博主的历史文章**，蒸馏出具有鲜明个人风格的文案写作技能。

每个技能包都基于博主的真实文章（通常数百到数千篇），通过逐篇阅读、特征提取、模式识别，最终形成可复用的写作技能。

### 核心理念

> "真正的风格不是模仿，而是理解背后的逻辑。"

- ✅ **基于真实数据**：不是凭空想象的特征，而是从真实文章中统计、提炼
- ✅ **全量分析**：不只分析几篇代表作，而是尽可能覆盖博主的所有文章
- ✅ **可复用**：蒸馏出的技能可以用于生成具有相似风格的新内容

---

## 项目结构

```
copywriter/
├── mimeng/              # 咪蒙风格（v4.1）
│   ├── skill.md         # 技能文件（基于1014篇文章蒸馏）
│   ├── reference/       # 1014篇参考文章（已清理PDF转换残留）
│   └── learning_progress.md
│
├── [风格2]/            # 未来扩展：其他博主/风格
├── [风格3]/            # 持续添加中...
│
├── README.md            # 本文件
└── .gitignore
```

---

## 已收录风格

### 1. 咪蒙（mimeng）✅

**基于 2015-2019 年共 1014 篇公众号文章全量蒸馏**

| 项目 | 详情 |
|------|------|
| **文章数** | 1014 篇 |
| **时间跨度** | 2015-2019 年 |
| **技能版本** | v4.1（2026-07-01 更新） |
| **特征维度** | 标题/选题/开头/金句/技巧/情绪/广告 |
| **风格特点** | 替读者发声、情绪共鸣、金句密集、口语化 |

**已清理**：reference 文件已移除 PDF 转换残留（WCplus 工具头部、不当换行符、重复内容），从 2,557,807 字符清理至 2,174,636 字符。

---

## 使用方式

### 安装技能

将需要的风格目录复制到 Claude Code 的 skills 目录：

**Linux/macOS:**
```bash
# 安装咪蒙风格
cp -r mimeng ~/.claude/skills/mimeng
```

**Windows (PowerShell):**
```powershell
# 安装咪蒙风格
Copy-Item -Recurse -Force mimeng $HOME\.claude\skills\mimeng
```

### 调用技能

在 Claude Code 对话中输入：
```
/mimeng
```

然后提供你的写作需求，Claude 会基于咪蒙的风格生成文案。

---

## 未来计划

- [ ] 添加更多文案风格（知乎爆款回答、小红书爆款笔记等）
- [ ] 优化蒸馏流程（自动化特征提取）
- [ ] 添加风格对比工具（不同风格的特征对比）
- [ ] 提供在线 demo（基于 Streamlit 的风格生成器）

**欢迎贡献！** 如果你有喜欢的博主/风格，可以提交 PR 或 Issue。

---

## 如何添加新的风格

1. **收集文章**：尽可能收集博主的所有历史文章（公众号、知乎、小红书等）
2. **清理数据**：移除 PDF 转换残留、广告、无关内容
3. **特征提取**：逐篇分析，提取标题/选题/开头/金句/技巧/情绪等维度
4. **蒸馏技能**：基于统计和模式识别，编写 skill.md
5. **提交 PR**：将你的风格包提交到本仓库

---

## 许可证

MIT License

---

## 声明

- 本项目的技能包基于**公开可获取的文章**进行蒸馏
- 技能包用于**学习和研究目的**，不用于商业用途
- 如果涉及版权问题，请联系我们删除

---

**Made with ❤️ for Claude Code users**
