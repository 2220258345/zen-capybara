# TOOLS.md - Local Notes

Skills define *how* tools work. This file is for *your* specifics — the stuff that's unique to your setup.

## What Goes Here

Things like:
- Camera names and locations
- SSH hosts and aliases
- Preferred voices for TTS
- Speaker/room names
- Device nicknames
- Anything environment-specific

## Examples

```markdown
### Cameras
- living-room → Main area, 180° wide angle
- front-door → Entrance, motion-triggered

### SSH
- home-server → 192.168.1.100, user: admin

### TTS
- Preferred voice: "Nova" (warm, slightly British)
- Default speaker: Kitchen HomePod
```

## Why Separate?

Skills are shared. Your setup is yours. Keeping them apart means you can update skills without losing your notes, and share skills without leaking your infrastructure.

---

## Skill Discovery 🧩

### Find Skills
- **技能搜索优先使用：** `npx skills find [查询]`
- **技能文档位置：** `~/.agents/skills/find-skills/SKILL.md`
- **安装命令：** `npx skills add <owner/repo@skill> -g -y`
- **技能市场（备用）：** https://skillsmp.com/zh（如果 find-skills 没有满意的结果）

**使用场景：**
- 用户问 "怎么做 X"（可能已有现成技能）
- 用户问 "有没有技能可以做 X"
- 用户想扩展某个功能或工具
- 常见分类：Web 开发、测试、DevOps、文档、代码质量、设计、效率工具

**搜索技巧：**
1. 用具体关键词：`react performance` 比 `performance` 更好
2. 尝试同义词：`deploy` 不行就试 `deployment` 或 `ci-cd`
3. 热门来源：`vercel-labs/agent-skills`、`ComposioHQ/awesome-claude-skills`

---

## 内容获取策略 📰

### 国内网络环境

**问题：** 国内网络无法访问 BBC、Al Jazeera 等外网

**解决方案：**

1. **优先使用：**
   - 新浪新闻：https://news.sina.com.cn/
   - 新浪科技：https://tech.sina.com.cn/
   - 新浪财经：https://finance.sina.com.cn/

2. **微信文章被拦截：**
   - web_fetch 只能获取标题
   - **处理方式：去技能库查找转换工具**
   - `npx skills find` 搜索相关技能
   - 安装能处理微信/内容解析的技能

3. **新闻内容筛选：**
   - ✅ 重点关注：科技、AI
   - ❌ 忽略：普通娱乐、八卦、非重要事件

---

## 已安装技能清单 ✅

### 核心技能
- **find-skills** - 技能发现助手
- **news-summary** - RSS 新闻总结（国内可访问）

### 待配置技能
- **google-news** - Google News（需认证，当前不可用）
- **firecrawl** - 强力网页抓取（需认证，当前不可用）

---

Add whatever helps you do your job. This is your cheat sheet.
