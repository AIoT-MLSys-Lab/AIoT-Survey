# A collection of survey, research papers, benchmarks, open-source resources, and seminars of AIoT (Artificial Intelligence of Things)

Papers selected from the following conferences: 
- mobile computing conferences (MobiCom/MobiSys/SenSys/IPSN)
- computer networks conferences (NSDI/SIGCOMM) 
- operating systems conferences (OSDI/SOSP/EuroSys/ASPLOS/ATC)
- AI + Systems conferences (MLSys)

Years: 2018 ~ Present

Find at most 10 papers in each sub-topic.

Each week, focus on Writing one sub-topic.


## What is AIoT?

Artificial Intelligence of Things (AIoT) is one of the most exciting areas that lies at the intersection of Artificial Intelligence (AI) and Internet of Things (IoT).

## Table of Contents
- [A collection of survey, research papers, benchmarks, open-source resources, and seminars of AIoT (Artificial Intelligence of Things)](#a-collection-of-survey-research-papers-benchmarks-open-source-resources-and-seminars-of-aiot-artificial-intelligence-of-things)
  - [What is AIoT?](#what-is-aiot)
  - [Table of Contents](#table-of-contents)
  - [Sensing (MobiCom, MobiSys, SenSys, NSDI)](#sensing-mobicom-mobisys-sensys-nsdi)
    - [Wireless Sensing (Look at papers from Jie Xiong @ UMASS)](#wireless-sensing-look-at-papers-from-jie-xiong--umass)
    - [Acoustic Sensing](#acoustic-sensing)
    - [Under Water Sensing (Look at papers from Fadel @ MIT)](#under-water-sensing-look-at-papers-from-fadel--mit)
    - [Multi-modal Sensing](#multi-modal-sensing)
    - [Vision Sensing](#vision-sensing)
  - [Computing](#computing)
    - [On-Device Inferences](#on-device-inferences)
      - [Scheduling](#scheduling)
      - [DNN Compressing](#dnn-compressing)
    - [On-Device Training Evaluation](#on-device-training-evaluation)
    - [Offloading](#offloading)
    - [Automated Machine Learning](#automated-machine-learning)
      - [NAS](#nas)
    - [Compiler for ML Systems](#compiler-for-ml-systems)
  - [Networking and Communication](#networking-and-communication)
    - [Backscatter (Look at papers from Shyam @ University of Washington)](#backscatter-look-at-papers-from-shyam--university-of-washington)
    - [LoRa](#lora)
    - [Under Water Communication](#under-water-communication)
  - [Security and Privacy](#security-and-privacy)
    - [Security of AIoT](#security-of-aiot)
    - [Federated Learning Systems](#federated-learning-systems)
  - [AIoT Systems and their Applications](#aiot-systems-and-their-applications)
    - [AIoT Systems for Healthcare and Social Good](#aiot-systems-for-healthcare-and-social-good)
    - [AIoT Systems for Video Analytics](#aiot-systems-for-video-analytics)
    - [AIoT Systems for Agriculture](#aiot-systems-for-agriculture)


## Others


## Sensing (MobiCom, MobiSys, SenSys, NSDI, UbiComp)

### Others

### Wireless Sensing (Look at papers from Jie Xiong @ UMASS)
* Augmenting Augmented Reality with Non-Line-of-Sight Perception,	NSDI	23	[[Paper]](https://www.usenix.org/conference/nsdi23/presentation/boroushaki)	(NO	ML)
* Placement Matters: Understanding the Effects of Device Placement for WiFi Sensing	,	IMWUT/UbiComp	22	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3517237)	(NO	ML)
* Exploring Multiple Antennas for Long-range WiFi Sensing	,	IMWUT/UbiComp	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3494979)	(NO	ML)
* Mobi2Sense: Empowering Wireless Sensing with Mobility	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560518)	(NO	ML)
* Experience: pushing indoor localization from laboratory to the wild	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560546)	(NO	ML)
* RF-URL: unsupervised representation learning for RF sensing	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560529)	
* Motion inspires notion: self-supervised visual-LiDAR fusion for environment depth estimation	,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538918)		
* LTE-Based Low-Cost and Low-Power Soil Moisture Sensing	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568525)	(NO	ML)
* M4esh: mmWave-Based 3D Human Mesh Construction for Multiple Subjects	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568545)		
* Empowering smart buildings with self-sensing concrete for structural health monitoring	,	SIGCOMM	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3544216.3544270)	(NO	ML)
* TyrLoc: a low-cost multi-technology MIMO localization system with a single RF chain	,	MobiSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467677)	(NO	ML)
* LTE-based Pervasive Sensing Across Indoor and Outdoor	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485943)	(NO	ML)
* UniTS: Short-Time Fourier Inspired Neural Networks for Sensory Time Series Classification	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485942)	
* Towards Position-Independent Sensing for Gesture Recognition with Wi-Fi, UbiComp 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3463504)
* General-purpose deep tracking platform across protocols for the internet of things	,	MobiSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3389029)		
* See through smoke: robust indoor mapping with low-cost mmWave radar	,	MobiSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388945)		
* Ember: energy management of batteryless event detection sensors with deep reinforcement learning	,	SenSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430734)		
* milliEgo: single-chip mmWave radar aided egomotion estimation via deep sensor fusion	,	SenSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430776)		
* Wi-fi see it all: generative adversarial network-augmented versatile wi-fi imaging, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430725)
* RF-net: a unified meta-learning framework for RF-enabled one-shot human activity recognition	,	SenSys	20	[[Paper]](https://dl.acm.org/doi/10.1145/3384419.3430735)		
* On the Feasibility of Wi-Fi Based Material Sensing	,	MobiCom	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345442)(NO	ML)	
* FaHo: deep learning enhanced holographic localization for RFID tags	,	SenSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360035)		
* Achieving Receiver-Side Cross-Technology Communication with Cross-Decoding	,	MobiCom	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241547)	(NO	ML)
* Cross-Frequency Communication: Near-Field Identification of UHF RFIDs with WiFi!	,	MobiCom	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241569)		

#### Wi-Fi Sensing

#### RFID Sensing
* MetaSight: Localizing Blocked RFID Objects by Modulating NLOS Signals via Metasurfaces, MobiSys 22 [[Paper]]

#### mmWave Sensing

#### TeraHertz Sensing


### Acoustic Sensing							
* Acoustic Sensing and Communication Using Metasurface	,	NSDI	23	[[Paper]](https://www.usenix.org/system/files/nsdi23-zhang-yongzhao.pdf)			
* Hybrid Neural Networks for On-device Directional Hearing	,	AAAI	22	[[Paper]](https://arxiv.org/abs/2112.05893)[[Code]](https://github.com/wanganran/HybridBeam)			
* LASense: Pushing the Limits of Fine-grained Activity Sensing Using Acoustic Sign	,	IMWUT/UbiComp	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3517253)	(NO	ML)	
* Experience: practical problems for acoustic sensing	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560527)(NO	ML)		
* ClearBuds: wireless binaural earbuds for learning-based speech enhancement	,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/10.1145/3498361.3538933)			
* SPiDR: ultra-low-power acoustic spatial sensing for micro-robot navigation	,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3539775)	(NO	ML)	
* SQEE: A Machine Perception Approach to Sensing Quality Evaluation at the Edge by Uncertainty Quantification	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568534)			
* SVoice: Enabling Voice Communication in Silence via Acoustic Sensing on Commodity Devices	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568530)			
* Enabling Contact-free Acoustic Sensing under Device Motion	,	UbiComp	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3550329)(NO	ML)		
* HeadFi: bringing intelligence to all headphones	,	MobiCom	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448624)	(NO	ML)	
* Owlet: enabling spatial information in ubiquitous acoustic devices	,	MobiSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467880)			
* MAVL: Multiresolution Analysis of Voice Localization	,	NSDI	21	[[Paper]](https://www.usenix.org/system/files/nsdi21-wang-mei.pdf)	(NO	ML)	
* MetaSense: few-shot adaptation to untrained conditions in deep mobile sensing	,	SenSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360020)			
* In-body backscatter communication and localization	,	SIGCOMM	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3230543.3230565)	(NO	ML)	
							
							
### Vision Sensing							
* Rhythmic pixel regions: multi-resolution visual sensing system towards high-precision visual computing at low power	,	ASPLOS	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3445814.3446737)			
* Approximate query service on autonomous IoT cameras	,	MobiSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388948)
* Starfish: resilient image compression for AIoT cameras	,	SenSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430769)	
* Source Compression with Bounded DNN Perception Loss for IoT Edge Computer Vision	,	MobiCom	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345448)			
* Banner: An Image Sensor Reconfiguration Framework for Seamless Resolution-based Tradeoffs	,	MobiSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326092)			


