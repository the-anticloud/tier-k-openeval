# L5 Narrow / L2 General Classification — K_OPENEVAL
**Platform:** Anticloud | **Tier:** TIER_6_SECURITY_EVAL | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
K_OPENEVAL uses PAX 27B as an evaluator judge for open-ended, subjective quality dimensions: response coherence, factual groundedness, instruction following, and Anticloud-specific domain accuracy. Narrow scope: Anticloud model evaluation.

## L2 General
L2 General: K_OPENEVAL provides consistent quality evaluation for any model or model update across all tiers. PAX 27B as judge ensures domain-specific quality assessment.

## PAX 27B Integration
One PAX 27B instance is the judge; another (or an older version) is the model under evaluation. K_OPENEVAL manages the pair-wise comparison and aggregation.

## AIOSS Audit Chain
Every evaluation run (evaluated model hash + judge model hash + pairwise comparisons hash + win rate + Anticloud score) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
ISO/IEC 42001 (AI evaluation methodology). NIST AI RMF 1.0.
