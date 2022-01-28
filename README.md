# A/B Test Bayesian Analysis Tool
A Shiny Application to support Bayesian A/B Testing

This application takes conversion and traffic inputs for control and test variants, calculates posterior distributions, and analyzes for:
- Probability the test is better than the control 
- Probability of a null result based on a region of practical equivalence
- Probability of a non-inferior result
- Probability of a significant result
- Probability of a result that meets ROI expectations


See the live version here: https://sdidev.shinyapps.io/bayesian-ab-app/

## Version History
#### 2.2 - 1/28/22
- Fixed posterior analysis for negative outcomes
- Added guidance for judging outcomes (compared at 95% probabilities)
- A few minor adjustments/fixes

#### 2.1 - 1/7/22
- Replaced `rstan` method (and the logistic regression + MCMC) with more basic `rbeta()` function. This enabled us to use the shinyapps.io server for the app, which didn't care for `stanarm`.
- Minor updates to color scheme, element positions and documentation
#### 2.0 - 1/3/22
- Complete rebuild built on stanarm R package with original concepts
#### 1.0 - 11/23/21
- Proof of concept using the bayseab R package and built on backbone of frequentist ab test analysis app