# Bayesian inference for SARS-CoV-2 transmission modelling, using Stan

## Author: Bethan Cracknell Daniels

The aim of this exemplar is to demonstrate how to design and fit a mathematical model of disease transmission to real data, in order to estimate key epidemiological parameters and inform public health responses. Specifically, we will model the emergence of the SARS-CoV-2 variant of concern Omicron in Gauteng, South Africa. To fit the model, we use Stan, a free, accessible and efficient Bayesian inference software. Adopting a Bayesian approach to model fitting allows us to account for uncertainty, which is especially important when modelling a new pathogen or variant. The transmission model uses compartments to track the population’s movement between states, for instance from susceptible to infectious. By fitting a compartmental model to genomic and epidemiological surveillance data, we will recreate the transmission dynamics of Omicron and other circulating variants, and estimate key epidemiological parameters. Together these estimates are useful for guiding policy, especially in the early stages of an emerging variant or pathogen, when there are lots of unknowns

### Prerequisites:

Required:
- Experience using R, for instance the Graduate school course *R programming*.
- Knowledge of Bayesian statistics, for instance, the textbook *A students guide to Bayesian statistics* by Ben Lambert is a great place to start. Chapter 16 also introduces Stan. 

Beneficial:
- Some familiarity with Stan. 

### Learning outcomes:

1.	Students will be able to design an infectious disease compartmental model to answer public health questions. 
2.	Students will gain appreciation of the benefits of using simulated data to debug models.  
3.	Students will be able to code up an Rstan model to fit an infectious disease model to observed data and estimate parameters.
4.	Students will be able to clean and format data using Tidyverse and produce high level plots using ggplot, in R. 

### Project structure 

The project is split into 2 parts, with each part introducing a progressively more complex infectious disease model. Each part demonstrate how to design an infectious disease model and fit it in Rstan to real data. 

#### Part 1 

In part 1, you will find the following folders: 

- scripts
- R (functions)
- data
- models
- figures 


Briefly, the **scripts folder** contains several R scripts:
 
- *simulate_model1_data.R* - this will simulate data
- *fit_model1_solver.R* - this will fit the simulated data using Rstan 
- *clean_model1_data.R* - this will clean and format the observed data, using tidyr
- *diagnose_model.R*  - this will check the model fit and help diagnose issues 
- *plot_model.R* - this will plot the model output against the observed data, using ggplot

The **R folder** contains the functions needed to run each of the scripts. 

The **data folder** contains the raw data which we fit out model to:

- simulated data generated by *simulate_model1_data.R*
- observed data cleaned in *clean_model1_data.R*

The **models folder** contains the Rstan model designed in part 1 

The **figures folder** is where we will save all our model fits. 

Moreover, each module will be accompanied  by lots of internal and external learning resources! 

##### 

```diff 

@@How to Use the Code@@

** Requirements **

- R (version XXX or higher)
- RStudio (if needed)
- packages
  - rstan
  - others (for example ....)

