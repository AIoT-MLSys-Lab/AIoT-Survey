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

### Wireless Sensing (Look at papers from Jie Xiong @ UMASS)
* Ember: energy management of batteryless event detection sensors with deep reinforcement learning, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430734)
* UniTS: Short-Time Fourier Inspired Neural Networks for Sensory Time Series Classification, SenSys21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485942)
* FaHo: deep learning enhanced holographic localization for RFID tags, SenSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360035)
* General-purpose deep tracking platform across protocols for the internet of things, MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3389029)
* milliEgo: single-chip mmWave radar aided egomotion estimation via deep sensor fusion, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430776)
* RF-net: a unified meta-learning framework for RF-enabled one-shot human activity recognition, SenSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3384419.3430735)
* Mobi2Sense: Empowering Wireless Sensing with Mobility, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560518) (NO ML)
* LTE-Based Low-Cost and Low-Power Soil Moisture Sensing, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568525) (NO ML)
* Experience: pushing indoor localization from laboratory to the wild, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560546) (NO ML)
* Placement Matters: Understanding the Effects of Device Placement for WiFi Sensing, IMWUT/UbiComp 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3517237) (NO ML)
* Exploring Multiple Antennas for Long-range WiFi Sensing, IMWUT/UniComp 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3494979) (NO ML)
* LTE-based Pervasive Sensing Across Indoor and Outdoor, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485943) (NO ML)
* RF-URL: unsupervised representation learning for RF sensing, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560529)
* Achieving Receiver-Side Cross-Technology Communication with Cross-Decoding, MobiCom 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241547) (NO ML) 
* Augmenting Augmented Reality with Non-Line-of-Sight Perception, NSDI 23 [[Paper]](https://www.usenix.org/conference/nsdi23/presentation/boroushaki) (NO ML)
* Cross-Frequency Communication: Near-Field Identification of UHF RFIDs with WiFi!, MobiCom 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241569)
* See through smoke: robust indoor mapping with low-cost mmWave radar, MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388945)
* TyrLoc: a low-cost multi-technology MIMO localization system with a single RF chain, MobiSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467677) (NO ML) 
* M4esh: mmWave-Based 3D Human Mesh Construction for Multiple Subjects, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568545)
* Motion inspires notion: self-supervised visual-LiDAR fusion for environment depth estimation, MobiSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538918)
* On the Feasibility of Wi-Fi Based Material Sensing, MobiCom 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345442)(NO ML)
* Empowering smart buildings with self-sensing concrete for structural health monitoring, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3544216.3544270) (NO ML)



### Acoustic Sensing
* MetaSense: few-shot adaptation to untrained conditions in deep mobile sensing, SenSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360020)
* ClearBuds: wireless binaural earbuds for learning-based speech enhancement, MobiSys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3498361.3538933)
* In-body backscatter communication and localization, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3230543.3230565) (NO ML)
* Hybrid Neural Networks for On-device Directional Hearing, AAAI 22 [[Paper]](https://arxiv.org/abs/2112.05893)[[Code]](https://github.com/wanganran/HybridBeam)
* Experience: practical problems for acoustic sensing, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560527)(NO ML)
* Enabling Contact-free Acoustic Sensing under Device Motion, UbiComp 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3550329)(NO ML)
* LASense: Pushing the Limits of Fine-grained Activity Sensing Using Acoustic Sign, IMWUT/UbiComp 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3517253) (NO ML)
* HeadFi: bringing intelligence to all headphones, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448624) (NO ML)
* MAVL: Multiresolution Analysis of Voice Localization, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-wang-mei.pdf) (NO ML)
* SQEE: A Machine Perception Approach to Sensing Quality Evaluation at the Edge by Uncertainty Quantification, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568534)
* SPiDR: ultra-low-power acoustic spatial sensing for micro-robot navigation, MobiSys 22  [[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3539775) (NO ML)
* Owlet: enabling spatial information in ubiquitous acoustic devices, MobiSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467880)
* Acoustic Sensing and Communication Using Metasurface, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-zhang-yongzhao.pdf)
* SVoice: Enabling Voice Communication in Silence via Acoustic Sensing on Commodity Devices, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568530)



### Under Water Sensing (Look at papers from Fadel @ MIT)
Sunflower: locating underwater robots from the air, MobiSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3539773)



