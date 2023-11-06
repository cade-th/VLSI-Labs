# Lab 3: NMOS with Basic ESD Pad Protection

Cade Thornton

10/30/2023

ENCE 3501

## Table of Contents

-------

+ [Introduction](#Introduction )
+ [ESD Pad Cell](#Link)
    * [Schematic](#Schematic)
    * [Layout](#Layout)
+ [ESD Padfame](#Link)
    * [Schematic](#Schematic)
    * [Layout](#Layout)
+ [Final IC](#Link)
    * [Schematic](#Schematic)
    * [Layout](#Layout)
+ [Conclusion](#Conclusion)

## Introduction 

<p align="center"> 
In this lab, the objective is to re-create the padframe from the previous lab, but this time with electrostatic discharge protection that prevents the internal logic from being damaged. The cicuit in the padframe this time will be a simple NMOS transistor instead of a DACc
</p>

<p align="center">
  <img src="ICESD/documentation/finalICESD/schematics/generalidea.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 1 (General Idea of Padframe IC)
  </p>
</div>

## ESD Pad Cell

### Schematic

<p align="center"> 
The pad cell schematic is essentially an PMOS transistor, with the input connected to a pActive-nWell diode, the ground connected to a pWell-nActive diode, and the export pin of the cell connected between both diodes.
</p>

<p align="center">
  <img src="ICESD/documentation/padESD
/schematics/padESDsch.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 2 (ESD Pad Cell Schematic)
  </p>
</div>

<p align="center"> 
And this is the generated icon for from the previous schematic.
</p>

<p align="center">
  <img src="ICESD/documentation/padESD
/schematics/padESDicon.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 3 (ESD Pad Cell Schematic Icon)
  </p>
</div>

### Layout 

<p align="center"> 
Using the existing pWell-nActive and pActive-nWell diode designs, the pad cell layout was constructed. The pad cell is linked to a pActive-nWell diode, which connects to a metal one contact designated as the voltage output. For grounding, the pWell-nActive diode is tied to the pad cell and then to a contact that bridges metal one and metal two layers. This setup leads to a metal two layer that stretches to an additional metal one contact, serving as the ground output. Moreover, the metal two layer that connects to the pWell-nActive diode is strategically placed to cross over the voltage bus in the overall padframe design. Positioned on the metal two layer, the input/output pin connects the two diodes within the pad cell's architecture.
</p>

<p align="center">
  <img src="ICESD/documentation/padESD
/layouts/padCell_layout.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 4 (ESD Pad Cell Layout)
  </p>
</div>

<p align="center"> 
Here is a 3D view to better see how the diodes are connected
</p>

<p align="center">
  <img src="ICESD/documentation/padESD
/3Dview/padCell3D.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 4 (ESD Pad Cell Layout)
  </p>
</div>

------

## ESD Padframe

### Schematic 

<p align="center"> 
Next, we can use the pad cell icon to constuct the padframe in a similar manner to the previous lab, with eight exports connected to a bus (pin[1] - pin[8]) to accomodate the NMOS transistor's four outputs and four inputs.
</p>

<p align="center">
  <img src="ICESD/documentation/padframeESD
/schematics/ESDpadframe.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 5 (ESD Pad Frame Schematic)
  </p>
</div>

<p align="center"> 
And the correspoding icon from electricVLSI:
</p>

<p align="center">
  <img src="ICESD/documentation/padframeESD
/schematics/ESDpadframeIcon.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 6 (ESD Pad Frame Schematic Icon)
  </p>
</div>

### Layout 

<p align="center">
The padframe layout was made using eight of the cell layouts used previusly with ESD protection. A bus is used to connect the ground and voltage for each cell. 
</p>

<p align="center">
  <img src="ICESD/documentation/padframeESD
/layouts/padFrameESDlayout.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 7 (ESD Pad Frame Layout)
  </p>
</div>

<p align="center">
And here is the 3D view of the padframe layout
</p>

<p align="center">
  <img src="ICESD/documentation/padframeESD
/3Dview/ESDpadframe3D.png" alt="img">
</p>

<div align="center">
  <p style="font-size: small;">
    Figure 8 (ESD Pad Frame Layout in 3D)
  </p>
</div>

## Final IC

### Schematic 



### Layout 


-------

## Conclusion

------


