# 02_SPEC.md · what “done” means · includes one-page PRD · BUSS215-06·07

---

## Part A · Blank template (Lecture B · Template 2)

```markdown
ONE-PAGE PRD · Team ________ Date: ____
1. Problem Who is stuck, and where? (one real situation)
2. User Who exactly? (not “everyone”)
3. Main task What ONE thing must the user be able to do?
4. Success What number tells us it works? (4 of 5 users…)
5. Features (MoSCoW)
   Must: What is the smallest set for the main task?
   Should: Important, but the product still works without it?
   Could: Nice to have, only if time allows?
6. Out of scope What will we NOT build? (= Won’t, this time)
7. Risks and assumptions What are we guessing? What could stop us?
8. How we check Which golden tasks? Which user test?
```

### Writing tips
1. One page. If it does not fit, the scope is too big.
2. Success needs a number you can count in a test.
3. Out of scope tells agents what **not** to build.
4. Keep Must short enough to finish early; testing fills the rest.
5. Common mistake: writing a solution as the problem.

Source: `/workspace/lectureB/Templates.txt` p.5–6 · video 34:10–37:23 · `261029_templates_source_text.txt` lines 89–136.

---

## Part B · Filled AnvylTube PRD + acceptance checks

ONE-PAGE PRD · Team AnvylTube · Date: 2026-11-09

1. **Problem** A BUSS215 student who wants AI learning videos does not know which titles are repeatedly recommended over years, and cannot read 6,454 HackerTube rows in class.
2. **User** BUSS215-06·07 students (English-taught) and the instructor showing a worked example at group-project kickoff.
3. **Main task** Open the static page, filter by topic / level / type, and open one recommended video card with a short English “why” — without creating an account.
4. **Success** In a quiet classroom test: **4 of 5** classmates (codes T1–T5, no real names) can find a matching AI video for a stated topic within **2 minutes**.
5. **Features (MoSCoW)**
   - **Must:** static HTML page · filters for topic, level, type · 80 AI videos from selection script · at least 12 finished English cards · youtube-nocookie embed / thumbnail · footer with ODC-By credit + “Inspired by Andrej Karpathy’s HackerTube; not affiliated with either.” · 2-week pilot note
   - **Should:** Anvyl Labs homepage design tone (dark `#0A0A0C`, copper `#CC785C`, Plus Jakarta Sans / Outfit) · equal card sizes · hide unfinished-card badges on shared view · “How this was built” link to this `md/` folder
   - **Could:** full 80 English cards · course-week mapping per video · YouTube duration/views after API key exists
6. **Out of scope (Won’t, this time)** Length filter (no duration data) · HN user IDs · login / analytics / server · Korean page copy · public affiliation claim · deleting prior files → see `decisions/`
7. **Risks and assumptions** API key not issued (durations stay out). Selection keyword/category heuristics may miss or over-include titles (**NEEDS CHECK** by human sample review). Projector readability on dark UI.
8. **How we check** Five golden tasks in `evidence/golden_tasks.md` after every important UI change · five-line user test in `evidence/user_test.md`

### Acceptance table (done means)

| ID | Done means | How we check |
|---|---|---|
| AT-01 | `select.py` writes `selection_raw.json` from `videos.jsonl` | Run script; count printed; file exists |
| AT-02 | `build_cards.py` writes English `cards.json` / `cards.js`; `general`→Beginner | Inspect levels Counter; spot-check 3 vids |
| AT-03 | Page filters topic / level / type; no length filter | Manual click on local `index.html` |
| AT-04 | 12 cards have English `lines` + `why` | `card_state==ready` count = 12 |
| AT-05 | Footer states source credit + not affiliated | Visual check / screenshot |
| AT-06 | No API keys or extra personal names on student-facing screens | Grep + human read |
