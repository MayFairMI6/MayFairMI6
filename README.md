# Aravinda V.

I’m a Computer Science undergraduate at the University of South Florida. My research interests include mathematical reasoning and verifier robustness, adversarial evaluation of learned representations, and generalization across environments. My current projects examine cross-airport transfer, room-impulse-response simulation, spatial audio interaction, and decision-support systems.

## Selected public work

- **[AirBorder](https://github.com/MayFairMI6/AirBorder)** — Swift/iOS layover and airport-transfer prototype combining seeded Monte Carlo estimates, route selection, source freshness checks, and a Cloudflare Worker proxy.
- **[SkyBridge](https://github.com/MayFairMI6/skybridge-network-recovery-optimizer)** — synthetic airline-recovery simulation with a Jenkins–Docker–Terraform deployment pipeline. Recovery policies use authored cost and disruption assumptions; a separate script provides a starting point for fitting a cancellation model.
- **[SpendSwift](https://github.com/MayFairMI6/tp)** — team Java budgeting project with a currency-conversion extension repaired in this personal fork. My [original contribution record](https://github.com/MayFairMI6/tp/blob/master/docs/team/ppp-2.md) covers budget management, category views, tests, and design documentation; the README distinguishes the later repair from the course submission.
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
