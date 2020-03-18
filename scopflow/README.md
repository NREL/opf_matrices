### General

This directory contains the matrices and right-hand sides generated from IPOPT on running the SCOPFLOW application. Each subdirectory represents a case run on a given netwok with some preset number contingencies. The directory name has the format <networkname_baseplus<n>ctgc where networkname is name of the network and n is the number of contingencies. Each subdirectory contains a matrix file (.mat) and a right-side vector file (.rhs). The matrix file has matrices from IPOPT iterations stored every 10th iteration (or rather every 10th time new_matrix flag is set). several matrices stored from the IPOPT iterations. More description on the matrix equations are given in Andreas Waechter's paper (see eq. 11 in his paper). The rhs file contains the corresponding right-hand side.

## To-do
Separate matrices in .mat file in separate files. Do the same with right-hand side files.