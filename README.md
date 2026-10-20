# Errors-in-variables estimation in Stata and Mata

Research code for estimating linear regression models with mismeasured regressors using information in higher-order cumulants and moments.

The repository includes the `XTEWreg` command, its Mata implementation and supporting routines, plus `Symbolic.mata`, a symbolic-algebra library for Mata.

## Files

- `XTEWreg.ado` and `XTEWreg.sthlp`: command and help file.
- `EWreg.mata`, `EWdata.mata`, `EWopt.mata`, `EWproblem.mata`: estimator and supporting components.
- `Partitions.mata` and `Symbolic.mata`: supporting mathematical routines.
- `Example.do`: an original example script. It references a local working directory and `EJW1.dta`; the dataset is not included in the repository root, so this is not a self-contained demonstration.

## Using the command

The repository help file describes syntax, options and model assumptions. The [SSC package record](https://econpapers.repec.org/software/bocbocode/s457525.htm) lists the distributed command, its dependencies and example files. Install it from Stata:

```stata
ssc install xtewreg
help xtewreg
```

This repository is an earlier research snapshot, last updated in 2014. It predates the 2017 journal article; do not assume it is identical to the distributed package or the published software release. Current installation and execution were not tested in this documentation update.

## Related publication

Timothy Erickson, Robert Parham and Toni M. Whited (2017), [Fitting the errors-in-variables model using high-order cumulants and moments](https://www.stata-journal.com/article.html?article=st0469), *Stata Journal*.

[Software overview](https://kn.owled.ge/software/#ewreg) · [Research](https://kn.owled.ge/research/)

Existing file-level authorship and license notices are retained.
