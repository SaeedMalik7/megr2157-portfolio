# A5 – [Bracket Design]

## Objective
Detail design a bracket, using the concept design in Appendix B, to hold a horizontal force applied symmetrically by a strap outline in resource #1. The bracket’s dimensions are designed with different fit classes. Each dimension of the T beam is part of the fit:

- “a” intention for use where accuracy is not essential

- “b” is about the closest fits that can be expected to run freely

- “c” is where accurate location and minimum play is desired

Design using a safety factor of 4 and applied load in between 500 lbf < F < 800 lbf. Choose one of three metals, aluminum 6061 T6, Steel (ASTM A36), or Titanium (Ti-6Al-V4). Furthermore, state assumptions and approximations about the design in order to use fundamental strength of materials analysis. For example, use the proper stress analysis and deflection analysis where appropriate. Assume no failure due to direct shear stress. 

Note: If the bracket is designed symmetrically a lot of work would be cut.
<img width="821" height="376" alt="image" src="https://github.com/user-attachments/assets/598eb29e-b6d8-4c9a-96cc-75b7d9689cef" />
<img width="786" height="927" alt="image" src="https://github.com/user-attachments/assets/f6b676d9-9ca8-45b9-80d0-b8949e6f395f" />
<img width="832" height="947" alt="image" src="https://github.com/user-attachments/assets/36c67b50-4c0d-4d4f-9cb1-4ec5e9420ca2" />
<img width="800" height="646" alt="image" src="https://github.com/user-attachments/assets/1d4f5d9e-3b35-4a8d-8dd6-a9683deca7c7" />

## Analyze
<img width="727" height="401" alt="image" src="https://github.com/user-attachments/assets/d1433fb5-565a-4157-ac61-a1c72b9819bf" />

Before beginning on this project, I had to select my values from the given objectives. I chose to go with the highest force value of 800 lbf and I chose A36 steel as it is available in SolidWorks.

### Calculating Dimensions from Stress Analysis

First up was the stress analysis calculations for Features A-E. All the features required the known values, unknown values, assumptions, free body diagrams, nominal and algebraic solutions. The known values were mostly the same for all features, they included the force value, safety factor, yield strength and max deflection. The unknown was always the same as we were looking for dimension of the feature whether it was the height, length or width. The assumptions were mostly the same as well. The free body diagrams differed for all the features. 

<img width="723" height="512" alt="image" src="https://github.com/user-attachments/assets/0cce8757-8ae8-441c-b3cc-99de0cdabb1e" />
<img width="727" height="735" alt="image" src="https://github.com/user-attachments/assets/f824707c-9866-4e53-b51e-b21d71c2bc7b" />
<img width="672" height="737" alt="image" src="https://github.com/user-attachments/assets/4ff975af-3ed0-460a-bd73-08922a84b7e5" />
<img width="711" height="872" alt="image" src="https://github.com/user-attachments/assets/c171bd8d-0f6a-4d2e-bc64-2b9dde3d0df4" />
<img width="730" height="782" alt="image" src="https://github.com/user-attachments/assets/c76dc0e3-d33b-4f5e-8df9-5f7d1c63ee65" />
<img width="722" height="861" alt="image" src="https://github.com/user-attachments/assets/a0da56ab-3bd2-4cdc-bf65-00d38fa4feec" />

Below are the following feature value calculations: 

- Feature A 1.00in Length x 1.22in Diameter
- Feature B 0.146in thickness
- Feature C 0.468in height
- Feature D 0.663in thickness
- Feature E 0.936in thickness

Thickness and Height are interchangable values for most cases

### Calculating Dimensions from Stifness Analysis

For the stiffness analysis, the same known values, unknown values, assumptions, free body diagrams, nominal and algebraic solutions were required for all features. The known values were mostly the same for all features, they included the force value, safety factor, yield strength and max deflection. The unknown was always the same as we were looking for dimension of the minimum feature whether it was the height, length or width. The assumptions were mostly the same as well. The free body diagrams differed for all the features but were the same as the one used in the stress calculations. The point behind conducting the stiffness analysis was to find the max value between stiffness and stress to see which value the bracket would be governed by. All the minimum stiffness values were lower than the stress values, meaning the stress values governed the bracket. 

<img width="781" height="801" alt="image" src="https://github.com/user-attachments/assets/87c6ef70-6c00-4f59-b18b-ed472d80fa49" />
<img width="745" height="593" alt="image" src="https://github.com/user-attachments/assets/aedcca0e-d71d-44c8-9e68-43bf24035e81" />
<img width="777" height="668" alt="image" src="https://github.com/user-attachments/assets/ccb581de-5b4e-499c-918a-e9d2f70fa7bb" />
<img width="830" height="691" alt="image" src="https://github.com/user-attachments/assets/9c8b8640-8e26-4cea-9721-2f937521469a" />
<img width="853" height="901" alt="image" src="https://github.com/user-attachments/assets/a7bfbdcf-9129-46f6-a823-247d0ee39a63" />

Below are the following feature value calculations: 

- Feature A 1.00in Length x 0.523in Diameter
- Feature B 0.0091in thickness
- Feature C 0.131in height
- Feature D 0.263in thickness
- Feature E 0.356in thickness

Thickness and Height are interchangable values for most cases

## Decide
### Multiview Sketches
Below are two Multiview sketches using the calculated feature values.

<img width="881" height="837" alt="image" src="https://github.com/user-attachments/assets/c75d8077-9358-4e94-b3b0-1e20e9b29b38" />
<img width="832" height="705" alt="image" src="https://github.com/user-attachments/assets/e1e582ab-1c67-42b2-aec8-6a8cf61c300c" />

### CAD Model

The CAD Model for this assignment, will be available on the A6 assignment page.
## Communicate
### Lessons Learned

The governing failure mode for all five features was the stress values. All the stress values were higher for all features A-E, meaning that the strength requirement was more restive in this case. Feature E required 0.936in from the stress analysis while the stiffness only needed 0.356in. That is 0.580in difference and this was the case for all of the features. To my current knowledge no errors have occurred during this design process, a propagation method I used was when I carried the reaction force from Feature A into the axial load of Feature B. I checked the reactions using symmetry and equilibrium and at each feature before using the applied loads for the features, this helped prevent any errors. I assumed the length to be 1.00in. This plays a big role in the whole calculations for stress and stiffens, as this number is prevalent in both formulas for both features. I assumed the length as the length had to be greater than 3/4in and 1in was assumed, if the actual length is longer than the required cross sections would increase and if it is shorter they would decrease. I spent around 2 days working on this assignment. 

