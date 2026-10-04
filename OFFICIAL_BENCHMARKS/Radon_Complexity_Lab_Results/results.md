# Radon_Complexity_Lab_Results
**Project:** `L_AGENCYSWARM` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 3.625730994152047}`
- **complexity_grade:** `A`
- **complexity_score:** `3.625730994152047`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_AGENCYSWARM\UPSTREAM\conftest.py - A (48.13)
E:\fenta\Downloa`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_AGENCYSWARM\UPSTREAM\conftest.py
    F 369:0 _filter_response_headers - C (15)
    F 347:0 _filter_request_headers - B (8)
    F 404:0 vcr_cassette_dir - B (6)
    F 16:0 _patch_vcrpy_aiohttp_compat - A (5)
    F 137:0 _patched_make_vcr_request - A (4)
    F 253:0 setup_test_environment - A (4)
    F 130:0 bedrock_host_matcher - A (3)
    F 444:0 vcr_config - A (3)
    F 124:0 _normalize_bedrock_host - A (2)
    F 173:4 _patched_from_serialized_response - A (2)
    F 191:0 cleanup_event_handlers - A (2)
    F 206:0 reset_tracing_state - A (1)
    F 238:0 reset_event_state - A (1)
    F 438:0 pytest_recording_configure - A (1)
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_AGENCYSWARM\UPSTREAM\_anticloud_egress.py
    F 38:0 _is_frontier - A (4)
    F 43:0 guarded_connect - A (4)
    F 61:0 install - A (3)
    F 33:0 is_offline - A (1)
    C 29:0 EgressDenied - A (1)
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_AGENCYSWARM\UPSTREAM\scripts\age90_file_input_runner.py
    F 41:0 _sanitize_payload - B (8)
    F 98:0 run_crew_kickoff - B (7)
    F 201:0 main - B (7)
    F 28:0 _content_summary - A (5)
    F 58:0 inspect_native_path - A (5)
    F 81:0 inspect_fallback_tool - A (3)
    F 164:0 parse_args - A (1)
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_AGENCYSWARM\UPSTREAM\scripts\wharf_runner.py
    F 230:0 main - C (11)
    C 105:0 FirecrawlAgent - B (6)
    M 108:4 FirecrawlAgen
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_