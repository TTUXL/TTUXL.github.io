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
3. **Small form factor:** The small wavelength of mm Wave implies that massive antennas can easily be equipped at both macro and small-cell BSs, which can easily be deployed with low-cost sites(e.g., light poles, building walls, bus stations).  $`\sqrt{2}`$.

```math
SE = \frac{\sigma}{\sqrt{n}}
```
#### MmWave Channels with Spatial/Angular Sparsity
MmWave massive MIMO channels exhibit the obviously spatial/angular sparsity due to its high path loss for non-line-of-sight (NLOS) signals. If we consider the widely used uniform linear array (ULA), the point-to-point mmWave massive MIMO channel can be modeled as[[3]](https://ieeexplore.ieee.org/abstract/document/6847111)(Cited by 1091):  
