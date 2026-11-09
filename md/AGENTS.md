# AGENTS.md · BUSS215-06·07 · AnvylTube example

Course: BUSS215-06·07 · Korea University · Instructor: KyungBae Park, Ph.D.  
Tool: Google Antigravity · Method: Core 5 + AGENTS.md (Lecture B, 2026-10-29)

---

## Part A · Blank template (copy for your team)

```markdown
# AGENTS.md · Team ____ (example structure, not an official template)

## 1. Start of every session
- Read HOME → TASKS → newest WORKLOG entry
- Say in one sentence: What will you do today, and who asked?

## 2. While working
- Change only this task’s files. Which files?
- Show what will change before changing it
- Not sure it is true? Mark it NEEDS CHECK
- Never use real personal data
- Our own rule: What must never happen to our files?

## 3. End of every session
- Update TASKS
- Add one WORKLOG line: role · agent used · what was done
- Unfinished? Write a four-line handoff note

## Secrets
- Never write API keys, passwords, or tokens into any file except .env.
- Never open, print, copy, or summarize .env. Use placeholders like YOUR_API_KEY.
- If a key is needed, stop and tell me where to put it myself.

## 4. Never without a human (stop and wait for OK)
- Deleting, moving, or renaming files
- Running terminal commands that install, delete, or download anything
- Signing in, or typing any password or key
- Uploading, posting, deploying, or sending anything outside this folder
- Changing SPEC
- Approved by: Which named teammate (by role)?
```

### Writing tips (Lecture B · Template 1)
1. One page, really. Antigravity cuts off a very long rule file. Move details into Core 5 and point with `@file-name`.
2. Write instructions an agent can follow: “Read HOME first”, not “Be careful”.
3. Name a role, not “the team”: “the spec owner approves SPEC changes”.
4. Do not paste the whole PRD here — that belongs in SPEC / shelf three.
5. Add a rule when something goes wrong (near miss → new line).
6. AGENTS.md is guidance, not a lock. Keep Terminal command auto execution on **Request Review**.

Source: `/workspace/lectureB/Templates.txt` p.3–4 · `/workspace/ku_mdarch_CD/handoff/references/261029_templates_source_text.txt` lines 22–56 · Lecture B note Chapter 3 (~video 14:15).

---

## Part B · Filled AnvylTube example

# AGENTS.md · Team AnvylTube (course example for BUSS215-06·07)

Project: a 2-week static pilot page that helps students pick AI videos worth their time, using the public HackerTube dataset by Andrej Karpathy.

## 1. Start of every session
- Read `00_HOME.md` → `03_TASKS.md` → newest entry in `04_WORKLOG.md`
- State today’s task and who asked (course example Owner: Spec owner / Builder)

## 2. While working
- Change only files for today’s TASK id; show the diff before saving
- Never edit `02_SPEC.md` without Spec owner approval
- Mark unverified claims **NEEDS CHECK**
- Student-facing screens may show only: KyungBae Park (instructor) and Andrej Karpathy (data source credit). No other real personal names.
- Never write API keys, passwords, or tokens into any file
- Do not delete existing project files; keep dated backups instead

## 3. End of every session
- Update `03_TASKS.md`
- Append one WORKLOG line: role · agent used · what was done
- If unfinished, add a four-line handoff note

## Secrets
- Never write API keys, passwords, or tokens into any file except `.env`
- Never open, print, copy, or summarize `.env`. Use placeholders like `YOUR_API_KEY`
- YouTube Data API key is **not issued yet** for this pilot — do not invent one

## 4. Never without a human (stop and wait for OK)
- Deleting, moving, or renaming files
- Installing / downloading / deploying / sending outside this folder
- Changing SPEC or MoSCoW scope
- Sharing the pilot link (human review required before any share)
- Approved by: Spec owner (role)
