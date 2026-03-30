---
name: pmm-research-p1
description: Run Phase 1 PMM Market and Brand Discovery using a company-agnostic framework with separated market/company research, comparative competitor analysis, and strategic synthesis. Use when given company name, website, and dynamic competitor inputs, and return structured text output with evidence-led insights including category tension, positioning summary, and competitor dominant narrative.
---

You are executing a structured PMM research framework.

This is not a free-form analysis task.

You must follow the defined sections exactly.

# PMM Research Phase 1

## Framework Intent
Use this as a reusable PMM Market and Brand Discovery Framework (Phase 1).
Apply it across industries, business models, and maturity stages.
Produce a detailed internal working board that can directly feed Phase 2 (persona, pains, desired outcomes, alternatives) and Phase 3 (positioning).

## Required Inputs
Collect these inputs before analysis:
- `company_name` (string)
- `website` (string URL)
- `competitors` (array of competitor names; dynamic length)

If any required input is missing, request it before proceeding.

## Output Contract (Text Only)
Return structured plain text only.
Do not output JSON, code fences, or metadata.
Use this output order:


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

For competitors, use one subsection per competitor in the input order with:
- Name
- Target Audience
- Value Prop
- Messaging
- Positioning
- Dominant Narrative

## Output Depth Requirements
- Do not overly condense outputs.
- Write with enough detail to support downstream ICP, segmentation, messaging, and positioning work.
- `Challenges`, `Opportunities`, `Trends`, `Gaps`, and `Strategic Opportunities` must each contain 3-6 items.
- Each item may be 1-3 sentences where needed for strategic clarity.
- Avoid generic phrasing; include concrete user behaviors, segments, trigger moments, and implications.
- All insights must be specific and actionable
- Avoid vague phrases such as "improve", "enhance", "build stronger"
- Each point must clearly indicate:
  - who (persona or segment)
  - what (problem or use case)
  - why it matters

## Framework Alignment Thinking
Ensure each section is immediately reusable for later phases:
- `Challenges` should imply persona pains and frictions.
- `Opportunities` should imply desired outcomes and value priorities.
- `Competitors` should imply customer alternatives and switching logic.
- `Gaps` should imply positioning whitespace in the category.
- `Positioning`, `Positioning Summary`, and `Category Tension` should provide raw material for a final positioning statement.

## Workflow
Execute the workflow in order.
Use verifiable evidence from official pages, product and pricing pages, documentation, investor materials, and credible market sources.
If evidence is weak, mark it as a careful inference instead of stating certainty.

### Step 1: Market and Company Audit
Run two distinct tracks and keep them separate in reasoning.

#### 1A) Marketing Research
Populate:
- Market Overview
- Challenges
- Opportunities
- Trends
- Explicitly state what this means for how companies must compete differently


Method:
1. Identify the single most important market dynamic and state its practical implication in Market Overview.
2. Identify key trigger moments that force evaluation or switching behavior.
3. Map pain patterns by segment and buying context.
4. Reframe source claims into strategic implications, not copy.

Field requirements:
- Market Overview must highlight one dominant market dynamic and the implication for strategy.
- Challenges must surface real pains and constraints, not broad category cliches.
- Opportunities must point toward outcomes customers want but cannot reliably get today.
- Trends must be decision-relevant and connected to changing buyer behavior.

#### 1B) Company Research
Populate:
- Vision
- Goals
- USP
- Positioning
- Define one dominant narrative for the client (3–5 words)
- This should represent how the company wants to be perceived in the category

Method:
1. Extract explicit strategic intent and implicit strategic direction.
2. Translate product and feature claims into value mechanisms tied to user jobs.
3. Clarify where the company chooses focus and what it deprioritizes.
4. Express Positioning as one strong comparative statement.

Field requirements:
- Positioning must clearly differentiate the company versus alternatives in one sentence.
- USP should emphasize concrete differentiators with user and business implications.
- Use inference carefully when evidence is partial.

### Step 2: Comparative Competitor Analysis
Do not analyze competitors in isolation.
Always compare competitors against the focal company and each other.

Populate competitor sections with:
- Name
- Target Audience
- Value Prop
- Messaging
- Positioning
- Dominant Narrative

