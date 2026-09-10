# Architecture Scorecard

Score candidate pilot architectures out of 100. Score evidence confidence separately.

| Criterion | Weight |
|---|---:|
| End-user adoption / low behavior change | 20 |
| Reliability and recovery | 15 |
| Data completeness and billing safety | 15 |
| Integration feasibility | 12 |
| Speed to pilot | 10 |
| Human validation / reversibility | 8 |
| Security and privacy | 8 |
| Offline/degraded-network tolerance | 5 |
| Operating cost | 4 |
| Scalability / reuse across clients | 3 |

## Decision bands
- 80–100: preferred pilot architecture
- 65–79: viable with explicit mitigations
- 50–64: technical proof required before build
- <50: reject/redesign

## Evidence confidence
- High: capability verified in client environment or official vendor documentation
- Medium: capability documented but not yet tested in client environment
- Low: assumption, undocumented behavior, or inferred compatibility

A high score with low evidence confidence is not a build decision.