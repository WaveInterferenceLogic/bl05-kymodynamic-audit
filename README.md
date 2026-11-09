# J-PARC BL05 Kymodynamic Velocity-Stratified Audit Pipeline

**Version:** 1.0.0  
**Author:** Justin L. Cameron (Wave Interference Logic)  
**DOI:** 10.5281/zenodo.10839391

## Overview
This repository contains the C++/ROOT calibration suite utilized in the *Physical Review Letters* submission regarding the Kymodynamic Stepped Slipstream Hypothesis. The pipeline mathematically evaluates the J-PARC BL05 ultracold neutron lifetime data, generating a full systematic covariance matrix ($\rho = 0.12$) to test flat velocity invariance ($H_0$) against the topological kink-soliton boundary limit ($H_1$).

## Prerequisites
* C++11 compiler or higher
* [CERN ROOT](https://root.cern/) (v6.00 or higher)
* CMake (v3.10 or higher)

## Execution via ROOT Macro (Fastest)
If ROOT is installed and sourced on your machine, you can execute the script directly without compiling:
```bash
root -l -q bl05_kymodynamic_audit.cpp