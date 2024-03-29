# Memory Design Workshop 2021
<img src = "media/poster.jpg">
This repository reflects the work done in the lab sessions the Memory Design Workshop 2021 (MDW), offered by IEEE Banglore Section and IEEE CAS Banglore Chapter. The event was comprised of 5 days of lectures,2 in a day from Industry maestros and esteemed academicians, followed by self-paced hands-on lab session spanning over 2 weeks, aiming to familiarise ourselves with freeware tools, PDKs, Analog Design focusing on Memory Designs and Concepts.

## Table of Contents

- [About](#about)
- [Lab 1](#Lab-1)
- [Lab 2](#Lab-2)
- [Lab 3](#Lab-3)
- [Lab 4](#Lab-4)
- [Future Scope](#future-scope)


## About
This workshop presents a basic overview of different SRAM Cell Designs using [LTSpice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) and ASU's [Arizona State Predictive PDK (ASAP)](https://asap.asu.edu/) 14nm FinFET node, using an intuitive approach to designing a simple SRAM Cells. This workshop also provides deep insights into recent advancements and current research trends in Memory Cell Designs. Here I have uploaded all the works done by me in 4 lab sessions organized by this workshop.

## Lab 1
- Understand basic analysis types in LTSpice.
- Run an inverter transient and DC analysis.
- Assignment :
	- Calculate the power of a nominally sized inverter driving a load of 1fF/5fF.
	- Calculate Fan out of 1 (FO1) and Fan out of 4 (F04) delay of the nominally sized inverter at nominal and +/-10% supply.
	- Calculate the leakage power of a 50fin inverter and compare it with a 22nm planar FET inverter of the same width.

Schematic Diagram :
- NMOS: Id vs Vgs Schematic Diagram </br>
  <img src = "lab1/nmos_id_vgs_l1.jpg" width="50%" height="50%"> </br>
- NMOS: Id vs Vds Schematic Diagram  </br> 
  <img src = "lab1/nmos_id_vds_l1.jpg" width="50%" height="50%"> </br>
- PMOS: Id vs Vgs Schematic Diagram  </br> 
  <img src = "lab1/pmos_id_vgs_l1.jpg" width="50%" height="50%"> </br>
- PMOS: Id vs Vds Schematic Diagram  </br> 
  <img src = "lab1/pmos_id_vds.jpg" width="50%" height="50%"> </br>

Resultant Waveform :
- NMOS: Id vs Vgs plots </br>
<img src = "lab1/op_nmos_id_vgs.jpg" width="70%" height="70%"> </br>
Different colors showing different values of Id when w = 320, 640, 960, 3200, 4200n </br>
- NMOS: Id vs Vds plots </br>
<img src = "lab1/op_nmos_id_vds.jpg" width="70%" height="70%"> </br>
Different colors showing different values of Id when Vgs = 0, 1, 2, 3, 4, 5 V </br>
- PMOS: Id vs Vgs plots </br>
<img src = "lab1/op_nmos_id_vgs.jpg" width="70%" height="70%"> </br>
Different colors showing different values of Id when w = 320, 640, 960, 3200, 4200n </br>
- PMOS: Id vs Vds plots </br>
<img src = "lab1/op_pmos_id_vds.jpg" width="70%" height="70%"> </br>
Different colors showing different values of Id when Vgs = 0, 1, 2, 3, 4, 5 V </br>


## Lab 2
- Run an inverter transient and DC analysis.
- Assignment :
	- Calculate the power of a nominally sized inverter driving a load of 1fF/5fF.
	- Calculate Fan out of 1 (FO1) and Fan out of 4 (F04) delay of the nominally sized inverter at nominal and +/-10% supply.
	- Calculate the leakage power of a 50fin inverter and compare it with a 22nm planar FET inverter of the same width.

Schematic Diagram :
- CMOS Inverter Schematic Diagram </br>
DC Analysis </br>
<img src = "lab2/dc_cmos_inv.jpg" width="50%" height="50%"> </br>
AC Analysis </br>
<img src = "lab2/ac_cmos_inv.jpg" width="50%" height="50%"> </br>
Transient Analysis </br>
<img src = "lab2/cmos_inv.jpg" width="50%" height="50%"> </br>

Resultant Waveform :
- CMOS Inverter Waveform </br>
DC Analysis </br>
<img src = "lab2/op_dc_cmos_inv.jpg" width="70%" height="70%"> </br>
AC Analysis </br>
<img src = "lab2/op_ac_cmos_inv_corr.jpg" width="70%" height="70%"> </br>
Transient Analysis </br>
<img src = "lab2/op_cmos_inv.jpg" width="70%" height="70%"> </br>
- Power Analysis </br>
Load = 1fF </br>
<img src = "lab2/power_cmos_1f.jpg" width="70%" height="70%"> </br>
Total Power consumed by CMOS Inverter = 201.78 μW (PMOS) + 202.57 μW (NMOS) </br>
Load = 5fF </br>
<img src = "lab2/power_cmos_5f.jpg" width="70%" height="70%"> </br>
Total Power consumed by CMOS Inverter = 202.57 μW (PMOS) + 202.83 μW (NMOS) </br>


## Lab 3
- Desing and Analysis of 6T SRAM Cell.
- Perform Static-noise margin analysis of the same refer to this ["Static-noise margin analysis of MOS SRAM cells"](https://ieeexplore.ieee.org/document/1052809) and [Link](https://engineering.purdue.edu/~vlsi/ECE559_Fall09/HW/HW6_Solution.pdf)

Schematic Diagram :
- Transient Analysis of 6T SRAM Cell </br>
<img src = "lab3/sram_6t.jpg" width="50%" height="50%"> </br>
- Static-noise margin analysis of 6T SRAM Cell </br>
<img src = "lab3/sram_6t_snm.jpg" width="50%" height="50%"> </br>

Resultant Waveform :
- Transient Analysis of 6T SRAM Cell </br>
<img src = "lab3/op_Sram_6t.jpg" width="70%" height="70%"> </br>
- Static-noise margin analysis of 6T SRAM Cell </br>
<img src = "lab3/op_sram6t_snm_1.jpg" width="70%" height="70%"> </br>
<img src = "lab3/op_sram6t_snm_2.jpg" width="70%" height="70%"> </br>
<img src = "lab3/op_sram6t_snm_3.jpg" width="70%" height="70%"> </br>


## Lab 4
- Desing and Analysis of 8T and 10T SRAM Cell.
- Perform Static-noise margin analysis of the same refer to this ["Static-noise margin analysis of MOS SRAM cells"](https://ieeexplore.ieee.org/document/1052809) and [Link](https://engineering.purdue.edu/~vlsi/ECE559_Fall09/HW/HW6_Solution.pdf)

Schematic Diagram :
- Transient Analysis of 8T SRAM Cell </br>
<img src = "lab4/sram_8t/sram_8t.jpg" width="50%" height="50%"> </br>
- Static-noise margin analysis of 6T SRAM Cell </br>
<img src = "lab4/sram_8t/sram8t_snm.jpg" width="50%" height="50%"> </br>

- Transient Analysis of 10T SRAM Cell </br>
<img src = "lab4/sram_10t/sram_10t.jpg" width="50%" height="50%"> </br>
- Static-noise margin analysis of 10T SRAM Cell </br>
<img src = "lab4/sram_10t/sram10t_snm.jpg" width="50%" height="50%"> </br>

Resultant Waveform :
- Transient Analysis of 8T SRAM Cell </br>
<img src = "lab4/sram_8t/op_sram8t.jpg" width="70%" height="70%"> </br>
- Static-noise margin analysis of 8T SRAM Cell </br>
<img src = "lab4/sram_8t/op_sram8t_snm.jpg" width="70%" height="70%"> </br>
<img src = "lab4/sram_8t/op_sram8t_snm_1.jpg" width="70%" height="70%"> </br>
<img src = "lab4/sram_8t/op_sram8t_snm_2.jpg" width="70%" height="70%"> </br>

- Transient Analysis of 10T SRAM Cell </br>
<img src = "lab4/sram_10t/op_sram10t.jpg" width="70%" height="70%"> </br>
- Static-noise margin analysis of 10T SRAM Cell </br>
<img src = "lab4/sram_10t/op_sram10t_snm_1_1.jpg" width="70%" height="70%"> </br>
<img src = "lab4/sram_10t/op_sram_10t_snm_2_1.jpg" width="70%" height="70%"> </br>
<img src = "lab4/sram_10t/op_sram10t_snm_3.jpg" width="70%" height="70%"> </br>


## Future Scope
- Work on getting specifications and change your designs according to them.
- After changing in your design, make this design as your own IP.
- Design Layouts and Verify them with LVS and DRC Checks.
