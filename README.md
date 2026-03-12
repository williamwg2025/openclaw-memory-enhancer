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
- ⚡ **Token 优化** - 分析并优化 token 消耗（NEW!）

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
python3 memory-enhancer/scripts/search.py "飞书配置"
```

### 自动提炼

```bash
python3 memory-enhancer/scripts/summarize.py --session today
```

### Token 优化分析

```bash
# 分析当前 token 使用
python3 memory-enhancer/scripts/token-optimizer.py --analyze

# 生成优化建议
python3 memory-enhancer/scripts/token-optimizer.py --suggest

# 压缩旧记忆（保留最近 30 天）
python3 memory-enhancer/scripts/token-optimizer.py --compress --days 30

# 完整优化（分析 + 建议 + 压缩）
python3 memory-enhancer/scripts/token-optimizer.py --full
```

### 定时优化任务

```bash
# 启用定时任务
python3 memory-enhancer/scripts/scheduled-optimizer.py enable

# 查看状态
python3 memory-enhancer/scripts/scheduled-optimizer.py status

# 手动执行
python3 memory-enhancer/scripts/scheduled-optimizer.py analyze   # 分析
python3 memory-enhancer/scripts/scheduled-optimizer.py compress  # 压缩
python3 memory-enhancer/scripts/scheduled-optimizer.py suggest   # 建议

# 禁用定时任务
python3 memory-enhancer/scripts/scheduled-optimizer.py disable
```

**定时任务计划：**
- 每天早上 8 点：自动分析 token 使用
- 每周日凌晨 3 点：自动压缩旧记忆
- 每周一早上 8 点：生成优化建议

---

## 🛠️ 脚本列表

| 脚本 | 功能 |
|------|------|
| `search.py` | 语义搜索 |
| `summarize.py` | 自动提炼 |
| `classify.py` | 智能分类 |
| `token-optimizer.py` | Token 优化分析（NEW） |

---

## 📊 Token 优化功能

### 优化方向

| 优化项 | 预计节省 | 说明 |
|--------|---------|------|
| 智能上下文裁剪 | 30-50% | 只读取相关记忆片段 |
| 会话历史摘要 | 40-60% | 用摘要替代完整历史 |
| 记忆压缩 | 20-30% | 定期合并/压缩旧记忆 |
| Token 监控 | - | 统计 + 优化建议 |

### 使用示例

```bash
# 查看当前 token 使用统计
python3 memory-enhancer/scripts/token-optimizer.py

# 输出示例：
# 文件                    字符数      Token 数       行数
# MEMORY.md              1,878          469       91
# SESSION-STATE.md       1,734          433       71
# USER.md                  640          160       46
# 总计                   9,492        2,371
```

---

**作者：** @williamwg2025  
**版本：** 1.2.0（新增定时优化任务）

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
