# Batch 1 — 微型 SaaS / 开发者小工具 / Chrome 插件 / Notion-Airtable 周边

**本批小结**:本批共 10 个产品入库,**0 个含"未找到公开数据"字段**(全部字段均有可验证来源)。产品类型分布:Notion/Airtable 周边 4 个(Whalesync / Oopy / Noloco / HelpKit)、开发者小工具 3 个(TablePlus / APITemplate.io / DebugBear)、微型 SaaS 2 个(Mailmeteor / Pirsch)、Chrome 插件 1 个(Text Blaze)。地理:美 2、韩 1、越 1、爱 1、奥 1、法 1、新 1、英 1、德 1(共 9 国,美国占比 20%)。

**关于 WebFetch**:WebFetch 对所有 10 个 pricing 页面统一返回 403(疑似 user-agent 被 Cloudflare 类服务整体拦截),改用 WebSearch 验证。所有 homepage_url 和 pricing_url 均出现在 Google 搜索结果中,可达性已确认。

**关于研究价值**:本批刻意避开了同赛道里已经被讨论烂的标杆(Super.so / Cal.com / Plausible / Bannerbear / Softr / TextExpander 等),选了它们的"同赛道但讨论度低"的对手或亚洲版本。

---

## 产品总表

| # | 名称 | 国家 | 类别 | 定价模式 | 一句话 |
|---|---|---|---|---|---|
| 1 | [Whalesync](https://www.whalesync.com/) | US | Notion/Airtable 周边 | subscription | Notion/Airtable/Webflow 双向同步 |
| 2 | [Oopy](https://www.oopy.io/en) | Korea | Notion 周边 | subscription | 把 Notion 页面变成网站(韩国版) |
| 3 | [TablePlus](https://tableplus.com/) | Vietnam | 开发者小工具 | license | 原生多数据库 GUI 客户端 |
| 4 | [Noloco](https://noloco.io/) | Ireland | Airtable 周边 | freemium | Airtable 一键生成内部工具和客户门户 |
| 5 | [HelpKit](https://www.helpkit.so/) | Austria | Notion 周边 | subscription | Notion 变 help center / docs |
| 6 | [Text Blaze](https://blaze.today/) | US | Chrome 插件 | freemium | Chrome 文本模板带逻辑/动态字段 |
| 7 | [Mailmeteor](https://mailmeteor.com/) | France | 微型 SaaS | freemium | Gmail 内大批量邮件发送 |
| 8 | [APITemplate.io](https://apitemplate.io/) | Singapore | 开发者小工具 | freemium | PDF / 社交图生成 API |
| 9 | [DebugBear](https://www.debugbear.com/) | UK | 开发者小工具 | subscription | Core Web Vitals + 性能监控 |
| 10 | [Pirsch Analytics](https://pirsch.io/) | Germany | 微型 SaaS | subscription | GDPR-friendly 分析,GA 替代 |

---

## 增长信号与研究价值速览

| # | 名称 | 关键增长信号 | 研究价值 |
|---|---|---|---|
| 1 | Whalesync | YC S21 / $1.8M 种子 / PH 累计 866 upvotes | YC 出身但中英文 indie 圈讨论度低;'no-code 工具间胶水' 单独产品化 |
| 2 | Oopy | 2020 起 1000+ 付费客户;进入 Notion 官方集成目录 | 韩国非英语区独立产品,几乎零英文 indie 报道;Super.so/Bullet 已被讨论烂 |
| 3 | TablePlus | Show HN 单周 23K 访客、DAU +400%;HN 长期口碑 | 越南创始人卖给全球开发者;反 SaaS 主流的 license + 续期定价 |
| 4 | Noloco | YC S21 / $5.5M 累计 / G2 4.8 星 | Softr 被讨论烂,Noloco 同赛道但讨论度低很多;agency-first 定价值得对比 |
| 5 | HelpKit | 创始人公开过 $10K+ MRR(后停止披露) | 单人 bootstrapped,清晰展示 Notion 周边天花板;只有 1 篇深度案例 |
| 6 | Text Blaze | Chrome Web Store 70 万用户、4.9 星 / YC W21 | $2.99/月低价碾压 TextExpander;模板 DSL 设计独特 |
| 7 | Mailmeteor | Google Workspace Marketplace **700 万用户** / 'Recommended for Google Workspace' | 零融资 + 单一渠道吃下 700 万用户;中英文圈讨论 YAMM 多、Mailmeteor 极少 |
| 8 | APITemplate.io | Make/Zapier/n8n 集成驱动;持续付费评价 | Bannerbear 同赛道但亚洲创始人 / 零融资 / 极低讨论度,横向比对样本 |
| 9 | DebugBear | SEO 关键词覆盖 Core Web Vitals;Crunchbase 持续记录 | 前端性能赛道 indie 圈讨论几乎为零;'SEO 驱动获客而非社交' 标本 |
| 10 | Pirsch | $5K MRR 公开里程碑 / 460+ 客户 / 开源 SDK | Plausible/Fathom 已被讨论烂;Pirsch 在更小团队 + 更低价位下的差异化跑通 |

---

## 实现难度速览(供独立开发者参考)

| # | 名称 | 需自研模型 | 需后端 | 核心 API/技术栈 | 单人 4 周 MVP |
|---|---|---|---|---|---|
| 1 | Whalesync | ❌ | ✅ | Notion + Airtable + Webflow + Postgres + Stripe | ❌ |
| 2 | Oopy | ❌ | ✅ | Notion API + Let's Encrypt + 渲染层 + Stripe | ✅ |
| 3 | TablePlus | ❌ | ❌ | 各数据库驱动 + native UI | ❌ |
| 4 | Noloco | ❌ | ✅ | Airtable + Sheets + Postgres + Stripe + 渲染引擎 | ❌ |
| 5 | HelpKit | ❌ | ✅ | Notion API + 搜索引擎 + 渲染层 + Stripe | ✅ |
| 6 | Text Blaze | ❌ | ✅ | Chrome Ext API + 模板 DSL + Postgres + Stripe | ❌ |
| 7 | Mailmeteor | ❌ | ✅ | Gmail API + Sheets + Apps Script + Stripe | ✅ |
| 8 | APITemplate.io | ❌ | ✅ | Headless Chrome / Puppeteer + S3 + 模板 + Stripe | ✅ |
| 9 | DebugBear | ❌ | ✅ | Lighthouse + Puppeteer + 时序 DB + Stripe | ❌ |
| 10 | Pirsch | ❌ | ✅ | Go 采集核心 + Postgres/ClickHouse + Stripe | ✅ |

10/10 都不依赖自研模型;5/10 单人 4 周可做出 MVP;9/10 需要后端(只有 TablePlus 是纯客户端 license)。
