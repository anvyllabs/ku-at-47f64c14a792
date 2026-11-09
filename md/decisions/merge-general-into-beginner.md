# decisions/merge-general-into-beginner.md · BUSS215-06·07

---

## Part A · Blank template (Lecture B · Template 3)

```markdown
decisions/________.md (one file per decision)
Decision: What did we choose?
Options considered: What else was on the table?
Why this one: What tipped it?
Given up: What did we say no to?
Would reconsider if: What new fact would reopen this?
```

### Writing tips
1. Five lines, no more. Write it on the day you decide.
2. The last line turns a decision into a test.
3. Every MoSCoW “won’t” gets a file.
4. Common mistake: “Why: it is better.” Better for whom?

Source: `/workspace/lectureB/Templates.txt` p.7–8 · `261029_templates_source_text.txt` lines 137–168 · Lecture B Chapter 4.

---

## Part B · Filled AnvylTube example

```markdown
decisions/merge-general-into-beginner.md
Decision: Merge data-level “general” into Beginner / intro.
Options considered: Keep four levels · rename general to “General education” · merge into Beginner
Why this one: Instructor decision 2026-11-10; 33/80 pilot rows were general — fewer empty filter buckets for class use.
Given up: A separate “general” chip on the page.
Would reconsider if: Students cannot find survey-style videos under Beginner in classroom tests.
```
**Date:** 2026-11-10 · **Status:** Accepted · Implemented in `../build_cards.py` LEVEL_MAP
