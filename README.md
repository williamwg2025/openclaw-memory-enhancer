# Memory Enhancer - 记忆增强助手

强大的记忆管理工具，让 AI 记住所有重要信息。

[English Version](README_EN.md)

---

## ✨ 功能特性

- 🔍 **语义搜索** - 搜索所有记忆文件
- 📌 **自动提炼** - 自动提炼对话要点
- 🏷️ **智能分类** - 偏好/决策/待办/项目
- 🔗 **关联推荐** - 推荐相关记忆
- 🧹 **过期清理** - 自动清理过期记忆

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
python3 memory-enhancer/scripts/search.py "飞书配置"
```

### 自动提炼

```bash
python3 memory-enhancer/scripts/summarize.py --session today
```

---

## 🛠️ 脚本

| 脚本 | 功能 |
|------|------|
| `search.py` | 语义搜索 |
| `summarize.py` | 自动提炼 |
| `classify.py` | 智能分类 |

---

**作者：** @williamwg2025  
**版本：** 1.0.0
