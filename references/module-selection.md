# Module Selection

Select modules by pain point. Do not add a module because it looks impressive.

## Module Matrix

| User Need | Module | Include When | Avoid When |
|---|---|---|---|
| Progress anxiety | Control dashboard | User needs to see daily and total progress | User only wants plain text plans |
| Forgetting | Memorization system | There is large recall content | Content is mainly skill practice |
| Mind-map learning | Mind-map to cards | User builds frameworks manually | User expects the agent to create all frameworks |
| Wrong questions | Wrong-question review | Mistakes repeat or need transfer checks | User only needs one-time explanation |
| Subjective answers | Subjective-answer bank | Answers need scoring and revision | Exam has no subjective component |
| English reading/writing | English module | Themes, vocabulary, corpus, writing templates matter | English only needs maintenance |
| Political theory | Politics module | Concepts/frameworks need explanation | User is already stable |
| Automation | Reminder module | User wants morning/evening pushes | User will not configure channels |
| Knowledge base | Obsidian/notes module | Outputs need long-term retrieval | User only wants daily prompts |

## Default Minimal System

When requirements are unclear but user wants to start today:
1. Daily plan.
2. Total progress count.
3. Memorization log.
4. Wrong-question pool.
5. Weekly review.

Add Anki, dashboards, Feishu/WeChat, OCR, or detailed databases only after the user confirms they will use them.

## Agent-Style Roles

If the user wants a subagent system, define roles by workflow, not by decoration:
- Main controller: plans, checks progress, adjusts.
- Memorization agent: turns user-made frameworks into cards/review tasks.
- Wrong-question agent: explains, classifies, and tests transfer.
- Subjective-answer agent: scores and revises answers.
- Subject specialist agent: explains weak modules.
- Knowledge-base agent: formats outputs for the chosen system.

Keep one chat as the entrance if the user wants low friction. Agents can be roles inside the conversation rather than separate technical processes.
