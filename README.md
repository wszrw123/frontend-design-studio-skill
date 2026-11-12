# Frontend Design Studio

**A visual-first frontend product design and engineering skill for AI coding agents.**

Frontend Design Studio helps an agent move from requirements to a thoughtful visual direction, from image-led design to reusable components, and from implementation to evidence-based browser QA. It combines UI/UX judgment, frontend architecture, visual asset workflows, interaction-cost optimization, and practical engineering delivery.

[中文介绍](#中文介绍) · [Quick Start](#quick-start) · [Capabilities](#capabilities) · [Workflow](#workflow)

## Why Frontend Design Studio?

Many AI coding workflows jump from a screenshot straight to CSS. This skill adds the missing product-design and quality gates:

- Understand the business goal and user task before changing the interface.
- Preserve visual language and components that users already approve.
- Use image generation to explore high-fidelity design directions and required visual assets.
- Critique and iterate on the design before implementation.
- Reduce unnecessary input and interaction cost without hiding functionality.
- Reuse shared components and design tokens instead of creating one-off page styles.
- Compare the approved design with real browser output and verify complete task flows.

## Capabilities

| Area | What it provides |
|---|---|
| Requirements & scope | Clarify user goals, constraints, task paths, and authorized change scope |
| Visual design | Image-led redesign, visual language extraction, evidence-based design critique |
| Visual assets | Reuse or generate icon sets, illustrations, backgrounds, and empty states |
| Design system | Design tokens, component hierarchy, reusable page patterns, responsive rules |
| Interaction UX | Reduce redundant fields, clicks, waiting, and decision burden safely |
| Frontend engineering | Work within the existing framework, APIs, routes, permissions, and conventions |
| Quality assurance | Before/Target/After comparison, multi-viewport checks, accessibility, task-flow regression |

## Workflow

### Existing interface redesign

Requirements & scope → user task analysis → inspect screenshots and source code → extract approved visual language → Image redesign → independent design critique → interaction-cost optimization → component and asset planning → implementation → real-browser visual and task-flow acceptance.

### Greenfield design

Requirements → information architecture and task flow → visual direction → Image concept design → design critique and iteration → design tokens and component plan → implementation → responsive and business-flow acceptance.

## Design principles

1. **Understand before designing.** Existing interfaces must begin with requirements and real-state analysis.
2. **Design before coding.** An Image draft is not automatically a good design; critique and revise it before implementation.
3. **Preserve what works.** Extend approved visual language rather than replacing it without reason.
4. **Visual richness and operational simplicity are separate goals—and must be evaluated together.**
5. **Reuse before rebuilding.** Inspect component usage and impact before changing shared UI.
6. **Use real data semantics.** Distinguish zero, missing, unknown, loading, error, and no-permission states.
7. **Verify the real product.** A successful build is not visual QA; compare the approved target with clean browser screenshots.
8. **Be honest about tools.** If image generation, browser access, or test data is unavailable, report the blocker instead of claiming success.

## Quick Start

### Install for Codex / Agent Skills

Clone into your user-level skills directory:

```bash
git clone https://github.com/wszrw123/frontend-design-studio-skill.git ~/.agents/skills/frontend-design-studio
```

Windows PowerShell:

```powershell
gh repo clone wszrw123/frontend-design-studio-skill "$HOME\.agents\skills\frontend-design-studio"
```

To update an existing installation:

```bash
git -C ~/.agents/skills/frontend-design-studio pull --ff-only
```

Restart or refresh the agent client if the skill is not discovered immediately.

### Invoke

```text
$frontend-design-studio
```

Example:

```text
$frontend-design-studio

Understand the requirements and inspect the current page and codebase first.
Use Image to create a high-fidelity redesign, critique the draft before coding,
preserve approved visual language, reuse shared components, and optimize the
main user journey. Implement the approved direction and verify it in a real
browser across relevant viewports and data states.
```

## Repository structure

- `SKILL.md` — core skill instructions and workflow routing.
- `agents/openai.yaml` — agent-facing display name, description, and starter prompt.
- `references/` — detailed methods for redesign, critique, assets, components, interaction cost, state-driven layout, scope control, and QA.
- `templates/` — design briefs, review reports, visual-language audits, task-flow audits, and QA matrices.
- `docs/architecture.md` — workflow architecture diagrams.
- `examples/` — reusable invocation examples.

## Tool expectations

The skill provides methods and instructions; host-agent capabilities still matter:

- Image generation is required for needed visual assets when no suitable reusable asset exists. If the host cannot generate images, report the limitation and do not substitute emoji or text symbols for icons.
- Real-browser QA requires an available browser/runtime and valid access to the target project.
- Actual business-flow testing requires safe test data and authorized access.
- Never deploy, change production data, or trigger paid/external actions without authorization.

## Related skill

For a lighter, image-led UI and interaction-simplification workflow, see [image-led-ui-design](https://github.com/wszrw123/skills/tree/main/skills/image-led-ui-design).

## License

This project is licensed under the [MIT License](LICENSE).

---

## 中文介绍

**Frontend Design Studio 是一套面向 AI 编程助手的视觉驱动型前端产品设计与工程实施 Skill。**

它希望解决 AI 前端开发中常见的几个问题：没有理解需求就开始改页面、Image 生成的初稿未经评审就直接编码、页面看起来整齐却缺乏设计感、公共组件重复开发、视觉改造影响业务交互，以及代码构建成功却没有真实页面验收。

### 核心能力

- **需求与范围理解：** 先理解业务目标、用户角色、任务路径和不可改变的约束。
- **Image 驱动设计：** 使用 Image 生成高保真设计方向，并通过独立视角评审和必要迭代。
- **视觉语言继承：** 保留用户认可的设计区域、品牌色彩、字体、图标和组件模式。
- **视觉资产体系：** 统一规划图标、插画、背景图和空状态；缺少合适资产时按规则调用 Image 生成。
- **组件与设计系统：** 盘点公共组件引用，维护 Design Tokens，避免重复造轮子。
- **交互成本优化：** 减少重复输入、不必要点击、等待和决策，同时保护功能可发现性、用户控制权和业务安全。
- **工程实施与验收：** 基于现有技术栈实现，通过真实浏览器截图、跨视口检查和完整业务流程验收。

### 适用场景

已有 Web/H5 系统改造、移动端体验优化、PC 管理后台设计、企业工作台、组件库升级、设计系统建设，以及从零开始的新产品界面设计。

**核心理念：先理解，再设计；先评审，再编码；视觉与操作体验一起交付。**
