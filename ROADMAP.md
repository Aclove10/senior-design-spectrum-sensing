# Project roadmap

This is a dependency-based plan; owners and dates should be assigned in team issues. Checkboxes distinguish existing work from pending deliverables.

## 1. Preserve and document the baseline

- [x] Preserve existing GNU Radio transmitter flowgraph and generated Python.
- [x] Establish subsystem folders, contributor workflow and experiment documentation.
- [x] GNU Radio energy-detection simulation completed (team reported).
- [ ] Commit the completed simulation flowgraphs, generated code, exact settings and plots.
- [ ] Record environment versions and a reproducible simulation procedure.
- [ ] Have another teammate reproduce the simulation and attach a run record.

Exit evidence: a fresh checkout can reproduce the documented simulation. This gate does not imply RF validation.

## 2. Validate local sensing with RF hardware

- [ ] Confirm device discovery and implement/document the receiver.
- [ ] Establish noise-only baseline and threshold calibration.
- [ ] Run controlled signal-absent and signal-present trials.
- [ ] Sweep relevant signal levels and detector settings with repeated labeled trials.
- [ ] Measure detection probability, false-alarm probability and latency; report uncertainty and limitations.

Exit evidence: reviewed RF experiment records, configuration, raw-data references and measured results. RF validation remains pending.

## 3. Build cooperative sensing

- [ ] Define versioned node-report schema, identifiers, units and timestamps.
- [ ] Implement and compare candidate fusion rules.
- [ ] Test missing, delayed, duplicated and inconsistent node reports.
- [ ] Evaluate multi-node results against local detector baselines.

Exit evidence: reproducible multi-node trials with recorded inputs and fusion outputs.

## 4. Integrate blockchain

- [ ] Select chain/tooling and document the rationale.
- [ ] Define on-chain fields, access rules and off-chain data references.
- [ ] Implement contract and off-chain submission interface.
- [ ] Test authorization, invalid submissions, duplicate handling and transaction failure/retry.
- [ ] Deploy to a development/test network and verify sensing records against transaction receipts.

Exit evidence: documented contract tests, deployment configuration without secrets and end-to-end traceability. Blockchain integration remains pending.

## 5. Complete system evaluation and handoff

- [ ] Verify the RF-to-detection-to-fusion-to-ledger path.
- [ ] Compare simulation and RF results without conflating their evidence.
- [ ] Document limitations, reproducible demo, final report and presentation.
- [ ] Tag a reviewed release and archive the environment and evidence.

Schedule and scope changes belong in team issues and this roadmap.
