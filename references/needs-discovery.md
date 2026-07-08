# Needs Discovery

The goal is to understand the user's exam situation before designing a system. Ask in batches and stop when enough information exists to build a usable first version.

## Minimum Viable Intake

Ask these first when the user wants to start quickly:

1. Exam name and remaining days.
2. Target result or target scores.
3. Subjects/modules and current progress.
4. Guaranteed daily/weekly study time.
5. Current biggest problem: forgetting, wrong questions, subjective answers, schedule drift, anxiety, or messy materials.
6. Tools already used: Obsidian, Anki, Feishu, WeChat, XMind, Notion, handwritten notes, photos.

## Full Question Bank

Exam and target:
- What exam are you preparing for?
- How many days remain?
- What is the target school, score, ranking, or pass line?
- Which subjects carry the most weight?
- Which subjects are allowed to maintain rather than improve?

Current foundation:
- For each subject, is it from zero, learned but not memorized, one round done, or stable?
- Which modules repeatedly lose points?
- What scores did recent mocks or previous attempts produce?
- Which materials must be fully covered, and which are only for lookup?

Time:
- What weekday time is guaranteed?
- What weekday time is possible but unstable?
- Is weekend time stable?
- Which days are usually low energy?
- What is the maximum daily planning load the user can tolerate?

Memorization:
- What must be memorized?
- Does the user prefer mind maps, outlines, recitation, cards, or writing?
- Should review follow Ebbinghaus intervals, fixed weekly review, or a simpler rhythm?
- Should Anki be used now, later, or avoided?

Practice and wrong questions:
- What question types exist?
- Are wrong questions typed, handwritten, photographed, or mixed?
- Should wrong questions be summarized by knowledge point, error cause, or source?
- Does the user need agent-style questioning to verify mastery?
- Should wrong questions feed memorization cards? Do not assume yes.

Subjective answers:
- Are subjective answers important?
- Does the user need scoring, rewritten answers, standard answer comparison, or answer-pattern extraction?
- Should a searchable subjective-answer bank be built?

Reminders and automation:
- Does the user want morning plans and evening reviews?
- Which channel is preferred: Feishu, WeChat, email, local notification, or manual check-in?
- Is the user comfortable configuring webhooks or automation scripts?

Visual and knowledge-base preferences:
- Does the user want a minimal system, visual dashboard, or detailed database?
- Which visual style lowers anxiety?
- What information must appear on the homepage?
- Which information should be hidden in archives?

## Signals That Requirements Are Not Clear Enough

Do not build yet if:
- The exam and remaining time are unknown.
- The user has not chosen between light and detailed tracking.
- The system depends on tools the user has not installed.
- The user wants automation but has not chosen a delivery channel.
- The user's input format is unclear and would make daily use too heavy.

In these cases, ask only the missing questions needed for the next step.
