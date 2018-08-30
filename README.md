Calculation of next-to-leading order simplified likelihood coefficients
-----------------------------------------------------------------------

SL backgrounds b_i for signal region i are parametrised as
```math
b_i = A_i + B_i*\theta_i + C_i/2 * \theta_i^2
```
where the $theta_i$ are distributed as a multivariate normal.

This reference code has been written with reverse engineering and
comprehensibility of the calculations explicitly in mind. While it computes
likelihood statistics on a reasonable timescale, further (but less readable)
optimisations can be added for production code.

This package includes functions to calculate the SL $a_I$, $b_I$, $c_I$, and
$\rho_{IJ}$ coefficients from provided moments $m_{1,I}$, $m_{2,IJ}$ and
$m_{3,I}$; and an `SLParams` class which computes these and higher-level
statistics such as profile likelihoods, log likelihood-ratios, and related
limit-setting measures computed using observed and expected signal yields.
