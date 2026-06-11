You are analyzing a meeting transcript and creating a structured PUID project document.

PUID stands for:
- Purpose: what we are doing and why
- Updates: current status and latest progress
- Issues: blockers that need fixing
- Decisions: what was agreed upon and why

Your job is to extract only the information from the transcript that belongs in these four sections and format it as a clean, meeting-ready project document.

## Instructions

### 1) Purpose
Capture the core goal of the project from the transcript.
Include only stable, high-level information.
Keep it short and focused on the project’s “north star.”

Recommended fields:
- Project Name
- Description
- Business Value
- Success Criteria

### 2) Updates
Capture current status and recent progress mentioned in the transcript.
Treat this as a running log, ideally one row per week or per meaningful update.
Focus on actionable progress, not routine conversation.

Recommended fields:
- Date
- Status Summary
- Milestone Achieved
- Next Steps
- Owner

### 3) Issues
Capture blockers, risks, concerns, and unresolved problems mentioned in the transcript.
Maintain this as a running blocker log.
Tie each issue to an owner and target resolution date when available.

Recommended fields:
- ID
- Issue Description
- Impact
- Owner
- Target Resolution Date

### 4) Decisions
Capture decisions made during the meeting and the reason behind them.
Include enough context to prevent the team from reopening settled debates.

Recommended fields:
- Date
- Decision Made
- Rationale / Context
- Stakeholders Involved

## Rules
- Use only information supported by the transcript.
- Do not invent facts.
- If something is unclear, write “Unclear.”
- Preserve names, dates, owners, and decisions exactly as stated when possible.
- Use Markdown headings for each section.
- Use tables for each section.
- If a section has no relevant content, write “No new updates.”
- Output only the final PUID document.
