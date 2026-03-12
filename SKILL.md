---
name: memory-enhancer
displayName: Memory Enhancer
version: 1.2.0
description: 记忆增强助手，支持语义搜索、自动提炼、智能分类、Token 优化、定时任务。让 AI 记住所有重要信息，同时减少 token 消耗。
license: MIT-0
acceptLicenseTerms: true
tags: memory, search, ai, productivity, optimization, scheduled-tasks
---

# Memory Enhancer - 记忆增强助手

强大的记忆管理工具，让 AI 记住所有重要信息。

---

## ✨ 功能特性

- 🔍 **语义搜索** - 搜索所有记忆文件，找到相关内容
- 📌 **自动提炼** - 自动提炼对话要点，保存到 MEMORY.md
- 🏷️ **智能分类** - 自动分类（偏好/决策/待办/项目）
- 🔗 **关联推荐** - 推荐相关的记忆片段
- 🧹 **过期清理** - 自动清理过期记忆
- 📊 **使用统计** - 记忆文件统计、搜索历史

---

## 🚀 安装

```bash
cd ~/.openclaw/workspace/skills
# 技能已安装在：~/.openclaw/workspace/skills/memory-enhancer
chmod +x memory-enhancer/scripts/*.py
```

---

## 📖 使用

### 语义搜索

```bash
python3 memory-enhancer/scripts/search.py "上次提到的飞书配置"
```

### 自动提炼

```bash
python3 memory-enhancer/scripts/summarize.py --session today
```

### 记忆分类

```bash
python3 memory-enhancer/scripts/classify.py --auto
```

---

## 🛠️ 脚本说明

| 脚本 | 功能 |
|------|------|
| `search.py` | 语义搜索 |
| `summarize.py` | 自动提炼 |
| `classify.py` | 智能分类 |
| `cleanup.py` | 过期清理 |

---

## 📄 许可证

MIT-0

---

**作者：** @williamwg2025  
**版本：** 1.0.0

---

## 🔒 安全说明

- **本地执行：** 所有脚本在本地运行，不联网
- **权限范围：** 仅需读取 ~/.openclaw/ 目录
- **无外部依赖：** 不克隆外部仓库，所有代码已包含
- **数据安全：** 不上传任何数据到外部服务器

---

**作者：** @williamwg2025  
**版本：** 1.0.1  
**许可证：** MIT-0
