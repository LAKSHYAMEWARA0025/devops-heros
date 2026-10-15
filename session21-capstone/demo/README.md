# StockPilot: presentation and video

**Lakshya Mewara** · 24BCS10290 · Session 21 DevOps Final Capstone

| File | What it is |
|---|---|
| [`StockPilot-Capstone-Lakshya-Mewara.mp4`](./StockPilot-Capstone-Lakshya-Mewara.mp4) | Presentation video (MP4, 11 min). It walks through the deck and includes the live demo: a code change committed, the pipeline going green, and the deployment updated with Helm. |
| [`StockPilot-Capstone-Lakshya-Mewara.pptx`](./StockPilot-Capstone-Lakshya-Mewara.pptx) | Slide deck (PowerPoint, 16 slides). Each slide's speaker notes carry the narration. |
| [`StockPilot-Capstone-Lakshya-Mewara.pdf`](./StockPilot-Capstone-Lakshya-Mewara.pdf) | The same deck as a PDF, readable directly on GitHub |

The deck follows the capstone's presentation flow:

| # | Slide | # | Slide |
|---|---|---|---|
| 1 | StockPilot - title | 9 | DevSecOps: a gate that really blocks |
| 2 | What StockPilot does | 10 | Terraform: AWS VPC + EKS in Mumbai |
| 3 | Architecture at a glance | 11 | Kubernetes + Helm |
| 4 | Tech stack | 12 | Autoscaling under real load |
| 5 | Application: API and data | 13 | Observability: Prometheus + Grafana |
| 6 | Testing: the first quality gate | 14 | Troubleshooting lab |
| 7 | Docker: two images, one command | 15 | What I learned |
| 8 | CI/CD: nine jobs on every push | 16 | Thank you + live demo |

Every number on the slides comes from a real run; the evidence is in the [project README](../README.md).

## What the video shows

| Time | What happens |
|---|---|
| 0:00 | Introduction: slides 1–4 |
| 1:48 | The running app at `stockpilot.local`, served by the local Kubernetes cluster through the Ingress |
| 2:10 | The dashboard header is changed from *Main store* to *Mumbai store* in `frontend/src/App.jsx`, then committed and pushed |
| 3:12 | The push starts the nine-job pipeline in GitHub Actions |
| 3:36 | Slides 5–9 while the pipeline runs |
| 6:12 | Pipeline check in GitHub Actions |
| 6:36 | Slides 10–15: Terraform, Kubernetes + Helm, autoscaling, monitoring, troubleshooting, lessons |
| 9:12 | The pipeline is green; `helm upgrade` rolls the cluster to the new commit's images |
| 10:10 | Browser refresh: the header now reads **Mumbai store** |

The commit made during the demo is
[`67c89df`](https://github.com/LAKSHYAMEWARA0025/devops-heros/commit/67c89df43cc9c0bf7315d44e245db8f7c46c47de).
