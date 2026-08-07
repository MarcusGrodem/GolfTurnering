# Claude Web Setup for Hjemmebane

This folder prepares the repository for a Claude Project. The files in this folder do not replace the main project documentation; they tell Claude how to use it.

## Create the Project

1. Create a new Claude Project named **Hjemmebane**.
2. Paste the contents of `PROJECT_INSTRUCTIONS.md` into **Set project instructions**.
3. Upload the files listed below to **Project knowledge**, keeping their filenames unchanged.
4. Start the first chat with the prompt in `FIRST_MESSAGE.md`.

The project name and description in Claude's interface are for organization only. Put information Claude must always follow in the project instructions or uploaded knowledge files.

## Upload First

Upload these files for normal concept, planning, design, and website work:

1. `claude/START_HERE.md`
2. `CONTEXT.md`
3. `website/WEBSITE_CONTEXT.md`
4. `website/BRAND_IDENTITY.md`
5. `website/COLOR_PALETTES.md`
6. `budget/sola-gk-budget.md`
7. `budget/README.md`

## Upload When Relevant

- `budget/sola-gk-budget.xlsx` when asking Claude to inspect or revise the detailed Sola GK workbook.
- `budget/event-budget-template.xlsx` when working on reusable budget models.
- `budget/sola-gk-budget.csv` when tabular analysis is more important than workbook formatting.
- `tournament-names.md` only as historical naming material. **Hjemmebane is already the selected name.**
- Files from `website/brand/` when discussing or reviewing the actual SVG logo assets.
- Website source code once implementation begins.

Do not upload generated files that duplicate the same information unless the task requires their format. Duplicate knowledge increases the chance that old and new values are confused.

## Keeping Claude Current

Claude does not automatically know about later local edits. After changing a source document:

1. Replace the corresponding file in Project knowledge.
2. Update the date and change summary in `START_HERE.md` when the change is important.
3. Begin major new chats by naming the files Claude should consult.

Use separate chats for distinct workstreams such as website architecture, sponsorship packages, event operations, and visual design. Decisions made only inside one chat should be written back into the repository and re-uploaded, because chat context is not automatically shared across other chats.

## Recommended Prompt Pattern

For substantial requests, use:

```text
Read START_HERE.md first, then consult the source files it identifies for this task.

Task: [describe the task]

Before producing the result:
1. Separate confirmed decisions from assumptions.
2. Identify any conflict between source files.
3. Ask only questions that genuinely block the task.
4. Preserve the first-year scope and privacy rules.
5. End with the exact decisions or source files that should be updated.
```

