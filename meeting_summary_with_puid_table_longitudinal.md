Here is the updated PUID prompt. I have redesigned it to act as a longitudinal tracking tool. It now explicitly instructs the AI to analyze multiple transcripts, compare historical statuses to current ones, and track the lifecycle of issues and decisions across dates to create a true timeline of events.

***

**Copy and paste the following prompt:**

You are analyzing a series of weekly 1:1 meeting transcripts (historical and current) for a specific staff member and creating a structured, chronological PUID project timeline document. 

PUID stands for:
- Purpose: what we are doing and why
- Updates: current status and latest progress, tracked over time
- Issues: blockers that need fixing and their resolution lifecycle
- Decisions: what was agreed upon and why, mapped chronologically

Your job is to extract the information from the provided transcripts, compare the historical meeting notes to the current meeting notes, and format it as a clean, meeting-ready project timeline document.

## Instructions

### 1) Purpose
Capture the core goal of the project(s) from the transcripts.
Include only stable, high-level information.
Keep it short and focused on the project’s “north star.”

Recommended fields:
- Project Name
- Description
- Business Value
- Success Criteria

### 2) Updates (Timeline Log)
Capture the progression of the project by comparing previous meetings to the current meeting. 
Treat this as a running chronological log, creating a new row for each meeting date to show how the status or scope has evolved.
Focus on actionable progress, changes in momentum, and newly achieved milestones.

Recommended fields:
- Date
- Project
- Status Summary (Note any changes from the previous week, e.g., "Moved from In Progress to Blocked")
- Milestone Achieved
- Next Steps
- Owner

### 3) Issues (Blocker Lifecycle)
Capture blockers, risks, concerns, and unresolved problems mentioned across the transcripts.
Maintain this as a running blocker log, specifically tracking when an issue was first introduced and whether the current meeting shows it as resolved or escalating.

Recommended fields:
- ID
- Date Raised
- Issue Description
- Status (e.g., New, Ongoing, Escalated, Resolved)
- Date Resolved (Write "Ongoing" if still unresolved in the current meeting)
- Owner

### 4) Decisions (Chronological Log)
Capture decisions made during the meetings and the reasons behind them. 
Map these decisions by date to create a timeline of how project strategies have pivoted or solidified. Include enough context to prevent the team from reopening settled debates.

Recommended fields:
- Date
- Decision Made
- Rationale / Context
- Stakeholders Involved

## Rules
- Use only information supported by the transcripts.
- Do not invent facts or hallucinate progress.
- If a status or outcome from a previous week is unmentioned in the current week, do not assume it is resolved; mark it as "Unclear" or "No new updates."
- Preserve names, dates, owners, and decisions exactly as stated when possible.
- Use Markdown headings for each section.
- Use tables for each section.
- If a section has no relevant content, write “No new updates.”
- Output only the final PUID document.

***

### **Key Enhancements Made to Your Prompt:**
*   **Contextual Framing:** The AI is now explicitly told it is acting on a *series* of meetings (historical vs. current) rather than a single transcript. 
*   **Chronological Logging:** The **Updates** section now requires the AI to log progress by date and explicitly note *status changes* from the previous week.
*   **Issue Lifecycle Tracking:** The **Issues** section now includes "Date Raised" and "Date Resolved" columns to easily track how long blockers have been stalling a project. 
*   **Decision Timelines:** The **Decisions** section asks the AI to map decisions by date, creating a clear history of when and why strategies shifted over time.
