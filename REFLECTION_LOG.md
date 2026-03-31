# Reflection Log

<!-- Agents append reflections here. Human reviews and promotes to
     AGENTS.md. Append-only. -->

## Entry Format

- **Date**: YYYY-MM-DD
- **Agent**: which agent
- **Task**: what was done
- **Surprise**: what was unexpected
- **Proposal**: what to add to AGENTS.md
- **Improvement**: what would improve the process

---

- **Date**: 2026-03-31
- **Agent**: assessor (via /assess command)
- **Task**: First AI literacy assessment of the exemplar — Level 3 Habitat Engineer
- **Surprise**: The exemplar scored 10/10 on L3 habitat signals but the weakest discipline (guardrail design at 3/5) pulled the ceiling down from L4. The gap isn't missing infrastructure — it's missing practice. REFLECTION_LOG.md was empty, the harness hadn't been revisited, and the orchestrator pipeline had only been used once. The distinction between "configured" and "operational" is the difference between L3 and L4.
- **Proposal**: Add to GOTCHAS: "A fully configured habitat (all signals present) does not mean an operational one. The assessment distinguishes between infrastructure that exists and infrastructure that's been exercised. Empty REFLECTION_LOG.md and unrevised HARNESS.md are the clearest signals that the habitat is configured but not yet lived in."
- **Improvement**: The assessment revealed that the exemplar has no operating cadence documented anywhere. Add a "Quarterly Operating Cadence" section to CLAUDE.md that specifies when to run /harness-audit, review reflections, and check cost data.
