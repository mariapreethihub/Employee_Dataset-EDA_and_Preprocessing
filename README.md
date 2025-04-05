# Employee_Dataset-EDA_and_Preprocessing

### Table of Contents
-	[Project Overview](#project-overview)
-	[Data Source](#data-source)
-	[Tools](#tools)
-	[Data Preprocessing](#data-preprocessing)
-	[Tasks](#tasks)
-	[Insights](#insights)

### Project Overview

The main objective of this project is to design and implement a robust data preprocessing system that addresses common challenges such as missing values, outliers, inconsistent formatting, and noise. By performing effective data preprocessing, the project aims to enhance the quality, reliability, and usefulness of the data for machine learning.

### Data Source
File: [Employee.csv](https://drive.google.com/file/d/1F3lRf32JM8ejnXq-Cbf9y7fa57zSHGz_/view?usp=sharing )

### Tools
The analysis was conducted using Python 3.x [Download here](#http://python.org/)
with the following libraries: 

-     Pandas
       
  - Installation: ‘pip install pandas’.
    
-	    NumPy
  
  - Installation:  ‘pip install numpy’.
    
-	   Matplotlib
  
  - Installation:  ‘pip install matplotlib’.
    
-	   Seaborn
  
  - Installation: ‘pip install seaborn’.

-   from sklearn.model_selection import train_test_split

     - for xtrain and x test splitting
       
-   from sklearn.preprocessing import StandardScaler, MinMaxScaler,OneHotEncoder,LabelEncoder

     - for scaling and Encoding

### Data Preprocessing
In the initial data preparation, the following tasks were performed:
1. Loading data and inspecting the dataset.
2. Checking basic information (column types, number of rows, missing values, etc.).
3. Checking null values
4. Handling missing values.
5. Checking duplicate rows.

### Tasks
This step involved exploring data to answer the key questions such as:

#### Question 1: Data Exploration
            
            - Found the unique values in each feature and its length.
            - Performed summary statistics to understand the data distribution and renamed the columns.
            
#### Question 2: Data Cleaning
          
            - Missing and inappropriate values are treated.
            - Removed all duplicate rows.
            - Outliers are identified.
            - Replace the value 0 in age as NaN.
            - Null values in all columns are replaced with median(numerical) and mode(categorical)


           
#### Question 3: Data Cleaning

            - Filtered the data with age >40 and salary<5000
            - Plot the chart with age and salary
            - Counted the number of people from each place and represented them visually.

#### Question 4:Data Encoding

          - Converted categorical variables into numerical representations using techniques such as one-hot encoding, label encoding, 
            making them suitable for analysis by machine learning algorithms.

#### Question 5:Feature Scaling

          - Performed scaling of the features using standardscaler and minmaxscaler.

### Insights 

          - Most employees in the dataset belong to certain companies like TCS and Infosys.
          - Some age values were incorrectly recorded as 0 and same is cleaned.
          - Outliers in employee age and salary were identified using the Interquartile Range method and subsequently imputed using median values for data consistency and accuracy.
          - The highest number of employees are located in Mumbai.
