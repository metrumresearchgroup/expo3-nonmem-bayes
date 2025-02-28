# expo3-nonmem-bayes

This repository contains examples of the various tasks associated with the
completion of a modeling project with Bayesian estimation in NONMEM. The goal
is to represent the most up-to-date packages and methodologies for completing
these tasks. These will evolve with time so check back periodically.
be best to check back periodically.

# Data
- PK model estimation data set 
  - location : `data/derived/pk.csv`
  - spec file : `data/derived/pk.yml`

# Scripts
- Model creation, submission & management: `model-management.R`
  - Example code that may be used in model-management.R: `model-management-demo.Rmd`
- Diagnostic plots are created in: `model-diagnostics.R`
  - this R script uses Rmd templates to make html files that will be saved to
  your model directory:
    - `diagnostic-templates > template-model-bayes.Rmd` 
    - `diagnostic-templates > template-mcmc.Rmd` 
- Model summary: `model-summary.Rmd`
- Parameter tables: 
  - Parameter key for all tables is included in a yaml: `pk-parameter-key.yaml`
  - Parameter table for base model: `pk-base-model-table.R`
  - Parameter table for final model (incl. covariates): `pk-final-model-table.R`
- Figures for report 
  - Goodness-of-fit evaluations from `model-diagnostics.R` with `template-model-bayes.Rmd` 
  - MCMC diagnostics from `model-diagnostics.R` with `template-mcmc.Rmd` 
  - Covariate effects evaluation from `forest-plots.R`
- Visual predictive checks:
  - `pk-vpc-final.R`
  - `pk-pcvpc-final.R`


# Helper functions
- Helper functions for model management: `functions-model.R`
- Helper functions for scripts creating tables: `functions-tables.R`
- Helper functions for creating the model diagnostics: `functions-diagnostics.R`
- Helper functions for various Bayesian-specific diagnostics:
  `functions-mcmc-diagnostics.R` and `functions-diagnostics-rhat-ess.R`

# Metworx Version
- metworx-22-09.00.03

# R Version
- 4.1.3

# NONMEM Version
- 7.5.1


Copied from internal repo at a8d1475b6b867148393f493bd94a23cdf8d9d21b

