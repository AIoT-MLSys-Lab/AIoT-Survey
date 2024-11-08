# Artificial Intelligence of Things: A Survey 

> **[Artificial Intelligence of Things: A Survey](https://mi-zhang.github.io/papers/2024_ACMTOSN_AIoTSurvey.pdf)**

> *Shakhrul Iman Siam<sup>1</sup>, Hyunho Ahn<sup>1</sup>, Li Liu<sup>2</sup>, Samiul Alam<sup>1</sup>, Hui Shen<sup>1</sup>, Zhichao Cao<sup>2</sup>, Ness Shroff<sup>1</sup>, Bhaskar Krishnamachari<sup>3</sup>, Mani Srivastava<sup>4</sup>, Mi Zhang<sup>1</sup>*

> <sup>1</sup>The Ohio State University, <sup>2</sup>Michigan State University, <sup>3</sup>University of Southern California, <sup>4</sup>University of California, Los Angeles
### ⚡News: Our survey has been officially accepted by ACM Transactions on Sensor Networks (TOSN), August 2024. [[ACM Digital Library Link](https://dl.acm.org/doi/10.1145/3690639)]
```
@article{aiotsurvey2024tosn,
  title={Artificial Intelligence of Things: A Survey},
  author={Siam, Shakhrul Iman and Ahn, Hyunho and Liu, Li and Alam, Samiul and Shen, Hui and Cao, Zhichao and Shroff, Ness and Krishnamachari, Bhaskar and Srivastava, Mani and Zhang, Mi},
  journal={ACM Transactions on Sensor Networks (TOSN)},
  year={2024}
}
```
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
  - 🌡️ [Sensing (Total: 320)](#sensing)
    - [Motion Sensing](#motion-sensing)
    - [Wireless Sensing](#wireless-sensing)
    	- [RFID Sensing](#rfid-sensing)
    	- [Wi-Fi Sensing](#wi-fi-sensing)
    	- [mmWave Sensing](#mmwave-sensing)
       	- [LTE Sensing](#lte-sensing)
       	- [LoRa Sensing](#lora-sensing)
       	- [TeraHertz Sensing](#teraHertz-sensing)
    	- [UWB Sensing](#uwb-sensing)
    	- [Bluetooth Sensing](#bluetooth-sensing)
      	- [NFC Sensing](#nfc-sensing)
      	- [Others](#rf-sensing)
    - [Vision Sensing](#vision-sensing)
    - [Acoustic Sensing](#acoustic-sensing)
    - [Multi-Modal Sensing](#multi-modal-sensing)
    - [Earable Sensing](#earable-sensing)
    - [Visible Light Sensing](#light-sensing)
    - [Magentic Sensing](#magnetic-sensing)
    - [Cross-Medium Sensing](#cross-medium-sensing)
    - [Generative AI for Sensing](#generative-ai-for-sensing)
  - 📲 [Computing (Total: 168)](#computing)
    - [On-Device Inference](#on-device-inference)
      	- [Inference Optimization](#inference-optimization)
      	- [Multi-Tenant Inference](#multi-tenant-inference)
      	- [Cross-Processor Inference](#cross-processor-inference)
      	- [Runtime Adaptation](#runtime-adaptation)
      	- [Model Compression](#model-compression)
      	- [Privacy-Preserving Inference](#privacy-preserving)
      	- [Benchmarks](#benchmarks)
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
    - [AI Agents for AIoT](#ai-agent-aiot)
    - [Automated Machine Learning](#auto-ML)
    - [Compilers for AIoT](#compilers-for-aiot)
  - 📶 [Networking and Communication (Total: 324)](#networking-and-communication)
    - [Battery-powered Networking and Communication](#user-content-battery)
      - [Cellular/Mobile Networks](#user-content-cellular)
      - [Wi-Fi Networks](#user-content-wifi)
      - [Visible Light Communication](#user-content-visible-Light)
      - [LoRa/LoRaWAN](#user-content-loralorawan)
      - [mmWave Communication](#user-content-millimeter-Wave)
      - [LPWAN](#user-content-lpwan)
      - [SDR](#user-content-sdr)
      - [CTC](#user-content-ctc)
      - [Bluetooth](#user-content-bluetooth)
      - [UWB](#user-content-uwb)
      - [TV Whitespace](#user-content-tv-whitespace)
      - [Acoustic Communication](#user-content-acoustic)
      - [Multi-band Operation](#user-content-multi-band)
      - [Other Networks](#user-content-other-sensor-network)
    - [Batteryless Networking and Communication ](#user-content-batteryless)
      - [Wi-Fi Networks](#user-content-wifi-1)
      - [Visible Light Communication](#user-content-visible-Light-1)
      - [LoRa/LoRaWAN](#user-content-lora)
      - [mmWave Communication](#user-content-millimeter-wave-1)
      - [RFID](#user-content-rfid)
      - [Acoustic Communication](#user-content-acoustic-1)
      - [Other Networks](#user-content-other-batteryless-works)
  - 🚀 [Domain-specific AIoT Systems (Total: 255)](#domain-specific-aiot-systems)
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
## 🌡️ Sensing (320)

<a name="motion-sensing"></a>
### Motion Sensing (Total: 10 | No ML(1) | ML(2) | DL(7))
#### Human Activity Recognition
* Practically Adopting Human Activity Recognition, MobiCom 23 [[Paper]](https://dapowan.github.io/files/UniHAR.pdf) (DL)
* LIMU-BERT: Unleashing the Potential of Unlabeled Data for IMU Sensing Applications, SenSys 21 [[Paper]](https://tanrui.github.io/pub/LIMU_BERT.pdf) (DL)
* Transferring Activity Recognition Models for New Wearable Sensors with Deep Generative Domain Adaptation, IPSN 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3302506.3310391) (DL)
* SenseHAR: a robust virtual activity sensor for smartphones and wearables, SenSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3356250.3360032) (DL)
* Synchronous Dynamic View Learning: A Framework for Autonomous Training of Activity Recognition Models using Wearable Sensors, IPSN 17 [[Paper]](https://www.ceid.upatras.gr/webpages/courses/adhocnets/files/papers/paper7.pdf) (ML)
* Lasagna: Towards Deep Hierarchical Understanding and Searching over Mobile Sensing Data, MobiCom 16 [[Paper]](http://tns.thss.tsinghua.edu.cn/~cihangliu/papers/lasagna.pdf) (DL)  

#### Arm Tracking
* Real-Time Tracking of Smartwatch Orientation and Location by Multitask Learning, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568548) (DL)
* Real-time Arm Skeleton Tracking and Gesture Inference Tolerant to Missing Wearable Sensors, MobiSys 19 [[Paper]](https://yangliu-cs.github.io/YangLiu-CS/paper/2019-MobiSys-ArmTroi.pdf) (DL)
* Closing the Gaps in Inertial Motion Tracking, MobiCom 18 [[Paper]](https://synrg.csl.illinois.edu/papers/muse-mobicom18.pdf) (No ML)
* I am a Smartwatch and I can Track my User’s Arm, MobiSys 16 [[Paper]](https://synrg.csl.illinois.edu/papers/ArmTrak_Mobisys.pdf) (ML)

<a name="wireless-sensing"></a>
### Wireless Sensing (145)
<a name="rfid-sensing"></a>
#### RFID Sensing (Total: 29 | No ML(23) | ML(1) | DL(5))
* A Handheld Fine-Grained RFID Localization System with Complex-Controlled Polarization, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592504) (No ML)
* Fast, Fine-grained, and Robust Grouping of RFIDs, MobiCom 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3570361.3592510) (No ML)
* MetaSight: Localizing Blocked RFID Objects by Modulating NLOS Signals via Metasurfaces, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538947) (No ML)
* A Passive Eye-in-Hand “Camera” for Minature Robots, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568505) (No ML)
* ShakeReader: ‘Read’ UHF RFID using Smartphone, INFOCOM 21 [[Paper]](https://web.comp.polyu.edu.hk/csyqzheng/papers/ShakeReader-INFOCOM21.pdf) (No ML)
* Thermotag: item-level temperature sensing with a passive RFID tag, MobiSys 21 [[Paper]](https://cs.nju.edu.cn/liujia/papers/mobisys21-themotag.pdf) (No ML)
* RFGo: A Seamless Self-checkout System for Apparel Stores Using RFID, MobiCom 20 [[Paper]](https://genesys-lab.org/papers/RFGo-Mobicom.pdf) (DL)
* Food and Liquid Sensing in Practical Environments using RFIDs, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-ha.pdf) (DL)
* Exploring commodity RFID for contactless sub-millimeter vibration sensing, SenSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3384419.3430771) (No ML)
* Sensing Finger Input Using An RFID Transmission Line, SenSys 20 [[Paper]](http://web.cs.ucla.edu/~omid/Papers/Sensys20.pdf) (No ML)
* RTSense: RFID based Temperature Sensing, SenSys 20 [[Paper]](https://www.swadhinpradhan.com/papers/rtsense.pdf) (No ML)
* 3D-OmniTrack: 3D Tracking with COTS RFID Systems, IPSN 19 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/2019.4.pdf) (No ML)
* Are RFID Sensing Systems Ready for the Real World?, MobiSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3307334.3326084) (No ML)
* Detecting Misplaced RFID Tags on Static Shelved Items, MobiSys 19 [[Paper]](https://rtcl.eecs.umich.edu/rtclweb/assets/publications/2019/luo-mobisys19.pdf) (ML)
* RFID based real-time recognition of ongoing gesture with adversarial learning, SenSys 19 [[Paper]](https://dl.acm.org/doi/10.1145/3356250.3360045) (DL)
* FaHo: deep learning enhanced holographic localization for RFID tags, SenSys 19 [[Paper]](https://dapowan.github.io/files/FaHo.pdf) (DL)
* Tagtag: material sensing with commodity RFID, SenSys 19 [[Paper]](https://dl.acm.org/doi/10.1145/3356250.3360027) (No ML)
* Orientation-aware RFID Tracking with Centimeter-level Accuracy, IPSN 18 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/2018.8.pdf) (No ML)
* Challenge: RFID Hacking for Fun and Profit, MobiCom 18 [[Paper]](http://web.cs.ucla.edu/~omid/Papers/Mobicom18a.pdf) (No ML)
* WiSh: Towards a Wireless Shape-aware World using Passive RFIDs, MobiSys 18 [[Paper]](https://www.witechlab.com/papers/wish-mobisys2018.pdf) (No ML)
* Minding the Billions: Ultra-wideband Localization for Deployed RFID Tags, MobiCom 17 [[Paper]](https://www.mit.edu/~fadel/papers/RFind-paper.pdf) (No ML)
* TagScan: Simultaneous Target Imaging and Material Identification with Commodity RFID Devices, MobiCom 17 [[Paper]](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=4878&context=sis_research) (No ML)
* RIO: A Pervasive RFID-based Touch Gesture Interface, MobiCom 17 [[Paper]](https://dl.acm.org/doi/10.1145/3117811.3117818) (No ML)
* Enabling gesture-based interactions with objects, MobiSys 17 [[Paper]](https://core.ac.uk/download/pdf/286384108.pdf) (No ML)
* Gyro in the Air: Tracking 3D Orientation of Batteryless Internet-of-Things, MobiCom 16 [[Paper]](http://xyzhang.ucsd.edu/papers/TWei_MobiCom16_Tagyro.pdf) (No ML)
* 3D Real-time Indoor Localization via Broadband Nonlinear Backscatter in Passive Devices with Centimeter Precision, MobiCom 16 [[Paper]](https://yfmascgy.github.io/papers/3d-localization.pdf) (No ML)
* Analog On-Tag Hashing: Towards Selective Reading as Hash Primitives in Gen2 RFID Systems, MobiCom 16 [[Paper]](https://web.comp.polyu.edu.hk/csyanglei/data/files/tash-mobicom17.pdf) (No ML)
* The Design and Implementation of a Mobile RFID Tag Sorting Robot, MobiSys 16 [[Paper]](https://discovery.ucl.ac.uk/id/eprint/1493115/1/mobitagbot_for_rps.pdf) (No ML)
* Deep Learning for RFID-Based Activity Recognition, SenSys 16 [[Paper]](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6205502/) (DL)

<a name="wi-fi-sensing"></a>
#### Wi-Fi Sensing (Total: 56 | No ML(24) | ML(11) | DL(20) | GenAI(1))
##### Human Activity Recognition
* XGait: Cross-Modal Translation via Deep Generative Sensing for RF-based Gait Recognition, SenSys 23 [[Paper]](https://perfecthu.github.io/publications/23-sensys-xgait.pdf) (DL)
* SiFall: Practical Online Fall Detection with RF Sensing, SenSys 22 [[Paper]](https://arxiv.org/pdf/2301.03773.pdf) (DL)
* Counting a stationary crowd using off-the-shelf wifi, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3468012) (No ML)
* OneFi: One-Shot Recognition for Unseen Gesture via COTS WiFi, SenSys 21 [[Paper]](https://ruixiao24.github.io/files/rui_onefi.pdf) [[Code]](https://github.com/ruixiao24/onefi) (DL)
* RF-net: a unified meta-learning framework for RF-enabled one-shot human activity recognition,	SenSys	20 [[Paper]](https://arxiv.org/pdf/2111.04566.pdf) (DL)
* Zero-Effort Cross-Domain Gesture Recognition with Wi-Fi, MobiSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3307334.3326081) (DL)
* Widar2.0: Passive Human Tracking with a Single Wi-Fi Link, MobiSys 18 [[Paper]](https://www.cswu.me/papers/mobisys18_widar2.0_paper.pdf) (ML)
* Towards Environment Independent Device Free Human Activity Recognition, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241548) (DL)
* CrossSense: Towards Cross-Site and Large-Scale WiFi Sensing, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241570) (DL)
* WiWho: WiFi-Based Person Identification in Smart Spaces, IPSN 16 [[Paper]](https://ieeexplore.ieee.org/document/7460727) (ML)

##### 3D Human Mesh Reconstruction
* Construct 3D Hand Skeleton with Commercial WiFi, SenSys 23 [[Paper]](https://arxiv.org/pdf/2312.15507) (DL)
* Wi-Mesh: A WiFi Vision-based Approach for 3D Human Mesh Construction, SenSys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3560905.3568536) (DL)
* Towards 3D human pose construction using wifi, MobiCom 20 [[Paper]](https://cse.buffalo.edu/~lusu/papers/MobiCom2020.pdf) (DL)

##### Indoor Localization
* Understanding Localization by a Tailored GPT, Mobisys 24[[Paper]](https://dl.acm.org/doi/10.1145/3643832.3661869) (DL)
* BIFROST: Reinventing WiFi Signals Based on Dispersion Effect for Accurate Indoor Localization, SenSys 23 [[Paper]](https://wangwg1996.github.io/files/PDF/BIFROST_conf.pdf) (No ML)
* Enabling Ubiquitous Wi-Fi Sensing with Beamforming Reports, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/10.1145/3603269.3604817) (ML)
* RIScan: RIS-aided Multi-user Indoor Localization Using COTS Wi-Fi, SenSys 23 [[Paper]](https://www.chenhuangxun.com/files/sensys23-riscan.pdf) (No ML)
* Placement Matters: Understanding the Effects of Device Placement for WiFi Sensing, IMWUT 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3517237) (No ML)
* Experience: pushing indoor localization from laboratory to the wild, MobiCom 22  [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560546) (Best Community Contribution Runner-ups) (DL)
* Accurate Ubiquitous Localization with Off-the-Shelf IEEE 802.11ac Devices, MobiSys 21 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/963/main.pdf) (No ML)
* WiForce: Wireless Sensing and Localization of Contact Forces on a Space Continuum, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-gupta.pdf) (No ML)
* Deep learning based wireless localization for indoor navigation, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3380894) (DL)
* LocAP: Autonomous Millimeter Accurate Mapping of WiFi Infrastructure, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-ayyalasomayajula.pdf) (No ML)
* Multipath Triangulation: Decimeter-level WiFi Localization and Orientation with a Single Unaided Receiver, MobiSys 18 [[Paper]](https://elahe.web.illinois.edu/Elahe%20Soltan_files/papers/MobiSys18_MonoLoco_CameraReady.pdf) (No ML)
* Verification: Accuracy Evaluation of WiFi Fine Time Measurements on an Open Platform, MobiCom 18 [[Paper]](https://winlab.rutgers.edu/~gruteser/papers/ftm_mobicom.pdf) (No ML)
* Decimeter-Level Localization with a Single WiFi Access Point, NSDI 16 [[Paper]](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-vasisht.pdf) (No ML)
* LiFS: Low Human-Effort Device-Free Localization with Fine-Grained Subcarrier Information, MobiCom 16 [[Paper]](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=4390&context=sis_research) (No ML)
 
##### Imaging
* Wiffract: A New Foundation for RF Imaging via Edge Tracing, MobiCom 22 [[Paper]](https://web.ece.ucsb.edu/~ymostofi/papers/PallaproluKoranyMostofi_MobiCom2022.pdf) (ML)
* Wi-Fi See It All: Generative Adversarial Network-augmented Versatile Wi-Fi Imaging, SenSys 20 [[Paper]](https://cse.msu.edu/~caozc/papers/sensys20-chen.pdf) (DL)
* 3D Through-Wall Imaging with Unmanned Aerial Vehicles Using WiFi, IPSN 17 [[Paper]](https://web.ece.ucsb.edu/~ymostofi/papers/IPSN17_KaranamMostofi.pdf) (No ML)

##### Gesture Recognition
* RF-Diffusion: Radio Signal Generation via Time-Frequency Diffusion, MobiCom 24 [[Paper]](https://arxiv.org/pdf/2404.09140) (GenAI)
* UniFi: A Unified Framework for Generalizable Gesture Recognition with Wi-Fi Signals Using Consistency-guided Multi-View Networks, IMWUT 24 [[Paper]](https://dl.acm.org/doi/10.1145/3631429) (DL)
* SLNet: A Spectrogram Learning Neural Network for Deep Wireless Sensing, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-yang-zheng.pdf) (DL)
* MUSE-Fi: Contactless MUti-person SEnsing Exploiting Near-field Wi-Fi Channel Variation, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613290) (DL)
* RF-URL: unsupervised representation learning for RF sensing, MobiCom 22 [[Paper]](http://staff.ustc.edu.cn/~dongheng/dhfiles/rf-url.pdf) (DL)
* Solving the WiFi Sensing Dilemma in Reality Leveraging Conformal Prediction, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568529) (DL)
* Understanding WiFi signal frequency features for position-independent gesture sensing, IEEE Transactions on Mobile Computing 22 [[Paper]](https://hal.science/hal-03363402/file/Understanding_WiFi_Signal_Frequency_Features_for_Position-Independent_Gesture_Sensing.pdf) (No ML)
* Towards Position-Independent Sensing for Gesture Recognition with Wi-Fi, IMWUT 21 [[Paper]](https://www.researchgate.net/publication/352731286_Towards_Position-Independent_Sensing_for_Gesture_Recognition_with_Wi-Fi) (No ML)
* RF-based Inertial Measurement, SIGCOMM 19 [[Paper]](https://cswu.me/papers/sigcomm19_rim_paper.pdf) (No ML)
* Multi-User Gesture Recognition Using WiFi, MobiSys 18 [[Paper]](https://raghavhv.wordpress.ncsu.edu/files/2018/06/mobisys18-31-hampapur.pdf) (No ML)
* Position and Orientation Agnostic Gesture Recognition Using WiFi, MobiSys 17 [[Paper]](https://dl.acm.org/doi/10.1145/3081333.3081340) (ML)
* WiFi-Enabled Smart Human Dynamics Monitoring, SenSys 17 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3131672.3131692) (ML)
* Calibrating Time-variant, Device-specific Phase Noise for COTS WiFi Devices, SenSys 17 [[Paper]](https://netstech.org/wp-content/uploads/2018/10/phase_calibration_sensys17.pdf) (No ML)
* HeadScan: A Wearable System for Radio-based Sensing of Head and Mouth-related Activities, IPSN 16 [[Paper]](https://innovationcenter.msu.edu/wp-content/uploads/2021/07/HeadScan-A-Wearable-System-for-Radio-Based-Sensing-of-Head-and-Mouth-Related-Activities-1.pdf) (ML)
* BodyScan: Enabling Radio-based Sensing on Wearable Devices for Contactless Activity and Vital Sign Monitoring, MobiSys 16 [[Paper]](https://mi-zhang.github.io/papers/2016_MobiSys_BodyScan.pdf) (ML)

##### Respiration Monitoring
* MultiSense: Enabling Multi-person Respiration Sensing with Commodity WiFi, IMWUT 20 [[Paper]](https://hal.science/hal-03363355v1/file/3411816.pdf) (No ML)
* FarSense: Pushing the Range Limit of WiFi-based Respiration Sensing with CSI Ratio of Two Antennas, IMWUT 19 [[Ppaper]](https://arxiv.org/pdf/1907.03994) (No ML)

##### Tracking
* Tracking from One Side -- Multi-Person Passive Tracking with WiFi Magnitude Measurements, IPSN 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3302506.3310399) (No ML)
* Toward Reliable Localization by Unequal AoA Tracking, MobiSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3307334.3326103) (No ML)
* On the Feasibility of Wi-Fi Based Material Sensing, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345442) (ML)
* mD-Track: Leveraging Multi-Dimensionality for Passive Indoor Wi-Fi Tracking, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300133) (ML)
* Magnitude-Based Angle-of-Arrival Estimation, Localization, and Target Tracking, IPSN 18 [[Paper]](https://web.ece.ucsb.edu/~ymostofi/papers/IPSN18_KaranamKoranyMostofi.pdf) (No ML)

##### Copresence and proximity detection
* Next2You: Robust Copresence Detection Based on Channel State Information, SenSys 23 [[Paper]](https://arxiv.org/pdf/2111.05224) (DL)
* Proximity Detection with Single-Antenna IoT Devices, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300120) (No ML)

##### Human-Computer Interaction
* Exploring Multiple Antennas for Long-range WiFi Sensing, IMWUT 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3494979) (No ML)
* LiveTag: Sensing Human-Object Interaction through Passive Chipless WiFi Tags, NSDI 18 [[Paper]](https://www.usenix.org/system/files/conference/nsdi18/nsdi18-gao.pdf) (ML)

<a name="mmwave-sensing"></a>
#### mmWave Sensing (Total: 24 | No ML(7) | ML(3) | DL(13) | GenAI(1))

##### Human Activity Recognition
* mmFER: Millimetre-wave Radar based Facial Expression Recognition for Multimedia IoT Applications, MobiCom 23 [[Paper]](https://taogu.site/pub/paper/23-mobicom-mmFER.pdf) (DL)
* Towards Generalized mmWave-based Human Pose Estimation through Signal Augmentation, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613302) (DL)
* XGait: Cross-Modal Translation via Deep Generative Sensing for RF-based Gait Recognition, SenSys 23 [[Paper]](https://perfecthu.github.io/publications/23-sensys-xgait.pdf) (DL)
* SPARCS: A Sparse Recovery Approach for Integrated Communication and Human Sensing in mmWave Systems, IPSN 22 [[Paper]](https://arxiv.org/pdf/2205.03263.pdf) (DL)

##### 3D Human Mesh Reconstruction
* mm3DFace: Nonintrusive 3D Facial Reconstruction Leveraging mmWave Signals, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596839) (DL)
* m3Track: mmWave-based Multi-User 3D Posture Tracking, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538926) (DL)
* M4esh: mmWave-Based 3D Human Mesh Construction for Multiple Subjects,	SenSys	22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568545) (DL)
* Synthesized Millimeter-Waves for Human Motion Sensing, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568542) (DL)
* mmMesh: towards 3D real-time dynamic human mesh construction using millimeter-wave, MobiSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3458864.3467679) (DL)

##### Voice Reconstruction
* WaveEar: Exploring a mmWave-based Noise-resistant Speech Sensing for Voice-User Interface, Mobisys 19 [[Paper]](https://dl.acm.org/doi/10.1145/3307334.3326073) (DL)
* FerroTag: a paper-based mmWave-scannable tagging infrastructure, SenSys 19 [[Paper]](https://dl.acm.org/doi/10.1145/3356250.3360019) (Best Paper) (ML)

##### Object Recognition
* Fusang: Graph-inspired Robust and Accurate Object Recognition on Commodity mmWave Devices, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596849) [[Code]](https://github.com/OpenNISLab/Pro-Fusang) (DL)

##### Indoor Mapping
* See through smoke: robust indoor mapping with low-cost mmWave radar,	MobiSys	20 [[Paper]](https://arxiv.org/pdf/1911.00398.pdf) (DL)

##### Temperature Monitoring
* ThermoWave: A New Paradigm of Wireless Passive Temperature Monitoring via mmWave Sensing, MobiCom 20 [[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-mobicom2020b.pdf) (DL)

##### Localization
* Hawkeye: Hectometer-range Subcentimeter Localization for Large-scale mmWave Backscatter, MobiSys 23 [[Paper]](https://arxiv.org/pdf/2301.02402.pdf) (No ML)
* Accurate 3D Localization for 60 GHz Networks, SenSys 18 [[Paper]](https://dl.acm.org/doi/10.1145/3274783.3274852) (No ML)
* Augmenting mmWave localization accuracy through sub-6 GHz on off-the-shelf devices, MobiSys 22 [[Paper]](https://www.researchgate.net/publication/361567899_Augmenting_mmWave_localization_accuracy_through_sub-6_GHz_on_off-the-shelf_devices) (No ML)
* Millimetro: mmWave Retro-Reflective Tags for Accurate, Long Range Localization, MobiCom 21 [[Paper]](https://swarunkumar.com/papers/millimetro-mobicom2021.pdf) (No ML)

##### Measurement and displacement sensing
* Platypus: Sub-mm Micro-Displacement Sensing with Passive Millimeter-wave Tags As "Phase Carriers", IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586965) (No ML)
* mmVib: micrometer-level vibration measurement with mmwave radar, MobiCom 20 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/mmVib_MobiCom2020.pdf) (No ML)
* Dancing Waltz with Ghosts: Measuring Sub-𝑚𝑚-Level 2D Rotor Orbit with a Single mmWave Radar, IPSN 21 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/GWaltz_IPSN2021.pdf) (ML)

##### Miscellaneous Topics
* Push the Limit of Single-Chip mmWave Radar-Based Egomotion Estimation with Moving Objects in FoV, SenSys 23 [[Paper]](https://dl.acm.org/doi/10.1145/3625687.3625795) (No ML)
* RF Genesis: Zero-Shot Generalization of mmWave Sensing through Simulation-Based Data Synthesis and Generative Diffusion Models, SenSys 23 [[Paper]](http://xyzhang.ucsd.edu/papers/Xingyu.Chen_SenSys23_RFGen.pdf) (GenAI)
* Osprey: A mmWave Approach to Tire Wear Sensing, MobiSys 20 [[Paper]](https://swarunkumar.com/papers/osprey-mobisys2020.pdf) (ML)

<a name="lte-sensing"></a>
#### LTE Sensing (Total: 4 | No ML(3) | ML(0) | DL(1))
##### Traffic Monitoring
* Experience: Large-scale Cellular Localization for Pickup Position Recommendation at Black-hole, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613298) (DL)
* Enabling IoT Self-Localization Using Ambient 5G Signals, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-jog.pdf) (No ML)
* LTE-based Pervasive Sensing Across Indoor and Outdoor, Sensys 21 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/SenSys21-LTESensing.pdf) (No ML)

##### Soil Moisture Monitoring
* LTE-Based Low-Cost and Low-Power Soil Moisture Sensing, Sensys 22 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/SenSys22-SoilMoisture.pdf) (No ML)

<a name="lora-sensing"></a>
#### LoRa Sensing (Total: 5 | No ML(3) | ML(0) | DL(2))
* OrchLoc: In-Orchard Localization via a Single LoRa Gateway and Generative Diffusion Model-based Fingerprinting, MobiSys 24 [[Paper]](https://dl.acm.org/doi/10.1145/3643832.3661876) (DL)
* Boosting the Long Range Sensing Potential of LoRa, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596847) (No ML)
* XGait: Cross-Modal Translation via Deep Generative Sensing for RF-based Gait Recognition, SenSys 23 [[Paper]](https://perfecthu.github.io/publications/23-sensys-xgait.pdf) (DL)
* Embracing LoRa Sensing with Device Mobility, SenSys 22 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/SenSys22-LoRaSensingMobility.pdf) (No ML)
* Combating interference for long range LoRa sensing, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430731) (No ML)

<a name="teraHertz-sensing"></a>
#### TeraHertz Sensing (Total: 2 | No ML(2) | ML(0) | DL(0))
* Quasi-Optical 3D localization using Asymmetric Signatures above 100 GHz, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3517022) (No ML)
* LeakyTrack: Non-Coherent Single-Antenna Nodal and Environmental Mobility Tracking with a Leaky-Wave Antenna, SenSys 20 [[Paper]](https://www.brown.edu/research/labs/mittleman/sites/brown.edu.research.labs.mittleman/files/uploads/SenSys_2020.pdf) (No ML)

<a name="uwb-sensing"></a>
#### UWB Sensing (Total: 12 | No ML(9) | ML(1) | DL(2))
* Mobi2Sense: Empowering Wireless Sensing with Mobility, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560518) (No ML) (Best Paper Award Runner-ups) 
* Enabling High Accuracy Pervasive Tracking with Ultra Low Power UWB Tags, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560542) (No ML)
* SiWa: See into Walls via Deep UWB Radars, MobiCom 21 [[Paper]](https://arxiv.org/pdf/2110.14279.pdf) (DL)
* MoRe-Fi: Motion-robust and Fine-grained Respiration Monitoring via Deep-Learning UWB Radar, SenSys 21 [[Paper]](https://arxiv.org/pdf/2111.08195.pdf) (DL)
* UWHear: Through-wall Extraction and Separation of Audio Vibrations Using Wireless Signals, SenSys 20 [[Paper]](https://ziqi.plus/papers/UWHear.pdf) (No ML)
* Chorus: UWB Concurrent Transmissions for GPS-like Passive Localization of Countless Target, IPSN 19 [[Paper]](http://dit.unitn.it/~picco/papers/ipsn19-uwb.pdf) (No ML)
* SnapLoc: An Ultra-Fast UWB-Based Indoor Localization System for an Unlimited Number of Tag, IPSN 19 [[Paper]](http://www.carloalbertoboano.com/documents/grosswindhager19snaploc.pdf) (No ML)
* LiquID: A Wireless Liquid IDentifier, MobiSys 18 [[Paper]](https://synrg.csl.illinois.edu/papers/liquid_mobisys2018.pdf) (No ML)
* SALMA: UWB-based Single-Anchor Localization System using Multipath Assistance, SenSys 18 [[Paper]](http://www.carloalbertoboano.com/documents/grosswindhager18salma.pdf) (No ML)
* Calibration-Free Network Localization using Non-Line-of-Sight Ultra-Wideband Measurements, IPSN 17 [[Paper]](https://web.eecs.umich.edu/~prabal/pubs/papers/di_franco17nlos.pdf) (ML)
* SurePoint: Exploiting Ultra Wideband Flooding and Diversity to Provide Robust, Scalable, High-Fidelity Indoor Localization, SenSys 16 [[Paper]](https://patpannuto.com/pubs/kempke16surepoint.pdf) (No ML)
* Harmonium: Asymmetric, Bandstitched UWB for Fast, Accurate, and Robust Indoor Localization, IPSN 16 [[Paper]](https://patpannuto.com/pubs/kempke16harmonium.pdf) (No ML)

<a name="bluetooth-sensing"></a>
#### Bluetooth Sensing (Total: 5 | No ML(2) | ML(1) | DL(2))
* Experience: Practical Indoor Localization for Malls, MobiCom 22 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/mloc_mobicom22.pdf) (Best Community Contribution) (DL)
* BLE Can See: A Reinforcement Learning Approach for RF-based Indoor Occupancy Detection, IPSN 21 [[Paper]](https://www.cs.virginia.edu/~bjc8c/papers/billah21blecansee.pdf) (DL)
* From Conception to Retirement: a Lifetime Story of a 3-Year-Old Wireless Beacon System in the Wild, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-ding.pdf) (No ML)
* Nationwide Deployment and Operation of a Virtual Arrival Detection System in the Wild, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472911.pdf) (No ML)
* Group-In: Group Inference from Wireless Traces of Mobile Devices, IPSN 20 [[Paper]](https://arxiv.org/pdf/2005.12848.pdf) (ML)

<a name="nfc-sensing"></a>
#### NFC Sensing (Total: 1 | No ML(1) | ML(0) | DL(0))
* Locating Everyday Objects using NFC Textiles, IPSN 21 [[Paper]](https://swarunkumar.com/papers/textilesense-ipsn2021.pdf) (No ML)

<a name="rf-sensing"></a>
#### Others (Total: 7 | No ML(2) | ML(1) | DL(4))
* Quantum Wireless Sensing: Principle, Design and Implementation, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613258) (No ML)
* DancingAnt: Body-empowered Wireless Sensing Utilizing Pervasive Radiations from Powerline, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613272) (No ML)
* Quantifying the Physical Separability of RF-based Multi-Person Respiration Monitoring via SINR, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568513) (DL)
* RISE: robust wireless sensing using probabilistic and statistical assessments, MobiCom 21 [[Paper]](https://helda.helsinki.fi/server/api/core/bitstreams/e81bf5a7-1e69-442f-82d6-1bed63f39578/content) (DL)
* RF-based 3D skeletons, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230579) (DL)
* RF-Echo: A Non-Line-of-Sight Indoor Localization System Using a Low-Power Active RF Reflector ASIC Tag, MobiCom 17 [[Paper]](https://blaauw.engin.umich.edu/wp-content/uploads/sites/342/2019/12/RF-Echo-A-Non-Line-of-Sight-Indoor-Localization-System-Using-a-Low-Power-Active-RF-Reflector-ASIC-Tag.pdf) (DL）
* Emotion Recognition using Wireless Signals, MobiCom 16 [[Paper]](http://eqradio.csail.mit.edu/files/eqradio-paper.pdf) (ML)

<a name="vision-sensing"></a>
### Vision Sensing (Total: 30 | No ML(7) | ML(2) | DL(21))

#### Human Activity Recognition
* Mosaic: Extremely Low-resolution RFID Vision for Visually-anonymized Action Recognition, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586968) (DL)
* MobiPose: real-time multi-person pose estimation on mobile devices, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430726) (DL)

#### Image Enhancement
* NeuriCam: Key-Frame Video Super-Resolution and Colorization for IoT Cameras, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592523) (DL)
* MobiSpectral: Hyperspectral Imaging on Mobile Devices, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613296) [[Code]](https://github.com/mobispectral/mobicom23_mobispectral) (DL)
* MicroDeblur: Image Motion Deblurring on Microcontroller-based Vision Systems, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586970) (DL)
* DoCam: Depth Sensing with an Optical Image Stabilization Supported RGB Camera, MobiCom 22 [[Paper]](https://www.cs.sjtu.edu.cn/~yichao/assets/publications/mobicom22_pan.pdf) (No ML)
* Starfish: resilient image compression for AIoT cameras, SenSys 20 [[Paper]](https://panhu.me/pdf/2020/Starfish.pdf) (DL)
* MobiSR: Efficient On-Device Super-Resolution through Heterogeneous Mobile Processors, MobiCom 19 [[Paper]](https://arxiv.org/pdf/1908.07985.pdf) (DL)
* HyperSight: boosting distant 3D vision on a single dual-camera smartphone, SenSys 19 [[Paper]](https://dl.acm.org/doi/10.1145/3356250.3360029) (No ML)

#### Object Detection
* Mozart: A Mobile ToF System for Sensing in the Dark through Phase Manipulation, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596840) (DL)
* Squint: A Framework for Dynamic Voltage Scaling of Image Sensors Towards Low Power IoT Vision, MobiCom 23 [[Paper]](https://par.nsf.gov/servlets/purl/10466003) (DL)
* Testing Masks and Air Filters With Your Smartphones, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625807) (DL)
* QfaR: Location-Guided Scanning of Visual Codes from Long Distances, MobiCom 23 [[Paper]](https://wisionlab.com/wp-content/uploads/2023/06/MOBICOM_2023___QfaR.pdf) (DL)
* Detecting Counterfeit Liquid Food Products in a Sealed Bottle Using a Smartphone Camera, MobiSys 22 [[Paper]](https://www.comp.nus.edu.sg/~chanmc/papers-by-year/2022-mobisys.pdf) (DL)
* Edge-Eye: Rectifying Millimeter-Level Edge Deviation in Manufacturing using Camera-Enabled IoT Edge Device, IPSN 22 [[Paper]](https://taogu.site/pub/paper/IPSN2022.pdf) (DL)
* LAPD: Hidden Spy Camera Detection using Smartphone Time-of-Flight Sensors, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485941) (DL)
* UltraDepth: Exposing High-Resolution Texture from Depth Cameras, SenSys 21 [[Paper]](http://cvlab.cse.msu.edu/pdfs/Xie_Ouyang_Liu_Xing_UltraDepth_SenSys2021.pdf) (DL)
* EagleEye: wearable camera-based person identification in crowded urban spaces, MobiCom 20 [[Paper]](https://juheonyi.github.io/files/EagleEye.pdf) (DL)
* Wireless Computer Vision Using Commodity Radios, IPSN 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3302506.3310403) (ML)
* Banner: An Image Sensor Reconfiguration Framework for Seamless Resolution-based Tradeoffs, MobiSys 19	[[Paper]](https://meteor.ame.asu.edu/publications/mobisys19hu-banner.pdf) (No ML)
* Liquid Testing with Your Smartphone, MobiSys 19 [[Paper]](https://people.csail.mit.edu/scyue/projects/capcam/capcam.pdf) (No ML)
* ODDS: Real-Time Object Detection using Depth Sensors on Embedded GPUs, IPSN 18 [[Paper]](https://ieeexplore.ieee.org/document/8480074) (DL)
* Glimpse: A Programmable Early-Discard Camera Architecture for Continuous Mobile Vision, MobiSys 17 [[Paper]](https://archive.md2k.org/images/papers/sensors/mobisys17-Glimpse.pdf) (Honorable Mention) (No ML)

#### Eye Tracking
* Gaze Tracking on Any Surface with Your Phone, SenSys 22 [[Paper]](https://www.cs.cityu.edu.hk/~zhenjili/2022-SenSys-ASGaze.pdf) [[code]](https://github.com/Jiani-CAO/ASGaze) (DL)
* GazeGraph: Graph-based Few-Shot Cognitive Context Sensing from Human Visual Behavior, SenSys 20 [[Paper]](https://par.nsf.gov/servlets/purl/10296635) (DL)
* EMO: real-time emotion recognition from single-eye images for resource-constrained eyewear devices, MobiSys 20 [[Paper]](https://dongshuhao.github.io/assets/pdf/2020/Wu_2020.pdf) (DL)

#### Pose Estimation
* RoFin: 3D Hand Pose Reconstructing via 2D Rolling Fingertips, MobiSys 23 [[Paper]](https://tianxing.me/paper/zhang-mobisys23.pdf) (DL)
* MoiréPose: Ultra High Precision Camera-to-Screen Pose Estimation based on Moiré Pattern, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560537) (No ML)
* Glimpse.3D: A Motion-Triggered Stereo Body Camera for 3D Experience Capture and Preview, IPSN 18 [[Paper]](https://www.ceid.upatras.gr/webpages/courses/adhocnets/files/papers/paper8.pdf) (ML)

#### Depth Estimation
* MobiDepth: Real-Time Depth Estimation Using On-Device Dual Cameras, MobiCom 22 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2022/09/mobicom22-final138.pdf) (No ML)

<a name="acoustic-sensing"></a>
### Acoustic Sensing (Total: 51 | No ML(24) | ML(10) | DL(17))

#### Localization
* DeepEar: Sound Localization With Binaural Microphones, IEEE Transactions on Mobile Computing 2024 [[Paper]](https://ieeexplore.ieee.org/document/9954178) (DL)
* Owlet: enabling spatial information in ubiquitous acoustic devices,	MobiSys	21	[[Paper]](https://www.cs.umd.edu/~nirupam/images/2_publication/papers/Owlet_MobiSys21_nirupam.pdf) (DL)  
* DeepRange: Acoustic Ranging via Deep Learning, IMWUT 2020 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3432195) (DL)
* MOM: Microphone based 3D Orientation Measurement, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a120/962400a120.pdf) (ML)
* MAVL: Multiresolution Analysis of Voice Localization, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-wang-mei.pdf) (No ML)
* Voice Localization Using Nearby Wall Reflections, MobiCom 20 [[Paper]](https://synrg.csl.illinois.edu/papers/voloc_mobicom20.pdf) (No ML)
* Can a Phone Hear the Shape of a Room?, IPSN 19 [[Paper]](https://users.ece.cmu.edu/~agr/resources/publications/ipsn19-shih.pdf) (ML)

#### Movement Tracking
* Addressing Practical Challenges in Acoustic Sensing To Enable Fast Motion Tracking, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586954) (No ML)
* SVoice: Enabling Voice Communication in Silence via Acoustic Sensing on Commodity Devices, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568530) (DL)
* Experience: practical problems for acoustic sensing,	MobiCom	22 [[Paper]](https://people.cs.umass.edu/~dli/papers/MobiCom22_Experience.pdf) (No ML)
* Enabling Contact-free Acoustic Sensing under Device Motion, IMWUT 22 [[Paper]](https://jialinliu.me/papers/IMWUT22-SonicBot.pdf) (No ML)
* MagicInput: Training-free Multi-lingual Finger Input System using Data Augmentation based on MNISTs, ISPN 21 [[Paper]](https://www.cs.sjtu.edu.cn/~yichao/assets/publications/ipsn21_pan.pdf)	(ML)
* FM-Track: Pushing the Limits of Contactless Multi-target Tracking using Acoustic Signals, SenSys 20 [[Paper]](https://people.cs.umass.edu/~dli/papers/SenSys20_FM-Track.pdf) (No ML)
* RNN-Based Room Scale Hand Motion Tracking, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345439) (DL)
* Your Table Can Be an Input Panel: Acoustic-based Device-Free Interaction Recognition, IMWUT 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3314390) (DL)
* BreathListener: Fine-grained Breathing Monitoring in Driving Environments Utilizing Acoustic Signals, MobiSys 19 [[Paper]](https://www.cs.sjtu.edu.cn/~linghe.kong/2019/XuMOBISYS2019BreathListener.pdf) (DL)
* Rebooting Ultrasonic Positioning Systems for Ultrasound-incapable Smart Devices, MobiCom 19 [[Paper]](https://arxiv.org/pdf/1812.02349.pdf) (No ML)
* VSkin: Sensing Touch Gestures on Surfaces of Mobile Devices Using Acoustic Signals, MobiCom 18 [[Paper]](https://cs.nju.edu.cn/lxie/publication/Mobicom2018.pdf) (No ML)
* Strata: Fine-Grained Acoustic-based Device-Free Tracking, MobiSys 17 [[Paper]](https://www.cs.sjtu.edu.cn/~yichao/pmwiki/assets/publications/mobisys17_strata.pdf) (No ML)
* CAT: High-Precision Acoustic Motion Tracking, MobiCom 16 [[Paper]](https://dl.acm.org/doi/10.1145/2973750.2973755) (No ML)

#### Emotion Recognition
* Mic2Mic: Using Cycle-Consistent Generative Adversarial Networks to Overcome Microphone Variability in Speech Systems, IPSN 19 [[Paper]](https://core.ac.uk/download/pdf/219542364.pdf) (DL)
* Low-resource Multi-task Audio Sensing for Mobile and Embedded Devices via Shared Deep Neural Network Representations, UbiComp 17 [[Paper]](https://core.ac.uk/reader/227518690) (DL)
* DeepEar: robust smartphone audio sensing in unconstrained acoustic environments using deep learning, UbiComp 15 [[Paper]](https://core.ac.uk/download/pdf/42340233.pdf) (DL)

#### Keyword and Event Detection
* SoundSieve: Seconds-Long Audio Event Recognition on Intermittently-Powered Systems, MobiSys 23 [[Paper]](https://arxiv.org/pdf/2305.16445.pdf) (DL)
* A closer look at quality-aware runtime assessment of sensing models in multi-device environments, SenSys 19 [[Paper]](https://akhilmathurs.github.io/papers/min_sensys2019.pdf) (DL)

#### Gesture Recognition
* Device-Free Gesture Tracking Using Acoustic Signals, MobiCom 16 [[Paper]](https://cs.nju.edu.cn/ww/papers/mobicom16_ultrasound.pdf) (No ML)
* Sequence-Based Device-Free Gesture Recognition Framework for Multi-Channel Acoustic Signals, ICASSP 23 [[Paper]](https://ieeexplore.ieee.org/abstract/document/10095790) (DL)
* Room-scale Hand Gesture Recognition Using Smart Speakers, SenSys 22 [[Paper]](https://people.cs.umass.edu/~dli/papers/SenSys2022_SpeakerGesture.pdf) (ML)
* LASense: Pushing the Limits of Fine-grained Activity Sensing Using Acoustic Sign, IMWUT 22 [[Paper]](https://people.cs.umass.edu/~dli/papers/IMWUT22_LASense.pdf) (No ML)	

#### Source Identification
* Meta-Speaker: Acoustic Source Projection by Exploiting Air Nonlinearity, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613279) (No ML)
* SCAN: Learning Speaker Identity From Noisy Sensor Data, IPSN 17 [[Paper]](https://www.ceid.upatras.gr/webpages/courses/sensornets/papers/paper8.pdf) (ML)
* Symphony: Localizing Multiple Acoustic Sources with a Single Microphone Array, SenSys 20 [[Paper]](https://arxiv.org/pdf/2209.15325.pdf) (No ML)
* BodyBeat: A Mobile System for Sensing Non-Speech Body Sounds, MobiSys 14 [[Paper]](https://pac.cs.cornell.edu/pubs/body-beat-mobisys-2014.pdf) (ML)

####  Miscellaneous Topics
* PowerPhone: Unleashing the Acoustic Sensing Capability of Smartphones, MobiCom 23 [[Paper]](https://people.cs.umass.edu/~dli/papers/Mobicom23_PowerPhone.pdf) (DL)
* VeCare: Statistical Acoustic Sensing for Automotive In-Cabin Monitoring, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-zhang-yi.pdf) (No ML)
* Acoustic Sensing and Communication Using Metasurface, NSDI 23	[[Paper]](https://www.usenix.org/system/files/nsdi23-zhang-yongzhao.pdf) (No ML)
* AvA: An Adaptive Audio Filtering Architecture for Enhancing Mobile, Embedded, and Cyber-Physical Systems, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a106/962400a106.pdf) (ML)
* SPiDR: ultra-low-power acoustic spatial sensing for micro-robot navigation,	MobiSys	22	[[Paper]](https://www.cs.umd.edu/~nakul/assets/papers/spidr_mobisys2022_nakul.pdf) (No ML) (Best Paper)
* SQEE: A Machine Perception Approach to Sensing Quality Evaluation at the Edge by Uncertainty Quantification, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568534) (DL)
* SpeechQoE: A Novel Personalized QoE Assessment Model for Voice Services via Speech Sensing, SenSys 22 [[Paper]](https://ranger.uta.edu/~mingli/publications/SpeechQoE.pdf) (DL)
* Sound-Adapter: Multi-Source Domain Adaptation for Acoustic Classification Through Domain Discovery, IPSN 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3412382.3458265) (DL)
* CSafe: An Intelligent Audio Wearable Platform for Improving Construction Worker Safety in Urban Environments, IPSN 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3412382.3458267) (ML)
* Microphone Array Backscatter: An Application-Driven Design for Lightweight Spatial Sound Recording over the Air, MobiCom 21 [[Paper]](https://www2.cs.sfu.ca/~jcliu/Papers/Microphone21.pdf) (No ML)
* AcuTe: acoustic thermometer empowered by a single smartphone, SenSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3384419.3430714)[[Code]](https://github.com/caichao/AcuTe) (No ML)
* Cross-Platform Support for Rapid Development of Mobile Acoustic Sensing Applications, MobiSys 18 [[Paper]](https://rtcl.eecs.umich.edu/rtclweb/assets/publications/2018/paper_mobisys_final_acmart_upload.pdf) (ML)
* Sonoloc: Scalable positioning of commodity mobile devices, MobiSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3210240.3210324) (No ML)
* AIM: Acoustic Imaging on a Mobile, MobiSys 18 [[Paper]](https://www.cs.utexas.edu/~meiwang/uploads/8/9/9/1/89919297/aim.pdf) (Best Paper) (No ML)
* UbiTap: Leveraging Acoustic Dispersion for Ubiquitous Touch Interface on Solid Surfaces, SenSys 18 [[Paper]](http://cps.kaist.ac.kr/papers/18SenSys-UbiTap.pdf) (Best paper runner-up awards) (No ML)
* SoundSifter: Mitigating Overhearing of Continuous Listening Devices, MobiSys 17 [[Paper]](https://www.cs.unc.edu/~nirjon/paper/soundsifter-mobisys2017.pdf) (ML)
* DopEnc: Acoustic-based Encounter Profiling Using Smartphones, MobiCom 16 [[Paper]](https://zhoupf.github.io/assets/papers/MobiCom16-DopEnc.pdf) (No ML)
* Expansion of Human–Phone Interface By Sensing Structure-Borne Sound Propagation, MobiSys 16 [[Paper]](https://yctung.github.io/files/publication/mobisys16-forcephone.pdf) (No ML)
																
<a name="multi-modal-sensing"></a>
### Multi-Modal Sensing (Total: 37 | No ML(3) | ML(9) | DL(25))

#### Human Activity Recognition
* CMA: Cross-Modal Association Between Wearable and Structural Vibration Signal Segments for Indoor Occupant Sensing, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586960) (DL)
* MESEN: Exploit Multimodal Data to Design Unimodal Human Activity Recognition with Few Labels, SenSys 23 [[Paper]](https://arxiv.org/pdf/2404.01958) (DL)
* VMA: Domain Variance- and Modality-Aware Model Transfer for Fine-Grained Occupant Activity Recognition, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a247/962400a247.pdf) (DL)
* Cosmo: contrastive fusion learning with small data for multimodal human activity recognition,	MobiCom	22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560519)[[Code]](https://github.com/xmouyang/Cosmo) (DL)
* Low-latency speculative inference on distributed multi-modal data streams,MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3467884) (DL)
* Optimal sensor channel selection for resource-efficient deep activity recognition, IPSN 21 [[Paper]](https://acris.aalto.fi/ws/portalfiles/portal/64950790/ELEC_Souza_Leite_Xiao_Optimal_Sensor_Channel_IPSN_2021_acceptedauthormanuscript.pdf) (DL)
* Multimodal deep learning for activity and context recognition, UbiComp 18 [[Paper]](https://homepages.inf.ed.ac.uk/mmarina/papers/ubicomp18.pdf) (DL)

#### Human and Object Identification
* Contactless Material Identification with Millimeter Wave Vibrometry, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596850) (DL)
* Capricorn: Towards Real-Time Rich Scene Analysis Using RF-Vision Sensor Fusion, SenSys22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568504) (DL)
* Vi-Fi: Associating Moving Subjects across Vision and Wireless Sensor, IPSN 22 [[Paper]](https://www.winlab.rutgers.edu/~hansiiii/papers/ViFi_Paper___IPSN_2022__Camera_Ready_.pdf) (DL)
* RFID and camera fusion for recognition of human-object interactions, MobiCom	21 [[Paper]](https://taogu.site/pub/paper/22-mobicom-RFID.pdf) (DL)	
* XModal-ID: Using WiFi for Through-Wall Person Identification from Candidate Video Footage, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345437) (DL)

#### Tracking
* Interpersonal Distance Tracking with mmWave Radar and IMUs, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586958) (DL)
* ITrackU: tracking a pen-like instrument via UWB-IMU fusion, MobiSys 21 [[Paper]](https://faculty.cc.gatech.edu/~dhekne/itracku_mobisys2021.pdf) (No ML)		
* milliEgo: single-chip mmWave radar aided egomotion estimation via deep sensor fusion,	SenSys	20	[[Paper]](https://arxiv.org/pdf/2006.02266.pdf) (DL)
* BatTracker: High Precision Infrastructure-free Mobile Device Tracking in Indoor Environments, SenSys 17 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3131672.3131689) (ML)

#### Localization
* Indoor Smartphone SLAM with Learned Echoic Location Features, SenSys 22 [[Paper]](https://arxiv.org/pdf/2210.08493.pdf) (DL)
* RFusion: Robotic Grasping via RF-Visual Sensing and Learning, SenSys 21 [[Paper]](https://www.mit.edu/~fadel/papers/RFusion-paper.pdf) (DL)
* The Wisdom of 1,170 Teams: Lessons and Experiences from a Large Indoor Localization Competition, MobiCom 23 [[Paper]](https://yshu.org/paper/mobicom23comp.pdf) (DL) (Best Community Contributions Award)
* BatMapper: Acoustic Sensing Based Indoor Floor Plan Construction Using Smartphones, MobiSys 17 [[Paper]](https://zhoubinwy.github.io/pdf/batmapper.pdf) (No ML)
* Indoor localization via multi-modal sensing on smartphones, UbiComp 16 [[Paper]](https://zhouzimu.github.io/paper/ubicomp16-xu.pdf) (ML)

#### Speech Enhancement 
* Towards Bone-Conducted Vibration Speech Enhancement on Head-Mounted Wearables, MobiSys 23 [[Paper]](https://yanzhenyu.com/assets/pdf/VibVoice-MobiSys23.pdf) (DL)
* UltraSE: single-channel speech enhancement using ultrasound, MobiCom 21 [[Paper]](http://xyzhang.ucsd.edu/papers/Ke.Sun_MobiCom21_UltraSE.pdf) (DL)	
* Wavoice: A Noise-resistant Multi-modal Speech Recognition System Fusing mmWave and Audio Signals,	SenSys	21	[[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-sensys2021.pdf) (DL)

#### Miscellaneous Topics
* Physics-Informed Data Denoising for Real-Life Sensing Systems, Sensys 23 [[Paper]](https://arxiv.org/pdf/2311.06968) (DL)
* SudokuSens: Enhancing Deep Learning Robustness for IoT Sensing Applications using a Generative Approach, SenSys 23 [[Paper]](https://arxiv.org/pdf/2402.02275) (DL)
* MiLTOn: Sensing Product Integrity without Opening the Box using Non-Invasive Acoustic Vibrometry, IPSN 22 [[Paper]](https://swarunkumar.com/papers/milton-ipsn2022.pdf) (ML)
* Motion inspires notion: self-supervised visual-LiDAR fusion for environment depth estimation, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538918) (DL)
* UniTS: Short-Time Fourier Inspired Neural Networks for Sensory Time Series Classification,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485942) (DL)
* SmrtFridge: IoT-based,  user interaction-driven food item & quantity sensing,	SenSys 19 [[Paper]](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=5649&context=sis_research) (DL)
* CrowdEstimator: Approximating Crowd Sizes with Multi-modal Data for Internet-of-Things Services, MobiSys 18 [[Paper]](https://arxiv.org/pdf/1909.13673.pdf) (ML)	
* EAR: Exploiting Uncontrollable Ambient RF Signals in Heterogeneous Networks for Gesture Recognition, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274847) (ML)
* EngageMon: Multi-Modal Engagement Sensing for Mobile Games, UbiComp 18 [[Paper]](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=5060&context=sis_research) (ML)
* Bringing IoT to Sports Analytics, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-gowda.pdf) (No ML)
* Non-Intrusive Multi-Modal Estimation of Building Occupancy, SenSys 17 [[Paper]](http://www.phpathak.com/files/occupancy-sensys.pdf) (ML)
* Sensor-assisted Face Recognition System on Smart Glass via Multi-view Sparse Representation Classification, IPSN 16 [[Paper]](https://www.cse.unsw.edu.au/~wenh/xu_ipsn_20162.pdf) (ML)
* TransitLabel: A Crowd-Sensing System for Automatic Labeling of Transit Stations Semantics, MobiSys 16 [[Paper]](https://arxiv.org/pdf/1606.03302.pdf) (ML)

<a name="earable-sensing"></a>
### Earable Sensing (Total: 19 | No ML(4) | ML(8) | DL(7))
#### Facial Expression Sensing 
* FaceListener: Recognizing Human Facial Expressions via Acoustic Sensing on Commodity Headphones, IPSN 22 [[Paper]](https://sites.pitt.edu/~weigao/publications/ipsn22.pdf) [[Dataset]](https://developers.google.com/mediapipe) [[Code]](https://github.com/muxspace/facial_expressions) (DL)
* BioFace-3D: Continuous 3D Facial Reconstruction Through Lightweight Single-ear Biosensors, MobiCom 21 [[Paper]](https://people.cs.umass.edu/~phuc/papers/bioface_2021.pdf) (DL)

#### User Identification
* EarGate: Gait-based User Identification with In-ear Microphones, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483240) (DL)
* MandiPass: Secure and Usable User Authentication via Earphone IMU, IEEE Transactions on Mobile Computing 2021 [[Paper]](https://ieeexplore.ieee.org/document/9546415) (DL)
* HeadFi: bringing intelligence to all headphones, MobiCom 21	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3448624) (Best Paper Award Runner-up) (ML) 

#### Sound Localization
* DeepEar: Sound Localization With Binaural Microphones, IEEE Transactions on Mobile Computing 2024 [[Paper]](https://ieeexplore.ieee.org/document/9954178) (DL)
* ClearBuds: wireless binaural earbuds for learning-based speech enhancement, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538933) [[Code]](https://clearbuds.cs.washington.edu) (DL)
* Individualizing Head Related Transfer Functions for Binaural Acoustic Applications, IPSN 22 [[Paper]](https://arxiv.org/pdf/2203.11138.pdf) (DL)
* Personalizing Head Related Transfer Functions for Earables, SIGCOMM 21 [[Paper]](https://synrg.csl.illinois.edu/papers/UNIQ_Sigcomm21.pdf) (No ML)

#### Noise Cancellation
* WINC: A Wireless IoT Network for Multi-Noise Source Cancellation, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586964) (ML)
* MUTE: bringing IoT to noise cancellation, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230550) (No ML)

#### Miscellaneous Topics
* Sensing with Earables: A Systematic Literature Review and Taxonomy of Phenomena, IMWUT 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3550314) (Survey)
* OESense: employing occlusion effect for in-ear human sensing, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3467680) (ML)
* Ear-AR: indoor acoustic augmented reality on earphones, MobiCom 20 [[Paper]](https://synrg.csl.illinois.edu/papers/ear-ar_mobicom20.pdf) (ML)
* EarSense: Earphones as a Teeth Activity Sensor, MobiCom 20 [[Paper]](https://synrg.csl.illinois.edu/papers/earsense_mobicom20.pdf) (No ML)
* WAKE: A Behind-the-ear Wearable System for Microsleep Detection, MobiSys 20 [[Paper]](http://mnslab.org/tamvu/paper/2020%20WAKE_Nhat.pdf) (ML)
* EarphoneTrack: involving earphones into the ecosystem of acoustic motion tracking, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430730) (No ML)
* ERICA: Enabling Real-time Mistake Detection & Corrective Feedback for Free-Weights Exercises, SenSys 20 [[Paper]](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=6897&context=sis_research) (ML)
* TYTH-Typing On Your Teeth: Tongue-Teeth Localization for Human-Computer Interface, MobiSys 18 [[Paper]](http://mnslab.org/tamvu/paper/2018%20TYTH_Phuc.pdf) (ML)
* A Lightweight And Inexpensive In-ear Sensing System For Automatic Whole-night Sleep Stage Monitoring, SenSys 16 [[Paper]](http://mnslab.org/tamvu/paper/2016%20Inear%20Lan%20Anh.pdf) (ML)

<a name="light-sensing"></a>
### Visible Light Sensing (Total: 15 | No ML(7) | ML(7) | DL(1))
* LiT: Fine-grained Toothbrushing Monitoring with Commercial LED Toothbrush, MobiCom 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3570361.3613287) (ML)
* SMART: Screen-based Gesture Recognition on Commodity Mobile Devices, MobiCom 21 [[Paper]](https://huangqy7.github.io/Paper/mobicom21-SMART.pdf) (DL)
* Lili: Liquor Quality Monitoring Based on Light Signals, MobiCom 21 [[Paper]](https://luwang-szu.github.io/paper/LiliMobiCom.pdf) (ML)
* CurveLight:An Accurateand Practical Light Positioning System, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485934) (ML)
* LiTag: Localization and Posture Estimation with Passive Visible Light Tags, SenSys 20 [[Paper]](https://www.cse.msu.edu/~lilingk1/publications/sensys20-LiTag.pdf) (No ML)
* SolarGest: Ubiquitous and Battery-free Gesture Recognition using Solar Cells, MobiCom 19 [[Paper]](https://arxiv.org/pdf/1812.01766.pdf) (ML)
* RainbowLight: Towards Low Cost Ambient Light Positioning with Mobile Phones, MobiCom 18 [[Paper]](http://tns.thss.tsinghua.edu.cn/~jiliang/publications/MOBICOM2018-rainbowlight.pdf) (No ML)
* Battery-Free Eye Tracker on Glasses, MobiCom 18 [[Paper]](https://digitalcommons.dartmouth.edu/cgi/viewcontent.cgi?article=3975&context=facoa) (ML)
* Augmenting Indoor Inertial Tracking with Polarized Light, MobiSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3210240.3210340) (No ML)
* Pulsar: Towards Ubiquitous Visible Light Localization, MobiCom 17 [[Paper]](https://dl.acm.org/doi/10.1145/3117811.3117821) (No ML)
* CELLI: Indoor Positioning Using Polarized Sweeping Light Beams, MobiSys 17 [[Paper]](https://dl.acm.org/doi/10.1145/3081333.3081352) (ML)
* Enabling High-Precision Visible Light Localization in Today’s Buildings. MobiSys 17 [[Paper]](https://cseweb.ucsd.edu//~shz338/images/MobiSys_17.pdf) (ML)
* SmartLight: Light-weight 3D Indoor Localization Using a Single LED Lamp, SenSys 17 [[Paper]](https://www-users.cse.umn.edu/~tianhe/Papers/SmartLight.pdf) (No ML) (Best Paper)
* LiTell: Robust Indoor Localization Using Unmodified Light Fixtures, MobiCom 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2973750.2973767) (No ML)
* Practical Human Sensing in the Light, MobiSys 16 [[Paper]](https://www.cs.columbia.edu/~xia/publication/mobisys16-starlight/mobisys16-starlight.pdf) (No ML)

<a name="magnetic-sensing"></a>
### Magentic Sensing (Total: 6 | No ML(1) | ML(3) | DL(2))
* METRO: Magnetic Road Markings for All-weather, Smart Roads, SenSys 23 [[Paper]](https://theisclab.com/docs/2023_Sensys_METRO_Wang.pdf) (No ML)
* Automatic Calibration of Magnetic Tracking, MobiCom 22 [[Paper]](https://rtcl.eecs.umich.edu/rtclweb/assets/publications/2022/mobicom22-wang.pdf) (ML)
* MagX: Wearable, Untethered Hands Tracking with Passive Magnets, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483260) (ML)
* MET: a magneto-inductive sensing based electric toothbrushing monitoring system, MobiCom 20 [[Paper]](https://www.ece.stonybrook.edu/~slin/Publications/MOBICOM2020.pdf) (DL)
* MagHacker: Eavesdropping on Stylus Pen Writing via Magnetic Sensing from Commodity Mobile Devices, MobiSys 20 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobisys20.pdf) (DL)
* MagTrack: Enabling Safe Driving Monitoring with Wearable Magnetics, MobiSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3307334.3326107) (ML)

<a name="cross-medium-sensing"></a>
### Cross-Medium Sensing (Total: 2 | No ML(2) | ML(0) | DL(0))
* Underwater 3D positioning on smart devices, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3603269.3604851) (No ML)
* Sunflower: Locating Underwater Robots From the Air,	MobiSys	22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3539773) (No ML)

<a name="generative-ai-for-sensing"></a>
### Generative AI for Sensing (Total: 4 | No ML(0) | ML(0) | DL(0) | GenAI(4))
* MEIT: Multi-Modal Electrocardiogram Instruction Tuning on Large Language Models for Report Generation, Arxiv 24 [[Paper]](https://arxiv.org/abs/2403.04945) (GenAI)
* LLMSense: Harnessing LLMs for High-level Reasoning Over Spatiotemporal Sensor Traces, arxiv 24 [[Paper]](https://arxiv.org/pdf/2403.19857) (GenAI)
* LLaSA: Large Multimodal Agent for Human Activity Analysis Through Wearable Sensors, arxiv 24 [[Paper]](https://arxiv.org/pdf/2406.14498) (GenAI)
* Penetrative AI: Making LLMs Comprehend the Physical World, HOTMOBILE 24 [[Paper]](https://arxiv.org/pdf/2310.09605) (GenAI)
  
## 📲 Computing (168)							
<a name="computing"></a>	
### On-Device Inference	(Total: 61)					
<a name="on-device-inference"></a>

#### Inference Optimization (Total: 16)
<a name="inference-optimization"></a>
* Boosting DNN Cold Inference on Devices, MobiSys 23 [[Paper]](https://arxiv.org/pdf/2206.07446)
* LUT-NN: Empower Efficient Neural Network Inference with Centroid Learning and Table Lookup, MobiCom 23 [[Paper]](https://arxiv.org/pdf/2302.03213)
* Space-Efficient TREC for Enabling Deep Learning on Microcontrollers, ASPLOS 23 [[Paper]](https://research.csc.ncsu.edu/picture/publications/papers/asplos23a_mcu.pdf)
* ConvReLU++: Reference-based Lossless Acceleration of Conv-ReLU Operations on Mobile CPU, MobiSys 23 [[Paper]](https://yuanchun-li.github.io/static/files/MobiSys23_ConvReLU++.pdf) [[Code]](https://github.com/GAIR-team/conv_relu_plus_plus)
* mGEMM: Low-latency Convolution with Minimal Memory Overhead Optimized for Mobile Devices, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538940)
* NeuLens: spatial-based dynamic acceleration of convolutional neural networks on edge, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560528)
* BiSon-e: a lightweight and high-performance accelerator for narrow integer linear algebra computing on the edge, ASPLOS 22 [[Paper]](https://upcommons.upc.edu/bitstream/handle/2117/367954/bisone_paper.pdf?sequence=3)
* InFi: end-to-end learnable input filter for resource-efficient mobile-centric inference, MobiCom 22 [[Paper]](https://yuanmu97.github.io/preprint/InFi_MobiCom22.pdf)
* Flexible High-resolution Object Detection on Edge Devices with Tunable Latency, MobiCom 21 [[Paper]](https://yshu.org/paper/mobicom21remix.pdf)
* MCUNetV2: Memory-Efficient Patch-based Inference for Tiny Deep Learning, NeurIPS 21 [[Paper]](https://arxiv.org/pdf/2110.15352)
* Intelligence Beyond the Edge: Inference on Intermittent Embedded Systems, ASPLOS 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3297858.3304011)
* DeQA: On-Device Question Answering, MobiSys 19 [[Paper]](https://www3.cs.stonybrook.edu/~arunab/papers/deqa.pdf)   
* DeepCache: Principled Cache for Mobile Deep Vision, MobiCom 18 [[Paper]](https://arxiv.org/pdf/1712.01670.pdf) [[Code]](https://github.com/xumengwei/DeepCache) (DL)
* FastDeepIoT: Towards Understanding and Optimizing Neural Network Execution Time on Mobile and Embedded Devices, SenSys 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3274783.3274840)
* DeepMon: Mobile GPU-based Deep Learning Framework for Continuous Vision Applications, MobiSys 17 [[Paper]](https://www.cse.iitd.ac.in/~rijurekha/course/deepmon.pdf) 
* SC-DCNN: Highly-Scalable Deep Convolutional Neural Network using Stochastic Computing, ASPLOS 17 [[Paper]](http://alchem.usc.edu/portal/static/download/sc_dcnn.pdf) 

#### Multi-Tenant Inference (Total: 14)
* Miriam: Exploiting Elastic Kernels for Real-time Multi-DNN Inference on Edge GPU, SenSys 23 [[Paper]](https://arxiv.org/pdf/2307.04339)
* POS: An Operator Scheduling Framework for Multi-model Inference on Edge Intelligent Computing, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586953)
* Microsecond-scale Preemption for Concurrent GPU-accelerated DNN Inferences, OSDI 22 [[Paper]](https://www.usenix.org/conference/osdi22/presentation/han)
* YONO: Modeling Multiple Heterogeneous Neural Networks on Microcontrollers, IPSN 22 [[Paper]](https://arxiv.org/pdf/2203.03794.pdf)   
* VELTAIR: towards high-performance multi-tenant deep learning services via adaptive compilation and scheduling, ASPLOS	22 [[Paper]](https://cs.sjtu.edu.cn/~leng-jw/resources/Files/liu22asplos-veltair.pdf)
* RT-mDL: Supporting Real-Time Mixed Deep Learning Tasks on Edge Platforms, SenSys 21 [[Paper]](https://neawhen.github.io/neiwen.github.io/assets/pdf/RT-mDL_SenSys2021.pdf)
* LegoDNN: block-grained scaling of deep neural networks for mobile vision, MobiCom 21 [[Paper]](https://arxiv.org/pdf/2112.09852.pdf) (Best Community Paper Award Runner-Up)	
* NeuOS: A Latency-Predictable Multi-Dimensional Optimization Framework for DNN-driven Autonomous Systems, ATC 20 [[Paper]](https://www.usenix.org/system/files/atc20-bateni.pdf)
* Fast and scalable in-memory deep multitask learning via neural weight virtualization,	MobiSys	20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388947)		
* NestDNN: Resource-Aware Multi-Tenant On-Device Deep Learning for Continuous Mobile Vision, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241559)
* Potluck: Cross-Application Approximate Deduplication for Computation-Intensive Mobile Applications, ASPLOS 18	[[Paper]](https://www.cs.yale.edu/homes/guo-peizhen/files/potluck-asplos18.pdf) (DL)
* Mainstream: Dynamic Stem-Sharing for Multi-Tenant Video Processing, ATC 18 [[Paper]](https://www.usenix.org/system/files/conference/atc18/atc18-jiang.pdf)			
* DeepEye: Resource Efficient Local Execution of Multiple Deep Vision Models using Wearable Commodity Hardware, MobiSys 17 [[Paper]](https://akhilmathurs.github.io/papers/mathur_mobisys2017.pdf)
* MCDNN: An Approximation-Based Execution Framework for Deep Stream Processing Under Resource Constraints, MobiSys 17 [[Paper]](https://homes.cs.washington.edu/~arvind/papers/mcdnn.pdf)

#### Cross-Processor Inference (Total: 12)
<a name="cross-processor-inference"></a>
* NN-Stretch: Automatic Neural Network Branching for Parallel Inference on Heterogeneous Multi-Processors, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596870)
* PointSplit: Towards On-device 3D Object Detection with Heterogeneous Low-power Accelerators, IPSN 23 [[Paper]](https://www.researchgate.net/publication/370630326_PointSplit_Towards_On-device_3D_Object_Detection_with_Heterogeneous_Low-power_Accelerators)
* Band: Coordinated Multi-DNN Inference on Heterogeneous Mobile Processors, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538948)
* Mandheling: mixed-precision on-device DNN training with DSP offloading,MobiCom 22 [[Paper]](https://arxiv.org/pdf/2206.07509)			
* BlastNet: Exploiting Duo-Blocks for Cross-Processor Real-Time DNN Inference, SenSys 22 [[Paper]](https://yanzhenyu.com/assets/pdf/BlastNet-SenSys22.pdf)
* CoDL: Efficient CPU-GPU Co-execution for Deep Learning Inference on Mobile Devices, MobiSys 22 [[Paper]](https://chrisplus.me/assets/pdf/mobisys22-CoDL.pdf)
* AsyMo: Scalable and Efficient Deep-Learning Inference on Asymmetric Mobile CPUs, MobiCom 21 [[Paper]](https://www.msra.cn/wp-content/uploads/2021/03/mobicom21-asymo.pdf)
* Efficient Execution of Deep Neural Networks on Mobile Devices with NPU, IPSN 21 [[Paper]](http://mcn.cse.psu.edu/paper/tan-tianxiang/ipsn20-tan.pdf)		
* Neuro.ZERO: a zero-energy neural network accelerator for embedded sensing and inference systems, SenSys 19 [[Paper]](https://eisys.web.unc.edu/wp-content/uploads/sites/20971/2019/10/sensys19-final95.pdf)
* μLayer: Low Latency On-Device Inference Using Cooperative Single-Layer Acceleration and Processor-Friendly Quantization, EuroSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3302424.3303950)	
* Accelerating Mobile Audio Sensing Algorithms through On-Chip GPU Offloading, MobiSys 17 [[Paper]](https://www.cl.cam.ac.uk/~cm542/papers/mobisys17.pdf)
* DeepX: A Software Accelerator for Low-Power Deep Learning Inference on Mobile Devices, IPSN 16 [[Paper]](https://www.fahim-kawsar.net/papers/Lane.IPSN2016-Camera.pdf)

#### Runtime Adaptation (Total: 10)
<a name="runtime-adaptation"></a>
* AdaptiveNet: Post-deployment Neural Architecture Adaptation for Diverse Edge Environments, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592529)
* On-NAS: On-Device Neural Architecture Search on Memory-Constrained Intelligent Embedded Systems, SenSys 23 [[Paper]](https://aigs.unist.ac.kr/filebox/item/1917192674_8d43d5a0_On-NAS_SenSys2023.pdf) [[Code]](https://github.com/eai-lab/On-NAS)
* Adaptive Intelligence for Batteryless Sensors Using Software-Accelerated Tsetlin Machines, SenSys 22 [[Paper]](https://alessandro-montanari.github.io/papers/sensys2022.pdf)
* Memory-Efficient Domain Incremental Learning for Internet of Things,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568436)	
* LiteReconfig: Cost and Content Aware Reconfiguration of Video Object Detection Systems for Mobile GPUs, EuroSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3492321.3519577)
* Mistify: Automating DNN Model Porting for On-Device Inference at the Edge, NSDI 21	[[Paper]](https://www.usenix.org/system/files/nsdi21-guo.pdf)	
* Palleon: A Runtime System for Efficient Video Processing toward Dynamic Class Skew, ATC 21 [[Paper]](https://www.usenix.org/system/files/atc21-feng-boyuan.pdf)
* ApproxDet: Content and Contention-Aware Approximate Object Detection for Mobiles, SenSys 20 [[Paper]](https://arxiv.org/pdf/2010.10754.pdf)
* FlexDNN: Input-Adaptive On-Device Deep Learning for Efficient Mobile Vision, SEC 20 [[Paper]](https://mi-zhang.github.io/papers/2020_SEC_FlexDNN.pdf)
* MetaSense: few-shot adaptation to untrained conditions in deep mobile sensing, SenSys	19 [[Paper]](https://taesikgong.com/paper/SenSys19_MetaSense.pdf)
	
#### Model Compression (Total: 3)
<a name="model-compression"></a>
* On-Demand Deep Model Compression for Mobile Devices: A Usage-Driven Model Selection Framework, MobiSys 18 [[Paper]](https://tik-old.ee.ethz.ch/file//79a7dd6f6370f809e6180c0746232283/mobisys18-liu.pdf)
* DeepIoT: Compressing Deep Neural Network Structures for Sensing Systems with a Compressor-Critic Framework, SenSys 17 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3131672.3131675)
* Sparsification and Separation of Deep Learning Layers for Constrained Resource Inference on Wearables, SenSys 16 [[Paper]](https://discovery.ucl.ac.uk/id/eprint/1535346/1/main%20(3).pdf)
	
#### Privacy-Preserving Inference (Total: 3)
<a name="privacy-preserving"></a>
* Characterizing and Optimizing End-to-End Systems for Private Inference, ASPLOS 23 [[Paper]](https://arxiv.org/pdf/2207.07177.pdf)
* SOTER: Guarding Black-box Inference for General Neural Networks at the Edge, ATC 22 [[Paper]](https://www.usenix.org/system/files/atc22-shen.pdf)	
* Shredder: Learning Noise Distributions to Protect Inference Privacy, ASPLOS 20 [[Paper]](https://arxiv.org/pdf/1905.11814.pdf)
  
#### Benchmarks (Total: 3)
<a name="benchmarks"></a>
* nnPerf: Demystifying DNN Runtime Inference Latency on Mobile Platforms, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625797) [[Code]](https://github.com/nnperfwins/nnPerf)
* MLPerf Mobile Inference Benchmark, MLSys 22 [[Paper]](https://arxiv.org/pdf/2012.02328)
* URSABench: A System for Comprehensive Benchmarking of Bayesian Deep Neural Network Models and Inference methods, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/4a420924d20bc025ebb37849169e6ebd-Paper.pdf)	

### Offloading	(Total: 18)
#### Model Partitioning (Total: 3)
* Real-time Neural Network Inference on Extremely Weak Devices: Agile Offloading with Explainable AI, MobiCom 22 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobicom22.pdf)	
* CLIO: enabling automatic compilation of deep learning pipelines across IoT and cloud,	MobiCom	20 [[Paper]](https://www-users.cselabs.umn.edu/Fall-2021/csci8980-ec/papers/Clio.pdf)	
* Neurosurgeon: Collaborative Intelligence Between the Cloud and Mobile Edge, ASPLOS 17 [[Paper]](https://dl.acm.org/doi/10.1145/3037697.3037698)
  
#### Workload Partitioning (Total: 4)
* CoEdge: A Cooperative Edge System for Distributed Real-Time Deep Learning Tasks, IPSN 23 [[Paper]](https://neawhen.github.io/neiwen.github.io/assets/pdf/coedge_ipsn23.pdf)
* Elf: accelerate high-resolution mobile deep vision with content-aware parallel offloading, MobiCom 21 [[Paper]](https://www.msra.cn/wp-content/uploads/2021/03/mobicom21-elf.pdf)	
* Edge-SLAM: Edge-Assisted Visual Simultaneous Localization and Mapping, MobiSys 20 [[Paper]](https://par.nsf.gov/servlets/purl/10167133) (No ML) (Also AR)
* LEO: Scheduling Sensor Inference Algorithms across Heterogeneous Mobile Processors and Network Resources, MobiCom 16 [[Paper]](https://core.ac.uk/download/pdf/83939419.pdf)

#### Communication Optimization (Total: 6)
* Hyperion: A Generic and Distributed Mobile Offloading Framework on OpenCL, SenSys 22 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2022/11/sensys22-hyperion.pdf) (No ML)
* SwarmMap: Scaling Up Real-time Collaborative Visual SLAM at the Edge, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-xu_jingao.pdf) (No ML)
* Context-Aware Compilation of DNN Training Pipelines across Edge and Cloud, UbiComp 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3494981) [[code]](https://github.com/dixiyao/Context-Aware-Compilation-of-DNN-Training-Pipelines-across-Edge-and-Cloud)
* SPINN: synergistic progressive inference of neural networks over device and cloud, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419194)	
* Deep compressive offloading: speeding up neural network inference by trading edge computation for network latency,	SenSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430898)	
* Source Compression with Bounded DNN Perception Loss for IoT Edge Computer Vision,	MobiCom	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345448)		

#### Privacy-Preserving Offloading (Total: 5)
* PriMask: Cascadable and Collusion-Resilient Data Masking for Mobile Cloud Inference, SenSys 22 [[Paper]](https://arxiv.org/pdf/2211.06716.pdf)	
* EdgeFM: Leveraging Foundation Model for Open-set Learning on the Edge, SenSys 23 [[Paper]](https://arxiv.org/pdf/2311.10986) 
* AccuMO: Accuracy-Centric Multitask Offloading in Edge-Assisted Mobile Augmented Reality, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592531)
* Re-thinking computation offload for efficient inference on IoT devices with duty-cycled radios, MobiCom 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3570361.3592514)
* Walle: An End-to-End, General-Purpose, and Large-Scale Production System for Device-Cloud Collaborative Machine Learning, OSDI 22 [[Paper]](https://www.usenix.org/system/files/osdi22-lv.pdf)
	
### On-Device Training (Total: 13)
<a name="on-device-training"></a>
#### Training on a Single Device (Total: 11)
* Cost-effective On-device Continual Learning over Memory Hierarchy with Miro, MobiCom 23 [[Paper]](https://arxiv.org/pdf/2308.06053.pdf)
* LifeLearner: Hardware-Aware Meta Continual Learning System for Embedded Computing Platforms, SenSys 23 [[Paper]](https://arxiv.org/pdf/2311.11420)
* ElasticTrainer: Speeding Up On-Device Training with Runtime Elastic Tensor Selection, MobiSys 23 [[Paper]](https://hellokevin07.github.io/files/mobisys23-ElasticTrainer.pdf) [[Code]](https://github.com/HelloKevin07/ElasticTrainer)
* On-Device Training Under 256KB Memory, NeurIPS 22 [[Paper]](https://arxiv.org/abs/2206.15472)
* Campo: Cost-Aware Performance Optimization for Mixed-Precision Neural Network Training, ATC 22 [[Paper]](https://www.usenix.org/system/files/atc22-he.pdf)
* Memory-efficient DNN Training on Mobile Device, MobiSys 22	[[Paper]](https://dl.acm.org/doi/10.1145/3498361.3539765)	
* Melon: breaking the memory wall for resource-efficient on-device machine learning, MobiSys 22 [[Paper]](https://xumengwei.github.io/files/MobiSys22-Melo.pdf)
* Octo: INT8 Training with Loss-aware Compensation and Backward Quantization for Tiny On-device Learning,	ATC	21	[[Paper]](https://www.usenix.org/conference/atc21/presentation/zhou-qihua)
* MDLdroidLite: a release-and-inhibit control approach to resource-efficient deep neural networks on mobile devices,	SenSys	20	[[Paper]](https://taogu.site/pub/paper/Paper_3_SenSys_2020.pdf)	
* Full deep neural network training on a pruned weight budget,	MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/135.pdf)		
* Split-CNN: Splitting Window-based Operations in Convolutional Neural Networks for Memory System Optimization, ASPLOS 19 [[Paper]](https://dl.acm.org/doi/10.1145/3297858.3304038)	

#### Training across Distributed Devices (Total: 2)
* Mercury: Efficient On-Device Distributed DNN Training via Stochastic Importance Sampling, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485930)
* MDLdroid: a ChainSGD-reduce Approach to Mobile Deep Learning for Personal Mobile Sensing, IPSN 20 [[Paper]](https://arxiv.org/pdf/2002.02897.pdf)

### Federated Learning (Total: 41)
#### Data Heterogeneity (Total: 3)
* GPT-FL: Generative Pre-trained Model-Assisted Federated Learning." ArXiv 23 [[Paper]](https://arxiv.org/abs/2306.02210)
* BalanceFL: Addressing Class Imbalance in Long-tail Federated Learning, IPSN 22 [[Paper]](https://yanzhenyu.com/assets/pdf/BalanceFL-IPSN22.pdf) [[code]](https://github.com/sxontheway/BalanceFL)
*  FedBalancer: Data and Pace Control for Efficient Federated Learning on Heterogeneous Clients, MobiSys 22 [[Paper]](https://arxiv.org/pdf/2201.01601.pdf)

####  Communication Optimization (Total: 5)
* Faster Non-Convex Federated Learning via Global and Local Momentum, UAI 22 [[Paper]](https://openreview.net/forum?id=SSlLRUIs9e9)
* Adaptive Quantization of Model Updates for Communication-Efficient Federated Learning, ICASSP 21 [[Paper]](https://arxiv.org/pdf/2102.04487)
* Ensemble distillation for robust model fusion in federated learning, NeurIPS 20 [[Paper]](https://dl.acm.org/doi/abs/10.5555/3495724.3495922)
* FedPAQ: A Communication-Efficient Federated Learning Method with Periodic Averaging and Quantization, AISTATS 20 [[Paper]](http://proceedings.mlr.press/v108/reisizadeh20a/reisizadeh20a.pdf)
* A Distributed Synchronous SGD Algorithm with Global Top-k Sparsification for Low Bandwidth Networks, ICDCS 19 [[Paper]](https://www.computer.org/csdl/proceedings-article/icdcs/2019/251900c238/1ezRT3vzfcA)

#### System Heterogeneity (Total: 6)
* TimelyFL: Heterogeneity-aware Asynchronous Federated Learning with Adaptive Partial Training, CVPR Workshop 23 [[Paper]](https://arxiv.org/pdf/2304.06947)
* Federated Learning with Buffered Asynchronous Aggregation, AISTATS 22 [[Paper]](https://proceedings.mlr.press/v151/nguyen22b)
* FedSEA: A Semi-Asynchronous Federated Learning Framework for Extremely Heterogeneous Devices, SenSys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3560905.3568538)
* FedSA: A Semi-Asynchronous Federated Learning Mechanism in Heterogeneous Edge Computing, in IEEE Journal on Selected Areas in Communications 2021 [[Paper]](https://ieeexplore.ieee.org/document/9562538)
* SAFA: A Semi-Asynchronous Protocol for Fast Federated Learning With Low Overhead, in IEEE Transactions on Computers 2021 [[Paper]](https://wrap.warwick.ac.uk/id/eprint/136903/1/WRAP-safa-semi-asynchronous-protocol-fast-federated-learning-low-overhead-He-2020.pdf)
* Asynchronous Federated Optimization, Workshop on Optimization for Machine Learning in conjunction with NeurIPS 20 [[Paper]](https://arxiv.org/abs/1903.03934)

#### Personalization (Total: 6)
* FedSelect: Personalized Federated Learning with Customized Selection of Parameters for Fine-Tuning, CVPR 2024 [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/papers/Tamirisa_FedSelect_Personalized_Federated_Learning_with_Customized_Selection_of_Parameters_for_CVPR_2024_paper.pdf)
* AttFL: A Personalized Federated Learning Framework for Time-series Mobile and Embedded Sensor Data Processing, IMWUT 2024 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3610917) [[Code]](https://github.com/mobile-computing-K/AttFL)
* TailorFL: Dual-Personalized Federated Learning under System and Data Heterogeneity, SenSys 22 [[Paper]](https://dl.acm.org/doi/10.1145/3560905.3568503)
* Personalized Federated Learning by Structured and Unstructured Pruning under Data Heterogeneity, ICDCSW 21 [[Paper]](https://arxiv.org/pdf/2105.00562)
* FedDL: Federated Learning via Dynamic Layer Sharing for Human Activity Recognition, SenSys 21	[[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485946)	
* FedMask:  Joint Computation and Communication-Efficient Personalized Federated Learning via Heterogeneous Masking, SenSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485929)

#### Client Selection (Total: 3)
* PyramidFL: a fine-grained client selection framework for efficient federated learning, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517017)
* Oort: Efficient Federated Learning via Guided Participant Selection, OSDI 21 [[Paper]](https://www.usenix.org/system/files/osdi21-lai.pdf)		
* ClusterFL: a similarity-aware federated learning system for human activity recognition, MobiSys 21 [[Paper]](https://aiot.ie.cuhk.edu.hk/papers/ClusterFL.pdf)

#### Model Heterogeneity (Total: 7)
* FedRolex: Model-Heterogeneous Federated Learning with Rolling Sub-Model Extraction, NeurIPS 22 [[Paper]](https://openreview.net/forum?id=OtxyysUdBE)
* Heterogeneous Ensemble Knowledge Transfer for Training Large Models in Federated Learning, IJCAI 22 [[Paper]](https://www.ijcai.org/proceedings/2022/0399)
* FjORD: Fair and Accurate Federated Learning under heterogeneous targets with Ordered Dropout, NeurIPS 21 [[Paper]](https://proceedings.neurips.cc/paper/2021/file/6aed000af86a084f9cb0264161e29dd3-Paper.pdf)
* HeteroFL: Computation and Communication Efficient Federated Learning for Heterogeneous Clients, ICLR 21 [[Paper]](https://openreview.net/forum?id=TNkPBBYFkXg)
* Ensemble distillation for robust model fusion in federated learning, NeurIPS 20 [[Paper]](https://dl.acm.org/doi/abs/10.5555/3495724.3495922)
* FedMD: Heterogenous Federated Learning via Model Distillation, Workshop on Federated Learning for Data Privacy and Confidentiality in conjunction with NeurIPS 19 [[Paper]](https://arxiv.org/abs/1910.03581)
* Expanding the reach of federated learning by reducing client resource requirements, Arxiv 18 [[Paper]](https://arxiv.org/abs/1812.07210) 
			
#### Frameworks and Benchmarks (Total: 11)
* FedAIoT: A Federated Learning Benchmark for Artificial Intelligence of Things, DMLR 24 [[Paper]](https://openreview.net/forum?id=fYNw9Ukljz)
* FedMultimodal: A Benchmark for Multimodal Federated Learning, KDD 23 [[Paper]](https://arxiv.org/abs/2306.09486)
* FedAudio: A Federated Learning Benchmark for Audio Tasks, ICASSP 23 [[Paper]](https://arxiv.org/pdf/2210.15707.pdf)
* FedNLP: Benchmarking Federated Learning Methods for Natural Language Processing Tasks, NACCL 22 [[Paper]](https://arxiv.org/pdf/2104.08815.pdf) [[code]](https://github.com/FedML-AI/FedML/tree/master/python/app/fednlp) 
* Flower: A Friendly Federated Learning Research Framework, Arxiv 22 [[Paper]](https://arxiv.org/abs/2007.14390)
* FLamby: Datasets and Benchmarks for Cross-Silo Federated Learning in Realistic Healthcare Settings, NeurIPS 22 [[Paper]](https://openreview.net/forum?id=GgM5DiAb6A2)
* FLUTE: A Scalable, Extensible Framework for High-Performance Federated Learning Simulations, Workshop on Federated Learning: Recent Advances and New Challenges in conjunction with NeurIPS 22 [[Paper]](https://arxiv.org/abs/2203.13789)
* FedScale: Benchmarking Model and System Performance of Federated Learning at Scale, ICML 22 [[Paper]](https://openreview.net/forum?id=LZ5cx2yismf)
* FedCV: A Federated Learning Framework for Diverse Computer Vision Tasks, International Workshop on Trustable, Verifiable and Auditable Federated Learning in conjunction with AAAI 22 [[Paper]](https://arxiv.org/pdf/2111.11066.pdf) [[code]](https://github.com/FedML-AI/FedML/tree/master/python/app/fedcv)
* FedGraphNN: A Federated Learning System and Benchmark for Graph Neural Networks,  Workshop on Distributed and Private Machine Learning in conjunction with ICLR 21 [[Paper]](https://arxiv.org/abs/2104.07145)
* FedML: A Research Library and Benchmark for Federated Machine Learning, International Workshop on Scalability, Privacy, and Security in Federated Learning in conjunction with NeurIPS 20 [[Paper]](https://arxiv.org/abs/2007.13518)

### AI Agents for AIoT (Total: 5 | No ML(0) | ML(0) | DL(0) | GenAI(5))
<a name="ai-agent-aiot"></a>
* Mobile-Agent: Autonomous Multi-Modal Mobile Device Agent with Visual Perception, ICLR 2024 [[Paper]](https://arxiv.org/pdf/2401.16158) (GenAI)
* Octopus v2: On-device language model for super agent, Arxiv 2024 [[Paper]](https://arxiv.org/pdf/2404.01744) (GenAI)
* Octopus v3: Technical Report for On-device Sub-billion Multimodal AI Agent, Arxiv 2024 [[Paper]](https://arxiv.org/pdf/2404.11459v2) (GenAI)
* AutoDroid: LLM-powered Task Automation in Android, Mobicom '24 [[Paper]](https://chrisplus.me/assets/pdf/mobicom24-autoDroid.pdf) (GenAI)
* Towards an On-device Agent for Text Rewriting [[Paper]](https://arxiv.org/pdf/2308.11807) (GenAI)

### Automated Machine Learning (Total: 11)
<a name="auto-ML"></a>
* HarvNet: Resource-Optimized Operation of Multi-Exit Deep Neural Networks on Energy Harvesting Devices, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596845)
* Hyperscale Hardware Optimized Neural Architecture Search, ASPLOS 23 [[Paper]](https://dl.acm.org/doi/10.1145/3582016.3582049)
* Towards the Co-design of Neural Networks and Accelerators, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/4c430a4d0a7de11e85fa5b076e7f1895-Paper.pdf)
* MicroNets: Neural Network Architectures for Deploying TinyML Applications on Commodity Microcontrollers, MLSys 21	[[Paper]](https://arxiv.org/pdf/2010.11267)	
* nn-Meter: towards accurate latency prediction of deep-learning model inference on diverse edge devices, MobiSys 21 [[Paper]](https://air.tsinghua.edu.cn/pdf/nn-Meter-Towards-Accurate-Latency-Prediction-of-Deep-Learning-Model-Inference-on-Diverse-Edge-Devices.pdf) (Best Paper)		
* Neural Architecture Search as Program Transformation Exploration, ASPLOS 21 [[Paper]](https://arxiv.org/pdf/2102.06599.pdf)
* Mind Mappings: Enabling Efficient Algorithm-Accelerator Mapping Space Search, ASPLOS 21 [[Paper]](https://arxiv.org/pdf/2103.01489.pdf)
* Searching for Winograd-aware Quantized Networks, MLSys 20 [[Paper]](https://arxiv.org/pdf/2002.10711)
* SkyNet: a Hardware-Efficient Method for Object Detection and Tracking on Embedded Systems, MLSys 20 [[Paper]](https://arxiv.org/pdf/1909.09709)
* MCUNet: Tiny Deep Learning on IoT Devices,	NeurIPS	20	[[Paper]](https://proceedings.neurips.cc/paper/2020/hash/86c51678350f656dcc7f490a43946ee5-Abstract.html)	
* Does Unsupervised Architecture Representation Learning Help Neural Architecture Search?, NeurIPS 20 [[Paper]](https://proceedings.neurips.cc/paper/2020/hash/937936029af671cf479fa893db91cbdd-Abstract.html)	

### Compiler for AIoT (Total: 19)
<a name="compilers-for-aiot"></a>
* Heron: Automatically Constrained High-Performance Library Generation for Deep Learning Accelerators, ASPLOS 23 [[Paper]](https://dl.acm.org/doi/10.1145/3582016.3582061) [[Code]](https://github.com/IPRC-ICT/Heron)
* Bringing WebAssembly to Resource-constrained IoT Devices for Seamless Device-Cloud Integration, MobiSys 22 [[paper]](http://www.emnets.cn/zh/publication/mobisys-22-wait/WAIT.pdf) (No ML)
* Romou: rapidly generate high-performance tensor kernels for mobile GPUs,	MobiCom	22	[[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2022/02/mobigpu_mobicom22_camera.pdf)	
* The CoRa Tensor Compiler: Compilation for Ragged Tensors with Minimal Padding, MLSys 22 [[Paper]](https://arxiv.org/pdf/2110.10221)
* ROLLER: Fast and Efficient Tensor Compilation for Deep Learning,	OSDI	22	[[Paper]](https://www.usenix.org/conference/osdi22/presentation/zhu)			
* AStitch: Enabling a New Multi-dimensional Optimization Space for Memory-Intensive ML Training and Inference on Modern SIMT Architectures, ASPLOS 22 [[Paper]](https://github.com/alibaba/BladeDISC/blob/main/docs/papers/asplos-22-zhenzheng.pdf)
* TensorFlow Lite Micro: Embedded Machine Learning for TinyML Systems,	MLSys	21	[[Paper]](https://arxiv.org/pdf/2010.08678)
* Analytical Characterization and Design Space Exploration for Optimization of CNNs, ASPLOS 21 [[Paper]](https://arxiv.org/pdf/2101.09808.pdf)		
* Ordering Chaos: Memory-Aware Scheduling of Irregularly Wired Neural Networks for Edge Devices, MLSys 20 [[Paper]](https://arxiv.org/pdf/2003.02369)
* A Tensor Compiler for Unified Machine Learning Prediction Serving, OSDI 20 [[Paper]](https://www.usenix.org/system/files/osdi20-nakandala.pdf)
* Interstellar: Using Halide’s Scheduling Language to Analyze DNN Accelerators, ASPLOS 20 [[Paper]](https://arxiv.org/pdf/1809.04070.pdf)
* Rammer: Enabling Holistic Deep Learning Compiler Optimizations with rTasks,	OSDI 20	[[Paper]](https://www.usenix.org/system/files/osdi20-ma.pdf)		
* FlexTensor: An Automatic Schedule Exploration and Optimization Framework for Tensor Computation on Heterogeneous System, ASPLOS 20 [[Paper]](https://ceca.pku.edu.cn/docs/20200915213803856105.pdf)
* Ansor: Generating High-Performance Tensor Programs for Deep Learning,	OSDI	20	[[Paper]](https://www.usenix.org/system/files/osdi20-zheng.pdf)			
* MNN: A Universal and Efficient Inference Engine, MLSys 20 [[Paper]](https://arxiv.org/pdf/2002.12418)
* Astra: Exploiting Predictability to Optimize Deep Learning, ASPLOS 19 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2019/02/astra-asplos19.pdf)
* Bridging the Gap Between Neural Networks and Neuromorphic Hardware with A Neural Network Compiler, ASPLOS 18 [[Paper]](https://arxiv.org/pdf/1801.00746.pdf)
* CapeVM: A Safe and Fast Virtual Machine for Resource-Constrained Internet-of-Things Devices, SenSys 18 [[Paper]](https://dl.acm.org/doi/10.1145/3274783.3274842) (No ML)
* TVM: An Automated End-to-End Optimizing Compiler for Deep Learning, OSDI 18	[[Paper]](https://www.usenix.org/conference/osdi18/presentation/chen)	

<a name="networking-and-communication"></a>
## 📶 Networking and Communication (324)

<a name="user-content-battery"></a>
### Battery-powered Networking and Communication (225)
<a name="user-content-cellular"></a>
#### Cellular/Mobile Networks (Total: 48 | No ML(37) | ML(4) | DL(7)
* Scalable Distributed Massive MIMO Baseband Processing, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-gong.pdf) (No ML)
* DChannel: Accelerating Mobile Applications With Parallel High-bandwidth and Low-latency Channels, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-sentosa.pdf) (No ML)
* NeRF2: Neural Radio-Frequency Radiance Fields, MobiCom 23 [[Paper]](https://arxiv.org/pdf/2305.06118) (DL)
* Enabling Resilience in Virtualized RANs with Atlas, MobiCom 23 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2023/09/atlas_mobicom.pdf) (No ML)
* X-Plane: A High-Throughput Large-Capacity 5G UPF, MobiCom 23 [[Paper]](https://jhc.sjtu.edu.cn/~bjiang/papers/Liu_MobiCom2023_X-Plane.pdf) (No ML)
* CoreKube: An Efficient, Autoscaling and Resilient Mobile Core System, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3592522) [[Code]](https://github.com/netsys-edinburgh/CoreKube) (No ML) (Best Artifact Award)
* CA++: Enhancing Carrier Aggregation Beyond 5G, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592500) (No ML)
* Taking 5G RAN Analytics and Control to a New Level, MobiCom 23 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2022/12/JanusTechnicalReport.pdf) (No ML)
* Towards Ultra-low Power OFDMA Downlink Demodulation, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568509) (No ML)
* Warm-started quantum sphere decoding via reverse annealing for massive IoT connectivity, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560516) (No ML)
* Vivisecting Mobility Management in 5G Cellular Networks, SIGCOMM 22 [[Paper]](https://ahmadhassandebugs.github.io/assets/pdf/vivisectingmobility_sigcomm22.pdf) (No ML)
* Mobile Access Bandwidth in Practice: Measurement, Analysis, and Implications, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3544216.3544237) (No ML)
* Understanding 5G Performance for Real-world Services: a Content Provider’s Perspective, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3544216.3544219) (No ML)
* L25GC: A Low Latency 5G Core Network based on High-Performance NFV Platforms, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3544216.3544267) (No ML)
* Global Mobile Network Aggregators: Taxonomy, Roaming Performance and Optimization, MobiSys 22 [[Paper]](https://www.aqualab.cs.northwestern.edu/wp-content/uploads/2022/05/SAlcala-Marin-Mobisys22.pdf) (No ML)
* DeepRadar: A Deep-Learning-based Environmental Sensing Capability Sensor Design for CBRS, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3448632) (DL)
* FIRE: Enabling Reciprocity for FDD MIMO Systems, MobiCom 21 [[Paper]](https://deepakv.web.illinois.edu/assets/papers/FIRE_Mobicom2021.pdf) (DL)
* Nervion: A Cloud Native RAN Emulator for Scalable and Flexible Mobile Core Evaluation, MobiCom 21 [[Paper]](https://www.pure.ed.ac.uk/ws/portalfiles/portal/224348439/Nervion_LARREA_DOA13082021_AFV.pdf) (No ML)
* FSA: Fronthaul Slicing Architecture for 5G using dataplane programmable switches, MobiCom 21 [[Paper]](https://www.comp.nus.edu.sg/~chanmc/papers-by-year/2021-FSA.pdf) (No ML)
* Auric: Using Data-driven Recommendation to Automatically Generate Cellular Configuration, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472906.pdf) (DL)
* A Variegated Look at 5G in the Wild: Performance, Power, and QoE Implications, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472923.pdf)[[code]](https://github.com/SIGCOMM21-5G/artifact) (DL)
* A Nationwide Study on Cellular Reliability: Measurement, Analysis, and Enhancements, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472908.pdf) (No ML)
* Democratizing Cellular Access with CellBricks, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3473336.pdf) (No ML)
* Device-Based LTE Latency Reduction at the Application Layer, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-tan.pdf) (No ML)
* Challenge: COSMOS: A City-Scale Programmable Testbed for Experimentation with Advanced Wireless, MobiCom 20 [[Paper]](https://www.winlab.rutgers.edu/~sumitm/downloads/MobiCom2020_COSMOS.pdf) (No ML)
* DMM: Fast Map Matching for Cellular Data, MobiCom 20 [[Paper]](https://sites.ucmerced.edu/files/wdu/files/20mobicom-dmm.pdf) (DL)
* Microscope: Mobile Service Traffic Decomposition for Network Slicing as a Service, MobiCom 20 [[Paper]](https://core.ac.uk/download/pdf/334415278.pdf) (DL)
* A Low Latency and Consistent Cellular Control Plane, SIGCOMM 20 [[Paper]](https://web.lums.edu.pk/~zafar/sigcomm2020.pdf) (No ML)
* Understanding Operational 5G: A First Measurement Study on Its Coverage, Performance and Energy Consumption, SIGCOMM 20 [[Paper]](http://xyzhang.ucsd.edu/papers/DXu_SIGCOMM20_5Gmeasure.pdf) (No ML)
* Beyond 5G: Reliable Extreme Mobility Management, SIGCOMM 20 [[Paper]](http://www.yuanjiel.com/publication/sigcomm20.pdf) (No ML)
* A Systematic Way to LTE Testing, MobiCom 19 [[Paper]](https://people.computing.clemson.edu/~jmarty/projects/lowLatencyNetworking/papers/3GPP/LTE/AsystematicWayToMeasureLTE.pdf) (No ML)
* Detecting if LTE is the Bottleneck with BurstTracker, MobiCom 19 [[Paper]](https://cseweb.ucsd.edu/~schulman/docs/mobicom19-bursttracker.pdf) (No ML)
* Experiences: Design, Implementation, and Deployment of CoLTE, a Community LTE Solution, MobiCom 19 [[Paper]](https://kurti.sh/pubs/CoLTE_Mobicom_2019.pdf) (No ML)
* An Active-Passive Measurement Study of TCP Performance over LTE on High-speed Rails, MobiCom 19 [[Paper]](https://arxiv.org/pdf/1812.04823.pdf) (No ML)
* Bridging the Data Charging Gap in the Cellular Edge, SIGCOMM 19 [[Paper]](http://www.yuanjiel.com/publication/sigcomm19-camera-ready.pdf) (No ML)
* An In-depth Study of Commercial MVNO: Measurement and Optimization, MobiSys 19 [[Paper]](https://www.cs.binghamton.edu/~yaoliu/publications/mobisys19-mvno.pdf) (ML)
* CASTLE over the Air: Distributed Scheduling for Cellular Data Transmissions, MobiSys 19 [[Paper]](https://research.ece.cmu.edu/lions/Papers/CASTLE_MobiSys.pdf) (ML)
* How Should I Slice My Network? A Multi-Service Empirical Evaluation of Resource Sharing Efficiency, MobiCom 18 [[Paper]](https://core.ac.uk/download/pdf/288500453.pdf) (No ML)
* Mitigating the Latency-Accuracy Trade-off in Mobile Data Analytics Systems, MobiCom 18 [[Paper]](https://symbioticlab.org/publications/files/cellscope:mobicom18/cellscope-mobicom18.pdf) (ML)
* A reliable distributed cellular core network for hyper-scale public clouds, MobiCom 18 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2018/07/ECHO-Mobicom.pdf) (No ML)
* Chorus: Truly Distributed Distributed-MIMO, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230578) (No ML)
* Experience: Automating Diagnosis of Cellular Radio Access Network Problems, MobiCom 17 [[Paper]](https://www.cs.columbia.edu/~lierranli/publications/cellscope_mobicom17.pdf) (ML)
* A High Performance Packet Core for Next Generation Cellular Networks, SIGCOMM 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3098822.3098848) (No ML)
* QuickC: Practical sub-millisecond transport for small cells, MobiCom 16 [[Paper]](https://web.stanford.edu/~skatti/pubs/mobicom16-quickc.pdf) (No ML)
* LTE in Unlicensed Spectrum: Are We There Yet?, MobiCom 16 [[Paper]](http://www.cs.albany.edu/~mariya/courses/csi445660F16/papers/p135-chai.pdf) (No ML)
* Proteus: a network service control platform for service evolution in a mobile software defined infrastructure, MobiCom 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2973750.2973757) (No ML)
* Eliminating Channel Feedback in Next-Generation Cellular Networks, SIGCOMM 16 [[Paper]](https://dl.acm.org/doi/10.1145/2934872.2934895) (No ML)
* iCellular: Device-Customized Cellular Network Access on Commodity Smartphones, NSDI 16 [[Paper]](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-li-yuanjie.pdf) (No ML)

<a name="user-content-wifi"></a>
#### Wi-Fi Networks (Total: 16 | No ML(12) | ML(1) | DL(3))
* RF-Diffusion: Radio Signal Generation via Time-Frequency Diffusion, MobiCom 24 [[Paper]](https://arxiv.org/pdf/2404.09140) (DL)
* SlimWiFi: Ultra-Low-Power IoT Radio Architecture Enabled by Asymmetric Communication, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-zhao-renjie.pdf) (No ML)
* SenCom: Integrated Sensing and Communication with Practical WiFi, MobiCom 23 [[Paper]](https://hyh6540.github.io/pdf/He_mobicom_2023_isac_wifi.pdf) (No ML)
* Upscaling Fog Computing in Oceans for Underwater Pervasive Data Science Using Low-Cost Micro-Clouds, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3575801) (DL)
* AiFi: AI-Enabled WiFi Interference Cancellation with Commodity PHY-Layer Information, SenSys 22 [[Paper]](https://sites.pitt.edu/~weigao/publications/sensys22.pdf) (DL)
* Mobile Access Bandwidth in Practice: Measurement, Analysis, and Implications, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3544216.3544237) (No ML)
* TransFi: Emulating Custom Wireless Physical Layer from Commodity WiFi, MobiSys 22 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobisys22.pdf) (No ML)
* MIXIQ: re-thinking ultra-low power receiver design for next-generation on-body applications, MobiCom 21 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/Mobicom21-MIXIQ.pdf) (No ML)
* RFlens: metasurface-enabled beamforming for IoT communication and sensing, MobiCom 21 [[Paper]](https://dl.acm.org/doi/10.1145/3447993.3483238) (No ML)
* On-Off Noise Power Communication, MobiCom 19 [[Paper]](https://span.engineering.wustl.edu/pub/lundrigan2019onoff.pdf) (No ML)
* CloseTalker: Secure, Short-Range Ad Hoc Wireless Communication, MobiSys 19 [[Paper]](https://www.cs.dartmouth.edu/~dfk/research/pierson-closetalker/pierson-closetalker.pdf) (No ML)
* SWAN: Stitched Wi-Fi ANtennas, MobiCom 18 [[Paper]](https://people.computing.clemson.edu/~jmarty/projects/lowLatencyNetworking/papers/new/swanStitchedWiFiAntennas.pdf) (No ML)
* FlexCore: Massively Parallel and Flexible Processing for Large MIMO Access Points, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-husmann.pdf) (No ML)
* Wi-Fi Goes to Town: Rapid Picocell Switching for Wireless Transit Networks, SIGCOMM 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3098822.3098846) (No ML)
* Real-time Distributed MIMO Systems, SIGCOMM 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2934872.2934905) (No ML)
* Characterizing and Improving WiFi Latency in Large-Scale Operational Networks, MobiSys 16 [[Paper]](http://zmy.io/files/mobisys16-WiFiSeer.pdf) (ML)

<a name="user-content-visible-Light"></a>
#### Visible Light Communication (Total: 17 | No ML(14) | ML(0) | DL(3))
* Practical Optical Camera Communication Behind Unseen and Complex Backgrounds, MobiSys 24, [[Paper]](https://dl.acm.org/doi/10.1145/3643832.3661866) (DL)
* When VLC Meets Under-Screen Camera, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596855) (No ML)
* Harmony: An In-band Time Synchronisation System for Visible Light Communication, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568549) (No ML)
* CORE-lens: simultaneous communication and object recognition with disentangled-GAN cameras, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560526) (DL)
* SpiderWeb: Enabling Through-Screen Visible Light Communication, SenSys 21 [[Paper]](https://pure.tudelft.nl/ws/portalfiles/portal/103302355/3485730.3485948.pdf) (No ML)
* DeepLight: Robust & Unobtrusive Real-time Screen-Camera Communication for Real-World Displays, IPSN 21 [[Paper]](https://arxiv.org/pdf/2105.05092.pdf) (DL)
* AIRCODE: Hidden Screen-Camera Communication on an Invisible and Inaudible Dual Channel, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-qian-kun.pdf) (No ML)
* RayTrack: enabling interference-free outdoor mobile VLC with dynamic field-of-view, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3466867) (No ML)
* RadioInLight: Doubling the Data Rate of VLC Systems, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483271) (No ML)
* Shrimp: a robust underwater visible light communication system, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448616) (No ML)
* Zero-Wire: A Deterministic and Low-Latency Wireless Bus Through Symbol-Synchronous Transmission of Optical Signals, SenSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3384419.3430897) (No ML) (Best Paper)
* Breaking the Limitations of Visible Light Communication Through Its Side Channel, SenSys 20 [[Paper]](https://pure.tudelft.nl/ws/files/85899111/Sensys20_breaking.pdf) (No ML)
* ChromaCode: A Fully Imperceptible Screen-Camera Communication System, MobiCom 18 [[Paper]](https://cswu.me/papers/mobicom18_chromacode_paper.pdf) (No ML)
* ReflexCode: Coding with Superposed Reflection Light for LED-Camera Communication, MobiCom 17 [[Paper]](https://dl.acm.org/doi/10.1145/3117811.3117836) (No ML)
* POLI: Long-Range Visible Light Communications Using Polarized Light Intensity Modulation, MobiSys 17 [[Paper]](https://dl.acm.org/doi/10.1145/3081333.3081353) (No ML)
* Card-stunt as a Service: Empowering a Massively Packed Crowd for Instant Collective Expressiveness, MobiSys 17 [[Paper]](https://nclab.kaist.ac.kr/uploads/2017/08/mobisys2017_cardstunt.pdf) (No ML)
* The DarkLight Rises: Visible Light Communication in the Dark, MobiCom 16 [[Paper]](https://www.cs.dartmouth.edu/~xia/papers/mobicom16-darklight.pdf) (No ML)

<a name="user-content-loralorawan"></a>
#### LoRa/LoRaWAN (Total: 24 | No ML(18) | ML(2) | DL(4))
* ChirpTransformer: Versatile LoRa Encoding for Low-power Wide-area IoT, MobiSys 24, [[Paper]](https://dl.acm.org/doi/10.1145/3643832.3661861) (DL)
* XCopy: Boosting Weak Links for Reliable LoRa Communication, MobiCom 23 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/XCopy-MobiCom23.pdf) (No ML)
* Enabling Concurrency for Non-orthogonal LoRa Channels, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613268) (No ML)
* Citywide LoRa Network Deployment and Operation: Measurements, Analysis, and Implications, SenSys 23 [[Paper]](http://tns.thss.tsinghua.edu.cn/~jiliang/publications/SenSys23-CityWAN.pdf) (No ML)
* OpenLoRa: Validating LoRa Implementations through an Extensible and Open-sourced Framework, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-mishra.pdf) (No ML)
* BSMA: scalable LoRa networks using full duplex gateways, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560544) (No ML)
* LLDPC: A Low-Density Parity-Check Coding Scheme for LoRa Networks, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568547) (DL)
* MaLoRaGW: Multi-User MIMO Transmission for LoRa, SenSys 22 [[Paper]](https://www.cse.msu.edu/~hzeng/papers/Hossein22_Sensys_MaLoRaGW.pdf) (No ML)
* HyLink: Towards High Throughput LPWANs with LoRa Compatible Communication, SenSys 22 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/HyLink-SenSys22.pdf) (No ML)
* CurvingLoRa to Boost LoRa Network Throughput via Concurrent Transmission, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-li_chenning.pdf) (No ML)
* PCube: Scaling LoRa Concurrent Transmissions with Reception Diversities, MobiCom 21 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/PCube-MobiCom21.pdf) (No ML)
* Combating link dynamics for reliable lora connection in urban settings, MobiCom 21 [[Paper]](https://dl.acm.org/doi/10.1145/3447993.3483250) (No ML)
* DeepLoRa: Learning accurate path loss model for long distance links in LPWAN, INFOCOM 21 [[Paper]](https://cse.msu.edu/~caozc/papers/infocom21-liu.pdf) (DL)
* OwLL: Accurate LoRa Localization using the TV Whitespaces, IPSN 21 [[Paper]](https://swarunkumar.com/papers/owll-ipsn2021.pdf) (No ML)
* STeC: Exploiting Spatial and Temporal Correlation for Event-based Communication in WSNs, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485951) (No ML)
* NELoRa: Towards Ultra-low SNR LoRa Communication with Neural-enhanced Demodulation, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485928) [[Code]](https://github.com/hanqingguo/NELoRa-Sensys) (DL)
* Concurrent Interference Cancellation: Decoding Multi-Packet Collisions in LoRa, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472931.pdf) (No ML)
* SateLoc: A Virtual Fingerprinting Approach to Outdoor LoRa Localization using Satellite Images, IPSN 20 [[Paper]](https://taogu.site/pub/paper/21-tosn-SateLoc.pdf) (ML)
* LMAC: efficient carrier-sense multiple access for LoRa, MobiCom 20 [[Paper]](https://chaojiegu.github.io/assets/pdf/LMAC-TOSN.pdf) (No ML)
* Exploring LoRa for Long-range Through-wall Sensing, IMWUT/UbiComp 20 [[Paper]](https://www.researchgate.net/publication/342190956_Exploring_LoRa_for_Long-range_Through-wall_Sensing) (No ML)
* Automated Estimation of Link Quality for LoRa: A Remote Sensing Approach, IPSN 19 [[Paper]](https://pure.tudelft.nl/ws/files/55547022/IPSN2019.pdf) (ML)
* LongShoT: Long-Range Synchronization of Time, IPSN 19 [[Paper]](https://par.nsf.gov/servlets/purl/10107899) (No ML)
* FTrack: parallel decoding for LoRa transmissions, SenSys 19 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/FTrack_Sensys19.pdf) (No ML)
* WIDESEE: Towards Wide-Area Contactless Wireless Sensing, SenSys 19 [[Paper]](https://zwang4.github.io/publications/sensys19.pdf) (No ML)

<a name="user-content-millimeter-Wave"></a>
#### mmWave Communication (Total: 25 | No ML(23) | ML(2) | DL(0))
* mmRipple: Communicating with mmWave Radars through Smartphone Vibration, IPSN 23 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/mmRipple_IPSN2023.pdf) (No ML)
* Bringing Millimeter Wave Technology to Any IoT Device, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613255) (No ML)
* SIGNiPHY: Reconciling random access with directional reception for efficient mmWave WLANs, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596860) (No ML)
* mmWall: A Steerable, Transflective Metamaterial Surface for NextG mmWave Networks, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-cho-kun-woo.pdf) (No ML)
* M5: Facilitating Multi-user Volumetric Content Delivery with Multi-lobe Multicast over mmWave, SenSys 22 [[Paper]](http://www.phpathak.com/files/m5-sensys.pdf) (ML)
* Two beams are better than one: Towards Reliable and High Throughput mmWave Links, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472924.pdf) (No ML)
* Practical Null Steering in Millimeter Wave Networks, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-madani.pdf) (No ML)
* SpaceBeam: LiDAR-driven one-shot mmWave beam management, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3466864) (ML)
* X-Array: Approximating Omnidirectional Millimeter-Wave Coverage Using an Array of Phased Arrays, MobiCom 20 [[Paper]](http://xyzhang.ucsd.edu/papers/SWang_MobiCom20_X-Array.pdf) (No ML)
* Millimeter-Wave Full Duplex Radios, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3380879) (No ML)
* M-Cube: a millimeter-wave massive MIMO software radio, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3380892) (No ML) (Best Paper Award)
* mm-FLEX: An Open Platform for Millimeter-Wave Mobile Full-Bandwidth Experimentation, MobiSys 20 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/808/MOBISYS_2020_FINAL.pdf?sequence=1&isAllowed=y) (No ML)
* KinPhy: a kinetic in-band channel for millimetre-wave networks, SenSys 19 [[Paper]](https://dl.acm.org/doi/10.1145/3356250.3360039) (No ML)
* A Millimeter Wave Network for Billions of Things, SIGCOMM 19 [[Paper]](http://web.cs.ucla.edu/~omid/Papers/Sigcomm19.pdf) (No ML)
* Many-to-Many Beam Alignment in Millimeter Wave Networks, NSDI 19 [[Paper]](https://www.usenix.org/system/files/nsdi19-jog.pdf) (No ML)
* LiSteer: mmWave Beam Acquisition and Steering by Tracking Indicator LEDs on Wireless APs, MobiCom 18 [[Paper]](https://dl.acm.org/doi/10.1145/3241539.3241542) (No ML)
* Multi-Stream Beam-Training for mmWave MIMO Networks, MobiCom 18 [[Paper]](https://cse.buffalo.edu/faculty/dimitrio/publications/mobicom18_mute.pdf) (No ML)
* Towards Scalable and Ubiquitous Millimeter-Wave Wireless Networks, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241579) (No ML)
* Adaptive Codebook Optimization for Beam Training on Off-the-Shelf IEEE 802.11ad Devices, MobiCom 18 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/614/Adaptive_Codebook_Optimization_Beam_Training_Off-the-Shelf_IEEE%20802.11ad_Devices_2018_EN.pdf?sequence=1&isAllowed=y) (No ML)
* Fast Millimeter Wave Beam Alignment, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230581) (No ML)
* WiFi-Assisted 60 GHz Wireless Networks, MobiCom 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3117811.3117817) (No ML)
* Pose Information Assisted 60 GHz Networks: Towards Seamless Coverage and Mobility Support, MobiCom 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3117811.3117832) (No ML)
* Facilitating Robust 60 GHz Network Deployment by Sensing Ambient Reflectors, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-wei-teng.pdf) (No ML)
* OpenMili: A 60 GHz Software Radio Platform With a Reconfigurable Phased-Array Antenna, MobiCom 16 [[Paper]](http://xyzhang.ucsd.edu/papers/JZhang_MobiCom16_OpenMili.pdf) (No ML)
* BeamSpy: Enabling Robust 60 GHz Links Under Blockage, NSDI 16 [[Paper]](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-sur.pdf) (No ML)

<a name="user-content-lpwan"></a>
#### LPWAN (Total: 13  | No ML(12) | ML(0) | DL(1))
* Low-Bandwidth Self-Improving Transmission of Rare Training Data, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613300) (DL)
* FLoRa: Energy-Efficient, Reliable, and Beamforming-Assisted Over-The-Air Firmware Update in LoRa Networks, IPSN 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3583120.3586963) (No ML)
* Link Quality Modeling for LoRa Networks in Orchards, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586969) (No ML)
* LoPhy: A Resilient and Fast Covert Channel over LoRa PHY, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586952) (No ML)
* Seirios: Leveraging Multiple Channels for LoRaWAN Indoor and Outdoor Localization, MobiCom 21 [[Paper]](https://arxiv.org/pdf/2108.06884.pdf) (No ML)
* Frequency Configuration for Low-Power Wide-Area Networks in a Heartbeat, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-gadre.pdf) (No ML)
* Joltik: Enabling Energy-Efficient “Future-Proof” Analytics on Low-Power Wide-Area Networks, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419204) (No ML)
* Nephalai: Towards LPWAN C-RAN with Physical Layer Compression, MobiCom 20 [[Paper]](https://arxiv.org/pdf/2008.02599.pdf) (No ML)
* WiChronos: energy-efficient modulation for long-range, large-scale wireless networks, MobiCom 20 [[Paper]](https://uwconnect.ece.wisc.edu/wp-content/uploads/sites/1525/2021/10/WiChronos.pdf) (No ML)
* A Cloud-Optimized Link Layer for Low-Power Wide-Area Networks, MobiSys 20 [[Paper]](https://users.ece.cmu.edu/~agr/resources/publications/mobisys_20_opr.pdf) (No ML)
* Combating Packet Collisions Using Non-Stationary Signal Scaling in LPWANs, MobiSys 20 [[Paper]](http://tns.thss.tsinghua.edu.cn/~jiliang/publications/MOBISYS2020_NSCALE.pdf) (No ML)
* Challenge: Unlicensed LPWANs Are Not Yet the Path to Ubiquitous Connectivity, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345444) (No ML) 
* Data Prediction + Synchronous Transmissions = Ultra-low Power Wireless Sensor Networks, SenSys 16 [[Paper]](https://disi.unitn.it/~picco/papers/sensys16.pdf) (No ML)

<a name="user-content-sdr"></a>
#### SDR (Total: 7 | No ML(7) | ML(0) | DL(0))
* RFClock: Timing, Phase and Frequency Synchronization for Distributed Wireless Networks, MobiCom 21 [[Paper]](https://genesys-lab.org/papers/RFCLOCK_MOBICOM2021.pdf) (No ML)
* TyrLoc: a low-cost multi-technology MIMO localization system with a single RF chain,	MobiSys	21	[[Paper]](http://medianet.azurewebsites.net/wp-content/uploads/2023/02/tyrloc2021.pdf) (No ML)
* SDR receiver using commodity wifi via physical-layer signal reconstruction, MobiCom 20 [[Paper]](https://seit.egr.msu.edu/paper/Mobicom2020-SDRLite.pdf) (No ML)
* TinySDR: Low-Power SDR Platform for Over-the-Air Programmable IoT Testbeds, NSDI 20 [[Paper]](https://www.usenix.org/conference/nsdi20/presentation/hessar) (No ML)
* SparSDR: Sparsity-proportional Backhaul and Compute for SDRs, MobiSys 19 [[Paper]](http://people.csail.mit.edu/moein/papers/sparsdr-mobisys19.pdf) (No ML)
* Towards Programming the Radio Environment with Large Arrays of Inexpensive Antennas, NSDI 19 [[Paper]](https://www.usenix.org/system/files/nsdi19-li-zhuqi.pdf) (No ML)
* The Tick Programmable Low-Latency SDR System, MobiCom 17 [[Paper]](http://metro.cs.ucla.edu/papers/mobicom17-tick.pdf) (No ML) (Best Community Paper Award)

<a name="user-content-ctc"></a>
#### CTC (Total: 23 | No ML(22) | ML(0) | DL(1))
* RF-SIFTER: Sifting Signals at Layer-0.5 to Mitigate Wideband Cross-Technology Interference for IoT, MobiCom 23 [[Paper]](https://www.cs.cityu.edu.hk/~jhuan9/papers/rfsifter23mobicom.pdf) (No ML)
* Unify: Turning BLE/FSK SoC into WiFi SoC, MobiCom 23 [[Paper]](https://rtcl.eecs.umich.edu/rtclweb/assets/publications/2023/mobicom23-cho.pdf) (No ML)
* XiTuXi: Sealing the Gaps in Cross-Technology Communication by Neural Machine Translation, Sensys 23 [[Paper]](https://dl.acm.org/doi/10.1145/3625687.3625802) (DL)
* WibZig: Reliable and Commodity-device Compatible PHY-CTC via Chip Emulation in Phase, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3587046) (No ML)
* mmRipple: Communicating with mmWave Radars through Smartphone Vibration, IPSN 23 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/mmRipple_IPSN2023.pdf) (No ML)
* Towards Seamless Wireless Link Connection, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596833) (No ML)
* FLEW: Fully Emulated WiFi, MobiCom 22 [[Paper]](https://rtcl.eecs.umich.edu/rtclweb/assets/publications/2022/mobicom22-cho.pdf) (No ML)
* De-spreading over the air: long-range CTC for diverse receivers with LoRa, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560524) (No ML)
* TinyNet: a Lightweight, Modular, and Unified Network Architecture for the Internet of Things, MobiSys 22 [[Paper]](https://desword.github.io/assets/pdf/mobisys22-tinynet.pdf) (No ML)
* WiBeacon: Expanding BLE Location-based Services via WiFi, MobiCom 21 [[Paper]](https://liux4189.github.io/files/WiBeacon_MobiCom_CameraReady.pdf) (No ML)
* BlueFi: Bluetooth over WiFi, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472920.pdf) (No ML)
* X-MIMO: Cross-Technology Multi-User MIMO, SenSys 20 [[Paper]](https://par.nsf.gov/servlets/purl/10303948) (No ML)
* Parallel Inclusive Communication for Connecting Heterogeneous IoT Devices at the Edge, SenSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3356250.3360046) (No ML)
* LTE2B: Time-Domain Cross-Technology Emulation under LTE Constraints, SenSys 19 [[Paper]](https://liux4189.github.io/files/LTE2B_Sensys_CameraReady.pdf) (No ML)
* Exploiting WiFi Guard Band for Safeguarded ZigBee, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274835) (No ML)
* Cross-Frequency Communication: Near-Field Identification of UHF RFIDs with WiFi!, MobiCom 18 [[Paper]](https://www4.comp.polyu.edu.hk/~csyanglei/data/files/tifi-mobicom18.pdf) (No ML)
* Achieving Receiver-Side Cross-Technology Communication with Cross-Decoding, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241547) (No ML)
* Explicit Channel Coordination via Cross-technology Communication, MobiSys 18 [[Paper]](https://par.nsf.gov/servlets/purl/10076616) (No ML)
* Chiron: Concurrent High Throughput Communication for IoT Devices, MobiSys 18 [[Paper]](https://cis.csuohio.edu/~chi/publication/li-2018-cch-3210240-3210346/li-2018-cch-3210240-3210346.pdf) (No ML)
* Networking across boundaries: enabling wireless communication through the water-air interface SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/10.1145/3230543.3230580) (No ML)
* BlueBee: a 10,000x Faster Cross-Technology Communication via PHY Emulation, SenSys 17 [[Paper]](https://cs.gmu.edu/~song/paper/SenSys17_Wenchao.pdf) (No ML)
* WEBee: Physical-Layer Cross-Technology Communication via Emulation, MobiCom 16 [[Paper]](https://www-users.cse.umn.edu/~tianhe/Papers/WEBee.pdf) (No ML) (Best Paper Awards)
* B2W2: N-Way Concurrent Communication for IoT Devices, SenSys 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2994551.2994561) (No ML)

<a name="user-content-bluetooth"></a>
#### Bluetooth (Total: 4 | No ML(4) | ML(0) | DL(0))
* BLEX: Flexible Multi-Connection Scheduling for Bluetooth Low Energy, IPSN 21 [[Paper]](https://www.researchgate.net/publication/350524841_BLEX_Flexible_Multi-Connection_Scheduling_for_Bluetooth_Low_Energy) (No ML）
* enClosure: Group Communication via Encounter Closures, MobiSys 19 [[Paper]](https://people.mpi-sws.org/~druschel/publications/enclosure.pdf) (No ML)
* BLEach: Exploiting the Full Potential of IPv6 over BLE in Constrained Embedded IoT Devices, SenSys 17 [[Paper]](https://nes-lab.org/wordpress/wp-content/uploads/2019/11/spoerk17bleach.pdf) (No ML)
* Beetle: Flexible Communication for Bluetooth Low Energy, MobiSys 16 [[Paper]](http://iot.stanford.edu/pubs/beetle-mobisys16.pdf) (No ML)

<a name="user-content-uwb"></a>
#### UWB (Total: 5 | No ML(5) | ML(0) | DL(0))
* Network On or Off? Instant Global Binary Decisions over UWB with Flick, IPSN 23 [[Paper]](http://disi.unitn.it/~picco/papers/ipsn23.pdf) (No ML)
* WISE: Low-Cost Wide Band Spectrum Sensing Using UWB, SenSys 22 [[Paper]](https://huangqy7.github.io/Paper/WISE_final.pdf) (No ML)
* Understanding and Mitigating the Impact of Wi-Fi 6E Interference on Ultra-Wideband Communications and Ranging, IPSN 22 [[Paper]](http://www.carloalbertoboano.com/documents/brunner22uwbwifi.pdf) (No ML)
* Octopus: a practical and versatile wideband MIMO sensing platform, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483267) (No ML)
* One Flood to Route Them All:Ultra-fast Convergecast of Concurrent Flows over UWB, SenSys 20 [[Paper]](http://disi.unitn.it/~picco/papers/sensys20_weaver.pdf) (No ML)

<a name="user-content-tv-whitespace"></a>
#### TV Whitespace (Total: 5 | No ML(5) | ML(0) | DL(0))
* Whisper: IoT in the TV White Space Spectrum, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-chakraborty.pdf) (No ML)
* OwLL: Accurate LoRa Localization using the TV Whitespaces, IPSN 21 [[Paper]](https://swarunkumar.com/papers/owll-ipsn2021.pdf) (No ML)
* WhiteHaul: An Efficient Spectrum Aggregation System for Low-Cost and High Capacity Backhaul over White Spaces, MobiSys 20 [[Paper]](https://discovery.ucl.ac.uk/id/eprint/10114386/10/Kheirkhah_WhiteHaul_mobisys20.pdf) (No ML)
* Enabling Reliable, Asynchronous, and Bidirectional Communication in Sensor Networks over White Spaces, SenSys 17 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2018/02/sensys17.pdf) (No ML)
*  SNOW: Sensor Network over White Spaces, SenSys 16 [[Paper]](https://www.cse.wustl.edu/~lu/papers/sensys16.pdf) (No ML)

<a name="user-content-acoustic"></a>
#### Acoustic Communication (Total:9  | No ML(8) | ML(0) | DL(1))
* Towards Spatial Selection Transmission for Low-end IoT devices with SpotSound, MobiCom 23 [[Paper]](https://tachen-cs.github.io/data/papers/2023-mobicom-spotsound/SpotSound.pdf) (DL)
* AquaHelper: Underwater SOS Transmission and Detection in Swimming Pools, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625816) (No ML)
* Underwater Messaging Using Mobile Devices, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3544216.3544258)[[Code]](https://github.com/uw-x/watercomms) (No ML)
* Shrimp: a robust underwater visible light communication system, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3448616) (No ML)	
* Deaf-aid: mobile IoT communication exploiting stealthy speaker-to-gyroscope channel, MobiCom 20 [[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-mobicom2020c.pdf) (No ML)
* BatComm: Enabling Inaudible Acoustic Communication with High-throughput for Mobile Devices, SenSys 20 [[Paper]](https://web.eecs.utk.edu/~jliu/publications/bai2020batcomm.pdf) (No ML)
* AmphiLight: Direct Air-Water Communication with Laser Light, NSDI 20 [[Paper]](https://www.usenix.org/conference/nsdi20/presentation/carver) (No ML)
* Messages Behind the Sound: Real-Time Hidden Acoustic Signal Capture with Smartphones, MobiCom 16 [[Paper]](https://cse.buffalo.edu/~lusu/papers/MobiCom2016.pdf) (No ML)
* Near-Ultrasound Communication for TV's 2nd Screen Services,  MobiCom 16 [[Paper]](https://dl.acm.org/doi/10.1145/2973750.2973774) (No ML)
  
<a name="user-content-other-multi-band"></a>
#### Multi-band Operation (Total: 4 | No ML(4) | ML(0) | DL(0))
* A real-time experimentation platform for sub-6 GHz and millimeter-wave MIMO systems, MobiSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3458864.3466868) [[Code]](https://github.com/rafaruizortiz/MIMORPH) (No ML)
* MPBond: Efficient Network-level Collaboration Among Personal Mobile Devices, MobiSys 20 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/mpbond_mobisys20.pdf) (No ML)
* MuSher: An Agile Multipath-TCP Scheduler for Dual-Band 802.11ad/ac Wireless LANs, MobiCom 19 [[Paper]](https://cse.buffalo.edu/faculty/dimitrio/publications/mobicom19.pdf) (No ML)
* An In-depth Understanding of Multipath TCP on Mobile Devices: Measurement and System Design, MobiCom 16 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/multipath_mobicom16.pdf) (No ML)

<a name="user-content-other-sensor-network"></a>
#### Other Networks (Total: 25 | No ML(21) | ML(2) | DL(2))
* Everything has its Bad Side and Good Side: Turning Processors to Low Overhead Radios Using Side-Channels, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586959) (No ML)
* mmRipple: Communicating with mmWave Radars through Smartphone Vibration, IPSN 23 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/mmRipple_IPSN2023.pdf) (No ML)
* Hydra: Concurrent Coordination for Fault-tolerant Networking, IPSN 23 [[Paper]](https://www.research-collection.ethz.ch/bitstream/handle/20.500.11850/602741/7/3583120.3587047.pdf) (No ML)
* NeuroRadar: A Neuromorphic Radar Sensor for Low-Power IoT Systems, SenSys 23 [[Paper]](http://xyzhang.ucsd.edu/papers/Kai.Zheng_SenSys23_NeuroRadar.pdf) (ML)
* Sirius: A Self-Localization System for Resource-Constrained IoT Sensors, MobiSys 23 [[Paper]](https://www.cs.umd.edu/~nakul/assets/papers/sirius_mobisys2023_nakul.pdf) (DL)
* A Case for Stateless Mobile Core Network Functions in Space, SIGCOMM 22 [[Paper]](http://www.yuanjiel.com/publication/sigcomm22.pdf) (No ML)
* Adapting Wireless Mesh Network Configuration from Simulation to Reality via Deep Learning based Domain Adaptation, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-shi.pdf) (DL)
* A Community-Driven Approach to Democratize Access to Satellite Ground Stations, MobiCom 21 [[Paper]](https://swarunkumar.com/papers/quasar-mobicom2021.pdf) (No ML)
* COCOON-A Conductive Substrate-based Coupled Oscillator Network for Wireless Communication, SenSys 21 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/SenSys21-COCOON.pdf) (No ML)
* STeC: Exploiting Spatial and Temporal Correlation for Event-based Communication in WSNs, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485951) (No ML)
* LAVA: fine-grained 3D indoor wireless coverage for small IoT devices, SIGCOMM 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3452296.3472890) (No ML)
* Performant TCP for Low-Power Wireless Networks, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-kumar.pdf) (LLNs) (No ML)
* Understanding and Embracing the Complexities of the Molecular Communication Channel in Liquids, MobiCom 20 [[Paper]](https://haitham.ece.illinois.edu/Papers/BioMC.pdf) (ML)
* SkySense: Terrestrial and Aerial Spectrum Use Analysed Using Lightweight Sensing Technology with Weather Balloons, MobiSys 20 [[Paper]](https://www.lenders.ch/publications/conferences/mobisys20.pdf) (No ML)
* Blind Distributed MU-MIMO for IoT Networking over VHF Narrowband Spectrum, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345427) (No ML)
* NEOFog: Nonvolatility-Exploiting Optimizations for Fog Computing, ASPLOS 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3173162.3177154) (No ML)
* Mixer: Efficient Many-to-All Broadcast in Dynamic Wireless Mesh Networks, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274849) (No ML) (in principle Mixer works on any physical layer that features the capture effect)
* System Architecture Directions for Post-SoC/32-bit Networked Sensors, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274839) (No ML) (Best Paper Runner-up)
* Surface MIMO: Using Conductive Surfaces For MIMO Between Small Devices, MobiCom 18 [[Paper]](https://arxiv.org/pdf/1809.02726.pdf) (No ML)
* MagneComm: Magnetometer-based Near-Field Communication, MobiCom 17 [[Paper]](https://www.cs.sjtu.edu.cn/~yichao/pmwiki/assets/publications/mobicom17_pan.pdf) (No ML)
* Empowering Low-Power Wide Area Networks in Urban Settings, SIGCOMM 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3098822.3098845) (No ML)
* Network-wide Consensus Utilizing the Capture Effect in Low-power Wireless Networks, SenSys 17 [[Paper]](http://www.diva-portal.org/smash/get/diva2:1170407/FULLTEXT01.pdf) (No ML)
* Staffetta: Smart Duty-Cycling for Opportunistic Data Collection, SenSys 16 [[Paper]](https://www.st.ewi.tudelft.nl/marco/files/staffetta_Sensys16.pdf) (No ML)
* Effectively Capturing Attention Using the Capture Effect, SenSys 16 [[Paper]](https://tik-db.ee.ethz.ch/file/b468db98c89b23c868db49b3e72817d0/paper-sp.pdf) (No ML)
* Ripple II: Faster Communication through Physical Vibration, NSDI 16 [[Paper]](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-roy.pdf) (No ML)

<a name="user-content-batteryless"></a>
### Batteryless Networking and Communication (99)
<a name="user-content-wifi-1"></a>
#### Wi-Fi Networks (Total: 16 | No ML(16) | ML(0) | DL(0))
* Leggiero: Analog WiFi Backscatter with Payload Transparency, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596835) (No ML)
* Timespan-based Backscatter Using a Single COTS Receiver, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596858) (No ML)
* RF-Bouncer: A Programmable Dual-band Metasurface for Sub-6 Wireless Networks, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-li-xinyi.pdf) (No ML)
* Content-agnostic backscatter from thin air, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538930) (No ML)
* SyncScatter: Enabling WiFi like synchronization and range for WiFi backscatter Communication, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-dunna.pdf) (No ML)
* Verification and Redesign of OFDM Backscatter, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-liu-xin.pdf) (No ML)
* Verification: Can WiFi Backscatter replace RFID?, MobiCom 21 [[Paper]](https://cs.uwaterloo.ca/~brecht/papers/wifi-vs-rfid-mobicom-2021.pdf) (No ML)
* VMscatter: A Versatile MIMO Backscatter, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-liu.pdf) (No ML)
* ScatterMIMO: Enabling Virtual MIMO with Smart Surfaces, MobiCom 20 [[Paper]](https://wcsng.ucsd.edu/files/scattermimo.pdf) (No ML)
* WiTAG: Seamless WiFi Backscatter Communication, SIGCOMM 20 [[Paper]](https://cs.uwaterloo.ca/~brecht/papers/witag-sigcomm-2020.pdf) (No ML)
* OFDMA-Enabled Wi-Fi Backscatter,MobiCom 19 [[Paper]](https://renjiezhao.github.io/files/OFDMA_BS_paper.pdf) (No ML)
* X-Tandem: Towards Multi-hop Backscatter Communication with Commodity WiFi, MobiCom 18 [[Paper]](https://www2.cs.sfu.ca/~jcliu/Papers/MobiCom-18-X-Tandem.pdf) (No ML)
* Spatial Stream Backscatter Using Commodity WiFi, MobiSys 18 [[Paper]](https://www2.cs.sfu.ca/~jcliu/Papers/mobisys18-Liu.pdf) (No ML)
* Passive Wi-Fi: Bringing Low Power to Wi-Fi Transmissions, NSDI 16 [[Paper]](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-kellogg.pdf) (No ML) (Best Paper)
* HitchHike: Practical Backscatter Using Commodity WiFi, SenSys 16 [[Paper]](https://pengyuzhang.github.io/papers/sensys16_back_comm.pdf) (No ML)
* Enabling Practical Backscatter Communication for On-body Sensors, SIGCOMM 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2934872.2934901) (No ML)

<a name="user-content-visible-Light-1"></a>
#### Visible Light Communication (Total: 12 | No ML(10) | ML(0) | DL(2))
* SpectraLux: Towards Exploiting a Broader Spectrum with Passive VLC, IPSN 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3583120.3586966) (DL)
* U-star: an underwater navigation system based on passive 3D optical identification tags, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517019) (DL)
* Exploiting Digital Micro-Mirror Devices for Ambient Light Communication, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-xu_talia.pdf) (No ML)
* Low-Latency Visible Light Backscatter Networking with RetroMUMIMO, SenSys 22 [[Paper]](https://soar.group/pubs/RetroMUMIMO.SenSys22.pdf) (No ML)
* PassiveLiFi: Rethinking LiFi for Low-Power and Long Range RF Backscatter, MobiCom 21 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/1541/Mobicom_PassiveLiFi_authors_version.pdf?sequence=1) (No ML)
* A Principled Design for Passive Light Communication, MobiCom 21 [[Paper]](https://www.st.ewi.tudelft.nl/marco/files/chromalux_Mobicom21.pdf) (No ML)
* Two to Tango: Hybrid Light and Backscatter Networks for Next Billion Devices, MobiSys 20 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/811/tosubmit.pdf?sequence=1) (No ML)
* Turboboosting Visible Light Backscatter Communication, SIGCOMM 20 [[Paper]](https://ceca.pku.edu.cn/docs/20200826153441008514.pdf) (No ML)
* LuxLink: creating a wireless link from ambient light, SenSys 19 [[Paper]](https://www.st.ewi.tudelft.nl/marco/files/luxlink_Sensys19.pdf) (No ML)
* Charging a Smartphone Across a Room Using Lasers, UbiComp 18 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/laserpower.pdf)	(No ML)
* PassiveVLC: Enabling Practical Visible Light Backscatter Communication for Battery-free IoT Applications, MobiCom 17 [[Paper]](https://ceca.pku.edu.cn/media/lw/63a22162bb427709099f765883bf243b.pdf) (No ML)
* Focus: Robust Visual Codes for Everyone, MobiSys 16 [[Paper]](https://user.it.uu.se/~eding810/conferences/Mobisys16.pdf) (No ML)

<a name="user-content-lora"></a>
#### LoRa/LoRaWAN (Total: 8 | No ML(8) | ML(0) | DL(0))
* LocRa: Enable Practical Long-Range Backscatter Localization for Low-Cost Tags, MobiSys 23 [[Paper]](https://dl.acm.org/doi/10.1145/3581791.3596863) (No ML)
* Long-Range Ambient LoRa Backscatter with Parallel Decoding, MobiCom 21 [[Paper]](http://tns.thss.tsinghua.edu.cn/~jiliang/publications/MOBICOM21-p2lora.pdf) (No ML)
* Saiyan: Design and Implementation of a Low-power Demodulator for LoRa Backscatter Systems, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-guo.pdf) (No ML)	
* Sense Me on the Ride: Accurate Mobile Sensing over a LoRa Backscatter Channel, SenSys 21 [[Paper]](https://tns.thss.tsinghua.edu.cn/sun/members/XiuzhenGuo/palantir_confer.pdf) (No ML)
* Simplifying Backscatter Deployment: Full-Duplex LoRa Backscatter, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-katanbaf.pdf) (No ML)
* Aloba: Rethinking ON-OFF Keying Modulation for Ambient LoRa Backscatter, SenSys 20 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/aloba_2020.pdf) (No ML)
* PLoRa: A Passive Long-Range Data Network from Ambient LoRa Transmissions, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230567) (No ML)
* LoRa Backscatter: Enabling The Vision of Ubiquitous Connectivity, UbiComp 17 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/loRaBackscatter.pdf)	(No ML)

<a name="user-content-millimeter-Wave-1"></a>
#### mmWave Communication (Total: 6 | No ML(6) | ML(0) | DL(0))
* UniScatter: a Metamaterial Backscatter Tag for Wideband Joint Communication and Radar Sensing, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592526) (No ML)
* LeakyScatter: A Frequency-Agile Directional Backscatter Network Above 100 GHz, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-kludze.pdf) (No ML)
* A Millimeter Wave Backscatter Network for Two-Way Communication and Localization, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3603269.3604873) (No ML)
* MilliMirror: 3D Printed Reflecting Surface for Millimeter-Wave Coverage Expansion, MobiCom 22 [[Paper]](http://xyzhang.ucsd.edu/papers/Kun.Qian_MobiCom22_MilliMirror.pdf) (No ML)
* OmniScatter: extreme sensitivity mmWave backscattering using commodity FMCW radar,	MobiSys 22 [[Paper]](http://mason.gmu.edu/~ychae2/Omniscatter.pdf)	(No	ML) (Best Paper)
* mmTag: A Millimeter Wave Backscatter Network, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472917.pdf) (No ML)

<a name="user-content-rfid"></a>
#### RFID (Total: 12 | No ML(12) | ML(0) | DL(0))
* Battery-free Wideband Spectrum Mapping using Commodity RFID Tags, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592508) (No ML)
* Go Beyond RFID: Rethinking the Design of RFID Sensor Tags for Versatile Applications, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613284) (No ML)
* Revisiting Cardinality Estimation in COTS RFID Systems, MobiCom 23 [[Paper]](https://cs.nju.edu.cn/liujia/papers/mobicom23_counting.pdf) (No ML)
*  Retwork: Exploring Reader Network with COTS RFID Systems, ATC 20 [[Paper]](https://www.usenix.org/system/files/atc20-liu-jia_0.pdf) (No ML)
* Fireworks: Channel Estimation of Parallel Backscattered Signals, IPSN 20 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/2020.1.pdf) (No ML)
* Redefining passive in backscattering with commodity devices, MobiCom 20 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/xShift-Mobicom2020.pdf) (No ML)
*  Two to Tango: Hybrid Light and Backscatter Networks for Next Billion Devices, MobiSys 20 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/811/tosubmit.pdf?sequence=1) (No ML)
* Pushing the Range Limits of Commercial Passive RFIDs, NSDI 19 [[Paper]](https://www.usenix.org/system/files/nsdi19-wang-jingxian.pdf) (No ML)
* Parallel Backscatter in the Wild: When Burstiness and Randomness Play with You, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241544) (No ML)
* FlipTracer: Practical Parallel Decoding for Backscatter Communication, MobiCom 17 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/2017.1.pdf) (No ML)
* Drone Relays for Battery-Free Networks, SIGCOMM 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3098822.3098847) (No ML) 
* Making Sense of Mechanical Vibration Period with Sub-millisecond Accuracy Using Backscatter Signals, MobiCom 16 [[Paper]](https://www4.comp.polyu.edu.hk/~csyanglei/data/files/tagbeat-mobicom.pdf) (No ML)

<a name="user-content-acoustic-1"></a>
#### Acoustic Communication (Total: 5 | No ML(5) | ML(0) | DL(0))
* Enabling Long-Range Underwater Backscatter via Van Atta Acoustic Networks, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3603269.3604814) (No ML)
* Higher-order modulation for acoustic backscatter communication in metals, SIGCOMM 22 [[Paper]](http://www.bcrenner.de/publications/2021_Backscatter-preprint.pdf) (No ML)
* Microphone array backscatter: an application-driven design for lightweight spatial sound recording over the air, MobiCom 21 [[Paper]](https://www2.cs.sfu.ca/~jcliu/Papers/Microphone21.pdf) (No ML)
* Ultra-Wideband Underwater Backscatter via Piezoelectric Metamaterials, SIGCOMM 20 [[Paper]](https://www.mit.edu/~fadel/papers/U2B-paper.pdf) (No ML)
* Underwater backscatter networking, SIGCOMM 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3341302.3342091) (No ML)

<a name="user-content-other-batteryless-works"></a>
#### Other Networks (Total: 40 | No ML(36) | ML(3) | DL(1))
* RF-Bouncer: A Programmable Dual-band Metasurface for Sub-6 Wireless Networks, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-li-xinyi.pdf) (No ML)
* DeepGANTT: A Scalable Deep Learning Scheduler for Backscatter Networks, IPSN 23 [[Paper]](https://arxiv.org/pdf/2112.12985.pdf) (DL)
* SmartShell: A Near-Field Reflective Surface Enhancing RSS, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596866) (No ML)
* Magnetic Backscatter for In-body Communication and Localization, MobiCom 23 [[Paper]](https://deepakv.web.illinois.edu/assets/papers/innercompass_mobicom23.pdf) (No ML)
* The Underwater Backscatter Channel: Theory, Link Budget, and Experimental Validation, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613265) (No ML) (Best Paper Award)
* Eliminating Design Effort: A Reconfigurable Sensing Framework For Chipless, Backscatter Tags, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a298/962400a298.pdf) (ML)
* Magnetoelectric backscatter communication for millimeter-sized wireless biomedical implants, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560541) (No ML) (Best Paper Award)
* RF-Transformer: A Unified Backscatter Radio Hardware Abstraction, MobiCom 22 [[Paper]](https://arxiv.org/pdf/2209.15195.pdf) (No ML)
* PLatter: On the Feasibility of Building-scale Power Line Backscatter, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-zhang_junbo.pdf) (No ML)
* Passive DSSS: Empowering the Downlink Communication for Backscatter Systems, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-li_songfan.pdf) (No ML)
* Enabling software-defined PHY for backscatter networks, MobiSys 22 [[Paper]](https://chendy.tech/static/assets/files/mobisys22-Fengyuan-final.pdf) (No ML)
* Judo: addressing the energy asymmetry of wireless embedded systems through tunnel diode based wireless transmitters, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538923) (No ML)
* Pushing the Physical Limits of IoT Devices with Programmable Metasurfaces, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-chen.pdf) (No ML)
* One Tag, Two Codes: Identifying Optical Barcodes with NFC, MobiCom 21 [[Paper]](https://web.comp.polyu.edu.hk/csyanglei/data/files/coilcode-mobicom21.pdf) (No ML)
* Morphy: Software Defined Charge Storage for the IoT, SenSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485947) (No ML)
* MultiScatter: Multistatic Backscatter Networking for Battery-Free Sensors, SenSys 21 [[Paper]](https://par.nsf.gov/servlets/purl/10303864) (No ML)
* Enabling Passive Backscatter Tag Localization Without Active Receivers, SenSys 21 [[Paper]](http://www.wings.cs.stonybrook.edu/pdfs/2021-sensys.pdf) (No ML)
* Commodity-level BLE backscatter, MobiSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3466865) (No ML)
* RFocus: Beamforming Using Thousands of Passive Antennas, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-arun.pdf) (ML)
* Towards Flexible Wireless Charging for Medical Implants Using Distributed Antenna System, MobiCom 20 [[Paper]](https://arxiv.org/pdf/2001.07644.pdf) (No ML)
* Tunnel emitter: tunnel diode based low-power carrier emitters for backscatter tags, MobiCom 20 [[Paper]](https://lorenzocorneo.github.io/papers/2020-mobicom.pdf) (No ML)
* Internet-of-Microchips: Direct Radio-to-Bus Communication with SPI Backscatter, MobiCom 20 [[Paper]](https://dl.acm.org/doi/10.1145/3372224.3419182) (No ML)
* Gateway over the Air: Towards Pervasive Internet Connectivity for Commodity IoT, MobiSys 20 [[Paper]](https://yung-web.github.io/home/Publication/Conference/Gateway_over_the_Air-Towards_Pervasive_Internet_Connectivity_for_Commodity_IoT.pdf) (No ML)
* Towards scalable backscatter sensor mesh with decodable relay and distributed excitation, MobiSys 20 [[Paper]](https://www2.cs.sfu.ca/~jcliu/Papers/mobisys20-final157.pdf)	(No ML)
* DigiScatter: efficiently prototyping large-scale OFDMA backscatter networks, MobiSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3386901.3388914) (No ML)
* TagAlong: Efficient Integration of Battery-free Sensor Tags in Standard Wireless Networks, IPSN 20 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2020-2ZapWCkbA6ELdouTqExUlt/549700a169/549700a169.pdf) (No ML)
* Leveraging Ambient LTE Traffic for Ubiquitous Passive Communication, SIGCOMM 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3387514.3405861) (No ML)
* NetScatter: Enabling Large-Scale Backscatter Networks, NSDI 19 [[Paper]](https://www.usenix.org/system/files/nsdi19-hessar.pdf) (No ML)
* TunnelScatter: Low Power Communication for Sensor Tags using Tunnel Diodes, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345451) (No ML)
* Passive-ZigBee: Enabling ZigBee Communication in IoT Networks with 1000X+ Less Power Consumption, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274846) (Best paper runner-up awards) (No ML)
* BARNET: Activity Recognition using Passive Backscattering Tag-to-Tag Network, MobiSys 18 [[Paper]](http://www.wings.cs.sunysb.edu/pdfs/2018-Jihoon-mobisys.pdf) (ML)
* Slocalization: Sub-muW, Static, Decimeter-Accurate Localization with Ultra Wideband Backscatter, IPSN 18 [[Paper]](https://patpannuto.com/pubs/pannuto18slocalization.pdf) (No ML)
* In-body backscatter communication and localization, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3230543.3230565) (No ML)
* 3D Localization for Sub-Centimeter Sized Devices, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274851) (Best Paper) (No ML)
* FM Backscatter: Enabling Connected Cities and Smart Fabrics, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-wang-anran.pdf) (No ML)
* NICScatter: Backscatter as a Covert Channel in Mobile Devices, MobiCom 17 [[Paper]](https://www.yangzhice.com/docforweb/NICScatter/NICScatter_MobiCom.pdf) (No ML)
* Battery-Free Cellphone, UbiComp 17 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/phone.pdf) (No ML)
* LoRea: A Backscatter Architecture that Achieves a Long Communication Range, SenSys 17 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3131672.3131691) (No ML)
* Enabling Practical Backscatter Communication for On-body Sensors, SIGCOMM 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2934872.2934901) (No ML)
* Inter-Technology Backscatter: Towards Internet Connectivity for Implanted Devices, SIGCOMM 16 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2934872.2934894) (No ML)

<a name="domain-specific-aiot-systems"></a>
## 🚀 Domain-specific AIoT Systems (255)
							
### AIoT Systems for Healthcare and Well-being (Total:58 | No ML(22) | ML(9) | DL(23) | GenAI(4))
<a name="aiot-systems-for-healthcare-and-well-being"></a>
#### Vital Sign Monitoring 
* APG: Audioplethysmography for Cardiac Monitoring in Hearables, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613281) (No ML)
* DF-Sense: Multi-user Acoustic Sensing for Heartbeat Monitoring with Dualforming, MobiSys 23 [[Paper]](https://hal.science/hal-04309107v1/file/8%20DF-Sense%20Multi-user%20Acoustic%20Sensing%20for%20Heartbeat%20Monitoring%20with%20Dualforming.pdf) (No ML)
* Passive Vital Sign Monitoring via Facial Vibrations Leveraging AR/VR Headsets, MobiSys 23 [[Paper]](https://dl.acm.org/doi/10.1145/3581791.3596848) (DL)
* A Low-Cost In-situ System for Continuous Multi-Person Fever Screening, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a015/962400a015.pdf) (DL)
* PROS: an Efficient Pattern-Driven Compressive Sensing Framework for Low-Power Biopotential-based Wearables with On-chip Intelligence, MobiCom 22 [[Paper]](https://theyoungkwon.github.io/papers/articles/pham_pros_mobicom22.pdf) (DL)
* Network-side digital contact tracing on a large university campus, MobiCom 22 [[Paper]](https://arxiv.org/pdf/2201.10641.pdf) (No ML)
* Hearing Heartbeat from Voice: Towards Next Generation Voice-User Interfaces with Cardiac Sensing Function, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568508) (DL)
* mmBP: Contact-free Millimetre-wave Radar based Approach to Blood Pressure Measurement, SenSys 22 [[Paper]](https://taogu.site/pub/paper/mmBP.pdf) (ML)
* Your Smart Speaker Can “Hear” Your Heartbeat!, UbiComp 21 [[Paper]](https://hal.science/hal-03363346v1/file/3432237.pdf) (No ML)	
* Healthy diapering with passive RFIDs for diaper wetness sensing and urine pH identification, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3466870) (ML)
* Crisp-BP: Continuous Wrist PPG-based Blood Pressure Measurement, MobiCom 21 [[Paper]](https://cis.temple.edu/~yu/research/CrispBP-Mobicom21.pdf) (DL)
* MoVi-Fi: Motion-robust Vital Signs Waveform Recovery via Deep Interpreted RF Sensing, MobiCom 21 [[Paper]](https://rabbitnick.github.io/pubs/movifi.pdf) (DL)
* U-Verse: a miniaturized platform for end-to-end closed-loop implantable internet of medical things systems, SenSys 21, [[Paper]](https://ece.northeastern.edu/wineslab/papers/GuidaSENSYS2019.pdf) (No ML)
* SpiroSonic: monitoring human lung function via acoustic sensing on commodity smartphones, MobiCom 20 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobicom20.pdf) (DL)
* Contactless seismocardiography via deep learning radars, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419982) (DL)
* RFWash: A Weakly Supervised Tracking of Hand Hygiene Technique, SenSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3384419.3430733) (DL)
* Noninvasive Glucose Monitoring Using Polarized Light, SenSys 20 [[Paper]](https://www.cs.columbia.edu/~xia/publication/sensys20-glucose/sensys20-glucose.pdf) (ML)
* Contactless Infant Monitoring using White Noise, MobiCom 19 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/whitenoise.pdf)	(No ML)	
* Experience: Design, Development and Evaluation of a Wearable Device for mHealth Applications, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345432) (No ML)
* eBP: A Wearable System For Frequent and Comfortable Blood Pressure Monitoring From User's Ear, MobiCom 19 [[Paper]](https://par.nsf.gov/servlets/purl/10303241) (Best Paper) (No ML)
* pH Watch - Leveraging Pulse Oximeters in Existing Wearables for Reusable, Real-time Monitoring of pH in Sweat, MobiSys 19 [[Paper]](https://anantabalaji.github.io/projects/pH_watch/pH_watch.pdf) (No ML)
* VitaMon: measuring heart rate variability using smartphone front camera, SenSys 19 [[Paper]](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=5936&context=sis_research) (DL)
* Experience: Cross-Technology Radio Respiratory Monitoring Performance Study, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241560) (No ML)
* mCerebrum: A Mobile Sensing Software Platform for Development and Validation of Digital Biomarkers and Interventions, SenSys 17 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3131672.3131694) (ML)
* Monitoring a Person's Heart Rate and Respiratory Rate on a Shared Bed Using Geophones, SenSys 17 [[Paper]](https://www.cs.virginia.edu/~bjc8c/class/cs6501-f18/papers/jia17geophones.pdf) (No ML)
* PhO2: Smartphone based Blood Oxygen Level Measurement Systems using Near-IR and RED Wave-guided Light, SenSys 17 [[Paper]](https://mobile.cs.gsu.edu/aashok/Papers/12_2017_SenSys.pdf) (No ML)
* Monoxalyze: Verifying Smoking Cessation with a Keychain-sized Carbon Monoxide Breathalyzer, SenSys 16 [[Paper]](https://web.eecs.umich.edu/~prabal/pubs/papers/adkins16monoxalyze.pdf) (No ML)
* Burnout: A Wearable System for Unobtrusive Skeletal Muscle Fatigue Estimation, IPSN 16 [[Paper]](https://www.ceid.upatras.gr/webpages/courses/adhocnets/files/papers/paper21.pdf) (ML)
* HB-Phone: a Bed-Mounted Geophone-Based Heartbeat Monitoring System, IPSN 16 [[Paper]](https://ieeexplore.ieee.org/document/7460676) (No ML)

#### In-Situ Illness Detection and Monitoring 
* PTEase: Objective Airway Examination for Pulmonary Telemedicine using Commodity Smartphones, MobiSys 23 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobisys23-ptease.pdf) (DL)
* PDAssess: A Privacy-preserving Free-speech based Parkinson’s Disease Daily Assessment System, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625805) (DL)
* Camera-based remote photoplethysmography to predict blood pressure in clinic patients with cardiovascular disease, Journal of Hypertension 23 [[Paper]](https://journals.lww.com/jhypertension/abstract/2023/06003/camera_based_remote_photoplethysmography_to.8.aspx)
* Burnout and the Quantified Workplace: Tensions around Personal Sensing Interventions for Stress in Resident Physicians, ACM HCI 22 [[Paper]](https://dl.acm.org/doi/10.1145/3555531) (No ML)
* EarHealth: an earphone-based acoustic otoscope for detection of multiple ear diseases in daily life, MobiSys 22 [[Paper]](https://web.archive.org/web/20220703105522id_/https://dl.acm.org/doi/pdf/10.1145/3498361.3538935) (DL)
* Out-Clinic Pulmonary Disease Evaluation via Acoustic Sensing and Multi-Task Learning on Commodity Smartphones, SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568437) (DL)
* NFCapsule: An Ingestible Sensor Pill for Eosinophilic Esophagitis Detection Based on Near-field Coupling, SenSys 22 [[Paper]](https://swarunkumar.com/papers/nfcapsule-sensys2022.pdf) (No ML)
* Predicting Early Warning Signs of Psychotic Relapse From Passive Sensing Data: An Approach Using Encoder-Decoder Neural Networks, JMIR 20 [[Paper]](https://mhealth.jmir.org/2020/8/e19962) (DL)
* PDLens: smartphone knows drug effectiveness among Parkinson's via daily-life activity fusion,	MobiCom	20	[[Paper]](https://chenhanxu.github.io/publication/mobicom_20b/paper.pdf) (DL)
* Painometry: Wearable and Objective Quantification System for Acute Postoperative Pain, MobiSys 20 [[Paper]](http://mnslab.org/tamvu/paper/2020%20Painometry_Hoang.pdf) (ML)
* PDVocal: Towards Privacy-preserving Parkinson's Disease Detection using Non-speech Body Sounds, MobiCom 19 [[Paper]](https://chenhanxu.github.io/publication/mobicom_19/paper.pdf) (DL)
* HealthSense: Software-defined Mobile-based Clinical Trials, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345433) (Best Paper) (No ML)
* Glasses for the Third Eye: Improving the Quality of Clinical Data Analysis with Motion Sensor-based Data Filtering, SenSys 17 [[Paper]](http://nsl.cau.ac.kr/~jpaek/docs/medisense-sensys2017-published.pdf) (ML)
* Mobile Phone Sensor Correlates of Depressive Symptom Severity in Daily-Life Behavior: An Exploratory Study, JMIR 15 [[Paper]](https://www.jmir.org/2015/7/e175) (No ML)
* StudentLife: assessing mental health, academic performance and behavioral trends of college students using smartphones, UbiComp 14 [[Paper]](https://studentlife.cs.dartmouth.edu/studentlife.pdf) (ML)

#### Assistive Technology
* ARSteth: Enabling Home Self-Screening with AR-Assisted Intelligent Stethoscopes, IPSN 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3583120.3586962) (DL)
* AccessWear: Making Smartphone Applications Accessible to Blind Users, MobiCom 23 [[Paper]](https://www3.cs.stonybrook.edu/~jain/papers/MobiCom_AccessWear_2023.pdf) (No ML)
* Sign-to-911: Emergency Call Service for Sign Language Users with Assistive AR Glasses, MobiCom  23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613260) (ML)
* SignQuery: A Natural User Interface and Search Engine for Sign Languages with Wearable Sensors, MobiCom 23 [[Paper]](https://www.cse.psu.edu/~mkg31/papers/signquery.pdf) (DL)
* Wireless earbuds for low-cost hearing screening, Mobisys 23 [[Paper]](https://dl.acm.org/doi/10.1145/3581791.3596856) (No ML)
* An off-the-shelf otoacoustic-emission probe for hearing screening via a smartphone, Nature Biomedical Engineering 2022 [[Paper]](https://www.nature.com/articles/s41551-022-00947-6) (No ML)
* RehabPhone: A Sotware-Defined Tool using 3D Printing and Smartphones for Personalized Home-based Rehabilitation, MobiSys 20 [[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-mobisys2020a.pdf) (No ML)
* SignSpeaker: A Real-time, High-Precision SmartWatch-based Sign Language Translator, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300117) (DL)
* MobileDeepPill: A Small-Footprint Mobile Deep Learning System for Recognizing Unconstrained Pill Images, MobiSys 17 [[Paper]](https://mi-zhang.github.io/papers/2017_MobiSys_MobileDeepPill.pdf) (DL)
* DeepASL: Enabling Ubiquitous and Non-Intrusive Word and Sentence-Level Sign Language Translation,SenSys 17 [[Paper]](https://dl.acm.org/doi/10.1145/3131672.3131693) (DL)
* iBlink: Smart Glasses for Facial Paralysis Patients, MobiSys 17 [[Paper]](https://xiaohuatian.acemap.info/paper/2017-mobisys-iBlink.pdf) (DL)

#### Personal Health Insight Generation
* Towards a Personal Health Large Language Model, Arxiv 24 [[Paper]](https://arxiv.org/abs/2406.06474) (GenAI)
* Transforming Wearable Data into Health Insights using Large Language Model Agents, Arxiv 24 [[Paper]](https://arxiv.org/abs/2406.06464) (GenAI)
* From Classification to Clinical Insights: Towards Analyzing and Reasoning About Mobile and Behavioral Health Data With Large Language Models, IMWUT 24 [[Paper]](https://dl.acm.org/doi/10.1145/3659604) (GenAI)
* Large Language Models are Few-Shot Health Learners [[Paper]](https://arxiv.org/pdf/2305.15525) (GenAI)
* Health-LLM: Large Language Models for Health Prediction via Wearable Sensor Data [[Paper]](https://arxiv.org/pdf/2401.06866) (GenAI)

### AIoT Systems for Video Streaming (Total:51 | No ML(23) | ML(8) | DL(20))
<a name="aiot-systems-for-video-streaming"></a>
#### Adaptive Video Streaming 
* Enabling High Quality Real-Time Communications with Adaptive Frame-Rate, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-meng.pdf) (No ML)
* Dashlet: Taming Swipe Uncertainty for Robust Short Video Streaming, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-li-zhuqi.pdf) (No ML)
* Dragonfly: Higher Perceptual Quality For Continuous 360° Video Playback, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3603269.3604876) (No ML)
* XRON: A Hybrid Elastic Cloud Overlay Network for Video Conferencing at Planetary Scale, SIGCOMM 23 [[Paper]](https://ennanzhai.github.io/pub/xron-sigcomm23.pdf) (No ML)
* Sammy: smoothing video traffic to be a friendly internet neighbor, SIGCOMM 23 [[Paper]](https://brucespang.com/papers/sammy.pdf) (No ML)
* Veritas: Answering Causal Queries from Video Streaming Traces, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3603269.3604828) (ML)
* ZGaming: Zero-Latency 3D Cloud Gaming by Image Prediction, SICGOMM 23 [[Paper]](https://dl.acm.org/doi/10.1145/3603269.3604819) (DL)
* Swift: Adaptive Video Streaming with Layered Neural Codecs, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-dasari.pdf) (DL)
* GSO-Simulcast: Global Stream Orchestration in Simulcast Video Conferencing Systems, SIGCOMM 22 [[Paper]](https://yfmascgy.github.io/papers/gso-simulcast.pdf) (No ML)
* Proactive Energy-Aware Adaptive Video Streaming on Mobile Devices, ATC 21 [[Paper]](https://www.usenix.org/system/files/atc21-meng.pdf) (No ML)
* Loki: Improving Long Tail Performance of Learning-Based Real-Time Video Adaptation by Fusing Rule-Based Models, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483259) (DL)
* SENSEI: Aligning Video Streaming Quality with Dynamic User Sensitivity, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-zhang.pdf) (DL)
* Learning in situ: a randomized experiment in video streaming, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-yan.pdf) (DL)
* OnRL: improving mobile video telephony via online reinforcement learning, MobiCom 20 [[Paper]](https://static.aminer.cn/upload/pdf/1489/1347/1583/5f51b90d9fced0a24bdc7f64_0.pdf) (DL)
* PERCEIVE: Deep Learning-based Cellular Uplink Prediction Using Real-time Scheduling Patterns, MobiSys 20 [[Paper]](https://mail.netstech.org/wp-content/uploads/2021/07/perceive-mobisys-2020.pdf) (DL)
* Jigsaw: Robust Live 4K Video Streaming, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300127) (No ML)
* Learning to Coordinate Video Codec with Transport Protocol for Mobile Video Telephony, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345430) (DL)
* End-to-end transport for video QoE fairness, SIGCOMM 19 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3341302.3342077) (No ML)
* Vantage: optimizing video upload for time-shifted viewing of social live streams, SIGCOMM 19 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3341302.3342064) (No ML)
* Flare: Practical Viewport-Adaptive 360-Degree Video Streaming for Mobile Devices, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241565) (ML)
* Rubiks: Practical 360-Degree Streaming for Smartphones, MobiSys 18 [[Paper]](https://www.cse.psu.edu/~gxc27/teach/597/rubiks_mobisys.pdf) (ML)
* Oboe: Auto-tuning Video ABR Algorithms to Network Conditions, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230558) (No ML)
* Neural Adaptive Video Streaming with Pensieve, SIGCOMM 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3098822.3098843) (DL)
* RnB: Rate and Brightness Adaptation for Rate-Distortion-Energy Tradeoff in HTTP Adaptive Streaming over Mobile Devices, MobiCom 16 [[Paper]](https://mason.gmu.edu/~zyan4/papers/rnb_mobicom16.pdf) (ML)

#### Video Enhancement
* OmniLive: Super-Resolution Enhanced 360° Video Live Streaming for Mobile Devices, MobiSys 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581791.3596851) (DL)
* NeuroScaler: neural video enhancement at scale, SIGCOMM 22 [[Paper]](https://jaykim305.github.io/assets/pdf/neuroscaler-sigcomm22.pdf) (DL)
* YuZu: Neural-Enhanced Volumetric Video Streaming, NSDI 22 [[paper]](https://www.usenix.org/system/files/nsdi22-paper-zhang.pdf) (DL)
* NEMO: enabling neural-enhanced video streaming on commodity mobile devices, MobiCom 20 [[Paper]](https://hyunhoyeo.com/assets/pdf/3372224.3419185.pdf) (DL)
* Neural-Enhanced Live Streaming: Improving Live Video Ingest via Online Learning, SIGCOMM 20 [[Paper]](https://hyunhoyeo.com/assets/pdf/3387514.3405856.pdf) (DL)
* Neural Adaptive Content-aware Internet Video Delivery, OSDI 18 [[Paper]](https://www.usenix.org/system/files/osdi18-yeo.pdf) (DL)

#### Efficiency Optimization
* Tambur: Efficient loss recovery for videoconferencing via streaming codes, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-rudow.pdf) (DL)
* CellFusion: Multipath Vehicle-to-Cloud Video Streaming with Network Coding in the Wild, SIGCOMM 23 [[Paper]](https://ennanzhai.github.io/pub/cellfusion-sigcomm23.pdf) (No ML)
* Converge: QoE-driven Multipath Video Conferencing over WebRTC, SIGCOMM 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3603269.3604822) (No ML)
* LiveNet: a low-latency video transport network for large-scale live streaming, SIGCOMM 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3544216.3544236) (No ML)
* Warehouse-Scale Video Acceleration: Co-design and Deployment in the Wild, ASPLOS 21 [[Paper]](https://gwern.net/doc/cs/hardware/2021-ranganathan.pdf) (No ML)
* XLINK: QoE-Driven Multi-Path QUIC Transport in Large-scale Video Services, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472893.pdf) (No ML)
* Banner: An Image Sensor Reconfiguration Framework for Seamless Resolution-based Tradeoffs, MobiSys 19 [[Paper]](https://meteor.ame.asu.edu/publications/mobisys19hu-banner.pdf) (No ML)
* Pano: optimizing 360° video streaming with a better understanding of quality perception, SIGCOMM 19 [[Paper]](https://people.cs.uchicago.edu/~junchenj/docs/360StreamingQuality_SIGCOMM.pdf) (DL)
* VideoChef: Efficient Approximation for Streaming Video Processing Pipelines, ATC 18 [[Paper]](https://www.usenix.org/system/files/conference/atc18/atc18-xu-ran.pdf) (ML)
* Salsify: Low-Latency Network Video Through Tighter Integration Between a Video Codec and a Transport Protocol, NSDI 18 [[Paper]](https://www.usenix.org/system/files/conference/nsdi18/nsdi18-fouladi.pdf) (No ML)
* Towards Battery-Free HD Video Streaming, NSDI 18 [[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/videobackscatter.pdf) (No ML)
* Popularity Prediction of Facebook Videos for Higher Quality Streaming, ATC 17 [[Paper]](https://www.usenix.org/system/files/conference/atc17/atc17-tang.pdf) (DL)
* Encoding, Fast and Slow: Low-Latency Video Processing Using Thousands of Tiny Threads, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-fouladi.pdf) (No ML)
* SVE: Distributed Video Processing at Facebook Scale, SOSP 17 [[Paper]](https://www.cs.princeton.edu/~wlloyd/papers/sve-sosp17.pdf) (No ML)
* Disk|Crypt|Net: rethinking the stack for high-performance video streaming, SIGCOMM 17 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3098822.3098844) (No ML)
* CFA: A Practical Prediction System for Video QoE Optimization, NSDI 16 [[Paper]](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-jiang-junchen.pdf) (ML)

#### Volumetric Video Streaming  
* FarfetchFusion: Towards Fully Mobile Live 3D Telepresence Platform, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3592525) (DL)
* MetaStream: Live Volumetric Content Capture, Creation, Delivery, and Rendering in Real Time, MobiCom 23 [[Paper]](https://3dvar.com/Guan2023MetaStream.pdf) (DL)
* Vues: Practical Mobile Volumetric Video Streaming Through Multiview Transcoding, MobiCom22 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/vues_mobicom22.pdf) (ML)
* GROOT: a real-time streaming system of high-fidelity volumetric videos, MobiCom 20 [[Paper]](https://juheonyi.github.io/files/GROOT.pdf) (No ML)
* ViVo: visibility-aware mobile volumetric video streaming, MobiCom 20 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/vivo_mobicom20.pdf) (ML)

### AIoT Systems for Video Analytics	(Total:21 | No ML(1) | ML(0) | DL(20))
<a name="aiot-systems-for-video-analytics"></a>
#### Continuous Learning
* RECL: Responsive Resource-Efficient Continuous Learning for Video Analytics, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-khani.pdf) (DL)
* Ekya: Continuous Learning of Video Analytics Models on Edge Compute Servers, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-bhardwaj.pdf) (DL)

#### Runtime Adaptation
* Enhancing Video Analytics Accuracy via Real-time Automated Camera Parameter Tuning, SenSys 22 [[Paper]](https://arxiv.org/pdf/2107.03964.pdf) (DL)
* Turbo: Opportunistic Enhancement for Edge Video Analytics, SenSys 22 [[Paper]](https://arxiv.org/pdf/2207.00172.pdf) (DL)
* Distream: Scaling Live Video Analytics with Workload-Adaptive Distributed Edge Intelligence, SenSys 20 [[Paper]](https://mi-zhang.github.io/papers/2020_SenSys_Distream.pdf) (DL)
* Chameleon: scalable adaptation of video analytics, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230574) (DL)
* AWStream: Adaptive Wide-Area Streaming Analytics, SIGCOMM 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3230543.3230554) (DL)

#### Efficiency Optimization
* Gemel: Model Merging for Memory-Efficient, Real-Time Video Analytics at the Edge, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-padmanabhan.pdf) [[code]](https://github.com/artpad6/gemel_nsdi23) (DL)
* PacketGame: Multi-Stream Packet Gating for Concurrent Video Inference at Scale, SIGCOMM 23 [[Paper]](https://yuanmu97.github.io/preprint/packetgame_sigcomm23.pdf) (DL)
* CoVA: Exploiting Compressed-Domain Analysis to Accelerate Video Analytics, ATC 22 [[Paper]](https://www.usenix.org/system/files/atc22-hwang.pdf) (DL)
* AccMPEG: Optimizing Video Encoding for Video Analytics, MLSys 22 [[Paper]](https://arxiv.org/pdf/2204.12534.pdf) (DL)
* Server-Driven Video Streaming for Deep Learning Inference, SIGCOMM 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3387514.3405887) (DL)
* Reducto: On-Camera Filtering for Resource-Efficient Real-Time Video Analytics, SIGCOMM 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3387514.3405874) (DL)
* Scaling Video Analytics on Constrained Edge Nodes, MLSys 19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/197.pdf) (DL)
* Panoptes: Servicing Multiple Applications Simultaneously using Steerable Cameras, IPSN 17 [[Paper]](https://winlab.rutgers.edu/~shubhamj/papers/Shubham_Panoptes_IPSN2017.pdf) (No ML)

#### Query Optimization 
* Boggart: Towards General-Purpose Acceleration of Retrospective Video Analytics, NSDI 23 [[Paper]](https://www.usenix.org/system/files/nsdi23-agarwal-neil.pdf) (DL)
* Privid: Practical, Privacy-Preserving Video Analytics Queries, NSDI 22 [[Paper]](https://www.usenix.org/system/files/nsdi22-paper-cangialosi.pdf) (DL)
* Tutti: coupling 5G RAN and mobile edge computing for latency-critical video analytics, MobiCom 22 [[Paper]](https://dl.acm.org/doi/10.1145/3495243.3560538) (DL)
* Video Analytics with Zero-streaming Cameras, ATC 21 [[Paper]](https://xumengwei.github.io/files/ATC-DIVA.pdf) (DL)
* Approximate query service on autonomous IoT cameras,	MobiSys	20 [[Paper]](https://arxiv.org/pdf/1909.00841) (DL)
* Caesar: cross-camera complex activity recognition, SenSys 19 [[Paper]](http://web.cs.ucla.edu/~ravi/CS239_W20/papers/caesar.pdf) (DL)

### AIoT Systems for Autonomous Driving (Total:35 | No ML(15) | ML(3) | DL(17))
<a name="aiot-systems-for-autonomous-driving"></a>
#### Perception Enhancement
* Ghost-Probe: NLOS Pedestrian Rushing Detection with Monocular Camera for Automated Driving, SenSys 23 [[Paper]](https://mason.gmu.edu/~zyan4/papers/ghostprobe_sensys23.pdf) (DL)
* Robust Real-time Multi-vehicle Collaboration on Asynchronous Sensors, MobiCom 23 [[Paper]](https://ry4nzhu.github.io/publication/robust_real_time/robust_real_time.pdf) (DL)
* AutoFed: Heterogeneity-Aware Federated Multimodal Learning for Robust Autonomous Driving, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592517) (DL)
* Mosaic: leveraging diverse reflector geometries for omnidirectional around-corner automotive radar, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538944) (No ML)
* AutoMatch: Leveraging Traffic Camera to Improve Perception and Localization of Autonomous Vehicles, SenSys 22 [[Paper]](https://yanzhenyu.com/assets/pdf/AutoMatch-SenSys22.pdf) (DL)
* VIPS: Real-Time Perception Fusion for Infrastructure-Assisted Autonomous Driving, MobiCom 22 [[Paper]](https://yanzhenyu.com/assets/pdf/VIPS-MobiCom22.pdf) (Best Paper Award Runner-ups) (DL)
* AutoCast: scalable infrastructure-less cooperative perception for distributed collaborative driving, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538925) (No ML)
* EMP: Edge-assisted Multi-vehicle Perception, MobiCom 21 [[Paper]](https://xiaoshawnzhu.github.io/emp-mobicom21.pdf) (DL)
* VI-Eye: Semantic-based 3D Point Cloud Registration for Infrastructure-assisted Autonomous Driving, MobiCom 20 [[Paper]](https://aiot.ie.cuhk.edu.hk/papers/VI_Eye.pdf) (DL)
* Renovating road signs for infrastructure-to-vehicle networking: a visible light backscatter communication and networking approach, MobiCom 20 [[Paper]](https://soar.group/pubs/RetroI2V.MobiCom20.pdf) (No ML)
* Pointillism: Accurate 3D Bounding Box Estimation with Multi-Radars, SenSys 20 [[Paper]](https://wcsng.ucsd.edu/files/Pointillism_paper.pdf) [[code]](https://github.com/Kshitizbansal/pointillism-multi-radar-data) (DL)
* SmartDashCam: Automatic Live Calibration for DashCams, IPSN 19 [[Paper]](https://dl.acm.org/doi/10.1145/3302506.3310397) (No ML)
* AVR: Augmented Vehicular Reality, MobiSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3210240.3210319) (Best Paper Runner-Up) (No ML)
* Object Recognition and Navigation using a Single Networking Device, MobiSys 17 [[Paper]](https://people.cs.uchicago.edu/~ravenben/publications/pdf/60gradar-mobisys17.pdf) (No ML)

#### Localization, Tracking, and Mapping
* VI-Map: Infrastructure-Assisted Real-Time HD Mapping for Autonomous Driving, MobiCom 23 [[Paper]](https://yanzhenyu.com/assets/pdf/VI-Map-MobiCom23.pdf) (DL)
* uGPS: Design and Field-Tested Seamless GNSS Infrastructure in Metro City, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560520) (No ML)
* MVP: magnetic vehicular positioning system for GNSS-denied environments, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483264) (DL)
* Large-Scale Vehicle Trajectory Reconstruction with Camera Sensing Network, MobiCom 21 [[Paper]](https://dl.acm.org/doi/10.1145/3447993.3448617) (DL)
* Wi-Go: Accurate and Scalable Vehicle Positioning using WiFi Fine Timing Measurement, MobiSys 20 [[Paper]](https://www.winlab.rutgers.edu/~gruteser/papers/3386901.3388944.pdf) (No ML)
* CarMap: Fast 3D Feature Map Updates for Automobiles, NSDI 20 [[Paper]](https://www.usenix.org/system/files/nsdi20-paper-ahmad.pdf) (DL)
* VeMo: Enabling Transparent Vehicular Mobility Modeling at Individual Levels with Full Penetration, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300130) (ML)
* Experience: Understanding Long-Term Evolving Patterns of Shared Electric Vehicle Networks, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300132) (No ML)
* The Architectural Implications of Autonomous Driving: Constraints and Acceleration, ASPLOS 18 [[Paper]](https://people.computing.clemson.edu/~jmarty/projects/lowLatencyNetworking/papers/EmergingApplicationSystems/AutonomousVehicles/AutonomousCarConstraints.pdf) (DL)
* EXIMIUS: A Measurement Framework for Explicit and Implicit Urban Traffic Sensing, SenSys 18 [[Paper]](https://people.cs.rutgers.edu/~dz220/paper/Eximius.pdf) (No ML)

#### Automatic Testing
* Diagnosing Vehicles with Automotive Batteries, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300126) (ML)
* Automatic Unusual Driving Event Identification for Dependable Self-Driving, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274838) (DL)
* Sentio: Driver-in-the-Loop Forward Collision Warning Using Multisample Reinforcement Learning, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274843) (ML)
* BigRoad: Scaling Road Data Acquisition for Dependable Self-Driving, MobiSys 17 [[Paper]](https://personal.stevens.edu/~ychen6/papers/mobisys17-BigRoad.pdf) (DL)

#### Control and Actuation
* Eagle: End-to-end Deep Reinforcement Learning based Autonomous Control of PTZ Cameras, IoTDI 23 [[Paper]](https://dl.acm.org/doi/10.1145/3576842.3582366) (DL)

#### Vehicular Networking
* mmSV: mmWave Vehicular Networking using Street View Imagery in Urban Environments, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613291) (DL)
* RoS: Passive Smart Surface for Roadside-to-Vehicle Communication, SIGCOMM 21 [[Paper]](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472896.pdf) (No ML)
* Demystifying Millimeter-Wave V2X: Towards Robust and Efficient Directional Connectivity Under High Mobility, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419208) (No ML)
* RAVEN: Improving Interactive Latency for the Connected Car, MobiCom 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3241539.3241571) (No ML)
* CoReCast: Collision Resilient Broadcasting in Vehicular Networks, MobiSys 18 [[Paper]](https://abaxi.github.io/pdfs/corecast_paper.pdf) (No ML)
* Experience: Accurate Simulation of Dense Scenarios with Hundreds of Vehicular Transmitters, MobiCom 16 [[Paper]](https://winlab.rutgers.edu/~rostami/files/pdf/cheng2016experience.pdf) (No ML)

### AIoT Systems for AR/VR/MR (Total:38 | No ML(20) | ML(5) | DL(13))
<a name="aiot-systems-for-arvrmr"></a>
#### Object Detection 
* Augmenting Augmented Reality with Non-Line-of-Sight Perception, NSDI	23 [[Paper]](https://www.usenix.org/conference/nsdi23/presentation/boroushaki) (No ML)
* XRLoc: Accurate UWB Localization to Realize XR Deployments, SenSys 23 [[Paper]](https://arxiv.org/pdf/2307.12512) (No ML)
* Multi-User Augmented Reality with Infrastructure-free Collaborative Localization, IPSN 22 [[Paper]](https://arxiv.org/pdf/2111.00174.pdf) (No ML)
* DeepMix: mobility-aware, lightweight, and hybrid 3D object detection for headsets, MobiSys 22 [[Paper]](https://arxiv.org/pdf/2201.08812.pdf) (DL)
* FollowUpAR: enabling follow-up effects in mobile AR applications, MobiSys 21 [[Paper]](https://tns.thss.tsinghua.edu.cn/~jingao/assets/pdf/papers/mobisys21_followupar.pdf) (No ML)
* All that GLITTERs: Low-Power Spoof-Resilient Light Anchors for Augmented Reality, IPSN 20 [[Paper]](https://users.ece.cmu.edu/~vsekar/assets/pdf/ipsn20_glitter.pdf) (No ML)
* Edge Assisted Real-time Object Detection for Mobile Augmented Reality, MobiCom 19 [[Paper]](https://dl.acm.org/doi/10.1145/3300061.3300116) (DL)
* When IoT met Augmented Reality: Visualizing the Source of the Wireless Signal in AR View, MobiSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326079) (No ML)
* Frugal following: power thrifty object detection and tracking for mobile augmented reality, SenSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3356250.3360044) (DL)
* Empath-D: VR-based Empathetic App Design for Accessibility, MobiSys 18 [[Paper]](https://nclab.kaist.ac.kr/files/papers/Conference/mobisys18-10-kim.pdf) (No ML)

#### User Inputs
* UbiPose: Towards Ubiquitous Outdoor AR Pose Tracking using Aerial Meshes, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613263) (DL)
* Egocentric Human Pose Estimation using Head-mounted mmWave Radar, SenSys 23 [[Paper]](https://dl.acm.org/doi/10.1145/3625687.3625799) (DL)
* Cyclops: an FSO-based wireless link for VR headsets, SIGCOMM 22 [[Paper]](https://www3.cs.stonybrook.edu/~mdasari/papers/sigcomm-2022-paper.pdf) (No ML)
* ExGSense: Toward Facial Gesture Sensing and Reconstruction with a Sparse Near-Eye Sensor Array, IPSN 21 [[Paper]](http://xyzhang.ucsd.edu/papers/Chen.Chen_IPSN21_ExGSense.pdf) (DL)
* Aura: Inside-out Electromagnetic Controller Tracking MobiSys 19 [[Paper]](https://www.ericwhitmire.com/pdfs/aura.pdf) (ML)
* HandSense: capacitive coupling-based dynamic, micro finger gesture recognition, SenSys 19 [[Paper]](https://www.winlab.rutgers.edu/~gruteser/papers/sensys19-final195.pdf) (DL)
* Conductive Inkjet Printed Passive 2D TrackPad for VR Interaction, MobiCom 18 [[Paper]](http://xyzhang.ucsd.edu/papers/CGao_MobiCom18_Inkput.pdf) (No ML)
* Depth Aware Finger Tapping on Virtual Display, MobiSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3210240.3210315) (No ML)
* When Virtual Reality Meets Internet of Things in the Gym: Enabling Immersive Interactive Machine Exercises, UbiComp 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3214281) (ML)
* Ultra-Low Power Gaze Tracking for Virtual Reality, SenSys 17 [[Paper]](https://dlnext.acm.org/doi/pdf/10.1145/3131672.3131682) (ML)

#### Performance Enhancement
* Breaking edge shackles: Infrastructure-free collaborative mobile augmented reality, SenSys 22 [[Paper]](https://www.cs.ucr.edu/~jiasi/pub/freeAR-sensys22.pdf) (DL)
* Q-VR: System-Level Design for Future Collaborative Virtual Reality Rendering, ASPLOS 21 [[Paper]](https://arxiv.org/pdf/2102.13191) (ML)
* Coterie: Exploiting Frame Similarity to Enable High-Quality Multiplayer VR on Commodity Mobile Devices, ASPLOS 20 [[Paper]](https://ranger.uta.edu/~jmeng/pubs/asplos20.pdf) (No ML)
* Firefly: Untethered Multi-user VR for Commodity Mobile Devices, ATC 20 [[Paper]](https://www.usenix.org/system/files/atc20-liu-xing.pdf) (ML)
* CollabAR: Edge-assisted Collaborative Image Recognition for Mobile Augmented Reality, IPSN 20 [[Paper]](https://research.ece.cmu.edu/lions/Papers/CollabAR_IPSN.pdf) (DL)
* Heimdall: mobile GPU coordination platform for augmented reality applications, MobiCom 20 [[Paper]](https://juheonyi.github.io/files/Heimdall.pdf) (DL)
* Transparent AR Processing Acceleration at the Edge, EuroSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3301418.3313942) (DL)
* DeltaVR: Achieving High-Performance Mobile VR Dynamics through Pixel Reuse, IPSN 19 [[Paper]](https://sites.pitt.edu/~weigao/publications/ipsn19.pdf) (No ML)
* GLEAM: An Illumination Estimation Framework for Real-time Photorealistic Augmented Reality on Mobile Devices, MobiSys 19 [[Paper]](https://meteor.ame.asu.edu/publications/mobisys19prakash-gleam.pdf) (No ML)
* Freedom: Fast Recovery Enhanced VR Delivery Over Mobile Networks, MobiSys 19 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326087) (No ML)
* LpGL: Low-power Graphics Library for Mobile AR Headsets, MobiSys 19, [[Paper]](http://nsl.cau.ac.kr/~jpaek/docs/lpgl-mobisys2019.pdf) (No ML)
* Cutting the Cord: Designing a High-quality Untethered VR System with Low Latency Remote Rendering, MobiSys 18 [[Paper]](https://www.winlab.rutgers.edu/~gruteser/papers/mobisys18_low_latency_vr.pdf) (No ML)
* MARVEL: Enabling Mobile Augmented Reality with Low Energy and Low Latency, SenSys 18 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3274783.3274834) (No ML)
* Furion: Engineering High-Quality Immersive Virtual Reality on Today’s Mobile Devices, MobiCom 17 [[Paper]](https://www.cse.psu.edu/~gxc27/teach/597/Furion.pdf) (No ML)
* Enabling High-Quality Untethered Virtual Reality, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-abari.pdf) (No ML)
* FlashBack: Immersive Virtual Reality on Mobile Devices via Rendering Memoization, MobiSys 16 [[Paper]](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/06/flashback_mobisys2016.pdf) (No ML)

#### Omnidirectional AR
* SalientVR: Saliency-Driven Mobile 360-Degree Video Streaming with Gaze Information, MobiCom 22 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/salientvr_mobicom22.pdf) (DL)
* Xihe: a 3D vision-based lighting estimation framework for mobile augmented reality, MobiSys 21 [[Paper]](https://arxiv.org/pdf/2106.15280.pdf) (DL)

### AIoT Systems for Drones (Total: 25 | No ML(21) | ML(1) | DL(3))
<a name="aiot-systems-for-drones"></a>
* Anemoi: A Low-cost Sensorless Indoor Drone System for Automatic Mapping of 3D Airflow Fields,MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613292) (No ML)
* BatMobility: Towards Flying Without Seeing for Autonomous Drones, MobiCom 23 [[Paper]](https://arxiv.org/pdf/2307.11518.pdf) (DL)
* RF-Search: Searching Unconscious Victim in Smoke Scenes with RF-enabled Drone, MobiCom 23 [[Paper]](http://staff.ustc.edu.cn/~dongheng/dhfiles/2023RFSearch.pdf) (No ML)
* MilliSign: mmWave-Based Passive Signs for Guiding UAVs in Poor Visibility Conditions, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613264) (No ML)
* Taming Event Cameras with Bio-Inspired Architecture and Algorithm: A Case for Drone Obstacle Avoidance, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613269) (No ML)
* Placement Optimization for UAV-Enabled Wireless Networks with Multi-Hop Backhauls in Urban Environments, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a054/962400a054.pdf) (No ML)
* Wi-Drone: Wi-Fi-based 6-DoF Tracking for Indoor Drone Flight Control, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538936) (No ML)
* Reverse Engineering and Retrofitting Robotic Aerial Vehicle Control Firmware using DisPatch, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538938) (No ML)
* AIM: Acoustic Inertial Measurement for Indoor Drone Localization and Tracking, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568499) (No ML)
* MicNest: Long-Range Instant Acoustic Localization of Drones in Precise Landing, SenSys 22 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/2022.MicNest.pdf) (Best Paper Runner-up Award) (No ML)
* Throughput-Fairness Tradeoffs in Mobility Platforms, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3467881) (No ML)
* Quantifying the Design-Space Tradeoffs in Autonomous Drones, ASPLOS 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3445814.3446721) (No ML)
* Visage: Enabling Timely Analytics for Drone Imagery, MobiCom 21 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2021/09/Visage_Mobicom_2021.pdf) (DL)
* Bleep: motor-enabled audio side-channel for constrained UAVs, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419183) (No ML)
* C-14: Assured Timestamps for Drone Videos, MobiCom 20 [[Paper]](https://people.cs.umass.edu/~elm/papers/mobicom20-final809.pdf) (DL)
* BeeCluster: Drone Orchestration via Predictive Optimization, MobiSys 20 [[Paper]](http://people.csail.mit.edu/songtao/BeeCluster.pdf) (No ML)
* DroneScale: Drone Load Estimation via Remote Passive RF Sensing, SenSys 20 [[Paper]](http://mnslab.org/tamvu/paper/2020%20DroneScale_Phuc.pdf) (ML)
* FlyZone: A Testbed for Experimenting with Aerial Drone Application, MobiSys 19 [[Paper]](https://mottola.neslab.it/wp-content/uploads/2023/06/afanasov19flyzone.pdf) (No ML)
* TrackIO: Tracking First Responders Inside-Out, NSDI 19 [[Paper]](https://www.usenix.org/system/files/nsdi19-dhekne.pdf) (No ML)
* SkyCore: Moving Core to the Edge for Untethered and Reliable UAV-based LTE Networks, MobiCom 18 [[Paper]](https://dl.acm.org/doi/10.1145/3241539.3241549) (Best Paper Award) (No ML)
* Matthan: Drone Presence Detection by Identifying Physical Signatures in the Drone’s RF Communication, MobiSys 17 [[Paper]](http://mnslab.org/tamvu/paper/2017_Mobisys_Drone.pdf) (No ML)
* Indoor Follow Me Drone, MobiSys 17 [[Paper]](https://dl.acm.org/doi/10.1145/3081333.3081362) (Honorable Mention) (No ML)
* Argus: Realistic Target Coverage by Drones, IPSN 17 [[Paper]](https://saeed.github.io/files/argus_ipsn17.pdf) (No ML)
* Tracking Drone Orientation with Multiple GPS Receivers, MobiCom 16 [[Paper]](https://synrg.csl.illinois.edu/papers/drone-attitude-camera.pdf) (No ML)
* Reactive Control of Autonomous Drones, MobiSys 16 [[Paper]](https://mottola.neslab.it/wp-content/uploads/2023/06/bregu16reactive.pdf) (No ML) (Best Paper) 

### AIoT Systems for Satellites (Total: 7 | No ML(6) | ML(0) | DL(1))
<a name="aiot-systems-for-satellites"></a>
* Global Localization of Energy-Constrained Miniature RF Emitters using Low Earth Orbit Satellites, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625794) (No ML)
* A Networking Perspective on Starlink’s Self-Driving LEO Mega-Constellation, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3592519) (No ML)
* Transmitting, Fast and Slow: Scheduling Satellite Traffic through Space and Time, MobiCom 23 [[Paper]](https://deepakv.web.illinois.edu/assets/papers/umbra_mobicom_23.pdf) (No ML)
* PMSat: Optimizing Passive Metasurface for Low Earth Orbit Satellite Communication, MobiCom 23 [[Paper]](https://dl.acm.org/doi/10.1145/3570361.3613257) (No ML)
* GPSMirror: Expanding Accurate GPS Positioning to Shadowed and Indoor Regions with Backscatter, MobiCom 23 [[Paper]](https://arxiv.org/pdf/2304.07572.pdf) (No ML)
* SelfieStick: Towards Earth Imaging from a Low-Cost Ground Module Using LEO Satellites, IPSN 22 [[Paper]](https://swarunkumar.com/papers/selfiestick-ipsn2022.pdf) (DL)
* SOS: Isolated Health Monitoring System to Save Our Satellites, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3466862) (No ML)

### AIoT Systems for Agriculture (Total: 11 | No ML(8) | ML(2) | DL(1))
<a name="aiot-systems-for-agriculture"></a>
* Meta-Sticker: Sub-Terahertz Metamaterial Stickers for Non-Invasive Mobile Food Sensing, SenSys 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3625687.3625815) (No ML)
* AgriTera: Accurate Non-Invasive Fruit Ripeness Sensing via Sub-Terahertz Wireless Signals, MobiCom 23 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3570361.3613275) (ML) (Best Paper Award)
* DRLIC: Deep Reinforcement Learning for Irrigation Control, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a041/962400a041.pdf) (DL)
* IoTree: a battery-free wearable system with biocompatible sensors for continuous tree health monitoring, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3567652) (No ML)
* Estimating Soil Moisture using RF Signals, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3517025) (No ML) 
* LTE-Based Low-Cost and Low-Power Soil Moisture Sensing, SenSys 22 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/SenSys22-SoilMoisture.pdf) (No ML)
* Soil Moisture Sensing with Commodity RFID Systems, MobiSys 20 [[Paper]](http://web.cs.ucla.edu/~omid/Papers/Mobisys20.pdf) (No ML)
* Towards Low Cost Soil Sensing Using Wi-Fi, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345440) (No ML) (Honorable Mention)
* WISDOM: watering intelligently at scale with distributed optimization and modeling, SenSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3356250.3360023) (No ML)
* FarmBeats: An IoT Platform for Data-Driven Agriculture, NSDI 17 [[Paper]](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-vasisht.pdf) (ML)
* MAGIC: Model-Based Actuation for Ground Irrigation Control, IPSN 16 [[Paper]](https://faculty.ucmerced.edu/mcarreira-perpinan/papers/ipsn16.pdf) (No ML)

### AIoT Systems for Biology (Total: 9 | No ML(6) | ML(2) | DL(1))
<a name="aiot-systems-for-biology"></a>
* Towards Practical and Scalable Molecular Networks, SIGCOMM 23 [[Paper]](https://uwconnect.ece.wisc.edu/wp-content/uploads/sites/1525/2023/08/Towards-Practical-and-Scalable-Molecular-Networks.pdf) (ML)
* eTag: An Energy-Neutral Ear Tag for Real-Time Body Temperature Monitoring of Dairy Cattle, MobiCom 23 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3570361.3613262) (No ML)
* Wind dispersal of battery-free wireless devices, Nature 2022 [[Paper]](https://www.nature.com/articles/s41586-021-04363-9) (No ML)
* Vildehaye: A Family of Versatile, Widely-Applicable, and Field-Proven Lightweight Wildlife Tracking and Sensing Tags, IPSN 22 [[Paper]](https://conferences.computer.org/cpsiot/pdfs/IPSN2022-6R1M30NXCSXmbVKUqzz1Of/962400a001/962400a001.pdf) (No ML)
* mSAIL: milligram-scale multi-modal sensor platform for monarch butterfly migration tracking,	MobiCom	21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483263) (DL)	
* PigNet: Failure-Tolerant Pig Activity Monitoring System Using Structural Vibration, IPSN 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3412382.3458902) (ML)
* Airdropping Sensor Networks from Drones and Insects, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419981) (No ML)
* Estimating Heart Rate and Detecting Feeding Events of Fish Using an Implantable Biologger, IPSN 20 [[Paper]](https://research.csiro.au/dss/wp-content/uploads/sites/100/2020/02/Estimating_Heart_Rate_and_Detecting_Feeding_Events_of_Fish_Using_an_Implantable_Biologger-1.pdf) (No ML)
* Living IoT: A Flying Wireless Platform on Live Insects, MobiCom 19 [[Paper]](https://livingiot.cs.washington.edu/files/livingiot.pdf) (No ML)
