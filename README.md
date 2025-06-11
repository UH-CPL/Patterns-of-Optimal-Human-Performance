# Patterns of Optimal Human Performance

This repository contains R code and data for the *Patterns of Optimal Human Performance* research project. All configuration is self-contained in the scripts, so no external setup is required. Scripts prefixed with `Model_` fit the statistical models, and scripts prefixed with `Figure_` generate the analysis plots from those model results.

## Requirements

- **R** (version 4.0.3 or higher)  
- **R packages:**  
  - `moments`  
  - `poweRlaw`  
  - `car`  
  - `MASS`  
  - `STAND`  
  - `nortest`  
  - `truncdist`  
  - `EnvStats`  
  - `igraph`  
  - `knitr`  
  - `pander`  
  - `ggplot2`  

Install these using `install.packages()` as needed.

## Data

- The file `data_03312020.zip` contains all raw data files (CSV) used in the analysis.  
- See the included `DataDescription.docx` for dataset and variable details. Additional context is available on the [OSF project page](https://osf.io/9bjwx/).

## Reproducing the Results

1. **Install required packages**  
   In R, install any missing packages:
   ```r
   install.packages("poweRlaw")
   install.packages("ggplot2")
   # Repeat for the remaining packages

2. **Set the working directory**
Set your R or RStudio working directory to the folder containing the scripts and data.

3. **Prepare the data**
Unzip data_03312020.zip so that all data files are accessible in the working directory.
Data: https://osf.io/9bjwx/  

4. **Run model scripts**
Execute each script starting with Model_. These scripts fit statistical models to the data and save the results.

5. **Run figure scripts**
Execute each script starting with Figure_. These generate the plots based on the model outputs.

6. **Inspect the results**
Output figures will be saved in the working directory or as specified within each script.

No additional configuration is required; all paths and parameters are pre-set in the scripts.
