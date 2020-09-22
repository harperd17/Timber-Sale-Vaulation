# Predicting the Value of a Timber Plot
---
## Overview
---
A Data Science firm was contracted to build a pricing model for a logging company to aid in their bidding strategy for forest plots. The main goal is to be able to accurately predict the bidding price for a plot of land given data provided by the Bureau of Land Management (BLM). I built a linear regression pricing model that utilizes the estimate of board feet and cubic feet of wood on the plot of forest, the acres on the plot, and an interaction term between these two variables. This pricing model is fairly accurate in both the data used to build it, as well as testing data never seen by the model. However, the model is most accurate at predicting the value of plots less than 490 acres that have wood volume below a certain threshold.
## Data
---
Bureau wide BLM timber sale data was obtained from __[blm.gov](https://www.blm.gov/programs/natural-resources/forests-and-woodlands/timber-sales/bureau-wide-timber-data)__. The data is made up of 31 quarterly excel files each containing information on all active timber contracts from 2012 through 2020 as well as the winning bid price at auction. I combined the 31 excel files into one csv file. Since each timber contract is active for multiple quarters, each contract is displayed multiple times with values changing in response to progress in the logging operation. Therefore, the data needed to be thoroughly cleaned to only show one observation per contract before performing analysis. After cleaning, the data has 1,116 observations and each observation has 6 raw features of initial interest. The plots of land involved are located in either Alaska, Oregon, California, Montana, Idaho, Wyoming, or Colorado and vary greatly in size and value.
## Repository Navigation
---
<pre>
Code               : <a href=https://github.com/harperd17/Timber-Sale-Valuation/tree/master/Notebooks/Modelling Code.ipynb>Model Building Notebook </a>
Report             : <a href=https://github.com/harperd17/Timber-Sale-Valuation/tree/master/Report/Report Notebook.ipynb>Report Notebook</a>
</pre>
## Project Information
---
<b>Author: </b>David Harper <br>
<b>Language: </b>Python <br>
<b>Tools/IDE: </b>Anaconda <br>
<b>Libraries: </b>numpy, pandas, plotly, matplotlib, math, sklearn, statsmodels
