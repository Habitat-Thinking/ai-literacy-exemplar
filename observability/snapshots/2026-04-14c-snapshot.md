# Harness Health Snapshot — 2026-04-14 (post-promotion)

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

## Mutation Testing

- Go kill rate: available via CI artifacts (mutation-testing.yml, weekly)
- Trend: no new data since last snapshot — check CI artifacts

## Compound Learning

- REFLECTION_LOG entries: 8 (3 new since 2026-04-14 previous snapshot)
- Entries with signal (Surprise + Proposal): 8/8 (100%)
- AGENTS.md gotchas: 3 (2 new since previous snapshot)
- AGENTS.md arch decisions: 4
- Promotions since last snapshot: 2 (L4-to-L5, two-speed-pipeline)
- Unpromoted reflections awaiting review: 3 (entries 6, 7, 8; all from
  2026-04-14)

## Session Quality

- Depletion check documented: yes (CLAUDE.md)
- 90-minute pause cadence: documented

## Operational Cadence

- Last /harness-audit: 2026-04-14 (today, quarterly — on schedule)
- Last /assess: 2026-04-14 (today, quarterly — on schedule)
- Last /reflect: 2026-04-14 (today)
- Last snapshot: 2026-04-14 (today)
- Quarterly cadence documented: yes (CLAUDE.md)
- Outer loop overdue: no

## Cost Indicators

- Model routing configured: yes (MODEL_ROUTING.md)
- Cost snapshots captured: 0 (first capture due 2026-06-30)

## Meta

- Snapshot currency: current (today)
- Cadence compliance: all cadences on schedule
- Learning flow: active — 3 new reflections, 2 promotions since last
  snapshot. Promotion bottleneck resolved.
- GC effectiveness: 5 rules configured, 0 findings (2 consecutive
  snapshots — monitoring, not yet at 3-snapshot silent threshold)
- Trend alerts: none
- **Aggregate health: Healthy**

## Trends (vs 2026-04-14 revised)

| Metric | Previous | Current | Delta |
| --- | --- | --- | --- |
| Constraints enforced | 9/13 (69%) | 11/13 (85%) | +16% (2 secrets constraints promoted) |
| GC rules active | 5/5 | 5/5 | stable |
| REFLECTION_LOG entries | 8 | 8 | stable |
| Entries with signal | 100% | 100% | stable |
| AGENTS.md gotchas | 3 | 3 | stable |
| Unpromoted entries | 3 | 3 | stable |
| Snapshot age (days) | 0 | 0 | current |
| Cadence compliance | on schedule | on schedule | stable |
| Health status | Attention | Healthy | improved |
