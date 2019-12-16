## Problem Formulation

we formulate the optimization problem to minimize the total energy by ultra-reliable and low-latency communications(URLLC).

An ultra density network constructs by numbers of base stations, which can increase the capacity of network by using large number of base stations. Hoverer due to the increasing numbers of base station, the issue of energy consumption has more and more challenged.


Here, the network energy efficiency can be expressed as a non-convex optimization problem, considering the best energy efficiency under the premise of meeting Quality of service (QoS).
As the network becomes denser, the cost of acquiring channel state information increases significantly. Obtaining perfect CSI is almost no longer possible. A lot of literature has been researched on this issue []-[], and many practical methods to maximize energy efficiency have been proposed. However, how to improve QoS is the final goal.

In this problem, low latency and ultra-high reliability are two contradictory requirements. On one hand, if it is only optimized minimum waiting time, this requires using short packets, which results in a reduction in channel coding gain. At the same time, it increases the demand for channel information acquisition.  On the other hand, in order to ensure reliable transmission, more checksum redundancy is required. Although the need for real-time channel is reduced, the delay time is greatly increased. Considering these two control strategies, how to optimize them two has become an urgent need.
---
### A. Constraints:

##### Total power constraint:

<a href="https://www.codecogs.com/eqnedit.php?latex=\sum\limits_i&space;{{p_{ij}}&space;\le&space;{P_{\max&space;}}}&space;,\forall&space;j&space;\in&space;B" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\sum\limits_i&space;{{p_{ij}}&space;\le&space;{P_{\max&space;}}}&space;,\forall&space;j&space;\in&space;B" title="\sum\limits_i {{p_{ij}} \le {P_{\max }}} ,\forall j \in B" /></a>

where Pmax denotes the maximum transmit power between user i and BS j.

##### Delay constraint:

<a href="https://www.codecogs.com/eqnedit.php?latex=d{q_b}(t)&space;=&space;{a_b}(t)&space;-&space;{r_b}(t,Y(t),\overline{h(t)})dt" target="_blank"><img src="https://latex.codecogs.com/gif.latex?d{q_b}(t)&space;=&space;{a_b}(t)&space;-&space;{r_b}(t,Y(t),\overline{h(t)})dt" title="d{q_b}(t) = {a_b}(t) - {r_b}(t,Y(t),\overline{h(t)})dt" /></a>

where ab(t) and rb(·) are the vectors of arrivals and transmission rates at SBs. Y(t) is function of the Package length，h(t) is probability functions of CSI.


##### SNIR constraint:

<a href="https://www.codecogs.com/eqnedit.php?latex=\Pr&space;\left\{&space;{SNIR&space;\ge&space;{\gamma&space;_i}}&space;\right\}&space;\ge&space;1&space;-&space;{\rho&space;_i}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\Pr&space;\left\{&space;{SNIR&space;\ge&space;{\gamma&space;_i}}&space;\right\}&space;\ge&space;1&space;-&space;{\rho&space;_i}" title="\Pr \left\{ {SNIR \ge {\gamma _i}} \right\} \ge 1 - {\rho _i}" /></a>

##### Constraint on the number of associated users:

<a href="https://www.codecogs.com/eqnedit.php?latex=\sum\limits_i&space;{{x_{ij}}&space;=&space;{K_j}}&space;,&space;&{where}&{0&space;\le&space;{K_j}&space;\le&space;{N_u}}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\sum\limits_i&space;{{x_{ij}}&space;=&space;{K_j}}&space;,&space;&{where}&{0&space;\le&space;{K_j}&space;\le&space;{N_u}}" title="\sum\limits_i {{x_{ij}} = {K_j}} , &{where}&{0 \le {K_j} \le {N_u}}" /></a>

where Xij is the number of user under everyone BS.


### B. Energy Efficiency Optimization Problem

For energy efficient communication, we aim to maximize the total communication data rate with the unit power cost. Therefore, we formulate the system energy efficiency as a ratio of the system sum rate to the total power consumption. The energy efficiency of the system is formulated as

<a href="https://www.codecogs.com/eqnedit.php?latex={\eta&space;_{EE}}(U,P)&space;=&space;\frac{R(U,P)}{P_s(U,P)}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?{\eta&space;_{EE}}(U,P)&space;=&space;\frac{{R(U,P)}}{{P_s}(U,P)}" title="{\eta _{EE}}(U,P) = \frac{{R(U,P)}}{{{P_s}(U,P)}}" /></a>

where U is user scheduling policy, P is power allocation policy. R(U,P) is Data transfer rate. Ps(U, P) = Pc + PT is the total power consumption of the system; Pc and PT are the circuit power consumption and transmission power.
