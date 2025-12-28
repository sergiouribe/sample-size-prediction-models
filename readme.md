# Sample Size Calculations for Caries Prediction Models

Sample size calculations for developing and validating AI-based prediction models in caries research, following the criteria of Riley et al. (2019, 2020, 2021).

## Scripts

| Script | Outcome | Description |
|--------|---------|-------------|
| `01_binary_caries_incidence.R` | Binary | Predicting if a caries-free child will develop caries in 2 years |
| `02_continuous_new_lesions.R` | Continuous | Predicting number of new lesions in 2 years |
| `03_continuous_lesion_progression.R` | Continuous | Predicting how many existing lesions will progress |

## Requirements

```r
install.packages(c("pmsampsize", "pmvalsampsize", "tidyverse"))
```

## References

- Riley RD, et al. Minimum sample size for developing a multivariable prediction model: Part II binary and time-to-event outcomes. *Stat Med*. 2019;38:1276-96.
- Riley RD, et al. Calculating the sample size required for developing a clinical prediction model. *BMJ*. 2020;368:m441.
- Riley RD, et al. Minimum sample size for external validation of a clinical prediction model with a binary outcome. *Stat Med*. 2021;40:4230-51.

## License

MIT