# HF_Leaderboard_Lab_Results

**Project:** `K_OPENEVAL`  
**Tier:** `TIER_6_SECURITY_EVAL`  
**Slug:** `EleutherAI/lm-evaluation-harness`  
**Commit:** `d6de81643928`  
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
| Avg latency | **46.01 ms** |
| Min latency | 43.5 ms |
| Max latency | 51.54 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **41** |
| Tokenization latency | 1.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5895 |
| Classification latency | 79.99 ms |
| Status | **PASS** |

**Input text tokenized:**
```
K_OPENEVAL (EleutherAI/lm-evaluation-harness) — 16415 files, 108821 source lines, licence MIT, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'k', '_', 'open', '##eva', '##l', '(', 'el', '##eu', '##ther', '##ai', '/', 'l', '##m', '-', 'evaluation', '-', 'harness', ')', '—']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_