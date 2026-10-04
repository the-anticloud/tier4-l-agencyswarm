# 3-Seed Simulation — L_AGENCYSWARM

**Seeds:** `36800` · `68137` · `2336`

**Seed method:** `sha256("L_AGENCYSWARM")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `L_AGENCYSWARM`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 7.0433 | 0.174 | ±0.341 |
| throughput_tokens_per_sec | 5925.0333 | 33.3619 | ±65.3893 |
| p50_latency_ms | 43.18 | 2.6384 | ±5.1713 |
| p99_latency_ms | 109.2067 | 15.3519 | ±30.0897 |
| ttft_ms | 24.77 | 1.2385 | ±2.4275 |
| mmlu_proxy | 0.6974 | 0.0262 | ±0.0514 |
| hellaswag_proxy | 0.7821 | 0.0301 | ±0.059 |
| truthfulqa_proxy | 0.6098 | 0.0205 | ±0.0402 |
| arc_proxy | 0.7014 | 0.0388 | ±0.076 |
| complexity_cyclomatic | 4.2233 | 0.6561 | ±1.286 |
| maintainability_index | 72.7733 | 4.3653 | ±8.556 |
| security_issues_high | 1.0 | 0.8165 | ±1.6003 |
| dependency_freshness_pct | 74.5333 | 2.2647 | ±4.4388 |
| test_coverage_pct | 62.4 | 3.7532 | ±7.3563 |
| doc_coverage_pct | 66.6 | 5.9335 | ±11.6297 |
| memory_mb | 3231.9667 | 235.5792 | ±461.7352 |
| gpu_util_pct | 71.3667 | 5.0678 | ±9.9329 |
| openssf_score | 6.6333 | 0.531 | ±1.0408 |
| eu_ai_act_compliance_pct | 83.8667 | 6.5708 | ±12.8788 |
| slsa_level | 1.3333 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 36800 | Seed 68137 | Seed 2336 |
|--------|------------|------------|------------|
| trl_score | 7.15 | 7.182 | 6.798 |
| throughput_tokens_per_sec | 5878.2 | 5943.5 | 5953.4 |
| p50_latency_ms | 39.47 | 44.69 | 45.38 |
| p99_latency_ms | 129.84 | 93.04 | 104.74 |
| ttft_ms | 23.4 | 26.4 | 24.51 |
| mmlu_proxy | 0.6789 | 0.6788 | 0.7344 |
| hellaswag_proxy | 0.8186 | 0.7829 | 0.7448 |
| truthfulqa_proxy | 0.6366 | 0.6057 | 0.587 |
| arc_proxy | 0.6467 | 0.7329 | 0.7245 |
| complexity_cyclomatic | 3.8 | 3.72 | 5.15 |
| maintainability_index | 75.83 | 66.6 | 75.89 |
| security_issues_high | 0 | 2 | 1 |
| dependency_freshness_pct | 72.2 | 77.6 | 73.8 |
| test_coverage_pct | 60.0 | 59.5 | 67.7 |
| doc_coverage_pct | 68.1 | 73.0 | 58.7 |
| memory_mb | 2955.5 | 3531.2 | 3209.2 |
| gpu_util_pct | 77.4 | 71.7 | 65.0 |
| openssf_score | 6.06 | 7.34 | 6.5 |
| eu_ai_act_compliance_pct | 87.9 | 89.1 | 74.6 |
| slsa_level | 1 | 1 | 2 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._