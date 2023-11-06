# Lab 1: 5-Bit R2R VLSI

Cade Thornton

10/16/2023

ENCE 3501

## Table of Contents

+ [Introduction](#Introduction )
+ [Voltage Divider](#VoltageDivider)
    * [Schematic](#Schematic)
    * [Layout](#Layout)
    * [Simulations](#Simulations)
+ [5-Bit R2R DAC](#5-BitR2RDAC)
    * [Hand Calc](#HandCal)
    * [Schematic](#Schematic)
    * [Layout](#Layout)
    * [Simulations](#Simulations)
+ [Conclusion](#Conclusion)

## Introduction 
<p align="center">
In this lab, a  virtual 5-bit R2R DAC Circuit is made using Electric VLSI. The design is verified using LTSpice, and consists of a voltage divider resistor IC combined in parallel with other copies of the ic to form the DAC. The layout was made in a similar manner. 
</p>

<p align="center">
  <img src="5B_R2R_DAC/documentation/5B_R2R_DAC/schematics/lab1DACsch.png" alt="lab1Sch">
</p>
<div align="center">
  <p style="font-size: small;">
    Figure 1 (Schematic of R2R Ladder System)
  </p>
</div>



## Voltage Divider

### Schematic

<p align="center"> 
The provided schematic features two resistors. The one linked to the input boasts a resistance that is twice that of the resistor linked to the ground. With a resistance value of 10kΩ for the resistor connected to ground, the one connected to the input exhibits a resistance of 20kΩ.
</p>

<p align="center">
  <img src="5B_R2R_DAC/documentation/R_Divider/schematics/R_DIVSCH.png" alt="lab1Sch" width="400">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 2 (Schematic of Given Voltage Divider)
  </p>
</div>

<p align="center"> 
An electric VLSI schematic was created from the above schematic, with two 10k ohm resistors replacing 2R
</p>

<p align="center">
  <img src="5B_R2R_DAC/documentation/R_Divider/schematics/RDIVschematic.png" alt="lab1Sch">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 3 (ElectricVLSI Schematic of Voltage Divider)
  </p>
</div>

<p align="center"> 
The schematic generated an icon which was modified to be compact enough to be placed for the DAC

<p align="center">
  <img src="5B_R2R_DAC/documentation/R_Divider/schematics/RIDVicon.png" alt="lab1Sch">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 4 (ElectricVLSI Icon of Voltage Divider)
  </p>
</div>

</p>

### Layout 

### Simulations 

------

## 5-Bit R2R DAC

### Hand Calc
### Schematic 
### Layout 
### Simulations 


-------

## Conclusion

------


