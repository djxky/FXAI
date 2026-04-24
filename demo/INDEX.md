# demo · 导航

> 最后更新：2026-04-23 · 飞象 AI · v8.4 演示链路

## 当前主推（要给老板看的）

### 首页
- ⭐ **`v22-home-options/N1-plus.html`** — 主版本（待 v8.4 拍板后更新）
- 🧪 `v22-home-options/N1-plus-lab.html` — 设计实验台（4 组切换器：chip 形态 / 建议位置 / 班级卡详简 / 实体区顺序）
- 📋 `v22-home-options/index.html` — 首页 N1-N6 对比物料（汇报用）

### 飞象 AI 对话页（P3）
- ⭐ **`v23-ai-conversation/dialog-composition-grading.html`** — 基于某批作文批改数据的学情对话
  - 顶部 context 条：当前对话锚定的批次（高一(3)班 议论文 48 份《我的母亲》）
  - 主体：用户提问 + AI 回答 + 学情快照卡（5 维 / 分布 / 焦点学生） + 推荐下一步 chip
  - 下一步 chip 跳现有专业页（逐篇审改 / 看 7 篇待提升 / 范读候选 / 课堂订正小练 / 班级讲评 / 配置下载）
  - 底部 composer：可继续追问（追问范围 = 当前批次）

### 已打通的跳转链路
- 首页 (`N1-plus.html`) → 选「作文批改」chip → 选批次 → 发送 → 学情对话页（带 query `?q=`）

### 待做（P4-P6）
- ⬜ `v24-composition/` — 作文模块 AI 化首页（颠覆"布置作文"）
- ⬜ `v25-grading-with-aside/` — 现有作文批改页 + 飞象 AI 侧栏（演示无处不在）
- ⬜ 对话页：流式回答、追问后真渲染新消息、context 切换面板
- ⬜ 演示模式（▷ 自播放脚本）

## v22-home-options 内 N 系列说明

| 文件 | 角色 | 状态 |
|---|---|---|
| `N1-plus.html` | 推荐稿主版本 | ⭐ 主推 |
| `N1-plus-lab.html` | 实验台 · 多组切换 | 🧪 决策中 |
| `index.html` | N1-N6 对比物料 | 📋 汇报用 |
| `N1-rich-top-chip-out.html` | 丰富 / 上 / chip 外 (GPT 风) | 已淘汰 |
| `N2-rich-top-chip-in.html` | 丰富 / 上 / chip 内 (豆包风) | 已淘汰 |
| `N3-light-top-chip-in.html` | 简洁 / 上 / chip 内 (Claude 风) | 已淘汰 |
| `N4-rich-bottom-chip-out.html` | 丰富 / 下 / chip 外 (Cursor 风) | 已淘汰 |
| `N5-light-bottom-chip-in.html` | 简洁 / 下 / chip 内 (Notion AI 风) | 已淘汰 |
| `N6-pure-chat.html` | 纯对话 / 实体全收侧栏 (对照组) | 对照组 |

## archive · 历史归档

- `archive/early-explorations/` — v1-v19 早期探索（30+ 个文件）
- `archive/v20-agent-flow/` — v20 探索
- `archive/v21-home-options/` — v21 首页探索
- `archive/home-explore-codex/` — codex 早期方案
- `archive/opus demo/` — opus 早期 demo
- `archive/首屏探索-第1轮/` — 第一轮首屏
- `archive/N1-plus-suggest.html` — 已被 N1-plus-lab 包含

## 模块边界（v8.4 共识）

- **飞象 AI** = 全局智能层 + 上层调度
- **保留专业页**：作文批改 / 作文学情 / 作业批改 / 作业学情 / 报告下载（部分）
- **AI 颠覆候选**：布置作文 / 作文列表筛选 / 报告下载配置
- **不做单独入口**：飞象老师 / 学练机