### Under Water Sensing (Look at papers from Fadel @ MIT)
* Unsupervised Underwater Image Restoration: From a Homology Perspective, AAAI 22 [[Paper]](https://ojs.aaai.org/index.php/AAAI/article/view/19944)
* Sunflower: Locating Underwater Robots From the Air,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3539773)
* Learning To Remove Refractive Distortions From Underwater Images, ICCV 21 [[Paper]](https://openaccess.thecvf.com/content/ICCV2021/html/Thapa_Learning_To_Remove_Refractive_Distortions_From_Underwater_Images_ICCV_2021_paper.html)
* Restoration of Non-Rigidly Distorted Underwater Images Using a Combination of Compressive Sensing and Local Polynomial Image Representations, ICCV 19 [[Paper]](https://openaccess.thecvf.com/content_ICCV_2019/html/James_Restoration_of_Non-Rigidly_Distorted_Underwater_Images_Using_a_Combination_of_ICCV_2019_paper.html)
* Surface Normals and Shape From Water, ICCV 19 [[Paper]](https://openaccess.thecvf.com/content_ICCV_2019/html/Murai_Surface_Normals_and_Shape_From_Water_ICCV_2019_paper.html)


### Visible Light Sensing (Look at papers from Xia Zhou @ Columbia)	
		
							
							
							
### Multi-modal Sensing							
* Cosmo: contrastive fusion learning with small data for multimodal human activity recognition	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560519)			
* Capricorn: Towards Real-Time Rich Scene Analysis Using RF-Vision Sensor Fusion	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568504)			
* mSAIL: milligram-scale multi-modal sensor platform for monarch butterfly migration tracking	,	MobiCom	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483263)			
* UltraSE: single-channel speech enhancement using ultrasound	,	MobiCom	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448626)			
* RFID and camera fusion for recognition of human-object interactions	,	MobiCom	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483244)			
* Low-latency speculative inference on distributed multi-modal data streams	,	MobiSys	21	[[Paper]](https://dl.acm.org/doi/10.1145/3458864.3467884)			
* Wavoice: A Noise-resistant Multi-modal Speech Recognition System Fusing mmWave and Audio Signals	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485945)			
* Personalizing head related transfer functions for earables	,	SIGCOMM	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3452296.3472907)			
* Real-time Arm Skeleton Tracking and Gesture Inference Tolerant to Missing Wearable Sensors	,	MobiSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326109)			
* SenseHAR: a robust virtual activity sensor for smartphones and wearables	,	SenSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360032)			
* A closer look at quality-aware runtime assessment of sensing models in multi-device environments	,	SenSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360043)			
* VSkin: Sensing Touch Gestures on Surfaces of Mobile Devices Using Acoustic Signals	,	MobiCom	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241568)	(NO	ML)	
* CrowdEstimator: Approximating Crowd Sizes with Multi-modal Data for Internet-of-Things Services	,	MobiSys	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210320)	(NO	ML)	
* EngageMon: Multi-Modal Engagement Sensing for Mobile Games	,	UbiComp	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3191745)	(NO	ML)	
* Indoor localization via multi-modal sensing on smartphones	,	UbiComp	16	[[Paper]](https://dl.acm.org/doi/abs/10.1145/2971648.2971668)			
							
							
							
							
							
## Computing							
	
### Others

### On-Device Inferences							
#### Scheduling							

* CoDL: Efficient CPU-GPU Co-execution for Deep Learning Inference on Mobile Devices, MobiSys 2023
* Band: Coordinated Multi-DNN Inference on Heterogeneous Mobile Processors, MobiSys 2023
* ARK: GPU-driven Code Execution for Distributed Deep Learning	,	NSDI	23	[[Paper]](https://www.usenix.org/conference/nsdi23/presentation/hwang)			
* GPUReplay: a 50-KB GPU stack for client ML	,	ASPLOS	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507754)			
* VELTAIR: towards high-performance multi-tenant deep learning services via adaptive compilation and scheduling	,	ASPLOS	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507752)			
* CoDL: efficient CPU-GPU co-execution for deep learning inference on mobile devices	,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538932)			
* Microsecond-scale Preemption for Concurrent GPU-accelerated DNN Inferences	,	OSDI	22	[[Paper]](https://www.usenix.org/conference/osdi22/presentation/han)			
* BlastNet: Exploiting Duo-Blocks for Cross-Processor Real-Time DNN Inference	,	SenSys	22	[[Paper]](https://yanzhenyu.com/assets/pdf/BlastNet-SenSys22.pdf)			
* BlastNet: Exploiting Duo-Blocks for Cross-Processor Real-Time DNN Inference	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568520)			
* ElasticAI-Creator: Optimizing Neural Networks for Time-Series-Analysis for on-Device Machine Learning in IoT Systems	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568296)			
* IOS: Inter-Operator Scheduler for CNN Acceleration	,	MLSys	21	[[Paper]](https://proceedings.mlsys.org/paper_files/paper/2021/hash/38b3eff8baf56627478ec76a704e9b52-Abstract.html)			
* AsyMo: Scalable and Efficient Deep-Learning Inference on Asymmetric Mobile CPUs	,	MobiCom	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448625)			
* MobiPose: real-time multi-person pose estimation on mobile devices	,	SensSys20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430726)				
* MNN: A Universal and Efficient Inference Engine, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/8f14e45fceea167a5a36dedd4bea2543-Paper.pdf)
* μLayer: Low Latency On-Device Inference Using Cooperative Single-Layer Acceleration and Processor-Friendly Quantization	,	EuroSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3302424.3303950)			
* TicTac: Accelerating Distributed Deep Learning with Communication Scheduling	,	MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/index.html#schedule)			
* Efficient Deep Learning Inference on Edge Devices	,	MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/29.pdf)			
							
							
							
							
							
							
							
							
#### DNN Compressing							
* mGEMM: Low-latency Convolution with Minimal Memory Overhead Optimized for Mobile Devices, MobiSys 2023
* Mistify: Automating DNN Model Porting for On-Device Inference at the Edge, NSDI 2021	[[Paper]](https://www.usenix.org/system/files/nsdi21-guo.pdf)	
* BiSon-e: a lightweight and high-performance accelerator for narrow integer linear algebra computing on the edge	,	ASPLOS	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507746)			
* Bit-serial Weight Pools: Compression and Arbitrary Precision Execution of Neural Networks on Resource Constrained Processors, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/502e4a16930e414107ee22b6198c578f-Paper.pdf)
* Learning Compressed Embeddings for On-Device Inference, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/812b4ba287f5ee0bc9d43bbf5bbe87fb-Paper.pdf)
* SparTA: Deep-Learning Model Sparsity via Tensor-with-Sparsity-Attribute	,	OSDI	22	[[Paper]](https://www.usenix.org/system/files/osdi22-zheng-ningxin.pdf)			
* Memory-Efficient Domain Incremental Learning for Internet of Things	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568436)			
* LegoDNN: block-grained scaling of deep neural networks for mobile vision	,	MobiCom	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483249)			
* nn-Meter: towards accurate latency prediction of deep-learning model inference on diverse edge devices	,	MobiSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467882)			
* RT-mDL: Supporting Real-Time Mixed Deep Learning Tasks on Edge Platforms	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485938)			
* LIMU-BERT: Unleashing the Potential of Unlabeled Data for IMU Sensing Applications	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485937)			
* PCONV: The Missing but Desirable Sparsity in DNN Weight Pruning for Real-Time Execution on Mobile Devices	,	AAAI	20	[[Paper]](https://ojs.aaai.org/index.php/AAAI/article/view/5954)			
* PatDNN: Achieving Real-Time DNN Execution on Mobile Devices with Pattern-based Weight Pruning	,	ASPLOS	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3373376.3378534)			
* Fast and scalable in-memory deep multitask learning via neural weight virtualization	,	MobiSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388947)			
* Memory-Driven Mixed Low Precision Quantization for Enabling Deep Network Inference on Microcontrollers, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/9b8619251a19057cff70779273e95aa6-Paper.pdf)
* MDLdroidLite: a release-and-inhibit control approach to resource-efficient deep neural networks on mobile devices	,	SenSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430716)			
* Intelligence Beyond the Edge: Inference on Intermittent Embedded Systems	,	ASPLOS	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3297858.3304011)			
* ADMM-NN: An Algorithm-Hardware Co-Design Framework of DNNs Using Alternating Direction Methods of Multipliers	,	ASPLOS	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3297858.3304076)			
* Full deep neural network training on a pruned weight budget	,	MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/135.pdf)			
* Accurate and Efficient 2-bit Quantized Neural Networks	,	MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/168.pdf)			
* Ternary Hybrid Neural-Tree Networks for Highly Constrained IoT Applications	,	MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/107.pdf)			
* DeepThin: A Self-Compressing Library for Deep Neural Networks	,	MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/33.pdf)
* NestDNN: Resource-Aware Multi-Tenant On-Device Deep Learning for Continuous Mobile Vision, MobiCom 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241559)			
* On-Demand Deep Model Compression for Mobile Devices: A Usage-Driven Model Selection Framework	,	MobiSys	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210337)			
* FastDeepIoT: Towards Understanding and Optimizing Neural Network Execution Time on Mobile and Embedded Devices	,	SenSys	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3274783.3274840)			
							
							
							
