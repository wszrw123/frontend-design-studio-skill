# Frontend Design Studio Skill

**视觉设计驱动的前端设计与工程实施 Skill**。先理解需求，再分析现状；先做 Image 视觉设计，再拆解组件；最后实现代码并通过真实页面验收。

> Skill 版本：1.0.0；设计结构版本：V1.1。

## 核心能力

- 已有界面改造：需求理解 → 现状截图/页面分析 → Image 重设计 → 设计拆解 → 公共组件升级 → 页面实现 → 真实验收 → 资产沉淀。
- 从零开始设计：需求理解 → 页面规划 → Image 设计 → 设计拆解 → 组件与资产准备 → 代码落地 → 真实验收。
- 视觉资产治理：优先复用现有资产；没有合适图标、插画、背景图、Banner 或空状态素材时，必须使用 Image 模型生成。
- 组件复用：先盘点已有组件及引用范围，优先升级已有公共组件，避免重复造轮子和过度抽象。
- 真实验收：真实浏览器截图、交互测试、响应式检查和公共组件回归。

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
│   ├── image-prompt-playbook.md
│   ├── visual-assets.md
│   ├── component-governance.md
│   └── visual-qa.md
├── templates/
│   ├── design-brief.md
│   ├── component-audit.md
│   ├── asset-inventory.csv
│   └── visual-qa-report.md
└── examples/
    └── example-requests.md
\`\`\`

## 安装

### Codex / Agent Skills

将整个仓库克隆或下载到 Agent Skills 目录，并确保 \`SKILL.md\` 位于 Skill 根目录。常见个人目录为：

\`\`\`text
~/.agents/skills/frontend-design-studio/SKILL.md
\`\`\`

也可放入项目级目录：

\`\`\`text
<project>/.agents/skills/frontend-design-studio/SKILL.md
\`\`\`

如果你的运行环境使用不同的 Skills 搜索目录，请按该环境的安装约定放置整个目录。

### 使用示例

\`\`\`text
使用 frontend-design-studio skill，先理解本次优化目标，再分析当前页面。
以当前真实页面截图为参考，调用 Image 生成高保真重设计稿；盘点可复用组件和视觉资产，
缺少合适图标/背景/插画时必须生成，不要用符号或 Emoji 代替；完成代码实现并进行真实浏览器验收。
\`\`\`

## 重要约束

- 不把 Image 设计稿直接作为网页背景。
- 不用 Emoji、字符、普通符号或字母缩写代替正式图标。
- 没有合适可复用的视觉资产时，必须调用 Image 模型生成；如果执行环境不支持图像生成，明确报告阻塞，不得伪造生成结果。
- 不破坏原有 API、路由、权限和业务行为。
- 代码完成不等于视觉验收完成；无法打开真实页面时必须明确说明。

## 版本

- Skill：\`1.0.0\`
- 设计架构：\`V1.1\`
- 变更记录见 [CHANGELOG.md](CHANGELOG.md)。
