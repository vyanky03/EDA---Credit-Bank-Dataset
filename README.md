# EDA---Credit-Bank-Dataset
Did full EDA process on the bank dataset. This data is of a bank which provides loan to the consumers and want to analysis the trend of defaulters and non defaulters across different cateogries available.
## Process of EDA
### 1) Applcation Dataset
- Loaded the datasets and require necessary libraries
- Understanding of data (shape, info(), describe(),head, tail)
- Datacheck:
  1) Finding of % null values in dataset
  2) dropping such column from dataset
  3) Suggested imputation of 5 columns whose null % is above 13%
  4) Cheked datatypes
  5) Changed datatypes of column from object to category wherever possible (using .astype())
  6) Converted negative values to positivw using .abs() function for few columns
  7) founnd outliers in numerical columns
  8) did binning and bucketting for categorical data for better understanding
- Analysis -
  1) Data imbalance study of target column
  2) divided dataset into two seperate dataset of defaulter and other cases
  3) Performed Univariate bivariate and multivariate analysis
### 2) Previous Applcation Dataset
- Did dataset loading, libraries loading, understanding of dataset and data check
### 3) Merging of Previous and Applcation Dataset
- Merged two datasets into one as both datasets have common coloumn SK-Id
- Performed univariate, bivariate and multivariate analysis on merged dataset

## Conclusion- 
1) Data Imbalance Study
   
     ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/6c021d64-a66e-49cd-9922-1f7982843536)

  - The number of defaulters are very less when compared to the repayers
  - There are more female clients than male clients.
2) Univariate Analysis of Application dataset

    ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/a18ad095-e6c9-45c0-bf9c-5e887300cbb6)

  - Most of the client opting for loans are female whether is it defaulter or non defaulter
  - 
    ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/902a8fe7-4f4d-4133-8ff4-b3fb78ea5c26)

  - As mentioned earlier and after seeing this graph its confirmed that the loan takers have taken secondary education
    
    ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/2410c2b8-894a-4932-b127-ad93fc85029d)

  - Here, as the credit amt decrease the chances of default increase
  - In other words, when the credit amt is less the chances of payment gettigdefault is more

    ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/ce38c472-73f8-4571-a48b-7148c7497f32)
    
  - This shows strong linear relation of AMT_CREDIT and AMT_GOODS_PRICE
  - weak relation of AMT_INCOME_TOTAL and AMT_GOODS_PRICE
  - weak relation of AMT_ANNUITY and AMT_GOODS_PRICE
  - weak relation of AMT_INCOME_TOTAL with other 3 columns
    
3) Bivariate Analysis of Application dataset
   
   ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/c2c3f41d-e8c8-485e-9d02-6bbacc6b6322)
   
  - Male have higher amount application for both types of loan i.e. cash loans and revolving loans than females

    ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/63175ae5-e70a-4612-b100-be273cbc0f4d)

  - Defaulter
    - Female academic holders are earning higher amount still there is not a single male defaulter having academic degree
    - In all other cases, male are earning more than female in every single education category
  - Non-Defaulter
    - In non-defaulters, in each of the category of education male are earning more than female
      
4) Analysis of whole dataset(merged dataset)
   
  - Univariate Analysis
    - Numerical Column

      ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/d8b53902-bf32-4fd9-9a0e-a959d1ea92ef)

      - Most of the credited loan amount lies between 30k-1.25 lakhs

      ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/9da10db0-108b-45cb-853c-733ef9a268aa)

      - Mostly clients has asked for the amount in application is for upto50k
    - Categorical Column
      
      ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/2353fb5c-b3c6-4989-ba53-f94868d28fd5)

      - The number of loans taken as cashloansis far more than revolving loans
     
      ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/28a12ce0-180c-4f41-85c3-36e5961ed93c)

      - Most of the customers who has taken loans has income type as worker
     
      ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/caa7261f-65f0-4060-a49c-997e7a67a9c9)

      - Approved loans has higher number than cancelled or refused loans
        
  - Bivariate Analysis
    
    ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/640d790b-b49c-4467-8cee-afcf5a2c452d)

    - Client as unaccompanied type suite has applied loan mostly

    ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/213ca5ba-c2af-4d61-92c6-809fca3a5977)

    - Client as family status married has applied for most of the loans
      
    ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/9afa2334-a860-4efa-ac35-4a163bfbe9c5)

    - In all the above cases/graphs, its clearly visible that females has applied for the more number of loans than male did
      
  - Multivariate Analysis

    ![image](https://github.com/vyanky03/EDA---Credit-Bank-Dataset/assets/99646164/66f447d7-1913-485b-8d6b-628ec7da77b5)

    - AMT_GOODS_PRICE and AMT_CREDIT has shown greater correlation
    - AMT_GOODS_PRICE, AMT_CREDIT and AMT_ANNUITY has weak correlation with AMT_INCOME_TOTAL
    - AMT_ANNUITY with AMT_GOODS_PRICE and AMT_CREDIT has shown moderate correlation with each other



