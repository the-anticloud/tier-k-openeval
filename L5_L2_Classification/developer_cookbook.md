# Developer Cookbook — K_OPENEVAL
**Stack:** Python 3.11, PAX 27B (judge), eval datasets, AIOSS_FORMAT
**Domain:** OpenEval: open-ended evaluation with PAX 27B as judge for subjective quality

## PAX-judge evaluation
```python
from k_openeval import OpenEvalJudge

judge = OpenEvalJudge(
    judge_model="./pax-27b-q4.gguf",
    eval_model="./pax-27b-q4-candidate.gguf",
    aioss_chain="./openeval.aioss"
)

results = judge.pairwise_eval(
    test_prompts="./anticloud_open_prompts.jsonl",
    n_comparisons=200
)
print(f"Candidate win rate: {results.candidate_win_rate:.2%}")
print(f"Tie rate: {results.tie_rate:.2%}")
print(f"Anticloud domain score: {results.domain_score:.3f}")
print(f"Chain: {results.chain_hash}")
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
