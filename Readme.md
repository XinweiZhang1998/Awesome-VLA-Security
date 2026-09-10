# Awesome VLA Security

This repository collects papers on security and safety for Vision-Language-Action (VLA) models, including surveys, attacks, privacy, defenses, and evaluation benchmarks. Papers are grouped by topic, with links to original PDFs where available.

**Last literature search: September 10, 2026.** This update includes September 2026 releases and revisions, alongside earlier relevant work missing from the list. Coverage is selective rather than exhaustive.

**If you’re interested in VLA security, feel free to email xwzhang1998@gmail.com to connect and explore potential collaborations**.

![Attack categories](category.png)

## Overview and Contents

1. [Surveys](#surveys) — VLA safety reviews and related embodied AI security surveys.
2. [Backdoor/Poisoning](#backdoorpoisoning) — Hidden triggers or poisoned data cause targeted misbehavior.
3. [Patch Attacks](#patch-attacks) — Physical or digital patches and object textures steer actions.
4. [Adversarial Attacks](#adversarial-attacks) — Crafted inputs or prompts induce failures without changing model weights.
5. [Weight Integrity Attacks](#weight-integrity-attacks) — Faults or malicious changes to deployed model weights.
6. [Privacy Attacks](#privacy-attacks) — Inference of training-data membership from VLA behavior or representations.
7. [Robustness/Sensor Attacks](#robustnesssensor-attacks) — Sensor variations and instruction context stress the perception-action pipeline.
8. [Benchmarks](#benchmarks) — Evaluation suites for VLA security and physical or semantic safety.
9. [Defenses](#defenses) — Robust training, safety constraints, and runtime failure detection.
10. [VLM](#vlm) — Related VLM and embodied-agent security research.

Venue labels marked **\*** are acceptance statements in the authors' arXiv metadata, rather than independently checked proceedings records. The surveys explicitly labeled as broader embodied AI cover systems beyond end-to-end VLA policies. Failure detection and collision avoidance are included as safety methods; their inclusion does not imply demonstrated resistance to adversarial attacks.

## Surveys

| Title | Year | Venue/Type | PDF / Paper |
| --- | --- | --- | --- |
| Vision-Language-Action Safety: Threats, Challenges, Evaluations, and Mechanisms | 2026 | arXiv survey; VLA safety | [PDF](https://arxiv.org/pdf/2604.23775) |
| Safety of Vision-Language-Action Models: A Survey from Lifecycle Perspectives | 2026 | Authorea preprint; VLA safety | [Paper](https://www.authorea.com/doi/full/10.22541/au.177524426.60806944/v1) |
| SoK: Security and Privacy of Foundation-Model-Powered Robots | 2026 | arXiv SoK; broader embodied AI | [PDF](https://arxiv.org/pdf/2606.16788) |
| Embodied Intelligence Security with Vision-language Models: A Survey | 2026 | Machine Intelligence Research; broader embodied AI | [PDF](https://link.springer.com/content/pdf/10.1007/s11633-025-1626-x.pdf) |
| Towards Robust and Secure Embodied AI: A Survey on Vulnerabilities and Attacks | 2026 | ACM Computing Surveys; broader embodied AI; preprint PDF | [PDF](https://arxiv.org/pdf/2502.13175) |

## Backdoor/Poisoning

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| TrapVLA: Trapping Vision-Language-Action Models in Configured Failure Modes | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2608.26578) |
| !Imperio, smolVLA: The Implications of Data Poisoning on Open Source Robotics | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2607.04146) |
| ATAAT: Adaptive Threat-Aware Adversarial Tuning Framework against Backdoor Attacks on Vision-Language-Action Models | 2026 | Findings of ACL 2026 | [PDF](https://aclanthology.org/2026.findings-acl.1077.pdf) |
| FlowHijack: A Dynamics-Aware Backdoor Attack on Flow-Matching Vision-Language-Action Models | 2026 | CVPR 2026 | [PDF](https://openaccess.thecvf.com/content/CVPR2026/papers/An_FlowHijack_A_Dynamics-Aware_Backdoor_Attack_on_Flow-Matching_Vision-Language-Action_Models_CVPR_2026_paper.pdf) |
| Inject Once Survive Later: Backdooring Vision-Language-Action Models to Persist Through Downstream Fine-tuning | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2602.00500) |
| SilentDrift: Exploiting Action Chunking for Stealthy Backdoor Attacks on Vision-Language-Action Models | 2026 | Findings of ACL 2026* | [PDF](https://arxiv.org/pdf/2601.14323) |
| State Backdoor: Towards Stealthy Real-world Poisoning Attack on Vision-Language-Action Model in State Space | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2601.04266.pdf) |
| DropVLA: An Action-Level Backdoor Attack on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2510.10932) |
| BadVLA: Towards Backdoor Attacks on Vision-Language-Action Models via Objective-Decoupled Optimization | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2505.16640.pdf) |
| Goal-oriented Backdoor Attack against Vision-Language-Action Models via Physical Objects | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2510.09269.pdf) |
| TrojanRobot: Physical-world Backdoor Attacks Against VLM-based Robotic Manipulation | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2411.11683.pdf) |


## Patch Attacks

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| UniTexture: Cross-Task Universal Adversarial Textures for Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2608.13453) |
| VLA-Hijack: A Transferable Patch Attack against Vision-Language-Action Models via Visual Proprioception Hijacking | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2605.28083) |
| Tex3D: Objects as Attack Surfaces via Adversarial 3D Textures for Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2604.01618) |
| When Robots Obey the Patch: Universal Transferable Patch Attacks on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.21192.pdf) |
| Attention-Guided Patch-Wise Sparse Adversarial Attacks on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.21663.pdf) |
| Exploring the Adversarial Vulnerabilities of Vision-Language-Action Models in Robotics | 2025 | ICCV | [PDF](https://openaccess.thecvf.com/content/ICCV2025/papers/Wang_Exploring_the_Adversarial_Vulnerabilities_of_Vision-Language-Action_Models_in_Robotics_ICCV_2025_paper.pdf) |
| When Alignment Fails: Multimodal Adversarial Attacks on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.16203.pdf) |
| Model-Agnostic Adversarial Attack and Defense for Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2510.13237.pdf) |

## Adversarial Attacks

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| Trajectory-Level Redirection Attacks on Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2606.12978) |
| Adversarial Attacks on Robotic Vision Language Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2506.03350) |
| ANNIE: Be Careful of Your Robots | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2509.03383.pdf) |
| FreezeVLA: Action-Freezing Attacks against Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2509.19870.pdf) |

