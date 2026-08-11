---
name: design-document-writer
description: Create and audit evidence-based product design process documents in Farsi for Product Designers, Product Managers, and future design agents. Use when the user provides a product problem, PRD, research, analytics, design exploration, Figma links, screenshots, or a design decision and wants a structured Markdown design document, including when the decision is to iterate, defer, or make no change.
---

# Design document writer

Create a clear, evidence-based Farsi design process document for product design work. The document must show how the team moved from problem and evidence to analysis, design exploration, decision, delivery, and follow-up.

The audience is primarily Product Designers and Product Managers. Use Farsi as the main language and retain familiar English product terms where they improve precision, such as UX, User Flow, Metric, Figma, Component, MVP, API, and Post-Launch.

## Non-negotiable rules

- Inspect the supplied material before drafting.
- Do not invent facts, metrics, sources, user behavior, decisions, links, or design details.
- Keep every source link, research link, analysis link, Figma link, prototype link, and screenshot reference in the relevant section.
- Separate evidence, interpretation, assumption, decision, and open question.
- Keep Problem free of solution language. Move intended changes to Goals or Design Solution.
- Treat optional output sections as conditional, but check every applicable section before deciding to omit it.
- Ask about missing or ambiguous material before writing the Draft.
- If the author does not have requested information, record the absence explicitly as `Not provided`, `Not available`, `Not applicable`, or `Needs validation`.
- Never turn missing Evidence into a confident claim.
- Preserve the author's product meaning, terminology, numbers, and links while improving structure and writing quality.
- A valid outcome may be `Proceed`, `Iterate`, `Defer`, or `No change`. Do not force a new design.
- Write the final document in Markdown. Use tables or diagrams only when they improve usability.

## Workflow

Follow this sequence. Do not silently skip a relevant stage.

### 1. Intake

Read the author's problem description, process notes, PRD, research, analytics, design files, screenshots, and linked documents. Build an internal inventory of:

- claims and their evidence;
- source links and artifact links;
- research methods and participants;
- design options and iterations;
- constraints and dependencies;
- decisions already made;
- missing information.

Do not browse repositories or external files unless the user explicitly asks you to. When the author provides a Figma link and asks for Figma review, inspect it directly if the Figma tools and permissions are available. Use only accessible content and report any access limitation.

### Figma benchmark review

When a Figma link is provided for competitor or benchmark work and the author asks for review:

1. Parse the Figma URL. If a node-specific URL is required by the available tool and the link has no `node-id`, inspect the file or page overview first; ask for a node-specific link only when the tool requires it.
2. Open the relevant Figma file, page, section, or frame with the available read-only Figma context tool.
3. Review visible screens, labels, flows, annotations, design notes, comments, and comparison tables when the connected tool exposes them.
4. Record what was actually reviewed, including file, page, section, and frame names and the original Figma link.
5. Separate direct Figma observations from the author's interpretation.
6. Summarize what was discovered and explain which Design decision, requirement, or Open Question each finding affected.
7. Do not assume that an inaccessible note, hidden comment, or unavailable page does not exist. Mark it `Not accessible` or `Needs validation`.

Use the benchmark table in [references/document-template.md](references/document-template.md) when comparing multiple competitors or products. Never fabricate competitor names, features, screenshots, notes, or conclusions.

### 2. Completeness audit

Check the supplied material against the required document structure in [references/document-template.md](references/document-template.md) and the question set in [references/question-checklist.md](references/question-checklist.md).

Ask focused questions for every relevant gap. Group questions by section and avoid asking for information that is already present. Ask before drafting, not after silently filling gaps.

If the author says the information does not exist, record the appropriate status and continue. Do not repeatedly ask for unavailable information.

### 3. Draft the evidence map

Before writing analysis, distinguish:

- **Evidence**: observed data, research output, interview finding, benchmark, support signal, or directly supplied artifact.
- **Interpretation**: what the evidence may mean.
- **Assumption**: an unverified belief used in the work.
- **Decision**: a chosen direction and its rationale.
- **Open question**: an unresolved uncertainty that may affect scope, design, or outcome.

For metrics, preserve the available definition and source. When a metric exists, capture `Metric`, `Baseline`, `Target`, `Timeframe`, `Data Source`, and `Owner`. If a field is unavailable, mark it rather than estimating it.

### 4. Write the document

Use the canonical structure in [references/document-template.md](references/document-template.md). Keep sections that are relevant and have content. For each omitted optional section, do not invent content; if the omission matters, state why it is not included.

Use the supplied links in place. Do not replace a Figma link with a description such as "design link". Add the link beside the relevant option, iteration, screen, component, or decision.

### 5. Review design reasoning

Make the chain explicit:

`Evidence → Insight → Design question → Options → Trade-offs → Decision → Constraint → Expected outcome`

For each option supplied by the author, include its pros, cons, rejection or selection reason, and source link when available. Include iterations when they change the reasoning or final design.

### 6. Validate and deliver

Run the quality checklist in [references/validation-checklist.md](references/validation-checklist.md). Check that:

- Problem contains no solution proposal;
- strong claims have Evidence or a visible validation status;
- links are preserved;
- metrics are not fabricated;
- Goals and Non-Goals define the boundary;
- the final decision can be `No change` or `Defer`;
- Open Questions are distinct from Future Work;
- Post-Launch checks are concrete;
- the writing is clear, natural, concise, and product-oriented.

Return the Markdown document after the review. If critical information remains unresolved, keep the document in Draft status and clearly identify what needs validation.

## Writing style

Apply [references/writing-style.md](references/writing-style.md). Use natural, direct Farsi with familiar English product terms. Prefer specific verbs and concrete explanations. Avoid promotional language, inflated significance, unsupported attribution, filler, repetitive structure, artificial synonym changes, and fabricated certainty.

Use UX-writing principles when documenting UI copy, errors, empty states, confirmations, onboarding, and interaction details. Keep those details short, actionable, accessible, and consistent with the product context.

Before delivery, run the humanize pass in [references/humanizing-checklist.md](references/humanizing-checklist.md). This is a quality pass for natural Farsi writing, not a promise to bypass AI detectors. Do not add mistakes, fake informality, or unsupported personality. Preserve all product meaning, Evidence, numbers, terminology, source links, and decisions.

## Multiple problem streams

When one initiative contains several connected problems, keep one initiative-level Context and create separate Problem Streams for materially different issues. For example:

```text
Initiative
├── Problem stream: order segregation
├── Problem stream: homepage layout
└── Problem stream: tabs and tables
```

Do not merge unrelated problems into one vague Problem statement. Connect each stream to its own Evidence, options, decision, and follow-up.

## Decision outcomes

Support all of these endings:

- **Proceed**: implement or develop the selected direction.
- **Iterate**: gather more Evidence or test additional design directions.
- **Defer**: keep the issue visible for a later phase or trigger.
- **No change**: preserve the current behavior because the impact, Evidence, or risk profile does not justify change.

For `Defer` or `No change`, document the Evidence, risks of changing, what remains unknown, and the condition that should trigger reconsideration.
