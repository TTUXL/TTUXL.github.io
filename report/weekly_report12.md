Ultra-Dense Networks Notes
---

### Cited by 107. Samarakoon, Sumudu, et al. "Ultra dense small cell networks: Turning density into energy efficiency." IEEE Journal on Selected Areas in Communications 34.5 (2016): 1267-1280.[[1]](https://ieeexplore.ieee.org/abstract/document/7439746/)

The author of this paper focuses on the study of two issues. Joint power control and user scheduling in Ultra-Dense Networks.  
>Optimal Power control: ***Mean Field Theory***  
>UE Scheduling: ***Lyapunov Framework***

As the number of SBSs becomes large(BS->∞), the author considers that the interference tends to be bounded, since the path loss is modeled according to the inverse square law.

<center>
<img src="./Photos/mean_field_interference.jpg" width="650" height="400">
<center>Figure 1. Mean-field interference from the perspective of an SBS<a href="https://ieeexplore.ieee.org/abstract/document/7439746/">[1]</a></center>
</center>

**As BS->∞,the Interference**

<img src="https://latex.codecogs.com/gif.latex?I(t,{\rho}(t)\right))&space;=&space;{\eta}&space;\int_{\mathcal{X}}&space;p\left(t,\bm{x}^{\prime}\right)\vert&space;\tilde{h}\vert&space;^2\rho(t,\bm{x}^{\prime})&space;d\bm{x}^{\prime}" title="I(t,{\rho}(t)\right)) = {\eta} \int_{\mathcal{X}} p\left(t,\bm{x}^{\prime}\right)\vert \tilde{h}\vert ^2\rho(t,\bm{x}^{\prime}) d\bm{x}^{\prime}" />

<center>
<img src="./Photos/number_of_interations_to_solve_hjb_fpk.jpg" width="650" height="400">
<center>Figure 2. Number of iterations to solve the HJB-FPK PDEs for different number of SBSs in the system.<a href="https://ieeexplore.ieee.org/abstract/document/7439746/">[1]</a></center>
</center>

The optimal transmit power strategy is given by  

<img src="https://latex.codecogs.com/gif.latex?p^\star(t,\check{x}(t))=\underset{p(t,\check{x}(t))}{arg&space;max}\left&space;[&space;X_t&space;\frac{\partial}{\partial&space;x}[\Gamma(t,\check{x}(t)]&plus;f(t)&plus;\frac{1}{2}tr\left(X^2_z&space;\frac{\partial^2}{\partial&space;x^2}[\Gamma(t,\check{x}(t)]\right)\right&space;]" title="p^\star(t,\check{x}(t))=\underset{p(t,\check{x}(t))}{arg max}\left [ X_t \frac{\partial}{\partial x}[\Gamma(t,\check{x}(t)]+f(t)+\frac{1}{2}tr\left(X^2_z \frac{\partial^2}{\partial x^2}[\Gamma(t,\check{x}(t)]\right)\right ]" />

---
### Cited by 24. Liu, Liang, Shuowen Zhang, and Rui Zhang. "CoMP in the sky: UAV placement and movement optimization for multi-user communications." IEEE Transactions on Communications (2019).[[2]](https://ieeexplore.ieee.org/abstract/document/8675440)

The author consider the case where the users may move on the ground, thus the UAVs need to adjust their locations in accordance with the user locations over time to maximize the network throughput.   
***The contribution*** is to give the upper and lower bounded of ergodic rate.

<center>
<img src="./Photos/CoMP_UAV.jpg" width="650" height="400">
<center>Figure 3. Schematic of a UAV-enabled CoMP system.<a href="https://ieeexplore.ieee.org/abstract/document/7439746/">[2]</a></center>
</center>

In case of  LoS channel with Random phase.

<center>
<img src="./Photos/LoS_channel_random_phase.jpg" width="650" height="400">
<center>Figure 4. Simulated user ergodic rate under the LoS channel with random phase versus various approximations.<a href="https://ieeexplore.ieee.org/abstract/document/7439746/">[2]</a></center>
</center>

<img src="https://latex.codecogs.com/gif.latex?R_{k,l}^{upper}[n]&space;=&space;{\log&space;_2}&space;\left&space;(&space;{1&space;&plus;&space;\frac{PE{\left[|w_{k,l}[n]^Hh_{k,l}[n]|^2\right]}}{\sigma^2}&space;}&space;\right)" title="R_{k,l}^{upper}[n] = {\log _2} \left ( {1 + \frac{PE{\left[|w_{k,l}[n]^Hh_{k,l}[n]|^2\right]}}{\sigma^2} } \right)" />
