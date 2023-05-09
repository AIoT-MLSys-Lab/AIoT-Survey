# A collection of survey, research papers, benchmarks, open-source resources, and seminars of AIoT (Artificial Intelligence of Things)

Papers selected from the following conferences: 
- mobile computing and IoT conferences (MobiCom/MobiSys/SenSys/IPSN/UbiComp)
- computer networks conferences (NSDI/SIGCOMM) 
- computer systems conferences (OSDI/SOSP/EuroSys/ASPLOS/ATC)
- AI Systems conferences (MLSys)

Years: 2018 ~ Present

Find at most 10 papers in each sub-topic.

Each week, focus on Writing one sub-topic.


#### TODO  
* Re-organize the paper by its category (vision-sensing -> computing, video... and Lots of other sensing papers) (AR/Video/Vision?)
* Seems some "wifi network" paper goes to "wifi sensing" -> need double check 


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
* RetroIoT: Retrofitting Internet of Things Deployments by Hiding Data in Battery Readings, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560536) (NO ML) (Maybe new section battery?)
* Protean: An Energy-Efficient and Heterogeneous Platform for Adaptive and Hardware-Accelerated Battery-free Computing, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568561)
* zTT: learning-based DVFS with zero thermal throttling for mobile devices, MobiSys 21 [[Paper]](https://netstech.org/wp-content/uploads/2021/07/zTT_MobiSys21.pdf) (Best Paper)
* LIMU-BERT: Unleashing the Potential of Unlabeled Data for IMU Sensing Applications, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485937)
* TinyLink 2.0: Integrating Device, Cloud, and Client Development for IoT Applications, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3380890)
* Understanding power consumption of NB-IoT in the wild: tool and large-scale measurement, MobiCom 20 [[Paper]](https://www.cs.cityu.edu.hk/~jhuan9/papers/nbiot20mobicom.pdf) (NO ML)
* ePerceptive - Energy Reactive Embedded Intelligence for Batteryless Sensors, SenSys 20 [[Paper]](https://ubicomplab.cs.washington.edu/pdfs/ePerceptive.pdf)




## Sensing (MobiCom, MobiSys, SenSys, NSDI, UbiComp)

### Others
FabToys: plush toys with large arrays of fabric-based pressure sensors to enable fine-grained interaction detection, MobiSys 22 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/FabToy-MobiSys22.pdf)
* MagX: Wearable, Untethered Hands Tracking with Passive Magnets, MobiCom 21 [[Paper]](https://alansonsample.com/publications/docs/2021%20-%20MobiCom%20-%20MagX-%20Wearable,%20Untethered%20Hands%20Tracking%20with%20Passive%20Magnets.pdf) (using magnetic)
* BioFace-3D: Continuous 3D Facial Reconstruction Through Lightweight Single-ear Biosensors, MobiCom 21 [[Paper]](http://wsslab.org/vpnguyen/papers/bioface_2021.pdf) (Reconstruct 3D image using earphone shape bio-sensor)
* From relative azimuth to absolute location: pushing the limit of PIR sensor based localization, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3380878)
* General-purpose deep tracking platform across protocols for the internet of things	,	MobiSys	20	[[Paper]](https://www4.comp.polyu.edu.hk/~csyanglei/data/files/iark-mobisys20.pdf)
* MagHacker: Eavesdropping on Stylus Pen Writing via Magnetic Sensing from Commodity Mobile Devices, MobiSys 20 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobisys20.pdf)
* SkySense: Terrestrial and Aerial Spectrum Use Analysed Using Lightweight Sensing Technology with Weather Balloons, MobiSys 20 [[Paper]](https://www.lenders.ch/publications/conferences/mobisys20.pdf)
* Neuroplex: Learning to Detect Complex Events in Sensor Networks through Knowledge Injection, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3431158)




### UWB Sensing
* Mobi2Sense: Empowering Wireless Sensing with Mobility	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560518)	(NO	ML) (Best Paper Award Runner-ups) 
* Enabling High Accuracy Pervasive Tracking with Ultra Low Power UWB Tags, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560542) (NO ML) 
* WISE: Low-Cost Wide Band Spectrum Sensing Using UWB, SenSys 22 [[Paper]](https://huangqy7.github.io/Paper/WISE_final.pdf) (NO ML)
* SiWa: See into Walls via Deep UWB Radars, MobiCom 21 [[Paper]](https://arxiv.org/pdf/2110.14279.pdf)
* MoRe-Fi: Motion-robust and Fine-grained Respiration Monitoring via Deep-Learning UWB Radar, SenSys 21 [[Paper]](https://arxiv.org/pdf/2111.08195.pdf)
* UWHear: Through-wall Extraction and Separation of Audio Vibrations Using Wireless Signals, SenSys 20 [[Paper]](https://ziqi.plus/papers/UWHear.pdf) (NO ML)



### Wireless Sensing (Look at papers from Jie Xiong @ UMASS)
* Augmenting Augmented Reality with Non-Line-of-Sight Perception,	NSDI	23	[[Paper]](https://www.usenix.org/conference/nsdi23/presentation/boroushaki)	(NO	ML)
* Placement Matters: Understanding the Effects of Device Placement for WiFi Sensing	,	IMWUT/UbiComp	22	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3517237)	(NO	ML)
* Exploring Multiple Antennas for Long-range WiFi Sensing	,	IMWUT/UbiComp	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3494979)	(NO	ML)
* Motion inspires notion: self-supervised visual-LiDAR fusion for environment depth estimation	,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538918)		
* Empowering smart buildings with self-sensing concrete for structural health monitoring	,	SIGCOMM	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3544216.3544270)	(NO	ML)
* TyrLoc: a low-cost multi-technology MIMO localization system with a single RF chain	,	MobiSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467677)	(NO	ML)
* LTE-based Pervasive Sensing Across Indoor and Outdoor	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485943)	(NO	ML)
* UniTS: Short-Time Fourier Inspired Neural Networks for Sensory Time Series Classification	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485942)	
* Towards Position-Independent Sensing for Gesture Recognition with Wi-Fi, UbiComp 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3463504)
* Ember: energy management of batteryless event detection sensors with deep reinforcement learning	,	SenSys	20	[[Paper]](https://assets.amazon.science/60/cf/c743fa3b4078825ff4ec05120fe7/ember-energy-management-of-batteryless-event-detection-sensors-with-deep-reinforcement-learning.pdf)		
* Wi-fi see it all: generative adversarial network-augmented versatile wi-fi imaging, SenSys 20 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430725)
* RF-net: a unified meta-learning framework for RF-enabled one-shot human activity recognition	,	SenSys	20	[[Paper]](https://dl.acm.org/doi/10.1145/3384419.3430735)		
* On the Feasibility of Wi-Fi Based Material Sensing	,	MobiCom	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345442)(NO	ML)	
* FaHo: deep learning enhanced holographic localization for RFID tags	,	SenSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360035)		
* Achieving Receiver-Side Cross-Technology Communication with Cross-Decoding	,	MobiCom	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241547)	(NO	ML)
* Cross-Frequency Communication: Near-Field Identification of UHF RFIDs with WiFi!	,	MobiCom	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241569)		

#### General Wireless Sensing (Temporal subsubsectionn that using RF signal)
* LiqRay: non-invasive and fine-grained liquid recognition system, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560540)
* RISE: robust wireless sensing using probabilistic and statistical assessments, MobiCom 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483253)
* Octopus: a practical and versatile wideband MIMO sensing platform, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483267)




#### Bluetooth Sensing
* Experience: Practical Indoor Localization for Malls, MobiCom 22 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/mloc_mobicom22.pdf) (Best Community Contribution)
* Intermittently-powered bluetooth that works, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538934)



