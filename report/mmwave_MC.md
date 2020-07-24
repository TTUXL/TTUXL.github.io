https://ieeexplore.ieee.org/abstract/document/7528494
#### Multi-connectivity in 5G mmWave cellular networks

The millimeter wave (mmWave) frequencies offer the potential of orders of magnitude increases in capacity for next-generation cellular wireless systems. However, links in mmWave networks are highly susceptible to blocking and may suffer from rapid variations in quality.Connectivity to multiple cells - both in the mmWave and in the traditional lower frequencies - is thus considered essential for robust connectivity. However, one of the challenges in supporting multi-connectivity in the mmWave space is the requirement for the network to track the direction of each link in addition to its power and timing.
>毫米波（mmWave）频率为下一代蜂窝无线系统提供了容量增加几个数量级的潜力。但是，mmWave网络中的链接极易受到阻塞的影响，并且质量可能会快速变化。但是，在毫米波空间中支持多连接性的挑战之一是，除了网络的功率和时序外，还要求网络跟踪每个链路的方向。对于高度定向的波束和快速变化的信道，这种定向跟踪可能是实现强大的毫米波网络的主要瓶颈。(我觉得不应该是跟踪，应该是到达角度判定（或信道相关性判断），才能保证不会同时被阻断)

However, one of the challenges in designing cellular networks in the mmWave bands is robustness, and one likely key feature of mmWave cellular networks that can improve robustness is multi-connectivity (MC)
>然而，在毫米波频段设计蜂窝网络的挑战之一是鲁棒性，而毫米波蜂窝网络可以提高鲁棒性的一个可能的关键特征是多连接性（MC）[Mobility modeling and performance evaluation of multi-connectivity in 5G intra-frequency networks", 2015]

Multi-connectivity is a feature in which each UE maintains multiple possible signal paths to different cells so that drops in one link can be overcome by switching data paths.
>多连接性是一种特征，其中每个UE维护通向不同小区的多个可能信号路径，从而可以通过切换数据路径来克服一条链路中的掉线。


 this paper proposes a novel multicell measurement reporting system where each UE directionally broadcasts a sounding reference signal (SRS) in a time-varying direction that continuously sweeps the angular space. Each potential serving cell scans all its angular directions and monitors the strength of the received SRS along with its variance, to better capture the dynamics of the channel. A centralized controller obtains complete directional knowledge from all the potential cells in the network to make the optimal serving cell selection and scheduling decision.
 >本文提出了一种新颖的多小区测量报告系统，其中，每个UE沿时变方向有方向地广播探测参考信号（SRS），该信号不断扫描角度空间。每个潜在服务小区均扫描其所有角度方向，并监视接收到的SRS的强度及其变化，以更好地捕获信道的动态。集中式控制器从网络中所有潜在的小区中获取完整的方向性知识，以做出最佳的服务小区选择和调度决策。


The key challenge in implementing multi -cell connectivity is that the network must, in essence, monitor the signal strength on each of the directions pairs for each of the possible links. This is done by each SCell building a report tables (RT), based on the channel quality of each receiving direction, per each user.
>实施多小区连接的主要挑战在于，网络本质上必须监视每个可能链路的每个方向对上的信号强度。这是由每个SCell根据每个接收方向，每个用户的报告质量（RT）构建报告表（RT）来完成的。

Frequent handover, even for fixed UEs, is a potential drawback of mmWave systems due to their vulnerability to random obstacles, which is not the case in LTE.
>毫米波系统由于容易受到随机障碍的影响，即使对于固定UE，频繁切换也是mmWave系统的潜在缺点，而LTE中并非如此

The key input information for the handover decision includes (i) instantaneous channel quality, (ii) channel variance, and (iii) cell occupancy.
>用于切换决定的关键输入信息包括（i）瞬时信道质量，（ii）信道方差和（iii）小区占用。


https://ieeexplore.ieee.org/abstract/document/7744807
#### Initial Access(IA) in 5G mmWave Cellular Networks

Moreover, small mmWave wave-lengths make it practical to build very large antenna arrays (e.g., with 32 or more elements) to provide further gains from spatial isolation and multiplexing.
>此外，小的mmWave波长使得建造非常大的天线阵列（例如，具有32个或更多的元件）以从空间隔离和多路复用中获得进一步的增益成为现实。

initial access (IA), which allows a mobile user equipment (UE) to establish a physical link connection with a base station (BS), a necessary step to access the network.
>初始访问（IA），它允许移动用户设备（UE）与基站（BS）建立物理链路连接，这是访问网络的必要步骤。

In mmWave bands, it may instead be essential to exploit the BF gains even during the CS phase, since omnidirectional signaling may generate a mismatch between the relatively short range at which a cell can be detected (C-plane range), and the much longer range at which a user could directionally send and receive data (U-plane range)
>在毫米波频段中，甚至在CS阶段也必须利用BF增益，因为全向信令可能会在相对短的距离（在此范围内可以检测到一个小区）（C平面范围）和更长的距离之间产生不匹配。用户可以定向发送和接收数据的范围（U平面范围）

In mmWave cellular networks, IA messages may not be received due to deafness or blockage phenomena. Deafness refers to a situation where the transmit-receive beams do not point to each other, whereas blockage causes a failed message delivery due to a channel drop, which may be related to obstacles, hand rotations, and other mmWave-sensitive events.
>在mmWave蜂窝网络中，由于耳聋或阻塞现象，可能不会收到IA消息。失聪是指发射-接收波束彼此不指向，而阻塞由于信道下降而导致消息传递失败，这种情况可能与障碍，手旋转以及其他mmWave敏感事件有关。

Due to denser topologies, association schemes based on reference signal received power (RSRP) would be highly inefficient in mmWave cellular networks, an issue already encountered in HetNets [6]. However, the challenge with higher frequencies is the need to also account for dynamics such as directionality and intermittency.
>由于拓扑密度较高，基于参考信号接收功率（RSRP）的关联方案在mmWave蜂窝网络中效率极低，这在HetNets中已经遇到[6]。但是，更高频率的挑战是还需要考虑动态性，例如方向性和间歇性。

In this study, we evaluate the performance in terms of:

Discovery delay, which is the time required by the BS and the UE to complete their angular scans (sending and receving PSS control messages, respectively), to determine and select the best directions through which to steer their beams

Misdetection probability (PMD), which is the probability that a UE within the cell is not detected by the BS in the cell search phase, perceiving an SNR below threshold
>在本研究中，我们根据以下方面评估性能：
>发现延迟，即BS和UE完成其角度扫描（分别发送和接收PSS控制消息）所需的时间，以确定并选择最佳的方向来控制波束
>误检测概率（PMD），是指在SNR低于阈值的情况下，BS在小区搜索阶段未检测到小区内的UE的概率

Periodical signaling for beam tracking, besides increasing the system complexity, results in additional resource and energy consumption.
>用于波束跟踪的定期信令除了增加系统复杂性之外，还导致额外的资源和能量消耗。

https://ieeexplore.ieee.org/document/7378276
#### User Association in 5G Networks: A Survey and an Outlook

Regardless of the technology adopted, a user association mechanism is needed to determine whether a user is associated with a particular base station (BS) before data transmission commences. User association plays a pivotal role in enhancing the load balancing, the spectrum efficiency, and the energy efficiency of networks.
>无论采用哪种技术，都需要一种用户关联机制来确定用户是否在数据传输开始之前与特定基站（BS）关联。用户关联在增强网络的负载平衡，频谱效率和能效方面起着关键作用.

A popular method of overcoming this issue is to make the problem convex by relaxing the user association matrix from xmn={0,1} to xmn=[0,1]. Then, the classic Lagrangian dual analysis [99] can be invoked, followed by recovering the primal user association matrix x from the optimal dual problem.
>解决此问题的一种流行方法是通过将用户关联矩阵从xmn = {0,1}放到xmn = [0,1]来使问题凸出。然后，可以调用经典的拉格朗日对偶分析[99]，然后从最佳对偶问题中恢复原始用户关联矩阵x。

The velocity of mobility also has a substantial effect on mmWave user association/re-association, which suggests that mobility management has to be adopted in mmWave networks [38]. Considering the fact that mmWave links are sensitive to blockage and mobility, the channel conditions may vary significantly over time and it may be necessary to request re-association after each channel coherence time.
>移动速度对mmWave用户关联/重新关联也有很大影响，这表明必须在mmWave网络中采用移动管理[38]。考虑到mmWave链路对阻塞和移动性敏感的事实，信道条件可能会随时间发生显着变化，并且可能有必要在每个信道相干时间之后请求重新关联.
