# About this repository
This repository collects papers on security for Vision-Language-Action (VLA) models. Papers are grouped by attack type, with links to PDFs for quick access.

![Attack categories](category.png)

## Overview and Contents
1. [Backdoor/Poisoning](#backdoorpoisoning) — Hidden triggers or poisoned data cause targeted misbehavior under specific conditions.
2. [Patch Attacks](#patch-attacks) — Physical or digital patches steer perception and downstream actions.
3. [Adversarial Attacks](#adversarial-attacks) — Crafted inputs or prompts induce failures without changing model weights.
4. [Action Manipulation](#action-manipulation) — Attacks disrupt action outputs (e.g., freezing or drifting actions).
5. [Robustness/Sensor Attacks](#robustnesssensor-attacks) — Physical or sensor-level variations stress the perception-action pipeline.
6. [Defense](#defense) — Methods that improve robustness through training, filtering, or detection.
7. [Benchmarks](#benchmarks) — Datasets and evaluation suites for VLA security and robustness.

## Backdoor/Poisoning
| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| State Backdoor: Towards Stealthy Real-world Poisoning Attack on Vision-Language-Action Model in State Space | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2601.04266.pdf) |
| BadVLA: Towards Backdoor Attacks on Vision-Language-Action Models via Objective-Decoupled Optimization | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2505.16640.pdf) |
| Goal-oriented Backdoor Attack against Vision-Language-Action Models via Physical Objects | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2510.09269.pdf) |
| TrojanRobot: Physical-world Backdoor Attacks Against VLM-based Robotic Manipulation | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2411.11683.pdf) |

## Patch Attacks
| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| When Robots Obey the Patch: Universal Transferable Patch Attacks on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.21192.pdf) |
| Attention-Guided Patch-Wise Sparse Adversarial Attacks on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.21663.pdf) |

## Adversarial Attacks
| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| ANNIE: Be Careful of Your Robots | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2509.03383.pdf) |
| Exploring the Adversarial Vulnerabilities of Vision-Language-Action Models in Robotics | 2025 | ICCV | [PDF](https://openaccess.thecvf.com/content/ICCV2025/papers/Wang_Exploring_the_Adversarial_Vulnerabilities_of_Vision-Language-Action_Models_in_Robotics_ICCV_2025_paper.pdf) |
| When Alignment Fails: Multimodal Adversarial Attacks on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.16203.pdf) |

## Action Manipulation
| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| FreezeVLA: Action-Freezing Attacks against Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2509.19870.pdf) |

## Robustness/Sensor Attacks
| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| Eva-VLA: Evaluating Vision-Language-Action Models' Robustness Under Real-World Physical Variations | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2509.18953.pdf) |
| Phantom Menace: Exploring and Enhancing the Robustness of VLA Models Against Physical Sensor Attacks | 2025 | arXiv preprint (AAAI 2026) | [PDF](https://arxiv.org/pdf/2511.10008.pdf) |
| Exploring the Robustness of Vision-Language-Action Models against Sensor Attacks | 2025 | LAMPS '25 (workshop) | [PDF](https://www.zjushine.top/lamps-vla-robustness.github.io/static/pdfs/LAMPS2025_VLA_Robustness.pdf) |


## Benchmarks
| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| AttackVLA: Benchmarking Adversarial and Backdoor Attacks on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.12149.pdf) |


## Defense
| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| Model-Agnostic Adversarial Attack and Defense for Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2510.13237.pdf) |
| Double Visual Defense: Adversarial Pre-training and Instruction Tuning for Improving Vision-Language Model Robustness | 2025 | arXiv preprint (VLM robustness) | [PDF](https://arxiv.org/pdf/2501.09446.pdf) |
| Attack as Defense: Safeguarding Large Vision-Language Models from Jailbreaking by Adversarial Attacks | 2025 | EMNLP Findings (VLM defense) | [PDF](https://aclanthology.org/2025.findings-emnlp.1095.pdf) |
