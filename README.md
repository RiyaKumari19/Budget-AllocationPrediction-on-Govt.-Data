# Budget-AllocationPrediction-on-Govt.-Data

**SARVA SHIKSHA ABHIYAAN EXPLORATORY DATA ANALYSIS PROJECT**




#**CONTENTS**

#**1.INTRODUCTION**

1.1-->DESCRIPTION

1.2--> ABBREVIATION USED


#**2.DATASET**

2.1-->SOURCE LINK

2.2-->DATA DESCRIPTION


#**3.DATA UNDERSTANDING**

3.1-->IMPORTING THE RELEVANT LIBRARY

3.2-->IMPORTING DATASET

3.3-->READING COLUMNS IN THE DATASETS

3.4-->RENAMING ALL COLUMN NAMES

3.5-->COPYING DATA TO ssa DATAFRAME FROM ssa_df

3.6-->DATA INFORMATION

3.7-->DATASET SHAPE

3.8-->DESCRIPTIVE ANALYSIS

#**4.DATA CLEANING**

**PART A: MISSING VALUE(INTERPRETING NUMERICALLLY)**

4.1-->CHECKING FOR MISSING VALUES

4.2-->CHECKING MISSING PERCENTAGE

4.3-->REASON FOR MISSING 100% DATA

4.4-->DROPPING ROWS/COLUMNS

**PART B: VISUALIZING THE MISSING VALUES(INTERPRETING GRAPHICALLY)**

4.5--> Visualize missing values as a matrix

**PART C:DEALING WITH MISSING VALUES**

4.6--> DROP/DELETE MISSING VALUES

4.7--> PRINTING ALL ROWS WITH NULL VALUES

**PART D:REASONS AND IMPUTING NULL VALUES**

4.8--> REASON AND IMPUTING MISSING VALUE OF released_funds_in_state

4.9--> REASON AND IMPUTING MISSING VALUE OF of total_funds

4.10--> REASON AND IMPUTING MISSING VALUE OF funds_released_against_budgetapproved

4.11--> DISPLAYING VALUES AFTER COMPUTING

4.12--> CHECKING AGAIN TOTAL NUMBER OF NULL VALUES

#**5.DATA VISUALIZATION**

5.1-->BUBBLE CHART

5.2-->HEATMAP

5.3-->STACKED BAR CHART

5.4-->DYNAMIC DASHBOARD
      (POWER BI)
#**6.DATA PREDICTION**

**PART 1:**

6.1-->FINDING CORRELATION

6.2-->PREPROCESSING DATA FOR MODELING

**PART B:MACHINE LEARNING MODELING**

6.3-->OBJECTIVES

6.4-->RESULT

#**1. INTRODUCTION**
**1.1 DESCRIPTION**

The EDA project in Sarva Shiksha Abhiyan financial data involves analyzing historical budget allocation and expenditure data to identify patterns and trends. Using this analysis, a predictive model is developed to estimate the budget allocation for the next year.

**1.2 ABBREVIATION USED**

1. SMA - SARVA SHIKSHA ABHIYAN

2. ssa_df =DATAFRAME NAME FROM INDEX 3.2 TO 3.4

3. ssa - DATAFRAME NAME

**2.1 SOURCE LINK**
Data source - https://openbudgetsindia.org/dataset/sarva-shiksha-abhiyan-ssa-2015-16-to-2017-18
**2.2 DATA DESCRIPTION**

-->Overall narrative summary of data:-

i)There are total 999 observation in our ssa dataset.

ii)There are total 26 variable in our dataset.

iii)In our final dataset we have found only 108 rows and 11 variables are usefull other rows and columns are null.

iv)Below is the Data type of variables:-
  
    0   State --> object
    
    1   State_UT_Code --> float64
    
    2   Financial Year --> object
    
    3   Budget Approved --> float64
    
    4   Funds Released by the Government of India -->  float64
    
    5   Funds Released by the States/UTs  --> float64
    
    6   Total Funds Released (Government of India and States' Share) --> float64

    7   Expenditure Incurred by the States/UTs  --> float64
    
    8   Unspent Balance --> float64
    
    9   Extent of Funds Released against Budget Approved --> float64
    
    10  Extent of Funds Utilised against Budget Approved --> float64t

v)The Sarva Shiksha Abhiyan (SSA) dataset contains information on the budget, funds released, expenditure, and utilization of funds for elementary education in India. The dataset includes the following variables:

    State: A categorical variable indicating the state in India for which the data is reported.

    State_UT_Code: A numerical code for the state/UT (Union Territory).

    Financial Year: The year for which the budget and expenditure data are reported.

    Budget Approved: The budget approved for the SSA program in the given financial year.

    Funds Released by the Government of India: The funds released by the central government for the SSA program in the given financial year.

    Funds Released by the States/UTs: The funds released by the state/UT government for the SSA program in the given financial year.

    Total Funds Released (Government of India and States' Share): The total funds released for the SSA program in the given financial year.

    Expenditure Incurred by the States/UTs: The expenditure incurred by the state/UT government for the SSA program in the given financial year.

    Unspent Balance: The unspent balance of the funds released for the SSA program in the given financial year.

    Extent of Funds Released against Budget Approved(%): The extent to which the funds released for the SSA program match the budget approved for the given financial year.

    Extent of Funds Utilised against Budget Approved(%): The extent to which the funds utilized for the SSA program match the budget approved for the given financial year.


The SSA program aims to provide universal access to primary education in India and to improve the quality of education. This dataset can be used to analyze the implementation and effectiveness of the program in different states/UTs of India

