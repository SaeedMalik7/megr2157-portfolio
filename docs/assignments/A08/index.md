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

First up I wrote out the given values from the description. 

- Input torque	0.46875 in·lbf
- Input speed	2933.33 rpm
- Shaft diameter	0.125 in
- Shaft length	1 in
- Material	AISI 1018 cold-drawn steel

<img width="911" height="532" alt="image" src="https://github.com/user-attachments/assets/400e4a46-12a0-432f-b2bf-a008a25e5b4b" />
 
### Input Shaft Design

I started with the Input Shaft first, I wrote the knowns which were mostly from the description, the unknowns, assumptions and drew the Free body diagram. The unknowns were to solve for Torque in, Speed in and max output. 
<img width="811" height="567" alt="image" src="https://github.com/user-attachments/assets/46217b60-b98f-44c7-be33-64044d65ac52" />
<img width="793" height="891" alt="image" src="https://github.com/user-attachments/assets/ba4a0af6-38ce-44ec-99c7-f21cd17b996a" />

#### Final Calculations 

The given Input Shaft calculations are below. The given shaft size was sufficient. 

- Maximum shear stress	1,222 psi
- Factor of safety	21.69
- Shaft sufficient

### Output Shaft Design

Next up was the Output Shaft design, this followed the same layout. I wrote the unknowns, knowns, assumptions and drew the free body diagram.The unknowns were to solve for Torque in, Speed in and max output. 
<img width="751" height="922" alt="image" src="https://github.com/user-attachments/assets/96641422-e5a9-4499-86f0-db9391c52772" />
<img width="750" height="283" alt="image" src="https://github.com/user-attachments/assets/5a5d641d-fe56-4684-9c50-598a8211deaf" />

#### Final Calculations 

The given Output Shaft calculations are below. The given shaft size was sufficient, again. 

- Maximum shear stress	407.44 psi
- Factor of safety	65.04
- Shaft sufficient
  
### Journal Bearings Design

Next up was calculating the Journal Bearings, I broke it into two categories, of input and output. I wrote the given knowns for both and then for the assumptions and the unknowns of all the required Forces, pressure, velocity and PV values. I also drew the Free body diagram and solved the equations after. 
<img width="745" height="490" alt="image" src="https://github.com/user-attachments/assets/631456fc-4b1c-4d23-be47-76a1e4c3b5cf" />
<img width="770" height="892" alt="image" src="https://github.com/user-attachments/assets/a118d646-b747-422c-b499-ef4a1b5c6dd6" />
<img width="781" height="873" alt="image" src="https://github.com/user-attachments/assets/a4261411-72fb-4b28-8555-e1a61560eaf1" />
<img width="820" height="232" alt="image" src="https://github.com/user-attachments/assets/ef0c6479-1089-4142-8d21-81deac91c514" />

#### Calculations

I wrote the calculated values below for both the input and output bearings.

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

The material I chose was Porous Bronze after looking at Machinery's Handbook and comparing my values below. The Values of Porous Bronze mix well with what I require for these bearings. 

 Porous Bronze

- Max Load - 4,500 psi
- Max temperature - 160 F
- Max surface speed - 1500 fpm
- Max PV 50,000 psi-fpm

<img width="813" height="371" alt="image" src="https://github.com/user-attachments/assets/f5e4b629-6581-4a44-835c-72e53091cf68" />

### Journal Bearing Thickness

Lastly, I had to calculate the bearing thickness, which followed the same procedure as before of unknowns, knowns, free body diagrams and calculations. The calculated value was 0.257 in. 
<img width="817" height="403" alt="image" src="https://github.com/user-attachments/assets/14f33749-74d7-461e-8c99-aa8188e23526" />
<img width="848" height="947" alt="image" src="https://github.com/user-attachments/assets/b3a106b5-bf79-4e1e-9034-0bf03c0bd3bb" />

## Decide
### McMaster-Carr

These are SAE 841 Oil-impregnated sintered bronze which is almost ideal to Porous Bronze, as these were the only ones valuables for the size I needed. 

Input Bearing 
<img width="1261" height="920" alt="image" src="https://github.com/user-attachments/assets/e9efca09-9b41-4c13-b123-149965317f60" />
-<a href="./Input936T95.SLDPRT" download>Input Bearing</a>

Output Bearing
<img width="1242" height="916" alt="image" src="https://github.com/user-attachments/assets/84bdb359-3a1e-481b-9610-737a758cb449" />
-<a href="./Output936T13.SLDPRT" download>Output Bearing</a>

Below are the chosen Input and output shafts 

Input Shaft

<img width="1262" height="932" alt="image" src="https://github.com/user-attachments/assets/48a0b6c1-f42e-4fab-b946-81e94319c3ce" />

-<a href="./Inputshaft7880K19.SLDPRT" download>Input Shaft</a>

Output Shaft

<img width="1272" height="935" alt="image" src="https://github.com/user-attachments/assets/28661862-869e-4fe2-9731-db1cad4b4704" />

-<a href="./Outputshaft6832K45.SLDPRT" download>Output Shaft</a>

### Sketch

I drew a rough idea sketch of what I wanted to make in CAD, the inspiration for this came from an automotive differential housing shape, that is why it is a elliptical shape because the two gears are different sizes, hence a rounded shape is not needed. I added bolt holes on the edges so that it can hold the housing together. 
<img width="798" height="422" alt="image" src="https://github.com/user-attachments/assets/567db163-d692-496f-b117-8a2ebd57c34f" />

### CAD

First up are some of the equations I used, which were the housing size and bolt size.

<img width="1302" height="817" alt="image" src="https://github.com/user-attachments/assets/ccab160c-c4d6-4698-be2e-4e59d61e2764" />

Next up was drawing and extruding the base ellipse. 
<img width="1802" height="982" alt="image" src="https://github.com/user-attachments/assets/ca4ac794-e1bb-4153-bdc0-5a1859213ca6" />

Then I shelled it and I did not add a cover so that it is possible to see how the gears allign inside.
<img width="1802" height="957" alt="image" src="https://github.com/user-attachments/assets/9cf54889-0547-48ee-b397-a9a0ccb57216" />

Next up I drew a construction ellipse line, so that I could add the bolt holes. Unfortunatly I could not circular sketch pattern the bolts since it is an ellipse, so I had to do it individually. 
<img width="1467" height="942" alt="image" src="https://github.com/user-attachments/assets/695d7dff-d99f-42ae-857d-916ad9fb9fd3" />

Next up, I made a quick assembly of all the parts together without the housing cover so you can see what goes inside. The housing cover would just bolt to the front of the casing, enclosing the housing.
<img width="1342" height="885" alt="image" src="https://github.com/user-attachments/assets/5d1299c5-9be2-47c1-a13b-5197a9c74e43" />
<img width="1067" height="707" alt="image" src="https://github.com/user-attachments/assets/97bdde47-165c-429c-9de0-ec939933202d" />

-<a href="./A8 Gear.SLDPRT" download>Gear</a>

## Communicate
### Lessons Learned
This was a tough assignment, probably the most challenging one to date. It was challenging as I have never really done anything related to Gears before, especially on this level. The process of calculating the correct gear sizes along with force and torque values for the gears was a new experiment. Overall I learned a lot about Gears and bearings and how they can work mesh to work together. This assignment took me around 9 hours to complete. Most of the time was spent calculating the values. 
