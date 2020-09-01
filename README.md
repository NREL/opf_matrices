### Overview

Matrices and Right-Hand Sides (RHSs) were printed from NLP Solver [Ipopt](https://github.com/coin-or/Ipopt).
They give the linear problem as detailed by equation (11) of 
[(Watcher and Biegler 2005)](https://link.springer.com/article/10.1007%2Fs10107-004-0559-y).
A brief outline of how this was done can be found in the `HOW_TO_GUIDE.md` in the
`Ipopt` directory.

The test systems are broken into two directories.  The `acopf` directory contains 
AC optimal power flow problems (both stochastic and multiperiod) while the `scopflow` 
directory contains security constrained AC optimal power flow problems.  Additional 
details can be found in the READMEs in those directories as well as the individual 
case directories.

Note: The repository is quite large and uses Git LFS. If you plan to clone the repository, you will need to
install it.

### Matching Right-Hand Side with a Matrix

Both right-hand sides and matrices are in [Matrix Market format](https://math.nist.gov/MatrixMarket/formats.html).
The header section in both the right-hand side and matrix files contains a unique
ID number.  In order to match a specific right-hand side vector with its corresponding 
matrix, simply match the two IDs.  For example, say the right-hand side file
has the header
```
%%MatrixMarket matrix array real general
% ID: 70
```
Then the corresponding matrix should have the header
```
%%MatrixMarket matrix coordinate real symmetric
% ID: 70
```
so the ID field in both files match.

### Authors

This repository was created by Shrirang Abhyankar of PNNL and Jonathan Maack of NREL.
