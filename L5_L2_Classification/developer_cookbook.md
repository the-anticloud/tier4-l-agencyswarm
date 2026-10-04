# Developer Cookbook — L_AGENCYSWARM
**Stack:** Python 3.11, agencyswarm 0.x, PAX 27B, asyncio, AIOSS_FORMAT
**Domain:** AgencySwarm: hierarchical multi-agent framework for Anticloud sovereign workflows

## Define a compliance audit agency
```python
from l_agencyswarm import AnticloudAgency, CEOAgent, ManagerAgent, WorkerAgent

# Define agents
ceo = CEOAgent(name="ComplianceCEO", pax_model="./pax-27b-q4.gguf",
               system_prompt="You direct compliance audit operations for Anticloud.",
               aioss_chain="./agency_ceo.aioss")

mgr = ManagerAgent(name="AuditManager", pax_model="./pax-27b-q4.gguf",
                   system_prompt="You coordinate audit evidence collection.",
                   aioss_chain="./agency_mgr.aioss")

worker = WorkerAgent(name="EvidenceCollector", pax_model="./pax-27b-q4.gguf",
                     system_prompt="You collect AIOSS chain evidence for compliance reports.",
                     aioss_chain="./agency_worker.aioss")

agency = AnticloudAgency(
    agents=[ceo, mgr, worker],
    hierarchy={"CEO": ["AuditManager"], "AuditManager": ["EvidenceCollector"]},
    coordinator_aioss="./agency_coordinator.aioss"
)

# Run agency task
result = agency.run("Audit all TIER_7 projects for HIPAA compliance and generate evidence package")
print(result.final_output)
print(f"Agency chain: {result.chain_hash}")
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
