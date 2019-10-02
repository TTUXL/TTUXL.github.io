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
