# A7 – [FEA on Bracket]

## Objective

- Use Finite Element Analysis (FEA) to improve the bracket design from previous assignments.
- Ensure high stiffness, strength, and lightweight optimization through iterative design.
- Conduct multiple FEA simulations, refining geometry based on results.
- Perform static stress analysis, including constraints, loading, and meshing selection.
- Interpret data by identifying max stress, displacement, and safety factors.
- Optimize the design by modifying geometry to enhance performance.
- Document the entire process with images, calculations, and insights.
- Reflect on key engineering lessons learned and time spent.

Description:
Your task is simply to create a high stiff, high strength, and lightweight component. Use Finite Element analysis to drive your decision making process throughout your design. Each step of the analysis and before you make geometric changes make sure the component’s results (stress/displacement/Safety Factor) converge on a 7% difference. Achieve this by modifying the number of elements. If after three attempts to converge use the stiffness and stress from the finer mesh size use the finest mesh size and proceed through the process.
<img width="798" height="727" alt="image" src="https://github.com/user-attachments/assets/8b0d9610-1e7a-4794-a85d-86467a9a5c23" />

## Analyze
### Setup

Before I could begin with the simulations, I had to set up the bracket. I added a fixed load on the insides of the bracket on top and on bottom as viewed. I also added a force value of 2F, to the cylindrical part of the bracket. The 2F value was taken from the given description of the bracket. The material was kept the same as before, of ASTM A36 Steel. The material, fixed load and force values were repeated for all Iterations and all Mesh types.

<img width="1517" height="945" alt="image" src="https://github.com/user-attachments/assets/7f2d75f8-e808-4938-bf41-1ff358ac608f" />
<img width="1583" height="897" alt="image" src="https://github.com/user-attachments/assets/3e7f2dff-9ee8-4f3d-af90-f243206fb5b7" />

### Iteration I

First up I used the original bracket design and conducted a stress, deflection, safety factor analysis. The mesh values went from Coarse to medium to Fine mesh for all three iterations. 

#### Coarse Mesh

<img width="1583" height="915" alt="image" src="https://github.com/user-attachments/assets/768a22a4-9038-44e2-a26a-7ac30c5bad5d" />
First up is the original bracket design with a coarse mesh including 1192 total elements. 
<img width="1492" height="922" alt="image" src="https://github.com/user-attachments/assets/e1b5eaee-0950-45f6-b4d5-f064a6c36b5f" />
<img width="1542" height="935" alt="image" src="https://github.com/user-attachments/assets/753642a2-d6eb-4581-84ed-0c124863dc03" />
The two pictures above are the stress pictures from an isometric and right side view. The Max stress occurs at point right below the connection in Part B, the value is 4557 Nm^2.

<img width="1505" height="922" alt="image" src="https://github.com/user-attachments/assets/67c32a12-8efd-4e84-aa1d-1acaff315499" />
<img width="1465" height="921" alt="image" src="https://github.com/user-attachments/assets/d9fa63ee-62e9-4b05-a024-e0f68bd0da7a" />
The two pictures above are the max deflection pictures after conducting the analysis. The Max deflection occurs at the bottom of the circle which is part A, the value is 0.000001539 mm.

<img width="1507" height="932" alt="image" src="https://github.com/user-attachments/assets/afa8b5ce-ab23-446b-8a23-074c5faaf675" />

This is a safety factor test and it shows a max value of 5.5e+04, which would fail as the requirement for this design was to be of 4. It will fail due to a lack of enough requried matrial.

<img width="542" height="966" alt="image" src="https://github.com/user-attachments/assets/a1eb7beb-4a0a-48d0-8f81-6339540188a3" />

The mass of the original iteration is 1.86 pounds. 

#### Medium Mesh
Next up was a medium mesh analysis. 
<img width="1485" height="937" alt="image" src="https://github.com/user-attachments/assets/04e0e408-f72a-48cd-84b6-1c9f7c9c3e0b" />
<img width="1525" height="936" alt="image" src="https://github.com/user-attachments/assets/344aa02a-581c-44e2-a905-6869e595b0da" />
<img width="1481" height="930" alt="image" src="https://github.com/user-attachments/assets/87ac2a0a-a707-46eb-9651-d3f7cfa06d73" />

The two pictures right above are the pictures right after a stress analysis was conducted. The max stress value was 4871 N/mm^2 and it occurred at the same location as in the coarse mesh.
<img width="1482" height="932" alt="image" src="https://github.com/user-attachments/assets/3cdfc2a2-0355-46e7-8821-c7e0009253b8" />
<img width="1507" height="931" alt="image" src="https://github.com/user-attachments/assets/1fb5240e-e916-4eac-b14c-8bb013bf3a34" />

