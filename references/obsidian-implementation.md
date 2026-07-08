# Obsidian Implementation

Obsidian is an optional implementation, not the system itself. Use it when the user wants local notes, dashboards, templates, and durable retrieval.

## Recommended Folder Structure

```text
00_Control/
  Daily/
  Weekly Review/
  Total Plan.md
  Homepage.md
01_Subject_A/
02_Subject_B/
03_Subject_C/
04_Wrong_Questions/
05_Templates/
06_Agents/
07_Memorization/
08_Subjective_Bank/
09_Reminders/
10_Config/
assets/
```

Rename folders to match the exam and language of the vault.

## Plugin Policy

Start with native Obsidian. Add plugins only when they solve a real problem:
- Dataview: useful for database-like summaries.
- Tasks: useful for task queries and dates.
- Kanban: useful for workflow boards.
- Style Settings: useful if the chosen theme supports it.
- Banners: avoid as a dependency for critical homepage layout; use Markdown images for stability.

## Layout Lessons

Use stable selectors:
- Prefer custom callouts like `[!todo]`, `[!summary]`, `[!week]`.
- Style by `data-callout` in CSS.
- Avoid relying only on `cssclasses` for important layout.
- For grids, use simple HTML wrappers when Markdown cannot make stable columns.
- Keep native checkboxes for todo lists.

Common issues:
- Reading view and editing view may render differently.
- Plugin themes can override layout.
- Banners plugins can inject duplicate or misplaced images.
- Wide grids may collapse unexpectedly if CSS targets the wrong wrapper.

## Core Templates

Use or adapt assets from `assets/obsidian/`:
- `homepage-template.md`
- `dashboard-css.css`
- `review-pool-template.md`
- `memorization-template.md`
- `subjective-bank-template.md`

After creating files, verify:
- Internal links open.
- CSS snippet is enabled.
- Todo checkboxes are clickable.
- Dashboard works in reading view.
- The homepage is not too crowded.
