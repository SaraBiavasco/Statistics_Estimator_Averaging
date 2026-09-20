# Estimator Averaging: Reproduction of Lavancier & Rochet (2015)

Statistics for Data Science project developed for the **M.Sc. in Data Science and Business Informatics** at the **University of Pisa**, A.Y. 2025/2026.

## Overview

This project reproduces selected experiments from the paper *“A General Procedure to Combine Estimators”* by Lavancier and Rochet (2015).

The paper studies how different estimators of the same parameter can be combined through weighted averaging, with the aim of obtaining an estimator that performs well compared with the individual estimators.

The project focuses on three applications presented in the paper:
- location estimation using the sample mean and median;
- parameter estimation for a Boolean model;
- quantile estimation under model misspecification.

## Project Structure

- `00_setup_theory.R` — common setup and implementation of the estimator averaging procedure.
- `01_section_4_1.R` — Section 4.1: location estimation combining sample mean and median.
- `03_section_4_3.R` — Section 4.3: parameter estimation for a Boolean model.
- `04_section_4_4.R` — Section 4.4: quantile estimation under model misspecification.

## Methods

The project implements the estimator averaging framework and applies it to three experiments from the paper:

- **Location estimation:** comparison of the sample mean, sample median and their averaged estimators across different symmetric distributions.
- **Boolean model estimation:** combination of different estimators for the parameters of a stationary Boolean model.
- **Quantile estimation:** combination of non-parametric and parametric estimators for the 0.99 quantile, including scenarios where the parametric models are misspecified.

Monte Carlo simulations and bootstrap procedures are used to evaluate and compare the estimators.

## How to Run

The analyses were developed in **R**.

The scripts should be run in the following order:

1. `00_setup_theory.R`
2. `01_section_4_1.R`
3. `03_section_4_3.R`
4. `04_section_4_4.R`

The three analysis scripts source `00_setup_theory.R`, which contains the common setup and estimator averaging functions.

## Reference

Lavancier, F., & Rochet, P. (2016). *A General Procedure to Combine Estimators*. Computational Statistics & Data Analysis, 94, 175–192.

## Authors

- Sara Biavasco
- Elena Fuschi
- Alice Giovagnini