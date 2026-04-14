# Harness Health Snapshot — 2026-04-14 (post-format-feature)

## Enforcement

- Constraints: 11/13 enforced (85%)
- Technical: 5 deterministic | 2 agent | 1 weekly deterministic | 1 unverified
- Governance: 3 deterministic | 1 agent | 1 unverified
- Unverified: SBOM generation (activate with first external dependency),
  approved dependency licenses (activate with first external dependency)
- Drift detected: no

## Garbage Collection

- Rules active: 5/5
- Findings since last snapshot: 0
- Consecutive zero-finding snapshots: 4 (crossed 3-snapshot threshold —
  verify GC rules are executing, not just configured)

## Mutation Testing

- Go kill rate: unavailable — 2026-04-13 run crashed (Go 1.26.1
  toolchain panic in go/types). Go 1.26.2 merged to main via PR #29;
  next weekly run (2026-04-20) should produce a valid score.
- Trend: no usable data yet

## Compound Learning

- REFLECTION_LOG entries: 7
- Entries with signal (Surprise + Proposal): 7/7 (100%)
- AGENTS.md gotchas: 3
- AGENTS.md arch decisions: 4
- Promotions since last snapshot: 0
- Unpromoted reflections awaiting review: 3 (entries 5, 6, 7; all from
  2026-04-14)

## Session Quality

- Depletion check documented: yes (CLAUDE.md)
- 90-minute pause cadence: documented

## Operational Cadence

- Last /harness-audit: 2026-04-14 (quarterly — on schedule)
- Last /assess: 2026-04-14 (quarterly — on schedule)
- Last /reflect: 2026-04-14
- Last snapshot: 2026-04-14
- Quarterly cadence documented: yes (CLAUDE.md)
- Outer loop overdue: no

## Cost Indicators

- Model routing configured: yes (MODEL_ROUTING.md)
- Cost snapshots captured: 0 (first capture due 2026-06-30)

## Meta

- Snapshot currency: current (today)
- Cadence compliance: all cadences on schedule
- Learning flow: 3 unpromoted reflections from today — not yet overdue
  (30-day review window). No new promotions since last snapshot.
- GC effectiveness: 4 consecutive zero-finding snapshots — crossed the
  3-snapshot silent threshold. Next action: manually run one GC rule
  (e.g. documentation freshness) to confirm it executes and produces
  expected output. If it genuinely finds nothing, the codebase is clean.
  If it errors silently, the rule needs fixing.
- Trend alerts: mutation testing data gap (Go toolchain crash)
- **Aggregate health: Healthy**

## Trends (vs 2026-04-14c)

| Metric | Previous | Current | Delta |
| --- | --- | --- | --- |
| Constraints enforced | 11/13 (85%) | 11/13 (85%) | stable |
| GC rules active | 5/5 | 5/5 | stable |
| REFLECTION_LOG entries | 8 | 7 | -1 (recount correction) |
| Entries with signal | 100% | 100% | stable |
| AGENTS.md gotchas | 3 | 3 | stable |
| Unpromoted entries | 3 | 3 | stable |
| Consecutive GC zeroes | 2 | 4 | +2 (threshold crossed) |
| Mutation data | unavailable | unavailable | gap persists |
| Health status | Healthy | Healthy | stable |

---

```yaml
observatory_metrics:
  schema_version: "1.0.0"
  snapshot_date: "2026-04-14"

  habitat_configuration:
    context_depth:
      claude_md: true
      agents_md: true
      model_routing_md: true
      skills_count: 5
      score: 1.0

    constraint_maturity:
      total: 13
      enforced: 11
      deterministic: 9
      agent: 3
      unverified: 2
      enforcement_ratio: 0.85

    entropy_management:
      gc_rules_total: 5
      gc_rules_active: 5
      gc_active_ratio: 1.0
      gc_findings_since_last: 0
      consecutive_zero_snapshots: 4

    compound_learning:
      reflection_count: 7
      signal_ratio: 1.0
      gotcha_count: 3
      arch_decision_count: 4
      promotions_since_last: 0
      unpromoted_count: 3
      velocity: 0.0

    feedback_loops:
      depletion_check: true
      session_cadence_minutes: 90

    agent_delegation:
      agent_count: 7
      model_routing: true

    observability:
      snapshot_cadence: "weekly"
      last_audit: "2026-04-14"
      last_assessment: "2026-04-14"
      last_reflection: "2026-04-14"
      cadence_compliance: true

  outcomes:
    mutation_kill_rate_go: null
    cost_monthly_avg: null
    cost_budget_status: "not set"

  operational_cadence:
    days_since_audit: 0
    days_since_assessment: 0
    days_since_reflection: 0
    days_since_snapshot: 0

  regression_indicators:
    snapshot_stale: false
    cadence_overdue: false
    learning_stalled: false
    gc_silent_threshold_crossed: true
    mutation_data_gap: true

  governance:
    constraint_count: 5
    deterministic_count: 3
    agent_count: 1
    unverified_count: 1

  health: "Healthy"
```

---