### Multi-modal Sensing
* Low-latency speculative inference on distributed multi-modal data streams, MobiSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3458864.3467884)
* Indoor localization via multi-modal sensing on smartphones, UbiComp 16 [[Paper]](https://dl.acm.org/doi/abs/10.1145/2971648.2971668)
* EngageMon: Multi-Modal Engagement Sensing for Mobile Games, UniComp 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3191745) (NO ML)
* mSAIL: milligram-scale multi-modal sensor platform for monarch butterfly migration tracking, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483263)
* UltraSE: single-channel speech enhancement using ultrasound, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448626)
* RFID and camera fusion for recognition of human-object interactions, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483244)
* Cosmo: contrastive fusion learning with small data for multimodal human activity recognition, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560519)
* Personalizing head related transfer functions for earables, SIGCOMM 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3452296.3472907)
* VSkin: Sensing Touch Gestures on Surfaces of Mobile Devices Using Acoustic Signals, MobiCom 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241568) (NO ML) 
* CrowdEstimator: Approximating Crowd Sizes with Multi-modal Data for Internet-of-Things Services, MobiSys 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210320) (NO ML) 
* Wavoice: A Noise-resistant Multi-modal Speech Recognition System Fusing mmWave and Audio Signals, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485945)
* SenseHAR: a robust virtual activity sensor for smartphones and wearables, SenSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360032)
* Capricorn: Towards Real-Time Rich Scene Analysis Using RF-Vision Sensor Fusion, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568504)
* A closer look at quality-aware runtime assessment of sensing models in multi-device environments, SenSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360043)
* Real-time Arm Skeleton Tracking and Gesture Inference Tolerant to Missing Wearable Sensors, MobiSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326109)


### Vision Sensing
* Rhythmic pixel regions: multi-resolution visual sensing system towards high-precision visual computing at low power, ASPLOS 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3445814.3446737)
* Source Compression with Bounded DNN Perception Loss for IoT Edge Computer Vision, MobiCom 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345448)
* Approximate query service on autonomous IoT cameras, MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388948)
* Starfish: resilient image compression for AIoT cameras,SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430769) 
* Banner: An Image Sensor Reconfiguration Framework for Seamless Resolution-based Tradeoffs, MobiSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326092)



## Computing

### On-Device Inferences
#### Scheduling
* CoDL: efficient CPU-GPU co-execution for deep learning inference on mobile devices, MobiSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538932)
* BlastNet: Exploiting Duo-Blocks for Cross-Processor Real-Time DNN Inference, SenSys 22 [[Paper]](https://yanzhenyu.com/assets/pdf/BlastNet-SenSys22.pdf)
* MobiPose: real-time multi-person pose estimation on mobile devices, SensSys20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430726)
* GPUReplay: a 50-KB GPU stack for client ML, ASPLOS 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507754)
* AsyMo: Scalable and Efficient Deep-Learning Inference on Asymmetric Mobile CPUs, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448625)
* Microsecond-scale Preemption for Concurrent GPU-accelerated DNN Inferences, OSDI 22 [[Paper]](https://www.usenix.org/conference/osdi22/presentation/han)
* μLayer: Low Latency On-Device Inference Using Cooperative Single-Layer Acceleration and Processor-Friendly Quantization, EuroSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3302424.3303950)
* BlastNet: Exploiting Duo-Blocks for Cross-Processor Real-Time DNN Inference, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568520)



#### DNN Compressing
* Fast and scalable in-memory deep multitask learning via neural weight virtualization, MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388947)
* BiSon-e: a lightweight and high-performance accelerator for narrow integer linear algebra computing on the edge, ASPLOS 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507746)
* Intelligence Beyond the Edge: Inference on Intermittent Embedded Systems, ASPLOS 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3297858.3304011)
* ADMM-NN: An Algorithm-Hardware Co-Design Framework of DNNs Using Alternating Direction Methods of Multipliers, ASPLOS 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3297858.3304076)
* Mistify: Automating DNN Model Porting for On-Device Inference at the Edge, NSDI 2021 [[Paper]](https://www.usenix.org/system/files/nsdi21-guo.pdf)
* LegoDNN: block-grained scaling of deep neural networks for mobile vision, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483249)
* FastDeepIoT: Towards Understanding and Optimizing Neural Network Execution Time on Mobile and Embedded Devices, SenSys 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3274783.3274840)
* nn-Meter: towards accurate latency prediction of deep-learning model inference on diverse edge devices, MobiSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467882)
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
* Campo: Cost-Aware Performance Optimization for Mixed-Precision Neural Network Training, ATC 22 [[Paper]](https://www.usenix.org/system/files/atc22-he.pdf)



### Offloading
* CLIO: enabling automatic compilation of deep learning pipelines across IoT and cloud, MobiCom 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3372224.3419215) 
* Elf: accelerate high-resolution mobile deep vision with content-aware parallel offloading, MobiCom21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448628)
* Deep compressive offloading: speeding up neural network inference by trading edge computation for network latency, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430898)
* Walle: An End-to-End, General-Purpose, and Large-Scale Production System for Device-Cloud Collaborative Machine Learning, OSDI 22 [[Paper]](https://www.usenix.org/system/files/osdi22-lv.pdf)
* FoggyCache: Cross-Device Approximate Computation Reuse, MobiCom 18, [[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241557)
* InFi: end-to-end learnable input filter for resource-efficient mobile-centric inference, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517016)
* Neuro.ZERO: a zero-energy neural network accelerator for embedded sensing and inference systems, SenSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360030)
* Hyperion: A Generic and Distributed Mobile Offloading Framework on OpenCL, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568511)




