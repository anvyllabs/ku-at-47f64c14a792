# 04_WORKLOG.md · history + handoffs · BUSS215-06·07

---

## Part A · Blank template (Lecture B · Template 6)

```markdown
# WORKLOG
(add at the bottom; never rewrite others’ lines)

YYYY-MM-DD · role · agent used · one line: what was done

HANDOFF NOTE · four lines (when unfinished or passing work)
Did: What did I finish?
Checked: How did I check it? Which golden tasks?
Not confirmed: What am I not sure about? (NEEDS CHECK)
Next: What should you do first?

## Unfinished (End session)
- Item: …
- Why unfinished: …
- Resume when: …
```

### Writing tips
1. Append only. Never rewrite a teammate’s earlier lines.
2. Name the **role** and the **agent** (e.g. Member A (+agent)).
3. “Not confirmed” is the most useful handoff line — mark NEEDS CHECK.
4. End session: record unfinished items and why (Lecture A / classroom 30-min flow).
5. Check the diff before saving.

Source: `/workspace/lectureB/Templates.txt` p.13–14 · `261029_templates_source_text.txt` lines 231–264 · Lecture B Chapters 2–4.

---

## Part B · Filled AnvylTube example

# WORKLOG — AnvylTube

2026-11-09 · Spec owner · (+agent) · Confirmed public HackerTube dataset facts (~43M comments; ≥3 recommenders in ≥3 months; 6,454 videos; 576 AI-area; ODC-By 1.0) and wrote selection plan. Checked: counts against `/workspace/hackertube_research/` data folder listing + prior research note. Not confirmed: YouTube API quota for enrichment — NEEDS CHECK. Next: Builder runs `select.py`.

2026-11-09 · Member A (+agent) · Ran `select.py` → `selection_raw.json` (AI keyword/category filter; dropped news shelf_life; exclusion id set). Checked: script printed length + topic Counter. Not confirmed: whether every exclusion id is still required — NEEDS CHECK. Next: Builder drafts static page.

2026-11-09 · Member A (+agent) · Built first static `index.html` + card pipeline; captured screenshots via `shoot.py` (local server :8765). Checked: thumbnails loaded for first 12 cards in Playwright run. Not confirmed: classroom projector contrast — NEEDS CHECK. Next: Spec owner reviews sample cards.

2026-11-09 · Spec owner · (+agent) · Recorded product decisions (as-is titles/channels; no HN user IDs; footer credit; no length filter → type filter). Checked: decisions mirrored in page footer draft. Next: English card pass.

2026-11-10 · Member A (+agent) · Added `cards_en.py` + `build_cards.py`; merged data-level `general` into Beginner; rebuilt `cards.json`/`cards.js`. Checked: 12 `ready` cards; level Counter shows Beginner includes former general. Not confirmed: full human review of all 12 lines — sample_reviewed set is only 3 ids. Next: Verifier spot-checks.

2026-11-10 · Spec owner · Instructor confirmed: disclose Karpathy/HackerTube origin; English-only page; merge General into Beginner. Checked: ADRs written under `decisions/`. Next: UI English + design tone tasks (T-10, T-11).

2026-11-10 · Member A (+agent) · Created Core 5 example tree under `md/` (AGENTS + 00–04 + decisions/evidence/outputs/members) following Lecture B templates; did not edit `index.html` in this task. Checked: file list vs Lecture A folder map. Not confirmed: instructor header branding card still open — NEEDS CHECK. Next: Member B runs golden tasks after UI freeze.

### HANDOFF NOTE · Member A (+agent) → Member B (+agent)
Did: Seeded Core 5 + Lecture B companion files for AnvylTube; documented real scripts (`select.py`, `build_cards.py`, `cards_en.py`, `shoot.py`) without inventing API work.
Checked: Local paths exist; 12 English card ids listed in `cards_en.py`; ADRs dated 2026-11-09/10.
Not confirmed: Final shared `index.html` English/design pass (owned elsewhere); YouTube API enrichment; week mapping.
Next: Member B — after UI freeze, run `evidence/golden_tasks.md` and append the score here.

2026-11-10 · Spec owner · Instructor confirmed header: “AnvylTube by Anvyl Labs” on top, course line “BUSS215-06·07 · Prof. KyungBae Park” below. Story: Karpathy built HackerTube; Anvyl Labs tried the same approach; now it's your team's turn. No sales copy, no contact buttons, no student data. Checked: ADR `header-brand-first.md` written. Next: re-shoot captures after UI freeze.
