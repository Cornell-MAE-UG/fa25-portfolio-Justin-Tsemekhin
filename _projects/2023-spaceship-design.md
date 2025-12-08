---
layout: project
title: Torque Wrench
description: Finite element analysis of torque wrench design
technologies: [ANSYS, MatLab, AutoDesk Fusion]
image: /assets/images/ansys.jpg
---

This image shows a modified CAD model for a torque wrench with acceptable factors of safety for a 600 lb-in moment. The material used for calculations is Aluminum, 2017, T4 given its high yield strength and relatively low cost (~$1.34/lb). This material is one of the cheapest that meets the design criteria, as calculated by hand, and would allow for lower cost for production. 

E = 10.7e6 psi
Yield Strength = 57.9e3 psi
Poisson's Ratio = 0.365
Fracture Toughness = 26.2e3 psi*in^1/2
Fatigue strength @10^6 cycles = 29.15e3 psi

## **Dimensioned CAD Model**
![Torque Wrench Dimensions]({{ "/assets/images/Wrench_dims.jpg" | relative_url }}){: style="width: 550px;"}

This updated model of the a rectangular torque wrench features a 4.5" handle for improved comfort whilst maintaining other basic dimensions. The driver is 3/8", the overall length 16", the width 0.75" (1.1" at the widest part of the handle) and is 0.5" in height. 

## **Loads and Boundary Conditions**
![Torque Wrench Dimensions]({{ "/assets/images/boundary_conditions.jpg" | relative_url }}){: style="width: 550px;"}

Applied 37.5lb load at 16in away from driven bit to create 600in-lbf torque which created a 0.38589" maximum deflection at tip furthest from driven bit. 

## **Normal Strain Contours**
![Torque Wrench Dimensions]({{ "/assets/images/strain_contour.jpg" | relative_url }}){: style="width: 550px;"}
## **Maximum Principle Stress**
![Torque Wrench Dimensions]({{ "/assets/images/max_ps.jpg" | relative_url }}){: style="width: 550px;"}

The value for maximum principle stress from the FEM is significantly higher than what was calculated by hand. This is likely due to a large stress concentration resulting from a sharp corner at a filet intersection. This should be improved upon in future iterations. 

## **Maximum Normal Stress**
![Torque Wrench Dimensions]({{ "/assets/images/max_ns.jpg" | relative_url }}){: style="width: 550px;"}

## **Hand Calculated Results** 

hand calculated (FEM result)

max deflection = 0.272 in (0.38579in)
Max stress = 12.80 ksi(36.549ksi)
strain @ guage = 1121 microstrain (1149 microstrain)

## **Torque Wrench Sensitivity** 
sensitivty in mV/V = 1.18 mV/V based on hand calculations and 1.15 based on FEM (half bridge)

## **Strain Guage Selected** 
SGD-3/350-LY13
![Torque Wrench Dimensions]({{ "/assets/images/sguage.jpg" | relative_url }}){: style="width: 500px;"}
[Link to Guage](https://www.dwyeromega.com/en-us/linear-strain-gages/SGD-LINEAR1-AXIS/p/SGD-3-350-LY13)







