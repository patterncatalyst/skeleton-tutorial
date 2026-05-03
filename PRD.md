# Product Requirements Document — TODO: Project name

> Replace every `TODO:` marker before considering this PRD complete.
> Anything still saying TODO is something you haven't decided yet,
> and you should decide before writing tutorial content.

---

## 1. Summary

**One sentence:** TODO: what this tutorial teaches, to whom.

**One paragraph:** TODO: a slightly longer version. What's the
topic, what's the reader's situation when they arrive, what's
their situation when they finish, and why does this tutorial need
to exist when other resources don't already serve this audience?

---

## 2. Problem statement

### Who is the reader?

TODO: write 2-4 sentences describing the reader concretely. Not
"developers" — that's too vague. Try:

- What's their job title or role?
- What do they already know? (assumed prerequisites)
- What don't they know that this tutorial covers?
- What's their motivation for picking up this tutorial — a
  deadline, a curiosity, a job requirement, a personal project?

### What's their pain today?

TODO: what problem do they hit without this tutorial? "Existing
docs are scattered" / "the official documentation assumes prior
exposure to X" / "people end up cargo-culting working examples
without understanding why" / etc. Be specific.

### Why now?

TODO: optional, but useful. Is the topic newly relevant? Did
something change upstream that makes this worth writing? Did you
just spend a hard week debugging something and want to spare
others?

---

## 3. Goals and non-goals

### Goals (what success looks like)

TODO: 3-6 bullet points. Each should be testable.

- A reader who finishes the tutorial can do TODO without
  consulting other resources
- A reader who finishes the tutorial understands why TODO works
  the way it does, not just the commands to copy
- The tutorial's runnable examples build and run end-to-end on
  TODO platforms with no manual fixups
- TODO: any other measurable goal

### Non-goals (what this is NOT)

TODO: 3-5 bullet points. These are things readers might
reasonably expect but you've decided not to cover. Being explicit
prevents scope creep.

- This tutorial does NOT teach TODO (assumed prerequisite)
- This tutorial does NOT cover TODO (out of scope; deeper topic
  for a follow-on)
- This tutorial does NOT compare TODO with TODO (vendor-neutral
  language; readers can compare for themselves)
- TODO: any other deliberate omission

---

## 4. Audience details

### Primary audience

TODO: who is this for first? What's their level? What platform
are they on? What's their stack?

### Secondary audience

TODO: who else might benefit, even if they're not the focus? How
will the tutorial gracefully serve them without distracting the
primary?

### Audience NOT served

TODO: who is this explicitly not for? "Beginners with no
container experience" / "people on Windows without WSL" / etc.
Saying so up front prevents wasted effort and frustrated readers.

---

## 5. Scope and section outline

A first-cut list of sections. This will evolve as you write —
that's expected. The goal here is to set rough scope and
estimate effort.

### Sections

| §  | Title                       | Purpose                                       | Est. duration |
|----|-----------------------------|-----------------------------------------------|---------------|
| 0  | Outline                     | Reader's map of what's ahead                  | 2 min         |
| 1  | Prerequisites               | What needs to be installed and configured     | 15 min        |
| 2  | TODO: introduction          | Conceptual grounding before any commands      | TODO          |
| 3  | TODO: first hands-on        | Smallest possible working example             | TODO          |
| 4  | TODO                        | TODO                                          | TODO          |
| ...| ...                         | ...                                           | ...           |
| N  | Where to go next            | Pointers to deeper resources                  | 5 min         |

**Total estimated duration for a reader:** TODO sum

### Optional appendices or follow-ons

TODO: list any sections you'd like to write but consider
optional or deferrable. Things like "advanced patterns,"
"troubleshooting," or "production considerations."

---

## 6. Runnable examples

### Will this tutorial have runnable code examples?

- [ ] Yes
- [ ] No
- [ ] Partial (some sections, not others)

### If yes, what languages or tools?

TODO: list. For each, note:

- The expected runtime versions
- The build tool (Maven, npm, pip, go build, cargo, etc.)
- Whether it needs a service to talk to (database, queue, etc.)
- Whether it needs special hardware (GPU, FIPS-validated host,
  etc.)

### Test strategy for examples

How will you confirm the examples actually work? Options:

- [ ] Per-example test scripts under `scripts/` (recommended for
  HTTP services and CLI tools — see `scripts/test-template.sh`)
- [ ] Aggregator script that runs all tests in sequence
- [ ] CI integration via GitHub Actions
- [ ] Manual verification only (lower bar, document why)

The reconciliation plan should track every example's verification
state — `unverified` until a test confirms it works.

---

## 7. Diagrams

### Will this tutorial use diagrams?

- [ ] Yes, paired SVG + Excalidraw source as the skeleton supports
- [ ] Yes, but a different format (specify TODO)
- [ ] No

### Anticipated diagrams

TODO: rough list. Don't try to be exhaustive — diagrams emerge
from prose. But sketch the obvious ones:

