---
name: memory-enhancer
displayName: Memory Enhancer
version: 1.0.0
description: 记忆增强助手，支持语义搜索、自动提炼、智能分类。让 AI 记住所有重要信息，不再遗漏关键内容。
license: MIT-0
acceptLicenseTerms: true
tags: memory, search, ai, productivity
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
cd /root/.openclaw/workspace/skills
git clone https://github.com/williamwg2025/openclaw-memory-enhancer.git memory-enhancer
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
