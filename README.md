#WARNING: Use [Florian Schwendinger's](https://github.com/FlorianSchwendinger/scs) package instead. This package is deprecated.


OLD README:

# scs-r
R interface for [SCS](https://github.com/cvxgrp/scs) 2.0.0 and higher.

To install SCS as an R package from source:
```shell
git clone --recursive https://github.com/bodono/scs-r.git
cd scs-r
./install.sh
```
this should install SCS globally. To test type
```shell
R --no-save < test/random_lp.R
```
(this is also called by the install script).

To call SCS use the function `scs`, defined as
```R
scs <- function(A, b, c, cone, params)
```
where `A` is a `Matrix` object, `b` and `c` are vectors, and `cone` and `params`
are lists specifying the cone dimensions and input params respectively.

