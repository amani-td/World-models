# World Models: JEPA paper collection

This is a collection of JEPA papers and the latent world models built on them, together with closely related non-JEPA world models. Each entry links to the paper, to its published version where one exists, and to its code where code is available.

## How the list is arranged

Papers are grouped by topic. Within each group they are ordered by arXiv identifier, so older work comes first.

| Group | What it contains |
|---|---|
| [Surveys and position papers](#surveys-and-position-papers) | Surveys of world models, JEPA and physical AI, plus position papers. |
| [JEPA foundations](#jepa-foundations) | The core joint-embedding predictive architectures and their training objectives and theory: I-JEPA, MC-JEPA, IWM, V-JEPA, V-JEPA 2 / 2.1, LeJEPA, EB-JEPA and follow-ups. |
| [Robotics and aerial applications](#robotics-and-aerial-applications) | World models used on robots, drones, underwater vehicles and in driving, e.g. DINO-WM, SkyJEPA, DroneWAM, AquaJEPA. |
| [Action-conditioned models and planning](#action-conditioned-models-and-planning) | Models that predict the effect of actions and are used for planning or policy learning: LeWorldModel, PLDM, hierarchical and goal-conditioned planners, VLA models, evaluation and robustness studies. |
| [Latent dynamics, physics structure and theory](#latent-dynamics-physics-structure-and-theory) | Structured latent dynamics (Hamiltonian, symplectic, Koopman, bilinear, semigroup), probabilistic JEPAs, collapse and identifiability analyses. |
| [3D, spatial and object-centric models](#3d-spatial-and-object-centric-models) | Point-cloud, depth, LiDAR, 3D-scene, object-centric and graph-structured predictive models. |
| [Related non-JEPA world models](#related-non-jepa-world-models) | Reconstruction-based and Dreamer-style latent world models (World Models, Dreamer V1–V4, DayDreamer), including physics-structured variants, kept for comparison. |

**Columns**

- **Paper** links to the arXiv abstract page.
- **Published** gives the journal or conference version, with its DOI or proceedings link. An empty cell means no peer-reviewed version was found. "(accepted)" marks papers accepted at a venue whose proceedings had not appeared yet.
- **Code** gives the authors' repository, taken from the paper itself, its Hugging Face page, or the authors' own GitHub project. "(announced, not public yet)" means the paper names a repository that is not online yet. Repositories marked *(unofficial)* are by other people and cite the paper in their README; they have not been checked for correctness. An empty cell means no code was found.

Last updated: 11 November 2026.

## Surveys and position papers

Surveys of world models, JEPA and physical AI, plus position papers.

| Paper | arXiv | Published | Code |
|---|---|---|---|
| [A survey of world models for physical AI with uncertainty representation and control](https://doi.org/10.1007/s44163-026-02122-1) | — | [Discover Artificial Intelligence 2026](https://doi.org/10.1007/s44163-026-02122-1) |  |
| [Understanding World or Predicting Future? A Comprehensive Survey of World Models](https://arxiv.org/abs/2411.14499) | 2411.14499 | [ACM Computing Surveys 2025](https://doi.org/10.1145/3746449) | [tsinghua-fib-lab/World-Model](https://github.com/tsinghua-fib-lab/World-Model) |
| [Critique of World Model](https://arxiv.org/abs/2507.05169) | 2507.05169 |  |  |
| [A Comprehensive Survey on World Models for Embodied AI](https://arxiv.org/abs/2510.16732) | 2510.16732 |  | [Li-Zn-H/AwesomeWorldModels](https://github.com/Li-Zn-H/AwesomeWorldModels) |
| [Robotic Video World Models: A Survey of Applications, Research Challenges, Future Directions](https://arxiv.org/abs/2601.07823) | 2601.07823 |  | [irom-princeton/awesome-robotics-video-world-model-papers](https://github.com/irom-princeton/awesome-robotics-video-world-model-papers) |
| [From Alignment to Prediction: A Study of Self-Supervised Learning and Predictive Representation Learning](https://arxiv.org/abs/2604.13518) | 2604.13518 |  |  |
| [World Model for Robot Learning: A Comprehensive Survey](https://arxiv.org/abs/2605.00080) | 2605.00080 | [IJRR 2026](https://doi.org/10.1177/02783649261488980) | [NTUMARS/Awesome-World-Model-for-Robotics-Policy](https://github.com/NTUMARS/Awesome-World-Model-for-Robotics-Policy) |
| [Physically Native World Models: A Hamiltonian Perspective on Generative World Modeling](https://arxiv.org/abs/2605.00412) | 2605.00412 |  |  |
| [World Models for Robotic Manipulation: A Survey](https://arxiv.org/abs/2606.00113) | 2606.00113 | [SmartBot 2026](https://doi.org/10.1002/smb2.70053) |  |
| [World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications](https://arxiv.org/abs/2606.00133) | 2606.00133 |  |  |
| [A Tutorial on World Models and Physical AI](https://arxiv.org/abs/2606.12783) | 2606.12783 |  |  |
| [World-Action Models for Robot Learning and Control: A Survey](https://arxiv.org/abs/2609.16074) | 2609.16074 |  |  |
| [Do World Models Make Better Robots? A Survey of Evaluation Benchmarks for Predictive Embodied Intelligence](https://arxiv.org/abs/2609.29669) | 2609.29669 |  |  |
| [Physical AI: A Survey of Models, Learning, Systems, and Open Challenges](https://arxiv.org/abs/2610.21171) | 2610.21171 |  |  |

## JEPA foundations

The core joint-embedding predictive architectures and their training objectives and theory: I-JEPA, MC-JEPA, IWM, V-JEPA, V-JEPA 2 / 2.1, LeJEPA, EB-JEPA and follow-ups.

| Paper | arXiv | Published | Code |
|---|---|---|---|
| [Bootstrap your own latent: A new approach to self-supervised Learning](https://arxiv.org/abs/2006.07733) | 2006.07733 | NeurIPS 2020 | [google-deepmind/deepmind-research](https://github.com/google-deepmind/deepmind-research)<br>[lucidrains/byol-pytorch](https://github.com/lucidrains/byol-pytorch) (unofficial) |
| [VICReg: Variance-Invariance-Covariance Regularization for Self-Supervised Learning](https://arxiv.org/abs/2105.04906) | 2105.04906 | ICLR 2022 | [facebookresearch/vicreg](https://github.com/facebookresearch/vicreg)<br>[jolibrain/vicreg-loss](https://github.com/jolibrain/vicreg-loss) (unofficial) |
| [Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture](https://arxiv.org/abs/2301.08243) | 2301.08243 | [CVPR 2023](https://doi.org/10.1109/CVPR52729.2023.01499) | [facebookresearch/ijepa](https://github.com/facebookresearch/ijepa)<br>[gaasher/I-JEPA](https://github.com/gaasher/I-JEPA) (unofficial) |
| [DINOv2: Learning Robust Visual Features without Supervision](https://arxiv.org/abs/2304.07193) | 2304.07193 | TMLR 2024 | [facebookresearch/dinov2](https://github.com/facebookresearch/dinov2) |
| [MC-JEPA: A Joint-Embedding Predictive Architecture for Self-Supervised Learning of Motion and Content Features](https://arxiv.org/abs/2307.12698) | 2307.12698 |  |  |
| [Learning and Leveraging World Models in Visual Representation Learning](https://arxiv.org/abs/2403.00504) | 2403.00504 |  | [garrettallen14/JEPA-Image-World-Model](https://github.com/garrettallen14/JEPA-Image-World-Model) (unofficial) |
| [Revisiting Feature Prediction for Learning Visual Representations from Video](https://arxiv.org/abs/2404.08471) | 2404.08471 | TMLR 2024 | [facebookresearch/jepa](https://github.com/facebookresearch/jepa) |
| [Intuitive physics understanding emerges from self-supervised pretraining on natural videos](https://arxiv.org/abs/2502.11831) | 2502.11831 |  | [facebookresearch/jepa-intuitive-physics](https://github.com/facebookresearch/jepa-intuitive-physics) |
| [V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning](https://arxiv.org/abs/2506.09985) | 2506.09985 |  | [facebookresearch/vjepa2](https://github.com/facebookresearch/vjepa2) |
| [LeJEPA: Provable and Scalable Self-Supervised Learning Without the Heuristics](https://arxiv.org/abs/2511.08544) | 2511.08544 |  | [galilai-group/lejepa](https://github.com/galilai-group/lejepa) |
| [A Lightweight Library for Energy-Based Joint-Embedding Predictive Architectures](https://arxiv.org/abs/2602.03604) | 2602.03604 | ICLR 2026 Workshop on World Models | [facebookresearch/eb_jepa](https://github.com/facebookresearch/eb_jepa) |
| [V-JEPA 2.1: Unlocking Dense Features in Video Self-Supervised Learning](https://arxiv.org/abs/2603.14482) | 2603.14482 | [ECCV 2026](https://doi.org/10.1007/978-3-032-37369-4_36) | [facebookresearch/vjepa2](https://github.com/facebookresearch/vjepa2) |
| [Beyond Isotropy in JEPAs: Hamiltonian Geometry and Symplectic Prediction](https://arxiv.org/abs/2605.20107) | 2605.20107 |  | [R02AJ/HamJEPA-HamSIGReg](https://github.com/R02AJ/HamJEPA-HamSIGReg) |
| [A Generalization Theory for JEPA-Based World Models](https://arxiv.org/abs/2606.27014) | 2606.27014 |  |  |
| [Your Probabilistic JEPA Is Secretly a Hidden Markov Model: A State-Space Interpretation of Joint-Embedding Predictive Learning](https://arxiv.org/abs/2608.13621) | 2608.13621 |  | YongchaoHuang/HMM-JEPA (announced, not public yet) |
| [World Model for Energy Efficiency Maximization in Dynamic Metasurface Antennas](https://arxiv.org/abs/2610.35813) | 2610.35813 |  |  |
| [SuperJEPA: Pretraining with a Supervision-Augmented Joint-Embedding Predictive Architecture for High Energy Physics](https://arxiv.org/abs/2610.36121) | 2610.36121 |  |  |
| [Readout and Operating-Point Sensitivity in Event-Stream Candidate Selection](https://arxiv.org/abs/2610.36743) | 2610.36743 |  |  |
| [GUI-JEPA: Candidate-Conditioned JEPA Latents as a Fast Action Policy for Mobile GUI Agents](https://arxiv.org/abs/2610.36877) | 2610.36877 |  | [bcwang-sjtu/GUI-JEPA](https://github.com/bcwang-sjtu/GUI-JEPA) |
| [Vision-Language Agents Can Learn in Their Own Latent Worlds](https://arxiv.org/abs/2610.36925) | 2610.36925 |  | [Tom111-lhx/Dwell](https://github.com/Tom111-lhx/Dwell) |
| [Self-Supervised Latent Action-Conditioned World Modeling for Time Series](https://arxiv.org/abs/2610.37963) | 2610.37963 |  |  |
| [DES-JEPA: Learning a Shared Vocabulary for High-Dimensional Discrete Event Sequences](https://arxiv.org/abs/2610.38445) | 2610.38445 |  |  |
| [Explore Where It Matters: Targeted Exploration for Efficient Rover Adaptation](https://arxiv.org/abs/2610.38657) | 2610.38657 |  |  |
| [Generating Critic-Guided Synthetic Experience in Latent World Models](https://arxiv.org/abs/2610.39100) | 2610.39100 |  |  |
| [Proving and Improving the Platonic Representation Hypothesis with JEPAs](https://arxiv.org/abs/2610.39302) | 2610.39302 |  | [galilai-group/prh-proof](https://github.com/galilai-group/prh-proof)<br>[kmsmohamedansar/prh-jepa](https://github.com/kmsmohamedansar/prh-jepa) (unofficial) |
| [Cheap Retrieval and Observation Credit Assignment from One Quantity: The Value of Information](https://arxiv.org/abs/2610.40030) | 2610.40030 |  |  |
| [Latent Prediction Yields Cross-Subject Alignable Representations in Sensory-Evoked fMRI](https://arxiv.org/abs/2610.40280) | 2610.40280 |  |  |
| [JEDI: Joint-Embedding Demonstration Compression for In-Context Imitation Learning](https://arxiv.org/abs/2610.40356) | 2610.40356 |  |  |
| [Hierarchical World Models with Implicit Dynamics](https://arxiv.org/abs/2610.42146) | 2610.42146 |  | [gaoyuezhou/id_wm](https://github.com/gaoyuezhou/id_wm) |
| [Cross-Domain Joint-Embedding Pretraining For Heterogeneous Industrial Time Series](https://arxiv.org/abs/2611.02489) | 2611.02489 |  |  |
| [Computer-Use Agents Gain Little Benefit from a World Model When Conditioned on Tutorials](https://arxiv.org/abs/2611.04073) | 2611.04073 |  | [realjoenguyen/RAGPJ-official](https://github.com/realjoenguyen/RAGPJ-official) |
| [Ground-Wing: A Parametric 3D Wing-in-Ground-Effect Dataset for Benchmarking Neural Surrogate Models](https://arxiv.org/abs/2611.04571) | 2611.04571 |  |  |
| [Stabilizing Neural Emulation of Spatiotemporal Physical Dynamics through Denoising Koopman Latent Dynamics](https://arxiv.org/abs/2611.04642) | 2611.04642 |  |  |
| [ChangeJEPA: Predict Before You Compare for Remote Sensing Change Detection](https://arxiv.org/abs/2611.05570) | 2611.05570 |  | Buddhi19/ChangeJEPA (announced, not public yet) |
| [Translate, then decide: asymptotic optimality of latent-space control in bistable systems](https://arxiv.org/abs/2611.05736) | 2611.05736 |  |  |
| [Drift-adaptive Representation Preservation for Domain-Incremental Learning](https://arxiv.org/abs/2611.06093) | 2611.06093 |  |  |
| [CAPE-JEPA - Cross-modal Adversarial Probabilistic Embedding JEPA](https://arxiv.org/abs/2611.06247) | 2611.06247 |  |  |
| [GuidedWAM: Training-Free Energy Guidance for World Action Models in Autonomous Driving](https://arxiv.org/abs/2611.07912) | 2611.07912 |  |  |
| [A Stochastic Latent Variable Generalization of Joint-Embedding Predictive Architectures](https://arxiv.org/abs/2611.09302) | 2611.09302 |  | [giakoumoglou/sjepa](https://github.com/giakoumoglou/sjepa) |
| [LO-World: Unified BEV Latent Modeling for Joint 4D Occupancy and LiDAR Forecasting](https://arxiv.org/abs/2611.11912) | 2611.11912 |  | [lzzzzzm/LO-World](https://github.com/lzzzzzm/LO-World) |
| [Benchmarking language models and agents for scientific reasoning in evolving materials laboratories](https://arxiv.org/abs/2611.12014) | 2611.12014 |  |  |
| [Market-Conditioned JEPA: Learning from Unpredictable Market Shocks](https://arxiv.org/abs/2611.13572) | 2611.13572 |  | [OpenFinMind/MC-JEPA](https://github.com/OpenFinMind/MC-JEPA) |
| [An Energy-Based Perspective on Machine Learning](https://arxiv.org/abs/2611.14383) | 2611.14383 |  |  |
| [OnlyAct: Extracting Action Representations from Foundation Models for World Models](https://arxiv.org/abs/2611.14420) | 2611.14420 |  | [runjiali-rl/onlyact](https://github.com/runjiali-rl/onlyact) |
| [RS-JEPA: Remote Sensing Joint-Embedding Predictive Architecture with Scan-Path Views for Cross-Sensor Image Retrieval](https://arxiv.org/abs/2611.14496) | 2611.14496 |  | [Tanishq251/RSJEPA](https://github.com/Tanishq251/RSJEPA) |

## Robotics and aerial applications

World models used on robots, drones, underwater vehicles and in driving, e.g. DINO-WM, SkyJEPA, DroneWAM, AquaJEPA.

| Paper | arXiv | Published | Code |
|---|---|---|---|
| [NeuroBEM: Hybrid Aerodynamic Quadrotor Model](https://arxiv.org/abs/2106.08015) | 2106.08015 | [RSS 2021](https://doi.org/10.15607/RSS.2021.XVII.042) |  |
| [FAST-LIO2: Fast Direct LiDAR-inertial Odometry](https://arxiv.org/abs/2107.06829) | 2107.06829 | [IEEE T-RO 2022](https://doi.org/10.1109/tro.2022.3141876) | [hku-mars/FAST_LIO](https://github.com/hku-mars/FAST_LIO)<br>[p20030920p/SLAM_Learning](https://github.com/p20030920p/SLAM_Learning) (unofficial) |
| [KNODE-MPC: A Knowledge-based Data-driven Predictive Control Framework for Aerial Robots](https://arxiv.org/abs/2109.04821) | 2109.04821 | [IEEE RA-L 2022](https://doi.org/10.1109/LRA.2022.3144787) |  |
| [NTU VIRAL: A Visual-Inertial-Ranging-Lidar Dataset, From an Aerial Vehicle Viewpoint](https://arxiv.org/abs/2202.00379) | 2202.00379 | [IJRR 2021](https://doi.org/10.1177/02783649211052312) |  |
| [Neural-Fly Enables Rapid Learning for Agile Flight in Strong Winds](https://arxiv.org/abs/2205.06908) | 2205.06908 | [Science Robotics 2022](https://doi.org/10.1126/scirobotics.abm6597) | [aerorobotics/neural-fly](https://github.com/aerorobotics/neural-fly) |
| [PL-EVIO: Robust Monocular Event-based Visual Inertial Odometry with Point and Line Features](https://arxiv.org/abs/2209.12160) | 2209.12160 | [IEEE Transactions on Automation Science and Engineering 2024](https://doi.org/10.1109/tase.2023.3324365) |  |
| [ESVIO: Event-based Stereo Visual Inertial Odometry](https://arxiv.org/abs/2212.13184) | 2212.13184 | [IEEE RA-L 2023](https://doi.org/10.1109/lra.2023.3269950) |  |
| [MINS: Efficient and Robust Multisensor-aided Inertial Navigation System](https://arxiv.org/abs/2309.15390) | 2309.15390 | [Journal of Field Robotics 2025](https://doi.org/10.1002/rob.22546) |  |
| [FAST-LIVO2: Fast, Direct LiDAR-Inertial-Visual Odometry](https://arxiv.org/abs/2408.14035) | 2408.14035 | [IEEE T-RO 2025](https://doi.org/10.1109/tro.2024.3502198) | [hku-mars/FAST-LIVO2](https://github.com/hku-mars/FAST-LIVO2) |
| [Swarm-LIO2: Decentralized, Efficient LiDAR-inertial Odometry for UAV Swarms](https://arxiv.org/abs/2409.17798) | 2409.17798 | [IEEE T-RO 2025](https://doi.org/10.1109/tro.2024.3522155) | [hku-mars/Swarm-LIO2](https://github.com/hku-mars/Swarm-LIO2) |
| [DINO-WM: World Models on Pre-trained Visual Features enable Zero-shot Planning](https://arxiv.org/abs/2411.04983) | 2411.04983 | [ICML 2025](https://proceedings.mlr.press/v267/zhou25t.html) | [gaoyuezhou/dino_wm](https://github.com/gaoyuezhou/dino_wm)<br>[liuchangjie7/DINO-WM-Metadrive](https://github.com/liuchangjie7/DINO-WM-Metadrive) (unofficial) |
| [FAST-LIVO2 on Resource-Constrained Platforms: LiDAR-Inertial-Visual Odometry with Efficient Memory and Computation](https://arxiv.org/abs/2501.13876) | 2501.13876 | [IEEE RA-L 2025](https://doi.org/10.1109/lra.2025.3581125) |  |
| [Dream to Fly: Model-Based Reinforcement Learning for Vision-Based Drone Flight](https://arxiv.org/abs/2501.14377) | 2501.14377 | [ICRA 2026](https://doi.org/10.1109/ICRA57385.2026.11695931) |  |
| [Aerial Gym Simulator: A Framework for Highly Parallelized Simulation of Aerial Robots](https://arxiv.org/abs/2503.01471) | 2503.01471 | [IEEE RA-L 2025](https://doi.org/10.1109/lra.2025.3548507) |  |
| [cuVSLAM: CUDA accelerated visual odometry and mapping](https://arxiv.org/abs/2506.04359) | 2506.04359 |  |  |
| [FAST-Calib: LiDAR-Camera Extrinsic Calibration in One Second](https://arxiv.org/abs/2507.17210) | 2507.17210 | [IEEE Robotics and Automation Practice 2026](https://doi.org/10.1109/rap.2026.3692446) | [hku-mars/FAST-Calib](https://github.com/hku-mars/FAST-Calib) |
| [D^2-LIO: Enhanced Optimization for LiDAR-IMU Odometry Considering Directional Degeneracy](https://arxiv.org/abs/2508.14355) | 2508.14355 |  |  |
| [DiffAero: A GPU-Accelerated Differentiable Simulation Framework for Efficient Quadrotor Policy Learning](https://arxiv.org/abs/2509.10247) | 2509.10247 |  | [flyingbitac/diffaero](https://github.com/flyingbitac/diffaero) |
| [Active Inference-Driven World Modeling for Adaptive UAV Swarm Trajectory Design](https://arxiv.org/abs/2601.12939) | 2601.12939 |  |  |
| [Flying by Inference: Active Inference World Models for Adaptive UAV Swarms](https://arxiv.org/abs/2604.27935) | 2604.27935 |  |  |
| [AERO-VIS: Asynchronous Event-based Real-time Onboard Visual-Inertial SLAM](https://arxiv.org/abs/2605.07885) | 2605.07885 | [IEEE RA-L 2026](https://doi.org/10.1109/lra.2026.3726392) |  |
| [MAD: Mapping-Aware World Models for Agile Quadrotor Flight](https://arxiv.org/abs/2606.04534) | 2606.04534 |  |  |
| [SkyJEPA: Learning Long-Horizon World Models for Zero-Shot Sim-to-Real Control of Quadrotors](https://arxiv.org/abs/2606.23444) | 2606.23444 |  |  |
| [Flight-Ready LiDAR-Inertial Odometry for Embedded Drone Platforms](https://arxiv.org/abs/2607.22145) | 2607.22145 |  |  |
| [AquaJEPA: An Action-Conditioned Multimodal JEPA Family for Underwater Robot Dynamics](https://arxiv.org/abs/2607.29393) | 2607.29393 |  |  |
| [JEPLO: Joint-Embedding Predictive Learning for LiDAR-Based Legged Locomotion](https://arxiv.org/abs/2609.15770) | 2609.15770 |  | [ASIG-X/JEPLO](https://github.com/ASIG-X/JEPLO) |
| [DroneWAM: Efficient World Action Model for Drone Visual Navigation](https://arxiv.org/abs/2609.33148) | 2609.33148 |  | [1e12Leon/DroneWAM](https://github.com/1e12Leon/DroneWAM) |
| [AD-E2E-JEPA: A Joint-Embedding Predictive Architecture For End-to-End Autonomous Driving](https://arxiv.org/abs/2609.34085) | 2609.34085 |  | [HaoranZhuExplorer/AD-E2E-JEPA](https://github.com/HaoranZhuExplorer/AD-E2E-JEPA) |
| [RoboJEPA: Scaling Robotic Latent World Models](https://arxiv.org/abs/2610.10515) | 2610.10515 |  | [facebookresearch/robo_jepa](https://github.com/facebookresearch/robo_jepa) |
| [RynnWorld-Latent: A Cross-Embodiment World Model Conditioned on Universal Latent Actions](https://arxiv.org/abs/2610.36791) | 2610.36791 |  | [alibaba-damo-academy/RynnWorld-Latent](https://github.com/alibaba-damo-academy/RynnWorld-Latent) |
| [Neural Compression of Long ADMM Trajectory for Multiparametric Quadratic Program](https://arxiv.org/abs/2610.38079) | 2610.38079 |  | [SOLARIS-JHU/TQPNet](https://github.com/SOLARIS-JHU/TQPNet) |
| [SaiVLA-JEPA: Evaluating Future Latent Prediction in JEPA-Conditioned VLA Control](https://arxiv.org/abs/2610.38508) | 2610.38508 |  |  |
| [OpenFlyV2: An onboard vision-language-action model for aerial perception and navigation](https://arxiv.org/abs/2610.39287) | 2610.39287 |  | [Ideal-ljl/AeroBrain](https://github.com/Ideal-ljl/AeroBrain) |
| [Continuous-Action World Models: Learning Cross-Embodiment Spatiotemporal Dynamics Priors](https://arxiv.org/abs/2610.40401) | 2610.40401 |  |  |
| [OpenNWM: A Generalist Navigation World Model with Latent Action Pretraining](https://arxiv.org/abs/2611.01844) | 2611.01844 |  | [OpenSpace-Lab/OpenNWM](https://github.com/OpenSpace-Lab/OpenNWM) |
| [MKD2World: A Typed Spatial MarkDown World Model For Web Agents](https://arxiv.org/abs/2611.06544) | 2611.06544 |  | [OmniAI-Lab-CUHKSZ/MKD2World](https://github.com/OmniAI-Lab-CUHKSZ/MKD2World) |
| [Motion-guided Contrastive Regularization For Latent World Models](https://arxiv.org/abs/2611.06901) | 2611.06901 |  |  |
| [PlayGen2: Learning Real-Time Playable Worlds with Explicit 3D State](https://arxiv.org/abs/2611.07867) | 2611.07867 |  | [MajorDavidZhang/PlayGen-2](https://github.com/MajorDavidZhang/PlayGen-2) |
| [GPWM: Modeling the World as 3D Particle Motion](https://arxiv.org/abs/2611.08338) | 2611.08338 |  |  |
| [Extended Model-Based Learned Inertial Odometry](https://arxiv.org/abs/2611.09584) | 2611.09584 | [ICUAS 2026](https://doi.org/10.1109/ICUAS69441.2026.11598619) | [SasaKuruppuarachchi/Ex-IMO](https://github.com/SasaKuruppuarachchi/Ex-IMO) |
| [WorldFoundry: Towards Unified Infrastructure for World Intelligence](https://arxiv.org/abs/2611.10771) | 2611.10771 |  | [OpenEnvision/WorldFoundry](https://github.com/OpenEnvision/WorldFoundry) |
| [ScanDreamer: A Map-Grounded World Model for Quadrotor Navigation](https://arxiv.org/abs/2611.11605) | 2611.11605 |  | [WANGSHUAIzzzz/ScanDreamer](https://github.com/WANGSHUAIzzzz/ScanDreamer) |
| [Action Representation for Spatial Generalization in Robot World Models](https://arxiv.org/abs/2611.11869) | 2611.11869 |  |  |
| [Compass 1: Towards Open-World and Persistent Embodied Navigation from Monocular RGB Videos](https://arxiv.org/abs/2611.12087) | 2611.12087 |  | [OpenDriveLab/Compass](https://github.com/OpenDriveLab/Compass) |
| [DeRep: Learning Depth Representations for End-to-End Navigation in Cluttered Environments](https://arxiv.org/abs/2611.13499) | 2611.13499 |  |  |

## Action-conditioned models and planning

Models that predict the effect of actions and are used for planning or policy learning: LeWorldModel, PLDM, hierarchical and goal-conditioned planners, VLA models, evaluation and robustness studies.

| Paper | arXiv | Published | Code |
|---|---|---|---|
| [Navigation World Models](https://arxiv.org/abs/2412.03572) | 2412.03572 | [CVPR 2025](https://doi.org/10.1109/cvpr52734.2025.01472) | [facebookresearch/nwm](https://github.com/facebookresearch/nwm) |
| [ACT-JEPA: Novel Joint-Embedding Predictive Architecture for Efficient Policy Representation Learning](https://arxiv.org/abs/2501.14622) | 2501.14622 | [IEEE Access 2026](https://doi.org/10.1109/ACCESS.2026.3696039) | [act-jepa/act-jepa](https://github.com/act-jepa/act-jepa) |
| [Generalizing Safety Beyond Collision-Avoidance via Latent-Space Reachability Analysis](https://arxiv.org/abs/2502.00935) | 2502.00935 | [RSS 2025](https://doi.org/10.15607/rss.2025.xxi.113) |  |
| [Learning from Reward-Free Offline Data: A Case for Planning with Latent Dynamics Models](https://arxiv.org/abs/2502.14819) | 2502.14819 | [NeurIPS 2025](https://doi.org/10.52202/085713-1465) | [vladisai/PLDM](https://github.com/vladisai/PLDM) |
| [AdaWorld: Learning Adaptable World Models with Latent Actions](https://arxiv.org/abs/2503.18938) | 2503.18938 |  | [Little-Podi/AdaWorld](https://github.com/Little-Podi/AdaWorld) |
| [Uncertainty-aware Latent Safety Filters for Avoiding Out-of-Distribution Failures](https://arxiv.org/abs/2505.00779) | 2505.00779 |  |  |
| [Back to the Features: DINO as a Foundation for Video World Models](https://arxiv.org/abs/2507.19468) | 2507.19468 |  |  |
| [AnySafe: Adapting Latent Safety Filters at Runtime via Safety Constraint Parameterization in the Latent Space](https://arxiv.org/abs/2509.19555) | 2509.19555 | [ICRA 2026](https://doi.org/10.1109/icra57385.2026.11696562) |  |
| [How Well Do Latent World Models Understand Partially Observable Safety Constraints?](https://arxiv.org/abs/2510.06492) | 2510.06492 | CoRL 2026 (accepted) |  |
| [What Drives Success in Physical Planning with Joint-Embedding Predictive World Models?](https://arxiv.org/abs/2512.24497) | 2512.24497 | TMLR 2025 | [facebookresearch/jepa-wms](https://github.com/facebookresearch/jepa-wms) |
| [Value-guided action planning with JEPA world models](https://arxiv.org/abs/2601.00844) | 2601.00844 |  |  |
| [VLA-JEPA: Enhancing Vision-Language-Action Model with Latent World Model](https://arxiv.org/abs/2602.10098) | 2602.10098 | [ECCV 2026](https://doi.org/10.1007/978-3-032-37196-6_26) | [ginwind/VLA-JEPA](https://github.com/ginwind/VLA-JEPA)<br>[AmoghShrivastava/vlaJEPA](https://github.com/AmoghShrivastava/vlaJEPA) (unofficial) |
| [JEPA-Bisim: Learning Robust Visual Representations for Planning with Joint-Embedding Predictive World Models](https://arxiv.org/abs/2602.18639) | 2602.18639 |  | [jd-anderson/dino_bsmpc](https://github.com/jd-anderson/dino_bsmpc) |
| [LeWorldModel: Stable End-to-End Joint-Embedding Predictive Architecture from Pixels](https://arxiv.org/abs/2603.19312) | 2603.19312 |  | [lucas-maes/le-wm](https://github.com/lucas-maes/le-wm)<br>[gandhiashutosh14/lewm-t4](https://github.com/gandhiashutosh14/lewm-t4) (unofficial) |
| [Hierarchical Planning with Latent World Models](https://arxiv.org/abs/2604.03208) | 2604.03208 | CoRL 2026 (accepted) | [kevinghst/HWM_PLDM](https://github.com/kevinghst/HWM_PLDM) |
| [ELVIS: Ensemble-Calibrated Latent Imagination for Long-Horizon Visual MPC](https://arxiv.org/abs/2605.04709) | 2605.04709 |  |  |
| [PLUME: Probabilistic Latent Unified World Modeling and Parameter Estimation for Multi-Finger Manipulation](https://arxiv.org/abs/2606.11396) | 2606.11396 |  |  |
| [Delta-JEPA: Learning Action-Sensitive World Models via Latent Difference Decoding](https://arxiv.org/abs/2606.31232) | 2606.31232 |  |  |
| [Temporal-Distance JEPA: Plan-Aware Representation Learning for Latent World Model Predictive Control](https://arxiv.org/abs/2607.25337) | 2607.25337 |  | [HKBU-KnowComp/Temporal-Distance-JEPA](https://github.com/HKBU-KnowComp/Temporal-Distance-JEPA) |
| [JEPA-WAM: Learning Vision-Language-Action Policies with Joint-Embedding World Modeling](https://arxiv.org/abs/2608.09381) | 2608.09381 |  | [SpriteWithoutIce/JEPA_WAM](https://github.com/SpriteWithoutIce/JEPA_WAM) |
| [StageWAM: Joint-Embedding Stage Prediction for World-Action Models in Robot Manipulation](https://arxiv.org/abs/2608.10780) | 2608.10780 |  |  |
| [Diagnosing JEPA World Models with Action-Conditioned Predictive Consistency](https://arxiv.org/abs/2608.12939) | 2608.12939 |  | [Anguo-star/acpc-diagnostics](https://github.com/Anguo-star/acpc-diagnostics) |
| [SCALE: State-Calibrated Latent Embeddings for JEPA Planning in the Right Geometry](https://arxiv.org/abs/2608.16287) | 2608.16287 |  |  |
| [No Gaussian Required: Contrastive Inverse Dynamics for JEPA World Models](https://arxiv.org/abs/2608.17542) | 2608.17542 |  | [jackboyla/action-contrastive-jepa](https://github.com/jackboyla/action-contrastive-jepa) |
| [Toward Physically Grounded JEPA World Models for Goal-Conditioned Robotic Planning](https://arxiv.org/abs/2609.03565) | 2609.03565 | IROS 2026 Workshop | [zsibot/gawm](https://github.com/zsibot/gawm) |
| [D-JEPA: A Decision-Aligned Latent World Model](https://arxiv.org/abs/2609.24749) | 2609.24749 |  | [NEBULIS-Lab/D-JEPA](https://github.com/NEBULIS-Lab/D-JEPA) |
| [CF-JEPA: Improving Robustness of JEPA World Models via Controllability Factorization](https://arxiv.org/abs/2610.00727) | 2610.00727 |  |  |
| [TwinJEPA: Action-Preferred Predictive Representations for Goal-Conditioned Control](https://arxiv.org/abs/2610.02922) | 2610.02922 |  | [NICE-HKU/Twin-JEPA](https://github.com/NICE-HKU/Twin-JEPA) |
| [H-JEPA: End-to-End Learning of Hierarchical World Models for Visual Planning](https://arxiv.org/abs/2610.06805) | 2610.06805 |  | [kevinghst/H-JEPA](https://github.com/kevinghst/H-JEPA)<br>[zuiailaoyouji/H-JEPA-reproduction](https://github.com/zuiailaoyouji/H-JEPA-reproduction) (unofficial) |
| [A Belief-State World Model for Catheter Navigation under Sparse Fluoroscopy: A Planar Proof of Concept](https://arxiv.org/abs/2610.08469) | 2610.08469 |  |  |
| [LeWAM: End-to-End World and Action Modeling with JEPAs](https://arxiv.org/abs/2610.12818) | 2610.12818 |  | [MinghaoFu/lewam](https://github.com/MinghaoFu/lewam) |
| [Adapt for Planning, Not just Prediction: Optimistic Test-Time World Model Adaptation](https://arxiv.org/abs/2610.35636) | 2610.35636 | CoRL 2026 Workshop | [akshaymete/optta](https://github.com/akshaymete/optta) |
| [Cinematize from Unreal: Agentic Choreography for Controllable World Simulation](https://arxiv.org/abs/2610.38468) | 2610.38468 |  |  |
| [Structural-Test Geometry as an Inductive Bias for Partially Observable World Models](https://arxiv.org/abs/2610.38903) | 2610.38903 |  |  |
| [Agentic LinkDreamer: Adaptive Neuro-Fuzzy World-Model Decision Making for Intermittent V2X Cooperative Perception](https://arxiv.org/abs/2610.39258) | 2610.39258 |  |  |
| [PRIME W0: Physical Priors from World Models for Embodied Manipulation](https://arxiv.org/abs/2610.39528) | 2610.39528 |  |  |
| [world2vec: Mechanistic world models through latent dynamics learning](https://arxiv.org/abs/2610.40637) | 2610.40637 |  |  |
| [One Verdict Is Not Enough: Regression Testing Learned World Models and Their Test Harnesses](https://arxiv.org/abs/2610.41130) | 2610.41130 |  |  |
| [Online Learning of Heterogeneous Locomotion Dynamics under Reinforcement Learning Policies for Precise Loco-Manipulation](https://arxiv.org/abs/2610.41892) | 2610.41892 |  |  |
| [Spoofing the Latent State: Imperceptible Goal-Image Attacks Derail Planning in LeWorldModel](https://arxiv.org/abs/2611.00427) | 2611.00427 |  |  |
| [SCOUT: Planning under Occlusion via Object-Centric World Model Rollouts](https://arxiv.org/abs/2611.01600) | 2611.01600 |  |  |
| [Compression Forcing: Hierarchical History Tokenization Enables Flexible World Models](https://arxiv.org/abs/2611.04028) | 2611.04028 |  |  |
| [Time-to-Goal: Learned Temporal Metrics for Long-Horizon Planning with JEPA World Models](https://arxiv.org/abs/2611.05847) | 2611.05847 |  | [yrluestc/T2G-JEPA](https://github.com/yrluestc/T2G-JEPA) |
| [MAC-v2: Long-horizon model-based value expansion from pixels](https://arxiv.org/abs/2611.07245) | 2611.07245 |  |  |
| [Learning Robotic World Models with Semantic and Visual Feedback](https://arxiv.org/abs/2611.07850) | 2611.07850 |  | [Alexander-wu/RoboImagine](https://github.com/Alexander-wu/RoboImagine) |
| [La-JEPA: Compact Robot Policies with Latent World Modeling](https://arxiv.org/abs/2611.08156) | 2611.08156 |  | [mt-clemente/lajepa](https://github.com/mt-clemente/lajepa) |
| [Dynamics-Informed Action Learning for Goal-Conditioned Latent Planning](https://arxiv.org/abs/2611.10660) | 2611.10660 |  |  |
| [WARP-JEPA: World-Model-in-the-Loop Amortized Rollout Planning for Frozen Hierarchical Joint-Embedding Predictive Architectures](https://arxiv.org/abs/2611.10806) | 2611.10806 |  | [hideinsewer/WARP-JEPA](https://github.com/hideinsewer/WARP-JEPA) |
| [K-PWM: Control-Oriented Structured Bilinear World Models under Partial Observation](https://arxiv.org/abs/2611.11521) | 2611.11521 | NeurIPS 2026 (accepted) | [santoshrajkumar/k-pwm-world-model-control](https://github.com/santoshrajkumar/k-pwm-world-model-control) |
| [Planners Exploit Deterministic Error: Dithered Low-Bit World Models](https://arxiv.org/abs/2611.11780) | 2611.11780 |  |  |
| [How Many Candidates Does a One-Step World Model Need? A Random-Codebook Account of Nearest-of-m Training on Frozen DINO Tokens](https://arxiv.org/abs/2611.11887) | 2611.11887 |  |  |
| [An Evaluation of Tabular Foundation Models as Training-Free World Models](https://arxiv.org/abs/2611.11921) | 2611.11921 |  |  |
| [Σ-LeWM: Learning World Models via S-Information for Robot Control](https://arxiv.org/abs/2611.12732) | 2611.12732 |  | [zuxinrui/sigma-lewm](https://github.com/zuxinrui/sigma-lewm) |
| [Building World Models from Intrinsic Motivation](https://arxiv.org/abs/2611.13113) | 2611.13113 |  |  |
| [Few-Shot Residual Adaptation of Pretrained Latent World Models](https://arxiv.org/abs/2611.13592) | 2611.13592 |  |  |

## Latent dynamics, physics structure and theory

Structured latent dynamics (Hamiltonian, symplectic, Koopman, bilinear, semigroup), probabilistic JEPAs, collapse and identifiability analyses.

| Paper | arXiv | Published | Code |
|---|---|---|---|
| [Hamiltonian Neural Networks](https://arxiv.org/abs/1906.01563) | 1906.01563 | NeurIPS 2019 | [greydanus/hamiltonian-nn](https://github.com/greydanus/hamiltonian-nn)<br>[DarioPenagos/Hamiltonian-Neural-Networks](https://github.com/DarioPenagos/Hamiltonian-Neural-Networks) (unofficial)<br>[a-b-h-a-y-s-h-i-n-d-e/Hamiltonian_Neural_Network](https://github.com/a-b-h-a-y-s-h-i-n-d-e/Hamiltonian_Neural_Network) (unofficial) |
| [LagNetViP: A Lagrangian Neural Network for Video Prediction](https://arxiv.org/abs/2010.12932) | 2010.12932 |  |  |
| [Robust and Safe Autonomous Navigation for Systems with Learned SE(3) Hamiltonian Dynamics](https://arxiv.org/abs/2207.10840) | 2207.10840 | [IEEE Open Journal of Control Systems 2022](https://doi.org/10.1109/OJCSYS.2022.3201554) |  |
| [Uncertainty Representations in State-Space Layers for Deep Reinforcement Learning under Partial Observability](https://arxiv.org/abs/2409.16824) | 2409.16824 |  |  |
| [Learning Hamiltonian Dynamics with Bayesian Data Assimilation](https://arxiv.org/abs/2501.18808) | 2501.18808 |  |  |
| [KILO-EKF: Koopman-Inspired Learned Observations Extended Kalman Filter](https://arxiv.org/abs/2601.12463) | 2601.12463 |  |  |
| [VJEPA: Variational Joint Embedding Predictive Architectures as Probabilistic World Models](https://arxiv.org/abs/2601.14354) | 2601.14354 | [ICML 2026](https://icml.cc/virtual/2026/poster/61579) | [YongchaoHuang/VJEPA](https://github.com/YongchaoHuang/VJEPA) |
| [From Gradients to Riccati Geometry: Kalman World Models for Single-Pass Learning](https://arxiv.org/abs/2603.13423) | 2603.13423 |  |  |
| [Latent State Design for World Models under Sufficiency Constraints](https://arxiv.org/abs/2605.01694) | 2605.01694 |  |  |
| [HaM-World: Soft-Hamiltonian World Models with Selective Memory for Planning](https://arxiv.org/abs/2605.05951) | 2605.05951 | NeurIPS 2026 (accepted) | [HaoyunT/HaM_World](https://github.com/HaoyunT/HaM_World) |
| [Phys-JEPA: Physics-Informed Latent World Models for Multivariate Time-Series Forecasting](https://arxiv.org/abs/2606.16076) | 2606.16076 |  |  |
| [A Control Theory of Predictability in Latent World Models](https://arxiv.org/abs/2607.10362) | 2607.10362 |  |  |
| [Toward Goal-Agnostic Joint-Embedding Predictive Control of Partial Differential Equations](https://arxiv.org/abs/2607.21644) | 2607.21644 |  |  |
| [SJEPA: Learning Elegant Latent Dynamics with Hybrid Symbolic-Neural Predictors](https://arxiv.org/abs/2608.04060) | 2608.04060 |  |  |
| [PhyLatent: Learning Dynamics-Relevant Representations for JEPA World Models](https://arxiv.org/abs/2608.05720) | 2608.05720 |  | [Cherishings/PhyLatent](https://github.com/Cherishings/PhyLatent) |
| [Is Forward Prediction Enough? Physical State Grounding for JEPA World Models](https://arxiv.org/abs/2608.06799) | 2608.06799 |  | [Haodong-Yan/PSG-JEPA](https://github.com/Haodong-Yan/PSG-JEPA) |
| [JEPA-x: Cross-Predictive Physics Grounding for Forecastable Latent Dynamics](https://arxiv.org/abs/2608.24044) | 2608.24044 |  | [wkh923/jepa-x](https://github.com/wkh923/jepa-x) |
| [Flow-JEPA: Robust Latent Dynamics for JEPA World Models via Flow Matching](https://arxiv.org/abs/2608.29029) | 2608.29029 |  | [HuoYanchen/Flow-JEPA](https://github.com/HuoYanchen/Flow-JEPA) |
| [Semigroup-JEPA: Latent Dynamics Consistency for Zero-Shot Physics Generalization](https://arxiv.org/abs/2609.10464) | 2609.10464 |  |  |
| [I Act Therefore I Am: When Is JEPA's Action-Conditioning Enough to Learn Causal Mechanisms?](https://arxiv.org/abs/2609.31161) | 2609.31161 |  |  |
| [D-JEPA: Design-Recoverable JEPA Representation with Swappable Physics Decoders](https://arxiv.org/abs/2609.33110) | 2609.33110 |  |  |
| [Hamiltonian JEPA: Action-Conditioned World Models with an Inherited Control State](https://arxiv.org/abs/2609.33497) | 2609.33497 |  | [tmz-lab/hjepa](https://github.com/tmz-lab/hjepa) |
| [Bilinear World Models: Learning Representations with Structured Dynamics for Efficient Control](https://arxiv.org/abs/2609.36305) | 2609.36305 |  |  |
| [JEPA-TTT: Persistent Test-Time Training of Latent World Models for Planning under Dynamics Shifts](https://arxiv.org/abs/2610.00722) | 2610.00722 | NeurIPS 2026 Workshop on World Models in Physical AI |  |
| [AVL-JEPA: Preventing Causal Dynamics Information Collapse In Joint Embedding Predictive Architecture World Models](https://arxiv.org/abs/2610.03587) | 2610.03587 |  |  |
| [Frozen in a Frame: The Velocity Blind Spot in JEPA World Models](https://arxiv.org/abs/2610.04585) | 2610.04585 |  | [OliverZ-dot/TI-JEPA](https://github.com/OliverZ-dot/TI-JEPA) |
| [Preserving Unstable Modes Through Inverse Dynamics in JEPA World Models](https://arxiv.org/abs/2610.07540) | 2610.07540 |  | [LeoToso/JEPA_control](https://github.com/LeoToso/JEPA_control) |
| [MDN-VJEPA: Multimodal Probabilistic Joint-Embedding World Models](https://arxiv.org/abs/2610.13956) | 2610.13956 |  |  |
| [LeHami: Symplectic Latent Dynamics for World Models](https://arxiv.org/abs/2610.15267) | 2610.15267 |  | [rominay/LeHami](https://github.com/rominay/LeHami) |
| [DriveUniTok: A Unified Multimodal Tokenizer for Driving World-Action Models](https://arxiv.org/abs/2610.35044) | 2610.35044 |  |  |
| [Multi-Horizon Future Discovery for Physics-Informed Exploration](https://arxiv.org/abs/2610.35468) | 2610.35468 |  |  |
| [E0.5: From Reconstructive to Future-Predictive 3D Foundations for Robotic World-Action Modeling](https://arxiv.org/abs/2610.36011) | 2610.36011 |  |  |
| [AC-JEPA: Anchored Cross-Modal Joint Embedding Predictive Architecture for Visual-to-Symbolic Translation](https://arxiv.org/abs/2610.36493) | 2610.36493 |  |  |
| [SWIM: Learning What Matters from Behaviors for JEPA World Models](https://arxiv.org/abs/2610.36662) | 2610.36662 |  |  |
| [WorldFlow: Joint Video and 3D Motion Prediction via Large-Scale Pretraining](https://arxiv.org/abs/2610.39278) | 2610.39278 |  | [worldflow-rbs/worldflow](https://github.com/worldflow-rbs/worldflow) |
| [Bayesian Offline Multi-Agent Reinforcement Learning with Latent World Models](https://arxiv.org/abs/2610.39576) | 2610.39576 |  |  |
| [Learning momenta for Hamiltonian-based models](https://arxiv.org/abs/2611.01269) | 2611.01269 |  |  |
| [Identifiable Signed Causal Learning via Latent Stochastic Differential Equations for Inferring Brain Dynamic Effective Connectivity](https://arxiv.org/abs/2611.02876) | 2611.02876 |  | [Yiding00/ISCL](https://github.com/Yiding00/ISCL) |
| [ForceLDM: A Force-aware Latent Dynamics Model for Contact-Rich Manipulation](https://arxiv.org/abs/2611.03294) | 2611.03294 |  |  |
| [Embodied AI for Scientific Discovery: From Physical Action to Scientific Evidence](https://arxiv.org/abs/2611.04371) | 2611.04371 |  |  |
| [Comparing model representations and fitting methods for port-Hamiltonian system identification](https://arxiv.org/abs/2611.05031) | 2611.05031 |  | [SINTEF/PHSI](https://github.com/SINTEF/PHSI) |
| [SO(3)-Equivariant Learning on CAD Boundary Representations](https://arxiv.org/abs/2611.05449) | 2611.05449 |  | [UGent-CVAMO/so3brep](https://github.com/UGent-CVAMO/so3brep) |
| [Readable Is Not Steerable: Pre-Registered Tests of Physical Structure in Learned Fluid Representations](https://arxiv.org/abs/2611.05577) | 2611.05577 |  | [2025eb1100268-tech/readable-not-steerable](https://github.com/2025eb1100268-tech/readable-not-steerable) |
| [Dynamic Watermarking and Action-Conditioned Latent Dynamics for Secure Vision-Based Controllers](https://arxiv.org/abs/2611.07403) | 2611.07403 |  |  |
| [Equivariant Deep Learning in Direct-Product Space for Electronic-Structure Hamiltonian Prediction](https://arxiv.org/abs/2611.07695) | 2611.07695 |  |  |
| [Learning a patient world model for health system simulation in intensive care](https://arxiv.org/abs/2611.08392) | 2611.08392 |  |  |
| [Stochastic Port-Hamiltonian Gaussian Processes for Learning from Noisy Dynamics on Lie Groups](https://arxiv.org/abs/2611.10864) | 2611.10864 |  | [CVC-Lab/LieSPHGP](https://github.com/CVC-Lab/LieSPHGP) |
| [SurgWorld: Learning Surgical Representations Beyond Observation via Latent Prediction](https://arxiv.org/abs/2611.11140) | 2611.11140 |  |  |
| [DeepSoMo: Deformable Object Motion Estimation under Proprioceptive Partial Observability via Predictive Latent Dynamics](https://arxiv.org/abs/2611.11242) | 2611.11242 |  |  |
| [Good Views Are Not Enough: Global Counterexamples for Gaussian-Regularized JEPAs](https://arxiv.org/abs/2611.12137) | 2611.12137 |  |  |
| [ProTEUS: A mutation-resolved world model for closed-loop protein evolution](https://arxiv.org/abs/2611.13348) | 2611.13348 |  | [yikunpku/ProTEUS](https://github.com/yikunpku/ProTEUS) |
| [Evaluating LLM-Generated World Models for Neuro-Symbolic Reasoning](https://arxiv.org/abs/2611.14419) | 2611.14419 |  |  |

## 3D, spatial and object-centric models

Point-cloud, depth, LiDAR, 3D-scene, object-centric and graph-structured predictive models.

| Paper | arXiv | Published | Code |
|---|---|---|---|
| [Structured World Belief for Reinforcement Learning in POMDP](https://arxiv.org/abs/2107.08577) | 2107.08577 |  |  |
| [Point-JEPA: A Joint Embedding Predictive Architecture for Self-Supervised Learning on Point Cloud](https://arxiv.org/abs/2404.16432) | 2404.16432 | [WACV 2025](https://doi.org/10.1109/WACV61041.2025.00714) | [Ayumu-J-S/Point-JEPA](https://github.com/Ayumu-J-S/Point-JEPA) |
| [3D-JEPA: A Joint Embedding Predictive Architecture for 3D Self-Supervised Representation Learning](https://arxiv.org/abs/2409.15803) | 2409.15803 |  |  |
| [PlaySlot: Learning Inverse Latent Dynamics for Controllable Object-Centric Video Prediction and Planning](https://arxiv.org/abs/2502.07600) | 2502.07600 |  |  |
| [POMA-3D: The Point Map Way to 3D Scene Understanding](https://arxiv.org/abs/2511.16567) | 2511.16567 | [CVPR Findings 2026](https://doi.org/10.1109/CVPRF71909.2026.00699) |  |
| [CrossJEPA: Cross-Modal Joint-Embedding Predictive Architecture for Efficient 3D Representation Learning from 2D Images](https://arxiv.org/abs/2511.18424) | 2511.18424 |  |  |
| [Semantic Belief-State World Model for 3D Human Motion Prediction](https://arxiv.org/abs/2601.03517) | 2601.03517 |  |  |
| [Causal-JEPA: Learning World Models through Object-Level Latent Masking](https://arxiv.org/abs/2602.11389) | 2602.11389 | ICML 2026 | [galilai-group/cjepa](https://github.com/galilai-group/cjepa)<br>[Maverick-Ansh/causal-jepa-repro](https://github.com/Maverick-Ansh/causal-jepa-repro) (unofficial) |
| [Self-Supervised JEPA-based World Models for LiDAR Occupancy Completion and Forecasting](https://arxiv.org/abs/2602.12540) | 2602.12540 |  |  |
| [Le MuMo JEPA: Multi-Modal Self-Supervised Representation Learning with Learnable Fusion Tokens](https://arxiv.org/abs/2603.24327) | 2603.24327 |  | [ciemcornelissen/le-mumo-jepa](https://github.com/ciemcornelissen/le-mumo-jepa) |
| [UWM-JEPA: Predictive World Models That Imagine in Belief Space](https://arxiv.org/abs/2605.25313) | 2605.25313 |  | [santoshkumarradha/uwm-jepa](https://github.com/santoshkumarradha/uwm-jepa) |
| [Neural Voxel Dynamics: Learning Volumetric Feature Advection for 3D Physics in V-JEPA Latent Space](https://arxiv.org/abs/2606.26410) | 2606.26410 |  |  |
| [J-LAW: Joint Localization and Action-Conditioned World Modeling via Coupled Latent Factor Graphs](https://arxiv.org/abs/2606.28712) | 2606.28712 |  |  |
| [JEPADepth: Masked Predictive Representation Learning for Self-Supervised Monocular Depth Estimation](https://arxiv.org/abs/2607.26600) | 2607.26600 |  | [ionut-grigore99/JEPADepth](https://github.com/ionut-grigore99/JEPADepth) |
| [SR-JEPA: Learning Predictive Latent State in 3D Scenes](https://arxiv.org/abs/2608.05774) | 2608.05774 |  |  |
| [Does Latent Planning Survive Point Clouds? Action-Conditioned JEPA World Models for Geometric Observations and Goals](https://arxiv.org/abs/2608.29434) | 2608.29434 |  | [fafraob/point-lewm](https://github.com/fafraob/point-lewm) |
| [MotionJEPA: Preventing Temporal Feature Collapse by Capturing Visual Changes in Latent Space](https://arxiv.org/abs/2609.23881) | 2609.23881 |  | [mkarmann/motion-jepa](https://github.com/mkarmann/motion-jepa) |
| [4DGS-JEPA: Temporally Compositional Joint-Embedding Prediction for Dynamic Gaussian Splatting](https://arxiv.org/abs/2609.25036) | 2609.25036 |  | [Hongyang-Du/4DGS-JEPA](https://github.com/Hongyang-Du/4DGS-JEPA) (unofficial) |
| [BeliefGraph-JEPA: Structured Latent World Models for Action-Conditioned Time Series](https://arxiv.org/abs/2610.05409) | 2610.05409 |  |  |
| [GAWM: A Compact Latent World-Action Model for Multi-Task Robot Manipulation](https://arxiv.org/abs/2610.37091) | 2610.37091 |  | [gaoxiang12/ga-wm](https://github.com/gaoxiang12/ga-wm) |
| [JEPA-Inspired Latent Field Prediction for Sparse-Pilot MIMO-OFDM Channel Reconstruction](https://arxiv.org/abs/2610.37391) | 2610.37391 |  |  |
| [Representing the Unseen: Rethinking Visual Imagination for Spatial Reasoning](https://arxiv.org/abs/2610.37437) | 2610.37437 |  |  |
| [Understanding the limits of latent world models](https://arxiv.org/abs/2610.37588) | 2610.37588 |  | [dynamical-inference/faithful-world-models](https://github.com/dynamical-inference/faithful-world-models) |
| [Seeing and Imagining as One: Unified Video Generation and 4D Perception for Embodied World Modeling](https://arxiv.org/abs/2610.39232) | 2610.39232 |  | [gensight-rbs/gensight](https://github.com/gensight-rbs/gensight) |
| [GROME: GROunding Factorized MEmory into Video World Models](https://arxiv.org/abs/2610.39812) | 2610.39812 |  |  |
| [HiFOR: Hierarchical Foresight with Action-Guided World Grounding for Vision-Language-Action Model](https://arxiv.org/abs/2610.40373) | 2610.40373 |  |  |
| [Fight World Model: Customizable Combat through Visual Interaction Proxies](https://arxiv.org/abs/2610.40607) | 2610.40607 |  | [fight-world-model/FWM](https://github.com/fight-world-model/FWM) |
| [L3G-World: Real-Time Infinite World Generation with Latent 3D Gaussian Memory](https://arxiv.org/abs/2610.40614) | 2610.40614 |  | [cvlab-kaist/L3G-World](https://github.com/cvlab-kaist/L3G-World) |
| [Xiaomi Auto World Model 2.0: Causal World Models for Real-World Driving and Embodied Intelligence](https://arxiv.org/abs/2611.01677) | 2611.01677 |  |  |
| [AgiWorld: An Agentic Video World Model for Building Persistent Worlds](https://arxiv.org/abs/2611.02341) | 2611.02341 |  |  |
| [INTERACT: Learning Interaction-Aware World Dynamics from Driving Videos for Autonomous Driving](https://arxiv.org/abs/2611.02526) | 2611.02526 |  |  |
| [FlowBench: Counterfactual Imagination Training for Spatial Intelligence](https://arxiv.org/abs/2611.03937) | 2611.03937 |  | [liuyifan22/FlowBench](https://github.com/liuyifan22/FlowBench) |
| [Physical Experience Builds Continual Spatial World Models](https://arxiv.org/abs/2611.04016) | 2611.04016 |  |  |
| [Hybrid Particle-Voxel Dynamics for Multimodal 3D World Simulation](https://arxiv.org/abs/2611.04492) | 2611.04492 |  |  |
| [Trajectory Evaluation via Rollout-Free World Model for End-to-end Autonomous Driving](https://arxiv.org/abs/2611.05072) | 2611.05072 |  | [Rupertail/RFWorld](https://github.com/Rupertail/RFWorld) |
| [TouchéWorld tech report : Towards Online Unified Camera--Hand Exploration in Generative Worlds](https://arxiv.org/abs/2611.06061) | 2611.06061 |  | [yjainqdc/ToucheWorld](https://github.com/yjainqdc/ToucheWorld) |
| [GEKey: Learning Geodesic Eccentric 3D Keypoints via Self-Supervision](https://arxiv.org/abs/2611.07677) | 2611.07677 |  | [Pierreoo/GEKey](https://github.com/Pierreoo/GEKey) |
| [ObjectWorld: Scaling Object-Centric World Models with A Large-Scale 3D Full-Object Flow Dataset](https://arxiv.org/abs/2611.11085) | 2611.11085 |  |  |
| [DexForesight: Grounding Dexterous Policies with Implicit Spatial Foresight](https://arxiv.org/abs/2611.11166) | 2611.11166 |  |  |
| [ForeAct: Geometry-Guided Action Learning from World Representations](https://arxiv.org/abs/2611.11500) | 2611.11500 |  | [Bulrush666/ForeAct](https://github.com/Bulrush666/ForeAct) |
| [QCC-WM: Linking Macro-State Dynamics and Visual Generation via Quotient Causal Construction](https://arxiv.org/abs/2611.12353) | 2611.12353 |  |  |
| [LaST0.5: A Generalist World Action Model with Interaction-Centric Latent Reasoning](https://arxiv.org/abs/2611.14048) | 2611.14048 |  |  |
| [From Video Frames to Robot Meta-Frames: A Unified Latent Interface for World Action Models](https://arxiv.org/abs/2611.14365) | 2611.14365 |  | [showlab/MetaWAM](https://github.com/showlab/MetaWAM) |

## Related non-JEPA world models

Reconstruction-based and Dreamer-style latent world models (World Models, Dreamer V1–V4, DayDreamer), including physics-structured variants, kept for comparison.

| Paper | arXiv | Published | Code |
|---|---|---|---|
| [World Models](https://arxiv.org/abs/1803.10122) | 1803.10122 |  | [hardmaru/WorldModelsExperiments](https://github.com/hardmaru/WorldModelsExperiments)<br>[AppliedDataSciencePartners/WorldModels](https://github.com/AppliedDataSciencePartners/WorldModels) (unofficial) |
| [Recurrent World Models Facilitate Policy Evolution](https://arxiv.org/abs/1809.01999) | 1809.01999 | NeurIPS 2018 | [hardmaru/WorldModelsExperiments](https://github.com/hardmaru/WorldModelsExperiments) |
| [Learning Latent Dynamics for Planning from Pixels](https://arxiv.org/abs/1811.04551) | 1811.04551 | [ICML 2019](https://proceedings.mlr.press/v97/hafner19a.html) | [google-research/planet](https://github.com/google-research/planet)<br>[cross32768/PlaNet_PyTorch](https://github.com/cross32768/PlaNet_PyTorch) (unofficial) |
| [Dream to Control: Learning Behaviors by Latent Imagination](https://arxiv.org/abs/1912.01603) | 1912.01603 | ICLR 2020 | [danijar/dreamer](https://github.com/danijar/dreamer)<br>[cross32768/Dreamer_PyTorch](https://github.com/cross32768/Dreamer_PyTorch) (unofficial)<br>[minhphd/PyDreamerV1](https://github.com/minhphd/PyDreamerV1) (unofficial) |
| [PlaNet of the Bayesians: Reconsidering and Improving Deep Planning Network by Incorporating Bayesian Inference](https://arxiv.org/abs/2003.00370) | 2003.00370 | [IROS 2020](https://doi.org/10.1109/iros45743.2020.9340873) |  |
| [Mastering Atari with Discrete World Models](https://arxiv.org/abs/2010.02193) | 2010.02193 | ICLR 2021 | [danijar/dreamerv2](https://github.com/danijar/dreamerv2)<br>[sai-prasanna/dreamerv2_torch](https://github.com/sai-prasanna/dreamerv2_torch) (unofficial) |
| [DayDreamer: World Models for Physical Robot Learning](https://arxiv.org/abs/2206.14176) | 2206.14176 | CoRL 2022 | [danijar/daydreamer](https://github.com/danijar/daydreamer) |
| [Mastering Diverse Domains through World Models](https://arxiv.org/abs/2301.04104) | 2301.04104 | [Nature 2025](https://doi.org/10.1038/s41586-025-08744-2) | [danijar/dreamerv3](https://github.com/danijar/dreamerv3)<br>[NM512/dreamerv3-torch](https://github.com/NM512/dreamerv3-torch) (unofficial) |
| [TD-MPC2: Scalable, Robust World Models for Continuous Control](https://arxiv.org/abs/2310.16828) | 2310.16828 | ICLR 2024 | [nicklashansen/tdmpc2](https://github.com/nicklashansen/tdmpc2) |
| [Port-Hamiltonian Neural ODE Networks on Lie Groups For Robot Dynamics Learning and Control](https://arxiv.org/abs/2401.09520) | 2401.09520 | [IEEE Transactions on Robotics 2024](https://doi.org/10.1109/TRO.2024.3428433) | [thaipduong/LieGroupHamDL](https://github.com/thaipduong/LieGroupHamDL) |
| [Robotic World Model: A Neural Network Simulator for Robust Policy Optimization in Robotics](https://arxiv.org/abs/2501.10100) | 2501.10100 |  | [leggedrobotics/robotic_world_model](https://github.com/leggedrobotics/robotic_world_model) |
| [Training Agents Inside of Scalable World Models](https://arxiv.org/abs/2509.24527) | 2509.24527 |  | [nicklashansen/dreamer4](https://github.com/nicklashansen/dreamer4) (unofficial)<br>[lucidrains/dreamer4](https://github.com/lucidrains/dreamer4) (unofficial) |
| [PH-Dreamer: A Physics-Driven World Model via Port-Hamiltonian Generative Dynamics](https://arxiv.org/abs/2605.18303) | 2605.18303 |  |  |
| [Koopman Dreamer: Spectrally Constrained Latent Dynamics for Stable World-Model Imagination](https://arxiv.org/abs/2607.19719) | 2607.19719 |  |  |
| [Conservation Buys Stability and Factoring Buys Counterfactuals in Physical World Models](https://arxiv.org/abs/2609.19674) | 2609.19674 |  |  |
