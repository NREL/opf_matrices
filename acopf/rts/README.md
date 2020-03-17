### General

Linear systems in these directories are from ACOPF problems (NOT security constrained)
on the [RTS-GMLC] (https://github.com/GridMod/RTS-GMLC) (abbreviated as RTS) from the IPOPT solver.
There are two different ACOPF problems: one with a single period and the other with two time periods.
The objective function is linear in both problems.  Both directories include matrices (all named like
"matrix\_") and right-hand sides (all named like "rhs\_") an entire run of IPOPT for
the problem (that is, every linear solve that is performed by Ipopt to solve the
optimization problem).  The number in the file name gives the sequence the matrices
(right-hand sides) occurred in.  The larger the number, the later in the IPOPT
run they occurred.

### Formatting Info

Both matrices and right-hand sides are in [Matrix Market](https://math.nist.gov/MatrixMarket/formats.html) format.
The comment section in both give a unique ID number in order to match a given right-hand 
side with the corresponding matrix in the system.  Note there are more right-hand 
sides than matrices.
