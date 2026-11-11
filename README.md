# Frontend Design Studio Skill

**视觉设计驱动的前端产品设计与工程实施 Skill**。先理解需求和任务，再继承有效的视觉语言；用 Image 设计并独立评审，优化操作成本，最终以真实页面和完整任务验收。

> Skill 版本：1.3.0；设计结构版本：V1.4。

## V1.3.0 融合能力

- **视觉语言继承**：提取用户明确满意的区域和现有品牌语言，区分保留、延伸、待验证和应修复，避免每轮重做。
- **交互成本优化**：从完整任务路径分析必填项、输入、点击、等待、决策和异常恢复，减少重复操作但不隐藏核心功能。
- **Image 资产流水线**：按职责生成/复用图标、插画、背景和场景图，检查透明通道、裁切、小尺寸效果、来源和归档。
- **范围控制**：尊重用户只分析、只设计或要求实施的不同授权；不强制技术栈、子 Agent、worktree 或部署。
- **产品体验验收**：视觉品质与任务操作成本分别评估、一起验收，验证保存、修改、取消、撤销、重试和持久化。

## V1.2.0 已有能力

- **证据式独立评审**：先从不同视角审查 Image 初稿，记录问题区域、用户影响及复评结果，不允许自行打高分后直接编码。
- **真实内容驱动布局**：正确处理零值、无数据、未知、加载失败、长文案和密集数据。
- **三图差异闭环**：已有界面基线图（Before）→ 评审通过的 Image 设计稿（Target）→ 真实运行截图（After）。
- **多视口×状态×交互**：记录实际检查覆盖，包含完整滚动、固定导航、弹窗及关联组件回归。
- **通用质量反馈**：把失败归因到设计、数据、组件或验收规则，不写入任何页面专属补丁。

## V1.1.0 已有能力

- 设计评审门禁和通用设计质量量表。
- 产品视觉个性，避免无差别套用后台模板。
- 数据真实性、状态表达和可访问性检查。
- 干净截图验收，避免浏览器检查器覆盖层混入产品截图。

## 核心工作流

**视觉丰富与操作简单分别设计、一起验收。** 已有项目优先继承用户认可的视觉语言；交互优化从完整用户任务路径出发；最终同时验收视觉、操作成本和业务闭环。

### 已有界面改造

需求理解与范围确认 → 用户任务路径 → 现状与源码分析 → 视觉语言提取 → Image 重设计 → 证据式设计评审 → 交互成本优化 → 组件/资产拆解 → 代码实现 → 三图差异与任务闭环验收 → 经验沉淀。

### 从零开始设计

需求理解与范围确认 → 任务流程/信息架构 → 视觉方向 → Image 设计 → 证据式设计评审 → 交互成本优化 → 组件与资产准备 → 代码落地 → 视觉与业务任务验收。

## 目录结构

```text
frontend-design-studio-skill/
├── SKILL.md
├── README.md
├── CHANGELOG.md
├── LICENSE
├── agents/
│   └── openai.yaml
├── docs/
│   └── architecture.md
├── references/
│   ├── existing-interface-redesign.md
│   ├── greenfield-design.md
│   ├── design-critique.md
│   ├── visual-language-extraction.md
│   ├── interaction-cost-optimization.md
│   ├── image-asset-pipeline.md
│   ├── scope-control.md
│   ├── experience-acceptance.md
│   ├── state-driven-layout.md
│   ├── visual-diff.md
│   ├── quality-feedback-loop.md
│   ├── image-prompt-playbook.md
│   ├── visual-assets.md
│   ├── component-governance.md
│   └── visual-qa.md
├── templates/
│   ├── design-brief.md
│   ├── design-review-report.md
│   ├── visual-language-audit.md
│   ├── task-flow-audit.md
│   ├── viewport-state-matrix.md
│   ├── visual-diff-report.md
│   ├── component-audit.md
│   ├── asset-inventory.csv
│   └── visual-qa-report.md
└── examples/
    └── example-requests.md
```

## 安装与使用

将仓库克隆或更新到 Agent Skills 目录，并确保 `SKILL.md` 位于 Skill 根目录。常见个人目录：

```text
~/.agents/skills/frontend-design-studio/SKILL.md
```

在支持 Agent Skills 的客户端中显式调用：

```text
$frontend-design-studio
```

## 重要约束

- Image 设计稿是实现参考，不是整页背景图片。
- 正式图标不得用 Emoji、字符、普通符号或字母缩写代替。
- 没有合适可复用视觉资产时，对设计确实需要的素材必须调用 Image 生成。
- 设计稿必须先经过证据式独立视角评审和必要迭代，再进入编码；没有独立 Agent 时不得假装调用。
- 必须用真实数据状态与内容压力检查视觉层级，不得编造趋势或混淆零值/无数据。
- 必须对照设计稿与真实截图检查差异，记录视口、状态、交互覆盖和未验证项。
- 用户满意的视觉区域优先保留和延伸；不要每轮无理由推翻。
- 不得为了减少点击隐藏核心功能、跳过权限/审计或擅自触发外部动作。
- 任务成本改善数据必须区分实测与估计。
- 不破坏原有 API、路由、权限和业务行为。
- 不擅自扩大改造范围、部署、发版或触发未授权的付费/外部动作。
- 无法调用图像生成或无法启动真实浏览器时，必须如实报告，不得伪造完成状态。

## 版本

- Skill：`1.3.0`
- 设计架构：`V1.4`
- 变更记录见 [CHANGELOG.md](CHANGELOG.md)。