### On-Device Training Evaluation							
* Campo: Cost-Aware Performance Optimization for Mixed-Precision Neural Network Training	,	ATC	22	[[Paper]](https://www.usenix.org/system/files/atc22-he.pdf)			
* Mandheling: mixed-precision on-device DNN training with DSP offloading	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560545)			
* Memory-efficient DNN training on mobile devices	,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/10.1145/3498361.3539765)		
* URSABench: A System for Comprehensive Benchmarking of Bayesian Deep Neural Network Models and Inference methods, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/hash/3ef815416f775098fe977004015c6193-Abstract.html)	
* ML-EXray: Visibility into ML Deployment on the Edge, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/76dc611d6ebaafc66cc0879c71b5db5c-Paper.pdf)
* MLPerf Mobile Inference Benchmark, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/7eabe3a1649ffa2b3ff8c02ebfd5659f-Paper.pdf)
* Octo: INT8 Training with Loss-aware Compensation and Backward Quantization for Tiny On-device Learning	,	ATC	21	[[Paper]](https://www.usenix.org/conference/atc21/presentation/zhou-qihua)			
* Mercury: Efficient On-Device Distributed DNN Training via Stochastic Importance Sampling	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485930)			
* A Unified Architecture for Accelerating Distributed DNN Training in Heterogeneous GPU/CPU Clusters	,	OSDI	20	[[Paper]](https://www.usenix.org/system/files/osdi20-jiang.pdf)			
* Trained Quantization Thresholds for Accurate and Efficient Fixed-Point Inference of Deep Neural Networks, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/e2c420d928d4bf8ce0ff2ec19b371514-Paper.pdf)
							
							
							
