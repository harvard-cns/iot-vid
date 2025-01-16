# Selected Projects

### OctoCache: Caching Voxels for Accelerating 3D Occupancy Mapping in Autonomous Systems

Peiqing Chen, Minghao Li, Zishen Wan, Yu-Shun Hsiao, Minlan Yu, Vijay Janapa Reddi, Alan Zaoxing Liu.<br />
**In submission.**

> Abstract: Three-dimensional (3D) mapping systems are essential for generating digital representations of physical environments. They are widely used in applications involving autonomous robot navigation, 3D visualization, and augmented/virtual reality (AR/VR). In this paper, we focus on OctoMap, a prominent 3D mapping framework that utilizes an octree-based data structure with voxel occupancy values to achieve spatial efficiency and explicit dense map representation. Our analysis indicates that OctoMap's performance is constrained by slow mapping system updates, primarily attributed to costly memory accesses within its octree data storage. To address this issue, we introduce OctoCache, a software system designed to accelerate OctoMap's performance. OctoCache dramatically improves the mapping system's update speed through three primary mechanisms: (1) optimization of cache memory access, (2) refinement of voxel ordering, and (3) workflow parallelization. OctoCache in 3D environment construction tasks demonstrates significant performance improvement, with speedups ranging from 45.63%~88.01% compared to the standard OctoMap implementation. Furthermore, we validate the OctoCache by deploying it in multiple Unmanned Aerial Vehicle (UAV) autonomous navigation scenarios to quantify the end-to-end benefits. Our results indicate up to 3.02× speedup and a reduction in mission completion time of up to 28% across four environments. These findings substantiate OctoCache's capacity to markedly enhance the efficiency of 3D mapping systems in critical autonomous navigation applications, potentially facilitating advancements in robotics and environmental modeling.

### OMU: A Probabilistic 3D Occupancy Mapping Accelerator for Real-time OctoMap at the Edge

Tianyu Jia, En-Yu Yang, Yu-Shun Hsiao, Jonathan Cruz, David Brooks, Gu-Yeon Wei, Vijay Janapa Reddi.<br />
**At DATE'22.**

