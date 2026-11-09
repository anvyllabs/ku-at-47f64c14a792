# 00_HOME.md · the map · BUSS215-06·07

Course: BUSS215-06·07 · Instructor: KyungBae Park, Ph.D.  
Example project: **AnvylTube** (2-week pilot · English page)

---

## Part A · Blank template

```markdown
# [Project name] — HOME

Status (YYYY-MM-DD): [e.g., SPEC agreed; building MVP]
One-sentence goal:
Map: Context (01_CONTEXT.md) · Spec (02_SPEC.md) · Tasks (03_TASKS.md) · Worklog (04_WORKLOG.md)
Also: AGENTS.md · decisions/ · evidence/ · outputs/ · members/
Now: [the one task for today]
Blocked: [or “none”]
```

### Writing tips (Lecture A Day One · Lecture B Chapter 0)
1. HOME is the map, not the novel. Point to other files.
2. Status needs a date. “Almost done” is not a status.
3. At the end of the project, HOME tells the presentation story (Template 7 lives in `outputs/`; HOME links it).

Source: `/workspace/ku_mdarch_CD/handoff/references/261027_source_text.txt` ~lines 538–581 · Lecture B folder map (~video 01:31).

---

## Part B · Filled AnvylTube example

# AnvylTube — HOME

**Status (2026-11-10):** SPEC agreed · English MVP page in progress · 80 AI videos selected · 12 English cards finished · link-only 2-week pilot  
**Course:** BUSS215-06·07 · example for students starting a group project in Antigravity with Core 5  
**One-sentence goal:** Help a student answer “Which AI videos are worth my time?” from HackerTube’s public recommendations — without login, server code, or analytics.

### Map
| File / folder | Job |
|---|---|
| [AGENTS.md](AGENTS.md) | Rules every agent reads first |
| [01_CONTEXT.md](01_CONTEXT.md) | Why this pilot exists |
| [02_SPEC.md](02_SPEC.md) | One-page PRD + done means |
| [03_TASKS.md](03_TASKS.md) | What we do now |
| [04_WORKLOG.md](04_WORKLOG.md) | History + handoffs |
| [decisions/](decisions/) | Five-line decision records |
| [evidence/](evidence/) | Golden tasks + user-test script |
| [outputs/](outputs/) | Presentation outline |
| [members/](members/README.md) | Roles (no personal student names) |

### Code & data (parent folder, not invented)
- Page: `../index.html` · cards: `../cards.json` / `../cards.js`
- Select AI subset: `../select.py` · build cards: `../build_cards.py` · English lines: `../cards_en.py` · screenshots: `../shoot.py`
- Source dataset: `/workspace/hackertube_research/data/hackertube-data/` (public HackerTube / ODC-By 1.0)

### Now
- Apply English-only UI + Beginner merge + homepage design tone (see TASKS)
- Finish human review of remaining cards (68 still in progress)

### Blocked / NEEDS CHECK
- YouTube Data API key **not issued** → durations / views / publish dates stay out of the page
- Course week mapping for each video: still “Week mapping coming”
- (Resolved 2026-11-10) Header is brand-first: “AnvylTube by Anvyl Labs”, course line below — see `decisions/header-brand-first.md`
