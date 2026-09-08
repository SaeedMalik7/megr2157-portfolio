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
A circular pin hole is placed in the left side of the bar. After using the Peterson Stress Concentration Chart for a circular hole located in a flat tension bar, it gives an approximate hole to bar width ratio of d/W = 0.5 with a stress concentration of K =2.16 approximately. The nominal FEA stress was 2.233 ksi away from the hole. So the estimated peak stress at the hole would be (K)(StressMax) = (2.16)(2.233)= 4.82ksi. Using the given Aluminum yield strength of 40ksi, the safety factor would be 40/4.82= 8.30. In conclusion, even with a pin hole, the bar will still pass the strength requirement.  

### Lessons Learned 
I learned how do conduct an FEW simulation on CAD, I have never done one before. I had used an excel in past situations for Beam design but never a CAD simulation. So that whole process was new to me and I enjoyed it, as I learned how to do something new with CAD. It's always good when you can find out more features on a program that you like. I spent roughly around four and a half hours on this assignment, majority of the time came from writing on my website, as I was just going blank on how I wanted to describ my process. 
### CAD Link
-<a href="./Beam.SLDPRT" download>Truss Beam</a>


