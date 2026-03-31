# Changelog

---

## 31 March 2026

### AI Literacy Assessment

- **First AI literacy assessment: Level 3 — Habitat Engineer** — full
  evidence-based assessment documenting L2-L5 signals, three-discipline
  scoring (context 4/5, constraints 5/5, guardrails 3/5), strengths,
  gaps, and recommendations. Guardrail design ceiling identified:
  configured but not yet operational.
- **Assessment badge and mechanism map updated** — AI Literacy Level 3
  badge added to README, assessor agent and /assess command added to
  mechanism map.
- **First reflection captured** — REFLECTION_LOG.md populated with
  assessment reflection, activating the compound learning system.

---

## 30 March 2026

### Initial habitat and application

- **Project scaffolded with ai-literacy-superpowers** — CLAUDE.md,
  HARNESS.md (7 constraints, all enforced), AGENTS.md, MODEL_ROUTING.md,
  REFLECTION_LOG.md, six-agent team, four skills, CI workflows,
  Dependabot configuration, and weekly mutation testing.
- **mdcheck link checker implemented** — Go CLI that parses Markdown
  files for inline links, reference links, and autolinks, then checks
  each via HTTP HEAD (URLs) or file existence (local paths). Reports
  broken links with file, line, text, and reason. Spec-first workflow
  with TDD — 15 tests, 96% coverage on parser and checker.