[Paper](https://past.date-conference.com/proceedings-archive/2022/pdf/0127.pdf)

> Abstract: Autonomous machines (e.g., vehicles, mobile robots, drones) require sophisticated 3D mapping to perceive the dynamic environment. However, maintaining a real-time 3D map is expensive both in terms of compute and memory requirements, especially for resource-constrained edge machines. Probabilistic OctoMap is a reliable and memory-efficient 3D dense map model to represent the full environment, with dynamic voxel node pruning and expansion capacity. This paper presents the first efficient accelerator solution, i.e. OMU, to enable real-time probabilistic 3D mapping at the edge. To improve the performance, the input map voxels are updated via parallel PE units for data parallelism. Within each PE, the voxels are stored using a specially developed data structure in parallel memory banks. In addition, a pruning address manager is designed within each PE unit to reuse the pruned memory addresses. The proposed 3D mapping accelerator is implemented and evaluated using a commercial 12 nm technology. Compared to the ARM Cortex-A57 CPU in the Nvidia Jetson TX2 platform, the proposed accelerator achieves up to 62× performance and 708× energy efficiency improvement. Furthermore, the accelerator provides 63 FPS throughput, more than 2× higher than a real-time requirement, enabling real-time perception for 3D mapping.

### EdgeSight: Enabling Modeless and Cost-Efficient Inference at the Edge

ChonLam Lao, Jiaqi Gao, Ganesh Ananthanarayanan, Aditya Akella, Minlan Yu.<br />
**In submission.**

[Paper](https://arxiv.org/abs/2405.19213)

> Abstract: Traditional ML inference is evolving toward modeless inference, which abstracts the complexity of model selection from users, allowing the system to automatically choose the most appropriate model for each request based on accuracy and resource requirements. While prior studies have focused on modeless inference within data centers, this paper tackles the pressing need for cost-efficient modeless inference at the edge -- particularly within its unique constraints of limited device memory, volatile network conditions, and restricted power consumption.
> 
> To overcome these challenges, we propose EdgeSight, a system that provides cost-efficient modeless serving for diverse DNNs at the edge. EdgeSight employs an edge-data center (edge-DC) architecture, utilizing confidence scaling to reduce the number of model options while meeting diverse accuracy requirements. Additionally, it supports lossy inference in volatile network environments. Our experimental results show that EdgeSight outperforms existing systems by up to 1.6x in P99 latency for modeless services. Furthermore, our FPGA prototype demonstrates similar performance at certain accuracy levels, with a power consumption reduction of up to 3.34x.

### MAVFI: An End-to-End Fault Analysis Framework with Anomaly Detection and Recovery for Micro Aerial Vehicles

Yu-Shun Hsiao, Zishen Wan, Tianyu Jia, Radhika Ghosal, Abdulrahman Mahmoud, Arijit Raychowdhury, David Brooks, Gu-Yeon Wei, Vijay Janapa Reddi.<br />
**At DATE'23.**

[Paper](https://vlsiarch.eecs.harvard.edu/sites/hwpi.harvard.edu/files/vlsiarch/files/2105.12882.pdf?m=1651695066) | [Code](https://github.com/harvard-edge/MAVBench/tree/mavfi)

> Abstract: Reliability and safety are critical in autonomous machine services, such as autonomous vehicles and aerial drones. In this paper, we first present an open-source Micro Aerial Vehicles (MAVs) reliability analysis framework, MAVFI, to characterize transient fault’s impacts on the end-to-end flight metrics, e.g., flight time, success rate. Based on our framework, it is observed that the end-to-end fault tolerance analysis is essential for characterizing system reliability. We demonstrate the planning and control stages are more vulnerable to transient faults than the visual perception stage in the common “Perception-Planning-Control (PPC)” compute pipeline. Furthermore, to improve the reliability of the MAV system, we propose two low overhead anomaly-based transient fault detection and recovery schemes based on Gaussian statistical models and autoencoder neural networks. We validate our anomaly fault protection schemes with a variety of simulated photo-realistic environments on both Intel i9 CPU and ARM Cortex-A57 on Nvidia TX2 platform. It is demonstrated that the autoencoder-based scheme can improve the system reliability by 100% recovering failure cases with less than 0.0062% computational overhead in best-case scenarios. In addition, MAVFI framework can be used for other ROS-based cyber-physical applications and is open-sourced at [this link](https://github.com/harvard-edge/MAVBench/tree/mavfi).


### Other Publications

[A Throughput-Centric View of the Performance of Datacenter Topologies](https://minlanyu.seas.harvard.edu/writeup/sigcomm21-throughput.pdf)<br />
 Pooria Namyar, Sucha Supittayapornpong, Mingyang Zhang, Minlan Yu, Ramesh Govindan.<br />
**At SIGCOMM'21.**

[Jaqen: A High-Performance Switch-Native Approach for Detecting and Mitigating Volumetric DDoS Attacks with Programmable Switches](https://www.usenix.org/system/files/sec21-liu-zaoxing.pdf)<br />
Zaoxing Liu, Hun Namkung, Georgios Nikolaidis, Jeongkeun Lee, Changhoon Kim, Xin Jin, Vladimir Braverman, Minlan Yu, Vyas Sekar.<br />
**At USENIX Security'21.**

[Carbink: Fault-tolerant far memory](https://www.usenix.org/system/files/osdi22-zhou-yang.pdf)<br />
Yang Zhou, Hassan Wassel, Sihang Liu, Jiaqi Gao, James Mickens, Minlan Yu, Chris Kennelly, Paul Turner, David Culler, Hank Levy, Amin Vahdat.<br />
**At OSDI'22.**

[Optimal Oblivious Routing for Structured Networks](https://minlanyu.seas.harvard.edu/writeup/infocom22.pdf)<br />
Sucha Supittayapornpong, Pooria Namyar, Mingyang Zhang, Minlan Yu, Ramesh Govindan.<br />
**At INFOCOM'22.**

[Silent Data Corruption in Robot Operating System: A Case for End-to-End System-Level Fault Analysis Using Autonomous UAVs](https://ieeexplore.ieee.org/document/10315202)<br />
Yu-Shun Hsiao, Zishen Wan, Tianyu Jia, Radhika Ghosal, Abdulrahman Mahmoud, Arijit Raychowdhury, David Brooks, Gu-Yeon Wei, Vijay Janapa Reddi.<br />
**At IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems.**

[Scalable Distributed Massive MIMO Baseband Processing](https://www.usenix.org/system/files/nsdi23-gong.pdf).<br />
Junzhi Gong, Anuj Kalia, Minlan Yu.<br />
**At NSDI'23.**

[Rearchitecting the TCP Stack for I/O-Offloaded Content Delivery](https://www.usenix.org/system/files/nsdi23-kim-taehyun.pdf)<br />
Taehyun Kim, Deondre Martin Ng, Junzhi Gong, Youngjin Kwon, Minlan Yu, KyoungSoo Park.<br />
**At NSDI'23.**

[Boosting Existing DDoS Detection Systems Using Auxiliary Signals](https://minlanyu.seas.harvard.edu/writeup/conext22.pdf)<br />
Zhiying Xu, Sivaramakrishnan Ramanathan, Alexander Rush, Jelena Mirkovic, Minlan Yu.<br />
**At CoNEXT'22.**
