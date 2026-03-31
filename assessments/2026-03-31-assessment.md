# AI Literacy Assessment — ai-literacy-exemplar

**Date**: 2026-03-31
**Assessed level**: Level 3 — Habitat Engineer
**Assessor**: assessor agent (via /assess command)

---

## Evidence Summary

### Level 0 — Aware

| Signal | Present | Evidence |
| ------ | ------- | -------- |
| AI tools in use | Yes | Claude Code with ai-literacy-superpowers plugin |
| Basic prompting | Yes | Direct Claude Code sessions for development |

### Level 1 — Prompter

| Signal | Present | Evidence |
| ------ | ------- | -------- |
| Structured prompts | Yes | CLAUDE.md with conventions, spec-first workflow |
| Context provision | Yes | 4 skills provide domain context to agents |
| Output review | Yes | Code review agent in pipeline |

### Level 2 — Verifier

| Signal | Present | Evidence |
| ------ | ------- | -------- |
| CI workflows | Yes | `lint-markdown.yml`, `go-tests.yml` (2 workflows) |
| Test coverage | Yes | 96% on parser.go and checker.go (85% threshold) |
| Vulnerability scanning | Yes | govulncheck in CI, Dependabot for gomod + actions |
| Mutation testing | Yes | Weekly `mutation-testing.yml` via go-mutesting |
| Linting | Yes | markdownlint-cli2 on all Markdown files |

**L2 strength: 5/5** — comprehensive verification infrastructure

### Level 3 — Habitat Engineer

| Signal | Present | Evidence |
| ------ | ------- | -------- |
| CLAUDE.md | Yes | Literate programming, CUPID, spec-first, TDD, branch discipline |
| HARNESS.md | Yes | 7 constraints, 7/7 enforced (4 deterministic, 2 agent, 1 weekly) |
| AGENTS.md | Yes | Populated with ARCH_DECISIONS (3), GOTCHAS (2), STYLE (1) |
| MODEL_ROUTING.md | Yes | Model-tier guidance for 6-agent team |
| REFLECTION_LOG.md | Yes | Structure present, no entries yet |
| Skills | Yes | 4 project-local skills (LP, CUPID, supply chain, dep audit) |
| Agents | Yes | 7 agents (orchestrator, spec-writer, tdd, go-implementer, code-reviewer, integration, docker-security) |
| Commands | Yes | 3 commands (/reflect, /worktree, /assess) |
| Hooks | Yes | 3 hooks via plugin (PreToolUse constraint gate, Stop drift check, Stop reflection prompt) |
| Garbage collection | Yes | 1 GC rule (documentation freshness) |

**L3 strength: 10/10 signals present** — fully configured habitat

### Level 4 — Specification Architect

| Signal | Present | Evidence |
| ------ | ------- | -------- |
| Spec-first workflow | Yes | `specs/001-link-checker/spec.md` with stories, scenarios, FRs |
| Implementation plan | Yes | `specs/001-link-checker/plan.md` with module structure, algorithms |
| Orchestrator with gates | Yes | Plan approval gate + MAX_REVIEW_CYCLES=3 |
| Pipeline used | Partial | Orchestrator used for initial build; not yet used for subsequent changes |

**L4 assessment**: Evidence is present but the pipeline hasn't been
exercised across multiple feature cycles. The spec-first workflow is
declared in CLAUDE.md but there is only one spec to demonstrate it.

### Level 5 — Sovereign Engineer

| Signal | Present | Evidence |
| ------ | ------- | -------- |
| Cost tracking | No | No cost data collected or reviewed |
| Operating rhythm | No | No quarterly audit cadence established |
| Reflection practice | No | REFLECTION_LOG.md exists but has no entries |
| Cross-session learning | Partial | AGENTS.md populated but not from actual reflections |
| Observability dashboard | No | README describes what to track, no implementation |

**L5 assessment**: Infrastructure exists (MODEL_ROUTING.md,
REFLECTION_LOG.md) but operating practices have not started.

---

## Three-Discipline Assessment

| Discipline | Score | Rationale |
| ---------- | ----- | --------- |
| Context engineering | 4/5 | CLAUDE.md, skills, AGENTS.md all strong. No evidence of iterative refinement across sessions. |
| Architectural constraints | 5/5 | HARNESS.md 7/7 enforced, CI workflows, mutation testing, Dependabot. Exemplary. |
| Guardrail design | 3/5 | Agent pipeline exists with safety gates. Not exercised beyond initial build. No operating rhythm, no reflections captured, harness not revisited. |

**Ceiling**: Guardrail design at 3/5 limits the assessed level.

---

## Assessed Level: 3 — Habitat Engineer

The exemplar has strong L2 verification infrastructure and a fully
configured L3 habitat with all expected signals present. L4 evidence
exists (spec, plan, orchestrator) but hasn't been exercised across
multiple feature cycles. The weakest discipline (guardrail design at
3/5) sets the ceiling at Level 3.

---

## Top 3 Strengths

1. **Architectural constraints are exemplary** — 7/7 constraints
   enforced, covering tests, coverage, linting, vulnerability scanning,
   and mutation testing. Zero unverified constraints.
2. **Complete habitat configuration** — all 10 L3 signals present
   (CLAUDE.md, HARNESS.md, AGENTS.md, MODEL_ROUTING.md, skills,
   agents, commands, hooks, GC)
3. **Three-layer verification model** — tests verify behaviour,
   coverage verifies execution, mutation testing verifies the tests.
   The investigative loop is operational.

## Top 3 Gaps

1. **No reflections captured** — REFLECTION_LOG.md exists but is empty.
   The compound learning system is inert.
2. **No operating rhythm** — the harness has not been revisited since
   initial creation. No quarterly audit, no cadence documented.
3. **Pipeline not re-exercised** — the orchestrator was used for the
   initial build but has not been tested with a second feature cycle.

## Top 3 Recommendations

1. **Activate compound learning** — after the next task, run `/reflect`
   to capture the first reflection entry. Review monthly and promote
   useful entries to AGENTS.md.
2. **Establish quarterly operating cadence** — run `/harness-audit`
   quarterly. Document the cadence in CLAUDE.md. Target: first audit
   within 90 days of project creation.
3. **Exercise the pipeline on a second feature** — add a small feature
   (e.g. `--format json` output flag) end-to-end through the
   orchestrator to validate that the spec-first workflow works for
   incremental changes, not just initial builds.

---

## Immediate Adjustments Applied

1. Updated HARNESS.md audit date from 2026-03-30 to 2026-03-31
2. Added AI Literacy Level 3 badge to README.md
3. Added assessor agent and /assess command to README mechanism map
4. Captured assessment reflection in REFLECTION_LOG.md

## Workflow Operation Recommendations

| Recommendation | Frequency | First due |
| -------------- | --------- | --------- |
| Run `/reflect` after every task that produces commits | Per task | Next task |
| Run `/harness-audit` to verify harness matches reality | Quarterly | 2026-06-30 |
| Review REFLECTION_LOG.md and promote entries to AGENTS.md | Monthly | 2026-04-30 |
| Exercise orchestrator pipeline on a second feature | Once | Next feature |
| Collect and review AI usage cost data | Monthly | 2026-04-30 |