### Offloading							
* InFi: end-to-end learnable input filter for resource-efficient mobile-centric inference	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517016)			
* Walle: An End-to-End,  General-Purpose,  and Large-Scale Production System for Device-Cloud Collaborative Machine Learning	,	OSDI	22	[[Paper]](https://www.usenix.org/system/files/osdi22-lv.pdf)			
* Hyperion: A Generic and Distributed Mobile Offloading Framework on OpenCL	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568511)			
* Elf: accelerate high-resolution mobile deep vision with content-aware parallel offloading	,	MobiCom21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448628)				
* CLIO: enabling automatic compilation of deep learning pipelines across IoT and cloud	,	MobiCom	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3372224.3419215)			
* Deep compressive offloading: speeding up neural network inference by trading edge computation for network latency	,	SenSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430898)			
* Neuro.ZERO: a zero-energy neural network accelerator for embedded sensing and inference systems	,	SenSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360030)			
* Distributed Placement of Machine Learning Operators for IoT applications spanning Edge and Cloud Resources	,	MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/204.pdf)			
* FoggyCache: Cross-Device Approximate Computation Reuse	,	MobiCom	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241557)			
							
							
							
							
							
### Automated Machine Learning								
							
#### NAS
* Towards The Co-design of Neural Networks and Accelerators, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/31fefc0e570cb3860f2a6d4b38c6490d-Paper.pdf)				
* Improving Model Training with Multi-fidelity Hyperparameter Evaluation, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/a3c65c2974270fd093ee8a9bf8ae7d0b-Paper.pdf)			
* MicroNets: Neural Network Architectures for Deploying TinyML Applications on Commodity Microcontrollers	,	MLSys	21	[[Paper]](https://proceedings.mlsys.org/paper_files/paper/2021/hash/a3c65c2974270fd093ee8a9bf8ae7d0b-Abstract.html)			
* Searching for Winograd-aware Quantized Networks, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/45c48cce2e2d7fbdea1afc51c7c6ad26-Paper.pdf)
* SkyNet: a Hardware-Efficient Method for Object Detection and Tracking on Embedded Systems, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/93db85ed909c13838ff95ccfa94cebd9-Paper.pdf)
* MCUNet: Tiny Deep Learning on IoT Devices	,	NeurIPS	20	[[Paper]](https://proceedings.neurips.cc/paper/2020/hash/86c51678350f656dcc7f490a43946ee5-Abstract.html)		
* Does Unsupervised Architecture Representation Learning Help Neural Architecture Search?, NeurIPS 20 [[Paper]](https://proceedings.neurips.cc/paper/2020/hash/937936029af671cf479fa893db91cbdd-Abstract.html)	
* HM-NAS: Efficient Neural Architecture Search via Hierarchical Masking, ICCV 19 [[Paper]](https://openaccess.thecvf.com/content_ICCVW_2019/html/NeurArch/Yan_HM-NAS_Efficient_Neural_Architecture_Search_via_Hierarchical_Masking_ICCVW_2019_paper.html)
							
							
### Compiler for ML Systems							
* Romou: rapidly generate high-performance tensor kernels for mobile GPUs	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517020)		
* The CoRa Tensor Compiler: Compilation for Ragged Tensors with Minimal Padding, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/d3d9446802a44259755d38e6d163e820-Paper.pdf)	
* ROLLER: Fast and Efficient Tensor Compilation for Deep Learning	,	OSDI	22	[[Paper]](https://www.usenix.org/conference/osdi22/presentation/zhu)			
* A Deep Learning Based Cost Model for Automatic Code Optimization	,	MLSys	21	[[Paper]](https://proceedings.mlsys.org/paper_files/paper/2021/hash/3def184ad8f4755ff269862ea77393dd-Abstract.html)			
* TensorFlow Lite Micro: Embedded Machine Learning for TinyML Systems	,	MLSys	21	[[Paper]](https://proceedings.mlsys.org/paper_files/paper/2021/hash/d2ddea18f00665ce8623e36bd4e3c7c5-Abstract.html)			
* FlexTensor: An Automatic Schedule Exploration and Optimization Framework for Tensor Computation on Heterogeneous System	,	ASPLOS	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3373376.3378508)			
* Ordering Chaos: Memory-Aware Scheduling of Irregularly Wired Neural Networks for Edge Devices, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/9bf31c7ff062936a96d3c8bd1f8f2ff3-Paper.pdf)
* Rex: Preventing Bugs and Misconfiguration in Large Services Using Correlated Change Analysis	,	NSDI	20	[[Paper]](https://www.usenix.org/system/files/nsdi20-paper-mehta.pdf)			
* Rammer: Enabling Holistic Deep Learning Compiler Optimizations with rTasks	,	OSDI	20	[[Paper]]	(https://www.usenix.org/system/files/osdi20-ma.pdf)		
* Ansor: Generating High-Performance Tensor Programs for Deep Learning	,	OSDI	20	[[Paper]](https://www.usenix.org/system/files/osdi20-zheng.pdf)			
* Optimizing DNN Computation with Relaxed Graph Substitutions	,	MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/22.pdf)	
* Janus: Fast and Flexible Deep Learning via Symbolic Graph Execution of Imperative Programs	,	NSDI	19	[[Paper]](https://www.usenix.org/system/files/nsdi19-jeong.pdf)			
* TASO: optimizing deep learning computation with automatic generation of graph substitutions	,	SOSP	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3341301.3359630)			
* Intel® nGraph™ An Intermediate Representation,  Compiler,  and Executor for Deep Learning	,	MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/132.pdf)			
* Compiling machine learning programs via high-level tracing	,	MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/146.pdf)	
* TVM: An Automated End-to-End Optimizing Compiler for Deep Learning	,	OSDI	18	[[Paper]](https://www.usenix.org/conference/osdi18/presentation/chen)			
							
							
## Networking and Communication							

### Others

### Backscatter (Look at papers from Shyam @ University of Washington) 							
							
* Wind dispersal of battery-free wireless devices	,	Nature	2022	[[Paper]](https://www.nature.com/articles/s41586-021-04363-9)	(NO	ML)	
* OmniScatter: extreme sensitivity mmWave backscattering using commodity FMCW radar	,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538924)	(NO	ML)	
* Content-agnostic backscatter from thin air		MobiSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538930)	(NO	ML)	
* Low-Latency Visible Light Backscatter Networking with RetroMUMIMO	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568507)	(NO	ML)	
Simplifying Backscatter Deployment: Full-Duplex LoRa Backscatter, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-katanbaf.pdf) (NO ML)
* Microphone array backscatter: an application-driven design for lightweight spatial sound recording over the air,		MobiCom	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483265)	(NO	ML)	
* Self-Reconfgurable Micro-Implants for Cross-Tissue Wireless and Batteryless Connectivity	,	MobiCom	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3372224.3419216)	(NO	ML)	
* Towards scalable backscatter sensor mesh with decodable relay and distributed excitation	,	MobiSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388942)	(NO	ML)	
* VMscatter: A Versatile MIMO Backscatter	,	NSDI	20	[[Paper]](https://www.usenix.org/system/files/nsdi20-paper-liu.pdf)	(NO	ML)	
* Towards Battery-Free HD Video Streaming	,	NSDI	18	[[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/videobackscatter.pdf)	(NO	ML)	
* Charging a Smartphone Across a Room Using Lasers	,	UbiComp	18	[[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/laserpower.pdf)	(NO	ML)	
* LoRa Backscatter: Enabling The Vision of Ubiquitous Connectivity	,	UbiComp	17	[[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/loRaBackscatter.pdf)	(NO	ML)	
* Battery-Free Cellphone		UbiComp	17	[[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/phone.pdf) 	(NO ML)		
							
### LoRa							
* Saiyan: Design and Implementation of a Low-power Demodulator for LoRa Backscatter Systems	,	NSDI	22	[[Paper]](https://www.usenix.org/system/files/nsdi22-paper-guo.pdf)	(NO	ML)	
* Embracing LoRa Sensing with Device Mobility	,	SenSys	22	[[Paper]](https://people.cs.umass.edu/~dganesan/papers/SenSys22-LoRaSensingMobility.pdf)	(NO	ML)	
* HyLink: Towards High Throughput LPWANs with LoRa Compatible Communication	,	SenSys	22	[[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/HyLink-SenSys22.pdf)	(NO	ML)	
* Sensor-free Soil Moisture Sensing Using LoRa Signals		,MobiCom22	21	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3534608)	(NO	ML)	
* NELoRa: Towards Ultra-low SNR LoRa Communication with Neural-enhanced Demodulation	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485928)			
* LAVA: fine-grained 3D indoor wireless coverage for small IoT devices	,	SIGCOMM	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3452296.3472890)	(NO	ML)	
* Exploring LoRa for Long-range Through-wall Sensing	,	IMWUT/UbiComp	20	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3397326)	(NO	ML)	
* WIDESEE: Towards Wide-Area Contactless Wireless Sensing	,	SenSys	19	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3356250.3360031)	(NO	ML)	
							
### Under Water Communication							
* U-star: an underwater navigation system based on passive 3D optical identification tags	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517019)			
* Underwater Messaging Using Mobile Devices	,	SIGCOMM	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3544216.3544258)[[Code]](https://github.com/uw-x/watercomms)	(NO	ML)	
* Ultra-Wideband Underwater Backscatter via Piezoelectric Metamaterials	,	SIGCOMM	22	[[Paper]](https://www.mit.edu/~fadel/papers/U2B-paper.pdf)	(NO	ML)	
* Shrimp: a robust underwater visible light communication system,		MobiCom	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448616)	(NO	ML)	
* AmphiLight: Direct Air-Water Communication with Laser Light	,	NSDI	20	[[Paper]](https://www.usenix.org/conference/nsdi20/presentation/carver)			
* Underwater backscatter networking	,	SIGCOMM	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3341302.3342091)	(NO	ML)	
* Networking across boundaries: enabling wireless communication through the water-air interface		SIGCOMM	18	[[Paper]](https://dl.acm.org/doi/10.1145/3230543.3230580)	(NO	ML)	
							
							
## Security and Privacy							
							
### Security of AIoT							
* Client-optimized algorithms and acceleration for encrypted compute offloading	,	ASPLOS	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507737)			
* SOTER: Guarding Black-box Inference for General Neural Networks at the Edge	,	ATC	22	[[Paper]](https://www.usenix.org/system/files/atc22-shen.pdf)			
* G2Auth: secure mutual authentication for drone delivery without special user-side hardware,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538941)	(NO	ML)	
* A Tale of Two Models Constructing Evasive Attacks on Edge Models, MLSys 22 [[Paper]][(](https://proceedings.mlsys.org/paper_files/paper/2022/file/92cc227532d17e56e07902b254dfad10-Paper.pdf))
* Light Auditor: Power Measurement Can Tell Private Data Leakage through IoT Covert Channels,		SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568535)			
* HideSeeker: Uncover the Hidden Gems in Obfuscated Images,		SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568514)	
* FastZIP: faster and more secure zero-interaction pairing	,	MobiSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467883)	(NO	ML)	
* Sniffing Visible Light Communication Through Walls,		MobiCom	20	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419187)	(NO	ML)	
* DarkneTZ: towards model privacy at the edge using trusted execution environments,		MobiSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388946)			
* SecWIR: securing smart home IoT communications via wi-fi routers with embedded intelligence, MobiSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388941)
* Privacy-Preserving Bandits, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/42a0e188f5033bc65bf8d78622277c4e-Paper.pdf)
* Occlumency: Privacy-preserving Remote Deep-learning Inference Using SGX,		MObiCom	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345447)			
* Brain Password: A Secure and Truly Cancelable Brain Biometrics for Smart Headwear,		MobiSys	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210344)	(NO	ML)
							
