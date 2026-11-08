# Deploy Guide — K_OPENEVAL
**Tier:** TIER_6_SECURITY_EVAL | **Stack:** Python 3.11, PAX 27B (judge), eval datasets, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, PAX 27B as judge (requires good quality model), T4 GPU.

## Environment
Two PAX 27B instances (or sequential): one judge, one evaluated. T4 GPU.

## AIOSS Integration
```bash
aioss init --module K_OPENEVAL --output ./k_openeval.aioss
aioss append --chain ./k_openeval.aioss --payload ./output.bin --module K_OPENEVAL
aioss verify --chain ./k_openeval.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="K_OPENEVAL",
    aioss_chain="./K_OPENEVAL.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./K_OPENEVAL.aioss --verbose
python -m K_OPENEVAL.tests.smoke
```
