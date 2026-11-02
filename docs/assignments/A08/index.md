# A8 – Gears

## Objective
- Design a gearbox that can be assembled and disassembled.
- Analyze and size input and output shafts for strength.
- Design journal bearings to support shafts.
- Create a gearbox housing with proper clearance and fastening.
- Use parametric CAD modeling to generate a final design.
- Document calculations, sketches, and lessons learned.

Description:
Design a gearbox which can be assembled and disassembled. The spur gears have a gear ratio of 24:9 and are listed in the resource section. The output gear torque and speed are to be 1.25 in-lbf and 1100 rpm relative. The input (pinion,power-transmission) and output (gear, short shaft) shaft diameters are .125 and .25 inches respectively and each have a length of 1 inch. Use the appropriate equations in the Machinery’s Handbook for empirical units. The critical features of the gearbox include the shafts, and the journal bearings.

Assumptions: 

Assume appropriate strength of shafts, use Machinery’s Handbook.
The gear train is ideal.
The moment of the radial force from the gear train is small enough to be ignored.
Note:

The shafts are press fit through the hubs of the gears.
Make sure there is enough clearance between the gears and the gearbox.
Use a running sliding fit for the size of the hole for the shafts.
<img width="902" height="681" alt="image" src="https://github.com/user-attachments/assets/d6c6c735-fdff-44dc-94db-a71aed446128" />

## Analyze

- Input torque	0.46875 in·lbf
- Input speed	2933.33 rpm
- Shaft diameter	0.125 in
- Shaft length	1 in
- Material	AISI 1018 cold-drawn steel
  
### Input Shaft Design
#### Final Calculations 

- Maximum shear stress	1,222 psi
- Factor of safety	21.69
- Shaft sufficient

### Output Shaft Design
#### Final Calculations 

- Maximum shear stress	407.44 psi
- Factor of safety	65.04
- Shaft sufficient
  
### Journal Bearings Design
#### Calculations

Input Bearing Summary
  0.1250 in x 0.1250 in

- Bearing Pressure  170.30 psi
- Surface Velocity  96 fpm
- PV 16,349 psi fpm

Output Bearing Summary
 0.250 in x 0.250 in
 
- Bearing Pressure  42.58 psi
- Surface Velocity  72 fpm
-  PV 3066 psi fpm

#### Material
 Porous Bronze

- Max Load - 4,500 psi
- Max temperature - 160 F
- Max surface speed - 1500 fpm
- Max PV 50,000 psi-fpm


### Journal Bearing Thickness
## Decide
### Sketch
### CAD

## Communicate
### Lessons Learned
