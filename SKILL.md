---
name: exam-prep-system-designer
description: Design and build a personalized exam preparation support system after first diagnosing the user's exam goal, timeline, subject progress, study time, resources, memorization needs, wrong-question workflow, subjective-answer training, reminder needs, and preferred tools such as Obsidian, Anki, Feishu, WeChat, or XMind. Use when the user wants help creating, restructuring, or maintaining a long-cycle exam planning and review system, especially when requirements are unclear and need to be clarified before implementation.
---

# Exam Prep System Designer

## Core Rule

Do not start by applying a template. First diagnose the user's exam, constraints, habits, tools, and anxiety points, then design the lightest system that can work today.

Never assume:
- The user wants a complex system.
- The user will input everything in a fixed format.
- Wrong questions should become Anki cards.
- Obsidian is required.
- A homepage should contain every possible feature.

## Workflow

1. Needs discovery: identify exam type, remaining days, target score/result, subject progress, weak modules, available time, materials, and current pain points.
2. Planning: convert the target and available time into a total plan, phase plan, weekly rhythm, and daily minimum plan.
3. Module selection: add only the modules that solve the user's actual problems.
4. Implementation choice: choose tools and automation level based on the user's habits.
5. Build: create the smallest usable system first, then add visual polish and automation.
6. Verify: check links, templates, reminders, dashboards, and the user's first-day workflow.

## Ask In Batches

Start with the minimum questions needed. Use `references/needs-discovery.md` for the full question bank.

Batch 1: exam and goal
- What exam is this, and how many days remain?
- What is the target score/result?
- Which subjects or modules matter most?

Batch 2: current state and time
- What is the current progress for each subject?
- Which modules are weakest?
- What study time is guaranteed on weekdays and weekends?

Batch 3: system preference
- Does the user prefer a light checklist, a detailed dashboard, or both?
- Which tools are already used: Obsidian, Anki, Feishu, WeChat, XMind, handwritten notes, photos?
- What is the biggest problem: forgetting, wrong questions, subjective answers, procrastination, anxiety, messy materials, or schedule drift?

If the user asks to start immediately, build a minimum viable version with assumptions clearly stated, then ask for feedback after first use.

## Module Decision Rules

Use `references/module-selection.md` before proposing modules.

Common modules:
- Control module: daily plan, total progress, weekly review.
- Memorization module: records what was memorized and schedules review.
- Wrong-question module: logs errors, plans review, and tests transfer.
- Subjective-answer module: stores prompts, answers, scoring notes, revised answers, and reusable structures.
- English module: reading themes, vocabulary, writing corpus, template refinement.
- Political theory module: frameworks, logic, memory hooks, practice.
- Reminder module: morning plan and evening review through Feishu, WeChat, or local reminders.
- Knowledge-base module: organizes outputs into durable notes.

## Implementation Rules

Prefer the user's existing workflow. A system that is used daily is better than a beautiful one that is abandoned.

For Obsidian builds:
- Use native Markdown first.
- Use CSS snippets only for stable visual improvements.
- Use custom callouts and simple HTML only when Markdown cannot express the layout.
- Keep todo items as native checkboxes if the user wants to check them in Obsidian.
- Avoid plugin-dependent layouts unless the user has installed and accepted the plugin.
- A homepage should reduce anxiety by showing: today's tasks, total progress, current module progress, recent reviews, and clear entrances.

For Anki:
- Use knowledge-point cards for memorization.
- Do not turn every wrong question into a card by default.
- Generate cards from the user's own framework or mind map when possible.

For reminders:
- Do not hardcode secrets or webhooks into shared templates.
- Keep morning messages action-oriented and evening messages reflective.

## References

Load only the references needed for the current task:
- `references/needs-discovery.md`: requirement questions and intake logic.
- `references/planning-framework.md`: total plan, phase plan, weekly and daily planning.
- `references/module-selection.md`: decide which modules to include.
- `references/obsidian-implementation.md`: Obsidian folder, templates, plugin, and CSS guidance.
- `references/dashboard-design.md`: homepage/dashboard design principles.
- `references/reminder-system.md`: Feishu/WeChat/local reminder design.

Reusable Obsidian starter assets live in `assets/obsidian/`.
