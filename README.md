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
#### 2.0 - 1/3/22
- Complete rebuild built on stanarm R package with original concepts
#### 1.0 - 11/23/21
- Proof of concept using the bayseab R package and built on backbone of frequentist ab test analysis app