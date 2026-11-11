# World Models: JEPA paper collection

A curated list of **218 papers** on joint-embedding predictive architectures (JEPA) and the latent world models built on them, together with closely related non-JEPA world models. Each entry links to the paper; where a peer-reviewed version exists, the published venue is linked as well.

## How the list is arranged

Papers are grouped by topic. Within each group they are ordered by arXiv identifier, so older work comes first.

| Group | Papers | What it contains |
|---|---:|---|
| [Surveys and position papers](#surveys-and-position-papers) | 11 | Surveys of world models, JEPA and physical AI, plus position papers. |
| [JEPA foundations](#jepa-foundations) | 37 | The core joint-embedding predictive architectures and their training objectives and theory: I-JEPA, MC-JEPA, IWM, V-JEPA, V-JEPA 2 / 2.1, LeJEPA, EB-JEPA and follow-ups. |
| [Robotics and aerial applications](#robotics-and-aerial-applications) | 28 | World models used on robots, drones, underwater vehicles and in driving, e.g. DINO-WM, SkyJEPA, DroneWAM, AquaJEPA. |
| [Action-conditioned models and planning](#action-conditioned-models-and-planning) | 47 | Models that predict the effect of actions and are used for planning or policy learning: LeWorldModel, PLDM, hierarchical and goal-conditioned planners, VLA models, evaluation and robustness studies. |
| [Latent dynamics, physics structure and theory](#latent-dynamics-physics-structure-and-theory) | 48 | Structured latent dynamics (Hamiltonian, symplectic, Koopman, bilinear, semigroup), probabilistic JEPAs, collapse and identifiability analyses. |
| [3D, spatial and object-centric models](#3d-spatial-and-object-centric-models) | 39 | Point-cloud, depth, LiDAR, 3D-scene, object-centric and graph-structured predictive models. |
| [Related non-JEPA world models](#related-non-jepa-world-models) | 8 | Reconstruction-based or Dreamer-style world models with physical structure, kept for comparison. |

**Columns.** *Paper* links to the arXiv abstract page. *Published* gives the journal or conference version with its DOI or proceedings link, if one was found; an empty cell means the paper is, as far as we know, still a preprint. "(accepted)" marks papers accepted at a venue whose proceedings had not appeared when the list was updated.

Last updated: 11 November 2026.

## Surveys and position papers

Surveys of world models, JEPA and physical AI, plus position papers.

| # | Paper | arXiv | Published |
|---:|---|---|---|
| 1 | [A survey of world models for physical AI with uncertainty representation and control](https://doi.org/10.1007/s44163-026-02122-1) | — | [Discover Artificial Intelligence 2026](https://doi.org/10.1007/s44163-026-02122-1) |
| 2 | [Robotic Video World Models: A Survey of Applications, Research Challenges, Future Directions](https://arxiv.org/abs/2601.07823) | 2601.07823 |  |
| 3 | [From Alignment to Prediction: A Study of Self-Supervised Learning and Predictive Representation Learning](https://arxiv.org/abs/2604.13518) | 2604.13518 |  |
| 4 | [World Model for Robot Learning: A Comprehensive Survey](https://arxiv.org/abs/2605.00080) | 2605.00080 | [IJRR 2026](https://doi.org/10.1177/02783649261488980) |
| 5 | [Physically Native World Models: A Hamiltonian Perspective on Generative World Modeling](https://arxiv.org/abs/2605.00412) | 2605.00412 |  |
| 6 | [World Models for Robotic Manipulation: A Survey](https://arxiv.org/abs/2606.00113) | 2606.00113 | [SmartBot 2026](https://doi.org/10.1002/smb2.70053) |
| 7 | [World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications](https://arxiv.org/abs/2606.00133) | 2606.00133 |  |
| 8 | [A Tutorial on World Models and Physical AI](https://arxiv.org/abs/2606.12783) | 2606.12783 |  |
| 9 | [World-Action Models for Robot Learning and Control: A Survey](https://arxiv.org/abs/2609.16074) | 2609.16074 |  |
| 10 | [Do World Models Make Better Robots? A Survey of Evaluation Benchmarks for Predictive Embodied Intelligence](https://arxiv.org/abs/2609.29669) | 2609.29669 |  |
| 11 | [Physical AI: A Survey of Models, Learning, Systems, and Open Challenges](https://arxiv.org/abs/2610.21171) | 2610.21171 |  |

## JEPA foundations

The core joint-embedding predictive architectures and their training objectives and theory: I-JEPA, MC-JEPA, IWM, V-JEPA, V-JEPA 2 / 2.1, LeJEPA, EB-JEPA and follow-ups.

| # | Paper | arXiv | Published |
|---:|---|---|---|
| 1 | [Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture](https://arxiv.org/abs/2301.08243) | 2301.08243 | [CVPR 2023](https://doi.org/10.1109/CVPR52729.2023.01499) |
| 2 | [MC-JEPA: A Joint-Embedding Predictive Architecture for Self-Supervised Learning of Motion and Content Features](https://arxiv.org/abs/2307.12698) | 2307.12698 |  |
| 3 | [Learning and Leveraging World Models in Visual Representation Learning](https://arxiv.org/abs/2403.00504) | 2403.00504 |  |
| 4 | [Revisiting Feature Prediction for Learning Visual Representations from Video](https://arxiv.org/abs/2404.08471) | 2404.08471 | TMLR 2024 |
| 5 | [V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning](https://arxiv.org/abs/2506.09985) | 2506.09985 |  |
| 6 | [LeJEPA: Provable and Scalable Self-Supervised Learning Without the Heuristics](https://arxiv.org/abs/2511.08544) | 2511.08544 |  |
| 7 | [A Lightweight Library for Energy-Based Joint-Embedding Predictive Architectures](https://arxiv.org/abs/2602.03604) | 2602.03604 | ICLR 2026 Workshop on World Models |
| 8 | [V-JEPA 2.1: Unlocking Dense Features in Video Self-Supervised Learning](https://arxiv.org/abs/2603.14482) | 2603.14482 | [ECCV 2026](https://doi.org/10.1007/978-3-032-37369-4_36) |
| 9 | [Beyond Isotropy in JEPAs: Hamiltonian Geometry and Symplectic Prediction](https://arxiv.org/abs/2605.20107) | 2605.20107 |  |
| 10 | [A Generalization Theory for JEPA-Based World Models](https://arxiv.org/abs/2606.27014) | 2606.27014 |  |
| 11 | [Your Probabilistic JEPA Is Secretly a Hidden Markov Model: A State-Space Interpretation of Joint-Embedding Predictive Learning](https://arxiv.org/abs/2608.13621) | 2608.13621 |  |
| 12 | [World Model for Energy Efficiency Maximization in Dynamic Metasurface Antennas](https://arxiv.org/abs/2610.35813) | 2610.35813 |  |
| 13 | [SuperJEPA: Pretraining with a Supervision-Augmented Joint-Embedding Predictive Architecture for High Energy Physics](https://arxiv.org/abs/2610.36121) | 2610.36121 |  |
| 14 | [Readout and Operating-Point Sensitivity in Event-Stream Candidate Selection](https://arxiv.org/abs/2610.36743) | 2610.36743 |  |
| 15 | [GUI-JEPA: Candidate-Conditioned JEPA Latents as a Fast Action Policy for Mobile GUI Agents](https://arxiv.org/abs/2610.36877) | 2610.36877 |  |
| 16 | [Vision-Language Agents Can Learn in Their Own Latent Worlds](https://arxiv.org/abs/2610.36925) | 2610.36925 |  |
| 17 | [Self-Supervised Latent Action-Conditioned World Modeling for Time Series](https://arxiv.org/abs/2610.37963) | 2610.37963 |  |
| 18 | [DES-JEPA: Learning a Shared Vocabulary for High-Dimensional Discrete Event Sequences](https://arxiv.org/abs/2610.38445) | 2610.38445 |  |
| 19 | [Explore Where It Matters: Targeted Exploration for Efficient Rover Adaptation](https://arxiv.org/abs/2610.38657) | 2610.38657 |  |
| 20 | [Generating Critic-Guided Synthetic Experience in Latent World Models](https://arxiv.org/abs/2610.39100) | 2610.39100 |  |
| 21 | [Proving and Improving the Platonic Representation Hypothesis with JEPAs](https://arxiv.org/abs/2610.39302) | 2610.39302 |  |
| 22 | [Cheap Retrieval and Observation Credit Assignment from One Quantity: The Value of Information](https://arxiv.org/abs/2610.40030) | 2610.40030 |  |
| 23 | [Latent Prediction Yields Cross-Subject Alignable Representations in Sensory-Evoked fMRI](https://arxiv.org/abs/2610.40280) | 2610.40280 |  |
| 24 | [JEDI: Joint-Embedding Demonstration Compression for In-Context Imitation Learning](https://arxiv.org/abs/2610.40356) | 2610.40356 |  |
| 25 | [Hierarchical World Models with Implicit Dynamics](https://arxiv.org/abs/2610.42146) | 2610.42146 |  |
| 26 | [Cross-Domain Joint-Embedding Pretraining For Heterogeneous Industrial Time Series](https://arxiv.org/abs/2611.02489) | 2611.02489 |  |
| 27 | [Computer-Use Agents Gain Little Benefit from a World Model When Conditioned on Tutorials](https://arxiv.org/abs/2611.04073) | 2611.04073 |  |
| 28 | [Ground-Wing: A Parametric 3D Wing-in-Ground-Effect Dataset for Benchmarking Neural Surrogate Models](https://arxiv.org/abs/2611.04571) | 2611.04571 |  |
| 29 | [Stabilizing Neural Emulation of Spatiotemporal Physical Dynamics through Denoising Koopman Latent Dynamics](https://arxiv.org/abs/2611.04642) | 2611.04642 |  |
| 30 | [ChangeJEPA: Predict Before You Compare for Remote Sensing Change Detection](https://arxiv.org/abs/2611.05570) | 2611.05570 |  |
| 31 | [Translate, then decide: asymptotic optimality of latent-space control in bistable systems](https://arxiv.org/abs/2611.05736) | 2611.05736 |  |
| 32 | [Drift-adaptive Representation Preservation for Domain-Incremental Learning](https://arxiv.org/abs/2611.06093) | 2611.06093 |  |
| 33 | [CAPE-JEPA - Cross-modal Adversarial Probabilistic Embedding JEPA](https://arxiv.org/abs/2611.06247) | 2611.06247 |  |
| 34 | [GuidedWAM: Training-Free Energy Guidance for World Action Models in Autonomous Driving](https://arxiv.org/abs/2611.07912) | 2611.07912 |  |
| 35 | [A Stochastic Latent Variable Generalization of Joint-Embedding Predictive Architectures](https://arxiv.org/abs/2611.09302) | 2611.09302 |  |
| 36 | [LO-World: Unified BEV Latent Modeling for Joint 4D Occupancy and LiDAR Forecasting](https://arxiv.org/abs/2611.11912) | 2611.11912 |  |
| 37 | [Benchmarking language models and agents for scientific reasoning in evolving materials laboratories](https://arxiv.org/abs/2611.12014) | 2611.12014 |  |

## Robotics and aerial applications

World models used on robots, drones, underwater vehicles and in driving, e.g. DINO-WM, SkyJEPA, DroneWAM, AquaJEPA.

| # | Paper | arXiv | Published |
|---:|---|---|---|
| 1 | [NeuroBEM: Hybrid Aerodynamic Quadrotor Model](https://arxiv.org/abs/2106.08015) | 2106.08015 | [RSS 2021](https://doi.org/10.15607/RSS.2021.XVII.042) |
| 2 | [KNODE-MPC: A Knowledge-based Data-driven Predictive Control Framework for Aerial Robots](https://arxiv.org/abs/2109.04821) | 2109.04821 | [IEEE RA-L 2022](https://doi.org/10.1109/LRA.2022.3144787) |
| 3 | [Neural-Fly Enables Rapid Learning for Agile Flight in Strong Winds](https://arxiv.org/abs/2205.06908) | 2205.06908 | [Science Robotics 2022](https://doi.org/10.1126/scirobotics.abm6597) |
| 4 | [DINO-WM: World Models on Pre-trained Visual Features enable Zero-shot Planning](https://arxiv.org/abs/2411.04983) | 2411.04983 | [ICML 2025](https://proceedings.mlr.press/v267/zhou25t.html) |
| 5 | [Dream to Fly: Model-Based Reinforcement Learning for Vision-Based Drone Flight](https://arxiv.org/abs/2501.14377) | 2501.14377 | [ICRA 2026](https://doi.org/10.1109/ICRA57385.2026.11695931) |
| 6 | [Active Inference-Driven World Modeling for Adaptive UAV Swarm Trajectory Design](https://arxiv.org/abs/2601.12939) | 2601.12939 |  |
| 7 | [Flying by Inference: Active Inference World Models for Adaptive UAV Swarms](https://arxiv.org/abs/2604.27935) | 2604.27935 |  |
| 8 | [SkyJEPA: Learning Long-Horizon World Models for Zero-Shot Sim-to-Real Control of Quadrotors](https://arxiv.org/abs/2606.23444) | 2606.23444 |  |
| 9 | [AquaJEPA: An Action-Conditioned Multimodal JEPA Family for Underwater Robot Dynamics](https://arxiv.org/abs/2607.29393) | 2607.29393 |  |
| 10 | [JEPLO: Joint-Embedding Predictive Learning for LiDAR-Based Legged Locomotion](https://arxiv.org/abs/2609.15770) | 2609.15770 |  |
| 11 | [DroneWAM: Efficient World Action Model for Drone Visual Navigation](https://arxiv.org/abs/2609.33148) | 2609.33148 |  |
| 12 | [AD-E2E-JEPA: A Joint-Embedding Predictive Architecture For End-to-End Autonomous Driving](https://arxiv.org/abs/2609.34085) | 2609.34085 |  |
| 13 | [RoboJEPA: Scaling Robotic Latent World Models](https://arxiv.org/abs/2610.10515) | 2610.10515 |  |
| 14 | [RynnWorld-Latent: A Cross-Embodiment World Model Conditioned on Universal Latent Actions](https://arxiv.org/abs/2610.36791) | 2610.36791 |  |
| 15 | [Neural Compression of Long ADMM Trajectory for Multiparametric Quadratic Program](https://arxiv.org/abs/2610.38079) | 2610.38079 |  |
| 16 | [SaiVLA-JEPA: Evaluating Future Latent Prediction in JEPA-Conditioned VLA Control](https://arxiv.org/abs/2610.38508) | 2610.38508 |  |
| 17 | [OpenFlyV2: An onboard vision-language-action model for aerial perception and navigation](https://arxiv.org/abs/2610.39287) | 2610.39287 |  |
| 18 | [Continuous-Action World Models: Learning Cross-Embodiment Spatiotemporal Dynamics Priors](https://arxiv.org/abs/2610.40401) | 2610.40401 |  |
| 19 | [OpenNWM: A Generalist Navigation World Model with Latent Action Pretraining](https://arxiv.org/abs/2611.01844) | 2611.01844 |  |
| 20 | [MKD2World: A Typed Spatial MarkDown World Model For Web Agents](https://arxiv.org/abs/2611.06544) | 2611.06544 |  |
| 21 | [Motion-guided Contrastive Regularization For Latent World Models](https://arxiv.org/abs/2611.06901) | 2611.06901 |  |
| 22 | [PlayGen2: Learning Real-Time Playable Worlds with Explicit 3D State](https://arxiv.org/abs/2611.07867) | 2611.07867 |  |
| 23 | [GPWM: Modeling the World as 3D Particle Motion](https://arxiv.org/abs/2611.08338) | 2611.08338 |  |
| 24 | [Extended Model-Based Learned Inertial Odometry](https://arxiv.org/abs/2611.09584) | 2611.09584 | [ICUAS 2026](https://doi.org/10.1109/ICUAS69441.2026.11598619) |
| 25 | [WorldFoundry: Towards Unified Infrastructure for World Intelligence](https://arxiv.org/abs/2611.10771) | 2611.10771 |  |
| 26 | [ScanDreamer: A Map-Grounded World Model for Quadrotor Navigation](https://arxiv.org/abs/2611.11605) | 2611.11605 |  |
| 27 | [Action Representation for Spatial Generalization in Robot World Models](https://arxiv.org/abs/2611.11869) | 2611.11869 |  |
| 28 | [Compass 1: Towards Open-World and Persistent Embodied Navigation from Monocular RGB Videos](https://arxiv.org/abs/2611.12087) | 2611.12087 |  |

## Action-conditioned models and planning

Models that predict the effect of actions and are used for planning or policy learning: LeWorldModel, PLDM, hierarchical and goal-conditioned planners, VLA models, evaluation and robustness studies.

| # | Paper | arXiv | Published |
|---:|---|---|---|
| 1 | [ACT-JEPA: Novel Joint-Embedding Predictive Architecture for Efficient Policy Representation Learning](https://arxiv.org/abs/2501.14622) | 2501.14622 | [IEEE Access 2026](https://doi.org/10.1109/ACCESS.2026.3696039) |
| 2 | [Learning from Reward-Free Offline Data: A Case for Planning with Latent Dynamics Models](https://arxiv.org/abs/2502.14819) | 2502.14819 | [NeurIPS 2025](https://doi.org/10.52202/085713-1465) |
| 3 | [How Well Do Latent World Models Understand Partially Observable Safety Constraints?](https://arxiv.org/abs/2510.06492) | 2510.06492 | CoRL 2026 (accepted) |
| 4 | [What Drives Success in Physical Planning with Joint-Embedding Predictive World Models?](https://arxiv.org/abs/2512.24497) | 2512.24497 | TMLR 2025 |
| 5 | [Value-guided action planning with JEPA world models](https://arxiv.org/abs/2601.00844) | 2601.00844 |  |
| 6 | [VLA-JEPA: Enhancing Vision-Language-Action Model with Latent World Model](https://arxiv.org/abs/2602.10098) | 2602.10098 | [ECCV 2026](https://doi.org/10.1007/978-3-032-37196-6_26) |
| 7 | [JEPA-Bisim: Learning Robust Visual Representations for Planning with Joint-Embedding Predictive World Models](https://arxiv.org/abs/2602.18639) | 2602.18639 |  |
| 8 | [LeWorldModel: Stable End-to-End Joint-Embedding Predictive Architecture from Pixels](https://arxiv.org/abs/2603.19312) | 2603.19312 |  |
| 9 | [Hierarchical Planning with Latent World Models](https://arxiv.org/abs/2604.03208) | 2604.03208 | CoRL 2026 (accepted) |
| 10 | [ELVIS: Ensemble-Calibrated Latent Imagination for Long-Horizon Visual MPC](https://arxiv.org/abs/2605.04709) | 2605.04709 |  |
| 11 | [PLUME: Probabilistic Latent Unified World Modeling and Parameter Estimation for Multi-Finger Manipulation](https://arxiv.org/abs/2606.11396) | 2606.11396 |  |
| 12 | [Delta-JEPA: Learning Action-Sensitive World Models via Latent Difference Decoding](https://arxiv.org/abs/2606.31232) | 2606.31232 |  |
| 13 | [Temporal-Distance JEPA: Plan-Aware Representation Learning for Latent World Model Predictive Control](https://arxiv.org/abs/2607.25337) | 2607.25337 |  |
| 14 | [JEPA-WAM: Learning Vision-Language-Action Policies with Joint-Embedding World Modeling](https://arxiv.org/abs/2608.09381) | 2608.09381 |  |
| 15 | [StageWAM: Joint-Embedding Stage Prediction for World-Action Models in Robot Manipulation](https://arxiv.org/abs/2608.10780) | 2608.10780 |  |
| 16 | [Diagnosing JEPA World Models with Action-Conditioned Predictive Consistency](https://arxiv.org/abs/2608.12939) | 2608.12939 |  |
| 17 | [SCALE: State-Calibrated Latent Embeddings for JEPA Planning in the Right Geometry](https://arxiv.org/abs/2608.16287) | 2608.16287 |  |
| 18 | [No Gaussian Required: Contrastive Inverse Dynamics for JEPA World Models](https://arxiv.org/abs/2608.17542) | 2608.17542 |  |
| 19 | [Toward Physically Grounded JEPA World Models for Goal-Conditioned Robotic Planning](https://arxiv.org/abs/2609.03565) | 2609.03565 | IROS 2026 Workshop |
| 20 | [D-JEPA: A Decision-Aligned Latent World Model](https://arxiv.org/abs/2609.24749) | 2609.24749 |  |
| 21 | [CF-JEPA: Improving Robustness of JEPA World Models via Controllability Factorization](https://arxiv.org/abs/2610.00727) | 2610.00727 |  |
| 22 | [TwinJEPA: Action-Preferred Predictive Representations for Goal-Conditioned Control](https://arxiv.org/abs/2610.02922) | 2610.02922 |  |
| 23 | [H-JEPA: End-to-End Learning of Hierarchical World Models for Visual Planning](https://arxiv.org/abs/2610.06805) | 2610.06805 |  |
| 24 | [A Belief-State World Model for Catheter Navigation under Sparse Fluoroscopy: A Planar Proof of Concept](https://arxiv.org/abs/2610.08469) | 2610.08469 |  |
| 25 | [LeWAM: End-to-End World and Action Modeling with JEPAs](https://arxiv.org/abs/2610.12818) | 2610.12818 |  |
| 26 | [Adapt for Planning, Not just Prediction: Optimistic Test-Time World Model Adaptation](https://arxiv.org/abs/2610.35636) | 2610.35636 | CoRL 2026 Workshop |
| 27 | [Cinematize from Unreal: Agentic Choreography for Controllable World Simulation](https://arxiv.org/abs/2610.38468) | 2610.38468 |  |
| 28 | [Structural-Test Geometry as an Inductive Bias for Partially Observable World Models](https://arxiv.org/abs/2610.38903) | 2610.38903 |  |
| 29 | [Agentic LinkDreamer: Adaptive Neuro-Fuzzy World-Model Decision Making for Intermittent V2X Cooperative Perception](https://arxiv.org/abs/2610.39258) | 2610.39258 |  |
| 30 | [PRIME W0: Physical Priors from World Models for Embodied Manipulation](https://arxiv.org/abs/2610.39528) | 2610.39528 |  |
| 31 | [world2vec: Mechanistic world models through latent dynamics learning](https://arxiv.org/abs/2610.40637) | 2610.40637 |  |
| 32 | [One Verdict Is Not Enough: Regression Testing Learned World Models and Their Test Harnesses](https://arxiv.org/abs/2610.41130) | 2610.41130 |  |
| 33 | [Online Learning of Heterogeneous Locomotion Dynamics under Reinforcement Learning Policies for Precise Loco-Manipulation](https://arxiv.org/abs/2610.41892) | 2610.41892 |  |
| 34 | [Spoofing the Latent State: Imperceptible Goal-Image Attacks Derail Planning in LeWorldModel](https://arxiv.org/abs/2611.00427) | 2611.00427 |  |
| 35 | [SCOUT: Planning under Occlusion via Object-Centric World Model Rollouts](https://arxiv.org/abs/2611.01600) | 2611.01600 |  |
| 36 | [Compression Forcing: Hierarchical History Tokenization Enables Flexible World Models](https://arxiv.org/abs/2611.04028) | 2611.04028 |  |
| 37 | [Time-to-Goal: Learned Temporal Metrics for Long-Horizon Planning with JEPA World Models](https://arxiv.org/abs/2611.05847) | 2611.05847 |  |
| 38 | [MAC-v2: Long-horizon model-based value expansion from pixels](https://arxiv.org/abs/2611.07245) | 2611.07245 |  |
| 39 | [Learning Robotic World Models with Semantic and Visual Feedback](https://arxiv.org/abs/2611.07850) | 2611.07850 |  |
| 40 | [La-JEPA: Compact Robot Policies with Latent World Modeling](https://arxiv.org/abs/2611.08156) | 2611.08156 |  |
| 41 | [Dynamics-Informed Action Learning for Goal-Conditioned Latent Planning](https://arxiv.org/abs/2611.10660) | 2611.10660 |  |
| 42 | [WARP-JEPA: World-Model-in-the-Loop Amortized Rollout Planning for Frozen Hierarchical Joint-Embedding Predictive Architectures](https://arxiv.org/abs/2611.10806) | 2611.10806 |  |
| 43 | [K-PWM: Control-Oriented Structured Bilinear World Models under Partial Observation](https://arxiv.org/abs/2611.11521) | 2611.11521 | NeurIPS 2026 (accepted) |
| 44 | [Planners Exploit Deterministic Error: Dithered Low-Bit World Models](https://arxiv.org/abs/2611.11780) | 2611.11780 |  |
| 45 | [How Many Candidates Does a One-Step World Model Need? A Random-Codebook Account of Nearest-of-m Training on Frozen DINO Tokens](https://arxiv.org/abs/2611.11887) | 2611.11887 |  |
| 46 | [An Evaluation of Tabular Foundation Models as Training-Free World Models](https://arxiv.org/abs/2611.11921) | 2611.11921 |  |
| 47 | [Σ-LeWM: Learning World Models via S-Information for Robot Control](https://arxiv.org/abs/2611.12732) | 2611.12732 |  |

## Latent dynamics, physics structure and theory

Structured latent dynamics (Hamiltonian, symplectic, Koopman, bilinear, semigroup), probabilistic JEPAs, collapse and identifiability analyses.

| # | Paper | arXiv | Published |
|---:|---|---|---|
| 1 | [Robust and Safe Autonomous Navigation for Systems with Learned SE(3) Hamiltonian Dynamics](https://arxiv.org/abs/2207.10840) | 2207.10840 | [IEEE Open Journal of Control Systems 2022](https://doi.org/10.1109/OJCSYS.2022.3201554) |
| 2 | [Uncertainty Representations in State-Space Layers for Deep Reinforcement Learning under Partial Observability](https://arxiv.org/abs/2409.16824) | 2409.16824 |  |
| 3 | [Learning Hamiltonian Dynamics with Bayesian Data Assimilation](https://arxiv.org/abs/2501.18808) | 2501.18808 |  |
| 4 | [KILO-EKF: Koopman-Inspired Learned Observations Extended Kalman Filter](https://arxiv.org/abs/2601.12463) | 2601.12463 |  |
| 5 | [VJEPA: Variational Joint Embedding Predictive Architectures as Probabilistic World Models](https://arxiv.org/abs/2601.14354) | 2601.14354 | [ICML 2026](https://icml.cc/virtual/2026/poster/61579) |
| 6 | [From Gradients to Riccati Geometry: Kalman World Models for Single-Pass Learning](https://arxiv.org/abs/2603.13423) | 2603.13423 |  |
| 7 | [Latent State Design for World Models under Sufficiency Constraints](https://arxiv.org/abs/2605.01694) | 2605.01694 |  |
| 8 | [HaM-World: Soft-Hamiltonian World Models with Selective Memory for Planning](https://arxiv.org/abs/2605.05951) | 2605.05951 | NeurIPS 2026 (accepted) |
| 9 | [Phys-JEPA: Physics-Informed Latent World Models for Multivariate Time-Series Forecasting](https://arxiv.org/abs/2606.16076) | 2606.16076 |  |
| 10 | [A Control Theory of Predictability in Latent World Models](https://arxiv.org/abs/2607.10362) | 2607.10362 |  |
| 11 | [Toward Goal-Agnostic Joint-Embedding Predictive Control of Partial Differential Equations](https://arxiv.org/abs/2607.21644) | 2607.21644 |  |
| 12 | [SJEPA: Learning Elegant Latent Dynamics with Hybrid Symbolic-Neural Predictors](https://arxiv.org/abs/2608.04060) | 2608.04060 |  |
| 13 | [PhyLatent: Learning Dynamics-Relevant Representations for JEPA World Models](https://arxiv.org/abs/2608.05720) | 2608.05720 |  |
| 14 | [Is Forward Prediction Enough? Physical State Grounding for JEPA World Models](https://arxiv.org/abs/2608.06799) | 2608.06799 |  |
| 15 | [JEPA-x: Cross-Predictive Physics Grounding for Forecastable Latent Dynamics](https://arxiv.org/abs/2608.24044) | 2608.24044 |  |
| 16 | [Flow-JEPA: Robust Latent Dynamics for JEPA World Models via Flow Matching](https://arxiv.org/abs/2608.29029) | 2608.29029 |  |
| 17 | [Semigroup-JEPA: Latent Dynamics Consistency for Zero-Shot Physics Generalization](https://arxiv.org/abs/2609.10464) | 2609.10464 |  |
| 18 | [I Act Therefore I Am: When Is JEPA's Action-Conditioning Enough to Learn Causal Mechanisms?](https://arxiv.org/abs/2609.31161) | 2609.31161 |  |
| 19 | [D-JEPA: Design-Recoverable JEPA Representation with Swappable Physics Decoders](https://arxiv.org/abs/2609.33110) | 2609.33110 |  |
| 20 | [Hamiltonian JEPA: Action-Conditioned World Models with an Inherited Control State](https://arxiv.org/abs/2609.33497) | 2609.33497 |  |
| 21 | [Bilinear World Models: Learning Representations with Structured Dynamics for Efficient Control](https://arxiv.org/abs/2609.36305) | 2609.36305 |  |
| 22 | [JEPA-TTT: Persistent Test-Time Training of Latent World Models for Planning under Dynamics Shifts](https://arxiv.org/abs/2610.00722) | 2610.00722 | NeurIPS 2026 Workshop on World Models in Physical AI |
| 23 | [AVL-JEPA: Preventing Causal Dynamics Information Collapse In Joint Embedding Predictive Architecture World Models](https://arxiv.org/abs/2610.03587) | 2610.03587 |  |
| 24 | [Frozen in a Frame: The Velocity Blind Spot in JEPA World Models](https://arxiv.org/abs/2610.04585) | 2610.04585 |  |
| 25 | [Preserving Unstable Modes Through Inverse Dynamics in JEPA World Models](https://arxiv.org/abs/2610.07540) | 2610.07540 |  |
| 26 | [MDN-VJEPA: Multimodal Probabilistic Joint-Embedding World Models](https://arxiv.org/abs/2610.13956) | 2610.13956 |  |
| 27 | [LeHami: Symplectic Latent Dynamics for World Models](https://arxiv.org/abs/2610.15267) | 2610.15267 |  |
| 28 | [DriveUniTok: A Unified Multimodal Tokenizer for Driving World-Action Models](https://arxiv.org/abs/2610.35044) | 2610.35044 |  |
| 29 | [Multi-Horizon Future Discovery for Physics-Informed Exploration](https://arxiv.org/abs/2610.35468) | 2610.35468 |  |
| 30 | [E0.5: From Reconstructive to Future-Predictive 3D Foundations for Robotic World-Action Modeling](https://arxiv.org/abs/2610.36011) | 2610.36011 |  |
| 31 | [AC-JEPA: Anchored Cross-Modal Joint Embedding Predictive Architecture for Visual-to-Symbolic Translation](https://arxiv.org/abs/2610.36493) | 2610.36493 |  |
| 32 | [SWIM: Learning What Matters from Behaviors for JEPA World Models](https://arxiv.org/abs/2610.36662) | 2610.36662 |  |
| 33 | [WorldFlow: Joint Video and 3D Motion Prediction via Large-Scale Pretraining](https://arxiv.org/abs/2610.39278) | 2610.39278 |  |
| 34 | [Bayesian Offline Multi-Agent Reinforcement Learning with Latent World Models](https://arxiv.org/abs/2610.39576) | 2610.39576 |  |
| 35 | [Learning momenta for Hamiltonian-based models](https://arxiv.org/abs/2611.01269) | 2611.01269 |  |
| 36 | [Identifiable Signed Causal Learning via Latent Stochastic Differential Equations for Inferring Brain Dynamic Effective Connectivity](https://arxiv.org/abs/2611.02876) | 2611.02876 |  |
| 37 | [ForceLDM: A Force-aware Latent Dynamics Model for Contact-Rich Manipulation](https://arxiv.org/abs/2611.03294) | 2611.03294 |  |
| 38 | [Embodied AI for Scientific Discovery: From Physical Action to Scientific Evidence](https://arxiv.org/abs/2611.04371) | 2611.04371 |  |
| 39 | [Comparing model representations and fitting methods for port-Hamiltonian system identification](https://arxiv.org/abs/2611.05031) | 2611.05031 |  |
| 40 | [SO(3)-Equivariant Learning on CAD Boundary Representations](https://arxiv.org/abs/2611.05449) | 2611.05449 |  |
| 41 | [Readable Is Not Steerable: Pre-Registered Tests of Physical Structure in Learned Fluid Representations](https://arxiv.org/abs/2611.05577) | 2611.05577 |  |
| 42 | [Dynamic Watermarking and Action-Conditioned Latent Dynamics for Secure Vision-Based Controllers](https://arxiv.org/abs/2611.07403) | 2611.07403 |  |
| 43 | [Equivariant Deep Learning in Direct-Product Space for Electronic-Structure Hamiltonian Prediction](https://arxiv.org/abs/2611.07695) | 2611.07695 |  |
| 44 | [Learning a patient world model for health system simulation in intensive care](https://arxiv.org/abs/2611.08392) | 2611.08392 |  |
| 45 | [Stochastic Port-Hamiltonian Gaussian Processes for Learning from Noisy Dynamics on Lie Groups](https://arxiv.org/abs/2611.10864) | 2611.10864 |  |
| 46 | [SurgWorld: Learning Surgical Representations Beyond Observation via Latent Prediction](https://arxiv.org/abs/2611.11140) | 2611.11140 |  |
| 47 | [DeepSoMo: Deformable Object Motion Estimation under Proprioceptive Partial Observability via Predictive Latent Dynamics](https://arxiv.org/abs/2611.11242) | 2611.11242 |  |
| 48 | [Good Views Are Not Enough: Global Counterexamples for Gaussian-Regularized JEPAs](https://arxiv.org/abs/2611.12137) | 2611.12137 |  |

## 3D, spatial and object-centric models

Point-cloud, depth, LiDAR, 3D-scene, object-centric and graph-structured predictive models.

| # | Paper | arXiv | Published |
|---:|---|---|---|
| 1 | [Structured World Belief for Reinforcement Learning in POMDP](https://arxiv.org/abs/2107.08577) | 2107.08577 |  |
| 2 | [Point-JEPA: A Joint Embedding Predictive Architecture for Self-Supervised Learning on Point Cloud](https://arxiv.org/abs/2404.16432) | 2404.16432 | [WACV 2025](https://doi.org/10.1109/WACV61041.2025.00714) |
| 3 | [3D-JEPA: A Joint Embedding Predictive Architecture for 3D Self-Supervised Representation Learning](https://arxiv.org/abs/2409.15803) | 2409.15803 |  |
| 4 | [POMA-3D: The Point Map Way to 3D Scene Understanding](https://arxiv.org/abs/2511.16567) | 2511.16567 | [CVPR Findings 2026](https://doi.org/10.1109/CVPRF71909.2026.00699) |
| 5 | [CrossJEPA: Cross-Modal Joint-Embedding Predictive Architecture for Efficient 3D Representation Learning from 2D Images](https://arxiv.org/abs/2511.18424) | 2511.18424 |  |
| 6 | [Semantic Belief-State World Model for 3D Human Motion Prediction](https://arxiv.org/abs/2601.03517) | 2601.03517 |  |
| 7 | [Causal-JEPA: Learning World Models through Object-Level Latent Masking](https://arxiv.org/abs/2602.11389) | 2602.11389 | ICML 2026 |
| 8 | [Self-Supervised JEPA-based World Models for LiDAR Occupancy Completion and Forecasting](https://arxiv.org/abs/2602.12540) | 2602.12540 |  |
| 9 | [UWM-JEPA: Predictive World Models That Imagine in Belief Space](https://arxiv.org/abs/2605.25313) | 2605.25313 |  |
| 10 | [Neural Voxel Dynamics: Learning Volumetric Feature Advection for 3D Physics in V-JEPA Latent Space](https://arxiv.org/abs/2606.26410) | 2606.26410 |  |
| 11 | [J-LAW: Joint Localization and Action-Conditioned World Modeling via Coupled Latent Factor Graphs](https://arxiv.org/abs/2606.28712) | 2606.28712 |  |
| 12 | [JEPADepth: Masked Predictive Representation Learning for Self-Supervised Monocular Depth Estimation](https://arxiv.org/abs/2607.26600) | 2607.26600 |  |
| 13 | [SR-JEPA: Learning Predictive Latent State in 3D Scenes](https://arxiv.org/abs/2608.05774) | 2608.05774 |  |
| 14 | [Does Latent Planning Survive Point Clouds? Action-Conditioned JEPA World Models for Geometric Observations and Goals](https://arxiv.org/abs/2608.29434) | 2608.29434 |  |
| 15 | [MotionJEPA: Preventing Temporal Feature Collapse by Capturing Visual Changes in Latent Space](https://arxiv.org/abs/2609.23881) | 2609.23881 |  |
| 16 | [4DGS-JEPA: Temporally Compositional Joint-Embedding Prediction for Dynamic Gaussian Splatting](https://arxiv.org/abs/2609.25036) | 2609.25036 |  |
| 17 | [BeliefGraph-JEPA: Structured Latent World Models for Action-Conditioned Time Series](https://arxiv.org/abs/2610.05409) | 2610.05409 |  |
| 18 | [GAWM: A Compact Latent World-Action Model for Multi-Task Robot Manipulation](https://arxiv.org/abs/2610.37091) | 2610.37091 |  |
| 19 | [JEPA-Inspired Latent Field Prediction for Sparse-Pilot MIMO-OFDM Channel Reconstruction](https://arxiv.org/abs/2610.37391) | 2610.37391 |  |
| 20 | [Representing the Unseen: Rethinking Visual Imagination for Spatial Reasoning](https://arxiv.org/abs/2610.37437) | 2610.37437 |  |
| 21 | [Understanding the limits of latent world models](https://arxiv.org/abs/2610.37588) | 2610.37588 |  |
| 22 | [Seeing and Imagining as One: Unified Video Generation and 4D Perception for Embodied World Modeling](https://arxiv.org/abs/2610.39232) | 2610.39232 |  |
| 23 | [GROME: GROunding Factorized MEmory into Video World Models](https://arxiv.org/abs/2610.39812) | 2610.39812 |  |
| 24 | [HiFOR: Hierarchical Foresight with Action-Guided World Grounding for Vision-Language-Action Model](https://arxiv.org/abs/2610.40373) | 2610.40373 |  |
| 25 | [Fight World Model: Customizable Combat through Visual Interaction Proxies](https://arxiv.org/abs/2610.40607) | 2610.40607 |  |
| 26 | [L3G-World: Real-Time Infinite World Generation with Latent 3D Gaussian Memory](https://arxiv.org/abs/2610.40614) | 2610.40614 |  |
| 27 | [Xiaomi Auto World Model 2.0: Causal World Models for Real-World Driving and Embodied Intelligence](https://arxiv.org/abs/2611.01677) | 2611.01677 |  |
| 28 | [AgiWorld: An Agentic Video World Model for Building Persistent Worlds](https://arxiv.org/abs/2611.02341) | 2611.02341 |  |
| 29 | [INTERACT: Learning Interaction-Aware World Dynamics from Driving Videos for Autonomous Driving](https://arxiv.org/abs/2611.02526) | 2611.02526 |  |
| 30 | [FlowBench: Counterfactual Imagination Training for Spatial Intelligence](https://arxiv.org/abs/2611.03937) | 2611.03937 |  |
| 31 | [Physical Experience Builds Continual Spatial World Models](https://arxiv.org/abs/2611.04016) | 2611.04016 |  |
| 32 | [Hybrid Particle-Voxel Dynamics for Multimodal 3D World Simulation](https://arxiv.org/abs/2611.04492) | 2611.04492 |  |
| 33 | [Trajectory Evaluation via Rollout-Free World Model for End-to-end Autonomous Driving](https://arxiv.org/abs/2611.05072) | 2611.05072 |  |
| 34 | [TouchéWorld tech report : Towards Online Unified Camera--Hand Exploration in Generative Worlds](https://arxiv.org/abs/2611.06061) | 2611.06061 |  |
| 35 | [GEKey: Learning Geodesic Eccentric 3D Keypoints via Self-Supervision](https://arxiv.org/abs/2611.07677) | 2611.07677 |  |
| 36 | [ObjectWorld: Scaling Object-Centric World Models with A Large-Scale 3D Full-Object Flow Dataset](https://arxiv.org/abs/2611.11085) | 2611.11085 |  |
| 37 | [DexForesight: Grounding Dexterous Policies with Implicit Spatial Foresight](https://arxiv.org/abs/2611.11166) | 2611.11166 |  |
| 38 | [ForeAct: Geometry-Guided Action Learning from World Representations](https://arxiv.org/abs/2611.11500) | 2611.11500 |  |
| 39 | [QCC-WM: Linking Macro-State Dynamics and Visual Generation via Quotient Causal Construction](https://arxiv.org/abs/2611.12353) | 2611.12353 |  |

## Related non-JEPA world models

Reconstruction-based or Dreamer-style world models with physical structure, kept for comparison.

| # | Paper | arXiv | Published |
|---:|---|---|---|
| 1 | [Learning Latent Dynamics for Planning from Pixels](https://arxiv.org/abs/1811.04551) | 1811.04551 | [ICML 2019](https://proceedings.mlr.press/v97/hafner19a.html) |
| 2 | [PlaNet of the Bayesians: Reconsidering and Improving Deep Planning Network by Incorporating Bayesian Inference](https://arxiv.org/abs/2003.00370) | 2003.00370 | [IROS 2020](https://doi.org/10.1109/iros45743.2020.9340873) |
| 3 | [Mastering Diverse Domains through World Models](https://arxiv.org/abs/2301.04104) | 2301.04104 | [Nature 2025](https://doi.org/10.1038/s41586-025-08744-2) |
| 4 | [TD-MPC2: Scalable, Robust World Models for Continuous Control](https://arxiv.org/abs/2310.16828) | 2310.16828 | ICLR 2024 |
| 5 | [Port-Hamiltonian Neural ODE Networks on Lie Groups For Robot Dynamics Learning and Control](https://arxiv.org/abs/2401.09520) | 2401.09520 | [IEEE Transactions on Robotics 2024](https://doi.org/10.1109/TRO.2024.3428433) |
| 6 | [PH-Dreamer: A Physics-Driven World Model via Port-Hamiltonian Generative Dynamics](https://arxiv.org/abs/2605.18303) | 2605.18303 |  |
| 7 | [Koopman Dreamer: Spectrally Constrained Latent Dynamics for Stable World-Model Imagination](https://arxiv.org/abs/2607.19719) | 2607.19719 |  |
| 8 | [Conservation Buys Stability and Factoring Buys Counterfactuals in Physical World Models](https://arxiv.org/abs/2609.19674) | 2609.19674 |  |
