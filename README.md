# Artificial Intelligence of Things: A Survey  
> Artificial Intelligence of Things: A Survey

> *Shakhrul Iman Siam<sup>1</sup>, Hyunho Ahn<sup>1</sup>, Li Liu<sup>2</sup>, Samiul Alam<sup>1</sup>, Hui Shen<sup>1</sup>, Zhichao Cao<sup>2</sup>, Ness Shroff<sup>1</sup>, Bhaskar Krishnamachari<sup>3</sup>, Mani Srivastava<sup>4</sup>, Mi Zhang<sup>1</sup>*

> <sup>1</sup>The Ohio State University, <sup>2</sup>Michigan State University, <sup>3</sup>University of Southern California, <sup>4</sup>University of California, Los Angeles

## ❤️ Community Support
This repository is maintained by <ins>[shakhrulsiam268](https://github.com/shakhrulsiam268)</ins> (siam.5@osu.edu), <ins>[HyunhoAhn](https://github.com/HyunhoAhn)</ins> (ahn.377@osu.edu), and <ins>[mi-zhang](https://github.com/mi-zhang)</ins> (mizhang.1@osu.edu). We welcome feedback, suggestions, and contributions that can help improve this survey and repository so as to make them valuable resources to benefit the entire community.

We will actively maintain this repository by incorporating new research as it emerges. If you have any suggestions regarding our taxonomy, find any missed papers, or update any preprint arXiv paper that has been accepted to some venue, feel free to send us an email or submit a **pull request** using the following markdown format.

```markdown
Paper Title, <ins>Conference/Journal/Preprint, Year</ins>  [[pdf](link)] [[other resources](link)].
```

## 📌 What is This Survey About?
Artificial Intelligence of Things (AIoT) is one of the most exciting and promising areas that lies at the intersection of Internet of Things (IoT) and modern Artificial Intelligence (AI). At its core, AIoT is grounded on three key com-
ponents: sensing, computing, and networking & communication. Compared to conventional IoT, the computing component of AIoT is concentrated on AI-oriented compute tasks. Moreover, the sensing and networking & communication components of AIoT are AI empowered. It is these two key distinctions that allow AIoT to empower billions of everyday devices with breakthroughs brought by modern AI. 

In this survey, we provide a systematic and comprehensive review of AIoT research. We examine AIoT literature related to sensing, computing, and networking & communication. We also review domain-specific AIoT systems that are designed for various important application domains. We primarily focus on literature on sensing, computing, networking & communication, and domain-specific AIoT systems that are built upon modern AI techniques such as deep learning, foundation models, and Generative AI.

As both IoT and AI become increasingly critical to our society, we believe AIoT is emerging as an essential research field. We hope this survey will serve as a valuable resource for those engaged in AIoT research and act as a catalyst for future explorations to bridge gaps and drive advancements in this exciting field.

<p align="center">
<img src="https://github.com/AIoT-MLSys-Lab/AIoT-Survey/blob/main/img/AIoT_Overview.PNG" width="40%" height="40%"></p>

## :film_strip: OSU AIoT Seminar Series
Besides the survey and the repository, we also host the OSU AIoT Seminar Series where we invite speakers at the frontier of AIoT from both academia and industry to talk about their works. The talk videos are available at: https://sites.google.com/view/osu-aiot-seminar.

## 📖 Table of Content
  - [Sensing (Total: 319)](#sensing)
    - [Motion Sensing](#motion-sensing)
    - [Wireless Sensing](#wireless-sensing)
    	- [RFID Sensing](#rfid-sensing)
    	- [Wi-Fi Sensing](#wi-fi-sensing)
    	- [mmWave Sensing](#mmwave-sensing)
    	- [TeraHertz Sensing](#teraHertz-sensing)
    	- [UWB Sensing](#uwb-sensing)
     	- [Cellular Sensing](#cellular-sensing)
    	- [LoRa Sensing](#lora-sensing)
       	- [LTE Sensing](#lte-sensing)
    	- [Bluetooth Sensing](#bluetooth-sensing)
     	- [Aerial Sensing](#ariel-sensing)
      	- [NFC Sensing](#nfc-sensing)
      	- [RF Sensing](#rf-sensing)
    - [Vision Sensing](#vision-sensing)
    - [Acoustic Sensing](#acoustic-sensing)
    - [Multi-Modal Sensing](#multi-modal-sensing)
    - [Earable Sensing](#earable-sensing)
    - [Visible Light Sensing](#light-sensing)
    - [Magentic Sensing](#magnetic-sensing)
    - [Cross-Medium Sensing](#cross-medium-sensing)
    - [Generative AI for Sensing](#generative-ai-for-sensing)
  - [Computing (Total: 154)](#computing)
    - [On-Device Inference](#on-device-inference)
      	- [Model Compression](#model-compression)
      	- [Inference Optimization](#inference-optimization)
      	- [Multi-Tenant Inference](#multi-tenant-inference)
      	- [Cross-Processor Inference](#cross-processor-inference)
      	- [Runtime Adaptation](#runtime-adaptation)
    - [Offloading](#offloading)
      - [Model Partitioning](#model-partitioning)
      - [Workload Partitioning](#workload-partitioning)
      - [Communication Optimization](#communication-optimization)   
      - [Privacy-Preserving Offloading](#privacy-preserving-offloading)
    - [On-Device Training](#on-device-training)
    	- [Training on a Single Device](#training-on-a-single-device)
    	- [Training across Distributed Devices](#training-on-distributed-devices)
    - [Federated Learning](#federated-learning)
    	- [Data Heterogeneity](#data-heterogeneity)
     	- [Communication Optimization](#communication-optimization)
    	- [System Heterogeneity](#system-heterogeneity)
      	- [Personalization](#personalization)
        - [Client Selection](#client-selection)
      	- [Model Heterogeneity](#model-heterogeneity)
       	- [Frameworks and Benchmarks](#frameworks-and-benchmarks)
    - [Model Deployment on the Edge](#model-deployment-on-the-edge)
    - [Compilers for AIoT](#compilers-for-aiot)
    - [AI Agents for AIoT](#ai-agents-for-aiot)
  - [Networking and Communication (Total: 337)](#networking-and-communication)
    - [Battery](#user-content-battery)
      - [Cellular](#user-content-cellular)
      - [WiFi](#user-content-wifi)
      - [Acoustic](#user-content-acoustic)
      - [Visible Light](#user-content-visible-Light)
      - [Bluetooth](#user-content-bluetooth)
      - [Millimeter-Wave](#user-content-millimeter-Wave)
      - [UWB](#user-content-uwb)
      - [TV Whitespace](#user-content-tv-whitespace)
      - [LoRa/LoRaWAN](#user-content-loralorawan)
      - [LPWAN](#user-content-lpwan)
      - [SDR](#user-content-sdr)
      - [CTC](#user-content-ctc)
      - [Multi-band Operation](#user-content-multi-band)
      - [... ](#user-content-other-sensor-network)
    - [Batteryless](#user-content-batteryless)
      - [LoRa](#user-content-lora)
      - [Millimeter-Wave](#user-content-millimeter-wave-1)
      - [WiFi](#user-content-wifi-1)
      - [RFID](#user-content-rfid)
      - [Visible Light](#user-content-visible-Light-1)
      - [Acoustic](#user-content-acoustic-1)
      - [...](#user-content-other-batteryless-works)
    - [Hybrid](#hybrid)
    - [Others](#na) 
  - [Domain-specific AIoT Systems (Total: 256)](#domain-specific-aiot-systems)
    - [AIoT Systems for Healthcare and Well-being](#aiot-systems-for-healthcare-and-well-being)
    - [AIoT Systems for Video Streaming](#aiot-systems-for-video-streaming)
    - [AIoT Systems for Video Analytics](#aiot-systems-for-video-analytics)
    - [AIoT Systems for Autonomous Driving](#aiot-systems-for-autonomous-driving)
    - [AIoT Systems for AR/VR/MR](#aiot-systems-for-arvrmr)
    - [AIoT Systems for Drones](#aiot-systems-for-drones)
    - [AIoT Systems for Satellites](#aiot-systems-for-satellites)
    - [AIoT Systems for Agriculture](#aiot-systems-for-agriculture)
    - [AIoT Systems for Biology](#aiot-systems-for-biology)
    	
⚡Note: "No ML" denotes no machine learning techniques are used. "ML" denotes traditional machine learning techniques are used. "DL" denotes deep learning techniques are used. "GenAI" denotes generative AI techniques are used.

<a name="sensing"></a>
## 🌡️ Sensing (319)

<a name="motion-sensing"></a>
### 👋 Motion Sensing (Total: 10 | No ML(1) | ML(2) | DL(7))
#### Human Activity Recognition
* Practically Adopting Human Activity Recognition, MobiCom 23 [[Paper]](https://dapowan.github.io/files/UniHAR.pdf) (DL)
* Real-Time Tracking of Smartwatch Orientation and Location by Multitask Learning, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568548) (DL)
* LIMU-BERT: Unleashing the Potential of Unlabeled Data for IMU Sensing Applications, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485937) (DL)
* Transferring Activity Recognition Models for New Wearable Sensors with Deep Generative Domain Adaptation, IPSN 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3302506.3310391) (DL)
* SenseHAR: a robust virtual activity sensor for smartphones and wearables, SenSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3356250.3360032) (DL)
* Closing the Gaps in Inertial Motion Tracking, MobiCom 18 [[Paper]](https://synrg.csl.illinois.edu/papers/muse-mobicom18.pdf) (No ML)
* Synchronous Dynamic View Learning: A Framework for Autonomous Training of Activity Recognition Models using Wearable Sensors, IPSN 17 [[Paper]](https://dl.acm.org/doi/10.1145/3055031.3055087) (ML)
* I am a Smartwatch and I can Track my User’s Arm, MobiSys 16 [[Paper]](https://synrg.csl.illinois.edu/papers/ArmTrak_Mobisys.pdf) (ML)
#### Arm Tracking
* Real-time Arm Skeleton Tracking and Gesture Inference Tolerant to Missing Wearable Sensors, MobiSys 19 [[Paper]](https://yangliu-cs.github.io/YangLiu-CS/paper/2019-MobiSys-ArmTroi.pdf) (DL)
* Lasagna: Towards Deep Hierarchical Understanding and Searching over Mobile Sensing Data, MobiCom 16 [[Paper]](http://tns.thss.tsinghua.edu.cn/~cihangliu/papers/lasagna.pdf) (DL)  


<a name="wireless-sensing"></a>
### 🌐 Wireless Sensing (145)
<a name="rfid-sensing"></a>
#### 🏷️ RFID Sensing (Total: 29 | No ML(23) | ML(1) | DL(5))
* A Handheld Fine-Grained RFID Localization System with Complex-Controlled Polarization, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592504) (NO ML)
* Fast, Fine-grained, and Robust Grouping of RFIDs, MobiCom 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3570361.3592510) (NO ML)
* MetaSight: Localizing Blocked RFID Objects by Modulating NLOS Signals via Metasurfaces, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538947) (NO ML)
* A Passive Eye-in-Hand “Camera” for Minature Robots, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568505) (NO ML)
* ShakeReader: ‘Read’ UHF RFID using Smartphone, INFOCOM 21 [[Paper]](https://web.comp.polyu.edu.hk/csyqzheng/papers/ShakeReader-INFOCOM21.pdf) (NO ML)
* Thermotag: item-level temperature sensing with a passive RFID tag, MobiSys 21 [[Paper]](https://cs.nju.edu.cn/liujia/papers/mobisys21-themotag.pdf) (NO ML)
* RFGo: A Seamless Self-checkout System for Apparel Stores Using RFID, MobiCom 20 [[Paper]](https://genesys-lab.org/papers/RFGo-Mobicom.pdf) (DL)
* Food and Liquid Sensing in Practical Environments using RFIDs, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-ha.pdf) (DL)
* Exploring commodity RFID for contactless sub-millimeter vibration sensing, SenSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3384419.3430771) (NO ML)
* Sensing Finger Input Using An RFID Transmission Line, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430712) (NO ML)
* RTSense: RFID based Temperature Sensing, SenSys 20 [[Paper]](https://www.swadhinpradhan.com/papers/rtsense.pdf) (NO ML)
* 3D-OmniTrack: 3D Tracking with COTS RFID Systems, IPSN 19 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/2019.4.pdf) (NO ML)
* Are RFID Sensing Systems Ready for the Real World?, MobiSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3307334.3326084) (NO ML)
* Detecting Misplaced RFID Tags on Static Shelved Items, MobiSys 19 [[Paper]](https://rtcl.eecs.umich.edu/rtclweb/assets/publications/2019/luo-mobisys19.pdf) (ML)
* RFID based real-time recognition of ongoing gesture with adversarial learning, SenSys 19 [[Paper]](https://dl.acm.org/doi/10.1145/3356250.3360045) (DL)
* FaHo: deep learning enhanced holographic localization for RFID tags, SenSys 19 [[Paper]](https://dapowan.github.io/files/FaHo.pdf) (DL)
* Tagtag: material sensing with commodity RFID, SenSys 19 [[Paper]](https://dl.acm.org/doi/10.1145/3356250.3360027) (NO ML)
* Orientation-aware RFID Tracking with Centimeter-level Accuracy, IPSN 18 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/2018.8.pdf) (NO ML)
* Challenge: RFID Hacking for Fun and Profit, MobiCom 18 [[Paper]](http://web.cs.ucla.edu/~omid/Papers/Mobicom18a.pdf) (NO ML)
* WiSh: Towards a Wireless Shape-aware World using Passive RFIDs, MobiSys 18 [[Paper]](https://www.witechlab.com/papers/wish-mobisys2018.pdf) (NO ML)
* Minding the Billions: Ultra-wideband Localization for Deployed RFID Tags, MobiCom 17 [[Paper]](https://www.mit.edu/~fadel/papers/RFind-paper.pdf) (NO ML)
* TagScan: Simultaneous Target Imaging and Material Identification with Commodity RFID Devices, MobiCom 17 [[Paper]](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=4878&context=sis_research) (NO ML)
* RIO: A Pervasive RFID-based Touch Gesture Interface, MobiCom 17 [[Paper]](https://dl.acm.org/doi/10.1145/3117811.3117818) (NO ML)
* Enabling gesture-based interactions with objects, MobiSys 17 [[Paper]](https://core.ac.uk/download/pdf/286384108.pdf) (NO ML)
* Gyro in the Air: Tracking 3D Orientation of Batteryless Internet-of-Things, MobiCom 16 [[Paper]](http://xyzhang.ucsd.edu/papers/TWei_MobiCom16_Tagyro.pdf) (NO ML)
* 3D Real-time Indoor Localization via Broadband Nonlinear Backscatter in Passive Devices with Centimeter Precision, MobiCom 16 [[Paper]](https://yfmascgy.github.io/papers/3d-localization.pdf) (NO ML)
* Analog On-Tag Hashing: Towards Selective Reading as Hash Primitives in Gen2 RFID Systems, MobiCom 16 [[Paper]](https://web.comp.polyu.edu.hk/csyanglei/data/files/tash-mobicom17.pdf) (NO ML)
* The Design and Implementation of a Mobile RFID Tag Sorting Robot, MobiSys 16 [[Paper]](https://discovery.ucl.ac.uk/id/eprint/1493115/1/mobitagbot_for_rps.pdf) (NO ML)
* Deep Learning for RFID-Based Activity Recognition, SenSys 16 [[Paper]](https://dl.acm.org/doi/10.1145/2994551.2994569) (DL)

<a name="wi-fi-sensing"></a>
#### 🌐 Wi-Fi Sensing (Total: 55 | No ML(24) | ML(11) | DL(20))
##### Human Activity Recognition
* SiFall: Practical Online Fall Detection with RF Sensing, SenSys 22 [[Paper]](https://arxiv.org/pdf/2301.03773.pdf) (DL)
* Counting a stationary crowd using off-the-shelf wifi, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3468012) (NO ML)
* OneFi: One-Shot Recognition for Unseen Gesture via COTS WiFi, SenSys 21 [[Paper]](https://ruixiao24.github.io/files/rui_onefi.pdf) [[Code]](https://github.com/ruixiao24/onefi) (DL)
* RF-net: a unified meta-learning framework for RF-enabled one-shot human activity recognition,	SenSys	20 [[Paper]](https://arxiv.org/pdf/2111.04566.pdf) (DL)
* Zero-Effort Cross-Domain Gesture Recognition with Wi-Fi, MobiSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3307334.3326081) (DL)
* Widar2.0: Passive Human Tracking with a Single Wi-Fi Link, MobiSys 18 [[Paper]](https://www.cswu.me/papers/mobisys18_widar2.0_paper.pdf) (ML)
* Towards Environment Independent Device Free Human Activity Recognition, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241548) (DL)
* CrossSense: Towards Cross-Site and Large-Scale WiFi Sensing, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241570) (DL)
* WiWho: WiFi-Based Person Identification in Smart Spaces, IPSN 16 [[Paper]](https://ieeexplore.ieee.org/document/7460727) (ML)


##### Indoor Localization
* Understanding Localization by a Tailored GPT, Mobisys 24[[Paper]](https://dl.acm.org/doi/10.1145/3643832.3661869) (DL)
* BIFROST: Reinventing WiFi Signals Based on Dispersion Effect for Accurate Indoor Localization, SensSys 23 [[Paper]](https://wangwg1996.github.io/files/PDF/BIFROST_conf.pdf) (NO ML)
* Enabling Ubiquitous Wi-Fi Sensing with Beamforming Reports, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/10.1145/3603269.3604817) (ML)
* RIScan: RIS-aided Multi-user Indoor Localization Using COTS Wi-Fi, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625806) (NO ML)
* Placement Matters: Understanding the Effects of Device Placement for WiFi Sensing, IMWUT 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3517237) (NO ML)
* Experience: pushing indoor localization from laboratory to the wild, MobiCom 22  [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560546) (Best Community Contribution Runner-ups) (DL)
* Accurate Ubiquitous Localization with Off-the-Shelf IEEE 802.11ac Devices, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3468850) (NO ML)
* WiForce: Wireless Sensing and Localization of Contact Forces on a Space Continuum, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-gupta.pdf) (NO ML)
* Deep learning based wireless localization for indoor navigation, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3380894) (DL)
* LocAP: Autonomous Millimeter Accurate Mapping of WiFi Infrastructure, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-ayyalasomayajula.pdf) (NO ML)
* Multipath Triangulation: Decimeter-level WiFi Localization and Orientation with a Single Unaided Receiver, MobiSys 18 [[Paper]](https://elahe.web.illinois.edu/Elahe%20Soltan_files/papers/MobiSys18_MonoLoco_CameraReady.pdf) (NO ML)
* Verification: Accuracy Evaluation of WiFi Fine Time Measurements on an Open Platform, MobiCom 18 [[Paper]](https://winlab.rutgers.edu/~gruteser/papers/ftm_mobicom.pdf) (NO ML)
* Decimeter-Level Localization with a Single WiFi Access Point, NSDI 16 [[Paper]](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-vasisht.pdf) (NO ML)
* LiFS: Low Human-Effort Device-Free Localization with Fine-Grained Subcarrier Information, MobiCom 16 [[Paper]](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=4390&context=sis_research)(NO ML)

 
##### Imaging
* Wiffract: A New Foundation for RF Imaging via Edge Tracing, MobiCom 22 [[Paper]](https://web.ece.ucsb.edu/~ymostofi/papers/PallaproluKoranyMostofi_MobiCom2022.pdf) (ML)
* Wi-Fi See It All: Generative Adversarial Network-augmented Versatile Wi-Fi Imaging, SenSys 20 [[Paper]](https://cse.msu.edu/~caozc/papers/sensys20-chen.pdf) (DL)
* 3D Through-Wall Imaging with Unmanned Aerial Vehicles Using WiFi, IPSN 17 [[Paper]](https://web.ece.ucsb.edu/~ymostofi/papers/IPSN17_KaranamMostofi.pdf) (NO ML)


##### 3D Human Reconstruction
* Construct 3D Hand Skeleton with Commercial WiFi, SenSys 23 [[Paper]](https://arxiv.org/pdf/2312.15507) (DL)
* Wi-Mesh: A WiFi Vision-based Approach for 3D Human Mesh Construction, SenSys 22 [[Paper]](https://arxiv.org/pdf/2210.10957.pdf) (DL)
* Towards 3D human pose construction using wifi, MobiCom 20 [[Paper]](https://cse.buffalo.edu/~lusu/papers/MobiCom2020.pdf) (DL)

##### Gesture Recognition
* RF-Diffusion: Radio Signal Generation via Time-Frequency Diffusion, MobiCom 24 [[Paper]](https://arxiv.org/pdf/2404.09140) (DL)
* UniFi: A Unified Framework for Generalizable Gesture Recognition with Wi-Fi Signals Using Consistency-guided Multi-View Networks, IMWUT 24 [[Paper]](https://dl.acm.org/doi/10.1145/3631429) (DL)
* SLNet: A Spectrogram Learning Neural Network for Deep Wireless Sensing, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-yang-zheng.pdf) (DL)
* MUSE-Fi: Contactless MUti-person SEnsing Exploiting Near-field Wi-Fi Channel Variation, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613290) (DL)
* RF-URL: unsupervised representation learning for RF sensing, MobiCom 22 [[Paper]](http://staff.ustc.edu.cn/~dongheng/dhfiles/rf-url.pdf) (DL)
* Solving the WiFi Sensing Dilemma in Reality Leveraging Conformal Prediction, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568529) (DL)
* Understanding WiFi signal frequency features for position-independent gesture sensing, IEEE Transactions on Mobile Computing 22 [[Paper]](https://hal.science/hal-03363402/file/Understanding_WiFi_Signal_Frequency_Features_for_Position-Independent_Gesture_Sensing.pdf) (NO ML)
* Towards Position-Independent Sensing for Gesture Recognition with Wi-Fi, IMWUT 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3463504) (NO ML)
* RF-based Inertial Measurement, SIGCOMM 19 [[Paper]](https://cswu.me/papers/sigcomm19_rim_paper.pdf) (NO ML)
* Multi-User Gesture Recognition Using WiFi, MobiSys 18 [[Paper]](https://raghavhv.wordpress.ncsu.edu/files/2018/06/mobisys18-31-hampapur.pdf) (NO ML)
* Position and Orientation Agnostic Gesture Recognition Using WiFi, MobiSys 17 [[Paper]](https://dl.acm.org/doi/10.1145/3081333.3081340) (ML)
* WiFi-Enabled Smart Human Dynamics Monitoring, SenSys 17 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3131672.3131692) (ML)
* Calibrating Time-variant, Device-specific Phase Noise for COTS WiFi Devices, SenSys 17 [[Paper]](https://netstech.org/wp-content/uploads/2018/10/phase_calibration_sensys17.pdf) (NO ML)
* HeadScan: A Wearable System for Radio-based Sensing of Head and Mouth-related Activities, IPSN 16 [[Paper]](https://innovationcenter.msu.edu/wp-content/uploads/2021/07/HeadScan-A-Wearable-System-for-Radio-Based-Sensing-of-Head-and-Mouth-Related-Activities-1.pdf) (ML)
* BodyScan: Enabling Radio-based Sensing on Wearable Devices for Contactless Activity and Vital Sign Monitoring, MobiSys 16 [[Paper]](https://mi-zhang.github.io/papers/2016_MobiSys_BodyScan.pdf) (ML)


##### Respiration Monitoring
* MultiSense: Enabling Multi-person Respiration Sensing with Commodity WiFi, IMWUT 20 [[Paper]](https://hal.science/hal-03363355v1/file/3411816.pdf) (NO ML)
* FarSense: Pushing the Range Limit of WiFi-based Respiration Sensing with CSI Ratio of Two Antennas, IMWUT 19 [[Ppaper]](https://arxiv.org/pdf/1907.03994) (NO ML)

##### Tracking
* Tracking from One Side -- Multi-Person Passive Tracking with WiFi Magnitude Measurements, IPSN 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3302506.3310399) (NO ML)
* Toward Reliable Localization by Unequal AoA Tracking, MobiSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3307334.3326103) (NO ML)
* On the Feasibility of Wi-Fi Based Material Sensing, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345442) (ML)
* mD-Track: Leveraging Multi-Dimensionality for Passive Indoor Wi-Fi Tracking, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300133) (ML)
* Magnitude-Based Angle-of-Arrival Estimation, Localization, and Target Tracking, IPSN 18 [[Paper]](https://web.ece.ucsb.edu/~ymostofi/papers/IPSN18_KaranamKoranyMostofi.pdf) (NO ML)

##### Copresence and proximity detection
* Next2You: Robust Copresence Detection Based on Channel State Information, SenSys 23 [[Paper]](https://arxiv.org/pdf/2111.05224) (DL)
* Proximity Detection with Single-Antenna IoT Devices, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300120) (NO ML)

##### Human-Computer Interaction
* Exploring Multiple Antennas for Long-range WiFi Sensing, IMWUT 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3494979) (NO ML)
* LiveTag: Sensing Human-Object Interaction through Passive Chipless WiFi Tags, NSDI 18 [[Paper]](https://www.usenix.org/system/files/conference/nsdi18/nsdi18-gao.pdf) (ML)


<a name="mmwave-sensing"></a>
#### 🌫️ mmWave Sensing (Total: 23 | No ML(7) | ML(3) | DL(13))
##### Human Mesh Reconstruction
* mm3DFace: Nonintrusive 3D Facial Reconstruction Leveraging mmWave Signals, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596839) (DL)
* m3Track: mmWave-based Multi-User 3D Posture Tracking, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538926) (DL)
* M4esh: mmWave-Based 3D Human Mesh Construction for Multiple Subjects,	SenSys	22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568545) (DL)
* Synthesized Millimeter-Waves for Human Motion Sensing, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568542) (DL)
* mmMesh: towards 3D real-time dynamic human mesh construction using millimeter-wave, MobiSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3458864.3467679) (DL)

  
##### Human Activity Recognition
* mmFER: Millimetre-wave Radar based Facial Expression Recognition for Multimedia IoT Applications, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3592515) (DL)
* Towards Generalized mmWave-based Human Pose Estimation through Signal Augmentation, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613302) (DL)
* SPARCS: A Sparse Recovery Approach for Integrated Communication and Human Sensing in mmWave Systems, IPSN 22 [[Paper]](https://arxiv.org/pdf/2205.03263.pdf) (DL)

##### Human Voice Recognition
* FerroTag: a paper-based mmWave-scannable tagging infrastructure, SenSys 19 [[Paper]](https://dl.acm.org/doi/10.1145/3356250.3360019) (Best Paper) (ML)

##### Object Recognition
* Fusang: Graph-inspired Robust and Accurate Object Recognition on Commodity mmWave Devices, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596849) [[Code]](https://github.com/OpenNISLab/Pro-Fusang) (DL)

##### Map Generation
* See through smoke: robust indoor mapping with low-cost mmWave radar,	MobiSys	20 [[Paper]](https://arxiv.org/pdf/1911.00398.pdf) (DL)

##### Temperature Monitoring
* ThermoWave: A New Paradigm of Wireless Passive Temperature Monitoring via mmWave Sensing, MobiCom 20 [[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-mobicom2020b.pdf) (DL)

##### Localization
* Hawkeye: Hectometer-range Subcentimeter Localization for Large-scale mmWave Backscatter, MobiSys 23 [[Paper]](https://arxiv.org/pdf/2301.02402.pdf) (NO ML)
* Accurate 3D Localization for 60 GHz Networks, SenSys 18 [[Paper]](https://dl.acm.org/doi/10.1145/3274783.3274852) (NO ML)
* Augmenting mmWave localization accuracy through sub-6 GHz on off-the-shelf devices, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538920) (NO ML)
* Millimetro: mmWave Retro-Reflective Tags for Accurate, Long Range Localization, MobiCom 21 [[Paper]](https://swarunkumar.com/papers/millimetro-mobicom2021.pdf) (NO ML)

##### Measurement and displacement sensing
* Platypus: Sub-mm Micro-Displacement Sensing with Passive Millimeter-wave Tags As "Phase Carriers", IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586965) (NO ML)
* mmVib: micrometer-level vibration measurement with mmwave radar, MobiCom 20 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/mmVib_MobiCom2020.pdf) (NO ML)
* Dancing Waltz with Ghosts: Measuring Sub-𝑚𝑚-Level 2D Rotor Orbit with a Single mmWave Radar, IPSN 21 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/GWaltz_IPSN2021.pdf) (ML)
+ Push the Limit of Single-Chip mmWave Radar-Based Egomotion Estimation with Moving Objects in FoV, SenSys 23 [[Paper]](https://dl.acm.org/doi/10.1145/3625687.3625795) (NO ML)
+ RF Genesis: Zero-Shot Generalization of mmWave Sensing through Simulation-Based Data Synthesis and Generative Diffusion Models, SenSys 23 [[Paper]](http://xyzhang.ucsd.edu/papers/Xingyu.Chen_SenSys23_RFGen.pdf) (GenAI)
+ Osprey: A mmWave Approach to Tire Wear Sensing, MobiSys 20 [[Paper]](https://swarunkumar.com/papers/osprey-mobisys2020.pdf) (ML)


<a name="lte-sensing"></a>
#### LTE Sensing (Total: 4 | No ML(3) | ML(0) | DL(1))
##### Traffic Monitoring
* LTE-based Pervasive Sensing Across Indoor and Outdoor, Sensys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485943)
##### Soil Moisture Monitoring
LTE-Based Low-Cost and Low-Power Soil Moisture Sensing, Sensys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3560905.3568525)

<a name="lora-sensing"></a>
#### LoRa Sensing (Total: 4 | No ML(3) | ML(0) | DL(1))
* In-Orchard Localization with a Single LoRa Gateway and Generative Model-based Efficient Fingerprinting, MobiSys 24 [[Paper]](https://dl.acm.org/doi/10.1145/3643832.3661876) (DL)
* Boosting the Long Range Sensing Potential of LoRa, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596847) (NO ML)
* Embracing LoRa Sensing with Device Mobility, SenSys 22 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/SenSys22-LoRaSensingMobility.pdf) (NO ML)
* Combating interference for long range LoRa sensing, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430731) (NO ML)


<a name="teraHertz-sensing"></a>
#### TeraHertz Sensing (Total: 2 | No ML(2) | ML(0) | DL(0))
* Quasi-Optical 3D localization using Asymmetric Signatures above 100 GHz, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3517022) (NO ML)
* LeakyTrack: Non-Coherent Single-Antenna Nodal and Environmental Mobility Tracking with a Leaky-Wave Antenna, SenSys 20 [[Paper]](https://www.brown.edu/research/labs/mittleman/sites/brown.edu.research.labs.mittleman/files/uploads/SenSys_2020.pdf) (NO ML)

<a name="uwb-sensing"></a>
#### UWB Sensing (Total: 12 | No ML(9) | ML(1) | DL(2))
* Mobi2Sense: Empowering Wireless Sensing with Mobility, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560518) (NO ML) (Best Paper Award Runner-ups) 
* Enabling High Accuracy Pervasive Tracking with Ultra Low Power UWB Tags, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560542) (NO ML)
* SiWa: See into Walls via Deep UWB Radars, MobiCom 21 [[Paper]](https://arxiv.org/pdf/2110.14279.pdf) (DL)
* MoRe-Fi: Motion-robust and Fine-grained Respiration Monitoring via Deep-Learning UWB Radar, SenSys 21 [[Paper]](https://arxiv.org/pdf/2111.08195.pdf) (DL) (Also healthcare)
* UWHear: Through-wall Extraction and Separation of Audio Vibrations Using Wireless Signals, SenSys 20 [[Paper]](https://ziqi.plus/papers/UWHear.pdf) (NO ML)
* Chorus: UWB Concurrent Transmissions for GPS-like Passive Localization of Countless Target, IPSN 19 [[Paper]](http://dit.unitn.it/~picco/papers/ipsn19-uwb.pdf) (NO ML)
* SnapLoc: An Ultra-Fast UWB-Based Indoor Localization System for an Unlimited Number of Tag, IPSN 19 [[Paper]](http://www.carloalbertoboano.com/documents/grosswindhager19snaploc.pdf) (NO ML)
* LiquID: A Wireless Liquid IDentifier, MobiSys 18 [[Paper]](https://synrg.csl.illinois.edu/papers/liquid_mobisys2018.pdf) (NO ML)
* SALMA: UWB-based Single-Anchor Localization System using Multipath Assistance, SenSys 18 [[Paper]](http://www.carloalbertoboano.com/documents/grosswindhager18salma.pdf) (NO ML)
* Calibration-Free Network Localization using Non-Line-of-Sight Ultra-Wideband Measurements, IPSN 17 [[Paper]](https://web.eecs.umich.edu/~prabal/pubs/papers/di_franco17nlos.pdf) (ML)
* SurePoint: Exploiting Ultra Wideband Flooding and Diversity to Provide Robust, Scalable, High-Fidelity Indoor Localization, SenSys 16 [[Paper]](https://patpannuto.com/pubs/kempke16surepoint.pdf) (NO ML)
* Harmonium: Asymmetric, Bandstitched UWB for Fast, Accurate, and Robust Indoor Localization, IPSN 16 [[Paper]](https://patpannuto.com/pubs/kempke16harmonium.pdf) (NO ML)

<a name="cellular-sensing"></a>
#### Cellular Sensing (Total: 4 | No ML(3) | ML(0) | DL(1))
* Experience: Large-scale Cellular Localization for Pickup Position Recommendation at Black-hole, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613298) (DL)
* Enabling IoT Self-Localization Using Ambient 5G Signals, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-jog.pdf) (NO ML)
* LTE-Based Low-Cost and Low-Power Soil Moisture Sensing, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568525) (NO ML)
* LTE-based Pervasive Sensing Across Indoor and Outdoor, SenSys	21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485943) (NO ML)


<a name="bluetooth-sensing"></a>
#### Bluetooth Sensing (Total: 5 | No ML(2) | ML(1) | DL(2))
* Experience: Practical Indoor Localization for Malls, MobiCom 22 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/mloc_mobicom22.pdf) (Best Community Contribution) (DL)
* BLE Can See: A Reinforcement Learning Approach for RF-based Indoor Occupancy Detection, IPSN 21 [[Paper]](https://www.cs.virginia.edu/~bjc8c/papers/billah21blecansee.pdf) (DL)
* From Conception to Retirement: a Lifetime Story of a 3-Year-Old Wireless Beacon System in the Wild, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-ding.pdf) (NO ML)
* Nationwide Deployment and Operation of a Virtual Arrival Detection System in the Wild, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472911.pdf) (NO ML)
* Group-In: Group Inference from Wireless Traces of Mobile Devices, IPSN 20 [[Paper]](https://arxiv.org/pdf/2005.12848.pdf) (ML)

<a name="ariel-sensing"></a>
#### Aerial Sensing (Total: 2 | No ML(2) | ML(0) | DL(0))
* BEAVIS: Balloon Enabled Aerial Vehicle for IoT and Sensing, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592498) (NO ML)
* Robust Indoor Localization with ADS-B, MobiCom 21 [[Paper]](https://dl.acm.org/doi/10.1145/3447993.3483257) (NO ML)

<a name="nfc-sensing"></a>
#### NFC Sensing (Total: 1 | No ML(1) | ML(0) | DL(0))
* Locating Everyday Objects using NFC Textiles, IPSN 21 [[Paper]](https://swarunkumar.com/papers/textilesense-ipsn2021.pdf) (NO ML)

<a name="rf-sensing"></a>
#### RF Sensing (Total: 8 | No ML(2) | ML(1) | DL(5))
* Quantum Wireless Sensing: Principle, Design and Implementation, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613258) (NO ML)
* DancingAnt: Body-empowered Wireless Sensing Utilizing Pervasive Radiations from Powerline, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613272) (NO ML)
* XGait: Cross-Modal Translation via Deep Generative Sensing for RF-based Gait Recognition, SenSys 23 [[Paper]](https://perfecthu.github.io/publications/23-sensys-xgait.pdf) (DL)
* Quantifying the Physical Separability of RF-based Multi-Person Respiration Monitoring via SINR, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568513) (DL)
* RISE: robust wireless sensing using probabilistic and statistical assessments, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483253)(DL)
* RF-based 3D skeletons, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230579) (DL)
* RF-Echo: A Non-Line-of-Sight Indoor Localization System Using a Low-Power Active RF Reflector ASIC Tag, MobiCom 17 [[Paper]](https://blaauw.engin.umich.edu/wp-content/uploads/sites/342/2019/12/RF-Echo-A-Non-Line-of-Sight-Indoor-Localization-System-Using-a-Low-Power-Active-RF-Reflector-ASIC-Tag.pdf) (DL）
* Emotion Recognition using Wireless Signals, MobiCom 16 [[Paper]](http://eqradio.csail.mit.edu/files/eqradio-paper.pdf) (ML)

<a name="vision-sensing"></a>
### 👁️ Vision Sensing (Total: 30 | No ML(7) | ML(2) | DL(21))
#### Image Enhancement
* NeuriCam: Key-Frame Video Super-Resolution and Colorization for IoT Cameras, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592523) (DL)
* MicroDeblur: Image Motion Deblurring on Microcontroller-based Vision Systems, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586970) (DL)
* Starfish: resilient image compression for AIoT cameras, SenSys 20 [[Paper]](https://panhu.me/pdf/2020/Starfish.pdf) (DL)
* MobiSR: Efficient On-Device Super-Resolution through Heterogeneous Mobile Processors, MobiCom 19 [[Paper]](https://arxiv.org/pdf/1908.07985.pdf) (DL)
* DoCam: Depth Sensing with an Optical Image Stabilization Supported RGB Camera, MobiCom 22 [[Paper]](https://www.cs.sjtu.edu.cn/~yichao/assets/publications/mobicom22_pan.pdf) (NO ML)

#### Object Detection
* Mozart: A Mobile ToF System for Sensing in the Dark through Phase Manipulation, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596840) (DL)
* Detecting Counterfeit Liquid Food Products in a Sealed Bottle Using a Smartphone Camera, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3539776) (DL)
* LAPD: Hidden Spy Camera Detection using Smartphone Time-of-Flight Sensors, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485941) (DL)
* UltraDepth: Exposing High-Resolution Texture from Depth Cameras, SenSys 21 [[Paper]](http://cvlab.cse.msu.edu/pdfs/Xie_Ouyang_Liu_Xing_UltraDepth_SenSys2021.pdf) (DL)
* EagleEye: wearable camera-based person identification in crowded urban spaces, MobiCom 20 [[Paper]](https://juheonyi.github.io/files/EagleEye.pdf) (DL)
* ODDS: Real-Time Object Detection using Depth Sensors on Embedded GPUs, IPSN 18 [[Paper]](https://www.osti.gov/servlets/purl/1811681) (DL)

#### Human Activity Recognition
* Mosaic: Extremely Low-resolution RFID Vision for Visually-anonymized Action Recognition, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586968) (DL)
* MobiPose: real-time multi-person pose estimation on mobile devices, SensSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430726) (DL)

#### Eye Gaze Recognition
* Gaze Tracking on Any Surface with Your Phone, SenSys 22 [[Paper]](https://www.cs.cityu.edu.hk/~zhenjili/2022-SenSys-ASGaze.pdf) [[code]](https://github.com/Jiani-CAO/ASGaze) (DL)
* GazeGraph: Graph-based Few-Shot Cognitive Context Sensing from Human Visual Behavior, SenSys 20 [[Paper]](https://par.nsf.gov/servlets/purl/10296635) (DL)
* EMO: real-time emotion recognition from single-eye images for resource-constrained eyewear devices, MobiSys 20 [[Paper]](https://dongshuhao.github.io/assets/pdf/2020/Wu_2020.pdf) (DL)

#### Gesture Reconstruction
* RoFin: 3D Hand Pose Reconstructing via 2D Rolling Fingertips, MobiSys 23 [[Paper]](https://tianxing.me/paper/zhang-mobisys23.pdf) (DL)
* MoiréPose: Ultra High Precision Camera-to-Screen Pose Estimation based on Moiré Pattern, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560537) (NO ML)
* Glimpse.3D: A Motion-Triggered Stereo Body Camera for 3D Experience Capture and Preview, IPSN 18 [[Paper]](https://www.ceid.upatras.gr/webpages/courses/adhocnets/files/papers/paper8.pdf) (ML)


* Squint: A Framework for Dynamic Voltage Scaling of Image Sensors Towards Low Power IoT Vision, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613303) (DL)
* MobiSpectral: Hyperspectral Imaging on Mobile Devices, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613296) (DL)
* QfaR: Location-Guided Scanning of Visual Codes from Long Distances, MobiCom 23 [[Paper]](https://wisionlab.com/wp-content/uploads/2023/06/MOBICOM_2023___QfaR.pdf) (DL)
* Testing Masks and Air Filters With Your Smartphones, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625807) (DL)
* Edge-Eye: Rectifying Millimeter-Level Edge Deviation in Manufacturing using Camera-Enabled IoT Edge Device, IPSN 22 [[Paper]](https://taogu.site/pub/paper/IPSN2022.pdf) (DL)
* MobiDepth: Real-Time Depth Estimation Using On-Device Dual Cameras, MobiCom 22 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2022/09/mobicom22-final138.pdf) (NO ML)
* BackCam: Wireless Computer Vision Using Commodity Devices, IPSN 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3302506.3310403) (ML)
* Banner: An Image Sensor Reconfiguration Framework for Seamless Resolution-based Tradeoffs, MobiSys 19	[[Paper]](https://meteor.ame.asu.edu/publications/mobisys19hu-banner.pdf) (NO ML)
* Liquid Testing with Your Smartphone, MobiSys 19 [[Paper]](https://people.csail.mit.edu/scyue/projects/capcam/capcam.pdf) (NO ML)
* HyperSight: boosting distant 3D vision on a single dual-camera smartphone, SenSys 19 [[Paper]](https://dl.acm.org/doi/10.1145/3356250.3360029) (NO ML)
* Glimpse: A Programmable Early-Discard Camera Architecture for Continuous Mobile Vision, MobiSys 17 [[Paper]](https://dl.acm.org/doi/10.1145/3081333.3081347) (Honorable Mention) (NO ML)

<a name="acoustic-sensing"></a>
### 🎵 Acoustic Sensing	(Total: 51 | No ML(24) | ML(10) | DL(17))

#### Localization
* DeepEar: Sound Localization With Binaural Microphones, IEEE Transactions on Mobile Computing 2024 [[Paper]](https://ieeexplore.ieee.org/document/9954178) (DL)
* Owlet: enabling spatial information in ubiquitous acoustic devices,	MobiSys	21	[[Paper]](https://www.cs.umd.edu/~nirupam/images/2_publication/papers/Owlet_MobiSys21_nirupam.pdf) (DL)  
* DeepRange: Acoustic Ranging via Deep Learning, IMWUT 2020 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3432195) (DL)
* MOM: Microphone based 3D Orientation Measurement, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a120/962400a120.pdf) (ML)
* MAVL: Multiresolution Analysis of Voice Localization, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-wang-mei.pdf) (NO ML)
* Voice Localization Using Nearby Wall Reflections, MobiCom 20 [[Paper]](https://synrg.csl.illinois.edu/papers/voloc_mobicom20.pdf) (NO ML)
* Can a Phone Hear the Shape of a Room?, IPSN 19 [[Paper]](https://users.ece.cmu.edu/~agr/resources/publications/ipsn19-shih.pdf) (ML)


#### Movement Tracking
* SVoice: Enabling Voice Communication in Silence via Acoustic Sensing on Commodity Devices, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568530) (DL)
* Experience: practical problems for acoustic sensing,	MobiCom	22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560527)(NO ML)
* FM-Track: Pushing the Limits of Contactless Multi-target Tracking using Acoustic Signals, SenSys 20 [[Paper]](https://people.cs.umass.edu/~dli/papers/SenSys20_FM-Track.pdf) (NO ML)
* RNN-Based Room Scale Hand Motion Tracking, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345439) (DL)
* Your Table Can Be an Input Panel: Acoustic-based Device-Free Interaction Recognition, IMWUT 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3314390) (DL)
* BreathListener: Fine-grained Breathing Monitoring in Driving Environments Utilizing Acoustic Signals, MobiSys 19 [[Paper]](https://www.cs.sjtu.edu.cn/~linghe.kong/2019/XuMOBISYS2019BreathListener.pdf) (DL)
* VSkin: Sensing Touch Gestures on Surfaces of Mobile Devices Using Acoustic Signals, MobiCom 18 [[Paper]](https://cs.nju.edu.cn/lxie/publication/Mobicom2018.pdf) (NO ML)
* Addressing Practical Challenges in Acoustic Sensing To Enable Fast Motion Tracking, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586954) (NO ML)
* CAT: High-Precision Acoustic Motion Tracking, MobiCom 16 [[Paper]](https://dl.acm.org/doi/10.1145/2973750.2973755) (NO ML)
* Strata: Fine-Grained Acoustic-based Device-Free Tracking, MobiSys 17 [[Paper]](https://www.cs.sjtu.edu.cn/~yichao/pmwiki/assets/publications/mobisys17_strata.pdf) (NO ML) (Also VR/AR)


#### Emotion Recognition
* Mic2Mic: Using Cycle-Consistent Generative Adversarial Networks to Overcome Microphone Variability in Speech Systems, IPSN 19 [[Paper]](https://core.ac.uk/download/pdf/219542364.pdf) (DL)
* Low-resource Multi-task Audio Sensing for Mobile and Embedded Devices via Shared Deep Neural Network Representations, UbiComp 17 [[Paper]](https://core.ac.uk/reader/227518690) (DL)
* DeepEar: robust smartphone audio sensing in unconstrained acoustic environments using deep learning, UbiComp 15 [[Paper]](https://core.ac.uk/download/pdf/42340233.pdf) (DL)


#### Keyword Detection
* SoundSieve: Seconds-Long Audio Event Recognition on Intermittently-Powered Systems, MobiSys 23 [[Paper]](https://arxiv.org/pdf/2305.16445.pdf) (DL)
* A closer look at quality-aware runtime assessment of sensing models in multi-device environments, SenSys 19 [[Paper]](https://akhilmathurs.github.io/papers/min_sensys2019.pdf) (DL)

#### Gesture Recognition
* Device-Free Gesture Tracking Using Acoustic Signals, MobiCom 16 [[Paper]](https://cs.nju.edu.cn/ww/papers/mobicom16_ultrasound.pdf) (NO ML)
* Sequence-Based Device-Free Gesture Recognition Framework for Multi-Channel Acoustic Signals, ICASSP 23 [[Paper]](https://ieeexplore.ieee.org/abstract/document/10095790) (DL)
* Room-scale Hand Gesture Recognition Using Smart Speakers, SenSys 22 [[Paper]](https://people.cs.umass.edu/~dli/papers/SenSys2022_SpeakerGesture.pdf) (ML)
* LASense: Pushing the Limits of Fine-grained Activity Sensing Using Acoustic Sign, IMWUT 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3517253) (NO ML)	


#### Source Identification
* Meta-Speaker: Acoustic Source Projection by Exploiting Air Nonlinearity, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613279) (NO ML)
* SCAN: Learning Speaker Identity From Noisy Sensor Data, IPSN 17 [[Paper]](https://www.ceid.upatras.gr/webpages/courses/sensornets/papers/paper8.pdf) (ML)
* Symphony: Localizing Multiple Acoustic Sources with a Single Microphone Array, SenSys 20 [[Paper]](https://arxiv.org/pdf/2209.15325.pdf) (NO ML)
* BodyBeat: A Mobile System for Sensing Non-Speech Body Sounds, MobiSys 14 [[Paper]](https://pac.cs.cornell.edu/pubs/body-beat-mobisys-2014.pdf) (ML)


#### 
* PowerPhone: Unleashing the Acoustic Sensing Capability of Smartphones, MobiCom 23 [[Paper]](https://people.cs.umass.edu/~dli/papers/Mobicom23_PowerPhone.pdf) (DL)
* VeCare: Statistical Acoustic Sensing for Automotive In-Cabin Monitoring, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-zhang-yi.pdf) (NO ML)
* Acoustic Sensing and Communication Using Metasurface, NSDI 23	[[Paper]](https://www.usenix.org/system/files/nsdi23-zhang-yongzhao.pdf) (NO ML)
* Enabling Contact-free Acoustic Sensing under Device Motion,	IMWUT	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3550329)(NO ML)	
* AvA: An Adaptive Audio Filtering Architecture for Enhancing Mobile, Embedded, and Cyber-Physical Systems, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a106/962400a106.pdf) (ML)
* SPiDR: ultra-low-power acoustic spatial sensing for micro-robot navigation,	MobiSys	22	[[Paper]](https://www.cs.umd.edu/~nakul/assets/papers/spidr_mobisys2022_nakul.pdf) (NO ML) (Best Paper)
* SQEE: A Machine Perception Approach to Sensing Quality Evaluation at the Edge by Uncertainty Quantification, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568534) (DL)
* SpeechQoE: A Novel Personalized QoE Assessment Model for Voice Services via Speech Sensing, SenSys 22 [[Paper]](https://ranger.uta.edu/~mingli/publications/SpeechQoE.pdf) (DL)
* MagicInput: Training-free Multi-lingual Finger Input System using Data Augmentation based on MNISTs, ISPN 21 [[Paper]](https://www.cs.sjtu.edu.cn/~yichao/assets/publications/ipsn21_pan.pdf)	(ML)
* Sound-Adapter: Multi-Source Domain Adaptation for Acoustic Classification Through Domain Discovery, IPSN 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3412382.3458265) (DL)
* CSafe: An Intelligent Audio Wearable Platform for Improving Construction Worker Safety in Urban Environments, IPSN 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3412382.3458267) (ML)
* Microphone Array Backscatter: An Application-Driven Design for Lightweight Spatial Sound Recording over the Air, MobiCom 21 [[Paper]](https://www2.cs.sfu.ca/~jcliu/Papers/Microphone21.pdf) (NO ML)
* AcuTe: acoustic thermometer empowered by a single smartphone, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430714#:~:text=AcuTe%20empowers%20a%20single%20smartphone,between%20temperature%20and%20sound%20speed.) (NO ML)
* Rebooting Ultrasonic Positioning Systems for Ultrasound-incapable Smart Devices, MobiCom 19 [[Paper]](https://arxiv.org/pdf/1812.02349.pdf) (NO ML)
* Cross-Platform Support for Rapid Development of Mobile Acoustic Sensing Applications, MobiSys 18 [[Paper]](https://dl.acm.org/doi/10.1145/3210240.3210312) (ML)
* Sonoloc: Scalable positioning of commodity mobile devices, MobiSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3210240.3210324) (NO ML)
* AIM: Acoustic Imaging on a Mobile, MobiSys 18 [[Paper]](https://www.cs.utexas.edu/~meiwang/uploads/8/9/9/1/89919297/aim.pdf) (Best Paper) (NO ML)
* UbiTap: Leveraging Acoustic Dispersion for Ubiquitous Touch Interface on Solid Surfaces, SenSys 18 [[Paper]](http://cps.kaist.ac.kr/papers/18SenSys-UbiTap.pdf) (Best paper runner-up awards) (NO ML)
* SoundSifter: Mitigating Overhearing of Continuous Listening Devices, MobiSys 17 [[Paper]](https://www.cs.unc.edu/~nirjon/paper/soundsifter-mobisys2017.pdf) (ML)
* DopEnc: Acoustic-based Encounter Profiling Using Smartphones, MobiCom 16 [[Paper]](https://wands.sg/team/pengfei/papers/MobiCom16-DopEnc.pdf) (NO ML)
* Expansion of Human–Phone Interface By Sensing Structure-Borne Sound Propagation, MobiSys 16 [[Paper]](https://yctung.github.io/files/publication/mobisys16-forcephone.pdf) (NO ML)
																
<a name="multi-modal-sensing"></a>
### 🖇️ Multi-Modal Sensing (Total: 37 | No ML(3) | ML(9) | DL(25))
#### Human and Object Identification
* Contactless Material Identification with Millimeter Wave Vibrometry, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596850) (DL)
* Capricorn: Towards Real-Time Rich Scene Analysis Using RF-Vision Sensor Fusion, SenSys22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568504) (DL)
* Vi-Fi: Associating Moving Subjects across Vision and Wireless Sensor, IPSN 22 [[Paper]](https://www.winlab.rutgers.edu/~hansiiii/papers/ViFi_Paper___IPSN_2022__Camera_Ready_.pdf) (DL)
* RFID and camera fusion for recognition of human-object interactions, MobiCom	21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483244) (DL)	
* XModal-ID: Using WiFi for Through-Wall Person Identification from Candidate Video Footage, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345437) (DL)


#### Tracking
* Interpersonal Distance Tracking with mmWave Radar and IMUs, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586958) (DL)
* milliEgo: single-chip mmWave radar aided egomotion estimation via deep sensor fusion,	SenSys	20	[[Paper]](https://arxiv.org/pdf/2006.02266.pdf) (DL)
* BatTracker: High Precision Infrastructure-free Mobile Device Tracking in Indoor Environments, SenSys 17 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3131672.3131689) (ML)


#### Localization
* Indoor Smartphone SLAM with Learned Echoic Location Features, SenSys 22 [[Paper]](https://arxiv.org/pdf/2210.08493.pdf) (DL)
* RFusion: Robotic Grasping via RF-Visual Sensing and Learning, SenSys 21 [[Paper]](https://www.mit.edu/~fadel/papers/RFusion-paper.pdf) (DL)
* The Wisdom of 1,170 Teams: Lessons and Experiences from a Large Indoor Localization Competition, MobiCom 23 [[Paper]](https://yshu.org/paper/mobicom23comp.pdf) (DL) (Best Community Contributions Award)
* Indoor localization via multi-modal sensing on smartphones, UbiComp	16	[[Paper]](https://dl.acm.org/doi/abs/10.1145/2971648.2971668) (ML)

#### Speech Enhancement 
* Towards Bone-Conducted Vibration Speech Enhancement on Head-Mounted Wearables, MobiSys 23 [[Paper]](https://yanzhenyu.com/assets/pdf/VibVoice-MobiSys23.pdf) (DL)
* UltraSE: single-channel speech enhancement using ultrasound, MobiCom 21 [[Paper]](http://xyzhang.ucsd.edu/papers/Ke.Sun_MobiCom21_UltraSE.pdf) (DL)	
* Wavoice: A Noise-resistant Multi-modal Speech Recognition System Fusing mmWave and Audio Signals,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485945) (DL)


#### Human Activity Recognition
* CMA: Cross-Modal Association Between Wearable and Structural Vibration Signal Segments for Indoor Occupant Sensing, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586960) (DL)
* VMA: Domain Variance- and Modality-Aware Model Transfer for Fine-Grained Occupant Activity Recognition, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a247/962400a247.pdf) (DL)
* Cosmo: contrastive fusion learning with small data for multimodal human activity recognition,	MobiCom	22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560519) (DL)
* Low-latency speculative inference on distributed multi-modal data streams,MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3467884) (DL)
* Optimal sensor channel selection for resource-efficient deep activity recognition, IPSN 21 [[Paper]](https://acris.aalto.fi/ws/portalfiles/portal/64950790/ELEC_Souza_Leite_Xiao_Optimal_Sensor_Channel_IPSN_2021_acceptedauthormanuscript.pdf) (DL)
* Multimodal deep learning for activity and context recognition, UbiComp 18 [[Paper]](https://homepages.inf.ed.ac.uk/mmarina/papers/ubicomp18.pdf) (DL)
* MESEN: Exploit Multimodal Data to Design Unimodal Human Activity Recognition with Few Labels, SenSys 23 [[Paper]](https://arxiv.org/pdf/2404.01958) (DL)



* Physics-Informed Data Denoising for Real-Life Sensing Systems, Sensys 23 [[Paper]](https://arxiv.org/pdf/2311.06968) (DL)
* SudokuSens: Enhancing Deep Learning Robustness for IoT Sensing Applications using a Generative Approach, SenSys 23 [[Paper]](https://arxiv.org/pdf/2402.02275) (DL)
* MiLTOn: Sensing Product Integrity without Opening the Box using Non-Invasive Acoustic Vibrometry, IPSN 22 [[Paper]](https://swarunkumar.com/papers/milton-ipsn2022.pdf) (ML)
* Motion inspires notion: self-supervised visual-LiDAR fusion for environment depth estimation, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538918) (DL)
* ITrackU: tracking a pen-like instrument via UWB-IMU fusion, MobiSys 21 [[Paper]](https://faculty.cc.gatech.edu/~dhekne/itracku_mobisys2021.pdf) (NO ML)		
* UniTS: Short-Time Fourier Inspired Neural Networks for Sensory Time Series Classification,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485942) (DL)
* SmrtFridge: IoT-based,  user interaction-driven food item & quantity sensing,	SenSys 19 [[Paper]](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=5649&context=sis_research) (DL)
* CrowdEstimator: Approximating Crowd Sizes with Multi-modal Data for Internet-of-Things Services, MobiSys 18 [[Paper]](https://arxiv.org/pdf/1909.13673.pdf) (ML)	
* EAR: Exploiting Uncontrollable Ambient RF Signals in Heterogeneous Networks for Gesture Recognition, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274847)(ML)
* EngageMon: Multi-Modal Engagement Sensing for Mobile Games, UbiComp 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3191745) (ML)
* Bringing IoT to Sports Analytics, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-gowda.pdf) (NO ML)
* BatMapper: Acoustic Sensing Based Indoor Floor Plan Construction Using Smartphones, MobiSys 17 [[Paper]](https://zhoubinwy.github.io/pdf/batmapper.pdf)(NO ML)
* Non-Intrusive Multi-Modal Estimation of Building Occupancy, SenSys 17 [[Paper]](http://www.phpathak.com/files/occupancy-sensys.pdf) (ML)
* Sensor-assisted Face Recognition System on Smart Glass via Multi-view Sparse Representation Classification, IPSN 16 [[Paper]](https://www.cse.unsw.edu.au/~wenh/xu_ipsn_20162.pdf) (ML)
* TransitLabel: A Crowd-Sensing System for Automatic Labeling of Transit Stations Semantics, MobiSys 16 [[Paper]](https://arxiv.org/pdf/1606.03302.pdf) (ML)

<a name="earable-sensing"></a>
### 🦻 Earable Sensing (Total: 20 | No ML(4) | ML(8) | DL(7))
#### Facial Landmark Detection
* FaceListener: Recognizing Human Facial Expressions via Acoustic Sensing on Commodity Headphones, IPSN 22 [[Paper]](https://sites.pitt.edu/~weigao/publications/ipsn22.pdf) [[Dataset]](https://developers.google.com/mediapipe) [[Code]](https://github.com/muxspace/facial_expressions) (DL)
* BioFace-3D: Continuous 3D Facial Reconstruction Through Lightweight Single-ear Biosensors, MobiCom 21 [[Paper]](https://people.cs.umass.edu/~phuc/papers/bioface_2021.pdf) (DL)

#### User Identification
* EarGate: Gait-based User Identification with In-ear Microphones, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483240) (DL)
* MandiPass: Secure and Usable User Authentication via Earphone IMU, IEEE Transactions on Mobile Computing 2021 [[Paper]](https://ieeexplore.ieee.org/document/9546415) (DL)

#### Sound Localization
* DeepEar: Sound Localization With Binaural Microphones, IEEE Transactions on Mobile Computing 2024 [[Paper]](https://ieeexplore.ieee.org/document/9954178) (DL)
* ClearBuds: wireless binaural earbuds for learning-based speech enhancement, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538933) [[Code]](https://clearbuds.cs.washington.edu) (DL)
* Individualizing Head Related Transfer Functions for Binaural Acoustic Applications, IPSN 22 [[Paper]](https://arxiv.org/pdf/2203.11138.pdf) (DL)
* Personalizing Head Related Transfer Functions for Earables, SIGCOMM 21 [[Paper]](https://synrg.csl.illinois.edu/papers/UNIQ_Sigcomm21.pdf) (NO ML)



* WINC: A Wireless IoT Network for Multi-Noise Source Cancellation, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586964) (ML)
* Sensing with Earables: A Systematic Literature Review and Taxonomy of Phenomena, IMWUT 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3550314) (Survey)
* HeadFi: bringing intelligence to all headphones, MobiCom 21	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3448624) (Best Paper Award Runner-up) (ML) 
* OESense: employing occlusion effect for in-ear human sensing, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3467680) (ML)
* Ear-AR: indoor acoustic augmented reality on earphones, MobiCom 20 [[Paper]](https://synrg.csl.illinois.edu/papers/ear-ar_mobicom20.pdf) (ML)
* EarSense: Earphones as a Teeth Activity Sensor, MobiCom 20 [[Paper]](https://synrg.csl.illinois.edu/papers/earsense_mobicom20.pdf) (NO ML)
* WAKE: A Behind-the-ear Wearable System for Microsleep Detection, MobiSys 20 [[Paper]](http://mnslab.org/tamvu/paper/2020%20WAKE_Nhat.pdf) (ML)
* EarphoneTrack: involving earphones into the ecosystem of acoustic motion tracking, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430730) (NO ML)
* ERICA: Enabling Real-time Mistake Detection & Corrective Feedback for Free-Weights Exercises, SenSys 20 [[Paper]](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=6897&context=sis_research) (ML)
* TYTH-Typing On Your Teeth: Tongue-Teeth Localization for Human-Computer Interface, MobiSys 18 [[Paper]](http://mnslab.org/tamvu/paper/2018%20TYTH_Phuc.pdf) (ML)
* MUTE: bringing IoT to noise cancellation, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230550) (NO ML)
* A Lightweight And Inexpensive In-ear Sensing System For Automatic Whole-night Sleep Stage Monitoring, SenSys 16 [[Paper]](http://mnslab.org/tamvu/paper/2016%20Inear%20Lan%20Anh.pdf) (ML)

<a name="light-sensing"></a>
### 💡 Visible Light Sensing (Total: 15 | No ML(7) | ML(7) | DL(1))
* LiT: Fine-grained Toothbrushing Monitoring with Commercial LED Toothbrush, MobiCom 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3570361.3613287) (ML)
* SMART: Screen-based Gesture Recognition on Commodity Mobile Devices, MobiCom 21 [[Paper]](https://huangqy7.github.io/Paper/mobicom21-SMART.pdf) (DL)
* Lili: Liquor Quality Monitoring Based on Light Signals, MobiCom 21 [[Paper]](https://luwang-szu.github.io/paper/LiliMobiCom.pdf) (ML)
* CurveLight:An Accurateand Practical Light Positioning System, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485934) (ML)
* LiTag: Localization and Posture Estimation with Passive Visible Light Tags, SenSys 20 [[Paper]](https://www.cse.msu.edu/~lilingk1/publications/sensys20-LiTag.pdf) (NO ML)
* SolarGest: Ubiquitous and Battery-free Gesture Recognition using Solar Cells, MobiCom 19 [[Paper]](https://arxiv.org/pdf/1812.01766.pdf) (ML)
* RainbowLight: Towards Low Cost Ambient Light Positioning with Mobile Phones, MobiCom 18 [[Paper]](http://tns.thss.tsinghua.edu.cn/~jiliang/publications/MOBICOM2018-rainbowlight.pdf) (NO ML)
* Battery-Free Eye Tracker on Glasses, MobiCom 18 [[Paper]](https://digitalcommons.dartmouth.edu/cgi/viewcontent.cgi?article=3975&context=facoa) (ML)
* Augmenting Indoor Inertial Tracking with Polarized Light, MobiSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3210240.3210340) (NO ML)
* Pulsar: Towards Ubiquitous Visible Light Localization, MobiCom 17 [[Paper]](https://dl.acm.org/doi/10.1145/3117811.3117821) (NO ML)
* CELLI: Indoor Positioning Using Polarized Sweeping Light Beams, MobiSys 17 [[Paper]](https://dl.acm.org/doi/10.1145/3081333.3081352) (ML)
* Enabling High-Precision Visible Light Localization in Today’s Buildings. MobiSys 17 [[Paper]](https://cseweb.ucsd.edu//~shz338/images/MobiSys_17.pdf) (ML)
* SmartLight: Light-weight 3D Indoor Localization Using a Single LED Lamp, SenSys 17 [[Paper]](https://www-users.cse.umn.edu/~tianhe/Papers/SmartLight.pdf) (NO ML) (Best Paper)
* LiTell: Robust Indoor Localization Using Unmodified Light Fixtures, MobiCom 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2973750.2973767) (NO ML)
* Practical Human Sensing in the Light, MobiSys 16 [[Paper]](https://www.cs.columbia.edu/~xia/publication/mobisys16-starlight/mobisys16-starlight.pdf) (NO ML)

<a name="magnetic-sensing"></a>
### 🧲 Magentic Sensing (Total: 6 | No ML(1) | ML(3) | DL(2))
* METRO: Magnetic Road Markings for All-weather, Smart Roads, SenSys 23 [[Paper]](https://theisclab.com/docs/2023_Sensys_METRO_Wang.pdf) (NO ML)
* Automatic Calibration of Magnetic Tracking, MobiCom 22 [[Paper]](https://rtcl.eecs.umich.edu/rtclweb/assets/publications/2022/mobicom22-wang.pdf) (ML)
* MagX: Wearable, Untethered Hands Tracking with Passive Magnets, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483260) (ML)
* MET: a magneto-inductive sensing based electric toothbrushing monitoring system, MobiCom 20 [[Paper]](https://www.ece.sunysb.edu/~slin/Publications/MOBICOM2020.pdf) (DL)
* MagHacker: Eavesdropping on Stylus Pen Writing via Magnetic Sensing from Commodity Mobile Devices, MobiSys 20 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobisys20.pdf) (DL)
* MagTrack: Enabling Safe Driving Monitoring with Wearable Magnetics, MobiSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3307334.3326107) (ML)

<a name="cross-medium-sensing"></a>
### 🔀 Cross-Medium Sensing (Total: 2 | No ML(2) | ML(0) | DL(0))
* Underwater 3D positioning on smart devices, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3603269.3604851) (NO ML)
* Sunflower: Locating Underwater Robots From the Air,	MobiSys	22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3539773) (NO ML)

<a name="generative-ai-for-sensing"></a>
### 📜 Generative AI for Sensing (Total: 3 | No ML(0) | ML(0) | DL(3))
* LLMSense: Harnessing LLMs for High-level Reasoning Over Spatiotemporal Sensor Traces, arxiv 24 [[Paper]](https://arxiv.org/pdf/2403.19857) (DL)
* LLaSA: Large Multimodal Agent for Human Activity Analysis Through Wearable Sensors, arxiv 24 [[Paper]](https://arxiv.org/pdf/2406.14498) (DL)
* Penetrative AI: Making LLMs Comprehend the Physical World, HOTMOBILE 24 [[Paper]](https://arxiv.org/pdf/2310.09605) (DL)
     
## 🧮 Computing							
<a name="computing"></a>	
### 📲 On-Device Inference						
<a name="on-device-inference"></a>

#### ⚡ Inference Optimization
<a name="inference-optimization"></a>
##### Computation Optimization
* Boosting DNN Cold Inference on Devices, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596842)
* ConvReLU++: Reference-based Lossless Acceleration of Conv-ReLU Operations on Mobile CPU, MobiSys 23 [[Paper]](https://yuanchun-li.github.io/static/files/MobiSys23_ConvReLU++.pdf) [[Code]](https://github.com/GAIR-team/conv_relu_plus_plus)
* NeuLens: spatial-based dynamic acceleration of convolutional neural networks on edge, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560528)
* BiSon-e: a lightweight and high-performance accelerator for narrow integer linear algebra computing on the edge, ASPLOS 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507746)
* InFi: end-to-end learnable input filter for resource-efficient mobile-centric inference, MobiCom 22 [[Paper]](https://yuanmu97.github.io/preprint/InFi_MobiCom22.pdf)	
* IOS: Inter-Operator Scheduler for CNN Acceleration, MLSys 21 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2021/hash/38b3eff8baf56627478ec76a704e9b52-Abstract.html)	
* Flexible High-resolution Object Detection on Edge Devices with Tunable Latency, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483274)
* Intelligence Beyond the Edge: Inference on Intermittent Embedded Systems, ASPLOS 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3297858.3304011)			
* DeepCache: Principled Cache for Mobile Deep Vision, MobiCom 18 [[Paper]](https://arxiv.org/pdf/1712.01670.pdf) [[Code]](https://github.com/xumengwei/DeepCache) (DL)
* FastDeepIoT: Towards Understanding and Optimizing Neural Network Execution Time on Mobile and Embedded Devices, SenSys 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3274783.3274840)
* DeepMon: Mobile GPU-based Deep Learning Framework for Continuous Vision Applications, MobiSys 17 [[Paper]](https://www.cse.iitd.ac.in/~rijurekha/course/deepmon.pdf) 
* SC-DCNN: Highly-Scalable Deep Convolutional Neural Network using Stochastic Computing, ASPLOS 17 [[Paper]](http://alchem.usc.edu/portal/static/download/sc_dcnn.pdf) 


##### Memory Optimization
+ LUT-NN: Empower Efficient Neural Network Inference with Centroid Learning and Table Lookup, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613285)
* Flexagon: A Multi-Dataflow Sparse-Sparse Matrix Multiplication Accelerator for Efficient DNN Processing, ASPLOS 23 [[Paper]](https://arxiv.org/pdf/2301.10852.pdf)
* Space-Efficient TREC for Enabling Deep Learning on Microcontrollers, ASPLOS 23 [[Paper]](https://research.csc.ncsu.edu/picture/publications/papers/asplos23a_mcu.pdf)
* mGEMM: Low-latency Convolution with Minimal Memory Overhead Optimized for Mobile Devices, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538940)
* SparTA: Deep-Learning Model Sparsity via Tensor-with-Sparsity-Attribute, OSDI	22 [[Paper]](https://www.usenix.org/system/files/osdi22-zheng-ningxin.pdf)			
* MCUNetV2: Memory-Efficient Patch-based Inference for Tiny Deep Learning, NeurIPS 21
* DeQA: On-Device Question Answering, MobiSys 19 [[Paper]](https://www3.cs.stonybrook.edu/~arunab/papers/deqa.pdf)

#### Multi-Tenant Inference
##### Resource Utilization
* YONO: Modeling Multiple Heterogeneous Neural Networks on Microcontrollers, IPSN 22 [[Paper]](https://arxiv.org/pdf/2203.03794.pdf)
* LegoDNN: block-grained scaling of deep neural networks for mobile vision, MobiCom 21 [[Paper]](https://arxiv.org/pdf/2112.09852.pdf) (Best Community Paper Award Runner-Up)	
* Fast and scalable in-memory deep multitask learning via neural weight virtualization,	MobiSys	20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388947)		
* Potluck: Cross-Application Approximate Deduplication for Computation-Intensive Mobile Applications, ASPLOS 18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3173162.3173185) (DL)
* Mainstream: Dynamic Stem-Sharing for Multi-Tenant Video Processing, ATC 18 [[Paper]](https://www.usenix.org/system/files/conference/atc18/atc18-jiang.pdf)			
* NestDNN: Resource-Aware Multi-Tenant On-Device Deep Learning for Continuous Mobile Vision, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241559)	

##### Execution Strategy
+ Miriam: Exploiting Elastic Kernels for Real-time Multi-DNN Inference on Edge GPU, SenSys 23 [[Paper]](https://arxiv.org/pdf/2307.04339)
* POS: An Operator Scheduling Framework for Multi-model Inference on Edge Intelligent Computing, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586953)
* Microsecond-scale Preemption for Concurrent GPU-accelerated DNN Inferences, OSDI 22 [[Paper]](https://www.usenix.org/conference/osdi22/presentation/han)			
* VELTAIR: towards high-performance multi-tenant deep learning services via adaptive compilation and scheduling, ASPLOS	22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507752)
* * RT-mDL: Supporting Real-Time Mixed Deep Learning Tasks on Edge Platforms, SenSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485938)		
* NeuOS: A Latency-Predictable Multi-Dimensional Optimization Framework for DNN-driven Autonomous Systems, ATC 20 [[Paper]](https://www.usenix.org/system/files/atc20-bateni.pdf)
* DeepEye: Resource Efficient Local Execution of Multiple Deep Vision Models using Wearable Commodity Hardware, MobiSys 17 [[Paper]](https://akhilmathurs.github.io/papers/mathur_mobisys2017.pdf)
* MCDNN: An Approximation-Based Execution Framework for Deep Stream Processing Under Resource Constraints, MobiSys 17 [[Paper]](https://homes.cs.washington.edu/~arvind/papers/mcdnn.pdf)

#### 🔀 Cross-Processor Inference (Total: 11)
<a name="cross-processor-inference"></a>
##### Model Partitioning
* NN-Stretch: Automatic Neural Network Branching for Parallel Inference on Heterogeneous Multi-Processors, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596870)
* BlastNet: Exploiting Duo-Blocks for Cross-Processor Real-Time DNN Inference, SenSys 22 [[Paper]](https://yanzhenyu.com/assets/pdf/BlastNet-SenSys22.pdf)
* CoDL: Efficient CPU-GPU Co-execution for Deep Learning Inference on Mobile Devices, MobiSys 22 [[Paper]](https://chrisplus.me/assets/pdf/mobisys22-CoDL.pdf)
* AsyMo: Scalable and Efficient Deep-Learning Inference on Asymmetric Mobile CPUs, MobiCom 21 [[Paper]](https://www.msra.cn/wp-content/uploads/2021/03/mobicom21-asymo.pdf)
* Efficient Execution of Deep Neural Networks on Mobile Devices with NPU, IPSN 21 [[Paper]](http://mcn.cse.psu.edu/paper/tan-tianxiang/ipsn20-tan.pdf)		
* DeepX: A Software Accelerator for Low-Power Deep Learning Inference on Mobile Devices, IPSN 16 [[Paper]](https://www.fahim-kawsar.net/papers/Lane.IPSN2016-Camera.pdf)


* Neuro.ZERO: a zero-energy neural network accelerator for embedded sensing and inference systems, SenSys 19 [[Paper]](https://eisys.web.unc.edu/wp-content/uploads/sites/20971/2019/10/sensys19-final95.pdf)
* μLayer: Low Latency On-Device Inference Using Cooperative Single-Layer Acceleration and Processor-Friendly Quantization, EuroSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3302424.3303950)	
* Accelerating Mobile Audio Sensing Algorithms through On-Chip GPU Offloading, MobiSys 17 [[Paper]](https://www.cl.cam.ac.uk/~cm542/papers/mobisys17.pdf)

##### Task Scheduling
* PointSplit: Towards On-device 3D Object Detection with Heterogeneous Low-power Accelerators, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3587045)
* Band: Coordinated Multi-DNN Inference on Heterogeneous Mobile Processors, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538948)
* Mandheling: mixed-precision on-device DNN training with DSP offloading,MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560545)			


#### ⏳ Runtime Adaptation
<a name="runtime-adaptation"></a>
* Memory-Efficient Domain Incremental Learning for Internet of Things,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568436)	
* LiteReconfig: Cost and Content Aware Reconfiguration of Video Object Detection Systems for Mobile GPUs, EuroSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3492321.3519577)
* Mistify: Automating DNN Model Porting for On-Device Inference at the Edge, NSDI 21	[[Paper]](https://www.usenix.org/system/files/nsdi21-guo.pdf)	
* Palleon: A Runtime System for Efficient Video Processing toward Dynamic Class Skew, ATC 21 [[Paper]](https://www.usenix.org/system/files/atc21-feng-boyuan.pdf)
* ApproxDet: Content and Contention-Aware Approximate Object Detection for Mobiles, SenSys 20 [[Paper]](https://arxiv.org/pdf/2010.10754.pdf)
* FlexDNN: Input-Adaptive On-Device Deep Learning for Efficient Mobile Vision, SEC 20 [[Paper]](https://www.egr.msu.edu/~mizhang/papers/2020_SEC_FlexDNN.pdf)
* MetaSense: few-shot adaptation to untrained conditions in deep mobile sensing, SenSys	19 [[Paper]](https://taesikgong.com/paper/SenSys19_MetaSense.pdf)

+ AdaptiveNet: Post-deployment Neural Architecture Adaptation for Diverse Edge Environments, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592529)
+ On-NAS: On-Device Neural Architecture Search on Memory-Constrained Intelligent Embedded Systems, SenSys 23 [[Paper]](https://dl.acm.org/doi/10.1145/3625687.3625814)
+ Adaptive Intelligence for Batteryless Sensors Using Software-Accelerated Tsetlin Machines, SenSys 22 [[Paper]](https://alessandro-montanari.github.io/papers/sensys2022.pdf)
		
#### Model Compression
* On-Demand Deep Model Compression for Mobile Devices: A Usage-Driven Model Selection Framework, MobiSys 18 [[Paper]](https://tik-old.ee.ethz.ch/file//79a7dd6f6370f809e6180c0746232283/mobisys18-liu.pdf)
* DeepIoT: Compressing Deep Neural Network Structures for Sensing Systems with a Compressor-Critic Framework, SenSys 17 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3131672.3131675)
* Sparsification and Separation of Deep Learning Layers for Constrained Resource Inference on Wearables, SenSys 16 [[Paper]](https://discovery.ucl.ac.uk/id/eprint/1535346/1/main%20(3).pdf)
	
#### 🔐 Privacy-Preserving Inference
* Characterizing and Optimizing End-to-End Systems for Private Inference, ASPLOS 23 [[Paper]](https://arxiv.org/pdf/2207.07177.pdf)
* SOTER: Guarding Black-box Inference for General Neural Networks at the Edge, ATC 22 [[Paper]](https://www.usenix.org/system/files/atc22-shen.pdf)	
* Shredder: Learning Noise Distributions to Protect Inference Privacy, ASPLOS 20 [[Paper]](https://arxiv.org/pdf/1905.11814.pdf)
  
#### 📊 Benchmarks (Total: 2)
+ nnPerf: Demystifying DNN Runtime Inference Latency on Mobile Platforms, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625797)
* MLPerf Mobile Inference Benchmark, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/7eabe3a1649ffa2b3ff8c02ebfd5659f-Paper.pdf)
* URSABench: A System for Comprehensive Benchmarking of Bayesian Deep Neural Network Models and Inference methods, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/hash/3ef815416f775098fe977004015c6193-Abstract.html)	

### Offloading	
#### Model Partitioning
* Real-time Neural Network Inference on Extremely Weak Devices: Agile Offloading with Explainable AI, MobiCom 22 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobicom22.pdf)	
* CLIO: enabling automatic compilation of deep learning pipelines across IoT and cloud,	MobiCom	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3372224.3419215)	
* Neurosurgeon: Collaborative Intelligence Between the Cloud and Mobile Edge, ASPLOS 17 [[Paper]](https://dl.acm.org/doi/10.1145/3037697.3037698)
  
#### Workload Partitioning
* CoEdge: A Cooperative Edge System for Distributed Real-Time Deep Learning Tasks, IPSN 23 [[Paper]](https://neawhen.github.io/neiwen.github.io/assets/pdf/coedge_ipsn23.pdf)
* Elf: accelerate high-resolution mobile deep vision with content-aware parallel offloading, MobiCom 21 [[Paper]](https://www.msra.cn/wp-content/uploads/2021/03/mobicom21-elf.pdf)	
* Edge-SLAM: Edge-Assisted Visual Simultaneous Localization and Mapping, MobiSys 20 [[Paper]](https://par.nsf.gov/servlets/purl/10167133) (NO ML) (Also AR)
* LEO: Scheduling Sensor Inference Algorithms across Heterogeneous Mobile Processors and Network Resources, MobiCom 16 [[Paper]](https://core.ac.uk/download/pdf/83939419.pdf)

#### Communication Optimization
* Hyperion: A Generic and Distributed Mobile Offloading Framework on OpenCL, SenSys 22 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2022/11/sensys22-hyperion.pdf) (NO ML)
* SwarmMap: Scaling Up Real-time Collaborative Visual SLAM at the Edge, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-xu_jingao.pdf) (NO ML)
* Context-Aware Compilation of DNN Training Pipelines across Edge and Cloud, UbiComp 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3494981) [[code]](https://github.com/dixiyao/Context-Aware-Compilation-of-DNN-Training-Pipelines-across-Edge-and-Cloud)
* SPINN: synergistic progressive inference of neural networks over device and cloud, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419194)	
* Deep compressive offloading: speeding up neural network inference by trading edge computation for network latency,	SenSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430898)	
* Source Compression with Bounded DNN Perception Loss for IoT Edge Computer Vision,	MobiCom	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345448)		
* FoggyCache: Cross-Device Approximate Computation Reuse, MobiCom 18 [[Paper]](https://www.cs.yale.edu/homes/guo-peizhen/files/foggycache-mobicom18.pdf)


#### Privacy-Preserving Offloading 
* PriMask: Cascadable and Collusion-Resilient Data Masking for Mobile Cloud Inference, SenSys 22 [[Paper]](https://arxiv.org/pdf/2211.06716.pdf)	

+ EdgeFM: Leveraging Foundation Model for Open-set Learning on the Edge, SenSys 23 [[Paper]](https://arxiv.org/pdf/2311.10986) 
+ Accuracy-Centric Multitask Offloading in Edge-Assisted Mobile Augmented Reality, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592531)
+ Re-thinking computation offload for efficient inference on IoT devices with duty-cycled radios, MobiCom 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3570361.3592514)
+ Walle: An End-to-End, General-Purpose, and Large-Scale Production System for Device-Cloud Collaborative Machine Learning, OSDI 22 [[Paper]](https://www.usenix.org/system/files/osdi22-lv.pdf)
	

### 🎯 On-Device Training
<a name="on-device-training"></a>
#### Training on a Single Device
+ Cost-effective On-device Continual Learning over Memory Hierarchy with Miro, MobiCom 23 [[Paper]](https://arxiv.org/pdf/2308.06053.pdf)
+ LifeLearner: Hardware-Aware Meta Continual Learning System for Embedded Computing Platforms, SenSys 23 [[Paper]](https://arxiv.org/pdf/2311.11420)
* ElasticTrainer: Speeding Up On-Device Training with Runtime Elastic Tensor Selection, MobiSys 23 [[Paper]](https://hellokevin07.github.io/files/mobisys23-ElasticTrainer.pdf) [[Code]](https://github.com/HelloKevin07/ElasticTrainer)
* On-Device Training Under 256KB Memory, NeurIPS 22 [[Paper]](https://arxiv.org/abs/2206.15472)
* Campo: Cost-Aware Performance Optimization for Mixed-Precision Neural Network Training, ATC 22 [[Paper]](https://www.usenix.org/system/files/atc22-he.pdf)
* Memory-efficient DNN Training on Mobile Device, MobiSys 22	[[Paper]](https://dl.acm.org/doi/10.1145/3498361.3539765)	
* Melon: breaking the memory wall for resource-efficient on-device machine learning, MobiSys 22 [[Paper]](https://xumengwei.github.io/files/MobiSys22-Melo.pdf)
* Octo: INT8 Training with Loss-aware Compensation and Backward Quantization for Tiny On-device Learning,	ATC	21	[[Paper]](https://www.usenix.org/conference/atc21/presentation/zhou-qihua)
* MDLdroidLite: a release-and-inhibit control approach to resource-efficient deep neural networks on mobile devices,	SenSys	20	[[Paper]](https://taogu.site/pub/paper/Paper_3_SenSys_2020.pdf)	
* Full deep neural network training on a pruned weight budget,	MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/135.pdf)		
* Split-CNN: Splitting Window-based Operations in Convolutional Neural Networks for Memory System Optimization, ASPLOS 19 [[Paper]](https://dl.acm.org/doi/10.1145/3297858.3304038)	

#### Training on Distributed Devices
* Mercury: Efficient On-Device Distributed DNN Training via Stochastic Importance Sampling, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485930)
* MDLdroid: a ChainSGD-reduce Approach to Mobile Deep Learning for Personal Mobile Sensing, IPSN 20 [[Paper]](https://arxiv.org/pdf/2002.02897.pdf)

#### Federated Learning
##### Data Heterogeneity
* GPT-FL: Generative Pre-trained Model-Assisted Federated Learning." ArXiv 23 [[Paper]](https://arxiv.org/abs/2306.02210)
* BalanceFL: Addressing Class Imbalance in Long-tail Federated Learning, IPSN 22 [[Paper]](https://yanzhenyu.com/assets/pdf/BalanceFL-IPSN22.pdf) [[code]](https://github.com/sxontheway/BalanceFL)
*  FedBalancer: Data and Pace Control for Efficient Federated Learning on Heterogeneous Clients,	MobiSys	22	[[Paper]](https://arxiv.org/pdf/2201.01601.pdf)
* FedDL:  Federated Learning via Dynamic Layer Sharing for Human Activity Recognition, SenSys '21 [[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485946)

#####  Communication Optimization
* Faster Non-Convex Federated Learning via Global and Local Momentum, UAI 22 [[Paper](https://openreview.net/forum?id=SSlLRUIs9e9)
* DeepReduce: A Sparse-tensor Communication Framework for Federated Deep Learning, NeurIPS 21 [[Paper]](https://proceedings.neurips.cc/paper/2021/hash/b0ab42fcb7133122b38521d13da7120b-Abstract.html)
* FedMask:  Joint Computation and Communication-Efficient Personalized Federated Learning via Heterogeneous Masking, SenSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485929)
* Adaptive Quantization of Model Updates for Communication-Efficient Federated Learning, ICASSP 21 [[Paper]](https://ieeexplore.ieee.org/document/9413697)
* Ensemble distillation for robust model fusion in federated learning, NeurIPS 20 [[Paper]](https://dl.acm.org/doi/abs/10.5555/3495724.3495922)
* FedPAQ: A Communication-Efficient Federated Learning Method with Periodic Averaging and Quantization, AISTATS 20 [[Paper]](http://proceedings.mlr.press/v108/reisizadeh20a/reisizadeh20a.pdf)
* A Distributed Synchronous SGD Algorithm with Global Top-k Sparsification for Low Bandwidth Networks, ICDCS 19 [[Paper]](https://www.computer.org/csdl/proceedings-article/icdcs/2019/251900c238/1ezRT3vzfcA)
* FedMD: Heterogenous Federated Learning via Model Distillation, Arxiv 2019 [[Paper]](https://arxiv.org/abs/1910.03581)

##### System Heterogeneity
* TimelyFL: Heterogeneity-aware Asynchronous Federated Learning with Adaptive Partial Training, CVPR 23 [[Paper]](https://ieeexplore.ieee.org/document/10208323)
* EEFL: High-Speed Wireless Communications Inspired Energy Efficient Federated Learning over Mobile Devices, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596865)
* AsyncFL: Asynchronous Federated Learning Using Majority Voting with Quantized Model Updates, AAAI 22 [[Paper]](https://ojs.aaai.org/index.php/AAAI/article/view/21624)
* Federated Learning with Buffered Asynchronous Aggregation, AISTATS 22 [[Paper]](https://proceedings.mlr.press/v151/nguyen22b)
* FedSEA: A Semi-Asynchronous Federated Learning Framework for Extremely Heterogeneous Devices, SenSys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3560905.3568538)
* FedSA: A Semi-Asynchronous Federated Learning Mechanism in Heterogeneous Edge Computing, in IEEE Journal on Selected Areas in Communications 2021 [[Paper]](https://ieeexplore.ieee.org/document/9562538)
* SAFA: A Semi-Asynchronous Protocol for Fast Federated Learning With Low Overhead, in IEEE Transactions on Computers 2021 [[Paper]](https://ieeexplore.ieee.org/document/9093123)
* Time Efficient Federated Learning with Semi-asynchronous Communication, ICPADS 20 [[Paper]](http://dx.doi.org/10.1109/ICPADS51040.2020.00030)
* 	Local SGD with Periodic Averaging: Tighter Analysis and Adaptive Synchronization, NeurIPS 19 [[Paper]](https://proceedings.neurips.cc/paper/2019/file/c17028c9b6e0c5deaad29665d582284a-Paper.pdf)

##### Personalization
* TailorFL: Dual-Personalized Federated Learning under System and Data Heterogeneity, SenSys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3560905.3568503)
* Distributed learning of fully connected neural networks using independent subnet training, VLDB 22 [[Paper]](https://dl.acm.org/doi/10.14778/3529337.3529343)
* Personalized Federated Learning by Structured and Unstructured Pruning under Data Heterogeneity, ICDCSW 21 [[Paper]](https://ieeexplore.ieee.org/document/9545941)
* FedDL: Federated Learning via Dynamic Layer Sharing for Human Activity Recognition, SenSys 21	[[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485946)	

##### Client Selection
* REFL: Resource-Efficient Federated Learning, EuroSys 23 [[Paper]](https://arxiv.org/pdf/2111.01108.pdf)
* PyramidFL: a fine-grained client selection framework for efficient federated learning, MobiCom 22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517017)
* Oort: Efficient Federated Learning via Guided Participant Selection, OSDI 21	[[Paper]](https://www.usenix.org/system/files/osdi21-lai.pdf)		
* ClusterFL: a similarity-aware federated learning system for human activity recognition, MobiSys 21	[[Paper]](https://aiot.ie.cuhk.edu.hk/papers/ClusterFL.pdf)
* Efficient Training Management for Mobile Crowd-Machine Learning: A Deep Reinforcement Learning Approach in IEEE Wireless Communications Letters 2019 [[Paper]](https://ieeexplore.ieee.org/abstract/document/8716527)

##### Model Heterogeneity
* Distillation-Based Semi-Supervised Federated Learning for Communication-Efficient Collaborative Training With Non-IID Private Data in IEEE Transactions on Mobile Computing, 2023 [[Paper]](https://ieeexplore.ieee.org/document/9392310)
* FedRolex: Model-Heterogeneous Federated Learning with Rolling Sub-Model Extraction, NeurIPS 22 [[Paper]](https://openreview.net/forum?id=OtxyysUdBE)
* Heterogeneous Ensemble Knowledge Transfer for Training Large Models in Federated Learning, IJCAI 22 [[Paper]](https://www.ijcai.org/proceedings/2022/0399)
* FjORD: Fair and Accurate Federated Learning under heterogeneous targets with Ordered Dropout, NeurIPS 21 [[Paper]](https://proceedings.neurips.cc/paper/2021/file/6aed000af86a084f9cb0264161e29dd3-Paper.pdf)
* HeteroFL: Computation and Communication Efficient Federated Learning for Heterogeneous Clients, ICLR 21 [[Paper]](https://openreview.net/forum?id=TNkPBBYFkXg)
			
##### Frameworks and Benchmarks
* FedAIoT: A Federated Learning Benchmark for Artificial Intelligence of Things, Arxiv 23 [[Paper]](https://arxiv.org/abs/2310.00109)
* FedMultimodal: A Benchmark for Multimodal Federated Learning, KDD 23
* FedAudio: A Federated Learning Benchmark for Audio Tasks, ICASSP 23 [[Paper]](https://arxiv.org/pdf/2210.15707.pdf)
* FedNLP: Benchmarking Federated Learning Methods for Natural Language Processing Tasks, NACCL 22 [[Paper]](https://arxiv.org/pdf/2104.08815.pdf) [[code]](https://github.com/FedML-AI/FedML/tree/master/python/app/fednlp) 
* Flower: A Friendly Federated Learning Research Framework, Arxiv 22 [[Paper]](https://arxiv.org/abs/2007.14390)
* FedScale: Benchmarking Model and System Performance of Federated Learning at Scale, ICML 22 [[Paper]](https://openreview.net/forum?id=LZ5cx2yismf)
* FedCV: A Federated Learning Framework for Diverse Computer Vision Tasks, Arxiv 21 [[Paper]](https://arxiv.org/pdf/2111.11066.pdf) [[code]](https://github.com/FedML-AI/FedML/tree/master/python/app/fedcv)
* FedML: A Research Library and Benchmark for Federated Machine Learning, Arxiv 20 [[Paper]](https://arxiv.org/abs/2007.13518)



									
### Model Deployment on the Edge
* ML-EXray: Visibility into ML Deployment on the Edge, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/76dc611d6ebaafc66cc0879c71b5db5c-Paper.pdf)
* GPUReplay: a 50-KB GPU stack for client ML, ASPLOS 22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507754)	
																				
### Automated Machine Learning for AIoT
* HarvNet: Resource-Optimized Operation of Multi-Exit Deep Neural Networks on Energy Harvesting Devices, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596845)
* Hyperscale Hardware Optimized Neural Architecture Search, ASPLOS 23 [[Paper]](https://dl.acm.org/doi/10.1145/3582016.3582049)
* Towards the Co-design of Neural Networks and Accelerators, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/31fefc0e570cb3860f2a6d4b38c6490d-Paper.pdf)			
* MicroNets: Neural Network Architectures for Deploying TinyML Applications on Commodity Microcontrollers, MLSys 21	[[Paper]](https://proceedings.mlsys.org/paper_files/paper/2021/hash/a3c65c2974270fd093ee8a9bf8ae7d0b-Abstract.html)	
* nn-Meter: towards accurate latency prediction of deep-learning model inference on diverse edge devices, MobiSys 21 [[Paper]](https://air.tsinghua.edu.cn/pdf/nn-Meter-Towards-Accurate-Latency-Prediction-of-Deep-Learning-Model-Inference-on-Diverse-Edge-Devices.pdf) (Best Paper)		
* Neural Architecture Search as Program Transformation Exploration, ASPLOS 21 [[Paper]](https://arxiv.org/pdf/2102.06599.pdf)
* Mind Mappings: Enabling Efficient Algorithm-Accelerator Mapping Space Search, ASPLOS 21 [[Paper]](https://arxiv.org/pdf/2103.01489.pdf)
* Searching for Winograd-aware Quantized Networks, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/45c48cce2e2d7fbdea1afc51c7c6ad26-Paper.pdf)
* SkyNet: a Hardware-Efficient Method for Object Detection and Tracking on Embedded Systems, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/93db85ed909c13838ff95ccfa94cebd9-Paper.pdf)
* MCUNet: Tiny Deep Learning on IoT Devices,	NeurIPS	20	[[Paper]](https://proceedings.neurips.cc/paper/2020/hash/86c51678350f656dcc7f490a43946ee5-Abstract.html)	
* Does Unsupervised Architecture Representation Learning Help Neural Architecture Search?, NeurIPS 20 [[Paper]](https://proceedings.neurips.cc/paper/2020/hash/937936029af671cf479fa893db91cbdd-Abstract.html)	
														
### Compiler for AIoT	
<a name="compilers-for-aiot"></a>
* Heron: Automatically Constrained High-Performance Library Generation for Deep Learning Accelerators, ASPLOS 23 [[Paper]](https://dl.acm.org/doi/10.1145/3582016.3582061)
* Bringing WebAssembly to Resource-constrained IoT Devices for Seamless Device-Cloud Integration, MobiSys 22 [[paper]](https://liborui.github.io/publication/2022-mobisys22-wait/2022-mobisys22-wait.pdf) (NO ML)
* Romou: rapidly generate high-performance tensor kernels for mobile GPUs,	MobiCom	22	[[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2022/02/mobigpu_mobicom22_camera.pdf)	
* The CoRa Tensor Compiler: Compilation for Ragged Tensors with Minimal Padding, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/d3d9446802a44259755d38e6d163e820-Paper.pdf)
* ROLLER: Fast and Efficient Tensor Compilation for Deep Learning,	OSDI	22	[[Paper]](https://www.usenix.org/conference/osdi22/presentation/zhu)			
* AStitch: Enabling a New Multi-dimensional Optimization Space for Memory-Intensive ML Training and Inference on Modern SIMT Architectures, ASPLOS 22 [[Paper]](https://pacman.cs.tsinghua.edu.cn/~zjd/publication/asplos-22-zhenzheng/asplos-22-zhenzheng.pdf)
* TensorFlow Lite Micro: Embedded Machine Learning for TinyML Systems,	MLSys	21	[[Paper]](https://proceedings.mlsys.org/paper_files/paper/2021/hash/d2ddea18f00665ce8623e36bd4e3c7c5-Abstract.html)
* Analytical Characterization and Design Space Exploration for Optimization of CNNs, ASPLOS 21 [[Paper]](https://arxiv.org/pdf/2101.09808.pdf)		
* Ordering Chaos: Memory-Aware Scheduling of Irregularly Wired Neural Networks for Edge Devices, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/9bf31c7ff062936a96d3c8bd1f8f2ff3-Paper.pdf)
* A Tensor Compiler for Unified Machine Learning Prediction Serving, OSDI 20 [[Paper]](https://www.usenix.org/system/files/osdi20-nakandala.pdf)
* Interstellar: Using Halide’s Scheduling Language to Analyze DNN Accelerators, ASPLOS 20 [[Paper]](https://arxiv.org/pdf/1809.04070.pdf)
* Rammer: Enabling Holistic Deep Learning Compiler Optimizations with rTasks,	OSDI 20	[[Paper]](https://www.usenix.org/system/files/osdi20-ma.pdf)		
* FlexTensor: An Automatic Schedule Exploration and Optimization Framework for Tensor Computation on Heterogeneous System, ASPLOS 20 [[Paper]](https://ceca.pku.edu.cn/docs/20200915213803856105.pdf)
* Ansor: Generating High-Performance Tensor Programs for Deep Learning,	OSDI	20	[[Paper]](https://www.usenix.org/system/files/osdi20-zheng.pdf)			
* MNN: A Universal and Efficient Inference Engine, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/8f14e45fceea167a5a36dedd4bea2543-Paper.pdf)
* Astra: Exploiting Predictability to Optimize Deep Learning, ASPLOS 19 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2019/02/astra-asplos19.pdf)
* Bridging the Gap Between Neural Networks and Neuromorphic Hardware with A Neural Network Compiler, ASPLOS 18 [[Paper]](https://arxiv.org/pdf/1801.00746.pdf)
* CapeVM: A Safe and Fast Virtual Machine for Resource-Constrained Internet-of-Things Devices, SenSys 18 [[Paper]](https://dl.acm.org/doi/10.1145/3274783.3274842) (NO ML)
* TVM: An Automated End-to-End Optimizing Compiler for Deep Learning, OSDI 18	[[Paper]](https://www.usenix.org/conference/osdi18/presentation/chen)	

<a name="networking-and-communication"></a>
## Networking and Communication (337)

<a name="user-content-battery"></a>
### 🔋 Battery (225)
<a name="user-content-cellular"></a>
#### 📶 Cellular (Total: 48 | No ML(37) | ML(4) | DL(7)
* iCellular: Device-Customized Cellular Network Access on Commodity Smartphones, NSDI 16 [[Paper]](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-li-yuanjie.pdf) (NO ML)
* Eliminating Channel Feedback in Next-Generation Cellular Networks, SIGCOMM 16 [[Paper]](https://dl.acm.org/doi/10.1145/2934872.2934895) (NO ML)
* Proteus: a network service control platform for service evolution in a mobile software defined infrastructure, MobiCom 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2973750.2973757) (NO ML)
* LTE in Unlicensed Spectrum: Are We There Yet?, MobiCom 16 [[Paper]](http://www.cs.albany.edu/~mariya/courses/csi445660F16/papers/p135-chai.pdf) (NO ML)
* QuickC: Practical sub-millisecond transport for small cells, MobiCom 16 [[Paper]](https://web.stanford.edu/~skatti/pubs/mobicom16-quickc.pdf) (NO ML)
* A High Performance Packet Core for Next Generation Cellular Networks, SIGCOMM 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3098822.3098848) (NO ML)
* Experience: Automating Diagnosis of Cellular Radio Access Network Problems, MobiCom 17 [[Paper]](https://www.anand-iyer.com/papers/ran-mobicom2017.pdf)(ML)
* Chorus: Truly Distributed Distributed-MIMO, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230578) (NO ML)
* Mitigating the Latency-Accuracy Trade-off in Mobile Data Analytics Systems, MobiCom 18 [[Paper]](https://www.anand-iyer.com/papers/cellscope-mobicom2018.pdf) (ML)
* How Should I Slice My Network? A Multi-Service Empirical Evaluation of Resource Sharing Efficiency, MobiCom 18 [[Paper]](https://core.ac.uk/download/pdf/288500453.pdf) (NO ML)
* A reliable distributed cellular core network for hyper-scale public clouds, MobiCom 18 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2018/02/ECHO-TR.pdf) (NO ML)
* CASTLE over the Air: Distributed Scheduling for Cellular Data Transmissions, MobiSys 19 [[Paper]](https://research.ece.cmu.edu/lions/Papers/CASTLE_MobiSys.pdf)(ML)
* An In-depth Study of Commercial MVNO: Measurement and Optimization, MobiSys 19 [[Paper]](https://www.cs.binghamton.edu/~yaoliu/publications/mobisys19-mvno.pdf)(ML)
* Bridging the Data Charging Gap in the Cellular Edge, SIGCOMM 19 [[Paper]](http://www.yuanjiel.com/publication/sigcomm19-camera-ready.pdf) (NO ML)
* An Active-Passive Measurement Study of TCP Performance over LTE on High-speed Rails, MobiCom 19 [[Paper]](https://arxiv.org/pdf/1812.04823.pdf) (NO ML)
* Experiences: Design, Implementation, and Deployment of CoLTE, a Community LTE Solution, MobiCom 19 [[Paper]](https://kurti.sh/pubs/CoLTE_Mobicom_2019.pdf) (NO ML)
* Detecting if LTE is the Bottleneck with BurstTracker, MobiCom 19 [[Paper]](https://cseweb.ucsd.edu/~schulman/docs/mobicom19-bursttracker.pdf) (NO ML)
* A Systematic Way to LTE Testing, MobiCom 19 [[Paper]](https://people.computing.clemson.edu/~jmarty/projects/lowLatencyNetworking/papers/3GPP/LTE/AsystematicWayToMeasureLTE.pdf) (NO ML)
* Beyond 5G: Reliable Extreme Mobility Management, SIGCOMM 20 [[Paper]](http://web.cs.ucla.edu/~qianruli/files/sigcomm20-rem.pdf) (NO ML)
* Understanding Operational 5G: A First Measurement Study on Its Coverage, Performance and Energy Consumption, SIGCOMM 20 [[Paper]](http://xyzhang.ucsd.edu/papers/DXu_SIGCOMM20_5Gmeasure.pdf) (NO ML)
* A Low Latency and Consistent Cellular Control Plane, SIGCOMM 20 [[Paper]](https://web.lums.edu.pk/~zafar/sigcomm2020.pdf) (NO ML)
* Microscope: Mobile Service Traffic Decomposition for Network Slicing as a Service, MobiCom 20 [[Paper]](https://core.ac.uk/download/pdf/334415278.pdf)(DL)
* DMM: Fast Map Matching for Cellular Data, MobiCom 20 [[Paper]](https://sites.ucmerced.edu/files/wdu/files/20mobicom-dmm.pdf)(DL)
* Challenge: COSMOS: A City-Scale Programmable Testbed for Experimentation with Advanced Wireless, MobiCom 20 [[Paper]](https://www.winlab.rutgers.edu/~sumitm/downloads/MobiCom2020_COSMOS.pdf) (NO ML)
* Device-Based LTE Latency Reduction at the Application Layer, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-tan.pdf)(NO ML)
* Democratizing Cellular Access with CellBricks, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3473336.pdf) (NO ML)
* A Nationwide Study on Cellular Reliability: Measurement, Analysis, and Enhancements, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472908.pdf) (NO ML)
* A Variegated Look at 5G in the Wild: Performance, Power, and QoE Implications, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472923.pdf)[[code]](https://github.com/SIGCOMM21-5G/artifact)(DL)
* Auric: Using Data-driven Recommendation to Automatically Generate Cellular Configuration, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472906.pdf)（DL）
* FSA: Fronthaul Slicing Architecture for 5G using dataplane programmable switches, MobiCom 21 [[Paper]](https://www.comp.nus.edu.sg/~chanmc/papers-by-year/2021-FSA.pdf) (NO ML)
*  Nervion: A Cloud Native RAN Emulator for Scalable and Flexible Mobile Core Evaluation, MobiCom 21 [[Paper]](https://www.pure.ed.ac.uk/ws/portalfiles/portal/224348439/Nervion_LARREA_DOA13082021_AFV.pdf)(No ML)
* DeepRadar: A Deep-Learning-based Environmental Sensing Capability Sensor Design for CBRS, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3448632) (DL)
* FIRE: Enabling Reciprocity for FDD MIMO Systems, MobiCom 21 [[Paper]](https://deepakv.web.illinois.edu/assets/papers/FIRE_Mobicom2021.pdf) (DL)
* Global Mobile Network Aggregators: Taxonomy, Roaming Performance and Optimization, MobiSys 22 [[Paper]](https://www.aqualab.cs.northwestern.edu/wp-content/uploads/2022/05/SAlcala-Marin-Mobisys22.pdf) (NO ML)
* L25GC: A Low Latency 5G Core Network based on High-Performance NFV Platforms, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3544216.3544267) (NO ML)
* Understanding 5G Performance for Real-world Services: a Content Provider’s Perspective, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3544216.3544219) (NO ML)
* Mobile Access Bandwidth in Practice: Measurement, Analysis, and Implications, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3544216.3544237) (NO ML)
* Vivisecting Mobility Management in 5G Cellular Networks, SIGCOMM 22 [[Paper]](https://zhan6841.github.io/files/vivisectingmobility-sigcomm22.pdf) (NO ML)
* Warm-started quantum sphere decoding via reverse annealing for massive IoT connectivity, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560516)  (NO ML)
* Towards Ultra-low Power OFDMA Downlink Demodulation, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568509) (NO ML)
* Taking 5G RAN Analytics and Control to a New Level, MobiCom 23 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2022/12/JanusTechnicalReport.pdf) (NO ML)
* CA++: Enhancing Carrier Aggregation Beyond 5G, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592500) (NO ML)
* CoreKube: An Efficient, Autoscaling and Resilient Mobile Core System, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3592522) [[Code]](https://github.com/netsys-edinburgh/CoreKube) (NO ML) (Best Artifact Award)
* X-Plane: A High-Throughput Large-Capacity 5G UPF, MobiCom 23 [[Paper]](https://jhc.sjtu.edu.cn/~bjiang/papers/Liu_MobiCom2023_X-Plane.pdf) (NO ML)
* Enabling Resilience in Virtualized RANs with Atlas, MobiCom 23 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2023/09/atlas_mobicom.pdf) (NO ML)
* NeRF2: Neural Radio-Frequency Radiance Fields, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3592527) (DL)
* DChannel: Accelerating Mobile Applications With Parallel High-bandwidth and Low-latency Channels, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-sentosa.pdf) (NO ML)
* Scalable Distributed Massive MIMO Baseband Processing, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-gong.pdf) (NO ML)


<a name="user-content-wifi"></a>
#### WiFi (Total: 16 | No ML(12) | ML(1) | DL(3))
* RF-Diffusion: Radio Signal Generation via Time-Frequency Diffusion, MobiCom 24 [[Paper]](https://arxiv.org/pdf/2404.09140) (DL)
* Characterizing and Improving WiFi Latency in Large-Scale Operational Networks, MobiSys 16 [[Paper]](http://zmy.io/files/mobisys16-WiFiSeer.pdf)（ML）
* Real-time Distributed MIMO Systems, SIGCOMM 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2934872.2934905) (NO ML)
* Wi-Fi Goes to Town: Rapid Picocell Switching for Wireless Transit Networks, SIGCOMM 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3098822.3098846) (NO ML)
* FlexCore: Massively Parallel and Flexible Processing for Large MIMO Access Points, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-husmann.pdf) (NO ML)
* SWAN: Stitched Wi-Fi ANtennas, MobiCom 18 [[Paper]](https://wands.sg/publications/full_list/papers/MobiCom_18_1.pdf) (NO ML)
* CloseTalker: Secure, Short-Range Ad Hoc Wireless Communication, MobiSys 19 [[Paper]](https://www.cs.dartmouth.edu/~dfk/research/pierson-closetalker/pierson-closetalker.pdf) (NO ML)
* On-Off Noise Power Communication, MobiCom 19 [[Paper]](https://span.engineering.wustl.edu/pub/lundrigan2019onoff.pdf) (NO ML)
* RFlens: metasurface-enabled beamforming for IoT communication and sensing, MobiCom 21 [[Paper]](https://dl.acm.org/doi/10.1145/3447993.3483238) (NO ML)
* MIXIQ: re-thinking ultra-low power receiver design for next-generation on-body applications, MobiCom 21 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/Mobicom21-MIXIQ.pdf) (NO ML)
* TransFi: Emulating Custom Wireless Physical Layer from Commodity WiFi, MobiSys 22 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobisys22.pdf) (NO ML)
* Mobile Access Bandwidth in Practice: Measurement, Analysis, and Implications, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3544216.3544237) (NO ML)
* AiFi: AI-Enabled WiFi Interference Cancellation with Commodity PHY-Layer Information, SenSys 22 [[Paper]](https://sites.pitt.edu/~weigao/publications/sensys22.pdf)（DL）
* Upscaling Fog Computing in Oceans for Underwater Pervasive Data Science Using Low-Cost Micro-Clouds, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3575801) (DL)
* SenCom: Integrated Sensing and Communication with Practical WiFi, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613274) (NO ML)
* SlimWiFi: Ultra-Low-Power IoT Radio Architecture Enabled by Asymmetric Communication, NSDI 23 [[paper]](https://www.usenix.org/system/files/nsdi23-zhao-renjie.pdf) (NO ML)

<a name="user-content-acoustic"></a>
#### 🎵 Acoustic (Total:9  | No ML(8) | ML(0) | DL(1))
* Messages Behind the Sound: Real-Time Hidden Acoustic Signal Capture with Smartphones, MobiCom 16 [[Paper]](https://cse.buffalo.edu/~lusu/papers/MobiCom2016.pdf) (NO ML)
* Near-Ultrasound Communication for TV's 2nd Screen Services,  MobiCom 16 [[Paper]](https://dl.acm.org/doi/10.1145/2973750.2973774) (NO ML)
* Deaf-aid: mobile IoT communication exploiting stealthy speaker-to-gyroscope channel, MobiCom 20 [[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-mobicom2020c.pdf) (NO ML)
* AmphiLight: Direct Air-Water Communication with Laser Light, NSDI 20 [[Paper]](https://www.usenix.org/conference/nsdi20/presentation/carver)(NO ML)
* BatComm: Enabling Inaudible Acoustic Communication with High-throughput for Mobile Devices, SenSys 20 [[Paper]](https://web.eecs.utk.edu/~jliu/publications/bai2020batcomm.pdf) (NO ML)
* Shrimp: a robust underwater visible light communication system, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448616) (NO ML)	
* Underwater Messaging Using Mobile Devices, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3544216.3544258)[[Code]](https://github.com/uw-x/watercomms) (NO ML)
* AquaHelper: Underwater SOS Transmission and Detection in Swimming Pools, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625816) (NO ML)
* Towards Spatial Selection Transmission for Low-end IoT devices with SpotSound, MobiCom 23 [[Paper]](https://tachen-cs.github.io/data/papers/2023-mobicom-spotsound/SpotSound.pdf) (DL)

<a name="user-content-visible-Light"></a>
#### 💡 Visible Light (Total: 17 | No ML(14) | ML(0) | DL(3))
* The DarkLight Rises: Visible Light Communication in the Dark, MobiCom 16 [[Paper]](https://www.cs.dartmouth.edu/~xia/papers/mobicom16-darklight.pdf) (NO ML)
* Card-stunt as a Service: Empowering a Massively Packed Crowd for Instant Collective Expressiveness, MobiSys 17 [[Paper]](https://nclab.kaist.ac.kr/uploads/2017/08/mobisys2017_cardstunt.pdf) (NO ML)
* POLI: Long-Range Visible Light Communications Using Polarized Light Intensity Modulation, MobiSys 17 [[Paper]](https://dl.acm.org/doi/10.1145/3081333.3081353) (NO ML)
* ReflexCode: Coding with Superposed Reflection Light for LED-Camera Communication, MobiCom 17 [[Paper]](https://dl.acm.org/doi/10.1145/3117811.3117836) (NO ML)
* ChromaCode: A Fully Imperceptible Screen-Camera Communication System, MobiCom 18 [[Paper]](https://cswu.me/papers/mobicom18_chromacode_paper.pdf) (NO ML)
* Breaking the Limitations of Visible Light Communication Through Its Side Channel, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430728)(NO ML)
* Zero-Wire: A Deterministic and Low-Latency Wireless Bus Through Symbol-Synchronous Transmission of Optical Signals, SenSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3384419.3430897) (NO ML) (Best Paper)
* RayTrack: enabling interference-free outdoor mobile VLC with dynamic field-of-view, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3466867) (NO ML)
* RadioInLight: Doubling the Data Rate of VLC Systems, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483271) (NO ML)
* Shrimp: a robust underwater visible light communication system, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448616) (NO ML)
* SpiderWeb: Enabling Through-Screen Visible Light Communication, SenSys 21 [[Paper]](https://pure.tudelft.nl/ws/portalfiles/portal/103302355/3485730.3485948.pdf) (NO ML)
* DeepLight: Robust & Unobtrusive Real-time Screen-Camera Communication for Real-World Displays, IPSN 21 [[Paper]](https://arxiv.org/pdf/2105.05092.pdf)(DL)
* AIRCODE: Hidden Screen-Camera Communication on an Invisible and Inaudible Dual Channel, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-qian-kun.pdf) (NO ML)
* When VLC Meets Under-Screen Camera, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596855) (NO ML)
* Harmony: An In-band Time Synchronisation System for Visible Light Communication, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568549) (NO ML)
* CORE-lens: simultaneous communication and object recognition with disentangled-GAN cameras, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560526)(DL)
* Practical Optical Camera Communication Behind Unseen and Complex Backgrounds, MobiSys 24, [[Paper]]([https://dl.acm.org/doi/10.1145/3643832.3661861)(https://dl.acm.org/doi/10.1145/3643832.3661866]) (DL)

<a name="user-content-bluetooth"></a>
#### Bluetooth (Total: 4 | No ML(4) | ML(0) | DL(0))
* Beetle: Flexible Communication for Bluetooth Low Energy, MobiSys 16 [[Paper]](http://iot.stanford.edu/pubs/beetle-mobisys16.pdf) (NO ML)
* BLEach: Exploiting the Full Potential of IPv6 over BLE in Constrained Embedded IoT Devices, SenSys 17 [[Paper]](https://nes-lab.org/wordpress/wp-content/uploads/2019/11/spoerk17bleach.pdf) (NO ML)
* enClosure: Group Communication via Encounter Closures, MobiSys 19 [[Paper]](https://people.mpi-sws.org/~druschel/publications/enclosure.pdf) (NO ML)
* BLEX: Flexible Multi-Connection Scheduling for Bluetooth Low Energy, IPSN 21 [[Paper]](https://dl.acm.org/doi/10.1145/3412382.3458271)（NO ML）

<a name="user-content-millimeter-Wave"></a>
#### 〰️ Millimeter-Wave (Total: 25 | No ML(23) | ML(2) | DL(0))
* BeamSpy: Enabling Robust 60 GHz Links Under Blockage, NSDI 16 [[Paper]](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-sur.pdf) (NO ML)
* OpenMili: A 60 GHz Software Radio Platform With a Reconfigurable Phased-Array Antenna, MobiCom 16 [[paper]](http://xyzhang.ucsd.edu/papers/JZhang_MobiCom16_OpenMili.pdf) (NO ML)
* Facilitating Robust 60 GHz Network Deployment by Sensing Ambient Reflectors, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-wei-teng.pdf) (NO ML)
* Pose Information Assisted 60 GHz Networks: Towards Seamless Coverage and Mobility Support, MobiCom 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3117811.3117832) (NO ML)
* WiFi-Assisted 60 GHz Wireless Networks, MobiCom 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3117811.3117817) (NO ML)
* Fast Millimeter Wave Beam Alignment, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230581) (NO ML)
* Adaptive Codebook Optimization for Beam Training on Off-the-Shelf IEEE 802.11ad Devices, MobiCom 18 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/614/Adaptive_Codebook_Optimization_Beam_Training_Off-the-Shelf_IEEE%20802.11ad_Devices_2018_EN.pdf?sequence=1&isAllowed=y)(NO ML)
* Towards Scalable and Ubiquitous Millimeter-Wave Wireless Networks, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241579) (NO ML)
* Multi-Stream Beam-Training for mmWave MIMO Networks, MobiCom 18 [[Paper]](https://cse.buffalo.edu/faculty/dimitrio/publications/mobicom18_mute.pdf)(NO ML)
* LiSteer: mmWave Beam Acquisition and Steering by Tracking Indicator LEDs on Wireless APs, MobiCom 18 [[Paper]](https://dl.acm.org/doi/10.1145/3241539.3241542) (NO ML)
* Many-to-Many Beam Alignment in Millimeter Wave Networks, NSDI 19 [[Paper]](https://www.usenix.org/system/files/nsdi19-jog.pdf) (NO ML)
* A Millimeter Wave Network for Billions of Things, SIGCOMM 19 [[Paper]](http://web.cs.ucla.edu/~omid/Papers/Sigcomm19.pdf) (NO ML)
* KinPhy: a kinetic in-band channel for millimetre-wave networks, SenSys 19 [[Paper]](https://dl.acm.org/doi/10.1145/3356250.3360039) (NO ML)
* mm-FLEX: An Open Platform for Millimeter-Wave Mobile Full-Bandwidth Experimentation, MobiSys 20 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/808/MOBISYS_2020_FINAL.pdf?sequence=1&isAllowed=y) (NO ML)
* M-Cube: a millimeter-wave massive MIMO software radio, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3380892) (NO ML) (Best Papaer Award)
* Millimeter-Wave Full Duplex Radios, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3380879)(NO ML)
* X-Array: Approximating Omnidirectional Millimeter-Wave Coverage Using an Array of Phased Arrays, MobiCom 20 [[Paper]](http://xyzhang.ucsd.edu/papers/SWang_MobiCom20_X-Array.pdf) (NO ML)
* SpaceBeam: LiDAR-driven one-shot mmWave beam management, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3466864)(ML)
* Practical Null Steering in Millimeter Wave Networks, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-madani.pdf) (NO ML)
* Two beams are better than one: Towards Reliable and High Throughput mmWave Links, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472924.pdf) (NO ML)
* M5: Facilitating Multi-user Volumetric Content Delivery with Multi-lobe Multicast over mmWave, SensSys 22 [[Paper]](http://www.phpathak.com/files/m5-sensys.pdf)(ML)
* mmWall: A Steerable, Transflective Metamaterial Surface for NextG mmWave Networks, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-cho-kun-woo.pdf) (NO ML)
* SIGNiPHY: Reconciling random access with directional reception for efficient mmWave WLANs, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596860) (NO ML)
* Bringing Millimeter Wave Technology to Any IoT Device, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613255) (NO ML)
* mmRipple: Communicating with mmWave Radars through Smartphone Vibration, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586956) (NO ML)

<a name="user-content-uwb"></a>
#### UWB (Total: 5 | No ML(5) | ML(0) | DL(0))
* One Flood to Route Them All:Ultra-fast Convergecast of Concurrent Flows over UWB, SenSys 20 [[Paper]](http://disi.unitn.it/~picco/papers/sensys20_weaver.pdf) (NO ML)
* Octopus: a practical and versatile wideband MIMO sensing platform, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483267)(NO ML but supports ML)
* Understanding and Mitigating the Impact of Wi-Fi 6E Interference on Ultra-Wideband Communications and Ranging, IPSN 22 [[Paper]](http://www.carloalbertoboano.com/documents/brunner22uwbwifi.pdf)(NO ML)
* WISE: Low-Cost Wide Band Spectrum Sensing Using UWB, SenSys 22 [[Paper]](https://huangqy7.github.io/Paper/WISE_final.pdf) (NO ML)
* Network On or Off? Instant Global Binary Decisions over UWB with Flick, IPSN 23 [[Paper]](http://disi.unitn.it/~picco/papers/ipsn23.pdf) (NO ML)

<a name="user-content-tv-whitespace"></a>
#### TV Whitespace (Total: 5 | No ML(5) | ML(0) | DL(0))
*  SNOW: Sensor Network over White Spaces, SenSys 16 [[Paper]](https://www.cse.wustl.edu/~lu/papers/sensys16.pdf) (NO ML)
* Enabling Reliable, Asynchronous, and Bidirectional Communication in Sensor Networks over White Spaces, SenSys 17 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2018/02/sensys17.pdf) (NO ML)
* WhiteHaul: An Efficient Spectrum Aggregation System for Low-Cost and High Capacity Backhaul over White Spaces, MobiSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3386901.3388950) (NO ML)(using 801.11ac cards)
* OwLL: Accurate LoRa Localization using the TV Whitespaces, IPSN 21 [[Paper]](https://swarunkumar.com/papers/owll-ipsn2021.pdf) (NO ML)
* Whisper: IoT in the TV White Space Spectrum, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-chakraborty.pdf) (NO ML)

<a name="user-content-loralorawan"></a>
#### LoRa/LoRaWAN (Total: 24 | No ML(18) | ML(2) | DL(4))
* WIDESEE: Towards Wide-Area Contactless Wireless Sensing, SenSys 19 [[Paper]](https://zwang4.github.io/publications/sensys19.pdf) (NO ML)	
* FTrack: parallel decoding for LoRa transmissions, SenSys 19 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/FTrack_Sensys19.pdf)(NO ML)
* LongShoT: Long-Range Synchronization of Time, IPSN 19 [[Paper]](https://par.nsf.gov/servlets/purl/10107899) (NO ML)
* Automated Estimation of Link Quality for LoRa: A Remote Sensing Approach, IPSN 19 [[Paper]](https://pure.tudelft.nl/ws/files/55547022/IPSN2019.pdf)(ML)
* Exploring LoRa for Long-range Through-wall Sensing, IMWUT/UbiComp 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3397326) (NO ML)	
* LMAC: efficient carrier-sense multiple access for LoRa, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419200) (NO ML)
* SateLoc: A Virtual Fingerprinting Approach to Outdoor LoRa Localization using Satellite Images, IPSN 20 [[Paper]](https://ieeexplore.ieee.org/document/9111031)(ML)
* Concurrent Interference Cancellation : Decoding Multi-Packet Collisions in LoRa, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472931.pdf) (NO ML)
* NELoRa: Towards Ultra-low SNR LoRa Communication with Neural-enhanced Demodulation, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485928)(DL)
* STeC: Exploiting Spatial and Temporal Correlation for Event-based Communication in WSNs, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485951)(NO ML)
* OwLL: Accurate LoRa Localization using the TV Whitespaces, IPSN 21 [[Paper]](https://swarunkumar.com/papers/owll-ipsn2021.pdf)(NO ML)
* DeepLoRa: Learning accurate path loss model for long distance links in LPWAN, INFOCOM 21 [[Paper]](https://ieeexplore.ieee.org/document/9488784)(DL)
* Combating link dynamics for reliable lora connection in urban settings, MobiCom 21 [[Paper]](https://dl.acm.org/doi/10.1145/3447993.3483250) (NO ML)
* PCube: Scaling LoRa Concurrent Transmissions with Reception Diversities, MobiCom 21 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/PCube-MobiCom21.pdf) (NO ML)
* CurvingLoRa to Boost LoRa Network Throughput via Concurrent Transmission, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-li_chenning.pdf) (NO ML)
* OpenLoRa: Validating LoRa Implementations through an Extensible and Open-sourced Framework, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-mishra.pdf) (NO ML)
* HyLink: Towards High Throughput LPWANs with LoRa Compatible Communication, SenSys 22 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/HyLink-SenSys22.pdf)(NO ML)
* MaLoRaGW: Multi-User MIMO Transmission for LoRa, SenSys 22 [[Paperp]](https://www.cse.msu.edu/~hzeng/papers/Hossein22_Sensys_MaLoRaGW.pdf) (NO ML)
* LLDPC: A Low-Density Parity-Check Coding Scheme for LoRa Networks, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568547) (DL)
* BSMA: scalable LoRa networks using full duplex gateways, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560544) (NO ML)
* Citywide LoRa Network Deployment and Operation: Measurements, Analysis, and Implications, SenSys 23 [[Paper]](http://tns.thss.tsinghua.edu.cn/~jiliang/publications/SenSys23-CityWAN.pdf) (NO ML)
* Enabling Concurrency for Non-orthogonal LoRa Channels, MobiCom23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613268) (NO ML)
* XCopy: Boosting Weak Links for Reliable LoRa Communication, MobiCom23 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/XCopy-MobiCom23.pdf) (NO ML)
* ChirpTransformer: Versatile LoRa Encoding for Low-power Wide-area IoT, MobiSys 24, [[Paper]](https://dl.acm.org/doi/10.1145/3643832.3661861) (DL) 

<a name="user-content-lpwan"></a>
#### LPWAN (Total: 13  | No ML(12) | ML(0) | DL(1))
* Data Prediction + Synchronous Transmissions = Ultra-low Power Wireless Sensor Networks, SenSys 16 [[Paper]](https://disi.unitn.it/~picco/papers/sensys16.pdf) (NO ML)
* Challenge: Unlicensed LPWANs Are Not Yet the Path to Ubiquitous Connectivity, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345444) (NO ML) 
* Combating Packet Collisions Using Non-Stationary Signal Scaling in LPWANs, MobiSys 20 [[Paper]](http://tns.thss.tsinghua.edu.cn/~jiliang/publications/MOBISYS2020_NSCALE.pdf) (NO ML)
* A Cloud-Optimized Link Layer for Low-Power Wide-Area Networks, MobiSys 20 [[Paper]](https://users.ece.cmu.edu/~agr/resources/publications/mobisys_20_opr.pdf) (NO ML)
* WiChronos: energy-efficient modulation for long-range, large-scale wireless networks, MobiCom 20 [[Paper]](https://uwconnect.ece.wisc.edu/wp-content/uploads/sites/1525/2021/10/WiChronos.pdf) (NO ML)
* Nephalai: Towards LPWAN C-RAN with Physical Layer Compression, MobiCom 20 [[Paper]](https://arxiv.org/pdf/2008.02599.pdf) (NO ML)
* Joltik: Enabling Energy-Efficient “Future-Proof” Analytics on Low-Power Wide-Area Networks, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419204) (NO ML)
* Frequency Configuration for Low-Power Wide-Area Networks in a Heartbeat, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-gadre.pdf) (NO ML)
* Seirios: Leveraging Multiple Channels for LoRaWAN Indoor and Outdoor Localization, MobiCom 21 [[Paper]](https://arxiv.org/pdf/2108.06884.pdf) (NO ML)
* LoPhy: A Resilient and Fast Covert Channel over LoRa PHY, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586952) (NO ML)
* Link Quality Modeling for LoRa Networks in Orchards, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586969) (NO ML)
* FLoRa: Energy-Efficient, Reliable, and Beamforming-Assisted Over-The-Air Firmware Update in LoRa Networks, IPSN 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3583120.3586963)(NO ML)
* Low-Bandwidth Self-Improving Transmission of Rare Training Data, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613300) (DL)

<a name="user-content-sdr"></a>
#### SDR (Total: 7 | No ML(7) | ML(0) | DL(0))
* The Tick Programmable Low-Latency SDR System, MobiCom 17 [[Paper]](https://web.cs.ucla.edu/~tan/documents/mobicom17.pdf)(NO ML) (Best Community Paper Award)
* SparSDR: Sparsity-proportional Backhaul and Compute for SDRs, MobiSys 19 [[Paper]](http://people.csail.mit.edu/moein/papers/sparsdr-mobisys19.pdf) (NO ML)
* Towards Programming the Radio Environment with Large Arrays of Inexpensive Antennas, NSDI 19 [[Paper]](https://www.usenix.org/system/files/nsdi19-li-zhuqi.pdf) (NO ML)(supports multiple objectives)
* SDR receiver using commodity wifi via physical-layer signal reconstruction, MobiCom 20 [[Paper]](https://seit.egr.msu.edu/paper/Mobicom2020-SDRLite.pdf)（No ML）（introduces a device identification application using DL）
* TinySDR: Low-Power SDR Platform for Over-the-Air Programmable IoT Testbeds, NSDI 20 [[Paper]](https://www.usenix.org/conference/nsdi20/presentation/hessar) (NO ML)
* TyrLoc: a low-cost multi-technology MIMO localization system with a single RF chain,	MobiSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467677)	(NO ML)
* RFClock: Timing, Phase and Frequency Synchronization for Distributed Wireless Networks, MobiCom 21 [[Paper]](https://genesys-lab.org/papers/RFCLOCK_MOBICOM2021.pdf) (NO ML)(works in 2.4GHz and 915MHz ISM band)

<a name="user-content-ctc"></a>
#### CTC (Total: 23 | No ML(22) | ML(0) | DL(1))
* B2W2: N-Way Concurrent Communication for IoT Devices, SenSys 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2994551.2994561) (NO ML)
* BlueBee: a 10,000x Faster Cross-Technology Communication via PHY Emulation, SenSys 17 [[Paper]](https://cs.gmu.edu/~song/paper/SenSys17_Wenchao.pdf) (NO ML)
* WEBee: Physical-Layer Cross-Technology Communication via Emulation, MobiCom 16 [[Paper]](https://www-users.cse.umn.edu/~tianhe/Papers/WEBee.pdf) (NO ML) (Best Paper Awards)
* Chiron: Concurrent High Throughput Communication for IoT Devices, MobiSys 18 [[Paper]](https://cis.csuohio.edu/~chi/publication/li-2018-cch-3210240-3210346/li-2018-cch-3210240-3210346.pdf) (NO ML)
* Explicit Channel Coordination via Cross-technology Communication, MobiSys 18 [[Paper]](https://par.nsf.gov/servlets/purl/10076616) (NO ML)
* Achieving Receiver-Side Cross-Technology Communication with Cross-Decoding, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241547) (NO ML)
* Cross-Frequency Communication: Near-Field Identification of UHF RFIDs with WiFi!, MiboCom 18 [[Paper]](https://www4.comp.polyu.edu.hk/~csyanglei/data/files/tifi-mobicom18.pdf) (NO ML)
* Exploiting WiFi Guard Band for Safeguarded ZigBee, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274835)(NO ML)
* LTE2B: Time-Domain Cross-Technology Emulation under LTE Constraints, SenSys 19 [[Paper]](https://liux4189.github.io/files/LTE2B_Sensys_CameraReady.pdf) (NO ML)
* Parallel Inclusive Communication for Connecting Heterogeneous IoT Devices at the Edge, SenSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3356250.3360046) (NO ML)
* X-MIMO: Cross-Technology Multi-User MIMO, SenSys 20 [[Paper]](https://par.nsf.gov/servlets/purl/10303948) (NO ML)
* BlueFi: Bluetooth over WiFi, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472920.pdf) (NO ML)
* WiBeacon: Expanding BLE Location-based Services via WiFi, MobiCom 21 [[Paper]](https://liux4189.github.io/files/WiBeacon_MobiCom_CameraReady.pdf) (NO ML)
* Network architecture, Internet of Things, Interoperability., MobiCom 22 [[Paper]](https://desword.github.io/paper/mobisys22-tinynet.pdf) (NO ML)
* De-spreading over the air: long-range CTC for diverse receivers with LoRa, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560524) (NO ML)
*  FLEW: Fully Emulated WiFi, MobiCom 22 [[Paper]](https://rtcl.eecs.umich.edu/rtclweb/assets/publications/2022/mobicom22-cho.pdf) (NO ML)
* Towards Seamless Wireless Link Connection, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596833) (NO ML)
* WibZig: Reliable and Commodity-device Compatible PHY-CTC via Chip Emulation in Phase, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3587046) (NO ML)
* mmRipple: Communicating with mmWave Radars through Smartphone Vibration, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586956) (NO ML)
* Networking across boundaries: enabling wireless communication through the water-air interface SIGCOMM 18[[Paper]](https://dl.acm.org/doi/10.1145/3230543.3230580) (NO	ML)
* XiTuXi: Sealing the Gaps in Cross-Technology Communication by Neural Machine Translation, Sensys 23 [[Paper]](https://dl.acm.org/doi/10.1145/3625687.3625802) (DL)
* Unify: Turning BLE/FSK SoC into WiFi SoC, MobiCom 23 [[Paper]](https://rtcl.eecs.umich.edu/rtclweb/assets/publications/2023/mobicom23-cho.pdf) (NO ML)
* RF-SIFTER: Sifting Signals at Layer-0.5 to Mitigate Wideband Cross-Technology Interference for IoT, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592513) (NO ML)


<a name="user-content-other-multi-band"></a>
#### Multi-band Operation (Total: 4 | No ML(4) | ML(0) | DL(0))
* An In-depth Understanding of Multipath TCP on Mobile Devices: Measurement and System Design, MobiCom 16 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/multipath_mobicom16.pdf) (NO ML)
* MuSher: An Agile Multipath-TCP Scheduler for Dual-Band 802.11ad/ac Wireless LANs, MobiCom 19 [[Paper]](https://cse.buffalo.edu/faculty/dimitrio/publications/mobicom19.pdf) (NO ML)
* MPBond: Efficient Network-level Collaboration Among Personal Mobile Devices, MobiSys 20 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/mpbond_mobisys20.pdf) (NO ML)
* A real-time experimentation platform for sub-6 GHz and millimeter-wave MIMO systems, MobiSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3458864.3466868) [[code]](https://github.com/rafaruizortiz/MIMORPH)(NO ML)


<a name="user-content-other-sensor-network"></a>
#### Other Sensor Network (Total: 25 | No ML(21) | ML(2) | DL(2))
* Ripple II: Faster Communication through Physical Vibration, NSDI 16 [[Paper]](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-roy.pdf) (NO ML)
* Effectively Capturing Attention Using the Capture Effect, SenSys 16 [[Paper]](https://tik-db.ee.ethz.ch/file/b468db98c89b23c868db49b3e72817d0/paper-sp.pdf) (NO ML)
* Staffetta: Smart Duty-Cycling for Opportunistic Data Collection, SenSys 16 [[Paper]](https://www.st.ewi.tudelft.nl/marco/files/staffetta_Sensys16.pdf) (NO ML)
* Network-wide Consensus Utilizing the Capture Effect in Low-power Wireless Networks, SenSys 17 [[Paper]](http://www.diva-portal.org/smash/get/diva2:1170407/FULLTEXT01.pdf)(NO ML)
* Empowering Low-Power Wide Area Networks in Urban Settings, SIGCOMM 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3098822.3098845) (NO ML)
* MagneComm: Magnetometer-based Near-Field Communication, MobiCom 17 [[Paper]](https://www.cs.sjtu.edu.cn/~yichao/pmwiki/assets/publications/mobicom17_pan.pdf) (NO ML)
* Surface MIMO: Using Conductive Surfaces For MIMO Between Small Devices, MobiCom 18 [[Paper]](https://arxiv.org/pdf/1809.02726.pdf) (NO ML)
* System Architecture Directions for Post-SoC/32-bit Networked Sensors, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274839) (NO ML) (Best Paper Runner-up)
* Mixer: Efficient Many-to-All Broadcast in Dynamic Wireless Mesh Networks, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274849) (NO ML)(in principle Mixer works on any physical layer that features the capture effect)
* NEOFog: Nonvolatility-Exploiting Optimizations for Fog Computing, ASPLOS 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3173162.3177154) (NO ML) 
* Blind Distributed MU-MIMO for IoT Networking over VHF Narrowband Spectrum, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345427)(NO ML)
* SkySense: Terrestrial and Aerial Spectrum Use Analysed Using Lightweight Sensing Technology with Weather Balloons, MobiSys 20 [[Paper]](https://www.lenders.ch/publications/conferences/mobisys20.pdf) (NO ML)
* Understanding and Embracing the Complexities of the Molecular Communication Channel in Liquids, MobiCom 20 [[Paper]](https://haitham.ece.illinois.edu/Papers/BioMC.pdf)(ML)
* Performant TCP for Low-Power Wireless Networks, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-kumar.pdf) (LLNs) (NO ML)
* LAVA: fine-grained 3D indoor wireless coverage for small IoT devices, SIGCOMM	21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3452296.3472890) (NO ML)	
* STeC: Exploiting Spatial and Temporal Correlation for Event-based Communication in WSNs, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485951) （NO ML）
* COCOON-A Conductive Substrate-based Coupled Oscillator Network for Wireless Communication, SenSys 21 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/SenSys21-COCOON.pdf) (NO ML)
* A Community-Driven Approach to Democratize Access to Satellite Ground Stations, MobiCom 21 [[Paper]](https://swarunkumar.com/papers/quasar-mobicom2021.pdf) (NO ML)
* Adapting Wireless Mesh Network Configuration from Simulation to Reality via Deep Learning based Domain Adaptation, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-shi.pdf)(DL)
* A Case for Stateless Mobile Core Network Functions in Space, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3544216.3544233) (NO ML)
* Sirius: A Self-Localization System for Resource-Constrained IoT Sensors, MobiSys 23 [[Paper]](https://www.cs.umd.edu/~nakul/assets/papers/sirius_mobisys2023_nakul.pdf) (DL)
* NeuroRadar: A Neuromorphic Radar Sensor for Low-Power IoT Systems, SenSys 23 [[Paper]](http://xyzhang.ucsd.edu/papers/Kai.Zheng_SenSys23_NeuroRadar.pdf) (ML)
* Hydra: Concurrent Coordination for Fault-tolerant Networking, IPSN 23 [[Paper]](https://www.research-collection.ethz.ch/bitstream/handle/20.500.11850/602741/7/3583120.3587047.pdf) (NO ML)
* mmRipple: Communicating with mmWave Radars through Smartphone Vibration, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586956) (NO ML)
* Everything has its Bad Side and Good Side: Turning Processors to Low Overhead Radios Using Side-Channels, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586959) (NO ML)( with LoRa modulation)


<a name="user-content-batteryless"></a>
### Batteryless (101)
<a name="user-content-lora"></a>
#### LoRa (Total: 9 | No ML(9) | ML(0) | DL(0))
* LoRa Backscatter: Enabling The Vision of Ubiquitous Connectivity, UbiComp 17 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/loRaBackscatter.pdf)	(NO ML)
* PLoRa: A Passive Long-Range Data Network from Ambient LoRa Transmissions, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230567) (NO ML)
* Rethinking ON-OFF Keying Modulation for Ambient LoRa Backscatter, SenSys 20 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/aloba_2020.pdf) (NO ML)
* Simplifying Backscatter Deployment: Full-Duplex LoRa Backscatter, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-katanbaf.pdf) (NO ML)
* Simplifying Backscatter Deployment: Full-Duplex LoRa Backscatter, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-katanbaf.pdf) (NO ML)
* Long-Range Ambient LoRa Backscatter with Parallel Decoding, MobiCom 21 [[Paper]](http://tns.thss.tsinghua.edu.cn/~jiliang/publications/MOBICOM21-p2lora.pdf) (NO ML)
* Sense Me on the Ride: Accurate Mobile Sensing over a LoRa Backscatter Channel, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485933) (NO ML)
* Saiyan: Design and Implementation of a Low-power Demodulator for LoRa Backscatter Systems, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-guo.pdf) (NO ML)	
* LocRa: Enable Practical Long-Range Backscatter Localization for Low-Cost Tags, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596863) (NO ML)

<a name="user-content-millimeter-Wave-1"></a>
#### Millimeter-Wave (Total: 6 | No ML(6) | ML(0) | DL(0))
* mmTag: A Millimeter Wave Backscatter Network, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472917.pdf) (NO ML)
* MilliMirror: 3D Printed Reflecting Surface for Millimeter-Wave Coverage Expansion, MobiCom 22 [[Paper]](http://xyzhang.ucsd.edu/papers/Kun.Qian_MobiCom22_MilliMirror.pdf) (NO ML)
* OmniScatter: extreme sensitivity mmWave backscattering using commodity FMCW radar,	MobiSys 22 [[Paper]](http://mason.gmu.edu/~ychae2/Omniscatter.pdf)	(NO	ML) (Best Paper)
* LeakyScatter: A Frequency-Agile Directional Backscatter Network Above 100 GHz, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-kludze.pdf) (NO ML)
* UniScatter: a Metamaterial Backscatter Tag for Wideband Joint Communication and Radar Sensing, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592526) (NO ML)
* A Millimeter Wave Backscatter Network for Two-Way Communication and Localization, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3603269.3604873) (NO ML)

<a name="user-content-wifi-1"></a>
#### WiFi (Total: 17 | No ML(17) | ML(0) | DL(0))
* Enabling Practical Backscatter Communication for On-body Sensors, SIGCOMM 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2934872.2934901) (NO ML)
* HitchHike: Practical Backscatter Using Commodity WiFi, SenSys 16 [[Paper]](https://pengyuzhang.github.io/papers/sensys16_back_comm.pdf) (NO ML)
* Passive Wi-Fi: Bringing Low Power to Wi-Fi Transmissions, NSDI 16 [[Paper]](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-kellogg.pdf) (NO ML) (Best Paper)
* Spatial Stream Backscatter Using Commodity WiFi, MobiSys 18 [[Paper]](https://www2.cs.sfu.ca/~jcliu/Papers/mobisys18-Liu.pdf)(NO ML)
* X-Tandem: Towards Multi-hop Backscatter Communication with Commodity WiFi, MobiCom 18 [[Paper]](https://www2.cs.sfu.ca/~jcliu/Papers/MobiCom-18-X-Tandem.pdf) (NO ML)
* OFDMA-Enabled Wi-Fi Backscatter,MobiCom 19 [[Paper]](https://renjiezhao.github.io/files/OFDMA_BS_paper.pdf) (NO ML)
* WiTAG: Seamless WiFi Backscatter Communication, SIGCOMM 20 [[Paper]](https://cs.uwaterloo.ca/~brecht/papers/witag-sigcomm-2020.pdf) (NO ML)
* ScatterMIMO: Enabling Virtual MIMO with Smart Surfaces, MobiCom 20 [[Paper]](https://wcsng.ucsd.edu/files/scattermimo.pdf)(NO ML)
* VMscatter: A Versatile MIMO Backscatter, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-liu.pdf) (NO ML)
* Verification: Can WiFi Backscatter replace RFID?, MobiCom 21 [[Paper]](https://cs.uwaterloo.ca/~brecht/papers/wifi-vs-rfid-mobicom-2021.pdf) (NO ML)
* Verification and Redesign of OFDM Backscatter, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-liu-xin.pdf) (NO ML)
* SyncScatter: Enabling WiFi like synchronization and range for WiFi backscatter Communication, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-dunna.pdf) (NO ML)
* Content-agnostic backscatter from thin air, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538930) (NO ML)
* RF-Bouncer: A Programmable Dual-band Metasurface for Sub-6 Wireless Networks, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-li-xinyi.pdf) (NO ML)
* Timespan-based Backscatter Using a Single COTS Receiver, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596858) (NO ML)
* Leggiero: Analog WiFi Backscatter with Payload Transparency, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596835) (NO ML)
* Leggiero: Analog WiFi Backscatter with Payload Transparency, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596835) (NO ML)

<a name="user-content-rfid"></a>
#### 🏷️ RFID (Total: 12 | No ML(12) | ML(0) | DL(0))
* Making Sense of Mechanical Vibration Period with Sub-millisecond Accuracy Using Backscatter Signals, MobiCom 16 [[Paper]](https://www4.comp.polyu.edu.hk/~csyanglei/data/files/tagbeat-mobicom.pdf)(NO ML)
* Drone Relays for Battery-Free Networks, SIGCOMM 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3098822.3098847) (NO ML) 
* FlipTracer: Practical Parallel Decoding for Backscatter Communication, MobiCom 17 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/2017.1.pdf)	(NO ML)
* Parallel Backscatter in the Wild: When Burstiness and Randomness Play with You, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241544)(NO ML)
* Pushing the Range Limits of Commercial Passive RFIDs, NSDI 19 [[Paper]](https://www.usenix.org/system/files/nsdi19-wang-jingxian.pdf) (NO ML)
*  Retwork: Exploring Reader Network with COTS RFID Systems, ATC 20 [[Paper]](https://www.usenix.org/system/files/atc20-liu-jia_0.pdf) (NO ML)
* Fireworks: Channel Estimation of Parallel Backscattered Signals, IPSN 20 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/2020.1.pdf)(NO ML)
* Redefining passive in backscattering with commodity devices, MobiCom 20 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/xShift-Mobicom2020.pdf)(NO ML)
*  Two to Tango: Hybrid Light and Backscatter Networks for Next Billion Devices, MobiSys 20 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/811/tosubmit.pdf?sequence=1)(NO ML)
* Battery-free Wideband Spectrum Mapping using Commodity RFID Tags, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592508) (NO ML)
* Go Beyond RFID: Rethinking the Design of RFID Sensor Tags for Versatile Applications, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613284) (NO ML)
* Revisiting Cardinality Estimation in COTS RFID Systems, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613295) (NO ML)

<a name="user-content-visible-Light-1"></a>
#### 💡 Visible Light (Total: 12 | No ML(10) | ML(0) | DL(2))
* Focus: Robust Visual Codes for Everyone, MobiSys 16 [[Paper]](https://user.it.uu.se/~eding810/conferences/Mobisys16.pdf) (NO ML)
* PassiveVLC: Enabling Practical Visible Light Backscatter Communication for Battery-free IoT Applications, MobiCom 17 [[Paper]](https://ceca.pku.edu.cn/media/lw/63a22162bb427709099f765883bf243b.pdf)(NO ML)
* Charging a Smartphone Across a Room Using Lasers, UbiComp 18 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/laserpower.pdf)	(NO ML)
* LuxLink: creating a wireless link from ambient light, SenSys 19 [[Paper]](https://www.st.ewi.tudelft.nl/marco/files/luxlink_Sensys19.pdf)(NO ML)
* Turboboosting Visible Light Backscatter Communication, SIGCOMM 20 [[Paper]](https://ceca.pku.edu.cn/docs/20200826153441008514.pdf) (NO ML)
* Two to Tango: Hybrid Light and Backscatter Networks for Next Billion Devices, MobiSys 20 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/811/tosubmit.pdf?sequence=1)(NO ML)
* A Principled Design for Passive Light Communication, MobiCom 21 [[Paper]](https://www.st.ewi.tudelft.nl/marco/files/chromalux_Mobicom21.pdf) (NO ML)
* PassiveLiFi: Rethinking LiFi for Low-Power and Long Range RF Backscatter, MobiCom 21 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/1541/Mobicom_PassiveLiFi_authors_version.pdf?sequence=1) (NO ML)
* Low-Latency Visible Light Backscatter Networking with RetroMUMIMO, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568507) (NO ML)	
* Exploiting Digital Micro-Mirror Devices for Ambient Light Communication, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-xu_talia.pdf) (NO ML)
* U-star: an underwater navigation system based on passive 3D optical identification tags, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517019)(DL)
* SpectraLux: Towards Exploiting a Broader Spectrum with Passive VLC, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586966)(DL)

<a name="user-content-acoustic-1"></a>
#### 🔊 Acoustic (Total: 5 | No ML(5) | ML(0) | DL(0))
* Underwater backscatter networking, SIGCOMM 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3341302.3342091) (NO ML)
* Ultra-Wideband Underwater Backscatter via Piezoelectric Metamaterials, SIGCOMM 20 [[Paper]](https://www.mit.edu/~fadel/papers/U2B-paper.pdf) (NO ML)
* Microphone array backscatter: an application-driven design for lightweight spatial sound recording over the air, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483265) (NO ML)
* Higher-order modulation for acoustic backscatter communication in metals, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3544216.3544261) (NO ML)
* Enabling Long-Range Underwater Backscatter via Van Atta Acoustic Networks, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3603269.3604814) (NO ML)

<a name="user-content-other-batteryless-works"></a>
#### Other Batteryless Works (Total: 40 | No ML(36) | ML(3) | DL(1))
* Inter-Technology Backscatter: Towards Internet Connectivity for Implanted Devices, SIGCOMM 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2934872.2934894) (NO ML)
* Enabling Practical Backscatter Communication for On-body Sensors, SIGCOMM 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2934872.2934901) (NO ML)
* LoRea: A Backscatter Architecture that Achieves a Long Communication Range, SenSys 17 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3131672.3131691) (NO ML)
* Battery-Free Cellphone, UbiComp 17 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/phone.pdf) (NO ML)
* NICScatter: Backscatter as a Covert Channel in Mobile Devices, MobiCom 17 [[Paper]](https://www.yangzhice.com/docforweb/NICScatter/NICScatter_MobiCom.pdf) (NO ML)
* FM Backscatter: Enabling Connected Cities and Smart Fabrics, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-wang-anran.pdf) (NO ML)
* 3D Localization for Sub-Centimeter Sized Devices, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274851) (Best Paper) (NO ML)
* In-body backscatter communication and localization, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3230543.3230565) (NO ML)
* Slocalization: Sub-muW, Static, Decimeter-Accurate Localization with Ultra Wideband Backscatter, IPSN 18 [[Paper]](https://patpannuto.com/pubs/pannuto18slocalization.pdf) (NO ML)
* TunnelScatter: Low Power Communication for Sensor Tags using Tunnel Diodes, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345451) (NO ML)
* BARNET: Activity Recognition using Passive Backscattering Tag-to-Tag Network, MobiSys 18 [[Paper]](http://www.wings.cs.sunysb.edu/pdfs/2018-Jihoon-mobisys.pdf)(ML)
* Passive-ZigBee: Enabling ZigBee Communication in IoT Networks with 1000X+ Less Power Consumption, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274846) (Best paper runner-up awards)(NO ML)
* NetScatter: Enabling Large-Scale Backscatter Networks, NSDI 19 [[Paper]](https://www.usenix.org/system/files/nsdi19-hessar.pdf) (NO ML)
* Leveraging Ambient LTE Traffic for Ubiquitous Passive Communication, SIGCOMM 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3387514.3405861) (NO ML)
* TagAlong: Efficient Integration of Battery-free Sensor Tags in Standard Wireless Networks, IPSN 20 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2020-2ZapWCkbA6ELdouTqExUlt/549700a169/549700a169.pdf) (NO ML)
* DigiScatter: efficiently prototyping large-scale OFDMA backscatter networks, MobiSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3386901.3388914) (NO ML)
* Towards scalable backscatter sensor mesh with decodable relay and distributed excitation, MobiSys 20 [[Paper]](https://www2.cs.sfu.ca/~jcliu/Papers/mobisys20-final157.pdf)	(NO ML)
* Gateway over the Air: Towards Pervasive Internet Connectivity for Commodity IoT, MobiSys 20 [[Paper]](https://yung-web.github.io/home/Publication/Conference/Gateway_over_the_Air-Towards_Pervasive_Internet_Connectivity_for_Commodity_IoT.pdf) (NO ML)
* Internet-of-Microchips: Direct Radio-to-Bus Communication with SPI Backscatter, MobiCom 20 [[Paper]](https://wands.sg/publications/full_list/papers/MobiCom_20_2.pdf) (NO ML)
* Tunnel emitter: tunnel diode based low-power carrier emitters for backscatter tags, MobiCom 20 [[Paper]](https://lorenzocorneo.github.io/papers/2020-mobicom.pdf) (NO ML)
* Towards Flexible Wireless Charging for Medical Implants Using Distributed Antenna System, MobiCom 20 [[Paper]](https://arxiv.org/pdf/2001.07644.pdf) (NO ML)
* RFocus: Beamforming Using Thousands of Passive Antennas, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-arun.pdf)（ML)
* Commodity-level BLE backscatter, MobiSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3466865) (NO ML)
* Enabling Passive Backscatter Tag Localization Without Active Receivers, SenSys 21 [[Paper]](http://www.wings.cs.stonybrook.edu/pdfs/2021-sensys.pdf) (NO ML)
* MultiScatter: Multistatic Backscatter Networking for Battery-Free Sensors, SenSys 21 [[Paper]](https://par.nsf.gov/servlets/purl/10303864) (NO ML)
* Morphy: Software Defined Charge Storage for the IoT, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485947) (NO ML)
* One Tag, Two Codes: Identifying Optical Barcodes with NFC, MobiCom 21 [[Paper]](https://web.comp.polyu.edu.hk/csyanglei/data/files/coilcode-mobicom21.pdf)(NO ML)
* Pushing the Physical Limits of IoT Devices with Programmable Metasurfaces, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-chen.pdf)(NO ML)
* Judo: addressing the energy asymmetry of wireless embedded systems through tunnel diode based wireless transmitters, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538923) (NO ML)
* Enabling software-defined PHY for backscatter networks, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538927) (NO ML)(support multiple protocols)
* Passive DSSS: Empowering the Downlink Communication for Backscatter Systems, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-li_songfan.pdf) (NO ML)
* PLatter: On the Feasibility of Building-scale Power Line Backscatter, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-zhang_junbo.pdf) (NO ML)
* RF-Transformer: A Unified Backscatter Radio Hardware Abstraction, MobiCom 22 [[Paper]](https://arxiv.org/pdf/2209.15195.pdf)(NO ML)
* Magnetoelectric backscatter communication for millimeter-sized wireless biomedical implants, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560541) (NO ML) (Best Paper Award)(near zero-power backscatter)
* Eliminating Design Effort: A Reconfigurable Sensing Framework For Chipless, Backscatter Tags, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a298/962400a298.pdf)(ML)
* The Underwater Backscatter Channel: Theory, Link Budget, and Experimental Validation, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613265) (NO ML) (Best Paper Award)
* Magnetic Backscatter for In-body Communication and Localization, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613301) (NO ML)
* SmartShell: A Near-Field Reflective Surface Enhancing RSS, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596866) (NO ML)
* DeepGANTT: A Scalable Deep Learning Scheduler for Backscatter Networks, IPSN 23 [[Paper]](https://arxiv.org/pdf/2112.12985.pdf)(DL)
* RF-Bouncer: A Programmable Dual-band Metasurface for Sub-6 Wireless Networks, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-li-xinyi.pdf) (NO ML)

<a name="hybrid"></a>
### Hybrid (Total: 2 | No ML(2) | ML(0) | DL(0))
* Braidio: An Integrated Active-Passive Radio for Mobile Devices with Asymmetric Energy Budgets, SIGCOMM 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2934872.2934902) (NO ML)
* Polymorphic radios: A new design paradigm for ultra-low power communication, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230571)(NO ML) (strawman solution that connects BLE with WISP)

<a name="na"></a>
### NA (Total: 9 | No ML(6) | ML(0) | DL(3))
* Idea: A System for Efficient Failure Management in Smart IoT Environments, MobiSys 16 [[Paper]](https://pages.cs.wisc.edu/~sdsen/papers/2016idea.pdf) (NO ML)
* Mobile Plus: Multi-device Mobile Platform for Cross-device Functionality Sharing, MobiSys 17 [[Paper]](http://cps.kaist.ac.kr/papers/mobisys17-mobileplus.pdf) (NO ML)
* Enabling deep-tissue networking for miniature medical devices, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230566) (NO ML)
* Supreme: Fine-grained Radio Map Reconstruction via Spatial-Temporal Fusion Network, IPSN 20 [[Paper]](https://ieeexplore.ieee.org/document/9110971) [[code]](https://github.com/lkh329/Supreme) （DL)
* Self-Reconfgurable Micro-Implants for Cross-Tissue Wireless and Batteryless Connectivity, MobiCom 20 [[Paper]]([https://dl.acm.org/doi/abs/10.1145/3372224.3419216](https://dl.acm.org/doi/pdf/10.1145/3372224.3419216)) (NO ML)
* Network Planning with Deep Reinforcement Learning, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472902.pdf) (DL)
* In-Network Velocity Control of Industrial Robot Arms, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-laki.pdf) (NO ML) (programmable data plane)
* Industrial Knee-jerk: In-Network Simultaneous Planning and Control on a TSN Switch, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596836) (DL)
* Softly, Deftly, Scrolls Unfurl Their Splendor: Rolling Flexible Surfaces for Wideband Wireless, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592520) (NO ML)

<a name="domain-specific-aiot-systems"></a>
## Domain-specific AIoT Systems (256)
							
### 🩺 AIoT Systems for Healthcare and Well-being ()
<a name="aiot-systems-for-healthcare-and-well-being"></a>
#### Physiological Monitoring (Total:  | No ML() | ML() | DL())
* APG: Audioplethysmography for Cardiac Monitoring in Hearables, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613281) (NO ML)
* DF-Sense: Multi-user Acoustic Sensing for Heartbeat Monitoring with Dualforming, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596867) (NO ML)
* Passive Vital Sign Monitoring via Facial Vibrations Leveraging AR/VR Headsets, MobiSys 23 [[Paper]](https://dl.acm.org/doi/10.1145/3581791.3596848) (DL)
* A Low-Cost In-situ System for Continuous Multi-Person Fever Screening, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a015/962400a015.pdf) (DL)
* PROS: an Efficient Pattern-Driven Compressive Sensing Framework for Low-Power Biopotential-based Wearables with On-chip Intelligence, MobiCom 22 [[Paper]](https://theyoungkwon.github.io/papers/articles/pham_pros_mobicom22.pdf) (DL)
* Network-side digital contact tracing on a large university campus, MobiCom 22 [[Paper]](https://arxiv.org/pdf/2201.10641.pdf) (NO ML)
* Hearing Heartbeat from Voice: Towards Next Generation Voice-User Interfaces with Cardiac Sensing Function, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568508) (DL)
* mmBP: Contact-free Millimetre-wave Radar based Approach to Blood Pressure Measurement, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568506) (ML)
* Your Smart Speaker Can “Hear” Your Heartbeat!, UbiComp 21 [[Paper]](https://dl.acm.org/doi/10.1145/3432237)	(NO ML)	
* Healthy diapering with passive RFIDs for diaper wetness sensing and urine pH identification, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3466870) (ML)
* Crisp-BP: Continuous Wrist PPG-based Blood Pressure Measurement, MobiCom 21 [[Paper]](https://cis.temple.edu/~yu/research/CrispBP-Mobicom21.pdf) (DL)
* MoVi-Fi: Motion-robust Vital Signs Waveform Recovery via Deep Interpreted RF Sensing, MobiCom 21 [[Paper]](https://rabbitnick.github.io/pubs/movifi.pdf) (DL)
* U-Verse: a miniaturized platform for end-to-end closed-loop implantable internet of medical things systems, SenSys 21, [[Paper]](https://ece.northeastern.edu/wineslab/papers/GuidaSENSYS2019.pdf)	(NO ML)
* SpiroSonic: monitoring human lung function via acoustic sensing on commodity smartphones, MobiCom 20 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobicom20.pdf) (DL)
* Contactless seismocardiography via deep learning radars, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419982) (DL)
* RFWash: A Weakly Supervised Tracking of Hand Hygiene Technique, SenSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3384419.3430733) (DL)
* Noninvasive Glucose Monitoring Using Polarized Light, SenSys 20 [[Paper]](https://www.cs.columbia.edu/~xia/publication/sensys20-glucose/sensys20-glucose.pdf) (ML)
* Contactless Infant Monitoring using White Noise, MobiCom 19 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/whitenoise.pdf)	(NO ML)	
* Experience: Design, Development and Evaluation of a Wearable Device for mHealth Applications, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345432) (NO ML)
* eBP: A Wearable System For Frequent and Comfortable Blood Pressure Monitoring From User's Ear, MobiCom 19 [[Paper]](https://par.nsf.gov/servlets/purl/10303241) (Best Paper) (NO ML)
* pH Watch - Leveraging Pulse Oximeters in Existing Wearables for Reusable, Real-time Monitoring of pH in Sweat, MobiSys 19 [[Paper]](https://anantabalaji.github.io/projects/pH_watch/pH_watch.pdf) (NO ML)
* VitaMon: measuring heart rate variability using smartphone front camera, SenSys 19 [[Paper]](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=5936&context=sis_research) (DL)
* Experience: Cross-Technology Radio Respiratory Monitoring Performance Study, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241560) (NO ML)
* mCerebrum: A Mobile Sensing Software Platform for Development and Validation of Digital Biomarkers and Interventions, SenSys 17 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3131672.3131694) (ML)
* Monitoring a Person's Heart Rate and Respiratory Rate on a Shared Bed Using Geophones, SenSys 17 [[Paper]](https://www.cs.virginia.edu/~bjc8c/class/cs6501-f18/papers/jia17geophones.pdf) (NO ML)
* PhO2: Smartphone based Blood Oxygen Level Measurement Systems using Near-IR and RED Wave-guided Light, SenSys 17 [[Paper]](https://mobile.cs.gsu.edu/aashok/Papers/12_2017_SenSys.pdf) (NO ML)
* Monoxalyze: Verifying Smoking Cessation with a Keychain-sized Carbon Monoxide Breathalyzer, SenSys 16 [[Paper]](https://web.eecs.umich.edu/~prabal/pubs/papers/adkins16monoxalyze.pdf) (NO ML)
* Burnout: A Wearable System for Unobtrusive Skeletal Muscle Fatigue Estimation, IPSN 16 [[Paper]](https://www.ceid.upatras.gr/webpages/courses/adhocnets/files/papers/paper21.pdf) (ML)
* HB-Phone: a Bed-Mounted Geophone-Based Heartbeat Monitoring System, IPSN 16 [[Paper]](https://ieeexplore.ieee.org/document/7460676) (NO ML)


#### In-Situ Disease Detection and Monitoring (Total:  | No ML() | ML() | DL())
* PTEase: Objective Airway Examination for Pulmonary Telemedicine using Commodity Smartphones, MobiSys 23 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobisys23-ptease.pdf) (DL)
* PDAssess: A Privacy-preserving Free-speech based Parkinson’s Disease Daily Assessment System, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625805) (DL)
* Burnout and the Quantified Workplace: Tensions around Personal Sensing Interventions for Stress in Resident Physicians, ACM HCI 22 [[Paper]](https://dl.acm.org/doi/10.1145/3555531)
* EarHealth: an earphone-based acoustic otoscope for detection of multiple ear diseases in daily life, MobiSys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3498361.3538935) (DL)
* Out-Clinic Pulmonary Disease Evaluation via Acoustic Sensing and Multi-Task Learning on Commodity Smartphones, SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568437) (DL)
* NFCapsule: An Ingestible Sensor Pill for Eosinophilic Esophagitis Detection Based on Near-field Coupling, SenSys 22 [[Paper]](https://swarunkumar.com/papers/nfcapsule-sensys2022.pdf) (NO ML)
* Predicting Early Warning Signs of Psychotic Relapse From Passive Sensing Data: An Approach Using Encoder-Decoder Neural Networks, JMIR 20 [[Paper]](https://mhealth.jmir.org/2020/8/e19962)
* PDLens: smartphone knows drug effectiveness among Parkinson's via daily-life activity fusion,	MobiCom	20	[[Paper]](https://www.acsu.buffalo.edu/~huiningl/papers/pdlens.pdf) (DL)
* Painometry: Wearable and Objective Quantification System for Acute Postoperative Pain, MobiSys 20 [[Paper]](http://mnslab.org/tamvu/paper/2020%20Painometry_Hoang.pdf) (ML)
* PDVocal: Towards Privacy-preserving Parkinson's Disease Detection using Non-speech Body Sounds, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300125) (DL)
* HealthSense: Software-defined Mobile-based Clinical Trials, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345433) (Best Paper) (NO ML)
* Glasses for the Third Eye: Improving the Quality of Clinical Data Analysis with Motion Sensor-based Data Filtering, SenSys 17 [[Paper]](http://nsl.cau.ac.kr/~jpaek/docs/medisense-sensys2017-published.pdf) (ML)
* Mobile Phone Sensor Correlates of Depressive Symptom Severity in Daily-Life Behavior: An Exploratory Study, JMIR 15 [[Paper]](https://www.jmir.org/2015/7/e175)
* StudentLife: assessing mental health, academic performance and behavioral trends of college students using smartphones, UbiComp 14 [[Paper]](https://dl.acm.org/doi/10.1145/2632048.2632054)


#### Assistive Technology (Total:  | No ML() | ML() | DL())
* ARSteth: Enabling Home Self-Screening with AR-Assisted Intelligent Stethoscopes, IPSN 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3583120.3586962) (DL)
* AccessWear: Making Smartphone Applications Accessible to Blind Users, MobiCom 23 [[Paper]](https://www3.cs.stonybrook.edu/~jain/papers/MobiCom_AccessWear_2023.pdf) (NO ML)
* Sign-to-911: Emergency Call Service for Sign Language Users with Assistive AR Glasses, MobiCom  23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613260) (ML)
* SignQuery: A Natural User Interface and Search Engine for Sign Languages with Wearable Sensors, MobiCom 23 [[Paper]](https://www.cse.psu.edu/~mkg31/papers/signquery.pdf) (DL)
* Wireless earbuds for low-cost hearing screening, Mobisys 23 [[Paper]](https://dl.acm.org/doi/10.1145/3581791.3596856)
* An off-the-shelf otoacoustic-emission probe for hearing screening via a smartphone, Nature Biomedical Engineering 2022 [[Paper]] (https://www.nature.com/articles/s41551-022-00947-6)
* RehabPhone: A Sotware-Defined Tool using 3D Printing and Smartphones for Personalized Home-based Rehabilitation, MobiSys 20 [[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-mobisys2020a.pdf) (NO ML)
* SignSpeaker: A Real-time, High-Precision SmartWatch-based Sign Language Translator, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300117) (DL)
* MobileDeepPill: A Small-Footprint Mobile Deep Learning System for Recognizing Unconstrained Pill Images, MobiSys 17 [[Paper]](https://mi-zhang.github.io/papers/2017_MobiSys_MobileDeepPill.pdf) (DL)
* DeepASL: Enabling Ubiquitous and Non-Intrusive Word and Sentence-Level Sign Language Translation,SenSys 17 [[Paper]](https://dl.acm.org/doi/10.1145/3131672.3131693) (DL)
* iBlink: Smart Glasses for Facial Paralysis Patients, MobiSys 17 [[Paper]](https://dl.acm.org/doi/10.1145/3081333.3081343) (DL)


#### Personal Health Insight Generation (Total:  | No ML() | ML() | DL())
* Towards a Personal Health Large Language Model, Arxiv 24 [[Paper]](https://arxiv.org/abs/2406.06474)
* Transforming Wearable Data into Health Insights using Large Language Model Agents, Arxiv 24 [[Paper]](https://arxiv.org/abs/2406.06464)
* From Classification to Clinical Insights: Towards Analyzing and Reasoning About Mobile and Behavioral Health Data With Large Language Models, IMWUT 24 [[Paper]](https://dl.acm.org/doi/10.1145/3659604)



### 📺 AIoT Systems for Video Streaming ()
<a name="aiot-systems-for-video-streaming"></a>
#### Adaptive Video Streaming (Total:  | No ML() | ML() | DL())
* Swift: Adaptive Video Streaming with Layered Neural Codecs, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-dasari.pdf) (DL)
* Loki: Improving Long Tail Performance of Learning-Based Real-Time Video Adaptation by Fusing Rule-Based Models, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483259) (DL)
* SENSEI: Aligning Video Streaming Quality with Dynamic User Sensitivity, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-zhang.pdf) (DL)
* Learning in situ: a randomized experiment in video streaming, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-yan.pdf) (DL)
* OnRL: improving mobile video telephony via online reinforcement learning, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419186) (DL)
* PERCEIVE: Deep Learning-based Cellular Uplink Prediction Using Real-time Scheduling Patterns, MobiSys 20 [[Paper]](https://mail.netstech.org/wp-content/uploads/2021/07/perceive-mobisys-2020.pdf)（DL）
* Neural Adaptive Video Streaming with Pensieve, SIGCOMM 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3098822.3098843) (DL)


#### Video Enhancement (Total:  | No ML() | ML() | DL())
* OmniLive: Super-Resolution Enhanced 360° Video Live Streaming for Mobile Devices, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596851) (DL)
* YuZu: Neural-Enhanced Volumetric Video Streaming, NSDI 22 [[paper]](https://www.usenix.org/system/files/nsdi22-paper-bhardwaj.pdf) (DL)
* NeuroScaler: neural video enhancement at scale, SIGCOMM 22 [[Paper]](https://jaykim305.github.io/assets/pdf/neuroscaler-sigcomm22.pdf) (DL)
* NEMO: enabling neural-enhanced video streaming on commodity mobile devices, MobiCom 20 [[Paper]](https://hyunhoyeo.com/assets/pdf/3372224.3419185.pdf) (DL)
* Neural-Enhanced Live Streaming: Improving Live Video Ingest via Online Learning, SIGCOMM 20 [[Paper]](https://hyunhoyeo.com/assets/pdf/3387514.3405856.pdf) (DL)
* Neural Adaptive Content-aware Internet Video Delivery, OSDI 18 [[Paper]](https://www.usenix.org/system/files/osdi18-yeo.pdf) (DL)


#### Efficiency Optimization (Total:  | No ML() | ML() | DL())
* Tambur: Efficient loss recovery for videoconferencing via streaming codes, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-rudow.pdf) (DL)
* Pano: optimizing 360° video streaming with a better understanding of quality perception, SIGCOMM 19 [[Paper]](https://people.cs.uchicago.edu/~junchenj/docs/360StreamingQuality_SIGCOMM.pdf) (DL)
* Popularity Prediction of Facebook Videos for Higher Quality Streaming, ATC 17 [[Paper]](https://www.usenix.org/system/files/conference/atc17/atc17-tang.pdf) (DL)

#### 
* MetaStream: Live Volumetric Content Capture, Creation, Delivery, and Rendering in Real Time, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3592530) (DL)
* FarfetchFusion: Towards Fully Mobile Live 3D Telepresence Platform, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3592525) (DL)
* Dragonfly: Higher Perceptual Quality For Continuous 360° Video Playback, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3603269.3604876) (NO ML)
* Converge: QoE-driven Multipath Video Conferencing over WebRTC, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3603269.3604822) (NO ML)
* CellFusion: Multipath Vehicle-to-Cloud Video Streaming with Network Coding in the Wild, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/10.1145/3603269.3604832) (NO ML)
* XRON: A Hybrid Elastic Cloud Overlay Network for Video Conferencing at Planetary Scale, SIGCOMM 23 [[Paper]](https://ennanzhai.github.io/pub/xron-sigcomm23.pdf) (NO ML)
* Sammy: smoothing video traffic to be a friendly internet neighbor, SIGCOMM 23 [[Paper]](https://brucespang.com/papers/sammy.pdf) (NO ML)
* Veritas: Answering Causal Queries from Video Streaming Traces, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3603269.3604828) (ML)
* ZGaming: Zero-Latency 3D Cloud Gaming by Image Prediction, SICGOMM 23 [[Paper]](https://dl.acm.org/doi/10.1145/3603269.3604819) (DL)
* Dashlet: Taming Swipe Uncertainty for Robust Short Video Streaming, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-li-zhuqi.pdf) (NO ML)
* Enabling High Quality Real-Time Communications with Adaptive Frame-Rate, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-meng.pdf) (NO ML)
* GSO-Simulcast: Global Stream Orchestration in Simulcast Video Conferencing Systems, SIGCOMM 22 [[Paper]](https://yfmascgy.github.io/papers/gso-simulcast.pdf) (NO ML)
* LiveNet: a low-latency video transport network for large-scale live streaming, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3544216.3544236) (NO ML)
* Vues: Practical Mobile Volumetric Video Streaming Through Multiview Transcoding, MobiCom22 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/vues_mobicom22.pdf) (ML)
* Warehouse-Scale Video Acceleration: Co-design and Deployment in the Wild, ASPLOS 21 [[Paper]](https://gwern.net/doc/cs/hardware/2021-ranganathan.pdf) (NO ML)
* XLINK: QoE-Driven Multi-Path QUIC Transport in Large-scale Video Services, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472893.pdf) (NO ML)
* Proactive Energy-Aware Adaptive Video Streaming on Mobile Devices, ATC 21 [[Paper]](https://www.usenix.org/system/files/atc21-meng.pdf) (NO ML)
* GROOT: a real-time streaming system of high-fidelity volumetric videos, MobiCom 20 [[Paper]](https://juheonyi.github.io/files/GROOT.pdf) (NO ML)
* ViVo: visibility-aware mobile volumetric video streaming, MobiCom 20 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/vivo_mobicom20.pdf) (ML)
* Server-Driven Video Streaming for Deep Learning Inference, SIGCOMM 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3387514.3405887) (DL)
* Jigsaw: Robust Live 4K Video Streaming, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300127) (NO ML)
* Learning to Coordinate Video Codec with Transport Protocol for Mobile Video Telephony, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345430) (DL)
* Banner: An Image Sensor Reconfiguration Framework for Seamless Resolution-based Tradeoffs, MobiSys 19 [Paper] (NO ML)
* End-to-end transport for video QoE fairness, SIGCOMM 19 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3341302.3342077) (NO ML)
* Vantage: optimizing video upload for time-shifted viewing of social live streams, SIGCOMM 19 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3341302.3342064) (NO ML)
* VideoChef: Efficient Approximation for Streaming Video Processing Pipelines, ATC 18 [[Paper]](https://www.usenix.org/system/files/conference/atc18/atc18-xu-ran.pdf) (ML)
* Flare: Practical Viewport-Adaptive 360-Degree Video Streaming for Mobile Devices, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241565) (ML)
* Salsify: Low-Latency Network Video Through Tighter Integration Between a Video Codec and a Transport Protocol, NSDI 18 [[Paper]](https://www.usenix.org/system/files/conference/nsdi18/nsdi18-fouladi.pdf) (NO ML)
* Towards Battery-Free HD Video Streaming, NSDI 18 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/videobackscatter.pdf) (NO ML)
* Oboe: Auto-tuning Video ABR Algorithms to Network Conditions, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230558) (NO ML)
* Rubiks: Practical 360-Degree Streaming for Smartphones, MobiSys 18 [[Paper]](https://dl.acm.org/doi/10.1145/3210240.3210323) (ML)
* Encoding, Fast and Slow: Low-Latency Video Processing Using Thousands of Tiny Threads, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-fouladi.pdf) (NO ML)
* SVE: Distributed Video Processing at Facebook Scale, SOSP 17 [[Paper]](https://www.cs.princeton.edu/~wlloyd/papers/sve-sosp17.pdf) (NO ML)
* Disk|Crypt|Net: rethinking the stack for high-performance video streaming, SIGCOMM 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3098822.3098844) (NO ML)
* CFA: A Practical Prediction System for Video QoE Optimization, NSDI 16 [[Paper]](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-jiang-junchen.pdf) (ML)
* RnB: Rate and Brightness Adaptation for Rate-Distortion-Energy Tradeoff in HTTP Adaptive Streaming over Mobile Devices, MobiCom 16 [[Paper]](https://mason.gmu.edu/~zyan4/papers/rnb_mobicom16.pdf) (ML)


### 🎦 AIoT Systems for Video Analytics	()
<a name="aiot-systems-for-video-analytics"></a>
#### Continuous Learning (Total:  | No ML() | ML() | DL())
* RECL: Responsive Resource-Efficient Continuous Learning for Video Analytics, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-khani.pdf) (DL)
* Ekya: Continuous Learning of Video Analytics Models on Edge Compute Servers, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-bhardwaj.pdf) (DL)

#### Adaptation (Total:  | No ML() | ML() | DL())
* Enhancing Video Analytics Accuracy via Real-time Automated Camera Parameter Tuning, SenSys 22 [[Paper]](https://arxiv.org/pdf/2107.03964.pdf) (DL)
* Chameleon: scalable adaptation of video analytics, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230574) (DL)
* AWStream: Adaptive Wide-Area Streaming Analytics, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230554) (DL)

#### Efficiency Optimization (Total:  | No ML() | ML() | DL())
* Gemel: Model Merging for Memory-Efficient, Real-Time Video Analytics at the Edge, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-padmanabhan.pdf) [[code]](https://github.com/artpad6/gemel_nsdi23) (DL)
* CoVA: Exploiting Compressed-Domain Analysis to Accelerate Video Analytics, ATC 22 [[Paper]](https://www.usenix.org/system/files/atc22-hwang.pdf) (DL)
* AccMPEG: Optimizing Video Encoding for Video Analytics, MLSys 22 [[Paper]](https://arxiv.org/pdf/2204.12534.pdf) (DL)
* Reducto: On-Camera Filtering for Resource-Efficient Real-Time Video Analytics, SIGCOMM 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3387514.3405874) (DL)
* Scaling Video Analytics on Constrained Edge Nodes, MLSys 19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/197.pdf) (DL)

#### Resource Management (Total:  | No ML() | ML() | DL())
* PacketGame: Multi-Stream Packet Gating for Concurrent Video Inference at Scale, SIGCOMM 23 [[Paper]](https://yuanmu97.github.io/preprint/packetgame_sigcomm23.pdf) (DL)
* Turbo: Opportunistic Enhancement for Edge Video Analytics, SenSys 22 [[Paper]](https://arxiv.org/pdf/2207.00172.pdf) (DL)
* Distream: Scaling Live Video Analytics with Workload-Adaptive Distributed Edge Intelligence, SenSys 20 [[Paper]](https://www.egr.msu.edu/~mizhang/papers/2020_SenSys_Distream.pdf) (DL)
* Caesar: cross-camera complex activity recognition, SenSys 19 [[Paper]](http://web.cs.ucla.edu/~ravi/CS239_W20/papers/caesar.pdf) (DL)
* Panoptes: Servicing Multiple Applications Simultaneously using Steerable Cameras, IPSN 17 [[Paper]](https://winlab.rutgers.edu/~shubhamj/papers/Shubham_Panoptes_IPSN2017.pdf) (NO ML)


#### Queries Optimization (Total:  | No ML() | ML() | DL())
* Boggart: Towards General-Purpose Acceleration of Retrospective Video Analytics, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-agarwal-neil.pdf) (DL)
* Privid: Practical, Privacy-Preserving Video Analytics Queries, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-cangialosi.pdf) (DL)
* Tutti: coupling 5G RAN and mobile edge computing for latency-critical video analytics, MobiCom 22 [[Paper]](https://dl.acm.org/doi/10.1145/3495243.3560538) (DL)
* Video Analytics with Zero-streaming Cameras, ATC 21 [[Paper]](https://xumengwei.github.io/files/ATC-DIVA.pdf) (DL)
* Approximate query service on autonomous IoT cameras,	MobiSys	20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388948) (DL)


### 🚘 AIoT Systems for Autonomous Driving ()
<a name="aiot-systems-for-autonomous-driving"></a>
#### Perception Enhancement (Total:  | No ML() | ML() | DL())
* AutoMatch: Leveraging Traffic Camera to Improve Perception and Localization of Autonomous Vehicles, SenSys 22 [[Paper]](https://yanzhenyu.com/assets/pdf/AutoMatch-SenSys22.pdf) (DL)
* VIPS: Real-Time Perception Fusion for Infrastructure-Assisted Autonomous Driving, MobiCom 22 [[Paper]](https://yanzhenyu.com/assets/pdf/VIPS-MobiCom22.pdf) (Best Paper Award Runner-ups) (DL)
* EMP: Edge-assisted Multi-vehicle Perception, MobiCom 21 [[Paper]](https://xiaoshawnzhu.github.io/emp-mobicom21.pdf) (DL)
* VI-Eye: Semantic-based 3D Point Cloud Registration for Infrastructure-assisted Autonomous Driving, MobiCom 20 [[Paper]](https://aiot.ie.cuhk.edu.hk/papers/VI_Eye.pdf) (DL)
* Pointillism: Accurate 3D Bounding Box Estimation with Multi-Radars, SenSys 20 [[Paper]](https://wcsng.ucsd.edu/files/Pointillism_paper.pdf) [[code]](https://github.com/Kshitizbansal/pointillism-multi-radar-data) (DL)


#### Localization, Tracking, and Mapping (Total:  | No ML() | ML() | DL())
* MVP: magnetic vehicular positioning system for GNSS-denied environments, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483264) (DL)
* Large-Scale Vehicle Trajectory Reconstruction with Camera Sensing Network, MobiCom 21 [[Paper]](https://wands.sg/publications/full_list/papers/MobiCom_21_1.pdf) (DL)
* CarMap: Fast 3D Feature Map Updates for Automobiles, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-ahmad.pdf) (DL)
* The Architectural Implications of Autonomous Driving: Constraints and Acceleration, ASPLOS 18 [[Paper]](https://people.computing.clemson.edu/~jmarty/projects/lowLatencyNetworking/papers/EmergingApplicationSystems/AutonomousVehicles/AutonomousCarConstraints.pdf) (DL)


#### Automatic Testing (Total:  | No ML() | ML() | DL())
* Automatic Unusual Driving Event Identification for Dependable Self-Driving, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274838) (DL)
* BigRoad: Scaling Road Data Acquisition for Dependable Self-Driving, MobiSys 17 [[Paper]](https://personal.stevens.edu/~ychen6/papers/mobisys17-BigRoad.pdf) (DL)

#### Control and Actuation (Total:  | No ML() | ML() | DL())
* Eagle: End-to-end Deep Reinforcement Learning based Autonomous Control of PTZ Cameras, IoTDI 23 [[Paper]](https://dl.acm.org/doi/10.1145/3576842.3582366)

#### 
* Ghost-Probe: NLOS Pedestrian Rushing Detection with Monocular Camera for Automated Driving, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625791) (DL)
* mmSV: mmWave Vehicular Networking using Street View Imagery in Urban Environments, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613291) (DL)
* VI-Map: Infrastructure-Assisted Real-Time HD Mapping for Autonomous Driving, MobiCom 23 [[Paper]](https://yanzhenyu.com/assets/pdf/VI-Map-MobiCom23.pdf) (DL)
* Robust Real-time Multi-vehicle Collaboration on Asynchronous Sensors, MobiCom 23 [[Paper]](https://ry4nzhu.github.io/publication/robust_real_time/robust_real_time.pdf) (DL)
* AutoFed: Heterogeneity-Aware Federated Multimodal Learning for Robust Autonomous Driving, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592517) (DL) (also federated learning)
* Mosaic: leveraging diverse reflector geometries for omnidirectional around-corner automotive radar, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538944) (NO ML)
* AutoCast: scalable infrastructure-less cooperative perception for distributed collaborative driving, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538925) (NO ML)
* Demystifying Millimeter-Wave V2X: Towards Robust and Efficient Directional Connectivity Under High Mobility, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419208) (NO ML)
* Renovating road signs for infrastructure-to-vehicle networking: a visible light backscatter communication and networking approach, MobiCom 20 [[Paper]](https://soar.group/pubs/RetroI2V.MobiCom20.pdf) (NO ML)
* Wi-Go: Accurate and Scalable Vehicle Positioning using WiFi Fine Timing Measurement, MobiSys 20 [[Paper]](https://www.andrew.cmu.edu/user/miahmed/papers/wi-go_mobisys.pdf) (NO ML)
* SmartDashCam: Automatic Live Calibration for DashCams, IPSN 19 [[Paper]](http://web.cse.ohio-state.edu/~sinha.43/publications/conf/ipsn19-smartdashcam.pdf) (NO ML)
* VeMo: Enabling Transparent Vehicular Mobility Modeling at Individual Levels with Full Penetration, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300130) (ML)
* Diagnosing Vehicles with Automotive Batteries, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300126) (ML)
* Experience: Understanding Long-Term Evolving Patterns of Shared Electric Vehicle Networks, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300132) (NO ML)
* RAVEN: Improving Interactive Latency for the Connected Car, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241571) (NO ML)
* CoReCast: Collision Resilient Broadcasting in Vehicular Networks, MobiSys 18 [[Paper]](http://web.cse.ohio-state.edu/~sinha.43/publications/conf/mobisys17-corecast.pdf) (NO ML)
* AVR: Augmented Vehicular Reality, MobiSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3210240.3210319) (Best Paper Runner-Up) (NO ML)
* Sentio: Driver-in-the-Loop Forward Collision Warning Using Multisample Reinforcement Learning, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274843) (ML)
* EXIMIUS: A Measurement Framework for Explicit and Implicit Urban Traffic Sensing, SenSys 18 [[Paper]](https://people.cs.rutgers.edu/~dz220/paper/Eximius.pdf) (NO ML)
* Object Recognition and Navigation using a Single Networking Device, MobiSys 17 [[Paper]](https://people.cs.uchicago.edu/~ravenben/publications/pdf/60gradar-mobisys17.pdf) (NO ML)
* Experience: Accurate Simulation of Dense Scenarios with Hundreds of Vehicular Transmitters, MobiCom 16 [[Paper]](https://www.winlab.rutgers.edu/~cb3974/publication_pdf/Experience_Simulation_MobiCom_2016.pdf)(NO ML)
* Experience: Understanding Long-Term Evolving Patterns of Shared Electric Vehicle Networks, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300132) (NO ML)
* uGPS: Design and Field-Tested Seamless GNSS Infrastructure in Metro City, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560520) (NO ML)
* RoS: Passive Smart Surface for Roadside-to-Vehicle Communication, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472896.pdf) (NO ML)

### 🥽 AIoT Systems for AR/VR/MR (Total:  | No ML() | ML() | DL())
<a name="aiot-systems-for-arvrmr"></a>
#### Object Detection (Total:  | No ML() | ML() | DL())
* DeepMix: mobility-aware, lightweight, and hybrid 3D object detection for headsets, MobiSys 22 [[Paper]](https://arxiv.org/pdf/2201.08812.pdf) (DL)
* Edge Assisted Real-time Object Detection for Mobile Augmented Reality, MobiCom 19 [[Paper]](https://dl.acm.org/doi/10.1145/3300061.3300116) (DL)
* Frugal following: power thrifty object detection and tracking for mobile augmented reality, SenSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3356250.3360044) (DL)

#### Gesture-Based Interaction (Total:  | No ML() | ML() | DL())
* ExGSense: Toward Facial Gesture Sensing and Reconstruction with a Sparse Near-Eye Sensor Array, IPSN 21 [[Paper]](http://xyzhang.ucsd.edu/papers/Chen.Chen_IPSN21_ExGSense.pdf) (DL)
* HandSense: capacitive coupling-based dynamic, micro finger gesture recognition, SenSys 19 [[Paper]](https://www.winlab.rutgers.edu/~gruteser/papers/sensys19-final195.pdf) (DL)


#### Performance Enhancement (Total:  | No ML() | ML() | DL())
* Breaking edge shackles: Infrastructure-free collaborative mobile augmented reality, SenSys 22 [[Paper]](https://www.cs.ucr.edu/~jiasi/pub/freeAR-sensys22.pdf) (DL)
* CollabAR: Edge-assisted Collaborative Image Recognition for Mobile Augmented Reality, IPSN 20 [[Paper]](https://research.ece.cmu.edu/lions/Papers/CollabAR_IPSN.pdf) (DL)
* Heimdall: mobile GPU coordination platform for augmented reality applications, MobiCom 20 [[Paper]](https://juheonyi.github.io/files/Heimdall.pdf) (DL)
* Transparent AR Processing Acceleration at the Edge, EuroSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3301418.3313942) (DL)


#### Omnidirectional AR (Total:  | No ML() | ML() | DL())
* SalientVR: Saliency-Driven Mobile 360-Degree Video Streaming with Gaze Information, MobiCom 22 [[Papaer]](https://www-users.cse.umn.edu/~fengqian/paper/salientvr_mobicom22.pdf) (DL)
* Xihe: a 3D vision-based lighting estimation framework for mobile augmented reality, MobiSys 21 [[Paper]](https://arxiv.org/pdf/2106.15280.pdf) (DL)

####
* Egocentric Human Pose Estimation using Head-mounted mmWave Radar, SenSys 23 [[Paper]](https://dl.acm.org/doi/10.1145/3625687.3625799) (DL)
* XRLoc: Accurate UWB Localization to Realize XR Deployments, SenSys 23 [[Paper]](https://arxiv.org/pdf/2307.12512) (NO ML)
* UbiPose: Towards Ubiquitous Outdoor AR Pose Tracking using Aerial Meshes, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613263) (DL)
* Augmenting Augmented Reality with Non-Line-of-Sight Perception, NSDI	23 [[Paper]](https://www.usenix.org/conference/nsdi23/presentation/boroushaki) (NO ML)
* Cyclops: an FSO-based wireless link for VR headsets, SIGCOMM 22 [[Paper]](http://www.contrib.andrew.cmu.edu/~malleshd/papers/sigcomm-2022-paper.pdf) (NO ML)
* Multi-User Augmented Reality with Infrastructure-free Collaborative Localization, IPSN 22 [[Paper]](https://arxiv.org/pdf/2111.00174.pdf) (NO ML)
* Q-VR: System-Level Design for Future Collaborative Virtual Reality Rendering, ASPLOS 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3445814.3446715) (ML)
* FollowUpAR: enabling follow-up effects in mobile AR applications, MobiSys 21 [[Paper]](http://tns.thss.tsinghua.edu.cn/~jingao/papers/mobisys21_followupar.pdf) (NO ML)
* All that GLITTERs: Low-Power Spoof-Resilient Light Anchors for Augmented Reality, IPSN 20 [[Paper]](https://users.ece.cmu.edu/~vsekar/assets/pdf/ipsn20_glitter.pdf) (NO ML)
* Coterie: Exploiting Frame Similarity to Enable High-Quality Multiplayer VR on Commodity Mobile Devices, ASPLOS 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3373376.3378516) (NO ML)
* Firefly: Untethered Multi-user VR for Commodity Mobile Devices, ATC 20 [[Paper]](https://www.usenix.org/system/files/atc20-liu-xing.pdf) (ML)
* DeltaVR: Achieving High-Performance Mobile VR Dynamics through Pixel Reuse, IPSN 19 [[Paper]](https://sites.pitt.edu/~weigao/publications/ipsn19.pdf) (NO ML)
* GLEAM: An Illumination Estimation Framework for Real-time Photorealistic Augmented Reality on Mobile Devices, MobiSys 19 [[Paper]](https://meteor.ame.asu.edu/publications/mobisys19prakash-gleam.pdf) (NO ML)
* Aura: Inside-out Electromagnetic Controller Tracking MobiSys 19 [[Paper]](https://dl.acm.org/doi/10.1145/3307334.3326090) (ML)
* When IoT met Augmented Reality: Visualizing the Source of the Wireless Signal in AR View, MobiSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326079) (NO ML)
* Freedom: Fast Recovery Enhanced VR Delivery Over Mobile Networks, MobiSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326087) (NO ML)
* LpGL: Low-power Graphics Library for Mobile AR Headsets, MobiSys 19, [[Paper]](http://nsl.cau.ac.kr/~jpaek/docs/lpgl-mobisys2019.pdf) (NO ML)
* Cutting the Cord: Designing a High-quality Untethered VR System with Low Latency Remote Rendering, MobiSys 18 [[Paper]](https://www.winlab.rutgers.edu/~gruteser/papers/mobisys18_low_latency_vr.pdf) (NO ML)
* Conductive Inkjet Printed Passive 2D TrackPad for VR Interaction, MobiCom 18 [[Paper]](http://xyzhang.ucsd.edu/papers/CGao_MobiCom18_Inkput.pdf) (NO ML)
* Empath-D: VR-based Empathetic App Design for Accessibility, MobiSys 18 [[Paper]](https://nclab.kaist.ac.kr/files/papers/Conference/mobisys18-10-kim.pdf) (NO ML)
* Depth Aware Finger Tapping on Virtual Display, MobiSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3210240.3210315) (NO ML)
* MARVEL: Enabling Mobile Augmented Reality with Low Energy and Low Latency, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274834) (NO ML)
* When Virtual Reality Meets Internet of Things in the Gym: Enabling Immersive Interactive Machine Exercises, UbiComp 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3214281) (ML)
* Furion: Engineering High-Quality Immersive Virtual Reality on Today’s Mobile Devices, MobiCom 17 [[Paper]](https://www.cse.psu.edu/~gxc27/teach/597/Furion.pdf) (NO ML)
* Enabling High-Quality Untethered Virtual Reality, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-abari.pdf) (NO ML)
* Ultra-Low Power Gaze Tracking for Virtual Reality, SenSys 17 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3131672.3131682) (ML)
* FlashBack: Immersive Virtual Reality on Mobile Devices via Rendering Memoization, MobiSys 16 [[Paper]](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/06/flashback_mobisys2016.pdf) (NO ML)

### AIoT Systems for Drones (Total: 25 | No ML(21) | ML(1) | DL(3))
<a name="aiot-systems-for-drones"></a>
* Anemoi: A Low-cost Sensorless Indoor Drone System for Automatic Mapping of 3D Airflow Fields,MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613292) (NO ML)
* BatMobility: Towards Flying Without Seeing for Autonomous Drones, MobiCom 23 [[Paper]](https://arxiv.org/pdf/2307.11518.pdf) (DL)
* RF-Search: Searching Unconscious Victim in Smoke Scenes with RF-enabled Drone, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613305) (NO ML)
* MilliSign: mmWave-Based Passive Signs for Guiding UAVs in Poor Visibility Conditions, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613264) (NO ML)
* Taming Event Cameras with Bio-Inspired Architecture and Algorithm: A Case for Drone Obstacle Avoidance, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613269) (NO ML)
* Placement Optimization for UAV-Enabled Wireless Networks with Multi-Hop Backhauls in Urban Environments, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a054/962400a054.pdf) (NO ML)
* Wi-Drone: Wi-Fi-based 6-DoF Tracking for Indoor Drone Flight Control, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538936) (NO ML)
* Reverse Engineering and Retrofitting Robotic Aerial Vehicle Control Firmware using DisPatch, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538938) (NO ML)
* AIM: Acoustic Inertial Measurement for Indoor Drone Localization and Tracking, SenSys 22 [[Paper]](https://mottola.faculty.polimi.it/papers/sun22aim.pdf) (NO ML)
* MicNest: Long-Range Instant Acoustic Localization of Drones in Precise Landing, SenSys 22 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/2022.MicNest.pdf) (Best Paper Runner-up Award) (NO ML)
* Throughput-Fairness Tradeoffs in Mobility Platforms, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3467881) (NO ML)
* Quantifying the Design-Space Tradeoffs in Autonomous Drones, ASPLOS 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3445814.3446721) (NO ML)
* Visage: Enabling Timely Analytics for Drone Imagery, MobiCom 21 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2021/09/Visage_Mobicom_2021.pdf) (DL)
* Bleep: motor-enabled audio side-channel for constrained UAVs, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419183) (NO ML)
* C-14: Assured Timestamps for Drone Videos, MobiCom 20 [[Paper]](https://people.cs.umass.edu/~elm/papers/mobicom20-final809.pdf) (DL)
* BeeCluster: Drone Orchestration via Predictive Optimization, MobiSys 20 [[Paper]](http://people.csail.mit.edu/songtao/BeeCluster.pdf) (NO ML)
* DroneScale: Drone Load Estimation via Remote Passive RF Sensing, SenSys 20 [[Paper]](http://mnslab.org/tamvu/paper/2020%20DroneScale_Phuc.pdf) (ML)
* FlyZone: A Testbed for Experimenting with Aerial Drone Application, MobiSys 19 [[Paper]](https://mottola.faculty.polimi.it/papers/afanasov19flyzone.pdf) (NO ML)
* TrackIO: Tracking First Responders Inside-Out, NSDI 19 [[Paper]](https://www.usenix.org/system/files/nsdi19-dhekne.pdf) (NO ML)
* SkyCore: Moving Core to the Edge for Untethered and Reliable UAV-based LTE Networks, MobiCom 18 [[Paper]](https://dl.acm.org/doi/10.1145/3241539.3241549) (Best Paper Award) (NO ML)
* Tracking Drone Orientation with Multiple GPS Receivers, MobiCom 16 [[Paper]](https://synrg.csl.illinois.edu/papers/drone-attitude-camera.pdf) (NO ML)
* Matthan: Drone Presence Detection by Identifying Physical Signatures in the Drone’s RF Communication, MobiSys 17 [[Paper]](http://mnslab.org/tamvu/paper/2017_Mobisys_Drone.pdf) (NO ML)
* Indoor Follow Me Drone, MobiSys 17 [[Paper]](https://dl.acm.org/doi/10.1145/3081333.3081362) (Honorable Mention) (NO ML)
* Argus: Realistic Target Coverage by Drones, IPSN 17 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3055031.3055078) (NO ML)
* Reactive Control of Autonomous Drones, MobiSys 16 [[Paper]](https://dl.acm.org/doi/10.1145/2906388.2906410) (NO ML) (Best Paper) 

### 🛰️ AIoT Systems for Satellites (Total: 7 | No ML(6) | ML(0) | DL(1))
<a name="aiot-systems-for-satellites"></a>
* Global Localization of Energy-Constrained Miniature RF Emitters using Low Earth Orbit Satellites, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625794) (NO ML)
* A Networking Perspective on Starlink’s Self-Driving LEO Mega-Constellation, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592519) (NO ML)
* Transmitting, Fast and Slow: Scheduling Satellite Traffic through Space and Time, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3592521) (NO ML)
* PMSat: Optimizing Passive Metasurface for Low Earth Orbit Satellite Communication, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613257) (NO ML)
* GPSMirror: Expanding Accurate GPS Positioning to Shadowed and Indoor Regions with Backscatter, MobiCom 23 [[Paper]](https://arxiv.org/pdf/2304.07572.pdf) (NO ML)
* SelfieStick: Towards Earth Imaging from a Low-Cost Ground Module Using LEO Satellites, IPSN 22 [[Paper]](https://swarunkumar.com/papers/selfiestick-ipsn2022.pdf) (DL)
* SOS: Isolated Health Monitoring System to Save Our Satellites, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3466862) (NO ML)

### 🌾 AIoT Systems for Agriculture (Total: 12 | No ML(9) | ML(2) | DL(1))
<a name="aiot-systems-for-agriculture"></a>
* Meta-Sticker: Sub-Terahertz Metamaterial Stickers for Non-Invasive Mobile Food Sensing, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625815) (NO ML)
* AgriTera: Accurate Non-Invasive Fruit Ripeness Sensing via Sub-Terahertz Wireless Signals, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613275) (ML) (Best Paper Award)
* eTag: An Energy-Neutral Ear Tag for Real-Time Body Temperature Monitoring of Dairy Cattle, MobiCom 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3570361.3613262) (NO ML)
* DRLIC: Deep Reinforcement Learning for Irrigation Control, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a041/962400a041.pdf) (DL)
* IoTree: a battery-free wearable system with biocompatible sensors for continuous tree health monitoring, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3567652) (NO ML)
* Estimating Soil Moisture using RF Signals, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3517025) (NO ML) 
* LTE-Based Low-Cost and Low-Power Soil Moisture Sensing, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568525) (NO ML)
* Soil Moisture Sensing with Commodity RFID Systems, MobiSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3386901.3388940) (NO ML)
* Towards Low Cost Soil Sensing Using Wi-Fi, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345440) (NO ML) (Honorable Mention)
* WISDOM: watering intelligently at scale with distributed optimization and modeling, SenSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3356250.3360023) (NO ML)
* FarmBeats: An IoT Platform for Data-Driven Agriculture, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-vasisht.pdf) (ML)
* MAGIC: Model-Based Actuation for Ground Irrigation Control, IPSN 16 [[Paper]](https://faculty.ucmerced.edu/mcarreira-perpinan/papers/ipsn16.pdf) (NO ML)

### 🧬 AIoT Systems for Biology (Total: 8 | No ML(5) | ML(2) | DL(1))
<a name="aiot-systems-for-biology"></a>
* Towards Practical and Scalable Molecular Networks, SIGCOMM 23 [[Paper]](https://uwconnect.ece.wisc.edu/wp-content/uploads/sites/1525/2023/08/Towards-Practical-and-Scalable-Molecular-Networks.pdf) (ML)
* Wind dispersal of battery-free wireless devices, Nature 2022 [[Paper]](https://www.nature.com/articles/s41586-021-04363-9) (No ML)
* Vildehaye: A Family of Versatile, Widely-Applicable, and Field-Proven Lightweight Wildlife Tracking and Sensing Tags, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a001/962400a001.pdf) (No ML)
* mSAIL: milligram-scale multi-modal sensor platform for monarch butterfly migration tracking,	MobiCom	21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483263) (DL)	
* PigNet: Failure-Tolerant Pig Activity Monitoring System Using Structural Vibration, IPSN 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3412382.3458902) (ML)
* Airdropping Sensor Networks from Drones and Insects, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419981) (No ML)
* Estimating Heart Rate and Detecting Feeding Events of Fish Using an Implantable Biologger, IPSN 20 [[Paper]](https://research.csiro.au/dss/wp-content/uploads/sites/100/2020/02/Estimating_Heart_Rate_and_Detecting_Feeding_Events_of_Fish_Using_an_Implantable_Biologger-1.pdf) (No ML)
* Living IoT: A Flying Wireless Platform on Live Insects, MobiCom 19 [[Paper]](https://livingiot.cs.washington.edu/files/livingiot.pdf) (No ML)


