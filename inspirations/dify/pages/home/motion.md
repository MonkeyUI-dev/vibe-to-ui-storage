# Motion — dify/home

> 实机短观察：加载 → 全页滚动 → 顶栏/CTA hover。未切换 `prefers-reduced-motion`（工具限制）。置信度：中高。

## Observation checklist

- [x] Page load / entrance — 首屏静态排版立即可读；英雄右侧摄影静态；下方深蓝舞台内嵌视频自动播放（控件可见「暂停/播放」）
- [x] Scroll / in-view — sticky 顶栏全程钉住；滚动本身平滑，未见强 parallax 或全页滚动劫持
- [x] Hover / focus — 顶栏链接与主按钮使用 150–200ms 颜色/`background-color` 过渡（`cubic-bezier(0.4,0,0.2,1)` / `(0,0,0.2,1)`）
- [ ] Optional: tab / modal — 能力区 Agent radio 点击被 sticky/拦截，未完成切换；结构上为竖向 rail 切换证据画布（推断为瞬时或轻淡入）
- [ ] `prefers-reduced-motion` — 未验证

## Motion DNA

| Dimension | Notes | Confidence |
|-----------|-------|------------|
| Roles | feedback（控件色变）、continuity（sticky nav）、atmosphere（视频循环） | high |
| Triggers | load（视频起播）、scroll（钉住顶栏）、hover（链接/按钮） | high |
| Tempo | snappy–moderate（150–200ms） | high |
| Easing character | Material-ish ease（cubic-bezier 标准减速） | high |
| Density | minimal / selective — 无装饰粒子场、无入场编排瀑布 | high |
| Signature motif | **稀缺蓝强调词 + 深蓝圆角产品舞台（含循环视频）**；动效服务于「生产可信」，不抢字 | medium–high |
| Reduced motion | 推断：关闭/简化视频自动播放与非必要 transition；未实测 | low |

## Transferable rules

- B2B landing：优先 **短时颜色反馈 + sticky 导航连续性**，把「氛围」交给摄影与一段产品视频，而不是滚动触发的复杂 choreography。
- 主按钮过渡保持 ≤200ms，避免 spring 弹跳。
- 若用视频作证据舞台，提供明确暂停控件，并在 reduced-motion 下默认静帧。

## Brand-specific (do not copy)

- 英雄区具体视频内容与深蓝舞台构图
- Dify 字标「i」蓝点的微交互（若有）
- 客户 logo 墙任何滚动/交错动画（若后续出现）
