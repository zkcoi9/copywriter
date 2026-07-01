# Copywriter

文案风格技能包 - 基于真实博主文章蒸馏的写作技能

## 项目结构

```
copywriter/
├── mimeng/           # 咪蒙风格
│   ├── skill.md      # 技能文件（v4.1）
│   ├── reference/    # 1014篇参考文章（已清理PDF转换残留）
│   └── learning_progress.md
└── [其他风格]/      # 未来扩展
```

## 已清理

- ✅ mimeng/reference: 移除 WCplus 工具头部、修复换行符、移除重复内容
- ✅ 从 2,557,807 字符清理至 2,174,636 字符（减少 383,171 字符）

## 使用

将对应的 skill 目录复制到 `~/.claude/skills/`：

```bash
cp -r mimeng ~/.claude/skills/mimeng
```

## 许可证

MIT
