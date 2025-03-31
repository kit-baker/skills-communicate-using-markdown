# This is an H1 header, using one hastag
### This is an H3 header, with three hashtags
###### and this is the smallest header, H6

Added three headers of different sizes to show the different types of headers

# below is an image of Yaktocat
![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)

# this is an example of python code used for D47crunch

```
import D47crunch  
mydata = D47crunch.D47data()  
import os  
import numpy as np  
os.chdir("/Users/KitBaker/Documents/Cambridge/PhD/Python/Formatted Easotope Data")  
mydata = D47crunch.D47data()  
mydata.ALPHA_18O_ACID_REACTION = np.float64(1.008709)  
  ### Read the CSV file
mydata.read('Cambridge_Northumbria_Combined.csv')
  ### Compute δ13C, δ18O of working gas
mydata.wg()
  ### Compute δ13C, δ18O, raw Δ47 values for each analysis
mydata.crunch()  
  ### Compute absolute Δ47 values for each analysis
mydata.standardize()
  ### Compute repeatabilities
mydata.repeatabilities()
```

# and this is R code for plotting my data
```
library(rio) # for importing excel files  
library(readxl)  
library(devtools)  
library(ggplot2)  
library(qpcR)    
setwd("~/Documents/Cambridge/PhD/CLumped/R")  
cbbPalette <- c("#000000", "#E69F00", "#56B4E9", "#009E73", "#F0E442", "#0072B2", "#D55E00", "#CC79A7", "#999999")  
fourtyseven <- 47  
par(mfrow=c(1,3))  
par(mar = c(3,6,3,6))  
myData <- import("HOBO bellows 47.xlsx")   
```
