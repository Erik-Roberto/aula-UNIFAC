# UNIFAC Implementation in Python
Created by: Eng. Erik Souza

Supervised by: Prof. Dr. Marcos Rogério Mafra

This repository contains a Python implementation of the UNIFAC (UNIversal Functional Activity Coefficient) method developed as supporting material for the Teaching Internship Course of the Master's Program in Chemical Engineering at the Federal University of Paraná (UFPR).

The material was prepared for the course Applied Thermodynamics to Chemical Engineering II (ENQ 052), offered in June 2026.

The notebook presents the complete implementation of the model from first principles, including the combinatorial and residual contributions, together with validation examples based on literature data.

## Objectives

- Introduce the fundamentals of the UNIFAC method.
- Demonstrate how activity coefficients can be estimated from molecular structure.
- Provide a transparent implementation of the model.
- Compare model predictions against experimental data.

## Contents

The notebook includes:

1. Definition of molecular structures using UNIFAC groups.
2. Assembly of interaction and group matrices.
3. Calculation of the combinatorial contribution.
4. Calculation of the residual contribution.
5. Calculation of activity coefficients.
6. Validation against literature data.

## Repository Structure
.\
├── experimental_data/\
│   ├── acetone_n-pentane.json\
│   └── ethanol_2-butanone-isooctane.json\
│\
├── parameters/\
│   ├── structural.csv\
│   └── interaction.csv\
│\
├── unifac.ipynb\
└── README.md

### experimental_data

Contains experimental activity coefficient data collected from the literature and used for model validation.

### parameters

Contains the UNIFAC parameter tables used by the implementation:

- Structural parameters (Rk and Qk)
- Group interaction parameters (amn)

### unifac.ipynb

Main notebook containing the complete implementation, examples, and validation cases.

## Requirements

The notebook was developed using Python 3 and requires the following packages:

- numpy
- pandas
- matplotlib

They can be installed with: **pip install numpy pandas matplotlib**

## Scope and Limitations

This implementation was developed for educational purposes and focuses on the original UNIFAC formulation.

Current limitations include:

- Classical UNIFAC only.
- No modified UNIFAC (Dortmund) implementation.
- No parameter regression routines.
- No phase equilibrium calculations.
- Parameter database restricted to the groups included in the supplied tables.

## References
Poling, B. E., Prausnitz, J. M., & O'Connell, J. P. The Properties of Gases and Liquids, 5th Edition.

Sandler, S. I. — Chemical and Engineering Thermodynamics (3rd ed., 1999)

Wen, C.-C., & Tu, C.-H. (2007). Vapor–liquid equilibria for binary and ternary mixtures of ethanol, 2-butanone, and 2,2,4-trimethylpentane at 101.3 kPa. Fluid Phase Equilibria, 258(2), 131–139. https://doi.org/10.1016/j.fluid.2007.06.005

Campbell, S. W., Wilsak, R. A., & Thodos, G. (1986). Isothermal vapor-liquid equilibrium measurements for the n-pentane–acetone system at 372.7, 397.7, and 422.6 K. Journal of Chemical & Engineering Data, 31(4), 424–430. https://doi.org/10.1021/je00046a016