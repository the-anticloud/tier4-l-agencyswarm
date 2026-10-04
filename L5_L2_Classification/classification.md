# L5 Narrow / L2 General Classification — L_AGENCYSWARM
**Platform:** Anticloud | **Tier:** TIER_4_INFERENCE_AGENTS | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
L_AGENCYSWARM integrates the AgencySwarm hierarchical agent framework with Anticloud's PAX harness. Narrow scope: Anticloud operational workflows — compliance auditing agencies, clinical analysis agencies, security evaluation agencies. Not a general-purpose agent platform.

## L2 General
L2 General: L_AGENCYSWARM enables any tier to define hierarchical agent agencies with CEO/manager/worker roles. TIER_6 security agencies and TIER_7 clinical agencies both use the same AgencySwarm primitives.

## PAX 27B Integration
PAX 27B powers all agents in the agency. CEO agent directs managers; managers direct workers; all inference calls go through PAX 27B with individual AIOSS chain entries per agent interaction.

## AIOSS Audit Chain
Every agency task (CEO directive hash + manager assignments hash + worker outputs hash + final synthesis hash) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
NIST AI RMF 1.0 (multi-agent accountability). ISO/IEC 42001 (AI governance).