### Automated Machine Learning


### Compiler for Deep Learning
* 



## Networking and Communication

### Backscatter (Look at papers from Shyam @ University of Washington) 
* Wind dispersal of battery-free wireless devices, Nature 2022 [[Paper]](https://www.nature.com/articles/s41586-021-04363-9) (NO ML)
* VMscatter: A Versatile MIMO Backscatter, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-liu.pdf) (NO ML)
* Towards Battery-Free HD Video Streaming, NSDI 18 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/videobackscatter.pdf) (NO ML)
* Charging a Smartphone Across a Room Using Lasers, UbiComp 18 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/laserpower.pdf) (NO ML)
* LoRa Backscatter: Enabling The Vision of Ubiquitous Connectivity, UbiComp 17 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/loRaBackscatter.pdf) (NO ML)
* Battery-Free Cellphone, UbiComp 17[[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/phone.pdf) (NO ML)
* OmniScatter: extreme sensitivity mmWave backscattering using commodity FMCW radar, MobiSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538924) (NO ML)
* Towards scalable backscatter sensor mesh with decodable relay and distributed excitation, MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388942) (NO ML)
* Content-agnostic backscatter from thin air, MobiSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538930) (NO ML)
* Low-Latency Visible Light Backscatter Networking with RetroMUMIMO, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568507) (NO ML)
* Microphone array backscatter: an application-driven design for lightweight spatial sound recording over the air, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483265) (NO ML)
* Self-Reconfgurable Micro-Implants for Cross-Tissue Wireless and Batteryless Connectivity, MobiCom 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3372224.3419216) (NO ML)



### LoRa
* NELoRa: Towards Ultra-low SNR LoRa Communication with Neural-enhanced Demodulation, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485928)
* Embracing LoRa Sensing with Device Mobility, SenSys 22 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/SenSys22-LoRaSensingMobility.pdf) (NO ML)
* Sensor-free Soil Moisture Sensing Using LoRa Signals, MobiCom22 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3534608) (NO ML) 
* Exploring LoRa for Long-range Through-wall Sensing, IMWUT/UbiComp 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3397326) (NO ML)
* WIDESEE: Towards Wide-Area Contactless Wireless Sensing, SenSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3356250.3360031) (NO ML)
* HyLink: Towards High Throughput LPWANs with LoRa Compatible Communication, SenSys 22 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/HyLink-SenSys22.pdf) (NO ML)
* LAVA: fine-grained 3D indoor wireless coverage for small IoT devices, SIGCOMM 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3452296.3472890) (NO ML)
* Saiyan: Design and Implementation of a Low-power Demodulator for LoRa Backscatter Systems, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-guo.pdf) (NO ML)



### Under Water Communication
* Underwater backscatter networking, SIGCOMM 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3341302.3342091) (NO ML)
* Underwater Messaging Using Mobile Devices, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3544216.3544258)[[Code]](https://github.com/uw-x/watercomms) (NO ML)
* Ultra-Wideband Underwater Backscatter via Piezoelectric Metamaterials, SIGCOMM22 [[Paper]](https://www.mit.edu/~fadel/papers/U2B-paper.pdf) (NO ML)
* Networking across boundaries: enabling wireless communication through the water-air interface, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/10.1145/3230543.3230580) (NO ML)
* Shrimp: a robust underwater visible light communication system, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448616) (NO ML)
* U-star: an underwater navigation system based on passive 3D optical identification tags, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517019)




## Security and Privacy

