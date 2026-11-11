# Frontend Design Studio Skill

**视觉设计驱动的前端设计与工程实施 Skill**。先理解需求，再分析现状；先用 Image 设计，再进行独立评审和迭代；设计通过后拆解组件、实现代码，最后进行真实页面验收。

> Skill 版本：1.2.0；设计结构版本：V1.3。

## V1.2.0 新增能力

- **证据式独立评审**：先从不同视角审查 Image 初稿，记录问题区域、用户影响及复评结果，不允许自行打高分后直接编码。
- **真实内容驱动布局**：正确处理零值、无数据、未知、加载失败、长文案和密集数据；不让占位符成为最大视觉焦点。
- **三图差异闭环**：已有界面基线图（Before）→ 评审通过的 Image 设计稿（Target）→ 真实运行截图（After）。
- **多视口×状态×交互**：记录实际检查覆盖，包含完整滚动、固定导航、弹窗及关联组件回归。
- **通用质量反馈**：把失败归因到设计、数据、组件或验收规则，不写入任何页面专属补丁。

## V1.1.0 已有能力

- **设计评审门禁**：Image 生成的第一版设计稿不能直接进入编码，必须先检查业务适配、信息层级、视觉个性、资产质量、交互、响应式、可访问性和工程可实现性。
- **设计质量量表**：用统一标准识别设计短板，记录证据和修订动作，不用“好看/高级”这种空泛判断。
- **设计方向与产品识别度**：避免无差别套用通用后台模板，建立符合品牌和业务的视觉语言。
- **数据与状态真实性**：区分零值、无数据、未知、加载中和错误；不编造图表、趋势或业务数字。
- **可访问性检查**：加入 WCAG AA 对比度、键盘焦点、触控区域和语义标签检查。
- **干净截图验收**：明确关闭浏览器调试/无障碍检查器覆盖层，避免把检查工具的高亮误认为产品 UI。

## 核心工作流

### 已有界面改造

需求理解 → 现状截图/页面分析 → 视觉方向 → Image 重设计 → 证据式设计评审与修订 → 状态与组件拆解 → 代码实现 → 三图差异/多状态验收 → 质量经验沉淀。

### 从零开始设计

需求理解 → 页面规划与状态约束 → 视觉方向 → Image 设计 → 证据式设计评审与修订 → 组件与资产准备 → 代码落地 → 设计稿/实现差异验收。

## 目录结构

```text
frontend-design-studio-skill/
├── SKILL.md
├── README.md
├── CHANGELOG.md
├── LICENSE
├── docs/
│   └── architecture.md
├── references/
│   ├── existing-interface-redesign.md
│   ├── greenfield-design.md
│   ├── design-critique.md
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
- 不破坏原有 API、路由、权限和业务行为。
- 真实视觉验收必须使用干净页面截图；检查器覆盖层应与产品截图分开。
- 无法调用图像生成或无法启动真实浏览器时，必须如实报告，不得伪造完成状态。

## 版本

- Skill：`1.2.0`
- 设计架构：`V1.3`
- 变更记录见 [CHANGELOG.md](CHANGELOG.md)。
