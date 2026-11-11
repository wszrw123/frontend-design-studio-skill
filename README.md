# Frontend Design Studio Skill

**视觉设计驱动的前端设计与工程实施 Skill**。先理解需求，再分析现状；先用 Image 设计，再进行独立评审和迭代；设计通过后拆解组件、实现代码，最后进行真实页面验收。

> Skill 版本：1.1.0；设计结构版本：V1.2。

## V1.1.0 新增能力

- **设计评审门禁**：Image 生成的第一版设计稿不能直接进入编码，必须先检查业务适配、信息层级、视觉个性、资产质量、交互、响应式、可访问性和工程可实现性。
- **设计质量量表**：用统一标准识别设计短板，记录证据和修订动作，不用“好看/高级”这种空泛判断。
- **设计方向与产品识别度**：避免无差别套用通用后台模板，建立符合品牌和业务的视觉语言。
- **数据与状态真实性**：区分零值、无数据、未知、加载中和错误；不编造图表、趋势或业务数字。
- **可访问性检查**：加入 WCAG AA 对比度、键盘焦点、触控区域和语义标签检查。
- **干净截图验收**：明确关闭浏览器调试/无障碍检查器覆盖层，避免把检查工具的高亮误认为产品 UI。

## 核心工作流

### 已有界面改造

需求理解 → 现状截图/页面分析 → 视觉方向定义 → Image 重设计 → 设计评审与迭代 → 设计拆解与资产策略 → 组件复用与抽象 → 代码实现 → 真实页面验收 → 资产沉淀。

### 从零开始设计

需求理解 → 页面规划 → 视觉方向定义 → Image 设计 → 设计评审与迭代 → 设计拆解 → 组件与资产准备 → 代码落地 → 真实页面验收 → 资产沉淀。

## 目录结构

\`\`\`text
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
│   ├── image-prompt-playbook.md
│   ├── visual-assets.md
│   ├── component-governance.md
│   └── visual-qa.md
├── templates/
│   ├── design-brief.md
│   ├── design-review-report.md
│   ├── component-audit.md
│   ├── asset-inventory.csv
│   └── visual-qa-report.md
└── examples/
    └── example-requests.md
\`\`\`

## 安装与使用

将仓库克隆或更新到 Agent Skills 目录，并确保 \`SKILL.md\` 位于 Skill 根目录。常见个人目录：

\`\`\`text
~/.agents/skills/frontend-design-studio/SKILL.md
\`\`\`

在支持 Agent Skills 的客户端中显式调用：

\`\`\`text
$frontend-design-studio
\`\`\`

## 重要约束

- Image 设计稿是实现参考，不是整页背景图片。
- 正式图标不得用 Emoji、字符、普通符号或字母缩写代替。
- 没有合适可复用视觉资产时，对设计确实需要的素材必须调用 Image 生成。
- 设计稿必须先经过独立评审和必要迭代，再进入编码。
- 不破坏原有 API、路由、权限和业务行为。
- 真实视觉验收必须使用干净页面截图；检查器覆盖层应与产品截图分开。
- 无法调用图像生成或无法启动真实浏览器时，必须如实报告，不得伪造完成状态。

## 版本

- Skill：\`1.1.0\`
- 设计架构：\`V1.2\`
- 变更记录见 [CHANGELOG.md](CHANGELOG.md)。
