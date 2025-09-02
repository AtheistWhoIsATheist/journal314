# Runbook — How to Operate NSPE

1) Ensure data files exist:
   - `data/journal314/j314_master.json` (canonical J314)
   - `data/ren/ren_episodes.json` (REN corpus)

2) Load the system prompt:
   - Use `engine/prompts/master_operational_prompt.txt` as the system prompt/context.

3) Start the φ-Loop:
   - Send: `:INITIATE_NT_DENSIFICATION_ENGINE: φ-LOOP ← 1 PASS ← α BEGIN`

4) Between passes:
   - Use Command DSL (`engine/spec/command_dsl.md`) to zoom, expand, or retreat.
   - Use Protocols (`engine/protocols/`) to run targeted methods.

5) Residue:
   - Every unresolved issue is logged to `engine/rmp/residue_ledger.json`.
   - Review and assign before each next loop.

6) Tests:
   - Use `engine/tests/paradox_cases.json` + `acceptance_matrix.yaml` for validation sweeps.

7) Governance:
   - Policies in `engine/compliance/`. Versioning rules in `engine/ops/versioning.md`.