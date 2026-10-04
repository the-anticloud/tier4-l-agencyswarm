# Deploy Guide — L_AGENCYSWARM
**Tier:** TIER_4_INFERENCE_AGENTS | **Stack:** Python 3.11, agencyswarm 0.x, PAX 27B, asyncio, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, agencyswarm 0.x (install from source), PAX 27B weights, asyncio.

## Environment
16GB RAM. GPU for PAX. Multiple concurrent PAX calls — use K_NANOVLLM continuous batching.

## AIOSS Integration
```bash
aioss init --module L_AGENCYSWARM --output ./l_agencyswarm.aioss
aioss append --chain ./l_agencyswarm.aioss --payload ./output.bin --module L_AGENCYSWARM
aioss verify --chain ./l_agencyswarm.aioss
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
    module="L_AGENCYSWARM",
    aioss_chain="./L_AGENCYSWARM.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./L_AGENCYSWARM.aioss --verbose
python -m L_AGENCYSWARM.tests.smoke
```
