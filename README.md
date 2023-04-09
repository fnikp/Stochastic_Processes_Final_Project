# Stochastic Equations Analysis

This project was completed as a final project for the course "Stochastic Processes" instructed by Prof. M. Reza Rahimi Tabar at Sharif University of Technology during the spring semester of 2022.

## Overview

The goal of this project was to analyze a system of stochastic equations:

$$\dot{x_1}(t) = 4 x_1(t) - x_1^3(t) + g \times \Gamma_1(t)$$

$$\dot{x_2}(t) = -x_1(t)x_2(t) + g \times \Gamma_2(t)$$

Here, $\Gamma_i$ is white noise. The equations were integrated for different strengths of noise ($g$), and the correlation between $x_1$ and $x_2$ was investigated by creating scatter plots of $x_1$ vs. $x_2$.

Additionally, an ensemble of size $10$ was created by integrating these equations. The binning method was used to group the time-series into an $11 \times 11$ grid space. The values of the components of the drift vector and the diffusion matrix were then calculated in each bin from the data. The theoretical values of these components were plotted as a surface, and the data-driven values were plotted as scattered points in 3D plots.

The jitcsde package was used for stochastic integrals in this project.

## Notebooks

The following notebooks were included in this project:

Correlation: This file contains code to plot the correlation between $x_1$ and $x_2$.
Phase_portrait: This file contains code to plot the phase portrait of the deterministic part of the system.
Kramers_Moyal_Coeffs: This file contains code to calculate and plot the components of the drift vector and the diffusion matrix.

## Required Packages

The following packages were used in this project:

* jitcsde
* numpy
* matplotlib
* seaborn

## License

This project is licensed under the MIT License - see the LICENSE file for details.