The two pictures above are the max deflection pictures after conducting the analysis. The Max deflection occurs at the bottom of the circle which is part A, the value is 0.000001527 mm.

<img width="1500" height="925" alt="image" src="https://github.com/user-attachments/assets/ed0143a7-fd6d-4cf2-9d3f-24b6d9fb912f" />

The safety factor did not change at all, it is the same value of 5.5e+04, and it still fails as it is not enough.

#### Fine Mesh

Lastly the analysis with a Fine Mesh was conducted for stress, deflection and safety factor. 
<img width="1517" height="922" alt="image" src="https://github.com/user-attachments/assets/552aacb2-c841-4647-b35b-151bae533b7b" />
<img width="1517" height="931" alt="image" src="https://github.com/user-attachments/assets/a255cb27-d907-4284-a25a-8181b8783e6d" />
<img width="1500" height="942" alt="image" src="https://github.com/user-attachments/assets/6ea45f4a-cf98-4eec-a30d-b613f4e7c236" />

The two pictures right above are pictures of a stress analysis, the max stress is almost gone and it it just at the connecting point of B to C. The max stress is 6364 Nm^2.

<img width="1485" height="930" alt="image" src="https://github.com/user-attachments/assets/67093204-8ab2-45d5-be8d-404fd4a25138" />
<img width="1467" height="930" alt="image" src="https://github.com/user-attachments/assets/12e8fe2c-3e6d-4c51-a0ec-c6e2b61175cf" />

The two pictures above are deflection analysis, the max location has not changed and is still at the bottom of the circle on the back side. The max value is 0.000001485 mm.
<img width="1492" height="926" alt="image" src="https://github.com/user-attachments/assets/cafc37cd-2fe8-4e1d-942c-3c076e4abf30" />

The safety factor decreased to a value of 3.9e+04 all around the bracket. This value is in line with the requirement of 4. 

Below is the link for the CAD Model.
-<a href="./A6 Bracket.SLDPRT" download>Bracket</a>

### Iteration II

<img width="1337" height="937" alt="image" src="https://github.com/user-attachments/assets/b250a8cd-ab6b-4bab-a9e2-b23410af076b" />

For the second iteration, I made part B thicker, I doubled the thickness value which was set when the bracket was made. Then I clicked rebuilt and re did all of the analysis. 

#### Coarse Mesh

<img width="1790" height="980" alt="image" src="https://github.com/user-attachments/assets/009bfd30-0ca8-4932-82ef-8d3562de7e1d" />
A coarse mesh was applied to the part with 1192 elements
<img width="1465" height="932" alt="image" src="https://github.com/user-attachments/assets/151f8bac-d4fa-4cea-a73d-a1e018eca93c" />
<img width="1462" height="936" alt="image" src="https://github.com/user-attachments/assets/10e27a3e-401e-42d2-8d39-7ad491f5372d" />
<img width="1465" height="937" alt="image" src="https://github.com/user-attachments/assets/425837ae-ef3f-45c7-a03e-cd48599698e6" />
<img width="1472" height="941" alt="image" src="https://github.com/user-attachments/assets/a263a22d-8f21-4bcd-968b-f85da66ee05b" />
<img width="1465" height="935" alt="image" src="https://github.com/user-attachments/assets/2db0556c-af82-43ea-bb38-a94811a10ec3" />

#### Medium Mesh

<img width="1448" height="928" alt="image" src="https://github.com/user-attachments/assets/419cbf12-dd78-42dd-bc3a-df626b1cdf27" />
<img width="1467" height="937" alt="image" src="https://github.com/user-attachments/assets/fa977eda-c27c-4933-aa3a-e4f17d1d5648" />
<img width="1466" height="937" alt="image" src="https://github.com/user-attachments/assets/44f300db-0b34-48a1-ad58-792242cbf0bc" />
<img width="1462" height="940" alt="image" src="https://github.com/user-attachments/assets/d45e883f-4b41-417f-b2bd-7bf6a4242835" />
<img width="1465" height="937" alt="image" src="https://github.com/user-attachments/assets/147b4d5e-4c1a-4493-9954-6e78ffabff33" />
<img width="1457" height="940" alt="image" src="https://github.com/user-attachments/assets/40d3830e-b047-4ef7-8b58-ff1f3faa68e4" />

#### Fine Mesh

