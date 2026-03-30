# PMM Research Phase 1 (pmm-research-p1)

A reusable Product Marketing (PMM) framework for running structured market, company, and competitor analysis.

This is designed to produce **decision-ready insights**, not just summaries — including category tension, positioning clarity, and whitespace opportunities.

---

## What this does

This skill runs a full Phase 1 PMM analysis:

* Market dynamics and shifts
* Customer pains and trigger moments
* Company positioning and strategy
* Competitor comparison (not isolated analysis)
* Category trade-offs (tension)
* Positioning summary (where the company wins and loses)
* Market gaps (true whitespace, not competitor weaknesses)
* Strategic opportunities mapped to those gaps

The output is structured to feed directly into:

* ICP definition (Phase 2)
* Messaging and positioning (Phase 3)

---

## How to use (Codex)

### 1. Open the repo in Codex or VS Code

### 2. Start a new thread

### 3. Run the skill:

Use the pmm-research-p1 skill.

company_name: [Company Name]
website: [Company URL]
competitors: [Competitor 1, Competitor 2, Competitor 3]

---

### Example

Use the pmm-research-p1 skill.

company_name: Endowus
website: https://endowus.com
competitors: StashAway, Syfe, MoneyOwl

---

## Required Inputs

* company_name
* website
* competitors (minimum 2–3 recommended)

If inputs are incomplete, the skill should request them before proceeding.

---

## Output Structure

The skill returns structured text in this order:

1. Market Overview
2. Challenges
3. Opportunities
4. Trends
5. Client Company
6. Vision
7. Goals
8. USP
9. Positioning
10. Client Dominant Narrative
11. Competitors
12. Key Trade-off (Category Tension)
13. Positioning Summary
14. Gaps
15. Non-Ideal Customer
16. Strategic Opportunities
17. Decision Mapping
18. Sources Used

---

## What makes this different

Most “analysis prompts”:

* describe the market
* summarise competitors
* stay neutral

This framework:

* forces trade-offs (no vague positioning)
* defines where the company wins and loses
* identifies real whitespace (not competitor gaps)
* maps insights to actual decisions

---

## When to use this

Use this when you need to:

* Understand a new market quickly
* Analyse a company and its competitors
* Prepare a positioning or messaging strategy
* Identify gaps in a crowded category
* Build a foundation for PMM work

---

## Notes

* Outputs are meant to be **internal working documents**, not polished decks
* You are expected to refine key sections (especially positioning and tension)
* Quality depends on input clarity and competitor selection

---

## Folder Structure

skills/
pmm-research-p1/
SKILL.md

---

## Next Steps

This is Phase 1.

Planned extensions:

* Phase 2: ICP, pains, desired outcomes, alternatives
* Phase 3: Positioning, messaging, and narrative

---

## License

Use freely for learning and internal work.