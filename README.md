# MS-Thesis-Dipole-Models-Full-Code

This repository contains the Python implementations developed for my Master's thesis on the numerical calculation of the **reduced deep inelastic scattering (DIS) cross section** in the small-$x$ regime using the dipole picture of QCD.

The objective of this project is to reproduce the reduced $\chi^2$ values reported by Tuomas Lappi and Heikki Mäntysaari in *Single inclusive particle production at high energy from HERA data to proton–nucleus collisions* (arXiv:1309.6963) by evaluating the same HERA reduced cross-section dataset with an independently developed numerical implementation.

## Repository Contents

- Numerical implementations of the **MV** and **MVe** dipole models.
- Backup versions of both models in `.txt` format.
- Appendix GBW model.
- An earlier implementation based on a precomputed Bessel function approach.
- Numerical routines for calculating:
  - the longitudinal structure function, $F_L$,
  - the proton structure function, $F_2$,
  - the reduced cross section, $\sigma_r$.
- Scripts used to generate the figures presented in the thesis.

## External Data

Both the MV and MVe implementations use tabulated dipole amplitudes generated with the **rcBK** evolution code:

- **rcBK evolved dipole amplitude for proton and lead**, commit `b1555ff`, by Heikki Mäntysaari.
- Repository: https://github.com/hejajama/rcbkdipole

## Requirements

The code was developed using Python 3 and requires the following packages:

- numpy
- scipy
- matplotlib
- numba
- joblib

These can be installed using

```bash
pip install numpy scipy matplotlib numba joblib
```

## Thesis

This repository accompanies my Master's thesis on the numerical calculation of deep inelastic scattering observables in the dipole picture at small Bjorken-$x$.

The implementation computes the longitudinal and transverse photon cross sections, evaluates the structure functions $F_L$ and $F_2$, and calculates the reduced cross section $\sigma_r$ for direct comparison with HERA measurements.

## References

T. Lappi and H. Mäntysaari,

*Single inclusive particle production at high energy from HERA data to proton–nucleus collisions*,

arXiv:1309.6963

https://arxiv.org/abs/1309.6963

H. Mäntysaari,

**rcBK evolved dipole amplitude for proton and lead**

https://github.com/hejajama/rcbkdipole

