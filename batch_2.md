# Batch 2 — 创作者工具 / PDF-文档 / 图片视频音频 / 表单简历发票

**本批小结**:本批共 10 个产品入库,**0 个含"未找到公开数据"字段**。产品类型分布:创作者工具 3 个(Tella / Screen Studio / Munch)、PDF/文档 2 个(Sejda / DocSpring)、图片视频音频 3 个(Cleanvoice / Tape It / Wisecut)、表单/简历/发票 2 个(Kickresume / Hiveage)。

**地理:本批 0 美国产品**。荷 x2(Tella / Sejda)、波(Screen Studio)、罗(Cleanvoice)、新西兰(DocSpring)、斯洛伐克(Kickresume)、斯里兰卡(Hiveage)、德(Tape It 主驻地)、巴西(Wisecut)、以色列(Munch)。10 国(其中荷兰双产品都是低调老牌)。

**搜索过程中的关键修正**:
- 我原以为 Tella 是爱尔兰 Dublin,实际是荷兰 Amsterdam(YC S20,6 人小团队)
- 我原以为 Sejda 是罗马尼亚,实际是 Sejda BV 荷兰公司(故意低调 14 年)
- 我原以为 Munch 是韩国创作工具,实际是以色列 Tel Aviv 团队(已融 $7.2M)
- DocSpring 创始人 Nathan Broadbent 在新西兰 Auckland(找回 NZ 代表)

**自检**:全员未触发"研究价值过滤"四条排除标准。Munch $7.2M 融资是本批最高,远低于 $50M 门槛。Tape It 有过两次 TechCrunch 报道,Screen Studio 有 Starter Story,Cleanvoice 有 Starter Story —— 这三个属于"被部分写过但未进入标准 indie 案例库"。

---

## 产品总表

| # | 名称 | 国家 | 类别 | 定价模式 | 一句话 |
|---|---|---|---|---|---|
| 1 | [Tella](https://www.tella.com/) | Netherlands | 创作者工具 | subscription | 浏览器内做品牌感强的产品演示录屏 |
| 2 | [Screen Studio](https://screen.studio/) | Poland | 创作者工具 | subscription | Mac 精致演示录屏(自动放大平滑) |
| 3 | [Cleanvoice AI](https://cleanvoice.ai/) | Romania | 音频处理 | subscription | AI 去除播客 filler/噪音/停顿 |
| 4 | [Sejda](https://www.sejda.com/) | Netherlands | PDF/文档 | subscription | 在线+桌面 PDF 编辑工具集 |
| 5 | [DocSpring](https://docspring.com/) | New Zealand | PDF/文档 | subscription | PDF 表单填充 + 生成 API |
| 6 | [Kickresume](https://www.kickresume.com/) | Slovakia | 简历生成 | freemium | 简历+cover letter+个人网站 |
| 7 | [Hiveage](https://www.hiveage.com/) | Sri Lanka | 发票生成 | freemium | 自由职业者发票+计时+账单 |
| 8 | [Tape It](https://tape.it/) | Germany* | 音频处理 | subscription | 音乐人 iPhone 高音质录音+去噪 |
| 9 | [Wisecut](https://www.wisecut.ai/) | Brazil | 视频处理 | subscription | 自动剪短视频+字幕 |
| 10 | [Munch](https://www.getmunch.com/) | Israel | 创作者工具 | subscription | AI 挑长视频中"最 viral"片段 |

\* Tape It 是 Berlin / London / LA / Stockholm 分布式 5 人团队,核心地标 Berlin。

---

## 增长信号与研究价值速览

| # | 名称 | 关键增长信号 | 研究价值 |
|---|---|---|---|
| 1 | Tella | YC S20 + Launch HN + Amsterdam 6 人小团队 | YC 出身但讨论度远低于 Loom;'browser-first + 自带品牌'路径 |
| 2 | Screen Studio | Starter Story:9 个月 8K 客户 | Poland 单人 sole proprietorship,走 macOS 重投资路线 |
| 3 | Cleanvoice AI | Starter Story / SEO MRR +300% / Bucharest solo | 罗马尼亚 solo founder + 纯 SEO 获客 + AI 音频 niche |
| 4 | Sejda | 14 年持续运营 / 刻意低调 / 周卡 $5 定价 | Smallpdf 旁边的隐形赢家,几乎零 indie 报道 |
| 5 | DocSpring | PDF Association 收录创始人 / 长期 B2B API 续费 | Auckland NZ 独立开发者,从签证表单痛点起步 |
| 6 | Kickresume | GetLatka 公开 2024 营收 $1.9M + 8K 客户 | Resume.io 同赛道但讨论度甩开几条街,Bratislava 团队 |
| 7 | Hiveage | Wikipedia 收录 + 10+ 年存活 + 多平台付费评价 | Sri Lanka 全球 B2B SaaS 极罕见,稳吃 freelancer 长尾 |
| 8 | Tape It | TechCrunch x2 + Show HN + MusicTech | 垂直音乐 SaaS,$20/年破坏性定价 + 5 人分布式 |
| 9 | Wisecut | Tim Draper $1M 领投(总 $1.29M) + VentureBeat | Brazilian 兄弟,Latino founder 资源 + Tim Draper 渠道 |
| 10 | Munch | $7.2M Seed (A* Capital) + AdExchanger + MarTech 报道 | Israeli 团队,B2B agency 定位而非 YouTuber |

---

## 实现难度速览(供独立开发者参考)

| # | 名称 | 自研模型 | 需后端 | 核心 API/技术栈 | 单人 4 周 MVP |
|---|---|---|---|---|---|
| 1 | Tella | ❌ | ✅ | WebRTC + MediaRecorder + ffmpeg.wasm + S3 + Stripe | ❌ |
| 2 | Screen Studio | ❌ | ❌ | ScreenCaptureKit + AVFoundation + Swift/Metal + Lemon Squeezy | ❌ |
| 3 | Cleanvoice AI | ✅ | ✅ | Whisper/Deepgram + 自训去噪 filler 检测 + S3 + Stripe | ❌ |
| 4 | Sejda | ❌ | ✅ | PDFBox / iText / Ghostscript + S3 + Stripe | ❌ |
| 5 | DocSpring | ❌ | ✅ | Rails + React + pdftk/iText + S3 + Stripe | ❌ |
| 6 | Kickresume | ❌ | ✅ | OpenAI API + PDF 渲染 + Postgres + Stripe | ✅ |
| 7 | Hiveage | ❌ | ✅ | Rails/Node + Postgres + Stripe + 邮件发票渲染 | ✅ |
| 8 | Tape It | ✅ | ❌ | iOS AVFoundation + Core ML / 第三方去噪 + IAP | ❌ |
| 9 | Wisecut | ❌ | ✅ | Whisper + ffmpeg + 镜头/静音检测 + S3 + Stripe | ❌ |
| 10 | Munch | ❌ | ✅ | OpenAI/Anthropic + ffmpeg + 视觉裁切 + S3 + Stripe | ❌ |

8/10 不依赖自研模型;只有 Cleanvoice 和 Tape It 涉及自研音频 ML 模型;3/10 单人 4 周可做 MVP(Kickresume / Hiveage / 不需要大模型的发票/简历类)。Screen Studio 是唯一纯客户端、Tape It 是唯一纯 mobile + IAP。
