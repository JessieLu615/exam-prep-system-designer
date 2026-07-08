# Dashboard Design

The dashboard exists to reduce anxiety and tell the user what to do next.

## Information Architecture

Recommended order:
1. Today's todo list.
2. Total task completion ratio.
3. This week's status.
4. Module progress.
5. Current task table.
6. Recent reviews.
7. Common entrances.

Remove anything that does not support action, progress awareness, or review.

## Visual Principles

- Use generous spacing.
- Keep cards visually distinct but calm.
- Use a limited Morandi palette.
- Avoid decorative complexity before the workflow is stable.
- Use one dominant neutral background.
- Use color to separate meaning, not to decorate randomly.

Suggested color roles:
- Todo: blue gray.
- Total progress: muted purple.
- Weekly status: gray white.
- Current task table: gray rose.
- Recent review: blue gray.
- Common entrances: muted purple.
- Other accents: blue gray.

## Layout Principles

- Put high-frequency actions near the top.
- Keep todo easy to scan and check.
- Show the total ratio clearly, such as `completed / total`.
- Use cards for repeated or bounded information.
- Avoid nested cards.
- Make paired cards equal height when visually aligned.
- Leave visible gaps between grid cards.

## Obsidian CSS Strategy

Prefer custom callout selectors:

```css
.markdown-preview-view .callout[data-callout="todo"] { }
.markdown-preview-view .callout[data-callout="summary"] { }
```

For module cards, use explicit HTML classes:

```html
<div class="exam-module-grid">
  <div class="exam-module-card">...</div>
</div>
```

This is more predictable than trying to force Markdown lists into complex layouts.
