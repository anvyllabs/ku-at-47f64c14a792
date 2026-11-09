# 01_CONTEXT.md · the why · BUSS215-06·07

---

## Part A · Blank template

```markdown
# CONTEXT — why this project exists

- Audience: Who is stuck?
- Problem: One real situation (not “we need an app”).
- Goal: What becomes easier if we succeed?
- Scope: What is inside this version?
- Out of scope: What we will not do (this time).
- Sources: Checked facts only; mark guesses NEEDS CHECK.
- Tooling: Antigravity + which files are source of truth?
```

### Writing tips (Lecture A · Context engineering; Lecture B Chapter 1)
1. A problem is about a person stuck somewhere — not a solution slogan.
2. Separate facts / assumptions / unknowns.
3. Context is the desk; the project folder is the bookshelf.

Source: `/workspace/ku_mdarch_CD/handoff/references/261027_source_text.txt` ~lines 142–157, 584 · Lecture B Chapter 1 (~01:31+).

---

## Part B · Filled AnvylTube example

# CONTEXT — AnvylTube pilot

- **Audience:** BUSS215-06·07 students in an English-taught MIS course who are starting a group project with Google Antigravity and need a concrete example of Core 5 in a small real build.
- **Problem:** Students hear about many AI videos but do not know which ones are repeatedly recommended by careful readers over years — and a raw Hacker News dump is unusable as a syllabus aid.
- **Goal:** Ship a **static, English, link-only** pilot page for ~2 weeks that surfaces ~80 AI-area videos from the public HackerTube dataset, with short cards students can scan in class.
- **Why HackerTube:** Public dataset by Andrej Karpathy (~43M HN comments, 2007–2026). A video is kept if recommended by ≥3 different people in ≥3 different months (~7,000 → **6,454** videos; **150** categories in **16** areas; **576** in the AI area). Score = `rec_months + 0.5 × strong-rec months`. License: **ODC-By 1.0**. Not affiliated with HackerTube or Karpathy.
- **Scope (this pilot):** Select AI subset → static HTML filters (topic / level / type) → 12 finished English cards → screenshots for lecture support → Core 5 folder as the student-facing method example.
- **Out of scope:** Login, server-side code, analytics, YouTube API enrichment (key not issued), HN user IDs, Korean UI (page is English only), deleting existing files.
- **Assumptions / NEEDS CHECK:** Students will open a shared link on laptop or projector; design tone should match Anvyl Labs homepage colors/fonts (copper `#CC785C`, dark background). Header is brand-first (ADR `header-brand-first.md`).
- **Human vs AI:** Humans chose scope, filters, and reviewed sample cards. Agents drafted page code, card text, selection scripts, and this MD set. Secrets never enter files.
