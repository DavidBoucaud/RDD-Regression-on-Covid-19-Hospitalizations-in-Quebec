# RDD-Regression-on-Covid-19-Hospitalizations-in-Quebec
RDD regression and analysis of daily admittance of covid-19 patients to hospitals in Quebec. The RDD regression focuses on important events during the pandemic.

## Introduction
  The concept here is simple: we will run several Ordinary Least Squares Linear Regressions (from statsmodels) on the daily Covid-19 cases detected. For each key event (lockdown, reopening), we will run a seperate regression before or after the date. If we capture a sufficient timeline, we can analyse the true effect of the event.
 I say this ('true effect') because the events are often a response to the growth or decline of Covid-19 cases. It is often true that the daily cases continue to rise following a lockdown, but a longer trend will reveal that the lockdown lowered the overall trend.
 
 ## The Plot
  I (hope) that the plot is farily intuitive (see RDD Plot.pdf). We see that the effects of the events are what would be expected, to varying degrees. I chose to generate the size of each scatter plot point from the current number of hospilizations from Covid-19, to further illustrate a worrying trend that seems to operate almost independently of the events.
  
 ## The Findings
  As mentioned, the effect of the events is farily intuitive. There are still a few important notes. The firth graph is the least effective in denoting a before/after trend (statistically proven by similar coefficients). This is likely due to insufficient test data at the beginning of the pandemic.
  
  An interesting note is the coefficient returned on the polynomiral feature. This coefficient, if negative, denotes that the trend is increasing. THe opposite is true if it is positive.
  
  Please feel free to contact me with any questions. The code here is really simple, and their are more events and data points since this project was completed.
