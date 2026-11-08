# Radon_Complexity_Lab_Results
**Project:** `K_OPENEVAL` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 3.8627450980392157}`
- **complexity_grade:** `A`
- **complexity_score:** `3.8627450980392157`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_OPENEVAL\UPSTREAM\examples\transformer-lens.py - A (72.54)
E:\fe`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_OPENEVAL\UPSTREAM\examples\transformer-lens.py
    F 12:0 evaluate_lm_eval - A (1)
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_OPENEVAL\UPSTREAM\lm_eval\defaults.py
    F 13:0 _strtobool - A (3)
    F 38:0 default_gen_kwargs - A (3)
    F 25:0 _envbool - A (2)
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_OPENEVAL\UPSTREAM\lm_eval\evaluator.py
    F 429:0 evaluate - F (60)
    F 55:0 simple_evaluate - F (55)
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_OPENEVAL\UPSTREAM\lm_eval\evaluator_utils.py
    F 173:0 _compute_task_aggregations - B (10)
    F 430:0 _propagate_higher_is_better - B (9)
    F 449:0 _log_selected_tasks - B (7)
    F 509:0 _handle_back_comp - B (6)
    F 328:0 _get_root_groups - A (5)
    F 421:0 _propagate_num_fewshot - A (5)
    C 99:0 EvalAcc - A (5)
    F 37:0 print_writeout - A (4)
    M 120:4 EvalAcc.collect - A (4)
    M 134:4 EvalAcc._to_eval_results - A (4)
    F 49:0 get_sample_size - A (3)
    F 58:0 find_test_root - A (3)
    F 248:0 _collect_results - A (3)
    F 76:0 run_task_tests - A (2)
    F 301:0 aggregate_groups - A (2)
    F 345:0 _collect_groups_bottom_up - A (2)
    F 375:0 _process_results - A (2)
    C 29:0 ResultAcc - A (1)
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\K_OPENEVAL\UPSTREAM\lm_eval\result_schema.py
    C 110:0 _TaskMetrics - A (1)
    C 131:0 _SampleCount - A (1)
    C 141:0 _EvalConfig - A (1)
    C 163:0 SampleResult - 
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_