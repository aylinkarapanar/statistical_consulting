# Mosquito Abundance Project (Simulation, Missingness, and Mixed-Effects Modelling)

This repository contains the full analytical workflow for simulating mosquito abundance data, diagnosing missingness mechanisms, and fitting mixed-effects models to study how environmental factors influence mosquito populations. The project also includes an example of spatial sampling using Copernicus land-use data.

## Repository Structure

Copernicus Data/NL013L3_NIJMEGEN_UA2018_v013/     # Land-use data used for spatial sampling

Simulated Data/                        # All mock datasets generated in the project

Data_Simulation.Rmd                    # Code for generating the mock mosquito dataset  
Data_Simulation.nb.html

Example_Sampling_Nijmegen.Rmd          # Example site-selection workflow using Copernicus data  
Example_Sampling_Nijmegen.nb.html

Missingness.Rmd                        # MCAR, MAR, MNAR simulations and diagnostics  
Missingness.nb.html  
Missigness comments and html/          # Annotated notes for the client

Mixed_Effects_Modelling.Rmd            # GLMM (glmmTMB) model for mosquito abundance  
Mixed_Effects_Modelling.nb.html

.gitattributes  
.gitignore  
README.md

# 1. Overview

This repository provides:

- A full mock mosquito dataset for teaching and planning  
- Simulations of missing data mechanisms (MCAR, MAR, MNAR)  
- A mixed-effects model using `glmmTMB`  
- Model diagnostics, predicted effects, and visualizations  
- A spatial sampling example using Copernicus land-cover layers  

# 2. Data Simulation

File: `Data_Simulation.Rmd`  
Generates realistic mock dataset with environmental variables, species, trap types, and negative binomial counts.

# 3. Missing Data Analysis

File: `Missingness.Rmd`  
Includes simulation and detection of MCAR, MAR, MNAR, and recommendations.

# 4. Mixed-Effects Modelling

File: `Mixed_Effects_Modelling.Rmd`  
Includes GLMM modelling, diagnostics, predictions, and plots.

# 5. Running Instructions

Install packages:

```
install.packages(c(
  "tidyverse", "lubridate", "glmmTMB", "DHARMa",
  "emmeans", "ggeffects", "sf", "terra"
))
```

To knit:  
Open any `.Rmd` file an click **Knit**.

# Authors 

Atakan1507 & aylinkarapanar
