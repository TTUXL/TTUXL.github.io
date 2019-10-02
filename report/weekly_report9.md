##  Ultra-Dense Network Notes  
---  
### MmWave massive-MIMO-based wireless backhaul for the 5G ultra-dense network, *Cited by 221*, IEEE Wireless Communications, 2015 [[1]](https://ieeexplore.ieee.org/document/7306533)
In this article, The author discusses the feasibility of mmWave massive-MIMO-based wireless backhaul for 5G UDN, and the benefits and challenges are also addressed. by leveraging the low-rank property of the mmWave massive MIMO channel matrix, The Author proposes a *digitally controlled phase shifter network*(***DPSN***)-based hybrid precoding/combining scheme and the associated *compressive sensing*(***CS***)-based channel estimation scheme.

#### The Advantages of MmWave are:
* A large amount of underutilized band in mmWave can be leveraged to provide the potential gigahertz transmission bandwidth.  
* A large number of antennas (massive MIMO) can easily be employed for mmWave communications due to the small wavelength of mmWave, which can improve the signal directivity (reduce the co-channel interference).  

#### MmWAVE is Suitable for Wireless Backhaul in 5G UDN:
1. **High-capacity:** A large amount of underutilized mmWave can provide potential gigahertz transmission bandwidth.
2. **Immunity to interference:** Due to high path loss, mmWave is suitable for UDN, where improved frequency reuse and reduced inter-cell interference are expected. If we consider very heavy rainfall of 25 mm/hr, the rain attenuation is only around 2 dB in E-band if we consider the distance of a backhaul link is 200 m in typical urban UDN[[2]](https://ieeexplore.ieee.org/abstract/document/7000981).  
3. **Small form factor:** The small wavelength of mm Wave implies that massive antennas can easily be equipped at both macro and small-cell BSs, which can easily be deployed with low-cost sites(e.g., light poles, building walls, bus stations).

<img src="https://latex.codecogs.com/gif.latex?H&space;=&space;\sqrt&space;{\frac{N_T&space;N_R}{\rho&space;}}&space;\sum\limits_{l&space;=&space;1}^L&space;{\alpha_l&space;\mathbf{a}_T({\theta_l})\mathbf{b}_R^&space;*({\varphi_l})}" title="H = \sqrt {\frac{N_T N_R}{\rho }} \sum\limits_{l = 1}^L {\alpha_l \mathbf{a}_T({\theta_l})\mathbf{b}_R^ *({\varphi_l})}" />

#### MmWave Channels with Spatial/Angular Sparsity
MmWave massive MIMO channels exhibit the obviously spatial/angular sparsity due to its high path loss for non-line-of-sight (NLOS) signals. If we consider the widely used uniform linear array (ULA), the point-to-point mmWave massive MIMO channel can be modeled as[[3]](https://ieeexplore.ieee.org/abstract/document/6847111)(Cited by 1091):



where NT and NR are the numbers of transmit and receive antennas, respectively, ρ is the average path loss, L is the number of paths, αl is the complex gain of the lth path, and Θ ∈[0,2π] and φ ∈[0,2π] are azimuth angles of departure or arrival (AoD/AoA). In addition,  

<img src="https://latex.codecogs.com/gif.latex?\mathbf{a}_{T}(\theta_{l})=\frac{1}{\sqrt{N_{T}}}[1,&space;e^{j2\pi&space;d\text{sm}(\theta)/\lambda},\cdots,&space;e^{j2\pi(N_{T}-1)d\sin(\theta_{l})/\lambda}]^{\text{T}}" title="\mathbf{a}_{T}(\theta_{l})=\frac{1}{\sqrt{N_{T}}}[1, e^{j2\pi d\text{sm}(\theta)/\lambda},\cdots, e^{j2\pi(N_{T}-1)d\sin(\theta_{l})/\lambda}]^{\text{T}}" />

and

<img src="https://latex.codecogs.com/gif.latex?\mathbf{b}_{R}(\varphi_{l})=\frac{1}{\sqrt{N_{R}}}[1,&space;e^{j2\pi&space;d\sin(\varphi)/\lambda},\cdots,&space;e^{j2\pi(N_{R}-1)d\sin(\varphi_{l})/\lambda}]^{\text{T}}" title="\mathbf{b}_{R}(\varphi_{l})=\frac{1}{\sqrt{N_{R}}}[1, e^{j2\pi d\sin(\varphi)/\lambda},\cdots, e^{j2\pi(N_{R}-1)d\sin(\varphi_{l})/\lambda}]^{\text{T}}" />

#### The Advantages of MmWave Massive MIMO for Channel Estimation  
1. Due to the fixed BS locations and close proximity, mmWave massive MIMO channels used for backhaul stay almost unchanged for a long time. This long coherence time of channels indicates that channels do not need to be estimated very frequently compared to that in RAN.  
2. The low-rank property of the mmWave massive MIMO channel matrix indicates that although the dimension of the matrix can be huge, its effective degrees of freedom (DoF) can be small.  

#### Open Issues
 To realize mmWave massive-MIMO-based backhaul, the cost of conventional high-speed ADC with high resolution can be unaffordable, so low-resolution ADC with low hardware cost is appealing. So far, l-bit ADC-based signal detection and precoding/com-bining have been investigated for mmWave massive MIMO. if low-resolution ADC is adopted, constellation mapping, channel estimation, training signals, and so on may need to be reconsidered.

---

#### Terahertz-Enabled Wireless System for Beyond-5G Ultra-Fast Networks: A Brief Survey, IEEE Network, 2019[[4]](https://ieeexplore.ieee.org/abstract/document/8782882)

This article provides a brief survey of the challenges and opportunities of THz band operation in wireless communication, along with some potential applications and future research directions.

**Beyond-5G (B5G) system**: With 5G Phase 1 finalized and 5G Phase 2 recently defined by 3GPP, B5G is expected to further enhance network performance.

##### There are three major ways to obtain several orders of increase in throughput gain:
  1. Extreme densification of the communication infrastructure.  
  2. Large quantities of newly available spectrum.  
  3. Massive antenna systems, allowing a throughput gain in the spatial dimension.

##### THz spectrum is different from mmWave spectrum
1.  In fact, in THz communications, tera-bit-per-second links could be realized with less spectral efficiency (SE) than at mmWave frequencies.
2.  In addition, THz frequencies enable more directionality than mmWave due to reduced antenna aperture.
3. The shorter wavelength of THz when compared to mmWave makes it more directional and less prone to free-space diffraction.
4. distances between the transmitter and receiver in THz will be much shorter than in mmWave. This will result in the reduction of power consumption.

##### The primary technical objectives for THz communication for B5G ultra-fast networks
* Ultra-high data rates per device (from multiple tens of gigabits to terabits per second) with sufficient transmission distance in complex network environments  
* Ultra-high data rates per area and ultra-massive amounts of connected devices  
* Ultra-reliable connectivity to support various critical applications in mobility environments  
*  Very high energy efficiency (EE) to support ultra-high rates for various mobile terminals and networks  

##### Standardization of THz Communication
Standardization of THz wireless communications started in early **2008** when IEEE established an Interest Group on THz communications (IGTHz).Subsequently, after a couple of years of inactivity, the **IEEE 802.15.3d** (100 Gb/s Wireless) Task Group was established in order to facilitate the standardization of THz communications.  The frequency range in focus has been mostly limited to **252–325 GHz**, while different types of communications (backhaul/fronthaul) for 5G.

##### Emerging Applications of THz Band Communication
automotive, indoor networking, aerospace, healthcare, intrinsically safe environments, location-based services, defense, underwater communication, and so on.  
**Vehicular Communications**
* **Vehicle-to-vehicle (V2V)** communications, where neighboring/cooperating vehicles share perceptual data with each other using THz bands for high-rate and low-latency communication.Each vehicle can use the shared data to extend its perception range, which enables it to reveal hidden objects ahead or in its blind spots and thereby avoid collision with other vehicles.   

* **ehicle-to-infrastructure (V2I)** communications in which the infrastructure or *roadside units (RSUs)* gather sensing data about the vehicles and the surrounding traffic. The sensed data can be used to provide realtime maps of the environment. These maps can be used by the transportation control system for congestion avoidance.

* **In-car communications** where THz bands can provide ultra-high-rate and short-range in-car communication for autonomous driving systems, as well as device-to-device (D2D)-like services for the passengers of the vehicles.

**THz Wireless Fronthaul for a C-RAN-Based System**  
The THz fronthaul is compatible with the ultra-dense deployment of small cells because the fronthaul link can be rather short, so as to mitigate the high path loss of THz signals and guarantee connectivity via line-of-sight (LoS) links.
<center>
<img src="./Photos/THz_fronthaul_c_ran.gif" width="850" height="300">
<center>Figure 1. THz band wireless fronthaul for C-RAN.<a href="https://ieeexplore.ieee.org/abstract/document/8782882">[4]</a></center>
</center>
