# Rainfall modelling - nonparametric regression
Project created for *Advanced Econometrics II* (org. *Zaawansowana Ekonometria II*) classes at WNE UW

Language:
 - Polish - classes, report and notebook

Semester: III (MA studies)

## About
The main objective of this project was to practice econometric methods learned during classes. We've got 4 parts of the material and we had to perpare 3 models, each from different part. This repo is about first part named *general methods* and contains standard OLS linear regression with diagnostics (Python) and non-parametric kernel regression (R). In this project Bartek Kuźma and I modelled monthly rainfall data in Poland with other atmospheric phenomena recorded at many weather stations (finally 17) during the 1960-2019 period. The data was collected from Polish Institute of Meteorology and Weather Management, loaded and cleaned with Python. Standard OLS with diagnostics was performed in Python too. Nonparametric regression was computed in R, but we lost that script, you can see what happened in our paper-style report (we had to send reports only as an assignment). This project was a little bit about data pre-analysis and much more about modelling. We applied a lot of diagnostic tools (many of them was written from scratch - statistical tests). We also coded a big wrapper for OLS in different variants (with lags, Box-Cox transform, VIF computation). The research idea was based on the found paper (Rahmatullah et. al.).

Findings
 - rainfall is such a complex process and modelling it in this way is about approximating cocount with chair (DGP and ommited variables stuff - endogenity), so statistical inference is not justified
 - there are much better methods for prediction
 - non-parametric methods are much more safe than OLS (no such strong assumptions)

In this project, I learned a bit of the econometric modelling practice (especially about Box-Cox transform). I practiced my Python skills too.

## Repository description
 - modele - folder with fitted models for different stations as html reports - easy to work with when report writing
 - Kuzma_Odziemczyk_minimodel_1.pdf - project report (I encourage you to check it, personally I like it)
 - Wczytywanie_danych.ipynb - Python notebook with data loading and saving (we've got lots of csv files)
 - data_cleaning_modelling_final.ipynb - PYthon notebook with data analysis and OLS modelling 
 - dane_pogodowe.csv - results of Wczytywanie_danych.ipynb 
 - dane_finalne.csv - final data
 - s_m_d_xx.csv - data from Polish Institute of Meteorology and Weather Management

## Technologies
 - Python (pandas, numpy, matplotlib.pyplot, seabor, statsmodels, stargazer, scipy, scikit-learn)
 - R (nonparametric regression - lost script not loaded into this repo)
 - LaTeX (report writing)
 
 ## Authors
 Bartek Kuźma
 Maciej Odziemczyk
 
 ## Note
 We used R to nonparametric regression due to lack of such package for Python<br>
 We had a different opinion from Rahmatullah et. al. about this task our conclusions was different too<br>
