# evidence/golden_tasks.md · BUSS215-06·07

---

## Part A · Blank template (Lecture B · Template 4)

```markdown
# Task | Input | Expected result | Pass? | Date
| 1 | Normal case? |  |  |  |  |
| 2 | Empty or wrong input? |  |  |  |  |
| 3 | Repeat or conflict? |  |  |  |  |
| 4 |  |  |  |  |  |
| 5 |  |  |  |  |  |
Score: ___ / 5 on ____ → save why each failure happened (one line).
```

### Writing tips
1. Write the expected result **before** you run the test.
2. Same set every time; the trend is your KPI.
3. One-line error analysis when something fails.
4. Do not silently change a test to improve the score.

Source: `/workspace/lectureB/Templates.txt` p.9–10 · `261029_templates_source_text.txt` lines 169–194.

---

## Part B · Filled AnvylTube example (pilot set)

| # | Task | Input | Expected result | Pass? | Date |
|---|---|---|---|---|---|
| 1 | Open page offline/local | Load `index.html` via local static server | Filters + cards render; no login wall | Yes | 2026-11-09 |
| 2 | Filter by topic | Choose “LLM basics & use” (or equivalent chip) | Only matching topic cards remain | Yes* | 2026-11-09 |
| 3 | Filter by level after merge | Choose Beginner | Former `general` rows appear under Beginner; no separate General chip | Yes | 2026-11-10 |
| 4 | Open a finished card | Open `wjZofJX0v4M` | English lines + why shown; embed/thumbnail path works | Yes | 2026-11-09 |
| 5 | Unfinished card behavior on share view | View a non-ready card in share configuration | No “pending review” badge noise on share view **or** card hidden — per SPEC Should | **NEEDS CHECK** | — |
| 6 | Footer honesty | Scroll to footer | ODC-By credit + not-affiliated / inspired-by line visible | Yes | 2026-11-09 |
| 7 | No secrets / extra names | Grep student-facing HTML+cards | No API keys; no personal names beyond KyungBae Park & Andrej Karpathy | Yes | 2026-11-10 |
| 8 | Length filter absent | Inspect filter bar | No duration/length filter control | Yes | 2026-11-09 |

\*Topic label strings moved KO→EN during English pass — re-run after UI freeze.

**Score:** 6 / 8 checked · 1 NEEDS CHECK · 1 to re-run after English UI freeze · 2026-11-10  
**Error analysis (one line):** Task 5 waits on share-view policy implementation in `index.html` (owned by parallel UI task).
