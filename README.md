# Awesome AIoT

A curated, but incomplete, list of AIoT resources. It should be noted that it is unfeasible to encompass every paper. Thus, we prefer to selectively choose papers that present a range of distinct ideas. We welcome contributions to further enrich and refine this list.

Veneus: 
- mobile conferences (MobiCom/MobiSys/SenSys/UbiComp)
- network conferences (NSDI/SIGCOMM) 
- core system conferences (OSDI/SOSP/EuroSys/ASPLOS/ATC)
- AI conferences (MLSys, NeurIPS, ICLR, ICML, CVPR, ICCV, ECCV, ACL)

Years: 2018 ~ Present


## What is AIoT?

## Table of Contents
* [Sensing](#sensing)
  * [Wireless Sensing](#wireless-sensing)
  * [Data Labeling](#data-labeling)
  * [Data Preparation](#data-preparation)
  * [Data Reduction](#data-reduction)
  * [Data Augmentation](#data-augmentation)
  * [Pipeline Search](#pipeline-search)
* [Inference Data Development](#inference-data-development)
  * [In-distribution Evaluation](#in-distribution-evaluation)
  * [Out-of-distribution Evaluation](#out-of-distribution-evaluation)
  * [Prompt Engineering](#prompt-engineering)
* [Data Maintenance](#data-maintenance)
  * [Data Understanding](#data-understanding)
  * [Data Quality Assurance](#data-quality-assurance)
  * [Data Storage and Retrieval](#data-storage-and-retrieval)
* [Data Benchmark](#data-benchmark)
  * [Training Data Development Benchmark](#training-data-development-benchmark)
  * [Inference Data Development Benchmark](#inference-data-development-benchmark)
  * [Data Maintenance Benchmark](#data-maintenance-benchmark)
  * [Unified Benchmark](#unified-benchmark)


### Sensing
Rhythmic pixel regions: multi-resolution visual sensing system towards high-precision visual computing at low power, ASPLOS 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3445814.3446737)

General-purpose deep tracking platform across protocols for the internet of things, MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3389029)

Ember: energy management of batteryless event detection sensors with deep reinforcement learning, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430734)

Low-latency speculative inference on distributed multi-modal data streams, MobiSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3458864.3467884)

UniTS: Short-Time Fourier Inspired Neural Networks for Sensory Time Series Classification
, SenSys21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485942)

FaHo: deep learning enhanced holographic localization for RFID tags, SenSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360035)

SmrtFridge: IoT-based, user interaction-driven food item & quantity sensing, SenSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360028)

When IoT met Augmented Reality: Visualizing the Source of the Wireless Signal in AR View, MobiSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326079)


### Privacy-Security

Client-optimized algorithms and acceleration for encrypted compute offloading, ASPLOS 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507737)

Occlumency: Privacy-preserving Remote Deep-learning Inference Using SGX, MObiCom 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345447)

Large-scale Urban IoT Activity Data for DDoS Attack Emulation, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3493695)

Light Auditor: Power Measurement Can Tell Private Data Leakage through IoT Covert Channels, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568535)

DarkneTZ: towards model privacy at the edge using trusted execution environments MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388946)

milliEgo: single-chip mmWave radar aided egomotion estimation via deep sensor fusion, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430776)



### Network

P4Pir: in-network analysis for smart IoT gateways, SIGCOMM 22 [[Poster]](https://dl.acm.org/doi/abs/10.1145/3546037.3546060)

NELoRa: Towards Ultra-low SNR LoRa Communication with Neural-enhanced Demodulation, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485928)




### Scheduling/Depolying

Potluck: Cross-Application Approximate Deduplication for Computation-Intensive Mobile Applications [[Paper]](https://dl.acm.org/doi/abs/10.1145/3173162.3173185)

GPUReplay: a 50-KB GPU stack for client ML, ASPLOS 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507754)

AsyMo: Scalable and Efficient Deep-Learning Inference on Asymmetric Mobile CPUs, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448625)

Fast and scalable in-memory deep multitask learning via neural weight virtualization, MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388947)

PyramidFL: a fine-grained client selection framework for efficient federated learning, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517017) 

Approximate query service on autonomous IoT cameras, MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388948)

CoDL: efficient CPU-GPU co-execution for deep learning inference on mobile devices, MobiSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538932)



### Offloading
CLIO: enabling automatic compilation of deep learning pipelines across IoT and cloud, MobiCom 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3372224.3419215) 

Source Compression with Bounded DNN Perception Loss for IoT Edge Computer Vision, MobiCom 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345448)
:(Data compression for badnwidth reduction)

Elf: accelerate high-resolution mobile deep vision with content-aware parallel offloading, MobiCom21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448628)

Deep compressive offloading: speeding up neural network inference by trading edge computation for network latency, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430898)




### DNN Compression (Inference) - DNN modification
TinyML-CAM: 80 FPS image recognition in 1 kB RAM, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3558264) 

Starfish: resilient image compression for AIoT cameras,SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430769) 

LIMU-BERT: Unleashing the Potential of Unlabeled Data for IMU Sensing Applications, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485937) 

Smart Objects: Impact Localization Powered by TinyML, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568298) 

ElasticAI-Creator: Optimizing Neural Networks for Time-Series-Analysis for On-Device Machine Learning in IoT Systems, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568296) 

Mercury: Efficient On-Device Distributed DNN Training via Stochastic Importance Sampling, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485930) 

RT-mDL: Supporting Real-Time Mixed Deep Learning Tasks on Edge Platforms, SenSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485938) 

Memory-Efficient Domain Incremental Learning for Internet of Things, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568436) 

Intelligence Beyond the Edge: Inference on Intermittent Embedded Systems, ASPLOS 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3297858.3304011)

PatDNN: Achieving Real-Time DNN Execution on Mobile Devices with Pattern-based Weight Pruning, ASPLOS 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3373376.3378534)

ADMM-NN: An Algorithm-Hardware Co-Design Framework of DNNs Using Alternating Direction Methods of Multipliers, ASPLOS 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3297858.3304076)

Mistify: Automating DNN Model Porting for On-Device Inference at the Edge, NSDI 2021 [[Paper]](https://www.usenix.org/system/files/nsdi21-guo.pdf)

LegoDNN: block-grained scaling of deep neural networks for mobile vision, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483249)

Characterising the Role of Pre-Processing Parameters in Audio-based Embedded Machine Learning, SenSys21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3493448)

FastDeepIoT: Towards Understanding and Optimizing Neural Network Execution Time on Mobile and Embedded Devices, SenSys 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3274783.3274840)

On-Demand Deep Model Compression for Mobile Devices: A Usage-Driven Model Selection Framework, MobiSys 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210337)

MetaSense: few-shot adaptation to untrained conditions in deep mobile sensing, SenSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360020)

MDLdroidLite: a release-and-inhibit control approach to resource-efficient deep neural networks on mobile devices, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430716)


### Applications
Mobile IoT-RoadBot: an AI-powered mobile IoT solution for real-time roadside asset management, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3558271)


### Architecture
BiSon-e: a lightweight and high-performance accelerator for narrow integer linear algebra computing on the edge, ASPLOS 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507746)
