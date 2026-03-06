# LI-Analyzer

A job match analyzer that tells you whether a role is worth your time before you spend an hour on a cover letter. Paste in a job description, point it at your resume, and get a qualification-by-qualification breakdown with an honest fit score and concrete direction on what to address. *Step by step instructions included at the end, if you need them.*

---

## Files in This System

**system-prompt.md** — The startup file. Paste this into your AI tool's system prompt or project instructions. It handles preferences setup, resume selection, and runs the full analysis flow.

**preferences.md** — Your job search criteria. Remote only or open to hybrid? Minimum salary? Industries you won't touch? Fill this in once and the system checks every role against it before running the full analysis. Created automatically on first run via a short quiz, or fill it in manually before your first session.

**Resumes/** — Drop your resume PDF(s) here. If you have multiple versions — one for IC roles, one for leadership, one for design — add them all. The system reads the job description first and recommends which resume is the best fit before running the match.

**Analyses/** — One markdown file per role analyzed, named by company and role slug. Generated automatically after each analysis.

**Analyses/index.md** — A running log of every role with fit score, resume used, date, and application status. Generated automatically and updated as you go.

---

## How to Get Started

You only need two things before your first session:

1. **Resumes/** — Add at least one resume. PDF works best. If you have more than one version, add them all.
2. **system-prompt.md** — Load this using one of the integration options below.

After that:

3. On first launch, the system will run a short preferences quiz — six questions, one at a time. Answer them and it produces your `preferences.md`. Every session after that, it loads silently.
4. Paste a job description when prompted. The system checks it against your preferences, then runs the full resume match.
5. Update **Analyses/index.md** as your application status changes — Interested, Applied, Interviewing, Offer, Passed, or Declined.

---

## How the System Grows

Every analysis adds a file to your Analyses folder and a row to your index. Over time the index becomes a real picture of where you've been spending your energy and what's converting. Update your preferences any time your criteria shift; the system reads the file fresh at the start of each session, so changes take effect immediately.

---

## Detailed Instructions

### Just Getting Started

If you aren't ready to create a project or use a desktop tool, this is for you. Download the files (click on each and then "Download Raw File"). Copy and paste the contents of `system-prompt.md` into Claude or ChatGPT. Upload your resume and `preferences.md` as attachments, or skip `preferences.md` and let the quiz build it for you on first run.

### Use This as a Claude Project

A Claude Project lets you upload your files once and have them available in every session automatically. No re-uploading, no copy-pasting prompts.

1. Go to [claude.ai](https://claude.ai) and create a new Project
2. Open Project Settings and paste the contents of `system-prompt.md` into the Custom Instructions field
3. Upload your resume file(s) and `preferences.md` as Project files

Every conversation you start inside the Project will have your resume and preferences loaded automatically. Skip the Analyses folder — those files change with every session. Download individual analysis files from the chat and store them wherever works for you.

### Use This in a Cowork Session

Cowork is Claude's desktop tool for file and task management. This is the most seamless setup — Claude reads your files directly from your computer, so analyses save automatically and your index stays in sync without any manual steps.

1. Store all files in a folder on your computer
2. Start a Cowork session and point it to the folder
3. Paste the contents of `system-prompt.md` as your starting instruction

Claude will read your resume and preferences directly, run the analysis, save the output to your Analyses folder, and update the index — all without you touching a file.
