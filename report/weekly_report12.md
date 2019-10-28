Ultra-Dense Networks Notes
---

### Cited by 107. Samarakoon, Sumudu, et al. "Ultra dense small cell networks: Turning density into energy efficiency." IEEE Journal on Selected Areas in Communications 34.5 (2016): 1267-1280.[[1]](https://ieeexplore.ieee.org/abstract/document/7439746/)

The author of this paper focuses on the study of two issues. Joint power control and user scheduling in Ultra-Dense Networks.  
>Optimal Power control: ***Mean Field Theory***
>UE Scheduling: ***Lyapunov Framework***

As the number of SBSs becomes large(|B|->∞), the author considers that the interference tends to be bounded, since the path loss is modeled according to the inverse square law.

<center>
<img src="./Photos/mean_field_interference.jpg" width="650" height="400">
<center>Figure 1. Mean-field interference from the perspective of an SBS<a href="https://ieeexplore.ieee.org/abstract/document/7439746/">[1]</a></center>
</center>

as |B|->∞,the Interference

<img src="https://latex.codecogs.com/gif.latex?I(t,{\rho}(t)\right))&space;=&space;{\eta}&space;\int_{\mathcal{X}}&space;p\left(t,\bm{x}^{\prime}\right)\vert&space;\tilde{h}\vert&space;^2\rho(t,\bm{x}^{\prime})&space;d\bm{x}^{\prime}" title="I(t,{\rho}(t)\right)) = {\eta} \int_{\mathcal{X}} p\left(t,\bm{x}^{\prime}\right)\vert \tilde{h}\vert ^2\rho(t,\bm{x}^{\prime}) d\bm{x}^{\prime}" />

<center>
<img src="./Photos/number_of_interations_to_solve_hjb_fpk.jpg" width="650" height="400">
<center>Figure 2. Number of iterations to solve the HJB-FPK PDEs for different number of SBSs in the system.<a href="https://ieeexplore.ieee.org/abstract/document/7439746/">[1]</a></center>
</center>
