# vibe-to-ui-storage

[English](README.md) | 简体中文

[Vibe-to-UI](https://github.com/MonkeyUI-dev) 的 **Design Context** 存储仓库。用于跨项目、跨平台保存品牌语言、设计令牌与平台适配规则，供本地设计伴侣工具读取与同步。

> **Build the dream you were told to put away.**

## 这是什么

本仓库不是 Vibe-to-UI 工具本身，而是其 **Design Context Profile** 的远程副本。每个 Profile 描述一个品牌/产品/客户的视觉与叙事上下文，而非某个具体输出平台。

当前包含的 Profile：

| Profile | 说明 |
|---------|------|
| [`vibe-to-ui`](profiles/vibe-to-ui/) | Vibe-to-UI 产品自身的跨平台品牌主档 |

本地运行时，Profile 通常位于 `~/.vibe-to-ui/profiles/<profile>/`。本仓库可作为团队共享、版本追踪与备份的来源。

## 目录结构

```
profiles/
└── vibe-to-ui/
    ├── profile.md      # Profile 元数据与摘要
    ├── brand.md        # 跨平台品牌主档（视觉语言、原则、护栏）
    ├── tokens.json     # 设计令牌（W3C DTCG 格式）
    ├── decisions.md    # 设计决策日志（只追加，不删除）
    ├── sources/        # 提取来源记录
    └── targets/        # 各发布平台的适配规则
        ├── github.md
        └── xiaohongshu.md
```

### 各文件职责

- **`profile.md`** — Profile 身份、一句话描述、可用 target 列表与来源摘要。
- **`brand.md`** — 共享品牌语言：气质、色彩故事、字体、空间与动效性格、设计原则与护栏。
- **`tokens.json`** — 可机读的设计令牌（颜色、字体、间距、圆角、阴影、动效等），遵循 [W3C DTCG Design Tokens Format](https://www.designtokens.org/)。
- **`decisions.md`** — 设计记忆：记录「决定了什么、为什么、影响哪些文件」。
- **`targets/*.md`** — 在共享品牌基础上的平台适配（版式、信息层级、产出物规格等）。
- **`sources/*.md`** — 品牌提取所依据的原始来源与置信度说明。

## 品牌速览（vibe-to-ui）

Vibe-to-UI 是一套面向 vibe-coding 开发者的本地设计伴侣，帮助将参考、感受与产品语境转化为可用的视觉方向与可复用的 Design Context。

视觉系统为 **Dusty Pink Brutalist** 风格：

| 角色 | 色值 | 用途 |
|------|------|------|
| Dusty Pink | `#DDCED2` | 结构画布 |
| Ink Black | `#121212` | 层级、边框、硬阴影 |
| Cool White | `#F8F9FA` | 工作面板 |
| Electric Blue | `#003BFF` | 主操作与活跃状态（点缀，不作满版填充） |

更多细节见 [`profiles/vibe-to-ui/brand.md`](profiles/vibe-to-ui/brand.md) 与 [`profiles/vibe-to-ui/tokens.json`](profiles/vibe-to-ui/tokens.json)。

## 使用方式

### 克隆与浏览

```bash
git clone https://github.com/MonkeyUI-dev/vibe-to-ui-storage.git
cd vibe-to-ui-storage
```

### 与本地 Profile 同步

若你已在本地使用 Vibe-to-UI CLI，可将本仓库中的 Profile 复制或链接到本地目录：

```bash
# 示例：将 vibe-to-ui profile 同步到本地
cp -r profiles/vibe-to-ui ~/.vibe-to-ui/profiles/vibe-to-ui
```

> **注意**：`profile.md` 头部注明本地副本为活数据（live copy）。Skill 更新不应覆盖用户本地 Profile；本仓库提供的是种子/共享版本。

### 按平台查阅适配规则

- GitHub README 与文档视觉 → [`profiles/vibe-to-ui/targets/github.md`](profiles/vibe-to-ui/targets/github.md)
- 小红书封面与轮播 → [`profiles/vibe-to-ui/targets/xiaohongshu.md`](profiles/vibe-to-ui/targets/xiaohongshu.md)

## 贡献

1. 在 `decisions.md` 中记录新决策（只追加，旧条目标记为 superseded 而非删除）。
2. 品牌级变更更新 `brand.md` 与 `tokens.json`；平台级变更更新对应 `targets/<platform>.md`。
3. 勿将密钥、凭证或 `.env` 文件提交到仓库（见 [`.gitignore`](.gitignore)）。

## 许可证

[MIT License](LICENSE) — Copyright (c) 2026 MonkeyUI-dev
