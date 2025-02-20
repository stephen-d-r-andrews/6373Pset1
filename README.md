# 6373Pset1
6.373 Pset 1 


Problem 1.4: [15 pts] Detecting Leukemia types
The data set golub consists of the expression levels of 3051 genes for 38 tumor mRNA samples.
Each tumor mRNA sample comes from one patient (i.e. 38 patients total), and 27 of these tumor
samples correspond to acute lymphoblastic leukemia (ALL) and the remaining 11 to acute myeloid
leukemia (AML). How many genes are associated with the different tumor types (meaning that
their expression level differs between the two tumor types) using (i) the uncorrected p-values, (ii)
the Holm-Bonferroni correction, and (iii) the Benjamini-Hochberg correction? Feel free to use
libraries for multiple hypothesis testing in R or python. You can use α = 0.05 for the significance
threshold.
Source of data: Golub et al. (1999). Molecular classification of cancer: class discovery and class
prediction by gene expression monitoring, Science, Vol. 286:531-537.

Problem 1.5 (a): [20 pts] Regression
In this problem, we will look at OLS.
i) Read in the synthetic data matrix syn_X.csv and the vector syn_y.csv of “observations”.
Compute the OLS estimator ˆβ by matrix inversion.
Next, we look at some real data. General Motors collected data (found in mortality.csv) from
60 US cities to study the contribution of air pollution to mortality. The dependent variable is the
age adjusted mortality (Mortality). The data include variables measuring climate characteristics
(JanTemp, JulyTemp, RelHum, Rain), variables measuring demographic characteristics of the
cities (Educ, Dens, NonWhite, WhiteCollar, Pop, House, Income), and variables recording
the pollution potential of three different air pollutants (HC, NOx, SO2).
ii) Get an overview of the data and account for possible problems. Which cities stand out?
Which of the variables need to be transformed?
iii) Carry out a multiple linear regression containing all variables with the necessary transfor-
mations (with matrix inversion as in (i)). Does the model fit well? Check the residuals.

Problem 1.5 (b): [10 pts] Computational Aspects of Regression
In this problem, we will consider some computational challenges that arise in practice when
performing linear regression.
i) Suppose you have a problem in which the data matrix, X, has 100 million rows and 200
columns (each row is a data point and each column is a feature / covariate). What challenge
will arise when you try to apply the matrix inversion method to compute the regression
coefficients as in the previous problem? (Hint: if each entry is a 64 bit float, how much
memory will be required to store X?)
ii) Suggest one method that will allow you to compute linear regression coefficients for this
problem. Be specific. Discuss pros and cons of your approach