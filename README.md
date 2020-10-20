
## __PROJECT__

### IBM Exploratory Data Analysis for Machine Learning


#### Course Project

Hannah_Reber

20.10.2020

#### project:
https://www.coursera.org/learn/ibm-exploratory-data-analysis-for-machine-learning/home/welcome



# Assignment topic: House_Prices

### Dataset download and description
https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data
"With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, this competition challenges you to predict the final price of each home."

### Dataset summary
- original dataset needed a lot of cleaning, but is very diverse and very good for cleaning practice


# Initial plan for data exploration: Predict House_Prices
#### aiming to predict the sales prices

"Predict sales prices and practice feature engineering, RFs, and gradient boosting"

# Actions taken for data cleaning and feature engineering
#### all actions taken: see sub/nb1-4

- NA-Handeling
- Assigning numeric values to all columns based on value count ranks
- Merge repetative columns
- Assigning contant

# Key Findings and Insights
#### all key findings in statistical-analysis.ipynb

*Correlations*
Top 5:
- 1. RANK: 'OveralQual' 
- 2. RANK: 'GrLivArea'
- 3. RANK: 'GarageCars'
- 4. RANK: 'GarageArea'
- 5. RANK: 'TotalBsmtSF'

*Timedependency*
SEASONALITY: 
- density (= number of houses sold) varies over time: peaks in summers     
- price range: most houses between 10K and 30K, only a handful prices >10K or >30K
- relation: prices also seem to increase during selling-season(=summer) 


# Hypothesis
#### 3 main hypothesis used in analysis

- 1. H1: Sales Prices are dependent on seasonality 
- 2. H2: Summer is the best selling season
- 3. H3: OveralQuality is most important real estate property



# Significance testing
#### full OLS models in sub4_STEP_4_OLS.ipynb 

Significance was tested via OLS modeling and visualized via scatterplot, boxplot correlations and time series.

# Next steps
#### ML model

Next steps suggestion: using the cleaned data to train a deep learning framework and compare predictions.


## _Contents_of_this_Repo_

#### 1/ _analysis_notebook_=_summary_+_overview_analysis
 _main_notebook_ = statistical-analysis.ipynb

#### 2/ _files_g1:9_
 _png_images_generated_in_sub_notebooks_and_integrated_in_main_notebook_ = statistical-analysis.ipynb

#### 3/ _data_folder_
 _input_and_output_csv_ = data

#### 4/ _subs_folder_
 _all_sub notebooks_with_detailed_analysis_steps_ = subs
