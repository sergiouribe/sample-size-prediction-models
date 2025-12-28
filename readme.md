# Sample Size Calculations for Caries Prediction Models

Sample size calculations for developing and validating AI-based prediction models in caries research, following Riley et al. methodology.

## Scripts

| Script | Stage | Outcome | R Package | Description |
|--------|-------|---------|-----------|-------------|
| `01_development_binary.qmd` | Development | Binary | `pmsampsize` | Sample size to develop a model predicting caries incidence (Yes/No) |
| `02_development_continuous.qmd` | Development | Continuous | `pmsampsize` | Sample size to develop a model predicting number of new lesions |
| `03_validation_binary.qmd` | Validation | Binary | `pmvalsampsize` | Sample size to externally validate a binary prediction model |
| `04_validation_continuous.qmd` | Validation | Continuous | `pmvalsampsize` | Sample size to externally validate a continuous prediction model |

## Key Distinction

- **Development** (`pmsampsize`): Calculates sample size to build a model with minimal overfitting. Depends on number of predictor parameters.
- **Validation** (`pmvalsampsize`): Calculates sample size to precisely estimate model performance (C-statistic, calibration). Independent of model complexity.

## Requirements
```r
install.packages(c("pmsampsize", "pmvalsampsize", "tidyverse"))
```

## References

- Riley RD et al. (2020). Calculating the sample size required for developing a clinical prediction model. *BMJ*. 368:m441. doi:10.1136/bmj.m441
- Riley RD et al. (2024). Evaluation of clinical prediction models (part 3): calculating the sample size required for an external validation study. *BMJ*. 384:e074821. doi:10.1136/bmj-2023-074821
- Uribe SE et al. (2021). Prevalence of early childhood caries. *Int J Paediatr Dent*. 31:817-830. doi:10.1111/ipd.12783

## Authors

**Sergio E. Uribe** <sup>a,b,c,d</sup>, **Alonso Carrasco-Labra** <sup>e</sup>, **Falk Schwendicke** <sup>c</sup>, **Ilze Maldupa** <sup>a,b</sup>

<sup>a</sup> Department of Conservative Dentistry and Oral Health, Riga Stradins University, Riga, Latvia  
<sup>b</sup> RSU Institute of Stomatology, Riga, Latvia  
<sup>c</sup> Department of Conservative Dentistry, Periodontology and Digital Dentistry, LMU University Hospital, LMU Munich, Munich, Germany  
<sup>d</sup> Baltic Biomaterials Centre of Excellence, Headquarters at Riga Technical University, Riga, Latvia  
<sup>e</sup> Center for Integrative Global Oral Health, University of Pennsylvania School of Dental Medicine, Philadelphia, PA, USA

## Contact

sergio.uribe [at] rsu [dot] lv

## License

MIT
