### General Information

This directory contains linear systems from AC optimal power flow problems (both stochastic and multiperiod problems).  The cases are divided into the synthetic network which was used when generating them.  The different networks correspond to different linear system sizes and output frequency.  A rough guide is
* RTS--small (less than 10^4 nonzeros), every iteration
* ACTIVSg200--moderate (on the order of 10^5 nonzeros), every 10 iterations
* ACTIVSg2000--moderate or large (on the order of 10^6 nonzeros), every 100 iterations

For more information about the RTS-GMLC network or to download it, see https://github.com/GridMod/RTS-GMLC

All ACTIVSg networks are from the TAMU Electric Grid Test Case Repository.  For more information or to download the networks, see https://electricgrids.engr.tamu.edu/

### Case Naming Convention

Case names generally follow the naming convention
```
<network name>_AC_s<number of stochastic scenarios>_p<number of time periods>
```
If the number of scenarios or time periods is 1, then the corresponding part of the case name is omitted.

### File and Formatting

Both matrices and right-hand sides are in [Matrix Market](https://math.nist.gov/MatrixMarket/formats.html) format.  All matrix files start with "matrix\_" and all right-hand side vectors start with "rhs\_".

The comment section in both give a unique ID number in order to match a given right-hand 
side with the corresponding matrix in the system.  Note there are more right-hand 
sides than matrices.

The matrix and right-hand sides from the last iteration of Ipopt (if available) are tagged with 'last' in the name.  For matrices, this is inplace of the number.  For right-hand sides, it precedes the number.