### Security of AIoT
* Client-optimized algorithms and acceleration for encrypted compute offloading, ASPLOS 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507737)
* Occlumency: Privacy-preserving Remote Deep-learning Inference Using SGX, MObiCom 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345447)
* Light Auditor: Power Measurement Can Tell Private Data Leakage through IoT Covert Channels, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568535) 
* DarkneTZ: towards model privacy at the edge using trusted execution environments MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388946)
* SOTER: Guarding Black-box Inference for General Neural Networks at the Edge, ATC 22 [[Paper]](https://www.usenix.org/system/files/atc22-shen.pdf)
* Sniffing Visible Light Communication Through Walls, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419187) (NO ML)
* Brain Password: A Secure and Truly Cancelable Brain Biometrics for Smart Headwear, MobiSys 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210344) (NO ML)
* FastZIP: faster and more secure zero-interaction pairing, MobiSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467883) (NO ML)
* HideSeeker: Uncover the Hidden Gems in Obfuscated Images, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568514)
* G2Auth: secure mutual authentication for drone delivery without special user-side hardware, MobiSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538941) (NO ML)








### Federated Learning Systems
* PyramidFL: a fine-grained client selection framework for efficient federated learning, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517017) 
* FedRolex: Model-Heterogeneous Federated Learning with Rolling Sub-Model Extraction, NeurIPS 22
* FedBalancer: data and pace control for efficient federated learning on heterogeneous clients, MobiSys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3498361.3538917)
* FedSEA: A Semi-Asynchronous Federated Learning Framework for Extremely Heterogeneous Devices
* Hermes: an efficient federated learning framework for heterogeneous mobile clients, MobiCom 21 [[Paper]](https://dl.acm.org/doi/10.1145/3447993.3483278)
* PPFL: privacy-preserving federated learning with trusted execution environments, MobiSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3458864.3466628)
* ClusterFL: a similarity-aware federated learning system for human activity recognition, MobiSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3458864.3467681)
* FedDL: Federated Learning via Dynamic Layer Sharing for Human Activity Recognition, SenSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485946)
* FedMask: Joint Computation and Communication-Efficient Personalized Federated Learning via Heterogeneous Masking, SenSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485929)
* Oort: Efficient Federated Learning via Guided Participant Selection, OSDI 21 [[Paper]](https://www.usenix.org/system/files/osdi21-lai.pdf)
* Billion-scale federated learning on mobile clients: a submodel design with tunable privacy, MobiCom 20 [[Paper]](https://dl.acm.org/doi/10.1145/3372224.3419188)




## AIoT Systems and their Applications

### AIoT Systems for Healthcare and Social Good
* MobileDeepPill: A Small-Footprint Mobile Deep Learning System for Recognizing Unconstrained Pill Images, MobiSys 17
* DeepASL: Enabling Ubiquitous and Non-Intrusive Word and Sentence-Level Sign Language Translation, SenSys 17
* Contactless Infant Monitoring using White Noise, MobiCom 19 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/whitenoise.pdf) (NO ML)
* SmartLens : Sensing Eye Activities Using Zero-power Contact Lens, MobiCom22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560532) (NO ML)
* Your Smart Speaker Can “Hear” Your Heartbeat!, IMWUT/UbiComp 21 [[Paper]](https://dl.acm.org/doi/10.1145/3432237) (NO ML)
* PDLens: smartphone knows drug effectiveness among Parkinson's via daily-life activity fusion, MobiCom 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3372224.3380889)
* U-Verse: a miniaturized platform for end-to-end closed-loop implantable internet of medical things systems, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360026) (NO ML)
* Out-Clinic Pulmonary Disease Evaluation via Acoustic Sensing and Multi-Task Learning on Commodity Smartphones, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568437)




### AIoT Systems for Video Analytics 
* Potluck: Cross-Application Approximate Deduplication for Computation-Intensive Mobile Applications [[Paper]](https://dl.acm.org/doi/abs/10.1145/3173162.3173185)
* SmrtFridge: IoT-based, user interaction-driven food item & quantity sensing, SenSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360028)
* When IoT met Augmented Reality: Visualizing the Source of the Wireless Signal in AR View, MobiSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326079)
* AutoMatch: Leveraging Traffic Camera to Improve Perception and Localization of Autonomous Vehicles, SenSys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3560905.3568519)
* Distream: Scaling Live Video Analytics with Workload-Adaptive Distributed Edge Intelligence, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430721)
* EMO: real-time emotion recognition from single-eye images for resource-constrained eyewear devices, MobiSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3386901.3388917)
* NeuriCam: Key-Frame Video Super-Resolution and Colorization for IoT Cameras, MobiCom 23 [[Paper]](https://arxiv.org/abs/2207.12496)[[Code]](https://github.com/vb000/NeuriCam)
* FollowUpAR: enabling follow-up effects in mobile AR applications,  MobiSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467675)
* Rubiks: Practical 360-Degree Streaming for Smartphones, MobiSys 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210323) (NO ML) 




### AIoT Systems for Communication 





