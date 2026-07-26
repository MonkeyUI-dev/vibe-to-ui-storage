# Design seed — product dify

> **产品级**候选，供项目 `DESIGN.md`（默认 `inspiration apply` 目标）。
> Status: **preview only** — 用户确认前不要写入。
> Generated: 2026-07-26

## Product Context

- **Inspiration product**: dify
- **Primary host**: dify.ai
- **Surfaces collected**:
  - `home` (landing, full-scroll) — Dify - 构建生产级 AI 应用
- **Page-type mix**: landing

## Visual Direction (cross-page)

- 白纸上的生产级冷静：超大无衬线主张、稀缺蓝信号、建筑/地质摄影气氛，以及真实工作流 UI / 产品视频证据。
- 适配到用户产品时保留 landing 的疏密节奏，不要压成工作台密度。
- **Kinds**: observed / transferable

## Colors

| Role | Direction | Kind |
|------|-----------|------|
| Canvas / paper | 近纯白；证据舞台可用深蓝块 | transferable |
| Ink | 近黑深墨，高对比 | transferable |
| Emphasis / signal | 单一饱和蓝：CTA、关键词染色、点缀 | transferable |
| Brand identity hues | Dify 蓝与 logo「i」点勿照搬 | brand-specific |

## Typography

- 招牌式大标题（中等字重、紧字距）+ 蓝染关键词母题；正文短段。
- 迁移时换等价几何无衬线，勿绑定 Söhne。
- **Kinds**: transferable / brand-specific

## Motion

- 产品动效人格：克制反馈（≤200ms）+ sticky 连续 + 可选产品视频气氛。
- 签名母题：蓝染关键词与深蓝圆角产品舞台，而非滚动编排。

## Do’s and Don’ts

### Do
- 默认 apply **产品** seed
- 用全滚动证据，不用英雄一图定调
- 保留「主张 → 证明 → 路径 → 能力 → 收口」节拍
- 三路径对比卡 + 左 UI / 右 rail 结构可迁移

### Don’t
- 无 `--confirm` 写入 `DESIGN.md`
- 复制字标、客户 logo、摄影与原文
- 把每张表面都做成同一套英雄落地页

## Apply gate

```bash
vibe-to-ui inspiration apply dify --project <path>
vibe-to-ui inspiration apply dify --project <path> --confirm
vibe-to-ui inspiration apply dify --page home --project <path> --confirm
```
