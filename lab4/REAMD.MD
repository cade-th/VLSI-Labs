# Lab 4: Inverter

Cade Thornton

10/28/2023

ENCE 3501

## Table of Contents

-------

+ [Introduction](#Introduction )
+ [Inverter 1](#Inverter1)
    * [Schematic](#Schematic)
    * [Layout](#Layout)
    * [Simulations](#Simulations)
+ [Inverter 2](#Inverter2)
    * [Schematic](#Schematic)
    * [Layout](#Layout)
    * [Simulations](#Simulations)
+ [Conclusion](#Conclusion)

## Introduction 

-------

<p align="center">
The purpose of this lab is to utilize NMOS, PMOS, NWELL and PWELL standard library components to construct a CMOS inverter of various sizes.
<p>

<p align="center">
  <img src="Inverter/documentation/CMOSinverter.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 1 (CMOS Inverter Schematic)
  </p>
</div>

## Inverter 1

### Schematic

<p align="center">
Below is the electricVLSI schematic of the first inverter. It is necessary to make the PMOS transistor larger than the NMOS (PMOS is 12 by 6 while the NMOS is 6 by 6)
<p>

<p align="center">
  <img src="Inverter/documentation/inverter1/schematics/inverter1sch.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 2 (CMOS inverter 1 schematic)
  </p>
</div>

<p align="center">
And here is the generated icon from electricVLSI
<p>

<p align="center">
  <img src="Inverter/documentation/inverter1/schematics/inverter1icon.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 3 (CMOS inverter 1 schematic icon)
  </p>
</div>

### Layout 

<p align="center">
Below is the created layout, which has been constructed in accordance with the schematic, utilizing the NMOS and PMOS provided by the standard library. The PMOS is tied to an nWell that serves as vdd, while the NMOS links to a pWell that functions as the ground. The connection of the NMOS and PMOS follows the design outlined in the schematic.
<p>

<p align="center">
  <img src="Inverter/documentation/inverter1/layouts/inverter1layout.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 4 (CMOS inverter 1 layout)
  </p>
</div>

<p align="center">
Here is a 3D view of the layout which demonstrates the pWell and nWell connections
<p>

<p align="center">
  <img src="Inverter/documentation/inverter1/3Dview/inverter1layout3D.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 5 (CMOS inverter 1 layout 3D view)
  </p>
</div>



### Simulations 

<p align="center">
The spice code applies 5V across the inverter for a duration of 1ms in the initial simulation of Inverter 1, which is aimed at evaluating the inverter's switching threshold. The optimal switching point for the inverter is expected to be at half of vdd.
<p>

<p align="center">
  <img src="Inverter/documentation/inverter1/simulations/Inverter1Sim.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 6 (CMOS inverter 1 simulation)
  </p>
</div>

<p align="center">
The waveform for the results of the simulation is shown below. The simulation results were deemed successful as the switching point occurred at 2.416V, which is approximately half of vdd, given that vdd was 5V. 
<p>




------

## Inverter 2

### Schematic 
### Layout 
### Simulations 


-------

## Conclusion

------