#### Wi-Fi Sensing
* Experience: pushing indoor localization from laboratory to the wild, MobiCom 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560546) (Best Community Contribution Runner-ups) (NO ML)
* Wiffract: A New Foundation for RF Imaging via Edge Tracing, MobiCom 22 [[Paper]](https://web.ece.ucsb.edu/~ymostofi/papers/PallaproluKoranyMostofi_MobiCom2022.pdf) (NO ML)
* RF-URL: unsupervised representation learning for RF sensing, MobiCom 22 [[Paper]](http://staff.ustc.edu.cn/~dongheng/dhfiles/rf-url.pdf)
* Wi-drone: wi-fi-based 6-DoF tracking for indoor drone flight control, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538936)
* Wi-Mesh: A WiFi Vision-based Approach for 3D Human Mesh Construction, SenSys 22 [[Paper]](https://arxiv.org/pdf/2210.10957.pdf)
* SiFall: Practical Online Fall Detection with RF Sensing, SenSys 22 [[Paper]](https://arxiv.org/pdf/2301.03773.pdf)
* Solving the WiFi Sensing Dilemma in Reality Leveraging Conformal Prediction, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568529)
* WiBeacon: Expanding BLE Location-based Services via WiFi, MobiCom 21 [[Paper]](https://liux4189.github.io/files/WiBeacon_MobiCom_CameraReady.pdf) (NO ML)
* Counting a stationary crowd using off-the-shelf wifi, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3468012) (NO ML)
* OneFi: One-Shot Recognition for Unseen Gesture via COTS WiFi, SenSys 21 [[Paper]](https://ruixiao24.github.io/files/rui_onefi.pdf)
* Deep learning based wireless localization for indoor navigation, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3380894)
* SDR receiver using commodity wifi via physical-layer signal reconstruction, MobiCom 20 [[Paper]](https://seit.egr.msu.edu/paper/Mobicom2020-SDRLite.pdf)
* Towards 3D human pose construction using wifi, MobiCom 20 [[Paper]](https://cse.buffalo.edu/~lusu/papers/MobiCom2020.pdf)
* Wi-Fi See It All: Generative Adversarial Network-augmented Versatile Wi-Fi Imaging, SenSys 20 [[Paper]](https://cse.msu.edu/~caozc/papers/sensys20-chen.pdf)
* Proximity Detection with Single-Antenna IoT Devices, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300120) (NO ML)
* mD-Track: Leveraging Multi-Dimensionality for Passive Indoor Wi-Fi Tracking, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300133) (NO ML)
* On the Feasibility of Wi-Fi Based Material Sensing, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345442)
* Zero-Effort Cross-Domain Gesture Recognition with Wi-Fi, MobiSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3307334.3326081)




#### RFID Sensing
* RF-DNA: Large-Scale Physical-layer Identifications of RFIDs via Dual Natural Attributes, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3517028)
* MetaSight: Localizing Blocked RFID Objects by Modulating NLOS Signals via Metasurfaces, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538947) (NO ML)
* A Passive Eye-in-Hand “Camera” for Minature Robots, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568505)
* Thermotag: item-level temperature sensing with a passive RFID tag, MobiSys 21 [[Paper]](https://cs.nju.edu.cn/liujia/papers/mobisys21-themotag.pdf)
* RFGo: A Seamless Self-checkout System for Apparel Stores Using RFID, MobiCom 20 [[Paper]](https://genesys-lab.org/papers/RFGo-Mobicom.pdf)
* Exploring commodity RFID for contactless sub-millimeter vibration sensing, SenSys 20 [[Paper]](https://dl.acm.org/doi/10.1145/3384419.3430771) (NO ML)
* Sensing Finger Input Using An RFID Transmission Line, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430712) (NO ML)
* RTSense: RFID based Temperature Sensing, SenSys 20 [[Paper]](https://www.swadhinpradhan.com/papers/rtsense.pdf) (NO ML)
* Are RFID Sensing Systems Ready for the Real World?, MobiSys 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3307334.3326084)
* Detecting Misplaced RFID Tags on Static Shelved Items, MobiSys 19 [[Paper]](https://rtcl.eecs.umich.edu/rtclweb/assets/publications/2019/luo-mobisys19.pdf)




#### mmWave Sensing
* Mask Does Not Matter: Anti-Spoofing Face Authentication using mmWave without On-site Registration, MobiCom 22 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/mmFace-MobiCom22.pdf) (NO ML)
* mmEve: Eavesdropping on Smartphone's Earpiece via COTS mmWave Device, MobiCom 22 [[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-mobicom2022.pdf)
* Augmenting mmWave localization accuracy through sub-6 GHz on off-the-shelf devices, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538920) (NO ML)
* m3Track:mmWave-based Multi-User 3D Posture Tracking, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538926)
* M4esh: mmWave-Based 3D Human Mesh Construction for Multiple Subjects	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568545)	
* M5: Facilitating Multi-user Volumetric Content Delivery with Multi-lobe Multicast over mmWave, SensSys 22 [[Paper]](http://www.phpathak.com/files/m5-sensys.pdf)
* SpaceBeam: LiDAR-driven one-shot mmWave beam management, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3466864)
* Synthesized Millimeter-Waves for Human Motion Sensing, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568542)
* mmMesh: towards 3D real-time dynamic human mesh construction using millimeter-wave, MobiSys 21 [[Paper]](https://dl.acm.org/doi/10.1145/3458864.3467679)
* Millimetro: mmWave Retro-Reflective Tags for Accurate, Long Range Localization, MobiCom21 [[Paper]](https://swarunkumar.com/papers/millimetro-mobicom2021.pdf) (NO ML)
* ThermoWave: A New Paradigm of Wireless Passive Temperature Monitoring via mmWave Sensing, MobiCom 20 [[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-mobicom2020b.pdf) (NO ML)
* M-Cube: a millimeter-wave massive MIMO software radio, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3380892) (NO ML) (Best Papaer Award)
* mm-FLEX: An Open Platform for Millimeter-Wave Mobile Full-Bandwidth Experimentation, MobiSys 20 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/808/MOBISYS_2020_FINAL.pdf?sequence=1&isAllowed=y) (NO ML)
* See through smoke: robust indoor mapping with low-cost mmWave radar	,	MobiSys	20	[[Paper]](https://arxiv.org/pdf/1911.00398.pdf)
* Osprey: A mmWave Approach to Tire Wear Sensing, MobiSys 20 [[Paper]](https://swarunkumar.com/papers/osprey-mobisys2020.pdf)	
* WaveEar: Exploring a mmWave-based Noise-resistant Speech Sensing for Voice-User Interface, MobiSys 19 [[Paper]](https://www.acsu.buffalo.edu/~huiningl/papers/waveear2019.pdf)	




#### TeraHertz Sensing
* Quasi-Optical 3D localization using Asymmetric Signatures above 100 GHz, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3517022) (NO ML)
* LeakyTrack: Non-Coherent Single-Antenna Nodal and Environmental Mobility Tracking with a Leaky-Wave Antenna, SenSys 20 [[Paper]](https://www.brown.edu/research/labs/mittleman/sites/brown.edu.research.labs.mittleman/files/uploads/SenSys_2020.pdf) (NO ML)

### Earables Sensing (Look at papers from Romit @ UIUC)
* Sensing with Earables: A Systematic Literature Review and Taxonomy of Phenomena, IMWUT 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3550314)
* ClearBuds: wireless binaural earbuds for learning-based speech enhancement	,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538933)	
* EarGate: Gait-based User Identification with In-ear Microphones, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483240)
* HeadFi: bringing intelligence to all headphones, MobiCom 21	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3448624) (NO ML)	(Best Paper Award Runner-up)
* Personalizing Head Related Transfer Functions for Earables, SIGCOMM 21 [[Paper]](https://synrg.csl.illinois.edu/papers/UNIQ_Sigcomm21.pdf) (NO ML)
* OESense: employing occlusion effect for in-ear human sensing, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3467680)
* Ear-AR: indoor acoustic augmented reality on earphones, MobiCom 20 [[Paper]](https://synrg.csl.illinois.edu/papers/ear-ar_mobicom20.pdf) (NO ML)
* EarSense: earphones as a teeth activity sensor, MobiCom 20 [[Paper]](https://synrg.csl.illinois.edu/papers/earsense_mobicom20.pdf) (NO ML)
* WAKE: A Behind-the-ear Wearable System for Microsleep Detection, MobiSys 20 [[Paper]](http://mnslab.org/tamvu/paper/2020%20WAKE_Nhat.pdf)
* EarphoneTrack: involving earphones into the ecosystem of acoustic motion tracking, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430730) (NO ML)
* ERICA: Enabling Real-time Mistake Detection & Corrective Feedback for Free-Weights Exercises, SenSys 20 [[Paper]](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=6897&context=sis_research)
* eBP: A Wearable System For Frequent and Comfortable Blood Pressure Monitoring From User's Ear, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345454) (NO ML) (Best Paper)



### Acoustic Sensing							
* Acoustic Sensing and Communication Using Metasurface	,	NSDI	23	[[Paper]](https://www.usenix.org/system/files/nsdi23-zhang-yongzhao.pdf)
* Hybrid Neural Networks for On-device Directional Hearing	,	AAAI	22	[[Paper]](https://arxiv.org/abs/2112.05893)[[Code]](https://github.com/wanganran/HybridBeam)			
* LASense: Pushing the Limits of Fine-grained Activity Sensing Using Acoustic Sign	,	IMWUT/UbiComp	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3517253)	(NO	ML)	
* Experience: practical problems for acoustic sensing	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560527)(NO	ML)				
* SPiDR: ultra-low-power acoustic spatial sensing for micro-robot navigation	,	MobiSys	22	[[Paper]](https://www.cs.umd.edu/~nakul/assets/papers/spidr_mobisys2022_nakul.pdf)	(NO	ML) (Best Paper)
* SQEE: A Machine Perception Approach to Sensing Quality Evaluation at the Edge by Uncertainty Quantification	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568534)
* Room-scale Hand Gesture Recognition Using Smart Speakers, SenSys 22 [[Paper]](https://people.cs.umass.edu/~dli/papers/SenSys2022_SpeakerGesture.pdf)
* AIM: Acoustic Inertial Measurement for Indoor Drone Localization and Tracking, SenSys 22 [[Paper]](https://mottola.faculty.polimi.it/papers/sun22aim.pdf)
* Indoor Smartphone SLAM with Learned Echoic Location Features, SenSys 22 [[Paper]](https://arxiv.org/pdf/2210.08493.pdf)
* MicNest: Long-Range Instant Acoustic Localization of Drones in Precise Landing, SenSys 22 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/2022.MicNest.pdf)
* SVoice: Enabling Voice Communication in Silence via Acoustic Sensing on Commodity Devices	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568530)	
* SpeechQoE: A Novel Personalized QoE Assessment Model for Voice Services via Speech Sensing, SenSys 22 [[Paper]](https://ranger.uta.edu/~mingli/publications/SpeechQoE.pdf)
* Telesonar: Robocall Alarm System by Detecting Echo Channel and Breath Timing, SenSys 22 [[Paper]](https://yanzhenyu.com/assets/pdf/Telesonar-SenSys22.pdf) (NO ML)		
* Enabling Contact-free Acoustic Sensing under Device Motion	,	UbiComp	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3550329)(NO	ML)		
* Microphone Array Backscatter: An Application-Driven Design for Lightweight Spatial Sound Recording over the Air, MobiCom 21 [[Paper]](https://www2.cs.sfu.ca/~jcliu/Papers/Microphone21.pdf) (NO ML)
* Owlet: enabling spatial information in ubiquitous acoustic devices	,	MobiSys	21	[[Paper]](https://www.cs.umd.edu/~nirupam/images/2_publication/papers/Owlet_MobiSys21_nirupam.pdf)	
* MAVL: Multiresolution Analysis of Voice Localization	,	NSDI	21	[[Paper]](https://www.usenix.org/system/files/nsdi21-wang-mei.pdf)	(NO	ML)	
* Voice Localization Using Nearby Wall Reflections, MobiCom 20 [[Paper]](https://synrg.csl.illinois.edu/papers/voloc_mobicom20.pdf)
* Deaf-aid: mobile IoT communication exploiting stealthy speaker-to-gyroscope channel, MobiCom 20 [[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-mobicom2020c.pdf) (NO ML)
* AcuTe: acoustic thermometer empowered by a single smartphone, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430714#:~:text=AcuTe%20empowers%20a%20single%20smartphone,between%20temperature%20and%20sound%20speed.)
* Symphony: Localizing Multiple Acoustic Sources with a Single Microphone Array, SenSys 20 [[Paper]](https://arxiv.org/pdf/2209.15325.pdf) (NO ML)
* FM-Track: Pushing the Limits of Contactless Multi-target Tracking using Acoustic Signals, SenSys 20 [[Paper]](https://people.cs.umass.edu/~dli/papers/SenSys20_FM-Track.pdf) (NO ML)
* Patronus: Preventing Unauthorized Speech Recordings with Support for Selective Unscrambling, SenSys 20 [[Paper]](https://cse.msu.edu/~caozc/papers/sensys20-ling.pdf)
* Rebooting Ultrasonic Positioning Systems for Ultrasound-incapable Smart Devices, MobiCom 19 [[Paper]](https://arxiv.org/pdf/1812.02349.pdf) (NO ML)
* RNN-Based Room Scale Hand Motion Tracking, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345439)
* BreathListener: Fine-grained Breathing Monitoring in Driving Environments Utilizing Acoustic Signals, MobiSys 19 [[Paper]](https://www.cs.sjtu.edu.cn/~linghe.kong/2019/XuMOBISYS2019BreathListener.pdf)
* Animal-Borne Anti-Poaching System, MobiSys 19 [[paper]](https://dl.acm.org/doi/pdf/10.1145/3307334.3326080) (NO ML)
* MetaSense: few-shot adaptation to untrained conditions in deep mobile sensing	,	SenSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360020)			
* In-body backscatter communication and localization	,	SIGCOMM	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3230543.3230565)	(NO	ML)	
							
							
### Vision Sensing		
* MoiréPose: Ultra High Precision Camera-to-Screen Pose Estimation based on Moiré Pattern, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560537) (NO ML)
* CORE-lens: simultaneous communication and object recognition with disentangled-GAN cameras, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560526)
* DoCam: Depth Sensing with an Optical Image Stabilization Supported RGB Camera, MobiCom 22 [[Paper]](https://www.cs.sjtu.edu.cn/~yichao/assets/publications/mobicom22_pan.pdf)
* MobiDepth: Real-Time Depth Estimation Using On-Device Dual Cameras, MobiCom 22 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2022/09/mobicom22-final138.pdf)
* Detecting Counterfeit Liquid Food Products in a Sealed Bottle Using a Smartphone Camera, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3539776)
* DeepMix: mobility-aware, lightweight, and hybrid 3D object detection for headsets, MobiSys 22 [[Paper]](https://arxiv.org/pdf/2201.08812.pdf)
* Gaze Tracking on Any Surface with Your Phone, SenSys 22 [[Paper]](https://www.cs.cityu.edu.hk/~zhenjili/2022-SenSys-ASGaze.pdf)
* Large-Scale Vehicle Trajectory Reconstruction with Camera Sensing Network, MobiCom 21 [[Paper]](https://wands.sg/publications/full_list/papers/MobiCom_21_1.pdf)
* Xihe: a 3D vision-based lighting estimation framework for mobile augmented reality, MobiSys 21 [[Paper]](https://arxiv.org/pdf/2106.15280.pdf)
* MotionCompass: pinpointing wireless camera via motion-activated traffic, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3467683)
* LAPD: Hidden Spy Camera Detection using Smartphone Time-of-Flight Sensors, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485941)
* UltraDepth: Exposing High-Resolution Texture from Depth Cameras, SenSys 21 [[Paper]](http://cvlab.cse.msu.edu/pdfs/Xie_Ouyang_Liu_Xing_UltraDepth_SenSys2021.pdf)
* FaceRevelio: a face liveness detection system for smartphones with a single front camera, MobiCom 20 [[Paper]](https://habiba-farrukh.github.io/files/FaceRevelio.pdf)
* Rhythmic pixel regions: multi-resolution visual sensing system towards high-precision visual computing at low power	,	ASPLOS	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3445814.3446737)			
* Approximate query service on autonomous IoT cameras	,	MobiSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388948)
* Starfish: resilient image compression for AIoT cameras	,	SenSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430769)	
* GazeGraph: Graph-based Few-Shot Cognitive Context Sensing from Human Visual Behavior, SenSys 20 [[Paper]](https://par.nsf.gov/servlets/purl/10296635)
* Banner: An Image Sensor Reconfiguration Framework for Seamless Resolution-based Tradeoffs,	MobiSys	19	[[Paper]](https://meteor.ame.asu.edu/publications/mobisys19hu-banner.pdf) (NO ML)
* Liquid Testing with Your Smartphone, MobiSys 19 [[Paper]](https://people.csail.mit.edu/scyue/projects/capcam/capcam.pdf)


### Under Water Sensing (Look at papers from Fadel @ MIT)
* Unsupervised Underwater Image Restoration: From a Homology Perspective, AAAI 22 [[Paper]](https://ojs.aaai.org/index.php/AAAI/article/view/19944)
* Sunflower: Locating Underwater Robots From the Air,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3539773)
* Learning To Remove Refractive Distortions From Underwater Images, ICCV 21 [[Paper]](https://openaccess.thecvf.com/content/ICCV2021/html/Thapa_Learning_To_Remove_Refractive_Distortions_From_Underwater_Images_ICCV_2021_paper.html)
* Restoration of Non-Rigidly Distorted Underwater Images Using a Combination of Compressive Sensing and Local Polynomial Image Representations, ICCV 19 [[Paper]](https://openaccess.thecvf.com/content_ICCV_2019/html/James_Restoration_of_Non-Rigidly_Distorted_Underwater_Images_Using_a_Combination_of_ICCV_2019_paper.html)
* Surface Normals and Shape From Water, ICCV 19 [[Paper]](https://openaccess.thecvf.com/content_ICCV_2019/html/Murai_Surface_Normals_and_Shape_From_Water_ICCV_2019_paper.html)


### Visible Light Sensing (Look at papers from Xia Zhou @ Columbia)	
* Bracelet+: Harvesting the Leaked RF Energy in VLC with Wearable Bracelet Antenna, SenSys 22 [[Paper]](https://people.cs.umass.edu/~minhaocui/sensys22.pdf)
* Harmony: An In-band Time Synchronisation System for Visible Light Communication, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568549) (NO ML)
* RadioInLight: Doubling the Data Rate of VLC Systems, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483271) (NO ML)
* Lili: Liquor Quality Monitoring Based on Light Signals, MobiCom 21 [[Paper]](https://www.huangyongzhi.com.cn/data/Lili.pdf) (NO ML)
* SMART: Screen-based Gesture Recognition on Commodity Mobile Devices, MobiCom 21 [[Paper]](https://huangqy7.github.io/Paper/mobicom21-SMART.pdf)
* CurveLight:An Accurateand Practical Light Positioning System, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485934) (NO ML)
* SpiderWeb: Enabling Through-Screen Visible Light Communication, SenSys 21 [[Paper]](https://pure.tudelft.nl/ws/portalfiles/portal/103302355/3485730.3485948.pdf) (NO ML)
* LiTag: Localization and Posture Estimation with Passive Visible Light Tags, SenSys 20 [[Paper]](https://www.cse.msu.edu/~lilingk1/publications/sensys20-LiTag.pdf)
* Breaking the Limitations of Visible Light Communication Through Its Side Channel, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430728)
		
							
							
							
### Multi-modal Sensing							
* Cosmo: contrastive fusion learning with small data for multimodal human activity recognition,	MobiCom	22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560519)
* Capricorn: Towards Real-Time Rich Scene Analysis Using RF-Vision Sensor Fusion	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568504)			
* mSAIL: milligram-scale multi-modal sensor platform for monarch butterfly migration tracking,	MobiCom	21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483263)			
* UltraSE: single-channel speech enhancement using ultrasound, MobiCom 21 [[Paper]](http://xyzhang.ucsd.edu/papers/Ke.Sun_MobiCom21_UltraSE.pdf)	
* RFID and camera fusion for recognition of human-object interactions, MobiCom	21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483244)			
* Low-latency speculative inference on distributed multi-modal data streams	,	MobiSys	21	[[Paper]](https://dl.acm.org/doi/10.1145/3458864.3467884)
* ITrackU: tracking a pen-like instrument via UWB-IMU fusion, MobiSys 21 [[Paper]](https://faculty.cc.gatech.edu/~dhekne/itracku_mobisys2021.pdf) (NO ML)		
* Wavoice: A Noise-resistant Multi-modal Speech Recognition System Fusing mmWave and Audio Signals	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485945)
* RFusion:Robotic Grasping via RF-Visual Sensing and Learning, SenSys 21 [[Paper]](https://www.mit.edu/~fadel/papers/RFusion-paper.pdf)	
* Personalizing head related transfer functions for earables	,	SIGCOMM	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3452296.3472907)
* * milliEgo: single-chip mmWave radar aided egomotion estimation via deep sensor fusion	,	SenSys	20	[[Paper]](https://arxiv.org/pdf/2006.02266.pdf)		
* XModal-ID: Using WiFi for Through-Wall Person Identification from Candidate Video Footage, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345437)	
* Real-time Arm Skeleton Tracking and Gesture Inference Tolerant to Missing Wearable Sensors	,	MobiSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326109)			
* SenseHAR: a robust virtual activity sensor for smartphones and wearables	,	SenSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360032)			
* A closer look at quality-aware runtime assessment of sensing models in multi-device environments	,	SenSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360043)		
* VSkin: Sensing Touch Gestures on Surfaces of Mobile Devices Using Acoustic Signals	,	MobiCom	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241568)	(NO	ML)	
* CrowdEstimator: Approximating Crowd Sizes with Multi-modal Data for Internet-of-Things Services	,	MobiSys	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210320)	(NO	ML)	
* EngageMon: Multi-Modal Engagement Sensing for Mobile Games	,	UbiComp	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3191745)	(NO	ML)	
* Indoor localization via multi-modal sensing on smartphones	,	UbiComp	16	[[Paper]](https://dl.acm.org/doi/abs/10.1145/2971648.2971668)			
							
							
							
							
							
## Computing							
	
### Others

### ML Systems	
* A Unified Architecture for Accelerating Distributed DNN Training in Heterogeneous GPU/CPU Clusters	,	OSDI	20	[[Paper]](https://www.usenix.org/system/files/osdi20-jiang.pdf)		


### On-Device Inferences							
#### Scheduling							

#### Multi-tenant Inference	

#### Cross-Processor Inference

* ARK: GPU-driven Code Execution for Distributed Deep Learning	,	NSDI	23	[[Paper]](https://www.usenix.org/conference/nsdi23/presentation/hwang)			
* GPUReplay: a 50-KB GPU stack for client ML, ASPLOS	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507754)			
* VELTAIR: towards high-performance multi-tenant deep learning services via adaptive compilation and scheduling, ASPLOS	22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507752)		
* CoDL: Efficient CPU-GPU Co-execution for Deep Learning Inference on Mobile Devices, MobiSys 22 [[Paper]](https://chrisplus.me/assets/pdf/mobisys22-CoDL.pdf)
* Band: Coordinated Multi-DNN Inference on Heterogeneous Mobile Processors, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538948)
* Microsecond-scale Preemption for Concurrent GPU-accelerated DNN Inferences	,	OSDI	22	[[Paper]](https://www.usenix.org/conference/osdi22/presentation/han)			
* BlastNet: Exploiting Duo-Blocks for Cross-Processor Real-Time DNN Inference	,	SenSys	22	[[Paper]](https://yanzhenyu.com/assets/pdf/BlastNet-SenSys22.pdf)
* Adaptive Intelligence for Batteryless Sensors Using Software-Accelerated Tsetlin Machines, SenSys 22 [[Paper]](https://alessandro-montanari.github.io/papers/sensys2022.pdf)
* ElasticAI-Creator: Optimizing Neural Networks for Time-Series-Analysis for on-Device Machine Learning in IoT Systems	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568296)			
* IOS: Inter-Operator Scheduler for CNN Acceleration	,	MLSys	21	[[Paper]](https://proceedings.mlsys.org/paper_files/paper/2021/hash/38b3eff8baf56627478ec76a704e9b52-Abstract.html)	
* AsyMo: Scalable and Efficient Deep-Learning Inference on Asymmetric Mobile CPUs , MobiCom 21 [[Paper]]([https://dl.acm.org/doi/abs/10.1145/3447993.3448625](https://www.msra.cn/wp-content/uploads/2021/03/mobicom21-asymo.pdf))
* nn-Meter: towards accurate latency prediction of deep-learning model inference on diverse edge devices, MobiSys 21 [[Paper]](https://air.tsinghua.edu.cn/pdf/nn-Meter-Towards-Accurate-Latency-Prediction-of-Deep-Learning-Model-Inference-on-Diverse-Edge-Devices.pdf) (Best Paper)		
* MNN: A Universal and Efficient Inference Engine, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/8f14e45fceea167a5a36dedd4bea2543-Paper.pdf)
* μLayer: Low Latency On-Device Inference Using Cooperative Single-Layer Acceleration and Processor-Friendly Quantization	,	EuroSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3302424.3303950)			
* TicTac: Accelerating Distributed Deep Learning with Communication Scheduling	,	MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/index.html#schedule)			
* Efficient Deep Learning Inference on Edge Devices	,	MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/29.pdf)		
* FastDeepIoT: Towards Understanding and Optimizing Neural Network Execution Time on Mobile and Embedded Devices	,	SenSys	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3274783.3274840)	

#### Applications

* Heimdall: mobile GPU coordination platform for augmented reality applications, MobiCom 20 [[Paper]](https://juheonyi.github.io/files/Heimdall.pdf)
* MobiPose: real-time multi-person pose estimation on mobile devices,	SensSys20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430726)	
* MobiSR: Efficient On-Device Super-Resolution through Heterogeneous Mobile Processors, MobiCom 19 [[Paper]](https://arxiv.org/pdf/1908.07985.pdf)
* DeQA: On-Device Question Answering, MobiSys 19 [[Paper]](https://www3.cs.stonybrook.edu/~arunab/papers/deqa.pdf)
		
	
							
							
#### Hardware Accelerators							
							
							
#### Memory Optimization							

* mGEMM: Low-latency Convolution with Minimal Memory Overhead Optimized for Mobile Devices, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538940)

							
#### Model Compression							

* Mistify: Automating DNN Model Porting for On-Device Inference at the Edge, NSDI 2021	[[Paper]](https://www.usenix.org/system/files/nsdi21-guo.pdf)	
* BiSon-e: a lightweight and high-performance accelerator for narrow integer linear algebra computing on the edge	,	ASPLOS	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3503222.3507746)			
* Bit-serial Weight Pools: Compression and Arbitrary Precision Execution of Neural Networks on Resource Constrained Processors, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/502e4a16930e414107ee22b6198c578f-Paper.pdf)
* NeuLens: spatial-based dynamic acceleration of convolutional neural networks on edge, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560528)
* SparTA: Deep-Learning Model Sparsity via Tensor-with-Sparsity-Attribute	,	OSDI	22	[[Paper]](https://www.usenix.org/system/files/osdi22-zheng-ningxin.pdf)			
* Memory-Efficient Domain Incremental Learning for Internet of Things	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568436)			
* LegoDNN: block-grained scaling of deep neural networks for mobile vision,	MobiCom	21 [[Paper]](https://arxiv.org/pdf/2112.09852.pdf) (Best Community Paper Award Runner-Up)		
* RT-mDL: Supporting Real-Time Mixed Deep Learning Tasks on Edge Platforms	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485938)			
* LIMU-BERT: Unleashing the Potential of Unlabeled Data for IMU Sensing Applications	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485937)			
* PCONV: The Missing but Desirable Sparsity in DNN Weight Pruning for Real-Time Execution on Mobile Devices	,	AAAI	20	[[Paper]](https://ojs.aaai.org/index.php/AAAI/article/view/5954)	
* PatDNN: Achieving Real-Time DNN Execution on Mobile Devices with Pattern-based Weight Pruning	,	ASPLOS	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3373376.3378534)			
* Fast and scalable in-memory deep multitask learning via neural weight virtualization	,	MobiSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3386901.3388947)			
* Memory-Driven Mixed Low Precision Quantization for Enabling Deep Network Inference on Microcontrollers, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/9b8619251a19057cff70779273e95aa6-Paper.pdf)
* Learning Compressed Embeddings for On-Device Inference, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/812b4ba287f5ee0bc9d43bbf5bbe87fb-Paper.pdf)
* MDLdroidLite: a release-and-inhibit control approach to resource-efficient deep neural networks on mobile devices	,	SenSys	20	[[Paper]](https://taogu.site/pub/paper/Paper_3_SenSys_2020.pdf)			
* ApproxDet: Content and Contention-Aware Approximate Object Detection for Mobiles, SenSys 20 [[Paper]](https://arxiv.org/pdf/2010.10754.pdf)
* Intelligence Beyond the Edge: Inference on Intermittent Embedded Systems	,	ASPLOS	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3297858.3304011)			
* ADMM-NN: An Algorithm-Hardware Co-Design Framework of DNNs Using Alternating Direction Methods of Multipliers	,	ASPLOS	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3297858.3304076)	
* Full deep neural network training on a pruned weight budget	,	MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/135.pdf)			
* Accurate and Efficient 2-bit Quantized Neural Networks	,	MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/168.pdf)			
* Ternary Hybrid Neural-Tree Networks for Highly Constrained IoT Applications	,	MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/107.pdf)			
* DeepThin: A Self-Compressing Library for Deep Neural Networks	,	MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/33.pdf)
* NestDNN: Resource-Aware Multi-Tenant On-Device Deep Learning for Continuous Mobile Vision, MobiCom 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241559)			
* On-Demand Deep Model Compression for Mobile Devices: A Usage-Driven Model Selection Framework	,	MobiSys	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210337)			
							
							
							
### On-Device Training							
* Campo: Cost-Aware Performance Optimization for Mixed-Precision Neural Network Training	,	ATC	22	[[Paper]](https://www.usenix.org/system/files/atc22-he.pdf)			
* Mandheling: mixed-precision on-device DNN training with DSP offloading	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3560545)			
* Memory-efficient DNN Training on Mobile Device, MobiSys	22	[[Paper]](https://dl.acm.org/doi/10.1145/3498361.3539765)		
* Melon: breaking the memory wall for resource-efficient on-device machine learning, MobiSys 22 [[Paper]](https://xumengwei.github.io/files/MobiSys22-Melo.pdf)
* URSABench: A System for Comprehensive Benchmarking of Bayesian Deep Neural Network Models and Inference methods, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/hash/3ef815416f775098fe977004015c6193-Abstract.html)	
* ML-EXray: Visibility into ML Deployment on the Edge, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/76dc611d6ebaafc66cc0879c71b5db5c-Paper.pdf)
* MLPerf Mobile Inference Benchmark, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/7eabe3a1649ffa2b3ff8c02ebfd5659f-Paper.pdf)
* Octo: INT8 Training with Loss-aware Compensation and Backward Quantization for Tiny On-device Learning	,	ATC	21	[[Paper]](https://www.usenix.org/conference/atc21/presentation/zhou-qihua)			
* Mercury: Efficient On-Device Distributed DNN Training via Stochastic Importance Sampling	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485930)			
* Trained Quantization Thresholds for Accurate and Efficient Fixed-Point Inference of Deep Neural Networks, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/e2c420d928d4bf8ce0ff2ec19b371514-Paper.pdf)
							

							
### Edge-Cloud Offloading							
* InFi: end-to-end learnable input filter for resource-efficient mobile-centric inference	,	MobiCom	22	[[Paper]]([https://dl.acm.org/doi/abs/10.1145/3495243.3517016](https://yuanmu97.github.io/preprint/InFi_MobiCom22.pdf))	
* Real-time Neural Network Inference on Extremely Weak Devices: Agile Offloading with Explainable AI, MobiCom 22 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobicom22.pdf)
* Walle: An End-to-End,  General-Purpose,  and Large-Scale Production System for Device-Cloud Collaborative Machine Learning	,	OSDI	22	[[Paper]](https://www.usenix.org/system/files/osdi22-lv.pdf)			
* PriMask: Cascadable and Collusion-Resilient Data Masking for Mobile Cloud Inference, SenSys 22 [[Paper]](https://arxiv.org/pdf/2211.06716.pdf)	
* Elf: accelerate high-resolution mobile deep vision with content-aware parallel offloading, MobiCom 21 [[Paper]]([https://dl.acm.org/doi/abs/10.1145/3447993.3448628](https://www.msra.cn/wp-content/uploads/2021/03/mobicom21-elf.pdf)	
* Visage: Enabling Timely Analytics for Drone Imagery, MobiCom 21 [[Paper]](https://www.microsoft.com/en-us/research/uploads/prod/2021/09/Visage_Mobicom_2021.pdf) 			
* CLIO: enabling automatic compilation of deep learning pipelines across IoT and cloud	,	MobiCom	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3372224.3419215)	
* SPINN: synergistic progressive inference of neural networks over device and cloud, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419194)		
* EagleEye: wearable camera-based person identification in crowded urban spaces, MobiCom 20 [[Paper]](https://juheonyi.github.io/files/EagleEye.pdf)
* Deep compressive offloading: speeding up neural network inference by trading edge computation for network latency	,	SenSys	20	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3384419.3430898)			
* Source Compression with Bounded DNN Perception Loss for IoT Edge Computer Vision	,	MobiCom	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3300061.3345448)			
* Neuro.ZERO: a zero-energy neural network accelerator for embedded sensing and inference systems	,	SenSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360030)		
* Distributed Placement of Machine Learning Operators for IoT applications spanning Edge and Cloud Resources	,	MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/204.pdf)	
* FoggyCache: Cross-Device Approximate Computation Reuse	,	MobiCom	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3241539.3241557)			
							
							
							
							
							
