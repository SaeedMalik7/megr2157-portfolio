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

The selected Material for the Bracket is the same as before, of ASTM A36 Steel.
<img width="1517" height="945" alt="image" src="https://github.com/user-attachments/assets/7f2d75f8-e808-4938-bf41-1ff358ac608f" />
<img width="1583" height="897" alt="image" src="https://github.com/user-attachments/assets/3e7f2dff-9ee8-4f3d-af90-f243206fb5b7" />
### Iteration I

#### Coarse
<img width="1583" height="915" alt="image" src="https://github.com/user-attachments/assets/768a22a4-9038-44e2-a26a-7ac30c5bad5d" />
<img width="1492" height="922" alt="image" src="https://github.com/user-attachments/assets/e1b5eaee-0950-45f6-b4d5-f064a6c36b5f" />
<img width="1542" height="935" alt="image" src="https://github.com/user-attachments/assets/753642a2-d6eb-4581-84ed-0c124863dc03" />
<img width="1505" height="922" alt="image" src="https://github.com/user-attachments/assets/67c32a12-8efd-4e84-aa1d-1acaff315499" />
<img width="1465" height="921" alt="image" src="https://github.com/user-attachments/assets/d9fa63ee-62e9-4b05-a024-e0f68bd0da7a" />
<img width="1507" height="932" alt="image" src="https://github.com/user-attachments/assets/afa8b5ce-ab23-446b-8a23-074c5faaf675" />
<img width="542" height="966" alt="image" src="https://github.com/user-attachments/assets/a1eb7beb-4a0a-48d0-8f81-6339540188a3" />

#### Medium Mesh
<img width="1485" height="937" alt="image" src="https://github.com/user-attachments/assets/04e0e408-f72a-48cd-84b6-1c9f7c9c3e0b" />
<img width="1525" height="936" alt="image" src="https://github.com/user-attachments/assets/344aa02a-581c-44e2-a905-6869e595b0da" />
<img width="1481" height="930" alt="image" src="https://github.com/user-attachments/assets/87ac2a0a-a707-46eb-9651-d3f7cfa06d73" />
<img width="1482" height="932" alt="image" src="https://github.com/user-attachments/assets/3cdfc2a2-0355-46e7-8821-c7e0009253b8" />
<img width="1507" height="931" alt="image" src="https://github.com/user-attachments/assets/1fb5240e-e916-4eac-b14c-8bb013bf3a34" />
<img width="1500" height="925" alt="image" src="https://github.com/user-attachments/assets/ed0143a7-fd6d-4cf2-9d3f-24b6d9fb912f" />

#### Fine Mesh
<img width="1517" height="922" alt="image" src="https://github.com/user-attachments/assets/552aacb2-c841-4647-b35b-151bae533b7b" />
<img width="1517" height="931" alt="image" src="https://github.com/user-attachments/assets/a255cb27-d907-4284-a25a-8181b8783e6d" />
<img width="1500" height="942" alt="image" src="https://github.com/user-attachments/assets/6ea45f4a-cf98-4eec-a30d-b613f4e7c236" />
<img width="1485" height="930" alt="image" src="https://github.com/user-attachments/assets/67093204-8ab2-45d5-be8d-404fd4a25138" />
<img width="1467" height="930" alt="image" src="https://github.com/user-attachments/assets/12e8fe2c-3e6d-4c51-a0ec-c6e2b61175cf" />
<img width="1492" height="926" alt="image" src="https://github.com/user-attachments/assets/cafc37cd-2fe8-4e1d-942c-3c076e4abf30" />

### Iteration II

#### Coarse Mesh
#### Medium Mesh
#### Fine Mesh

### Iteration III

#### Coarse Mesh
#### Medium Mesh
#### Fine Mesh

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
