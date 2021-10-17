### 🕵️‍ PERFORM ‘EXPLORATORY DATA ANALYSIS’ ON DATASET ‘SAMPLESUPERSTORE’ 
![yes (1)](https://user-images.githubusercontent.com/79318960/137638618-e0ce2b6f-aebb-4de4-b9c0-662e33341071.gif)

### We will explore a Data set and perform the exploratory data analysis in python

### 📝  step-1: Import the Necessary Libraries

  - Numpy,
Pandas,
Matplotlib,
seaborn.

### ⏳ step-2: Loading the Data set

 - loading the CSV file using pandas for this will be using read_csv file command

### 🔎 step-3: Basic Data Exploration

i. head of the dataset
 
  - The head function will tell you the top records in the data set. By default, python shows you only the top 5 records.

ii. shape of the dataset

-    The shape attribute tells us a number of observations and variables we have in the data set. It is used to check the dimension of data. The samplesuper store data set has 9994 observations and 13 variables in the data set.

-    Looking at the data in the head function and in info, we know that the variable Income and travel time are of float data type instead of the object.

iii. info of the dataset

-  info() is used to check the Information about the data and the datatypes of each respective attribute.
  
iv. summary of the dataset

-  The described method will help to see how data has been spread for numerical values. We can clearly see the minimum value, mean values, different percentile values, and maximum    values.

### 📝  step-4: Handling Missing Value

-  We can see that we have various missing values in the respective columns
-  Data.isnull().sum() for checking Null values
#### (Here All the columns variable are non-null)

### :broom:  step-5: Cleaning the Data

## 17 records are duplicate 😟
- Checking which 17 records are duplicated
- After that Removed the duplicated record from dataset using Data.drop_duplicates(inplace=True) command
- Again checking total no of duplicates which was 0
- checking shape again after removing 17 duplicated rows (9977,13)

#### We should drop the country, postal code columns. Because country,postal codes are of no use. so It will not affect further analysis
- removed the country,postal code
- checking the columns again, Here country postal code are deleted


 ### 📈 step-6: Data Visualization
- we need to compare linear relationship between attributes using correlation coefficient generated using heatmap
- calculated Total Sales 2296195.59
- Total Quantity sold 37820
- Total profit 286241.42
- pairplot visual, pairplot takes only numerical values that is the reason for we are using pairplot here
