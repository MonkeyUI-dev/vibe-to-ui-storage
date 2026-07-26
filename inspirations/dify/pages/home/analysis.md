# Aesthetic analysis — dify/home

> 基于 https://dify.ai/zh 全页滚动截图（fullpage + frame-01…07）与实机观察完成。文案语言跟随用户提示（中文）。

## Meta

- **Title**: Dify - 构建生产级 AI 应用
- **Product**: dify
- **Page**: home
- **Source**: https://dify.ai/zh
- **Collected**: 2026-07-26T04:00:45Z
- **Enriched**: 2026-07-26T04:10:00Z
- **Page type**: landing（次级：品牌展示 / 企业 SaaS 转化）
- **Density**: low → medium（首屏极疏；中段证据与三栏部署抬到 medium）
- **Confidence**: high
- **Evidence**: 说服型叙事、强英雄层级、产品视频/UI 证据、三档部署卡片、功能 rail、收尾 CTA、页脚合规背书
- **Categories covered**: composition, color, typography, space-components, visual-evidence, narrative
- **Capture coverage**: full-scroll
- **Scope**: URL 页面 — 全滚动视觉定位

## Stage 0 — 页面类型

| 项 | 判断 |
|----|------|
| Primary | Landing / marketing |
| Secondary | Brand showcase（建筑/材质摄影作气氛层） |
| Density | low（首屏）→ medium（logo 墙 / 部署三栏 / 功能拆分） |
| Confidence | high |
| Design consequences | 大标题 + 稀缺蓝强调；真实产品 UI/视频作证据；段落用摄影与浅灰底切换节奏；动效克制（150–200ms） |

## Judgment legend

| Kind | Meaning |
|------|---------|
| `observed` | 对应截图带内直接可见 |
| `inferred` | 基于观察的设计推断 |
| `transferable` | 可迁移到其他项目 |
| `brand-specific` | 属于品牌本体，勿照搬 |

## Full-scroll visual positioning

| Scroll band | Frame(s) | Visual job | Density | Notes |
|-------------|----------|------------|---------|-------|
| Hero / entry | frame-01 | 定位主张 + 品牌字标 + 右侧材质摄影 | low | 左文右图；「生产级」用品牌蓝染色 |
| Product stage | frame-02 | 圆角视频/产品舞台 + 开始社会证明标题 | low–medium | 深蓝舞台、白线粒子；sticky 顶栏始终在场 |
| Proof / logos | frame-03 | Logo 网格 + 客户引言 + 岩石摄影 | medium | 左图右证；引言与 logo 交织 |
| Deploy choice | frame-04 | 三栏部署路径（云 / 企业 / 开源） | medium | 建筑摄影浅底；卡片等权对比 |
| Capability | frame-05 | Workflow 真 UI + 右侧能力 rail | medium | 左证据右导航；功能章节切换 |
| Closing CTA | frame-06 | 商业价值收口 + 主次 CTA | low | 雪山弱背景；蓝字强调「商业价值」 |
| Footer | frame-07 | 链接列 + 合规章 + 大字标 | medium | 白底信息架构；logo「i」保留蓝点 |

## 1. Composition & visual hierarchy

- **observed**: 首屏为经典左右分栏：超大 Söhne 标题占左上，右侧竖向混凝土柱摄影形成「结构/建造」隐喻；主 CTA「开始使用」落在 sticky 顶栏右端，而非英雄区内。(`frame-01`)
- **observed**: 中段改用「证据舞台」：先全宽深蓝圆角视频卡，再进入左摄影 / 右 logo+引言的证明带，再切到三栏部署与左 UI / 右 rail 的能力带。(`frame-02`–`05`)
- **transferable**: Landing 可把主转化按钮固定在顶栏，英雄区只保留主张与意象，避免首屏堆叠双 CTA 与功能网格。
- **brand-specific**: Dify 字标形态与「i」的蓝点锁定。

