# HF_Leaderboard_Lab_Results

**Project:** `L_AGENCYSWARM`  
**Tier:** `TIER_4_INFERENCE_AGENTS`  
**Slug:** `crewAIInc/crewAI`  
**Commit:** `a0d16dde6ecf`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **53.47 ms** |
| Min latency | 46.01 ms |
| Max latency | 66.53 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **38** |
| Tokenization latency | 2.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5841 |
| Classification latency | 77.49 ms |
| Status | **PASS** |

**Input text tokenized:**
```
L_AGENCYSWARM (crewAIInc/crewAI) — 31865 files, 355698 source lines, licence MIT, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'l', '_', 'agency', '##sw', '##arm', '(', 'crew', '##ai', '##in', '##c', '/', 'crew', '##ai', ')', '—', '318', '##65', 'files', ',']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_