### Automated Machine Learning (AutoML) for AIoT								
							
* Towards The Co-design of Neural Networks and Accelerators, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/31fefc0e570cb3860f2a6d4b38c6490d-Paper.pdf)			
* Improving Model Training with Multi-fidelity Hyperparameter Evaluation, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/a3c65c2974270fd093ee8a9bf8ae7d0b-Paper.pdf)	
* MicroNets: Neural Network Architectures for Deploying TinyML Applications on Commodity Microcontrollers	,	MLSys	21	[[Paper]](https://proceedings.mlsys.org/paper_files/paper/2021/hash/a3c65c2974270fd093ee8a9bf8ae7d0b-Abstract.html)			
* Searching for Winograd-aware Quantized Networks, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/45c48cce2e2d7fbdea1afc51c7c6ad26-Paper.pdf)
* SkyNet: a Hardware-Efficient Method for Object Detection and Tracking on Embedded Systems, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/93db85ed909c13838ff95ccfa94cebd9-Paper.pdf)
* MCUNet: Tiny Deep Learning on IoT Devices	,	NeurIPS	20	[[Paper]](https://proceedings.neurips.cc/paper/2020/hash/86c51678350f656dcc7f490a43946ee5-Abstract.html)		
* Does Unsupervised Architecture Representation Learning Help Neural Architecture Search?, NeurIPS 20 [[Paper]](https://proceedings.neurips.cc/paper/2020/hash/937936029af671cf479fa893db91cbdd-Abstract.html)	
* HM-NAS: Efficient Neural Architecture Search via Hierarchical Masking, ICCV 19 [[Paper]](https://openaccess.thecvf.com/content_ICCVW_2019/html/NeurArch/Yan_HM-NAS_Efficient_Neural_Architecture_Search_via_Hierarchical_Masking_ICCVW_2019_paper.html)
							
							
### Compilers for AIoT							
* Romou: rapidly generate high-performance tensor kernels for mobile GPUs,	MobiCom	22	[[Paper]]([https://dl.acm.org/doi/abs/10.1145/3495243.3517020](https://www.microsoft.com/en-us/research/uploads/prod/2022/02/mobigpu_mobicom22_camera.pdf))	
* The CoRa Tensor Compiler: Compilation for Ragged Tensors with Minimal Padding, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/d3d9446802a44259755d38e6d163e820-Paper.pdf)
* DIPS: Debug Intermittently-Powered Systems Like Any Embedded System, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568543)
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
* Compiling machine learning programs via high-level tracing,	MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/146.pdf)	
* TVM: An Automated End-to-End Optimizing Compiler for Deep Learning, OSDI	18	[[Paper]](https://www.usenix.org/conference/osdi18/presentation/chen)			
							
							
## Networking and Communication							

### Others
* Warm-started quantum sphere decoding via reverse annealing for massive IoT connectivity, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560516)
* FIRE: Enabling Reciprocity for FDD MIMO Systems, MobiCom 21 [[Paper]](https://deepakv.web.illinois.edu/assets/papers/FIRE_Mobicom2021.pdf) (General network-channel estimation using ML)
* DeepRadar: A Deep-Learning-based Environmental Sensing Capability Sensor Design for CBRS, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3448632) (Bandwidth/Rader estimate/detection using DL)
* Blind Distributed MU-MIMO for IoT Networking over VHF Narrowband Spectrum, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345427)

### Backscatter (Look at papers from Shyam @ University of Washington) 							
							
* Wind dispersal of battery-free wireless devices	,	Nature	2022	[[Paper]](https://www.nature.com/articles/s41586-021-04363-9)	(NO	ML)	
* Magnetoelectric backscatter communication for millimeter-sized wireless biomedical implants, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560541) (NO ML) (Best Paper Award)
* RF-Transformer: A Unified Backscatter Radio Hardware Abstraction, MobiCom 22 [[Paper]](https://arxiv.org/pdf/2209.15195.pdf)(NO ML)
* OmniScatter: extreme sensitivity mmWave backscattering using commodity FMCW radar,	MobiSys	22	[[Paper]](http://mason.gmu.edu/~ychae2/Omniscatter.pdf)	(NO	ML) (Best Paper)
* Content-agnostic backscatter from thin air		MobiSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538930)	(NO	ML)	
* Judo: addressing the energy asymmetry of wireless embedded systems through tunnel diode based wireless transmitters, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538923) (NO ML)
* Content-agnostic backscatter from thin air, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538930) (NO ML)
* Enabling software-defined PHY for backscatter networks, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538927) (NO ML)
* Low-Latency Visible Light Backscatter Networking with RetroMUMIMO	,	SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568507)	(NO	ML)	
Simplifying Backscatter Deployment: Full-Duplex LoRa Backscatter, NSDI 21 [[Paper]](https://www.usenix.org/system/files/nsdi21-katanbaf.pdf) (NO ML)
* Microphone array backscatter: an application-driven design for lightweight spatial sound recording over the air,		MobiCom	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3447993.3483265)	(NO ML)	
* MIXIQ: re-thinking ultra-low power receiver design for next-generation on-body applications, MobiCom 21 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/Mobicom21-MIXIQ.pdf) (NO ML)
* Verification: Can WiFi Backscatter replace RFID?, MobiCom 21 [[Paper]](https://cs.uwaterloo.ca/~brecht/papers/wifi-vs-rfid-mobicom-2021.pdf) (NO ML)
* Long-Range Ambient LoRa Backscatter with Parallel Decoding, MobiCom 21 [[Paper]](http://tns.thss.tsinghua.edu.cn/~jiliang/publications/MOBICOM21-p2lora.pdf) (NO ML)
* PCube: Scaling LoRa Concurrent Transmissions with Reception Diversities, MobiCom 21 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/PCube-MobiCom21.pdf) (NO ML)
* Combating link dynamics for reliable lora connection in urban settings, MobiCom 21 [[Paper]](https://dl.acm.org/doi/10.1145/3447993.3483250) (NO ML)
* PassiveLiFi: Rethinking LiFi for Low-Power and Long Range RF Backscatter, MobiCom 21 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/1541/Mobicom_PassiveLiFi_authors_version.pdf?sequence=1) (NO ML)
* Commodity-level BLE backscatter, MobiSys 21 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3466865) (NO ML)
* Enabling Passive Backscatter Tag Localization Without Active Receivers, SenSys 21 [[Paper]](http://www.wings.cs.stonybrook.edu/pdfs/2021-sensys.pdf) (NO ML)
* Internet-of-Microchips: Direct Radio-to-Bus Communication with SPI Backscatter, MobiCom 20 [[Paper]](https://wands.sg/publications/full_list/papers/MobiCom_20_2.pdf) (NO ML)
* Tunnel emitter: tunnel diode based low-power carrier emitters for backscatter tags, MobiCom 20 [[Paper]](https://lorenzocorneo.github.io/papers/2020-mobicom.pdf) (NO ML)
* Redefining passive in backscattering with commodity devices, MobiCom 20 [[Paper]](https://people.cs.umass.edu/~dganesan/papers/xShift-Mobicom2020.pdf)
* Towards scalable backscatter sensor mesh with decodable relay and distributed excitation	,	MobiSys	20	[[Paper]](https://www2.cs.sfu.ca/~jcliu/Papers/mobisys20-final157.pdf)	(NO	ML)	
* Two to Tango: Hybrid Light and Backscatter Networks for Next Billion Devices, MobiSys 20 [[Paper]](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/811/tosubmit.pdf?sequence=1)
* Rethinking ON-OFF Keying Modulation for Ambient LoRa Backscatter, SenSys 20 [[Paper]](http://tns.thss.tsinghua.edu.cn/sun/publications/aloba_2020.pdf) (NO ML)
* VMscatter: A Versatile MIMO Backscatter	,	NSDI	20	[[Paper]](https://www.usenix.org/system/files/nsdi20-paper-liu.pdf)	(NO	ML)	
* OFDMA-Enabled Wi-Fi Backscatter,MobiCom 19 [[Paper]](https://renjiezhao.github.io/files/OFDMA_BS_paper.pdf) (NO ML)
* TunnelScatter: Low Power Communication for Sensor Tags using Tunnel Diodes, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345451) (NO ML)


* Towards Battery-Free HD Video Streaming	,	NSDI	18	[[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/videobackscatter.pdf)	(NO	ML)	
* Charging a Smartphone Across a Room Using Lasers	,	UbiComp	18	[[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/laserpower.pdf)	(NO	ML)	
* LoRa Backscatter: Enabling The Vision of Ubiquitous Connectivity	,	UbiComp	17	[[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/loRaBackscatter.pdf)	(NO	ML)	
* Battery-Free Cellphone		UbiComp	17	[[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/phone.pdf) 	(NO ML)		
							
### LoRa							
* Saiyan: Design and Implementation of a Low-power Demodulator for LoRa Backscatter Systems	,	NSDI	22	[[Paper]](https://www.usenix.org/system/files/nsdi22-paper-guo.pdf)	(NO	ML)	
* De-spreading over the air: long-range CTC for diverse receivers with LoRa, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560524) (NO ML)
* BSMA: scalable LoRa networks using full duplex gateways, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560544) (NO ML)
* LLDPC: A Low-Density Parity-Check Coding Scheme for LoRa Networks, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568547) 
* HyLink: Towards High Throughput LPWANs with LoRa Compatible Communication, SenSys 22 [[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/HyLink-SenSys22.pdf)
* MaLoRaGW: Multi-User MIMO Transmission for LoRa, SenSys 22 [[Paperp]](https://www.cse.msu.edu/~hzeng/papers/Hossein22_Sensys_MaLoRaGW.pdf) (NO ML)
* Seirios: Leveraging Multiple Channels for LoRaWAN Indoor and Outdoor Localization, MobiCom 21 [[Paper]](https://arxiv.org/pdf/2108.06884.pdf) (NO ML)
* Embracing LoRa Sensing with Device Mobility	,	SenSys	22	[[Paper]](https://people.cs.umass.edu/~dganesan/papers/SenSys22-LoRaSensingMobility.pdf)	(NO	ML)	
* HyLink: Towards High Throughput LPWANs with LoRa Compatible Communication	,	SenSys	22	[[Paper]](https://www4.comp.polyu.edu.hk/~csyqzheng/papers/HyLink-SenSys22.pdf)	(NO	ML)	
* NELoRa: Towards Ultra-low SNR LoRa Communication with Neural-enhanced Demodulation	,	SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3485730.3485928)	
* Sense Me on the Ride: Accurate Mobile Sensing over a LoRa Backscatter Channel, SenSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3485730.3485933) (NO ML)		
* LAVA: fine-grained 3D indoor wireless coverage for small IoT devices	,	SIGCOMM	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3452296.3472890)	(NO	ML)	
* Exploring LoRa for Long-range Through-wall Sensing	,	IMWUT/UbiComp	20	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3397326)	(NO	ML)	
* LMAC: efficient carrier-sense multiple access for LoRa, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419200) (NO ML)
* WiChronos: energy-efficient modulation for long-range, large-scale wireless networks, MobiCom 20 [[Paper]](https://uwconnect.ece.wisc.edu/wp-content/uploads/sites/1525/2021/10/WiChronos.pdf) (NO ML)
* Combating interference for long range LoRa sensing, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430731) (NO ML)
* SLoRa: Towards Secure LoRa Communications with Fine-grained Physical Layer Features, SenSys 20 [[Paper]](https://soar.group/pubs/SLoRa.SenSys20.pdf)



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
* Enabling Secure Touch-to-Access Device Pairing based on Human Body’s Electrical Response, MobiCom 22 [[Paper]](https://taogu.site/pub/paper/Device_Pairing.pdf)
* Non-Cooperative Wi-Fi Localization & its Privacy Implications, MobiCom 22 [[Paper]](https://deepakv.web.illinois.edu/assets/papers/WiPeep_Mobicom2022.pdf) (NO ML)
* Audio-domain Position-independent Backdoor Attack via Unnoticeable Triggers, MobiCom 22 [[Paper]](https://www.winlab.rutgers.edu/~yychen/papers/Audio-domain%20Position-independent%20Backdoor%20Attack%20via%20Subsecond%20Triggers.pdf)
* Authentication for Drone Delivery Through a Novel Way of Using Face Biometrics, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560550)
* G2Auth: secure mutual authentication for drone delivery without special user-side hardware,	MobiSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3498361.3538941)	(NO	ML)	
* Vronicle: verifiable provenance for videos from mobile devices, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538943)
* TEO: ephemeral ownership for IoT devices to provide granular data control, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3539774)
* A Tale of Two Models Constructing Evasive Attacks on Edge Models, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/92cc227532d17e56e07902b254dfad10-Paper.pdf)
* Light Auditor: Power Measurement Can Tell Private Data Leakage through IoT Covert Channels,		SenSys	22	[[Paper]](https://www.cs.wm.edu/~wsjung/publications/papers/sensys22-p169-light-auditor.pdf)			
* HideSeeker: Uncover the Hidden Gems in Obfuscated Images,		SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568514)
* KITE: Exploring the Practical Threat from Acoustic Transduction Attacks on Inertial Sensors, SenSys 22 [[Paper]](https://lemingshen.github.io/assets/publication/conference/kite/paper.pdf)
* Push the Limit of Adversarial Example Attack on Speaker Recognition in Physical Domain, SenSys 22 [[Paper]](http://eceweb1.rutgers.edu/~daisylab/papers/Push%20the%20Limit%20of%20Adversarial%20Example%20Attack%20on%20Speaker%20Recognition%20in%20Physical%20Domain.pdf)
* Accuth: Anti-Spoofing Voice Authentication via Accelerometer, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568522)
* Face-Mic: Inferring Live Speech and Speaker Identity via Subtle Facial Dynamics Captured by AR/VR Motion Sensors, MobiCom 21 [[Paper]](https://www.winlab.rutgers.edu/~yychen/papers/FaceMic.pdf)
* Data-plane signaling in cellular IoT: attacks and defense, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483255) (NO ML)
* Insecurity of Operational Cellular IoT Service: New Vulnerabilities, Attacks, and Countermeasures, MobiCom 21 [[Paper]](https://www.cs.purdue.edu/homes/chunyi/pubs/mobicom21-wang.pdf) (NO ML)
* Notification Privacy Protection via Unobtrusive Gripping Hand Verification Using Media Sounds, MobiCom 21 [[Paper]](https://csc.lsu.edu/~chenwang/source_files/mobicom2021notificaiton.pdf)
* FastZIP: faster and more secure zero-interaction pairing	,	MobiSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3458864.3467883)	(NO	ML)	
* Encrypted cloud photo storage using Google photos, MobiSys 21 [[Paper]](https://www.cs.columbia.edu/~nieh/pubs/mobisys2021_esp.pdf) (NO ML)
* Rushmore: securely displaying static and animated images using TrustZone, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3467887) (NO ML)
* MegaMind: a platform for security & privacy extensions for voice assistants, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3467962)
* Sniffing Visible Light Communication Through Walls,	MobiCom	20	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419187)	(NO ML) ( Honourable Mention Award)	
* TouchPass: towards behavior-irrelevant on-touch user authentication on smartphones leveraging vibrations, MobiCom 20 [[Paper]](http://eceweb1.rutgers.edu/~daisylab/papers/TouchPass%20Towards%20Behavior-irrelevant%20on-touch%20User%20Authentication%20on%20Smartphones%20Leveraging%20Vibrations.pdf)
* SonicPrint: A Generally Adoptable and Secure Fingerprint Biometrics in Smart Devices, MobiSys 20 [[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-mobisys2020b.pdf)
* DarkneTZ: towards model privacy at the edge using trusted execution environments,		MobiSys	20	[[Paper]](https://arxiv.org/pdf/2004.05703.pdf)			
* SecWIR: securing smart home IoT communications via wi-fi routers with embedded intelligence, MobiSys 20 [[Paper]](https://www.cse.msu.edu/~ghtu/published-papers/Lei-Mobisys20.pdf)
* BlueDoor: Breaking the Secure Information Flow Via BLE Vulnerability, MobiSys 20 [[Paper]](http://tns.thss.tsinghua.edu.cn/~jiliang/publications/MOBISYS2020_BlueDoor.pdf) (NO ML)
* Privacy-Preserving Bandits, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/42a0e188f5033bc65bf8d78622277c4e-Paper.pdf)
* Alexa, Stop Spying on Me!: Speech Privacy Protection Against Voice Assistants, SenSys 20 [[Paper]](http://xyzhang.ucsd.edu/papers/KSun_SenSys20_MicShield.pdf)
* VocalPrint: Exploring A Resilient and Secure Voice Authentication via mmWave Biometric Interrogation, SenSys 20 [[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-sensys2020.pdf)
* Spying with Your Robot Vacuum Cleaner: Eavesdropping via LIDAR Sensors, SenSys 20 [[Paper]](https://www.cs.umd.edu/~nirupam/images/2_publication/papers/LidarPhone_SenSys20_nirupam.pdf)
* Occlumency: Privacy-preserving Remote Deep-learning Inference Using SGX, MobiCom 19 [[Paper]](https://soar.group/pubs/Occlumency.MobiCom19.pdf)
* Towards Touch-to-Access Device Authentication Using Induced Body Electric Potentials, MobiCom 19 [[Paper]](https://arxiv.org/pdf/1902.07057.pdf) (NO ML)
* Touch Well Before Use: Intuitive and Secure Authentication for IoT Devices, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345434)
* Taprint: Secure Text Input for Commodity Smart Wristbands, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300124)
* Canceling Inaudible Voice Commands Against Voice Control Systems, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345429)
* SpecEye: Towards Pervasive and Privacy-Preserving Screen Exposure Detection in Daily Life, MobiSys 19 [[Paper]](https://cse.buffalo.edu/~wenyaoxu/papers/conference/xu-mobisys2019a.pdf)
* Brain Password: A Secure and Truly Cancelable Brain Biometrics for Smart Headwear,		MobiSys	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210344)	(NO	ML)
							
### Federated Learning Systems			
* PyramidFL: a fine-grained client selection framework for efficient federated learning	,	MobiCom	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3495243.3517017)			
* FedBalancer: Data and Pace Control for Efficient Federated Learning on Heterogeneous Clients,	MobiSys	22	[[Paper]](https://arxiv.org/pdf/2201.01601.pdf)
* LightSecAgg: a Lightweight and Versatile Design for Secure Aggregation in Federated Learning, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/d2ddea18f00665ce8623e36bd4e3c7c5-Paper.pdf)
* Papaya: Practical, Private, and Scalable Federated Learning, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/f340f1b1f65b6df5b5e3f94d95b11daf-Paper.pdf)
* FedRolex: Model-Heterogeneous Federated Learning with Rolling Sub-Model Extraction,		NeurIPS	22	[[Paper]](https://openreview.net/forum?id=OtxyysUdBE)			
* FedSEA: A Semi-Asynchronous Federated Learning Framework for Extremely Heterogeneous Devices,		SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568538)	
* TailorFL: Dual-Personalized Federated Learning under System and Data Heterogeneity, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568503)		
* Hermes: an efficient federated learning framework for heterogeneous mobile clients, MobiCom 21 [[Paper]](https://sites.duke.edu/angli/files/2021/10/2021_Mobicom_Hermes_v1.pdf)			
* PPFL: privacy-preserving federated learning with trusted execution environments,		MobiSys	21	[[Paper]](https://arxiv.org/pdf/2104.14380.pdf) (Best Paper)		
* ClusterFL: a similarity-aware federated learning system for human activity recognition, MobiSys	21	[[Paper]](https://aiot.ie.cuhk.edu.hk/papers/ClusterFL.pdf)			
* Oort: Efficient Federated Learning via Guided Participant Selection,		OSDI	21	[[Paper]](https://www.usenix.org/system/files/osdi21-lai.pdf)			
* FedDL: Federated Learning via Dynamic Layer Sharing for Human Activity Recognition,		SenSys	21	[[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485946)			
* FedMask: Joint Computation and Communication-Efficient Personalized Federated Learning via Heterogeneous Masking,		SenSys	21	[[Paper]](https://dl.acm.org/doi/10.1145/3485730.3485929)			
* Billion-scale federated learning on mobile clients: a submodel design with tunable privacy, MobiCom 20	[[Paper]](https://www.cs.sjtu.edu.cn/~fwu/res/Paper/NWTHJLWC20MobiCom.pdf)	
* Federated Optimization in Heterogeneous Networks, MLSys 20 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2020/file/38af86134b65d0f10fe33d30dd76442e-Paper.pdf)
* Towards Federated Learning at Scale: System Design,		MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/193.pdf)		
* Federated Kernelized Multi-Task Learning,		MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/30.pdf)			
							
							
## AIoT Systems and their Applications	

### Others
Experience: Adopting Indoor Outdoor Detection in On-demand Food Delivery Business, MobiCom22 [[Paper]](https://wands.sg/publications/full_list/papers/MobiCom_22_1.pdf)

							
### AIoT Systems for Healthcare and Social Good							
* SmartLens : Sensing Eye Activities Using Zero-power Contact Lens,		MobiCom	22	[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3560532)	(NO	ML)	
* Network-side digital contact tracing on a large university campus, MobiCom 22 [[Paper]](https://arxiv.org/pdf/2201.10641.pdf) (NO ML)
* PROS: an Efficient Pattern-Driven Compressive Sensing Framework for Low-Power Biopotential-based Wearables with On-chip Intelligence, MobiCom 22 [[Paper]](https://theyoungkwon.github.io/papers/articles/pham_pros_mobicom22.pdf)
* EarHealth: an earphone-based acoustic otoscope for detection of multiple ear diseases in daily life, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538935)
* Out-Clinic Pulmonary Disease Evaluation via Acoustic Sensing and Multi-Task Learning on Commodity Smartphones	, SenSys	22	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568437)
* NFCapsule: An Ingestible Sensor Pill for Eosinophilic Esophagitis Detection Based on Near-field Coupling, SenSys 22 [[Paper]](https://swarunkumar.com/papers/nfcapsule-sensys2022.pdf) (NO ML)
* Hearing Heartbeat from Voice: Towards Next Generation Voice-User Interfaces with Cardiac Sensing Function, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568508)	
* mmBP: Contact-free Millimetre-wave Radar based Approach to Blood Pressure Measurement, SenSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3560905.3568506)
* Your Smart Speaker Can “Hear” Your Heartbeat!, IMWUT/UbiComp	21	[[Paper]](https://dl.acm.org/doi/10.1145/3432237)	(NO	ML)	
* MoVi-Fi: Motion-robust Vital Signs Waveform Recovery via Deep Interpreted RF Sensing, MobiCom 21 [[Paper]](https://rabbitnick.github.io/pubs/movifi.pdf)
* Crisp-BP: Continuous Wrist PPG-based Blood Pressure Measurement, MobiCom 21 [[Paper]](https://cis.temple.edu/~yu/research/CrispBP-Mobicom21.pdf)
* Healthy diapering with passive RFIDs for diaper wetness sensing and urine pH identification, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3466870)
* Hivemind: social control-and-use of IoT towards democratization of public spaces, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3466626) (NO ML)
* U-Verse: a miniaturized platform for end-to-end closed-loop implantable internet of medical things systems		SenSys	21	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360026)	(NO	ML)	
* PDLens: smartphone knows drug effectiveness among Parkinson's via daily-life activity fusion,	MobiCom	20	[[Paper]](https://www.acsu.buffalo.edu/~huiningl/papers/pdlens.pdf)		
* MET: a magneto-inductive sensing based electric toothbrushing monitoring system, MobiCom 20 [[Paper]](https://www.ece.sunysb.edu/~slin/Publications/MOBICOM2020.pdf)
* Self-Reconfgurable Micro-Implants for Cross-Tissue Wireless and Batteryless Connectivity,	MobiCom	20	[[Paper]]([https://dl.acm.org/doi/abs/10.1145/3372224.3419216](https://dl.acm.org/doi/pdf/10.1145/3372224.3419216))	(NO	ML)	
* Towards flexible wireless charging for medical implants using distributed antenna system, MobiCom 20 [[Paper]](https://arxiv.org/pdf/2001.07644.pdf) (NO ML)
* SpiroSonic: monitoring human lung function via acoustic sensing on commodity smartphones, MobiCom 20 [[Paper]](https://sites.pitt.edu/~weigao/publications/mobicom20.pdf)
* Contactless seismocardiography via deep learning radars, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419982)
* Painometry: Wearable and Objective !antification System for Acute Postoperative Pain, MobiSys 20 [[Paper]](http://mnslab.org/tamvu/paper/2020%20Painometry_Hoang.pdf)
* RFWash: A Weakly Supervised Tracking of Hand Hygiene Technique, SenSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3384419.3430733)
* Contactless Infant Monitoring using White Noise,		MobiCom	19	[[Paper]](https://homes.cs.washington.edu/~gshyam/Papers/whitenoise.pdf)	(NO	ML)	
* Experience: Design, Development and Evaluation of a Wearable Device for mHealth Applications, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345432) (NO ML)
* HealthSense: Software-defined Mobile-based Clinical Trials, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345433) (Best Paper)
* PDVocal: Towards Privacy-preserving Parkinson's Disease Detection using Non-speech Body Sounds, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300125)
* SignSpeaker: A Real-time, High-Precision SmartWatch-based Sign Language Translator, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300117)
* CardioCam: Leveraging Camera on Mobile Devices to Verify Users While Their Heart is Pumping, MobiSys 19 [[Paper]](https://www.winlab.rutgers.edu/~gruteser/papers/CardioCam.pdf)

* When Virtual Reality Meets Internet of Things in the Gym: Enabling Immersive Interactive Machine Exercises, ubiComp 18 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3214281)	
* MobileDeepPill: A Small-Footprint Mobile Deep Learning System for Recognizing Unconstrained Pill Images,		MobiSys	17	[[Paper]](https://dl.acm.org/doi/10.1145/3081333.3081336)			
* DeepASL: Enabling Ubiquitous and Non-Intrusive Word and Sentence-Level Sign Language Translation,		SenSys	17	[[Paper]](https://dl.acm.org/doi/10.1145/3131672.3131693)

			
### AIoT Systems for Autonomous Driving					
* VIPS: Real-Time Perception Fusion for Infrastructure-Assisted Autonomous Driving, MobiCom 22 [[Paper]](https://yanzhenyu.com/assets/pdf/VIPS-MobiCom22.pdf) (Best Paper Award Runner-ups)
* Motion inspires notion: self-supervised visual-LiDAR fusion for environment depth estimation, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538918)
* Mosaic: leveraging diverse reflector geometries for omnidirectional around-corner automotive radar, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538944) (NO ML)
* AutoCast: scalable infrastructure-less cooperative perception for distributed collaborative driving, MobiSys 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3498361.3538925)
* AutoMatch: Leveraging Traffic Camera to Improve Perception and Localization of Autonomous Vehicles,		SenSys	22	[[Paper]](https://yanzhenyu.com/assets/pdf/AutoMatch-SenSys22.pdf)
* EMP: Edge-assisted Multi-vehicle Perception, MobiCom 21 [[Paper]](https://xiaoshawnzhu.github.io/emp-mobicom21.pdf)
* Towards Backdoor Attacks against LiDAR Object Detection in Autonomous Driving, SenSys 22 [[Paper]](https://www.acsu.buffalo.edu/~yzhu39/Yi_Zhu_homepage_files/papers/SenSys22.pdf)
* RayTrack: enabling interference-free outdoor mobile VLC with dynamic field-of-view, MobiSys 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3458864.3466867) (NO ML)
* Demystifying Millimeter-Wave V2X: Towards Robust and Efficient Directional Connectivity Under High Mobility, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419208)
* Renovating road signs for infrastructure-to-vehicle networking: a visible light backscatter communication and networking approach, MobiCom 20 [[Paper]](https://soar.group/pubs/RetroI2V.MobiCom20.pdf) (NO ML)
* Wi-Go: Accurate and Scalable Vehicle Positioning using WiFi Fine Timing Measurement, MobiSys 20 [[Paper]](https://www.andrew.cmu.edu/user/miahmed/papers/wi-go_mobisys.pdf) (NO ML)
* VeMo: Enabling Transparent Vehicular Mobility Modeling at Individual Levels with Full Penetration, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300130)
* Experience: Understanding Long-Term Evolving Patterns of Shared Electric Vehicle Networks, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300132) (NO ML)
* Diagnosing Vehicles with Automotive Batteries, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300126)	






### AIoT Systems for Video Analytics 							
* NeuriCam: Key-Frame Video Super-Resolution and Colorization for IoT Cameras,		MobiCom	23	[[Paper]](https://arxiv.org/abs/2207.12496)[[Code]](https://github.com/vb000/NeuriCam)	
* Multiview Transformers for Video Recognition, CVPR 22 [[Paper]](https://openaccess.thecvf.com/content/CVPR2022/html/Yan_Multiview_Transformers_for_Video_Recognition_CVPR_2022_paper.html)		
* AccMPEG: Optimizing Video Encoding for Video Analytics, MLSys 22 [[Paper]](https://proceedings.mlsys.org/paper_files/paper/2022/file/98f13708210194c475687be6106a3b84-Paper.pdf)
* SalientVR: Saliency-Driven Mobile 360-Degree Video Streaming with Gaze Information, MobiCom 22 [[Papaer]](https://www-users.cse.umn.edu/~fengqian/paper/salientvr_mobicom22.pdf)
* Vues: Practical Mobile Volumetric Video Streaming Through Multiview Transcoding, MobiCom22 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/vues_mobicom22.pdf)
* Tutti: coupling 5G RAN and mobile edge computing for latency-critical video analytics, MobiCom 22 [[Paper]](https://dl.acm.org/doi/10.1145/3495243.3560538)
* Breaking edge shackles: Infrastructure-free collaborative mobile augmented reality, SenSys 22 [[Paper]](https://www.cs.ucr.edu/~jiasi/pub/freeAR-sensys22.pdf)
* Turbo: Opportunistic Enhancement for Edge Video Analytics, SenSys 22 [[Paper]](https://arxiv.org/pdf/2207.00172.pdf)	
* Enhancing Video Analytics Accuracy via Real-time Automated Camera Parameter Tuning, SenSys 22 [[Paper]](https://arxiv.org/pdf/2107.03964.pdf)
* Loki: Improving Long Tail Performance of Learning-Based Real-Time Video Adaptation by Fusing Rule-Based Models, MobiCom 21 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3447993.3483259)
* FollowUpAR: enabling follow-up effects in mobile AR applications,		MobiSys	21	[[Paper]](http://tns.thss.tsinghua.edu.cn/~jingao/papers/mobisys21_followupar.pdf)	
* GROOT: a real-time streaming system of high-fidelity volumetric videos, MobiCom 20 [[Paper]](https://juheonyi.github.io/files/GROOT.pdf) (NO ML)
* OnRL: improving mobile video telephony via online reinforcement learning, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419186)
* NEMO: enabling neural-enhanced video streaming on commodity mobile devices, MobiCom 20 [[Paper]](https://hyunhoyeo.com/assets/pdf/3372224.3419185.pdf)
* ViVo: visibility-aware mobile volumetric video streaming, MobiCom 20 [[Paper]](https://www-users.cse.umn.edu/~fengqian/paper/vivo_mobicom20.pdf)
* C-14: Assured Timestamps for Drone Videos, MobiCom 20 [[Paper]](https://people.cs.umass.edu/~elm/papers/mobicom20-final809.pdf)
* EMO: real-time emotion recognition from single-eye images for resource-constrained eyewear devices,	MobiSys	20	[[Paper]](https://dongshuhao.github.io/assets/pdf/2020/Wu_2020.pdf)		
* Distream: Scaling Live Video Analytics with Workload-Adaptive Distributed Edge Intelligence,		SenSys	20	[[Paper]](https://www.egr.msu.edu/~mizhang/papers/2020_SenSys_Distream.pdf)	
* TSM: Temporal Shift Module for Efficient Video Understanding,		ICCV	19	[[Paper]](https://openaccess.thecvf.com/content_ICCV_2019/html/Lin_TSM_Temporal_Shift_Module_for_Efficient_Video_Understanding_ICCV_2019_paper.html)			
* Scaling Video Analytics on Constrained Edge Nodes,		MLSys	19	[[Paper]](https://mlsys.org/Conferences/2019/doc/2019/197.pdf)		
* Edge Assisted Real-time Object Detection for Mobile Augmented Reality, MobiCom 19 [[Paper]](https://dl.acm.org/doi/10.1145/3300061.3300116)
* Jigsaw: Robust Live 4K Video Streaming, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3300127) (NO ML)
* Learning to Coordinate Video Codec with Transport Protocol for Mobile Video Telephony, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345430)
* When IoT met Augmented Reality: Visualizing the Source of the Wireless Signal in AR View,		MobiSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3307334.3326079)			
* SmrtFridge: IoT-based,  user interaction-driven food item & quantity sensing,		SenSys	19	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3356250.3360028)			
* Potluck: Cross-Application Approximate Deduplication for Computation-Intensive Mobile Applications,		ASPLOS	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3173162.3173185)			
* EVA: An Efficient System for Exploratory Video Analysis,		MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/22.pdf)			
* Efficient Multi-Tenant Inference on Video using Microclassifiers,		MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/133.pdf)			
* Dynamic Stem-Sharing for Multi-Tenant Video Processing,		MLSys	18	[[Paper]](https://mlsys.org/Conferences/doc/2018/149.pdf)			
* Rubiks: Practical 360-Degree Streaming for Smartphones,		MobiSys	18	[[Paper]](https://dl.acm.org/doi/abs/10.1145/3210240.3210323)	(NO	ML)	


### AIoT Systems for Agriculture 

* IoTree: a battery-free wearable system with biocompatible sensors for continuous tree health monitoring, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3567652) (NO ML)
* Estimating Soil Moisture using RF Signals, MobiCom 22 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3495243.3517025) (NO ML) 
* LTE-Based Low-Cost and Low-Power Soil Moisture Sensing, SenSys 22 [[Paper]](https://dl.acm.org/doi/abs/10.1145/3560905.3568525) (NO ML)
* Airdropping sensor networks from drones and insects, MobiCom 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3372224.3419981) (NO ML)
* Soil Moisture Sensing with Commodity RFID Systems, MobiSys 20 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3386901.3388940)
* Towards Low Cost Soil Sensing Using Wi-Fi, MobiCom 19 [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3300061.3345440) (NO ML) (Honorable Mention)
* Living IoT: A Flying Wireless Platform on Live Insects, MobiCom 19 [[Paper]](https://livingiot.cs.washington.edu/files/livingiot.pdf)






