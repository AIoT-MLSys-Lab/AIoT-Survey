# A collection of survey, research papers, benchmarks, open-source resources, and seminars of AIoT (Artificial Intelligence of Things)

Papers selected from the following conferences: 
- mobile computing conferences (MobiCom/MobiSys/SenSys/UbiComp)
- computer networks conferences (NSDI/SIGCOMM) 
- operating systems conferences (OSDI/SOSP/EuroSys/ASPLOS/ATC)
- AI conferences (MLSys, NeurIPS, ICLR, ICML, CVPR, ICCV, ECCV, ACL)

Years: 2018 ~ Present

Find at most 10 papers in each sub-topic.

Each week, focus on Writing one sub-topic.


## What is AIoT?

Artificial Intelligence of Things (AIoT) is one of the most exciting areas that lies at the intersection of Artificial Intelligence (AI) and Internet of Things (IoT).

## Table of Contents
* [Sensing](#sensing)
  * [Wireless Sensing](#wireless-sensing)
  * [Acoustic Sensing](#acoustic-sensing)
  * [Under Water Sensing](#under-water-sensing)
  * [Multi-modal Sensing](#multimodal-sensing)
  * [Vision Sensing](#vision-sensing)
* [Computing](#computing)
  * [On-Device Inferences](#on-device-Inferences)
  * [On-Device Training Evaluation](#on-device-training-evaluation)
  * [Offloading](#offloading)
  * [Automated Machine Learning](#automated-machine-learning)
  * [Compiler for Deep Learning](#compiler-for-deep-learning)
* [Networking and Communication](#networking-and-communication)
  * [Backscatter](#backscatter)
  * [LoRa](#lora)
  * [Under Water Communication](#under-water-communication)
* [Security and Privacy](#security-and-privacy)
  * [Security of AIoT](#security-of-aiot)
  * [Federated Learning](#federated-learning)
* [AIoT Systems and their Applications](#building-aiot-systems)
  * [AIoT Systems for Healthcare](#aiot-for-healthcare-systems)
  * [AIoT Systems for Video Analytics](#aiot-for-video-analytics-systems)
  * [AIoT Systems for Communication](#aiot-for-communication-systems) 



## Sensing (MobiCom, MobiSys, SenSys, NSDI)

### Wireless Sensing
* Ember: energy management of batteryless event detection sensors with deep reinforcement learning, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430734)
* UniTS: Short-Time Fourier Inspired Neural Networks for Sensory Time Series Classification, SenSys21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485942)
* FaHo: deep learning enhanced holographic localization for RFID tags, SenSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360035)
* General-purpose deep tracking platform across protocols for the internet of things, MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3389029)
* milliEgo: single-chip mmWave radar aided egomotion estimation via deep sensor fusion, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430776)


### Acoustic Sensing
* MetaSense: few-shot adaptation to untrained conditions in deep mobile sensing, SenSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360020)


### Under Water Sensing


### Multi-modal Sensing
* Low-latency speculative inference on distributed multi-modal data streams, MobiSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3458864.3467884)

### Vision Sensing
* Rhythmic pixel regions: multi-resolution visual sensing system towards high-precision visual computing at low power, ASPLOS 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3445814.3446737)
* Source Compression with Bounded DNN Perception Loss for IoT Edge Computer Vision, MobiCom 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345448)
* Approximate query service on autonomous IoT cameras, MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388948)
* Starfish: resilient image compression for AIoT cameras,SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430769) 


## Computing

### On-Device Inferences
#### Scheduling
* CoDL: efficient CPU-GPU co-execution for deep learning inference on mobile devices, MobiSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538932)
#### Compressing
* GPUReplay: a 50-KB GPU stack for client ML, ASPLOS 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507754)
* AsyMo: Scalable and Efficient Deep-Learning Inference on Asymmetric Mobile CPUs, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448625)
* Fast and scalable in-memory deep multitask learning via neural weight virtualization, MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388947)
* BiSon-e: a lightweight and high-performance accelerator for narrow integer linear algebra computing on the edge, ASPLOS 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507746)
* Intelligence Beyond the Edge: Inference on Intermittent Embedded Systems, ASPLOS 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3297858.3304011)
* ADMM-NN: An Algorithm-Hardware Co-Design Framework of DNNs Using Alternating Direction Methods of Multipliers, ASPLOS 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3297858.3304076)
* Mistify: Automating DNN Model Porting for On-Device Inference at the Edge, NSDI 2021 [[Paper]](https://www.usenix.org/system/files/nsdi21-guo.pdf)
* LegoDNN: block-grained scaling of deep neural networks for mobile vision, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483249)
* Characterising the Role of Pre-Processing Parameters in Audio-based Embedded Machine Learning, SenSys21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3493448)
* FastDeepIoT: Towards Understanding and Optimizing Neural Network Execution Time on Mobile and Embedded Devices, SenSys 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3274783.3274840)
* On-Demand Deep Model Compression for Mobile Devices: A Usage-Driven Model Selection Framework, MobiSys 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210337)
* RT-mDL: Supporting Real-Time Mixed Deep Learning Tasks on Edge Platforms, SenSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485938) 
* PatDNN: Achieving Real-Time DNN Execution on Mobile Devices with Pattern-based Weight Pruning, ASPLOS 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3373376.3378534)
* Memory-Efficient Domain Incremental Learning for Internet of Things, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568436) 
* MDLdroidLite: a release-and-inhibit control approach to resource-efficient deep neural networks on mobile devices, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430716)
* LIMU-BERT: Unleashing the Potential of Unlabeled Data for IMU Sensing Applications, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485937) 