## 2. Color & value

- **observed**: 画布近纯白 `#fff`；正文近黑 `rgb(1,9,22)` / oklch 深墨；强调色为饱和蓝 `rgb(0,51,255)`，用于 CTA 填充、标题关键词染色、logo「i」。(`frame-01`, `frame-06`)
- **observed**: 价值带用深蓝填充大圆角舞台；部署带用浅棕建筑摄影作弱底；CTA 带用高调雪山摄影淡入。(`frame-02`, `frame-04`, `frame-06`)
- **transferable**: 白纸 + 近黑字 + **单一稀缺蓝信号**；摄影底只作氛围，不抢文字对比。
- **brand-specific**: 精确蓝值与蓝染色关键词策略。

## 3. Typography & typesetting

- **observed**: 全局 `Söhne`（Mono 用于代码感局部）；H1 ≈ 96px / weight 500 / 极紧字距（约 -2.8px）/ 行高≈字号，形成「建筑招牌」式标题。(`frame-01`, CSS)
- **observed**: 章节标题继续用大字号 + 关键词蓝染（「共同选择」「部署」「一切」「商业价值」）；正文短段、中等行宽。(`frame-02`–`06`)
- **transferable**: 中等字重大标题 + 关键词局部着色，比全标题纯色更有节奏；导航保持 14px 冷静。
- **brand-specific**: 专有字体 Söhne 本身。

## 4. Space & component language

- **observed**: sticky 顶栏矮（`--nav-h` 约 44–60px）、透明/白底、圆角 8px 主按钮；部署区三张等宽白卡片，圆角中等、轻阴影/细边，清单 + 底部按钮。(`frame-01`, `frame-04`)
- **observed**: 能力区左侧大圆角产品画布，右侧竖向 radio/rail（Workflow / Agent / 知识流水线 / 插件 / 发布与监控）。(`frame-05`)
- **transferable**: 「三路径对比卡」+「左证据 / 右章节 rail」适合 B2B 平台落地页；组件皮肤可换，结构可借。
- **inferred**: 阴影克制，主要靠圆角与色块分区，而非多层 elevation。

## 5. Visual evidence

- **observed**: 可信度来自三层：① 英雄后立刻出现的产品视频/深蓝舞台；② 全球企业 logo 墙 + 客户引言；③ Workflow Studio 真节点画布截图。合规章（GDPR / SOC2 / ISO）出现在部署卡与页脚。(`frame-02`–`05`, `frame-07`)
- **observed**: 气氛摄影（混凝土柱、岩石、古典柱廊、雪山）承担品牌气质，不直接解释功能。(`frame-01`, `frame-03`, `frame-04`, `frame-06`)
- **transferable**: 功能证明用真实 UI；品牌气质用非 UI 摄影；合规徽章贴近「可部署/可采购」决策点。
- **brand-specific**: 具体客户 logo、引言原文、摄影素材库。

## 6. Page narrative

- **observed** 节拍：主张（生产级 Agentic）→ 产品舞台 → 社会证明 → 部署路径选择 → 能力拆解 → 商业价值 CTA → 页脚资源/合规。
- **transferable**: 先定「为何可信」，再给「怎么买/怎么部署」，最后才深挖能力细节，适合开源+云+企业多路径产品。

## 7. Motion (see motion.md)

- 实机：英雄区视频自动播放；sticky 顶栏跟随滚动；控件 hover 约 150–200ms `cubic-bezier` 颜色过渡；未见 Framer/GSAP/Lottie 全局库。
- 签名动机：**关键词蓝染 + 深蓝产品舞台入场**，动效本身极克制。

## Capture notes

- Captures: `fullpage.jpg`（视口帧纵向拼接）+ `frame-01.jpg`…`frame-07.jpg`
- Prefer JPEG ~1440px 宽；已写入 `~/.vibe-to-ui/inspirations/dify/pages/home/captures/`
