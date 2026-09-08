# A3 – [Parametric and FEA]

## Objective

- Use axial deflection modeling to design its dimensions
- Use parametric design to determine a bars length
- Introduce you to FEA (Finite Element Analysis)
- Introduce you to linking dimensions to appropriate parameters in CAD.
- Compare and contrast the different analysis

### Description:
To design a bar which has a circular cross section where the values of the criteria given for the material, maximum deflection, and load. Determine the bar’s minimum geometry (ie.. length, diameter, and weight) through parametric design while under direct tension. Then verify the geometry through finite element analysis.
<img src="./Bar Requirements.png" alt="" width="800">
## Analyze
### Parametric Design

The first step in designing a bar was to pick between the direct applied loads of 300 lbf < F < 500 lbf. The other given choice was to pick between 8.5 to 11.5 x10^6 psi for the Youngs Modulus for our Aluminum Bar. Below are the chose values for this specific bar along with some given values. After selecting the values, area and length calculations were done using direct tension elongation equations found in the Machinery's Handbook so that I could parametrically determine the length of the bar. The Area came out to be 0.19635 in^2 and the length was 44.18 in. 

<img src="./image 1.png" alt="" width="800">

Next up these values were entered in the variable section of the CAD Model. 
- F is the chose applied Force value
- E is the chosen Young's Modulus value

<img src="./Equations.png" alt="" width="800">

After inputting all the necessary values, I began to Generate the bar in CAD by using my variables and Parameters. First up was to draw a circle and assign it the diameter. 

<img src="./Step 1.png" alt="" width="800">

After drawing the circle, I extruded it to the given length variable. 

<img src="./bar.png" alt="" width="800">

Before I could progress any further and do the FEA analysis, I needed to add the Aluminum material to my bar. There were a lot of Aluminum options to pick from but none had the right parameters for the Youngs Modulus, so I created my own Aluminum. I copied the values of the one Aluminum with a very close Young's Modulus value and then edited the value in my Custom Materials to be the required 10,000,000psi.

<img src="./Custom Material.png" alt="" width="800">

## Decide
### FEA
Before I could conduct an FEA, I had to correctly apply the fixed load to one end of the bar and a pulling force of 400 N to the other end of the bar. 

<img src="./Bar Load.png" alt="" width="800">

#### Deflection Map
<img src="./Deflection Map.png" alt="" width="800">

After conducting the Deflection Map, you can see that my Max Deflection came out to 0.009016 in which is slightly above the calculated value of 0.009 in. 

#### von Misses Stress Map
<img src="./Von Misses.png" alt="" width="800">
After conducting the von Misses Stress, the stress came out to be 2.233 ksi. 

#### Max Stress Check 
<img src="./image 2.png" alt="" width="800">
I did a quick calculation to confirm that the max calculated stress was lower than the Aluminum stress Sy=40 and the safety factor came out at 19.6 

## Communicate
### Design Reflection
<img src="./image 3.png" alt="" width="800">

The calculated deflection value was 0.009in and the FEA deflection value was 0.009016in. The percent difference comes out to 0.178%. This is a very minimal percent difference and this amount can be totally avoided by going with a slightly smaller bar to ensure that the stress stays under the max deflection amount. In all this minimal difference does not cause any concern. This minimal percent difference shows the harmony or almost harmony between the analytical and FEA stress results. The analytical equation describes a bar under uniform axial tension while the FEA accounts for actual constraints and numerical models. Both results in this case are consistent but the FEA provides a more detailed representation. I would personally go with the FEA results as it takes more data and constraints into consideration hence giving a more precise answer. I also included a percent difference for the stress calculation, along with a new safety factor calculation. The stress difference came out to 9.62% and the safety factor was 17.91. The bar still remains way below the yield strength and satisfies the strength requirements.

#### Pin Hole

### Lessons Learned 

### CAD Link


