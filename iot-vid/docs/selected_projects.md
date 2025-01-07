# Selected Projects

### MAVFI: An End-to-End Fault Analysis Framework with Anomaly Detection and Recovery for Micro Aerial Vehicles

Yu-Shun Hsiao, Zishen Wan, Tianyu Jia, Radhika Ghosal, Abdulrahman Mahmoud, Arijit Raychowdhury, David Brooks, Gu-Yeon Wei, Vijay Janapa Reddi. **Accepted at DATE'23.**

[Paper](https://vlsiarch.eecs.harvard.edu/sites/hwpi.harvard.edu/files/vlsiarch/files/2105.12882.pdf?m=1651695066) | [Code](https://github.com/harvard-edge/MAVBench/tree/mavfi)

> Abstract: Reliability and safety are critical in autonomous machine services, such as autonomous vehicles and aerial drones. In this paper, we first present an open-source Micro Aerial Vehicles (MAVs) reliability analysis framework, MAVFI, to characterize transient fault’s impacts on the end-to-end flight metrics, e.g., flight time, success rate. Based on our framework, it is observed that the end-to-end fault tolerance analysis is essential for characterizing system reliability. We demonstrate the planning and control stages are more vulnerable to transient faults than the visual perception stage in the common “Perception-Planning-Control (PPC)” compute pipeline. Furthermore, to improve the reliability of the MAV system, we propose two low overhead anomaly-based transient fault detection and recovery schemes based on Gaussian statistical models and autoencoder neural networks. We validate our anomaly fault protection schemes with a variety of simulated photo-realistic environments on both Intel i9 CPU and ARM Cortex-A57 on Nvidia TX2 platform. It is demonstrated that the autoencoder-based scheme can improve the system reliability by 100% recovering failure cases with less than 0.0062% computational overhead in best-case scenarios. In addition, MAVFI framework can be used for other ROS-based cyber-physical applications and is open-sourced at [this link](https://github.com/harvard-edge/MAVBench/tree/mavfi).

### OMU: A Probabilistic 3D Occupancy Mapping Accelerator for Real-time OctoMap at the Edge

Tianyu Jia, En-Yu Yang, Yu-Shun Hsiao, Jonathan Cruz, David Brooks, Gu-Yeon Wei, Vijay Janapa Reddi. **Accepted at DATE'22.**

[Paper](https://past.date-conference.com/proceedings-archive/2022/pdf/0127.pdf)

> Abstract: Autonomous machines (e.g., vehicles, mobile robots, drones) require sophisticated 3D mapping to perceive the dynamic environment. However, maintaining a real-time 3D map is expensive both in terms of compute and memory requirements, especially for resource-constrained edge machines. Probabilistic OctoMap is a reliable and memory-efficient 3D dense map model to represent the full environment, with dynamic voxel node pruning and expansion capacity. This paper presents the first efficient accelerator solution, i.e. OMU, to enable real-time probabilistic 3D mapping at the edge. To improve the performance, the input map voxels are updated via parallel PE units for data parallelism. Within each PE, the voxels are stored using a specially developed data structure in parallel memory banks. In addition, a pruning address manager is designed within each PE unit to reuse the pruned memory addresses. The proposed 3D mapping accelerator is implemented and evaluated using a commercial 12 nm technology. Compared to the ARM Cortex-A57 CPU in the Nvidia Jetson TX2 platform, the proposed accelerator achieves up to 62× performance and 708× energy efficiency improvement. Furthermore, the accelerator provides 63 FPS throughput, more than 2× higher than a real-time requirement, enabling real-time perception for 3D mapping.

### OctoCache: Caching Voxels for Accelerating 3D Occupancy Mapping in Autonomous Systems

Peiqing Chen, Minghao Li, Zishen Wan, Yu-Shun Hsiao, Minlan Yu, Vijay Janapa Reddi, Alan Zaoxing Liu. **In submission.**

> Abstract: coming soon.

### HawkVision: Low-Latency Modeless Edge AI Serving

ChonLam Lao, Jiaqi Gao, Ganesh Ananthanarayanan, Aditya Akella, Minlan Yu. **In submission.**

[Paper](https://arxiv.org/abs/2405.19213)

> Abstract: The trend of modeless ML inference is increasingly growing in popularity as it hides the complexity of model inference from users and caters to diverse user and application accuracy requirements. Previous work mostly focuses on modeless inference in data centers. To provide low-latency inference, in this paper, we promote modeless inference at the edge. The edge environment introduces additional challenges related to low power consumption, limited device memory, and volatile network environments.
> 
> To address these challenges, we propose HawkVision, which provides low-latency modeless serving of vision DNNs. HawkVision leverages a two-layer edge-DC architecture that employs confidence scaling to reduce the number of model options while meeting diverse accuracy requirements. It also supports lossy inference under volatile network environments. Our experimental results show that HawkVision outperforms current serving systems by up to 1.6× in P99 latency for providing modeless service. Our FPGA prototype demonstrates similar performance at certain accuracy levels with up to a 3.34× reduction in power consumption.


### Other Publications

[A Throughput-Centric View of the Performance of Datacenter Topologies](https://minlanyu.seas.harvard.edu/writeup/sigcomm21-throughput.pdf). Pooria Namyar, Sucha Supittayapornpong, Mingyang Zhang, Minlan Yu, Ramesh Govindan. **Accepted at SIGCOMM'21.**

[Jaqen: A High-Performance Switch-Native Approach for Detecting and Mitigating Volumetric DDoS Attacks with Programmable Switches](https://www.usenix.org/system/files/sec21-liu-zaoxing.pdf). Zaoxing Liu, Hun Namkung, Georgios Nikolaidis, Jeongkeun Lee, Changhoon Kim, Xin Jin, Vladimir Braverman, Minlan Yu, Vyas Sekar. **Accepted at USENIX Security'21.**

[Carbink: Fault-tolerant far memory](https://www.usenix.org/system/files/osdi22-zhou-yang.pdf). Yang Zhou, Hassan Wassel, Sihang Liu, Jiaqi Gao, James Mickens, Minlan Yu, Chris Kennelly, Paul Turner, David Culler, Hank Levy, Amin Vahdat. **Accepted at OSDI'22.**

[Optimal Oblivious Routing for Structured Networks](https://minlanyu.seas.harvard.edu/writeup/infocom22.pdf). Sucha Supittayapornpong, Pooria Namyar, Mingyang Zhang, Minlan Yu, Ramesh Govindan. **Accepted at INFOCOM'22.**

[Silent Data Corruption in Robot Operating System: A Case for End-to-End System-Level Fault Analysis Using Autonomous UAVs](https://ieeexplore.ieee.org/document/10315202). Yu-Shun Hsiao, Zishen Wan, Tianyu Jia, Radhika Ghosal, Abdulrahman Mahmoud, Arijit Raychowdhury, David Brooks, Gu-Yeon Wei, Vijay Janapa Reddi. **Accepted at IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems.**

[Scalable Distributed Massive MIMO Baseband Processing](https://www.usenix.org/system/files/nsdi23-gong.pdf). Junzhi Gong, Anuj Kalia, Minlan Yu. **Accepted at NSDI'23.**

[Rearchitecting the TCP Stack for I/O-Offloaded Content Delivery](). Taehyun Kim, Deondre Martin Ng, Junzhi Gong, Youngjin Kwon, Minlan Yu, KyoungSoo Park. **Accepted at NSDI'23.**

[Boosting Existing DDoS Detection Systems Using Auxiliary Signals](). Zhiying Xu, Sivaramakrishnan Ramanathan, Alexander Rush, Jelena Mirkovic, Minlan Yu. **Accepted at CoNEXT'22.**
