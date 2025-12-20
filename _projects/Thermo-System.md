---
layout: project
title: Thermodynamic Analysis 
description: Fridge system
technologies: [Thermodynamic Tables]
image: /assets/images/2210_cover.jpg
---


I decided to analyze the kitchen refrigerator at my house. The image I have included shows the compressor, an integral part of a functioning fridge and a part that has been replaced since the old one broke a few years ago. I began with looking up the exact details of the compressor in order to determine some of its operating conditions. 

![compressor]({{ "/assets/images/2210_com2.jpg" | relative_url }}){: style="width: 550px;"}



## **Compessor: Matsushita DC51C72RBU6**
- Evaporating Temperature: -23.3C
- Condensing Temperature: 54.4C
- Motor Input: 108W
- [Link to Compressor Specs](https://powertool.manualsonline.com/manuals/mfg/panasonic/dc51c72rcu6.html)

I was then able to determine both the isentropic efficiency and the mass flow of R-134a while making some key assumptions. Firstly, I assumed that the compressor control volume is adiabatic as there is no heat exchange with the environment. This is valid as the label on the part states "thermally protected". I used the temperatures listed above as well as the thermodynamic tables for R-134a in order to obtain the enthalpies in and out. To find the isentropic enthalpy out, I assumed the enthalpy in and out was the same. Using this, I was able to determine an approximate isentropic enthalpy to be 0.807. The calculations are certainly not precise as they would require interpolation between thermodynamic table data values, but serve as an approximation that is within the range for standard home fridges.

![Calculations]({{ "/assets/images/2210_math.jpg" | relative_url }}){: style="width: 500px;"}

Calculating the mass flow was more straightforward and yielded a mass flow of 0.00178 kg/s. This was based on the first law of thermodynamics and the adiabatic assumption. The enthalpy values used were the non-isentropic values obtained from the thermodynamic tables previosuly discussed. The mass flow is also within range for standard fridges but on the lower end. 


## **Future Considerations**

![heat]({{ "/assets/images/2210_heat-ex.jpg" | relative_url }}){: style="width: 450px;"}

I have also included an image of the heat exchanger that is connected to the compressor on the exterior of the fridge. A good next step would be to calculate the heat trasfer with the surroundings and calculate the overall effiency of the fridge. 
