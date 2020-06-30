These linear systems are generated from AC (stochastic and/or multiperiod) Economic Dispatch problems for the [ACTIVSg10k](https://electricgrids.engr.tamu.edu/electric-grid-test-cases/activsg10k/) (also called TAMU10k) network.

Linear system size can be estimated in the following way:
```
DIMENSION ~ 238000 * s * p
NONZEROS ~ 724000 * s * p
```
where `s` is the number of scenarios and `p` is the number of time periods.  Note that `s` and `p` are given directly in the case names by the number following the letter.  If not present in the case name, then the number is 1.