Internal structure requirements for each competitor:
- Target Audience: include specific segment, behavior pattern, and underlying intent.
- Value Prop: state the core problem solved and why this approach is preferred over alternatives.
- Messaging: describe tone, narrative angle, and what is consistently emphasized.
- Positioning: explain how the competitor wins versus alternatives.
- Dominant Narrative: summarize the category claim in 3-5 words.

Comparison rules:
- Explicitly show how each competitor differs from others.
- Keep narrative territories distinct and non-overlapping.
- Tie messaging to audience and positioning logic.

### Step 3: PMM Synthesis (Tension, Positioning, Gaps, Strategic Moves)
Use direct comparisons from Step 2 to generate synthesis.

Populate:
- Category Tension
- Positioning Summary
- Gaps
- Strategic Opportunities
- Non-Ideal Customer

Synthesis requirements:
- Category Tension must capture a real strategic trade-off in the market.
- Positioning Summary must:
  - clearly state when the company wins
  - specify what it is better at than alternatives
  - clarify what it intentionally does NOT optimise for
  - compare all major competitors and locate the focal company clearly
- Focus on strategic insight, not descriptive recap.

Gap logic (mandatory):
- Define Gaps as whitespace in the market, not weaknesses of a specific competitor.
- Derive Gaps from cross-competitor patterns, overlaps, and ignored demand signals.
- Do not mention competitor names in Gaps.
- Each gap should answer: "What positioning or narrative is currently not clearly owned?"
- Focus on unmet needs, ignored segments, behavioral gaps, or unclear narratives.
- Gaps must be tied to real customer needs, behaviours, or decision moments
- Avoid abstract or generic whitespace statements
- Each gap should be usable as a potential positioning angle

Strategic opportunity logic (mandatory):
- Map each Strategic Opportunity directly to one or more identified Gaps.
- Frame each item as a strategic move, not a generic recommendation.
- Include implied trade-offs where relevant (what is gained and what is sacrificed).
- Keep moves actionable for Phase 2 messaging development and Phase 3 positioning definition.

Non-ideal customer logic (mandatory):
- Define who the product is NOT built for
- Identify segments that would struggle with the product’s approach
- Base this on trade-offs in positioning and product design
- Avoid generic exclusions; be specific about behaviours, needs, or constraints
- This should reinforce positioning clarity, not dilute it

## Validation Checklist
Before final output, verify:
- Output is plain text only and follows the required section order.
- Competitor list is dynamic and reflects input length.
- Challenges, Opportunities, Trends, Gaps, and Strategic Opportunities each have 3-6 items.
- Market/company audit is separated from competitor analysis and synthesis.
- Each competitor includes one clear Dominant Narrative in 3-5 words.
- Market Overview contains one dominant market dynamic and implication.
- Positioning is one strong differentiating statement versus alternatives.
- Positioning Summary compares all competitors and clearly locates the company.
- Category Tension reflects a real market trade-off.
- Gaps are whitespace statements, pattern-derived, and contain no competitor names.
- Strategic Opportunities map to Gaps and include strategic trade-offs where relevant.

## Quality Rules

- Optimise for strategic usefulness, not brevity
- Avoid generic language (e.g. "innovative", "seamless", "end-to-end")
- Prefer specific segments, behaviours, and trigger moments
- Each bullet should contain a clear insight, not vague description
- Outputs should be usable to directly build ICP, messaging, and positioning
- Do not simplify to presentation-level summaries
- Maintain clarity but preserve nuance where it affects strategy
- Every insight should be usable to inform a landing page, ICP definition, or messaging angle
- If a point cannot be turned into a clear messaging angle, it is too vague
- If an insight could apply to any SaaS company, it is too generic and must be refined

## Decision Rules

- Do not remain purely descriptive. Every section must lead to a decision, trade-off, or implication.
- Make trade-offs explicit. Avoid neutral phrasing like "this depends" without clarifying what drives the decision.
- Clearly state where the client wins and where it loses relative to competitors.
- Avoid generic category language. Anchor insights in specific operational or buyer-level realities.
- Prefer sharp, opinionated synthesis over safe summaries.

### Writing Style Rules

- Use simple, clear language
- Avoid unnecessary jargon
- Use technical terms only when they improve clarity
- Prefer concrete phrasing over abstract phrasing
- Each bullet should be immediately understandable on first read
- Write like explaining to a smart operator, not a consultant

Bad:
"The strategic implication is that feature breadth is no longer enough"

Good:
"Having more features is no longer enough to win"