## Weight Integrity Attacks

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| Bit-Flip Attacks on Vision-Language-Action Models: Action-Decoding Architecture Shapes the Vulnerability | 2026 | arXiv preprint; revised September 9, 2026 | [PDF](https://arxiv.org/pdf/2608.15475) |

## Privacy Attacks

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| VLALeaks: Membership Inference Attacks against Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2606.15165) |
| Membership Inference Attacks on Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2605.07088) |

## Robustness/Sensor Attacks

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| Bring the Apple, Not the Sofa: Impact of Irrelevant Context in Embodied AI Commands on VLA Models | 2026 | EACL 2026 Student Research Workshop | [PDF](https://aclanthology.org/2026.eacl-srw.63.pdf) |
| Eva-VLA: Evaluating Vision-Language-Action Models' Robustness Under Real-World Physical Variations | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2509.18953.pdf) |
| Phantom Menace: Exploring and Enhancing the Robustness of VLA Models Against Physical Sensor Attacks | 2026 | AAAI 2026 | [PDF](https://arxiv.org/pdf/2511.10008.pdf) |
| Exploring the Robustness of Vision-Language-Action Models against Sensor Attacks | 2025 | LAMPS '25 (workshop) | [PDF](https://www.zjushine.top/lamps-vla-robustness.github.io/static/pdfs/LAMPS2025_VLA_Robustness.pdf) |


## Benchmarks

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| ForesightSafety-VLA: A Unified Diagnostic Safety Benchmark for Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2606.27079) |
| LIBERO-Safety: A Comprehensive Benchmark for Physical and Semantic Safety in Vision-Language-Action Models | 2026 | ECCV 2026* | [PDF](https://arxiv.org/pdf/2606.23686) |
| HazardArena: Evaluating Semantic Safety in Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2604.12447) |
| AttackVLA: Benchmarking Adversarial and Backdoor Attacks on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.12149.pdf) |

## Defenses

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| FailureSpot: Label-Efficient Timestamp-Level Failure Detection for Vision-Language-Action Models | 2026 | arXiv preprint; September 3, 2026 | [PDF](https://arxiv.org/pdf/2609.04277) |
| Structure-Aware Robust Fine-Tuning: Defending Vision-Language-Action Robots Against Physical Attention Hijacking | 2026 | IROS 2026* | [PDF](https://arxiv.org/pdf/2608.03231) |
| Neuro-Symbolic Safety Guidance for Vision-Language-Action Models via Constrained Flow Matching | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2607.01378) |
| Hide-and-Seek in Trajectories: Discovering Failure Signals for VLA Runtime Monitoring | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2605.30834) |
| Concept-Based Dictionary Learning for Inference-Time Safety in Vision Language Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2602.01834) |
| VLSA: Vision-Language-Action Models with Plug-and-Play Safety Constraint Layer | 2025 | IROS 2026* | [PDF](https://arxiv.org/pdf/2512.11891) |
| SAFE: Multitask Failure Detection for Vision-Language-Action Models | 2025 | NeurIPS 2025* | [PDF](https://arxiv.org/pdf/2506.09937) |
| SafeVLA: Towards Safety Alignment of Vision-Language-Action Model via Constrained Learning | 2025 | NeurIPS 2025 | [PDF](https://proceedings.neurips.cc/paper_files/paper/2025/file/e185c7be603426028c32ae1003a59d78-Paper-Conference.pdf) |

## VLM

Related work on VLM robustness and VLM-based embodied agents; these papers are not all direct evaluations of end-to-end VLA policies.

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| Double Visual Defense: Adversarial Pre-training and Instruction Tuning for Improving Vision-Language Model Robustness | 2025 | arXiv preprint (VLM robustness) | [PDF](https://arxiv.org/pdf/2501.09446.pdf) |
| Attack as Defense: Safeguarding Large Vision-Language Models from Jailbreaking by Adversarial Attacks | 2025 | EMNLP Findings (VLM defense) | [PDF](https://aclanthology.org/2025.findings-emnlp.1095.pdf) |
| ADVEDM: Fine-grained Adversarial Attack against VLM-based Embodied Agents | 2025 | NeurIPS | [PDF](https://arxiv.org/pdf/2509.16645.pdf) |
