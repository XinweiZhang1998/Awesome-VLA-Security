# Awesome VLA Security

This repository collects papers on security and safety for Vision-Language-Action (VLA) models, World Action Models (WAMs), and related embodied systems, including surveys, attacks, privacy, defenses, and evaluation benchmarks. Papers are grouped by topic, with links to original PDFs where available.

**Last literature search: September 10, 2026.** This update includes September 2026 releases and revisions, with expanded coverage of reasoning attacks, instruction robustness, embodied safety evaluation, and world-action/world-model security. Coverage is selective rather than exhaustive.

**If you’re interested in VLA security, feel free to email xwzhang1998@gmail.com to connect and explore potential collaborations**.

![Attack categories](category.png)

## Overview and Contents

1. [Surveys](#surveys)
2. [Backdoor/Poisoning](#backdoorpoisoning)
3. [Patch Attacks](#patch-attacks)
4. [Reasoning and Instruction Attacks](#reasoning-and-instruction-attacks)
5. [Adversarial Attacks](#adversarial-attacks)
6. [Weight Integrity Attacks](#weight-integrity-attacks)
7. [Privacy Attacks](#privacy-attacks)
8. [Robustness/Sensor Attacks](#robustnesssensor-attacks)
9. [Benchmarks](#benchmarks)
10. [Defenses](#defenses)
11. [World Action Models and World Models](#world-action-models-and-world-models): [attacks](#wam-attacks-and-security-evaluation), [safety](#world-model-safety-and-risk-analysis), [surveys and models](#wam-surveys-and-representative-models)
12. [Embodied-Agent Security and Safety](#embodied-agent-security-and-safety): [jailbreaks](#embodied-jailbreaks), [benchmarks](#embodied-safety-benchmarks)
13. [VLM](#vlm)

For arXiv-linked papers, **Year** records the first arXiv submission year; the venue column can refer to a later publication.

Venue labels marked **\*** are acceptance statements in the authors' arXiv metadata, rather than independently checked proceedings records. The surveys explicitly labeled as broader embodied AI cover systems beyond end-to-end VLA policies. Failure detection and collision avoidance are included as safety methods; their inclusion does not imply demonstrated resistance to adversarial attacks.

## Surveys

| Title | Year | Venue/Type | PDF / Paper |
| --- | --- | --- | --- |
| Vision-Language-Action Safety: Threats, Challenges, Evaluations, and Mechanisms | 2026 | arXiv survey; VLA safety | [PDF](https://arxiv.org/pdf/2604.23775) |
| Safety of Vision-Language-Action Models: A Survey from Lifecycle Perspectives | 2026 | Authorea preprint; VLA safety | [Paper](https://www.authorea.com/doi/full/10.22541/au.177524426.60806944/v1) |
| SoK: Security and Privacy of Foundation-Model-Powered Robots | 2026 | arXiv SoK; broader embodied AI | [PDF](https://arxiv.org/pdf/2606.16788) |
| Embodied Intelligence Security with Vision-language Models: A Survey | 2026 | Machine Intelligence Research; broader embodied AI | [PDF](https://link.springer.com/content/pdf/10.1007/s11633-025-1626-x.pdf) |
| Towards Robust and Secure Embodied AI: A Survey on Vulnerabilities and Attacks | 2025 | ACM Computing Surveys 2026; broader embodied AI; preprint PDF | [PDF](https://arxiv.org/pdf/2502.13175) |

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
| Clean-Action Backdoor Attacks on Vision-Language-Action Models via Sequential Error Exploitation | 2025 | OpenReview manuscript; acceptance not verified | [PDF](https://openreview.net/pdf?id=QQdn8nNqgi) |
| DropVLA: An Action-Level Backdoor Attack on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2510.10932) |
| BadVLA: Towards Backdoor Attacks on Vision-Language-Action Models via Objective-Decoupled Optimization | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2505.16640.pdf) |
| Goal-oriented Backdoor Attack against Vision-Language-Action Models via Physical Objects | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2510.09269.pdf) |
| Robot Collapse: Supply Chain Backdoor Attacks Against VLM-based Robotic Manipulation | 2024 | arXiv preprint; TrojanRobot framework | [PDF](https://arxiv.org/pdf/2411.11683.pdf) |

## Patch Attacks

See also [TRAP and reasoning attacks](#reasoning-and-instruction-attacks) and [WAM attacks](#wam-attacks-and-security-evaluation).

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| Partially Observable Adversarial Patch Attacks on Vision-Language-Action Models in Robotics | 2026 | IEEE Robotics and Automation Letters 2026* | [PDF](https://arxiv.org/pdf/2606.03556) |
| UniTexture: Cross-Task Universal Adversarial Textures for Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2608.13453) |
| VLA-Hijack: A Transferable Patch Attack against Vision-Language-Action Models via Visual Proprioception Hijacking | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2605.28083) |
| Tex3D: Objects as Attack Surfaces via Adversarial 3D Textures for Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2604.01618) |
| When Robots Obey the Patch: Universal Transferable Patch Attacks on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.21192.pdf) |
| Attention-Guided Patch-Wise Sparse Adversarial Attacks on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.21663.pdf) |
| Exploring the Adversarial Vulnerabilities of Vision-Language-Action Models in Robotics | 2025 | ICCV | [PDF](https://openaccess.thecvf.com/content/ICCV2025/papers/Wang_Exploring_the_Adversarial_Vulnerabilities_of_Vision-Language-Action_Models_in_Robotics_ICCV_2025_paper.pdf) |
| When Alignment Fails: Multimodal Adversarial Attacks on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.16203.pdf) |
| Model-Agnostic Adversarial Attack and Defense for Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2510.13237.pdf) |

## Reasoning and Instruction Attacks

Attacks and robustness studies on intermediate reasoning, language grounding, and the reasoning-to-action pathway. TRAP uses an adversarial visual patch; it is distinct from the backdoor method TrapVLA.

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| TRAP: Hijacking VLA CoT-Reasoning via Adversarial Patches | 2026 | ICML 2026* | [PDF](https://arxiv.org/pdf/2603.23117) |
| Reasoning as a Double-Edged Sword: Architecture and Cross-Stage Robustness in Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2607.17786) |
| ReasonBreak: Probing Vulnerabilities in Reasoning-Enabled Vision-Language-Action Models for Autonomous Driving | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2605.29114) |
| SABER: A Stealthy Agentic Black-Box Attack Framework for Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2603.24935) |
| Altered Thoughts, Altered Actions: Probing Chain-of-Thought Vulnerabilities in VLA Robotic Manipulation | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2603.12717) |
| Red-Teaming Vision-Language-Action Models via Quality Diversity Prompt Generation for Robust Robot Policies | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2603.12510) |

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
| How VLAs (Really) Work In Open-World Environments | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2604.21192) |
| ICR-Drive: Instruction Counterfactual Robustness for End-to-End Language-Driven Autonomous Driving | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2604.05378) |
| Bring the Apple, Not the Sofa: Impact of Irrelevant Context in Embodied AI Commands on VLA Models | 2026 | EACL 2026 Student Research Workshop | [PDF](https://aclanthology.org/2026.eacl-srw.63.pdf) |
| Confidence Calibration in Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2507.17383) |
| Evaluating Uncertainty and Quality of Vision-Language-Action-enabled Robots | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2507.17049) |
| Eva-VLA: Evaluating Vision-Language-Action Models' Robustness Under Real-World Physical Variations | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2509.18953.pdf) |
| Phantom Menace: Exploring and Enhancing the Robustness of VLA Models Against Physical Sensor Attacks | 2025 | AAAI 2026* | [PDF](https://arxiv.org/pdf/2511.10008.pdf) |
| Exploring the Robustness of Vision-Language-Action Models against Sensor Attacks | 2025 | LAMPS '25 (workshop) | [PDF](https://www.zjushine.top/lamps-vla-robustness.github.io/static/pdfs/LAMPS2025_VLA_Robustness.pdf) |

## Benchmarks

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| ForesightSafety-VLA: A Unified Diagnostic Safety Benchmark for Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2606.27079) |
| LIBERO-Safety: A Comprehensive Benchmark for Physical and Semantic Safety in Vision-Language-Action Models | 2026 | ECCV 2026* | [PDF](https://arxiv.org/pdf/2606.23686) |
| HazardArena: Evaluating Semantic Safety in Vision-Language-Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2604.12447) |
| VLA-Arena: An Open-Source Framework for Benchmarking Vision-Language-Action Models | 2025 | ICML 2026* | [PDF](https://arxiv.org/pdf/2512.22539) |
| LIBERO-Plus: In-depth Robustness Analysis of Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2510.13626) |
| LIBERO-PRO: Towards Robust and Fair Evaluation of Vision-Language-Action Models Beyond Memorization | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2510.03827) |
| AttackVLA: Benchmarking Adversarial and Backdoor Attacks on Vision-Language-Action Models | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.12149.pdf) |
| VLATest: Testing and Evaluating Vision-Language-Action Models for Robotic Manipulation | 2024 | FSE 2025* | [PDF](https://arxiv.org/pdf/2409.12894) |

## Defenses

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| VLAGuard: A Framework for Evaluating and Mitigating Physical Attention Hijacking in Vision-Language-Action Robots within Wireless Sensor Networks | 2026 | Ad Hoc & Sensor Wireless Networks* | [PDF](https://arxiv.org/pdf/2608.01028) |
| VLA-Forget: Vision-Language-Action Unlearning for Embodied Foundation Models | 2026 | ACL 2026 KnowFM workshop* | [PDF](https://arxiv.org/pdf/2604.03956) |
| Causal Scene Narration with Runtime Safety Supervision for Vision-Language-Action Driving | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2604.01723) |
| RC-NF: Robot-Conditioned Normalizing Flow for Real-Time Anomaly Detection in Robotic Manipulation | 2026 | CVPR 2026* | [PDF](https://arxiv.org/pdf/2603.11106) |
| Restoring Linguistic Grounding in VLA Models via Train-Free Attention Recalibration | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2603.06001) |
| Safe-Night VLA: Seeing the Unseen via Thermal-Perceptive Vision-Language-Action Models for Safety-Critical Manipulation | 2026 | IROS 2026* | [PDF](https://arxiv.org/pdf/2603.05754) |
| CompliantVLA-adaptor: VLM-Guided Variable Impedance Action for Safe Contact-Rich Manipulation | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2601.15541) |
| FailureSpot: Label-Efficient Timestamp-Level Failure Detection for Vision-Language-Action Models | 2026 | arXiv preprint; September 3, 2026 | [PDF](https://arxiv.org/pdf/2609.04277) |
| Structure-Aware Robust Fine-Tuning: Defending Vision-Language-Action Robots Against Physical Attention Hijacking | 2026 | IROS 2026* | [PDF](https://arxiv.org/pdf/2608.03231) |
| Neuro-Symbolic Safety Guidance for Vision-Language-Action Models via Constrained Flow Matching | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2607.01378) |
| Hide-and-Seek in Trajectories: Discovering Failure Signals for VLA Runtime Monitoring | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2605.30834) |
| Concept-Based Dictionary Learning for Inference-Time Safety in Vision Language Action Models | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2602.01834) |
| Affordance Field Intervention: Enabling VLAs to Escape Memory Traps in Robotic Manipulation | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2512.07472) |
| FailSafe: Reasoning and Recovery from Failures in Vision-Language-Action Models | 2025 | IROS 2026* | [PDF](https://arxiv.org/pdf/2510.01642) |
| VLSA: Vision-Language-Action Models with Plug-and-Play Safety Constraint Layer | 2025 | IROS 2026* | [PDF](https://arxiv.org/pdf/2512.11891) |
| SAFE: Multitask Failure Detection for Vision-Language-Action Models | 2025 | NeurIPS 2025* | [PDF](https://arxiv.org/pdf/2506.09937) |
| SafeVLA: Towards Safety Alignment of Vision-Language-Action Model via Constrained Learning | 2025 | NeurIPS 2025 | [PDF](https://proceedings.neurips.cc/paper_files/paper/2025/file/e185c7be603426028c32ae1003a59d78-Paper-Conference.pdf) |
| Run-time Observation Interventions Make Vision-Language-Action Models More Visually Robust | 2024 | arXiv preprint | [PDF](https://arxiv.org/pdf/2410.01971) |

## World Action Models and World Models

This section covers predictive models used for action generation, planning, or robot training. **WAM-specific** work studies models that couple predicted futures to actions; **world-model** work also includes Dreamer-style agents and learned simulators in robot-learning pipelines. Results for these systems should be interpreted within their respective threat models and evaluation settings.

### WAM Attacks and Security Evaluation

| Title | Year | Venue/Type | Scope / Focus | PDF |
| --- | --- | --- | --- | --- |
| BadWAM: When World-Action Models Dream Right but Act Wrong | 2026 | arXiv preprint | WAM; adversarial world-action drift and imagination-preserving attacks | [PDF](https://arxiv.org/pdf/2607.15207) |
| Attacking the Trusted Imagination: Oracle-Level Integrity Attacks on Imagine-then-Act World Models | 2026 | arXiv preprint | WAM; integrity of predicted futures consumed by planners and safety checks | [PDF](https://arxiv.org/pdf/2606.22966) |
| ARB4WM: An Adversarial Robustness Benchmark for World Models in Continuous Control | 2026 | arXiv preprint | World models; adversarial benchmark for Dreamer-style control agents | [PDF](https://arxiv.org/pdf/2606.16605) |
| Targeting World Models to Compromise Robot Learning Pipelines | 2026 | arXiv preprint | Robot-learning supply chain; world-model-mediated poisoning; VLA proof of concept | [PDF](https://arxiv.org/pdf/2606.09499) |
| JailWAM: Jailbreaking World Action Models in Robot Control | 2026 | arXiv preprint | WAM; jailbreak attacks and JailWAM-Bench | [PDF](https://arxiv.org/pdf/2604.05498) |

### World Model Safety and Risk Analysis

Safe planning methods and risk analyses for learned world models. Safe-RL results do not by themselves establish robustness against deliberate attacks on WAMs.

| Title | Year | Venue/Type | Scope / Focus | PDF |
| --- | --- | --- | --- | --- |
| Safety, Security, and Cognitive Risks in World Models | 2026 | arXiv preprint | Risk survey and proof-of-concept attacks on RSSM/Dreamer models | [PDF](https://arxiv.org/pdf/2604.01346) |
| Nightmare Dreamer: Dreaming About Unsafe States And Planning Ahead | 2026 | arXiv preprint | Safe model-based RL; anticipating unsafe states | [PDF](https://arxiv.org/pdf/2601.04686) |
| SafeDreamer: Safe Reinforcement Learning with World Models | 2023 | ICLR 2024* | Safe model-based RL; safety-constrained world-model planning | [PDF](https://arxiv.org/pdf/2307.07176) |

### WAM Surveys and Representative Models

Background references for understanding model architectures and potential evaluation targets. Inclusion here is not a claim that a model is secure or that it has been attacked in the papers above.

| Title | Year | Venue/Type | Scope / Focus | PDF |
| --- | --- | --- | --- | --- |
| World Action Models: A Survey | 2026 | arXiv preprint | Survey; WAM definitions, taxonomy, and action coupling | [PDF](https://arxiv.org/pdf/2606.20781) |
| World Model for Robot Learning: A Comprehensive Survey | 2026 | arXiv preprint | Survey; world models for robot learning, planning, and evaluation | [PDF](https://arxiv.org/pdf/2605.00080) |
| Native Video-Action Pretraining for Generalizable Robot Control | 2026 | arXiv preprint | LingBot-VA 2.0; native video-action pretraining | [PDF](https://arxiv.org/pdf/2607.08639) |
| World Action Models are Zero-shot Policies | 2026 | arXiv preprint | DreamZero; joint video-action modeling and generalization | [PDF](https://arxiv.org/pdf/2602.15922) |
| Causal World Modeling for Robot Control | 2026 | arXiv preprint | LingBot-VA; causal video-action modeling | [PDF](https://arxiv.org/pdf/2601.21998) |
| WorldVLA: Towards Autoregressive Action World Model | 2025 | arXiv preprint | WorldVLA; autoregressive action and world modeling | [PDF](https://arxiv.org/pdf/2506.21539) |

## Embodied-Agent Security and Safety

Related LLM/VLM-based robot and embodied-agent work. These entries cover planners and agent pipelines, which may differ from end-to-end VLA policies.

### Embodied Jailbreaks

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| The Shawshank Redemption of Embodied AI: Understanding and Benchmarking Indirect Environmental Jailbreaks | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2511.16347) |
| Jailbreaking LLM-Controlled Robots | 2024 | arXiv preprint | [PDF](https://arxiv.org/pdf/2410.13691) |
| BadRobot: Jailbreaking Embodied LLM Agents in the Physical World | 2024 | ICLR 2025* | [PDF](https://arxiv.org/pdf/2407.20242) |

### Embodied Safety Benchmarks

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| RoboJailBench: Benchmarking Adversarial Attacks and Defenses in Embodied Robotic Agents | 2026 | arXiv preprint | [PDF](https://arxiv.org/pdf/2605.19328) |
| AGENTSAFE: Benchmarking the Safety of Embodied Agents on Hazardous Instructions | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2506.14697) |
| Generating Robot Constitutions & Benchmarks for Semantic Safety | 2025 | arXiv preprint | [PDF](https://arxiv.org/pdf/2503.08663) |
| SafeAgentBench: A Benchmark for Safe Task Planning of Embodied LLM Agents | 2024 | arXiv preprint | [PDF](https://arxiv.org/pdf/2412.13178) |

## VLM

Related work on VLM robustness and VLM-based embodied agents; these papers are not all direct evaluations of end-to-end VLA policies.

| Title | Year | Venue/Type | PDF |
| --- | --- | --- | --- |
| Double Visual Defense: Adversarial Pre-training and Instruction Tuning for Improving Vision-Language Model Robustness | 2025 | arXiv preprint (VLM robustness) | [PDF](https://arxiv.org/pdf/2501.09446.pdf) |
| Attack as Defense: Safeguarding Large Vision-Language Models from Jailbreaking by Adversarial Attacks | 2025 | EMNLP Findings (VLM defense) | [PDF](https://aclanthology.org/2025.findings-emnlp.1095.pdf) |
| ADVEDM: Fine-grained Adversarial Attack against VLM-based Embodied Agents | 2025 | NeurIPS | [PDF](https://arxiv.org/pdf/2509.16645.pdf) |
