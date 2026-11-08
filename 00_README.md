# Anticloud × OPENEVAL
> Sovereign AI integration — air-gapped, zero cloud dependency.

**Part of:** Security Eval · Anticloud FZ LLE · 0-1.gg
**Upstream:** upstream/openeval (Apache-2.0)
**License:** Apache-2.0 OR LicenseRef-Anticommons-Enterprise-1.0
**IP:** USPTO pending · Lois-Kleinner Alpasan · 2026

Behavioral test suite for LLM outputs. We add tamper-evident benchmark tracking.

```python
from openeval_anticloud import Evaluator

ev = Evaluator(
    model="pax-one-27b",
    benchmarks=["mmlu", "gsm8k", "arc"],
    ledger_path="./eval_ledger.aioss",
    local_only=True,  # no API calls
)

results = ev.run_benchmarks()
# All scores: ledger-hashed, K5-signed, reproducible
```

**Plays well with:** K-VLMEVAL, L-OPENCOMP, PAX_INFERENCE_CORE (test subject)
