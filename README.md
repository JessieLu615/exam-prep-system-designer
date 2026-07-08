# Exam Prep System Designer

一个用于设计个性化考试复习系统的 Codex Skill。

它不是一个固定模板，而是一套“先确认需求，再搭建系统”的工作流。适合用来帮助长期备考者搭建复习计划、背诵系统、错题复盘、主观题题库、提醒系统和 Obsidian 知识库。

## 适合谁使用

这个 Skill 适合以下场景：

- 正在准备考研、法考、公考、资格考试、语言考试或其他长周期考试。
- 复习内容多，需要同时管理进度、背诵、做题和复盘。
- 想把 ChatGPT/Codex 作为复习总入口。
- 想搭建 Obsidian、Anki、飞书、微信、XMind 等工具组合。
- 需求还不完全清楚，需要先被提问、澄清，再开始搭建系统。

## 核心理念

这个 Skill 的核心不是“直接套一个看板”，而是：

1. 先确认考试目标、剩余时间、科目进度、可用学习时间和薄弱模块。
2. 再判断使用者真正需要哪些模块。
3. 最后选择合适的工具和实现方式。

它会避免以下常见问题：

- 一上来就搭建复杂系统，最后没人用。
- 默认所有人都需要 Obsidian 或 Anki。
- 默认错题都要变成 Anki 卡片。
- 默认使用者会按固定格式输入。
- 首页功能太多，反而增加焦虑。

## 它能做什么

### 1. 需求诊断

Skill 会先询问：

- 考试类型和剩余时间。
- 目标分数或目标结果。
- 各科当前进度和薄弱模块。
- 工作日、周末可用时间。
- 使用者已有资料和工具。
- 最大问题是遗忘、错题、主观题、拖延、焦虑，还是资料混乱。

### 2. 总规划

根据目标和时间，生成：

- 总复习规划。
- 阶段规划。
- 周计划。
- 每日最低可执行计划。
- 缓冲和调整机制。

### 3. 模块选择

根据需求选择必要模块，例如：

- 总控模块。
- 背诵模块。
- 错题复盘模块。
- 主观题题库模块。
- 英语专项模块。
- 政治或专业课专项模块。
- 提醒系统。
- Obsidian 知识库。

### 4. Obsidian 仪表盘

内置一个可复用的 Obsidian 起始模板，包括：

- 今日 Todo。
- 总任务完成占比。
- 本周状态。
- 模块进度。
- 当前任务表。
- 最近复盘。
- 常用入口。

模板使用稳定的 Markdown、Callout 和 CSS 片段，尽量减少对插件的依赖。

### 5. 背诵与错题复盘

支持：

- 从使用者自己做的框架或思维导图中提炼知识点卡片。
- 记录每日背诵内容。
- 安排复习节奏。
- 将错题单独归因和复盘。
- 通过提问检验知识点是否真正掌握。

## 目录结构

```text
exam-prep-system-designer/
  SKILL.md
  agents/
    openai.yaml
  references/
    needs-discovery.md
    planning-framework.md
    module-selection.md
    obsidian-implementation.md
    dashboard-design.md
    reminder-system.md
  assets/
    obsidian/
      homepage-template.md
      dashboard-css.css
      exam-homepage.svg
      review-pool-template.md
      memorization-template.md
      subjective-bank-template.md
```

## 快速使用

在 Codex 中可以这样触发：

```text
Use $exam-prep-system-designer to design a personalized study planning and review system for my exam.
```

中文也可以直接说：

```text
帮我根据我的考试目标、剩余时间和学习情况，设计一个考试复习辅助系统。
```

如果要搭建 Obsidian 系统，可以说：

```text
我想用 Obsidian 搭建一个考试复习看板，请先确认我的需求，再帮我设计。
```

## 使用建议

第一次使用时，建议先提供：

- 考试名称。
- 剩余天数。
- 目标分数或目标结果。
- 各科当前进度。
- 每天和每周可用学习时间。
- 当前最焦虑或最混乱的问题。
- 你已经在用的工具。

如果不想一次输入太多，也可以只说“你先问我必要问题”，让 Skill 分批提问。

## 注意事项

- 不要把私人 Webhook、飞书密钥、微信配置或个人资料上传到公开仓库。
- Obsidian 模板只是起点，应该根据考试和使用习惯调整。
- 如果只想要轻量系统，不需要启用所有模块。
- 如果使用 Anki，建议优先做知识点卡片，不要把所有错题机械转成卡片。

## License

You can add your preferred license here, such as MIT, CC BY-NC, or a private-use notice.
