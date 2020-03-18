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
