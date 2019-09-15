## LTE Implementation Issue on USRP Testbed
---
### The famous two LTE open source platforms do not support Ettus N210.
#### 1. OpenAirInterface
[https://gitlab.eurecom.fr/oai/openairinterface5g/wikis/OpenAirSystemRequirements#supported-rf](https://gitlab.eurecom.fr/oai/openairinterface5g/wikis/OpenAirSystemRequirements#supported-rf)
>**Supported RF:**
>
>   USRP B210 [http://www.ettus.com/product/details/UB210-KIT](http://www.ettus.com/product/details/UB210-KIT)
>
>   USRP X310 [http://www.ettus.com/product/details/X310-KIT](http://www.ettus.com/product/details/X310-KIT)
>
>   BladeRF [http://nuand.com/](http://nuand.com/)
>
>   LimeSDR [http://limesdr.org/](http://limesdr.org/)
>
>   EURECOM EXPRESSMIMO2 RF, [http://openairinterface.eurecom.fr](http://openairinterface.eurecom.fr)

#### 2. srsLTE
[https://github.com/srsLTE/srsLTE#hardware](https://github.com/srsLTE/srsLTE#hardware)
>**Hardware**
>
>The library currently supports the Ettus Universal Hardware Driver (UHD) and the bladeRF driver. Thus, any hardware supported by UHD or bladeRF can be used. There is no sampling rate conversion, therefore the hardware should support 30.72 MHz clock in order to work correctly with LTE sampling frequencies and decode signals from live LTE base stations.
>
>We have tested the following hardware:
>
>* USRP B210
>* USRP B205mini
>* USRP X300
>* limeSDR
>* bladeRF

----

###
