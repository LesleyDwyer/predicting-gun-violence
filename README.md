# Data wrangling and multiple regression to predict US gun violence from county health data

This is the coursework for my Principles of Data Science module at City, University of London in 2018-19. It was an individual project where I chose datasets, performed data analysis, data processing, feature engineering and model building. Then, I wrote a short paper explaining my findings. 

This project was to investigate whether health factors at a county level could be used to predict US gun violence. As part of the data analysis and processing, I used a web API call to supplement the data, I imputed missing values, checked for outliers, transformed data using log and square root transformation, and re-scaled the data. I then checked feature correlation and used Principle Component Analysis (PCA) for feature selection. Finally, I built multiple regression models: one using features from PCA and one using features ranked from a correlation matrix. I used 10-fold cross-validation to estimate the performance using the Mean Squared Error (MSE) and R-squared for each model. 

There are five files:
  1) gun_violence_with_FIPS.zip - Gun violence data from Kaggle for 2017 only. Unzip it first. The FIPS column has been added to this dataset via a web API. Source dataset can be found here: https://www.kaggle.com/jameslko/gun-violence-data
  2) 2018CountyHealthRankingsData-v1.xls - County Health Rankings data from: http://www.countyhealthrankings.org/explore-health-rankings/rankings-data-documentation 
  3) LDwyer INM430 Coursework Notebook.ipynb - the Jupyter Notebook I built including Python code and explanations
  4) LDwyer INM430 Coursework Report.pdf - the short paper I wrote explaining my findings.
  5) gun-violence-data_2017.zip - Gun violence data without FIPS column. This is not needed to run the code, but to re-create the steps I followed, unzip it and uncomment the web API section in the Jupyter Notebook before running. However, it will take several hours to run. 
  
To run the code, save files 1-3 into the same directory and ensure file 1 is unzipped. Open Jupyter Notebook and navigate to the directory where you've saved the files. Run the notebook.