Bad:
"Behavioural segmentation creates positioning pressure"

Good:
"Users split into two groups, making it harder to position clearly"

## Output Formatting Rules

- Use Markdown formatting that renders cleanly across platforms (Notion, docs, markdown viewers)

### Source Requirements

Use different source types depending on the section being generated.

#### Market Research (Market Overview, Challenges, Opportunities, Trends)

- Prioritise independent, third-party sources that describe the market as a whole
- Examples of acceptable sources:
  - Industry analysis and reports
  - Aggregated data platforms
  - Reputable publications and media
  - Regulatory or institutional sources (when relevant)
  - Expert or operator perspectives (if credible)

- Do NOT rely primarily on company or competitor websites for market-level insights
- Use company sources only to support or illustrate a trend, not define it

#### Company Research (Vision, Goals, USP, Positioning)

- Use official company sources:
  - Website (about, product, pricing)
  - Documentation or product materials
  - Public statements or materials

#### Competitor Analysis

- Use competitor websites as primary sources
- Supplement with third-party perspectives if needed

## Positioning

- Frame positioning as a decision, not a description.
- Define the competitive context (what alternatives exist).
- Clearly state why the client is chosen over those alternatives.
- Avoid vendor language. Use buyer decision language.

## Category Tension

- Identify the core trade-off that forces a real decision in this market.
- Frame it as a mutually exclusive choice (buyers cannot fully optimise both sides at once).
- Avoid generic trade-offs (e.g. "speed vs flexibility") unless grounded in specific operational context.
- Express the tension in buyer-relevant terms (e.g. operator vs management, short-term vs long-term, control vs adaptability).

## Client Dominant Narrative

Provide ONE dominant narrative for the client (3–5 words).

This must represent how the company wants to be perceived in the category.

Output format:
- Dominant Narrative: <3–5 word phrase>
- Explanation: <2–3 lines explaining why>

## Decision Mapping

Explicitly map where the client wins, loses, and best fits.

Output format:

### Wins When:
  <bullet points>
### Loses When:
  <bullet points>
### Best Fit Customer:
  <bullet points>

### Where the Client Wins
- Identify 3–5 scenarios where the client is the clear best choice.
- Anchor in real triggers (e.g. urgency, constraints, org structure).

### Where the Client Loses
- Identify 3–5 scenarios where competitors are better suited.
- Be explicit. Do not soften or generalise.

### Best-Fit Customer
- Describe the type of buyer who will see the most value.
- Include context: size, maturity, urgency, internal capabilities.

### Non-Ideal Customer
- Identify who should NOT choose this solution.
- Focus on structural mismatch, not just preferences.

## Confidence Level

Confidence Level should be applied for:
- Market Overview
- Challenges
- Opportunities
- Trends

- For key insights, indicate:
  - High confidence (clear evidence)
  - Medium (inference)
  - Low (directional)

#### General Rules

- Balance multiple perspectives when forming market-level conclusions
- Do not derive market trends purely from competitor messaging
- If external validation is limited, clearly state it as a directional inference
- The main market dynamic must reflect a real shift in user behaviour, not just product changes

### Section Structure

- Use a single H1 (#) for the company name at the very top

- Use H2 (##) for all main sections:
  - Market Overview
  - Challenges
  - Opportunities
  - Trends
  - Client Company
  - Vision
  - Goals
  - USP
  - Positioning
  - Competitors
  - Key Trade-off
  - Positioning Summary
  - Gaps
  - Strategic Opportunities
  - Sources Used

- Do NOT write section titles as plain text (e.g. "Market Overview:")
- ALWAYS use proper Markdown headers

### Competitor Formatting

- Each competitor must use H3 (###) with the competitor name

Example:
### Endowus

- Target Audience:
- Value Prop:
- Messaging:
- Positioning:
- Dominant Narrative:

### Content Formatting

- Use bullet points for all sections except:
  - Vision
  - Goals
  - USP
  - Positioning
  - Positioning Summary
  (these can be short paragraphs or bullets if needed)

- Keep bullets concise (1–2 lines preferred)
- Add one empty line after each header
- Do not add unnecessary spacing between bullets

### General Rules

- No emojis
- No bold-heavy formatting
- Keep structure clean and scannable

## Final Check

Before completing the output:

- Ensure ALL sections are present
- Ensure no section is missing
- Ensure headings match exactly

Do not return output if any section is missing.