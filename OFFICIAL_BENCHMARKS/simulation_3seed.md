# 3-Seed Simulation — K_OPENEVAL

**Seeds:** `62095` · `93432` · `27631`

**Seed method:** `sha256("K_OPENEVAL")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `K_OPENEVAL`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 6.94 | 0.1103 | ±0.2162 |
| throughput_tokens_per_sec | 1969.3333 | 23.7981 | ±46.6443 |
| p50_latency_ms | 42.12 | 4.4566 | ±8.7349 |
| p99_latency_ms | 112.5767 | 12.6514 | ±24.7967 |
| ttft_ms | 27.1367 | 4.7465 | ±9.3031 |
| mmlu_proxy | 0.7237 | 0.0304 | ±0.0596 |
| hellaswag_proxy | 0.7842 | 0.0264 | ±0.0517 |
| truthfulqa_proxy | 0.5729 | 0.0204 | ±0.04 |
| arc_proxy | 0.6583 | 0.0183 | ±0.0359 |
| complexity_cyclomatic | 4.4567 | 0.2894 | ±0.5672 |
| maintainability_index | 72.5733 | 4.1201 | ±8.0754 |
| security_issues_high | 0.3333 | 0.4714 | ±0.9239 |
| dependency_freshness_pct | 84.8 | 2.276 | ±4.461 |
| test_coverage_pct | 59.9333 | 10.3493 | ±20.2846 |
| doc_coverage_pct | 67.1333 | 6.5137 | ±12.7669 |
| memory_mb | 109.4333 | 6.6178 | ±12.9709 |
| gpu_util_pct | 68.0667 | 5.8019 | ±11.3717 |
| openssf_score | 6.42 | 0.5266 | ±1.0321 |
| eu_ai_act_compliance_pct | 83.3667 | 0.7134 | ±1.3983 |
| slsa_level | 1.3333 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 62095 | Seed 93432 | Seed 27631 |
|--------|------------|------------|------------|
| trl_score | 6.847 | 6.878 | 7.095 |
| throughput_tokens_per_sec | 2002.5 | 1947.8 | 1957.7 |
| p50_latency_ms | 48.41 | 38.63 | 39.32 |
| p99_latency_ms | 119.88 | 123.07 | 94.78 |
| ttft_ms | 33.76 | 24.77 | 22.88 |
| mmlu_proxy | 0.7452 | 0.7452 | 0.6807 |
| hellaswag_proxy | 0.7541 | 0.8183 | 0.7802 |
| truthfulqa_proxy | 0.5997 | 0.5689 | 0.5502 |
| arc_proxy | 0.6837 | 0.6499 | 0.6414 |
| complexity_cyclomatic | 4.7 | 4.62 | 4.05 |
| maintainability_index | 69.63 | 78.4 | 69.69 |
| security_issues_high | 0 | 1 | 0 |
| dependency_freshness_pct | 82.5 | 87.9 | 84.0 |
| test_coverage_pct | 67.5 | 67.0 | 45.3 |
| doc_coverage_pct | 60.3 | 65.2 | 75.9 |
| memory_mb | 109.1 | 101.5 | 117.7 |
| gpu_util_pct | 60.8 | 75.0 | 68.4 |
| openssf_score | 5.85 | 7.12 | 6.29 |
| eu_ai_act_compliance_pct | 82.4 | 83.6 | 84.1 |
| slsa_level | 1 | 1 | 2 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._