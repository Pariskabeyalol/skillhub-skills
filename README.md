<div align="center">

<img src="assets/banner.png" width="640" alt="SkillHub Skills 工作室"/>

# SkillHub Skills 工作室

_把生活难题做成开箱即用的 AI 技能_

![License](https://img.shields.io/badge/license-MIT-green)
![Skills](https://img.shields.io/badge/Skills-4个已上架-blue)
![兼容](https://img.shields.io/badge/兼容-Claude_Code_·_CodeBuddy_·_Cursor-orange)
![发布](https://img.shields.io/badge/发布-GitHub_Actions_自动化-9cf)

</div>

## 🧩 技能一览

| 技能 | 一句话介绍 | 亮点 | SkillHub |
|---|---|---|---|
| 🧧 **[份子钱参谋](https://skillhub.cn/skills/user_54e0fa64/fenziqian-advisor)** | 随礼多少、回礼怎么算,30 秒给区间和理由 | 全平台首个份子钱决策工具;城市基准 × 回礼对等 × 吉利数字校验 | [详情页](https://skillhub.cn/skills/user_54e0fa64/fenziqian-advisor) |
| 😏 **[互联网嘴替](https://skillhub.cn/skills/user_54e0fa64/internet-zuiti)** | 拒绝/催债/砍价/怼杠精,三档火力直接复制 | 🕊️体面 / 😏正常 / 🔥全开三档输出,8 大场景套路库 | [详情页](https://skillhub.cn/skills/user_54e0fa64/internet-zuiti) |
| 🎓 **[工校新生生存手册](https://skillhub.cn/skills/user_54e0fa64/hngy-freshman-guide)** | 河南省工业学校新生通关:报到、专业、升学 | 按中职真实生态设计:3+2/对口/单招三条升学路对比 | [详情页](https://skillhub.cn/skills/user_54e0fa64/hngy-freshman-guide) |
| 🏔️ **[珞珈新生生存手册](https://skillhub.cn/skills/user_54e0fa64/whu-freshman-guide)** | 武汉大学新生指南:报到、选课、食堂、黑话、猫 | 27 个来源交叉印证的黑话词典与校园猫图鉴 | [详情页](https://skillhub.cn/skills/user_54e0fa64/whu-freshman-guide) |

## 📦 安装

**方式一 · SkillHub CLI(推荐)**

```bash
skillhub install fenziqian-advisor --dir ~/.claude/skills/
skillhub install internet-zuiti   --dir ~/.claude/skills/
```

**方式二 · 直接拷贝**

每个目录就是一个标准 Agent Skill(`SKILL.md` + `references/`),拷进任意客户端的 skills 目录即可:

| 客户端 | 路径 |
|---|---|
| Claude Code | `~/.claude/skills/` |
| CodeBuddy(WorkBuddy) | `~/.codebuddy/skills/` |
| Cursor | `~/.cursor/skills/` |

## 🔄 更新流程

1. 修改技能目录下的文件,**`SKILL.md` 里的 `version` 升一位**
2. 本地发布:`skillhub publish <目录名> --changelog "改了什么"`
3. 或 push 后到 [Actions](https://github.com/Pariskabeyalol/skillhub-skills/actions/workflows/publish.yml) 手动触发 **Publish to SkillHub**(可指定单个目录)

![Publish workflow](https://github.com/Pariskabeyalol/skillhub-skills/actions/workflows/publish.yml/badge.svg)

## 📐 设计约定

- **指令与数据分离**:`SKILL.md` 只装行为逻辑(触发、路由、风格、红线),事实全部在 `references/` 按需加载——改数据不动指令
- **真实调研,查不到就说查不到**:所有事实基于公开来源交叉印证,并标注时效;不编造课程名、猫名、给分评价
- **诚实边界**:不预测分数线、不碰法律红线、时效信息引导到官方渠道复核

## 📄 License

[MIT](./LICENSE)