<img width="1462" height="933" alt="image" src="https://github.com/user-attachments/assets/7c840981-e5e1-4e68-8e1a-1aedce02af51" />
<img width="1461" height="940" alt="image" src="https://github.com/user-attachments/assets/47e5a4c4-1d39-449b-8d6a-d3df10bf4092" />
<img width="1472" height="937" alt="image" src="https://github.com/user-attachments/assets/d867afbd-f6d6-4c8b-b284-ae21f56caed6" />
<img width="1471" height="935" alt="image" src="https://github.com/user-attachments/assets/a06d28d6-65ce-4007-adf3-7ac83833fc08" />
<img width="1456" height="937" alt="image" src="https://github.com/user-attachments/assets/2bd489ae-2250-4dc4-a6a0-5fdb3d3f6ae5" />
<img width="1462" height="932" alt="image" src="https://github.com/user-attachments/assets/ef1f04d7-086f-469a-b318-d64ed12cfe3c" />

### Iteration III

<img width="1826" height="1017" alt="image" src="https://github.com/user-attachments/assets/906e59c8-1573-4121-b15d-e85cea1a70a1" />
<img width="1752" height="937" alt="image" src="https://github.com/user-attachments/assets/f2c9cd9f-c72b-42e0-b830-6b5bfbd5c9de" />

#### Coarse Mesh

<img width="1797" height="1000" alt="image" src="https://github.com/user-attachments/assets/0a301b2e-ce7a-463b-85a9-99346dd6ac5e" />
<img width="1472" height="947" alt="image" src="https://github.com/user-attachments/assets/a6b68bf4-07d1-4a12-a28e-cf0489533354" />
<img width="1460" height="940" alt="image" src="https://github.com/user-attachments/assets/f3be309b-2987-43e6-976a-9d1358abd97d" />
<img width="1457" height="940" alt="image" src="https://github.com/user-attachments/assets/ead6c58c-d804-4610-86a0-d01ad6a8810d" />
<img width="1462" height="937" alt="image" src="https://github.com/user-attachments/assets/34e293d1-2038-4851-a665-7806c2c222f8" />
<img width="1467" height="936" alt="image" src="https://github.com/user-attachments/assets/1f556851-866e-4c91-8ccb-3a9df9c2df69" />

#### Medium Mesh

<img width="1451" height="922" alt="image" src="https://github.com/user-attachments/assets/ceddcade-14ec-4306-86a9-548db3e23e37" />
<img width="1466" height="937" alt="image" src="https://github.com/user-attachments/assets/e9988929-fe86-4bd5-826f-fd04fd70b543" />
<img width="1456" height="937" alt="image" src="https://github.com/user-attachments/assets/eccdc7d3-8c28-4ed2-840a-273d658c63c7" />
<img width="1462" height="936" alt="image" src="https://github.com/user-attachments/assets/7a8ca134-82cd-46ec-a940-b1ff2d900016" />

#### Fine Mesh

<img width="1465" height="941" alt="image" src="https://github.com/user-attachments/assets/a59f45f0-ca44-4040-93a4-40c6c95903a9" />
<img width="1452" height="937" alt="image" src="https://github.com/user-attachments/assets/f05bcfd6-433d-40e6-8816-4ce314f02451" />
<img width="1452" height="935" alt="image" src="https://github.com/user-attachments/assets/7aca54d5-9d79-4dd7-9020-3eb12601ad5f" />
<img width="1462" height="940" alt="image" src="https://github.com/user-attachments/assets/969a3634-2226-4464-8c4b-1dedadf503c6" />

## Decide
### Data Table 
<table style="width: 100%; border-collapse: collapse; border: 1px solid black; font-family: 'Times New Roman', serif; font-size: 18px; color: black;">
    <thead>
        <tr style="height: 38px;">
            <th style="width: 26.5%; border: 1px solid black; padding: 6px 8px;"></th>
            <th style="width: 23.5%; border: 1px solid black; padding: 6px 8px; text-align: left;">Design 1</th>
            <th style="width: 25%; border: 1px solid black; padding: 6px 8px; text-align: left;">Design II</th>
            <th style="width: 25%; border: 1px solid black; padding: 6px 8px; text-align: left;">Design III</th>
        </tr>
    </thead>
    <tbody>
        <tr style="height: 37px;">
            <th style="border: 1px solid black; padding: 6px 8px; text-align: left;">Max Stress and location</th>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
        </tr>
        <tr style="height: 57px;">
            <th style="border: 1px solid black; padding: 6px 8px; text-align: left;">Max deflection and<br>location</th>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
        </tr>
        <tr style="height: 38px;">
            <th style="border: 1px solid black; padding: 6px 8px; text-align: left;">mass</th>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
        </tr>
        <tr style="height: 37px;">
            <th style="border: 1px solid black; padding: 6px 8px; text-align: left;">Safety Factor</th>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
        </tr>
        <tr style="height: 38px;">
            <th style="border: 1px solid black; padding: 6px 8px; text-align: left;">Number of elements</th>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
            <td style="border: 1px solid black; padding: 6px 8px;"></td>
        </tr>
    </tbody>
</table>

## Communicate
### Reflections 
