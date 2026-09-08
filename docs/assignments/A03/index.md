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
- F is the applied Force
- A
- 
<img src="./Equations.png" alt="" width="800">
<img src="./Step 1.png" alt="" width="800">
<img src="./bar.png" alt="" width="800">

<img src="./Custom Material.png" alt="" width="800">


## Decide
<img src="./Bar Load.png" alt="" width="800">
<img src="./Deflection Map.png" alt="" width="800">
<img src="./Von Misses.png" alt="" width="800">


## Communicate