- A high-level "how the pieces fit together" diagram for §2
- A flow or sequence diagram per major operational pattern
- TODO

---

## 8. Success metrics

How will you know this tutorial succeeded?

### Verification metrics (you control these)

- All runnable examples pass `scripts/test-all-examples.sh` on
  TODO platforms
- Reconciliation plan shows all G.2 rows as `verified`
- §1 prerequisites instructions tested on a fresh VM of each
  target platform
- TODO: other deliverable-level metrics

### Adoption metrics (harder to control, depend on external factors)

- TODO: any external metric you care about, like search rank,
  inbound links, or feedback. Note: these are slow signals and
  depend on factors outside the tutorial itself.

---

## 9. Constraints and dependencies

### Technical constraints

TODO: list. Examples:

- The tutorial assumes Podman, not Docker
- The tutorial targets Fedora 43+ and current macOS as primary
  platforms
- Examples must run rootless
- No examples may require paid services or accounts behind
  paywalls
- TODO

### Editorial constraints

TODO: list. Examples:

- Vendor-neutral language; no comparisons to specific competitor
  products
- No celebrity endorsements, no "we" voice (use "you" for the
  reader and either passive or third-person otherwise)
- Code examples must be copy-pasteable without modification
- Diagrams use SVG, not PNG, so they scale on hi-DPI displays
- TODO

### Dependencies

TODO: external things this tutorial depends on. Examples:

- Hummingbird image catalog availability at quay.io/hummingbird
- Specific Podman version with feature X
- Upstream tool TODO at version TODO
- TODO

If any of these become unavailable or change, what's the impact?

---

## 10. Risks and mitigations

| Risk                                         | Impact      | Likelihood | Mitigation                                          |
|----------------------------------------------|-------------|------------|-----------------------------------------------------|
| TODO: upstream tool changes mid-write        | TODO        | TODO       | Pin to specific versions; note in reconciliation plan |
| TODO: example runs on Fedora but not macOS   | TODO        | TODO       | Test cross-platform before declaring G.2 verified   |
| TODO: too long; readers don't finish         | High        | Medium     | Front-load value; sectioned so partial reads work   |
| TODO: too short; misses important context    | TODO        | TODO       | Cover the "why" alongside the "how" in each section |
| TODO                                         | TODO        | TODO       | TODO                                                |

---

## 11. Timeline and milestones

Rough estimates. Adjust as you go.

| Milestone                            | Est. effort   | Done? |
|--------------------------------------|---------------|-------|
| PRD reviewed and approved            | 1-2 hours     | [ ]   |
| Skeleton scaffolded and config'd     | 30 min        | [ ]   |
| §1 prerequisites drafted             | 2-4 hours     | [ ]   |
| First runnable example working       | 2-6 hours     | [ ]   |
| Hello-world tutorial section drafted | 2-4 hours     | [ ]   |
| Half the sections drafted            | TODO          | [ ]   |
| All sections drafted (zero-draft)    | TODO          | [ ]   |
| All examples passing test scripts    | TODO          | [ ]   |
| Cross-platform verification complete | TODO          | [ ]   |
| Diagrams drafted                     | TODO          | [ ]   |
| Editorial pass for tone and voice    | 4-8 hours     | [ ]   |
| Reconciliation plan reflects reality | TODO          | [ ]   |
| Public announce / launch             | -             | [ ]   |

**Hard deadline (if any):** TODO

**Realistic launch target:** TODO

---

## 12. Open questions

A list of things you don't have answers to yet. Update as you
think about them.

- TODO: question
- TODO: question
- TODO: question

---

## 13. Decision log

Major decisions made during the project, with rationale. Add to
this as you go — it's a future-self gift when you're trying to
remember why you chose X over Y.

| Date       | Decision                                | Rationale                                          |
|------------|-----------------------------------------|----------------------------------------------------|
| TODO       | TODO: e.g. "Podman over Docker"         | TODO: e.g. "default on target platform; rootless"  |
| TODO       | TODO                                    | TODO                                               |

---

## 14. Stakeholders

If anyone other than you cares about this project, list them
here. For solo projects, this section can be deleted.

| Name           | Role                              | What they need                          |
|----------------|-----------------------------------|------------------------------------------|
| TODO           | TODO: e.g. "Reviewer"             | TODO: e.g. "PR notifications on main"   |

---

## How to use this PRD

Once filled in, this document is meant to be:

- The first thing you read at the start of each work session — a
  3-minute scan to recenter on what you're building and why.
- The reference when scope creep tempts you ("is this in section
  5? no? then it's not in this project").
- The handoff document when an AI assistant or human collaborator
  joins partway through.

Keep it under version control alongside the rest of the project.
When something significant changes (new section added, scope
reduced, a goal dropped), update the relevant section and commit
the change with a clear message — your future self will thank
you for the audit trail.

When the project ships, this PRD becomes a record of "what we
intended" against the reconciliation plan's "what we shipped."
The gap between them is usually instructive.
