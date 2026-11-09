# 03_TASKS.md · what we do now · BUSS215-06·07

---

## Part A · Blank template

```markdown
# TASKS

## NOW
- [ ] T-01 — …
  - Owner: Member A (+agent) / Verifier: Member B (+agent)
  - Done means: (link to SPEC id)
  - Files: …

## NEXT
- [ ] T-02 — …

## BLOCKED
- [ ] … — reason · resume when …

## DONE
- [x] … — date · how verified
```

### Writing tips (Lecture A P4 · Lecture B weekly check-in)
1. One owner per task file set. Announce before editing a Core file.
2. Done means must point to SPEC / golden tasks — not “looks good”.
3. Attempted-but-unfinished work goes in WORKLOG with why; do not mark unattempted work as Failed.
4. Daily Start session: read `00_HOME` → `03_TASKS` → latest **1** entry of `04_WORKLOG`.

Source: `/workspace/ku_mdarch_CD/handoff/references/261027_source_text.txt` ~P4 lines 529–573 · Lecture B Chapter 4 weekly check-in.

---

## Part B · Filled AnvylTube example

# TASKS — AnvylTube pilot

## NOW
- [ ] **T-10** — Finish English UI pass on `index.html` (filters, badges, footer English; hide unfinished badges on share view)
  - Owner: Member A (+agent) · Verifier: Member B (+agent)
  - Done means: AT-03, AT-05 · files: `../index.html` (do not delete backups)
  - Note: another job owns large index edits; coordinate before overwrite

- [ ] **T-11** — Apply Anvyl Labs homepage design tone (colors/fonts/wordmark) without inventing a new brand system
  - Owner: Member A (+agent) · Verifier: Spec owner
  - Done means: visual match to homepage tokens listed in CONTEXT · capture new screenshots with `../shoot.py` after local server

- [ ] **T-12** — Human-review next batch of English cards beyond the 12 ready ones
  - Owner: Spec owner · Helper: Member C (+agent) drafts only
  - Done means: reviewed cards move to `card_state=ready` via `../cards_en.py` + `../build_cards.py`

## NEXT
- [ ] **T-13** — Issue YouTube Data API key (human only) then enrich durations — **blocked until key exists**
- [ ] **T-14** — Fill course-week mapping (currently `"Week mapping coming"`) once syllabus weeks are confirmed
- [ ] **T-15** — Run full golden-task set after UI freeze; record score in `evidence/`

## BLOCKED
- [ ] **T-13** — YouTube API key not issued · resume when Spec owner places key in `.env` only (never in chat/MD)
- [x] Header branding hierarchy · brand-first “AnvylTube by Anvyl Labs” · 2026-11-10 · ADR `header-brand-first.md`

## DONE
- [x] **T-01** — Research public HackerTube facts (counts, score, license) · 2026-11-09 · verified against dataset + public write-ups
- [x] **T-02** — `select.py` AI subset → `selection_raw.json` · 2026-11-09 · script print + file exists
- [x] **T-03** — Build first static page + Korean cards backup · 2026-11-09 · screenshots in `../captures/`
- [x] **T-04** — Decisions: as-is titles/channels, no HN user IDs, footer credit, drop length filter · 2026-11-09 · ADRs in `decisions/`
- [x] **T-05** — English cards for 12 videos + `build_cards.py` merge `general`→Beginner · 2026-11-10 · Counter + spot check
- [x] **T-06** — Instructor decisions: disclose Karpathy origin on both videos; merge General into Beginner; page English only · 2026-11-10 · ADRs
- [x] **T-07** — Seed this Core 5 example folder under `md/` · 2026-11-10 · files listed in HOME
