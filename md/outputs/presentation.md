# outputs/presentation.md · BUSS215-06·07

---

## Part A · Blank template (Lecture B · Template 7)

```markdown
GROUP PROJECT PRESENTATION · five parts
1. Problem Who is stuck, and where?
2. What we built Show ONE user doing the main task.
3. Evidence Golden-task score over time, and what users did.
4. Limits What does not work yet? One failure we learned from.
5. Next step What would we build with five more weeks?

BE READY FOR
Q1 How do you know it works? → evidence/
Q2 What did the AI do, and what did you do? → WORKLOG · decisions/
Q3 What would you do differently? → decisions/
```

### Writing tips
1. One task done well beats listing every feature.
2. Say a number, not “it works”.
3. Show one honest failure and what changed.
4. Explain the AI’s role honestly.

Source: `/workspace/lectureB/Templates.txt` p.15–16 · `261029_templates_source_text.txt` lines 265–315 · Lecture B Chapter 8–9.

---

## Part B · Filled AnvylTube example

PRESENTATION · AnvylTube (course example)

1. **Problem** A student who wants AI videos cannot tell which titles are repeatedly recommended across years.
2. **What we built** A static English filter page over 80 AI-area videos from public HackerTube data; open one card (e.g. transformers explainer) in under two minutes in our success test design.
3. **Evidence** Golden tasks 6/8 checked (2026-11-10); user-test script ready; classroom 4-of-5 timing test **not run yet** (TODO).
4. **Limits** No durations (API key not issued). 68/80 cards still in progress. Share-view badge policy NEEDS CHECK. We learned: do not advertise a length filter when the field is absent — ADR `no-length-filter.md`.
5. **Next step** Finish English cards; optional YouTube enrichment **if** key exists; only then revisit length filter (reopen line in that ADR).

### Be ready for
- **Q1** “We rerun the same golden tasks after UI changes; current sheet is in `evidence/golden_tasks.md`.”
- **Q2** “Agents drafted HTML/scripts/card text; humans set scope, wrote ADRs, and must approve share. See WORKLOG.”
- **Q3** “Write golden tasks before the first UI share; merge level labels earlier.”
