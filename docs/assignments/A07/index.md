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

The selected Material for the Bracket is the same as before, of ASTM A36 Steel.

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
```

## Decide


## Communicate

