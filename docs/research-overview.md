# Research overview — Aravinda V.

Updated October 11, 2026. My interests connect mathematical verification, transfer across environments, uncertainty, and spatial interaction. The studies below are at different stages; implemented methods, reproduced historical findings and proposed experiments are identified separately.

## Cross-Airport Transfer Under Temporal and Weather Shift

**Question:** when does a model trained at source airports transfer usefully to a different airport, and how do target history and weather affect its error and reliability?

The activity-stress study uses a trajectory-derived proxy, weather and calendar inputs, earlier source-airport dates, and later held-out target dates. A local reproducibility audit reran a revised random-forest calibration sensitivity: all eight point-reference errors matched the saved results, and the interval table reproduced exactly. Nominal 90% intervals covered 8.0–46.2% of target windows, exposing substantial undercoverage under shift. This revised representation is a post-hoc sensitivity on previously evaluated dates, rather than a fresh confirmatory test.

Point-prediction behavior depends on airport, forecast horizon, representation and model. The useful result is the combination of transfer gains, failure cases and unreliable source-calibrated intervals—not a blanket claim that one model generalizes across airports.

A separate study compares daily observed departure-delay prediction at PVG and SHA with 7/30/90/180 days of preceding target history. Saved-prediction checks showed that a simple target-history mean outperformed the pooled weather model. This motivates stronger temporal baselines and a controlled test of weather's incremental value. The daily delay endpoint is separate from the activity-stress proxy.

**Next:** reserve untouched evaluation periods; compare calendar/history and weather baselines on identical cases; report error in the endpoint's units, paired uncertainty, interval width and coverage, and error versus retained fraction under abstention. Event studies must meet independent date/pair support requirements before model fitting.

## Sparse room-impulse-response fault evaluation

**Question:** which acoustic residuals remain useful for detecting changes when recording conditions differ between training and testing?

The prototype simulates six shoebox rooms with paired nominal/fault responses and waveform-derived residual features. A fixed random forest is evaluated with each room held out together. Saved classifier inputs reproduced these four-class balanced accuracies:

| Training → test | One response pair | Three response pairs |
|---|---:|---:|
| Clean → clean | 97.2% | 95.8% |
| Matched noisy → noisy | 74.1% | 79.2% |
| Clean → noisy | 35.6% | 27.8% |

Chance is 25%. The clean-to-noisy failure motivates the next work. These are exploratory synthetic results across six rooms; full scene regeneration and measured-room evaluation were not performed in the October audit.

**Next:** increase independent room support, test nuisance controls and localized/multiple changes, and evaluate measured responses. Attribution and publication permissions for the local release candidate remain to be resolved.

## Cross-environment RF sensing

The implementation includes Wi-Fi CSI activity-classification pipelines with CNN, history-token transformer, temporal-attention and domain-adversarial variants. A separate mmWave pipeline uses skeleton-derived azimuth-sector labels.

The current work is reconciling report tables with raw run settings and auditing label consistency, split independence and profiling. Numerical performance comparisons will be revised after the run lineage and controlled evaluation are established. Explanations for domain-adversarial degradation remain hypotheses to test.

**Next:** freeze user/session splits and a global class map; save exact sample identities, per-seed predictions and code/configuration hashes; compare variants within the same transfer direction and training budget; profile with explicit device, batch, warm-up and synchronization settings.

## Quiet Cruise: spatial audio interaction

The local prototype combines authored cabin scenes, measured-HRTF rendering, controlled listening positions, and a duplicated-mono reference. Automated behavior checks and recorded tracking diagnostics are separate evidence streams.

Deterministic motion, bridge-authorization and tracking-geometry checks passed in the local audit. Saved sensor-session diagnostics examine delivery continuity, with timing observations kept separate from physical accuracy. Perceptual anchoring and hardware motion-to-sound latency require their own evaluation.

**Next:** resolve packaging and dependency attribution, improve delivery continuity, then evaluate perceptual outcomes with a defined study protocol.

## Mathematical reasoning and context retention — in progress

**Judge/verifier evaluation:** design paired mathematical-reasoning cases that hold the problem fixed while varying validity and presentation independently. Known-answer checks and disagreement records will make failures inspectable.

**Verifier-guided compaction:** design observable claim/dependency traces to compare full context, generic compaction and dependency-aware retention. The planned outcomes are verifier-checkable correctness, token use, latency and regressions after losing critical constraints or intermediate dependencies.

These entries describe study designs in progress. Completed benchmark results or measured compaction gains are not claimed.

## Public implementation evidence

[AirBorder](https://github.com/MayFairMI6/AirBorder) provides a Swift/iPhone layover and airport-transfer implementation with uncertain time estimates, seeded feasibility simulation, provenance and abstention for unresolved inputs. Its [verification note](https://github.com/MayFairMI6/AirBorder/blob/main/Documentation/Verification-2026-10-11.md) distinguishes passing Worker/unit checks from remaining UI and field-validation work.

The profile also links systems and team-contribution examples. Repository history and documented roles support contribution claims; simulation results, software checks, field outcomes and publication status remain separate.
