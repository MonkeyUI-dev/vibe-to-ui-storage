# Design seed — dify/home

> 页面级候选。**默认 apply 目标是产品**（`dify`）。仅在明确只要本页时用 `--page home`。
> Status: **preview only** — 用户确认前不要写入项目。
> Generated: 2026-07-26

## Page Context

- **Primary page type**: landing
- **Secondary**: brand showcase（材质/建筑摄影气氛）
- **Density**: low → medium
- **Interaction model**: 长滚动说服 + sticky 转化入口 + 章节 rail 浏览能力
- **Design consequences**: 大标题层级、稀缺蓝信号、真实 UI/视频证据、三路径部署对比；动效克制
- **Kinds**: observed / transferable

## Visual Direction

- 白纸上的生产级冷静：超大中性无衬线标题 + 单一饱和蓝作信号，气氛用建筑/地质摄影，功能用真 UI 与视频证明。
- **Kinds**: observed / transferable

## Colors

| Role | Direction | Kind |
|------|-----------|------|
| Canvas / paper | 近纯白；证据舞台可用深蓝块 | transferable |
| Ink | 近黑深墨，高对比正文 | transferable |
| Emphasis / signal | 单一蓝用于 CTA、关键词染色、关键点缀 | transferable |
| Brand identity hues | `#0033FF` 系与 logo「i」蓝点勿照搬 | brand-specific |

## Typography

- Heading posture: 超大、字重中等（~500）、极紧字距、关键词局部着色
- Body rhythm: 短副句、中等行宽、章节标题继续「大字 + 蓝染关键词」
- Font hints observed: Söhne / Söhne Mono（专有 → 迁移时换等价几何无衬线）
- **Kinds**: observed / transferable / brand-specific

## Motion

- 见同页 `motion.md`：150–200ms 色变反馈 + sticky 连续 + 产品视频气氛；无炫技编排。

## Do’s and Don’ts

### Do
- 顶栏固定主转化，英雄区留给主张与意象
- 用真实工作流 UI / 短视频作能力证据
- 多部署路径用等权三栏卡对比（托管 / 自托管 / 开源）
- 保持蓝信号稀缺，摄影底弱对比

### Don’t
- 把首屏做成功能仪表盘或密集卡片墙
- 复制 Dify 字标、客户 logo、具体摄影与营销句
- 堆叠紫色光晕、玻璃拟态装饰动效

## Transferable rules

- 白纸 + 近黑字 + 单一稀缺强调色，关键词局部染色形成节奏。_(transferable)_
- 社会证明（logo + 引言）紧跟产品舞台，再进入「如何获得」路径选择。_(transferable)_
- 能力叙事用「左证据画布 / 右章节 rail」。_(transferable)_
- 勿移植品牌标识与客户背书资产。_(brand-specific)_

## Apply gate

```bash
vibe-to-ui inspiration apply dify --project <path>
vibe-to-ui inspiration apply dify --page home --project <path>
vibe-to-ui inspiration apply dify --project <path> --confirm
```
