This package constitutes an interactive R problem set based on the RTutor package (https://github.com/skranz/RTutor). 

Welcome to this interactive RTutor problem set on China’s War on Pollution based on the scientific paper “Can Technology Solve the Principal-Agent Problem? Evidence from China’s War on Air Pollution” by Greenstone, He, Jia, and Liu, published in the American Economic Review: Insights journal in 2022. This problem set is part of my master’s thesis at Ulm University, and I hope it will pique your interest and expand your knowledge of R programming and econometrics.

Environmental pollution is a significant global issue, with China being especially affected due to its rapid economic growth in recent decades. This growth has led to a significant increase in air, water, and soil pollution, adversely affecting the health and well-being of billions of people. Therefore, environmental pollution is a highly relevant topic in Chinese politics. This interactive analysis focuses specifically on air pollution, which was also the centerpiece of the War on Pollution declared by the Chinese government in 2014. The initiative included a countrywide, real-time air quality monitoring and reporting program aimed at improving the availability and quality of air pollution data. Prior to the implementation of this new technology, local city governments, which are de facto subordinate to the Chinese central government, collected the data before it was published. As this scenario created a potential principal-agent problem, we will use a Regression Discontinuity (RD) design to analyze if there  is any evidence for structural data manipulation of air pollution data before the new technology was implemented.

## 1. Installation

RTutor and this package is hosted on Github. To install everything, run the following code in your R console.
```s
install.packages("RTutor",repos = c("https://skranz-repo.github.io/drat/",getOption("repos")))

if (!require(devtools))
  install.packages("devtools")

devtools::install_github("fwaldhans/RTutorAirPollutionChina")
```

## 2. Show and work on the problem set
To start the problem set first create a working directory in which files like the data sets and your solution will be stored. Then adapt and run the following code.
```
library(RTutorAirPollutionChina)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorAirPollutionChina")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorAirPollutionChina",
       auto.save.code=TRUE, clear.user=FALSE)
```
If everything works fine, a browser window should open, in which you can start exploring the problem set.
