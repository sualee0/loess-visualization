# LOESS Regression — Parameter Analysis & Visualization
## Overview
Final project for DATA 440 (Computational Methods for Data, Spring 2026). A from-scratch implementation of LOESS in Julia, exploring how parameter choices affect model fit through visual scenarios.

## What is LOESS?
LOESS fits a smooth curve by performing weighted least squares regression locally at every point, using only nearby data within a sliding window. The result is a non-parametric smoother that adapts to local data structure.

## Implementation
For each evaluation point c, the algorithm: isolates the local window → applies a weight function → builds the design matrix for 1st or 2nd order fit → solves weighted least squares → records the fitted value at c.

## Scenarios Explored
- 1st vs. 2nd order polynomial fits
- Cubic vs. uniform weight functions
- Window width: small (overfitting) vs. large (underfitting)
- Edge effects at data boundaries

## Tools
- Julia (implementation)
- ImageTank (visualization + implementation)
