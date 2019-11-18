Ultra-Dense Networks Problem Research
---

### Resource allocation for ultra-dense networks: A survey, some research issues and challenges. IEEE Communications Surveys & Tutorials (2018).[[1]](https://ieeexplore.ieee.org/document/8447187)

#### Open Research Directions
> A. High Computational Complexity
> "In UDNs, the Resource Allocation(RA) issues are always interpreted as highly complex large-scale optimization problems,"

The Optimization Problems is the work when the Base Stations is initialized. After that, the RA issues should be interpreted as the prediction problems of the best RA decision. The user's movement can be modeled as Brownian motion. There are many algorithms that can perform research in this area.(LQR, kalman filter.etc.)


>"Even though several approaches mentioned in this survey, like **MFG, stochastic geometry, stochastic optimization, grouping/clustering based methods**, etc. have provided some insights, effective algorithms of low complexity still need further exploration for the efficient resource utilization in UDNs."

Considering the high attenuation of millimeter-wave communication (LOS and N-LOS transmission models), we can set a threshold to simplify the transfer model using Distance weight or Principal Component Analysis(PCA). Corresponding to the MFG, stochastic geometry, stochastic optimization methods

The RA process can be decomposed into several sub-problems or conducted distributedly, thus significantly reducing the computational complexity[[2]](https://ieeexplore.ieee.org/abstract/document/8007415). Corresponding to the grouping/clustering based methods

---
>B. Significant Overhead and Feedback
>"The optimal resource distribution relies on the network-wide state information of a quite large number of APs or users, which is not easy to acquire the perfect CSI, QSI, CaSI etc., especially in large-scale networks like UDNs. This would bring about heavy signaling overhead as well as significant feedback."

Whether this problem can be turned into a Recommendation System. The Matrix Completion algorithm is used to recommend user requirements and reduce signaling overhead.


>D. Mobility Management
>"In dense scenarios, the challenges of mobility management are mainly induced by the large amount of different terminal types and a broad range of services and mobility demands ranging from zero or nomadic mobility to high speed terminals."

Mobile-Edge Computation Offloading：I haven’t studied this problem yet.

---
The Optimal Number of BS per unit area in UND Environment

>Optimal number of BS = min(f(wavelength，Sight rate) + QSI + Utility)

Function f is BS service range. Sight Rate is LoS/NLoS.
QSI characterization of Quality of services（QoS）.
utility is energy efficiency.



### Reference
[1]  Teng, Yinglei, et al. "Resource allocation for ultra-dense networks: A survey, some research issues and challenges." IEEE Communications Surveys & Tutorials (2018).  
[2] L. Dai, B. Bai, "Optimal decomposition for large-scale infrastructure-based wireless networks", IEEE Trans. Wireless Commun., vol. 16, no. 8, pp. 4956-4969, Aug. 2017.
