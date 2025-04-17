# House Value prediction

## Table of Contents

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning/Preparation](#data-cleaning/preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results/Findings](#results/findings)
- [Modeling](#modeling)
- [Recommendations](#recommendations)
- [Limitations](#limitations)

### Project Overview

The goal of this project is to predict the median house value using a combination of engineered features and machine learning models, the project aims at identifying key factors affecting house prices and provide insights through both python modeling and Power BI visualizations.

### Data Source

Housing Data: The primary dataset used for this analysis is the "housing.csv", containing detailed information about houses within the region.

### Tools 

- Python - Data Cleaning
- ML Libraries
   - numpy, pandas - Data Analysis
   - sklearn, tensorflow - Data Modeling
   - seaborn, matplotlib - Data Visualization
- Power BI - Creating reports

 ### Data Cleaning/Preparation

 In the initial data preparation phase,we performed the following tasks:
 - Data loading and inspection.
 - Handling missing values.
 - Data cleaning and preprocessing

  ### Exploratory Data Analysis
  
  EDA involved exploring the housing data to answer questions, such as:

![powerbi image](https://github.com/user-attachments/assets/76808c9b-eaf1-41b3-87c2-2cecde47391a)
  - what factors most influence housing prices?
  - Does proximity to the ocean affect house prices?
  - Is the number of rooms per household a strong predictor of house prices?




    

  ### Data Analysis

    ```python
     1️⃣ Rooms per Household
       data['rooms_per_household'] = data['total_rooms'] / data['households']
    2️⃣ Bedrooms per Room
      data['bedrooms_per_room'] = data['total_bedrooms'] / data['total_rooms']
    3️⃣ Population per Household
     data['population_per_household'] = data['population'] / data['households'];
    ```

  ### Results/Findings

    The analysis results are summarised as follows:
    1. Higher income categories, though smaller in number,significantly impact total house value, underscoring income as a strong determinant of housing prices
    2. Homes with more generous space allocations(lower bedrooms per room ratios) are associated with with higher values, highlighting the premium placed on spaciousness.
    3. The number of rooms per household does not have a consistent correlation with house prices, indicating that other factors may play more significant roles.
    4. Location,especially proximity to the ocean and latitude, affects house values, with inland properties exhibiting distinct patterns.

   ### Modeling

   Multiple machine learning models were trained and compared:


   ### Recommendations
   Based on the analysis,we recommend the following actions:
   1. Real estate agencies shoulf focus marketing and premium housing developments in high income areas to maximize profit.
   2. Design homes with spacious layouts to appeal to buyers  in higher price segments
   3. Highlight proximity to the ocean as a selling point in listings and marketing.

  ### Limitations
 - I had to handle missing values
 - I had to standardize the median income column to make meaning of it
 - I had to drop features that were not useful to the analysis.

  ### References
  1. Scikitlearn
  2. My Past Projects


       
