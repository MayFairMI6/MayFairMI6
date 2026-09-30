# Aravinda V.

I’m a Computer Science undergraduate at the University of South Florida. My research interests include mathematical reasoning and verifier robustness, adversarial evaluation of learned representations, and generalization across environments. My current projects examine cross-airport transfer, room-impulse-response measurements, spatial audio interaction, and decision-support systems.

## Selected public work

- **[AirBorder](https://github.com/MayFairMI6/AirBorder)** — Swift/iOS layover and airport-transfer prototype combining seeded Monte Carlo estimates, route selection, source freshness checks, and a Cloudflare Worker proxy.
- **[SkyBridge](https://github.com/MayFairMI6/skybridge-network-recovery-optimizer)** — synthetic airline-recovery simulation with a Jenkins–Docker–Terraform deployment pipeline. Recovery policies use authored cost and disruption assumptions; a separate script provides a starting point for fitting a cancellation model.
- **[SpendSwift](https://github.com/MayFairMI6/tp)** — team Java budgeting project with a currency-conversion extension repaired in this personal fork. My [original contribution record](https://github.com/MayFairMI6/tp/blob/master/docs/team/ppp-2.md) covers budget management, category views, tests, and design documentation; the README distinguishes the later repair from the course submission.
- **[Flask DevOps Lab](https://github.com/MayFairMI6/flask-devops-lab)** — a small HTTP service and container-packaging exercise, with version and runtime diagnostics.

## Current local work

These projects have been developed locally and are not currently published here:

- **Sparse room-impulse-response evaluation:** a six-room synthetic study comparing clean, noisy, and clean-to-noisy transfer with rooms held out together. The observed transfer failure motivates better treatment of measurement uncertainty.
- **Cross-airport transfer:** temporally separated model evaluation and evidence checks for transfer across airports. Data-access boundaries and a separate backend dependency need attention before a public release.
- **Quiet Cruise:** a spatial-audio interaction prototype with synthetic scenes, direct-sound HRTF playback, and a virtual cabin. Physical tracking and perceptual evaluation remain open.

I’m preparing a mathematical-verifier study that tests sensitivity to localized errors in reasoning traces while tracking final-answer correctness separately. I’m also interested in post-embedding evaluation: how perturbations to learned representations affect downstream decisions.