### Federated Learning Systems			
* PyramidFL: a fine-grained client selection framework for efficient federated learning	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517017)			
* FedBalancer: data and pace control for efficient federated learning on heterogeneous clients	,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/10.1145/3498361.3538917)			
* LightSecAgg: a Lightweight and Versatile Design for Secure Aggregation in Federated Learning, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/d2ddea18f00665ce8623e36bd4e3c7c5-Paper.pdf)
* Papaya: Practical, Private, and Scalable Federated Learning, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/f340f1b1f65b6df5b5e3f94d95b11daf-Paper.pdf)
* FedRolex: Model-Heterogeneous Federated Learning with Rolling Sub-Model Extraction,		NeurIPS	22	[[Paper]](https://openreview.net/forum?id=OtxyysUdBE)			
* FedSEA: A Semi-Asynchronous Federated Learning Framework for Extremely Heterogeneous Devices,		SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568538)			
* Hermes: an efficient federated learning framework for heterogeneous mobile clients,		MobiCom	21	[[Paper]](https://dl.acm.org/doi/10.1145/3447993.3483278)			
* PPFL: privacy-preserving federated learning with trusted execution environments,		MobiSys	21	[[Paper]](https://dl.acm.org/doi/10.1145/3458864.3466628)			
* ClusterFL: a similarity-aware federated learning system for human activity recognition,		MobiSys	21	[[Paper]](https://dl.acm.org/doi/10.1145/3458864.3467681)			
* Oort: Efficient Federated Learning via Guided Participant Selection,		OSDI	21	[[Paper]](https://www.usenix.org/system/files/osdi21-lai.pdf)			
* FedDL: Federated Learning via Dynamic Layer Sharing for Human Activity Recognition,		SenSys	21	[[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485946)			
* FedMask: Joint Computation and Communication-Efficient Personalized Federated Learning via Heterogeneous Masking,		SenSys	21	[[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485929)			
* Billion-scale federated learning on mobile clients: a submodel design with tunable privacy,		MobiCom	20	[[Paper]](https://dl.acm.org/doi/10.1145/3372224.3419188)	
* Federated Optimization in Heterogeneous Networks, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/38af86134b65d0f10fe33d30dd76442e-Paper.pdf)
* Towards Federated Learning at Scale: System Design,		MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/193.pdf)		
* Federated Kernelized Multi-Task Learning,		MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/30.pdf)			
							
							
## AIoT Systems and their Applications							
							
### AIoT Systems for Healthcare and Social Good							
* SmartLens : Sensing Eye Activities Using Zero-power Contact Lens,		MobiCom	22	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560532)	(NO	ML)	
* Out-Clinic Pulmonary Disease Evaluation via Acoustic Sensing and Multi-Task Learning on Commodity Smartphones	, SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568437)			
* Your Smart Speaker Can “Hear” Your Heartbeat!, IMWUT/UbiComp	21	[[Paper]](https://dl.acm.org/doi/10.1145/3432237)	(NO	ML)	
* U-Verse: a miniaturized platform for end-to-end closed-loop implantable internet of medical things systems		SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360026)	(NO	ML)	
* PDLens: smartphone knows drug effectiveness among Parkinson's via daily-life activity fusion,		MobiCom	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3372224.3380889)		
* When Virtual Reality Meets Internet of Things in the Gym: Enabling Immersive Interactive Machine Exercises, ubiComp 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3214281)	
* Contactless Infant Monitoring using White Noise,		MobiCom	19	[[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/whitenoise.pdf)	(NO	ML)	
* MobileDeepPill: A Small-Footprint Mobile Deep Learning System for Recognizing Unconstrained Pill Images,		MobiSys	17	[[Paper]](https://dl.acm.org/doi/10.1145/3081333.3081336)			
* DeepASL: Enabling Ubiquitous and Non-Intrusive Word and Sentence-Level Sign Language Translation,		SenSys	17	[[Paper]](https://dl.acm.org/doi/10.1145/3131672.3131693)

			
### AIoT Systems for Autonomous Driving							
							
### AIoT Systems for Video Analytics 							
* NeuriCam: Key-Frame Video Super-Resolution and Colorization for IoT Cameras,		MobiCom	23	[[Paper]](https://arxiv.org/abs/2207.12496)[[Code]](https://github.com/vb000/NeuriCam)	
* Multiview Transformers for Video Recognition, CVPR 22 [[Paper]](https://openaccess.thecvf.com/content/CVPR2022/html/Yan_Multiview_Transformers_for_Video_Recognition_CVPR_2022_paper.html)		
* AccMPEG: Optimizing Video Encoding for Video Analytics, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/98f13708210194c475687be6106a3b84-Paper.pdf)
* AutoMatch: Leveraging Traffic Camera to Improve Perception and Localization of Autonomous Vehicles,		SenSys	22	[[Paper]](https://dl.acm.org/doi/10.1145/3560905.3568519)			
* FollowUpAR: enabling follow-up effects in mobile AR applications,		MobiSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467675)			
* EMO: real-time emotion recognition from single-eye images for resource-constrained eyewear devices,		MobiSys	20	[[Paper]](https://dl.acm.org/doi/10.1145/3386901.3388917)			
* Distream: Scaling Live Video Analytics with Workload-Adaptive Distributed Edge Intelligence,		SenSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430721)			
* TSM: Temporal Shift Module for Efficient Video Understanding,		ICCV	19	[[Paper]](https://openaccess.thecvf.com/content_ICCV_2019/html/Lin_TSM_Temporal_Shift_Module_for_Efficient_Video_Understanding_ICCV_2019_paper.html)			
* Scaling Video Analytics on Constrained Edge Nodes,		MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/197.pdf)			
* When IoT met Augmented Reality: Visualizing the Source of the Wireless Signal in AR View,		MobiSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326079)			
* SmrtFridge: IoT-based,  user interaction-driven food item & quantity sensing,		SenSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360028)			
* Potluck: Cross-Application Approximate Deduplication for Computation-Intensive Mobile Applications,		ASPLOS	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3173162.3173185)			
* EVA: An Efficient System for Exploratory Video Analysis,		MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/22.pdf)			
* Efficient Multi-Tenant Inference on Video using Microclassifiers,		MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/133.pdf)			
* Dynamic Stem-Sharing for Multi-Tenant Video Processing,		MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/149.pdf)			
* Rubiks: Practical 360-Degree Streaming for Smartphones,		MobiSys	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210323)	(NO	ML)	


### AIoT Systems for Agriculture 




