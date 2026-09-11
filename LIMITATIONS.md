# Methodological Limitations

## Synthetic clinical metadata

The original multimodal notebook generates tabular variables (for example age, diabetes duration, HbA1c, blood pressure, and BMI) synthetically with random-number generators. These variables are not patient-linked observations from APTOS.

Consequences:

- the project can demonstrate software architecture and fusion mechanics;
- it cannot establish clinical utility of the metadata branch;
- performance differences must not be attributed to real clinical covariates;
- SHAP values for synthetic variables should be treated as demonstrations of the explanation pipeline rather than clinical associations.

## Dataset shift

APTOS and Messidor-2 differ in acquisition conditions and population/dataset characteristics. External validation is valuable but does not by itself establish deployment readiness.

## Clinical use

No part of this repository should be interpreted as a validated medical device or clinical decision-support system.

## Path to a stronger study

A rigorous follow-up should use real patient-linked structured covariates, predefined endpoints, leakage-safe patient-level splits, multi-seed evaluation, calibration analysis, subgroup analysis, and external validation with matched covariates.
