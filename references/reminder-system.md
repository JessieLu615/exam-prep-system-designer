# Reminder System

Reminder systems should make the daily plan easier to start and the evening review easier to finish.

## Morning Plan

Send once in the morning:
- Available study time.
- Must-finish tasks.
- Optional stretch tasks.
- One review item.
- One short warning if schedule risk exists.

Example:

```text
Today: 4h available
Must finish:
1. 312: one chapter framework
2. 312: 20 matching questions
3. Politics: new module 1h
Review:
- Revisit yesterday's memorization list
Evening feedback:
- Actual time, completed tasks, biggest blocker
```

## Evening Review

Send once at night:
- Ask for actual study time.
- Ask which tasks were completed.
- Ask for new wrong questions or subjective-answer outputs.
- Ask for one blocker.
- Update tomorrow's plan based on the response.

## Channel Rules

Feishu and WeChat both require user-specific setup. Do not put secrets in public files.

Store private values in local config or environment variables:
- Webhook URL.
- Secret/signature.
- User ID or group ID.

For GitHub templates, include placeholders only.

## Automation Level

Level 1: Manual prompts in the chat.
Level 2: Local scheduled script.
Level 3: Feishu or WeChat push.
Level 4: Two-way feedback collection and automatic plan update.

Start with the lowest level that the user will actually maintain.
