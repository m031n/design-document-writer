# Design document writer

[![skills.sh](https://skills.sh/b/m031n/design-document-writer)](https://skills.sh/m031n/design-document-writer)

Create evidence-based product design process documents in Farsi for Product Designers, Product Managers, and future design agents.

The skill turns a problem, research notes, analytics, benchmark work, design exploration, Figma links, and delivery decisions into a structured Markdown document. It asks about missing information before drafting and supports `Proceed`, `Iterate`, `Defer`, and `No change` outcomes.

## What it covers

- Problem and context, with a clear separation between evidence and solution
- Goals, Non-Goals, Success Metrics, and Guardrails
- Research methods, user insights, analytics, and benchmarks
- Competitor and Figma benchmark review, including accessible Notes and Annotations
- UX flows, screens, interactions, empty and error states
- Design options, Pros and Cons, iterations, and decision rationale
- Component anatomy, variants, rules, and reuse guidance
- Open Questions, Future Work, and Post-Launch checks
- Natural, human-readable Farsi with consistent product terminology

> [!IMPORTANT]
> The skill does not invent evidence, metrics, links, user behavior, or design decisions. If information is missing, it asks first. When the author confirms that information is unavailable, the document records `Not provided`, `Not available`, `Not applicable`, or `Needs validation`.

## Install with skills.sh

The recommended installer is the `skills` CLI, which runs through `npx` and requires no global CLI setup.

### Global installation

Use `-g` to make the skill available across your projects and supported agents:

```bash
npx skills add https://github.com/m031n/design-document-writer --skill design-document-writer --global --yes
```

### Project installation

Install it in the current project by omitting `--global`:

```bash
npx skills add https://github.com/m031n/design-document-writer --skill design-document-writer --yes
```

The repository exposes one skill, `design-document-writer`, so the `--skill` option makes the intended package explicit. To install all skills from a multi-skill repository, use `--all` instead.

### Verify the installation

List globally installed skills with:

```bash
npx skills ls --global
```

If the CLI is unavailable, clone the repository into the global skills directory used by your agent:

```bash
git clone https://github.com/m031n/design-document-writer.git ~/.codex/skills/design-document-writer
```

Restart the agent session if the skill does not appear in the available skills list.

## Use it

Ask for a design process document in Farsi and provide whatever source material is available:

```text
Create a design document for this problem. Here is the current context, the research process, the analytics, the design options, and the Figma links.
```

The workflow is:

1. Read the supplied problem, process, artifacts, and links.
2. Audit the input against the document structure and ask focused questions about missing sections.
3. Record unavailable information instead of filling gaps with assumptions.
4. Separate Evidence, Interpretation, Assumption, Decision, and Open Question.
5. Connect Evidence to Insights, Design Options, trade-offs, and the final decision.
6. Run a humanize and validation pass before returning the Markdown document.

## Figma benchmarks

When a Figma link is provided and direct review is requested, the skill can use available read-only Figma tools to inspect the relevant file, page, section, or frame. It records:

- the original Figma link;
- the exact pages, sections, or frames reviewed;
- visible screens, flows, labels, Notes, Annotations, Comments, and comparison tables when exposed by the connected tool;
- direct observations separately from interpretation;
- what each benchmark finding changed in the requirements or design decision.

If a Figma note or comment is not accessible, the skill marks it as `Not accessible` or `Needs validation`. It never assumes that hidden content is absent.

## Repository structure

```text
design-document-writer/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── document-template.md
    ├── examples.md
    ├── humanizing-checklist.md
    ├── question-checklist.md
    ├── validation-checklist.md
    └── writing-style.md
```

### References

- `document-template.md`: DDS-aligned Markdown structure and tables
- `question-checklist.md`: completeness questions asked before drafting
- `examples.md`: reusable patterns from SL/TP, order segregation, Market Depth, and benchmark review
- `writing-style.md`: Farsi product-writing guidance
- `humanizing-checklist.md`: targeted edits for natural Farsi writing
- `validation-checklist.md`: final Evidence, links, design reasoning, and writing QA

## Design decisions

The skill treats a decision to preserve the current experience as valid design work. A document may conclude that the team should:

- `Proceed`: implement the selected direction;
- `Iterate`: gather more Evidence or explore further;
- `Defer`: keep the issue visible for a later phase or trigger;
- `No change`: keep the current behavior because the evidence or risk profile does not justify a change.

For `Defer` and `No change`, the document should explain the evidence, remaining uncertainty, risks of changing, and the condition that would reopen the decision.
