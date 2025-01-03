# Projects

### OMU: A Probabilistic 3D Occupancy Mapping Accelerator for Real-time OctoMap at the Edge

Tianyu Jia, En-Yu Yang, Yu-Shun Hsiao, Jonathan Cruz, David Brooks, Gu-Yeon Wei, Vijay Janapa Reddi. **Accepted at DATE'22.**

[Paper](https://dl.acm.org/doi/abs/10.5555/3539845.3540058)

The OMU accelerator system transformed how flying devices like drones process their surroundings by introducing parallel processing units and efficient memory management. This system achieved faster processing, using two orders of magnitude less energy than standard processors, making autonomous navigation more practical and efficient. The research extended to safety considerations through the MAVFI framework, which addressed the critical challenge of system reliability. MAVFI enabled drones to detect and recover from silent system failures with minimal computational overhead, representing a significant advancement in autonomous system safety.

### OctoCache: Caching Voxels for Accelerating 3D Occupancy Mapping in Autonomous Systems

Peiqing Chen, Minghao Li, Zishen Wan, Yu-Shun Hsiao, Minlan Yu, Vijay Janapa Reddi, Alan Zaoxing Liu. **In submission.**

OctoMap is an accelerator for processing point cloud data for autonomous machines intelligently and effectively. We introduced OctoCache, a software system that dramatically improves the mapping system’s update speed. OctoCache in 3D environment construction tasks demonstrates significant performance improvement. Furthermore, we validate the OctoCache by deploying it in multiple Unmanned Aerial Vehicle (UAV) autonomous navigation scenarios to quantify the end-to-end benefits.

### HawkVision: Low-Latency Modeless Edge AI Serving

ChonLam Lao, Jiaqi Gao, Ganesh Ananthanarayanan, Aditya Akella, Minlan Yu. **In submission.**

[Paper](https://arxiv.org/abs/2405.19213)

We proposed HawkVision, which provides low-latency modeless serving of vision DNNs. HawkVision leverages a two-layer edge-cloud architecture that employs confidence scaling to reduce the number of model options while meeting diverse accuracy requirements. It also supports lossy inference under volatile network environments.