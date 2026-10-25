# README

**NOTE**: This is part of on-going research with Dr. Geist. You will be asked to contribute to a specific piece of this research project and, in exchange, you will also have the opportunity for co-authorship on the resulting methods paper. This opportunity is open to all students, and you do not need to have been involved in research in the past or familiar with surveys or survey weights to get involved.

## Project description
Large social surveys such as the CDC's Behavioral Risk Factor Surveillance System (BRFSS) use complex sampling designs and survey weights to support population-representative estimates. This project will investigate how incorporating survey weights affects machine learning analyses of self-reported coronary heart disease. The goal is to compare weighted and unweighted approaches using a clearly defined public health question and to develop practical recommendations for researchers applying machine learning to complex survey data. Primary uses could include:

- comparing predictive performance and calibration for weighted and unweighted models
- evaluating how weighting affects estimates of population-level patterns and subgroup performance
- investigating whether conclusions differ across interpretable baseline models and nonlinear machine learning methods
- developing reproducible recommendations for using survey weights in predictive analytics

## Research question
How does incorporating BRFSS survey weights affect the predictive performance, calibration, and population-level conclusions of machine-learning models for self-reported coronary heart disease?

The outcome should be defined using the selected BRFSS release's documented coronary heart disease and/or heart attack variables. If using the CDC-derived `_MICHD` variable, verify its definition and availability in the chosen year's codebook. This is a cross-sectional prediction task: the outcome represents reported disease history, not future disease incidence or prospective clinical risk.

## Data source
Centers for Disease Control and Prevention (CDC). Behavioral Risk Factor Surveillance System (BRFSS). https://www.cdc.gov/brfss/annual_data/annual_data.htm

BRFSS documentation and codebooks: https://www.cdc.gov/brfss/data_documentation/index.htm

## Suggested approach
- Select one annual BRFSS release and document the survey design, outcome definition, inclusion criteria, and predictor set
- Use a consistent training/test design for weighted and unweighted analyses
- Compare a simple interpretable baseline with at least one nonlinear model
- Specify separately whether weights are used during model fitting, performance evaluation, or both. Not every machine-learning implementation supports survey weights in the same way!
- Evaluate discrimination and calibration, and report population-weighted performance where appropriate
- Discuss how weighting changes the results, including subgroup patterns, and whether the conclusions are practically meaningful

## Important methodological considerations
Survey weighting does not necessarily improve every predictive metric. The purpose is to evaluate when and how weighting changes model behavior and population-level conclusions, not to assume one approach is universally superior. Account for the BRFSS sampling design when interpreting results, and distinguish predictive performance from population estimation and causal inference.

## Source citation
Centers for Disease Control and Prevention (CDC). Behavioral Risk Factor Surveillance System (BRFSS). Annual survey data and documentation. https://www.cdc.gov/brfss/annual_data/annual_data.htm

## Want a crash course in survey weights and why they matter?
Take a look at this [blog post](https://blog.djnavarro.net/posts/2025-09-27_survey-weights/) as a starting point! It's talking about the NHANES survey rather than the BRFSS, but the principles are the same!
