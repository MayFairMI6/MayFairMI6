# Aravinda V.

I’m a Computer Science undergraduate at the University of South Florida. My research interests include mathematical reasoning and verifier robustness, adversarial evaluation of learned representations, and generalization across environments. My current projects examine cross-airport transfer, room-impulse-response simulation, spatial audio interaction, and decision-support systems.

## Selected public work

- **[Cryo-EM model-building benchmark](https://github.com/MayFairMI6/mica-2026-cryoem-benchmark)** — benchmark of MICA against ModelAngelo, EModelX(+AF), CryoAtom and EMProt on 24 cryo-EM maps first released in 2026. Case selection was fixed before any method ran; all 120 primary runs were scored with complex TM-score, Cα quality and sequence-match metrics and paired case-bootstrap intervals. Code, run records and the [Zenodo dataset](https://doi.org/10.5281/zenodo.23581358) are public.
- **[AirBorder](https://github.com/MayFairMI6/AirBorder)** — Swift/iOS layover and airport-transfer prototype combining seeded Monte Carlo estimates, route selection, source freshness checks, and a Cloudflare Worker proxy.
- **[SkyBridge](https://github.com/MayFairMI6/skybridge-network-recovery-optimizer)** — synthetic airline-recovery simulation with a Jenkins–Docker–Terraform deployment pipeline. Recovery policies use authored cost and disruption assumptions; a separate script provides a starting point for fitting a cancellation model.
- **[Flask DevOps Lab](https://github.com/MayFairMI6/flask-devops-lab)** — a small HTTP service and container-packaging exercise, with version and runtime diagnostics.

## Research studies and prototypes

I’m studying how models behave when the evaluation setting changes—and which evidence is needed before their outputs can support a decision. My [research overview](docs/research-overview.md) summarizes the questions, implemented methods, reproduced results, and next experiments.

- **Cross-airport transfer:** activity-stress forecasting under temporal and regional shift, with separate observed-delay adaptation experiments at Shanghai airports.
- **Sparse-RIR fault evaluation:** room-held-out simulation examining how pose, material and geometry changes interact with recording uncertainty.
- **Cross-environment RF sensing:** Wi-Fi CSI activity classification and a separate mmWave azimuth-sector pipeline, with temporal-context and domain-adversarial experiments under methodological review.
- **Quiet Cruise:** spatial-audio interaction with authored scenes, measured-HRTF rendering, and local tracking diagnostics. Perceptual evaluation remains in progress.
- **Math-reasoning judges and verifiers — in progress:** paired cases designed to distinguish logical correctness from explanation length and presentation.
- **Verifier-guided context compaction — in progress:** dependency-aware context retention for mathematical reasoning, with explicit claims, corrections and verifier outcomes.

Research code and data for these studies remain local or private while reproducibility, attribution and release permissions are resolved. The public projects above provide implementation examples that can be inspected now.