### On-Device Training Evaluation
* Mercury: Efficient On-Device Distributed DNN Training via Stochastic Importance Sampling, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485930) 
* Memory-efficient DNN training on mobile devices. MobiSys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3498361.3539765)
* Octo: INT8 Training with Loss-aware Compensation and Backward Quantization for Tiny On-device Learning, ATC21 [[Paper]](https://www.usenix.org/conference/atc21/presentation/zhou-qihua)
* A Unified Architecture for Accelerating Distributed DNN Training in Heterogeneous GPU/CPU Clusters, OSDI 20 [[Paper]](https://www.usenix.org/system/files/osdi20-jiang.pdf)
* Mandheling: mixed-precision on-device DNN training with DSP offloading, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560545)






### Offloading
* CLIO: enabling automatic compilation of deep learning pipelines across IoT and cloud, MobiCom 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3372224.3419215) 
* Elf: accelerate high-resolution mobile deep vision with content-aware parallel offloading, MobiCom21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448628)
* Deep compressive offloading: speeding up neural network inference by trading edge computation for network latency, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430898)


### Automated Machine Learning


### Compiler for Deep Learning


## Networking and Communication

### Backscatter

### LoRa
* NELoRa: Towards Ultra-low SNR LoRa Communication with Neural-enhanced Demodulation, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485928)

### Under Water Communication


## Security and Privacy

### Security of AIoT
* Client-optimized algorithms and acceleration for encrypted compute offloading, ASPLOS 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507737)
* Occlumency: Privacy-preserving Remote Deep-learning Inference Using SGX, MObiCom 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345447)
* Large-scale Urban IoT Activity Data for DDoS Attack Emulation, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3493695)
* Light Auditor: Power Measurement Can Tell Private Data Leakage through IoT Covert Channels, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568535)
* DarkneTZ: towards model privacy at the edge using trusted execution environments MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388946)


### Federated Learning
* PyramidFL: a fine-grained client selection framework for efficient federated learning, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517017) 
* FedBalancer: data and pace control for efficient federated learning on heterogeneous clients, MobiSys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3498361.3538917)
* Hermes: an efficient federated learning framework for heterogeneous mobile clients, MobiCom 21 [[Paper]](https://dl.acm.org/doi/10.1145/3447993.3483278)
* PPFL: privacy-preserving federated learning with trusted execution environments, MobiSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3458864.3466628)
* ClusterFL: a similarity-aware federated learning system for human activity recognition, MobiSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3458864.3467681)
* FedDL: Federated Learning via Dynamic Layer Sharing for Human Activity Recognition, SenSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485946)
* FedMask: Joint Computation and Communication-Efficient Personalized Federated Learning via Heterogeneous Masking, SenSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485929)
* Oort: Efficient Federated Learning via Guided Participant Selection, OSDI 21 [[Paper]](https://www.usenix.org/system/files/osdi21-lai.pdf)
* Billion-scale federated learning on mobile clients: a submodel design with tunable privacy, MobiCom 20 [[Paper]](https://dl.acm.org/doi/10.1145/3372224.3419188)




## AIoT Systems and their Applications

### AIoT for Healthcare Systems

### AIoT for Video Analytics Systems
* Potluck: Cross-Application Approximate Deduplication for Computation-Intensive Mobile Applications [[Paper]](https://dl.acm.org/doi/abs/10.1145/3173162.3173185)
* SmrtFridge: IoT-based, user interaction-driven food item & quantity sensing, SenSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360028)
* When IoT met Augmented Reality: Visualizing the Source of the Wireless Signal in AR View, MobiSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326079)
* AutoMatch: Leveraging Traffic Camera to Improve Perception and Localization of Autonomous Vehicles, SenSys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3560905.3568519)

### AIoT for Communication Systems

