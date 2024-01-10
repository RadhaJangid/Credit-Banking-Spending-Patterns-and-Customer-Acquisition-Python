# Credit-Banking-Spending-Patterns-and-Customer-Acquisition

# Features
⚡Python Programming Language<br>
⚡EDA [For insights gathering and analysis]<br>
⚡Pandas [For working with datasets/For analyzing, cleaning, exploring, and manipulating data]<br>
⚡Matplotlib & Seaborn [For answer some business questions in the form of visuals]<br>
⚡Statistics [For calculating  mathematical statistics of numeric data]
    
# TABLE OF CONTENTS
<ul>
    <li><h4>ACKNOWLEDGMENT</h4></li>
</ul>
<ol><li><h4>INTRODUCTION</h4></li>
    <ol type="i">
      <li>About The Project</li>
      <li>Scope</li>
      <li>About the Organization</li>
    </ol>
    <li><h4>DATASET USED</h4></li>
    <ol type="i">
      <li>Customer Acquisition</li>
      <li>Spend</li>
      <li>Repayment</li>
    </ol>
    <li><h4>DATA ANALYTICS PROCESS</h4></li>
    <li><h4>METHODOLOGY</h4></li>
    <ol type="i">
    <li>Objective</li>
    <li>Data Gathering</li>
    <li>Data Cleaning</li>
    <li>Field Level Analysis</li>
        <ol>
            <li>Missing Value Treatement</li>
            <li>Handling Outliers</li>
            <li>Data Type Analysis</li>
        </ol>
    <li>Data Consolidation</li>
        <ol>
            <li>Merging Data</li>
            <li>Defining Relationship In Data</li>
        </ol>
    <li>Data Analysis And Business Insides</li>    
</ol>

# ACKNOWLEDGMENT
<p>There are many people who contributed to my work on this Project. I owe my gratitude to all of 
them who have made this Project possible.</p>
<p> I am grateful to the entire team at <b>Edulyt India</b> for providing necessary facilities and permitting me to carry out this project in the organization. I would especially like to thank <b>Mr. Lalit 
Chaudhary</b> for providing me this wonderful opportunity to work on this project and for their 
continuous guidance and support throughout the project.
</p>

# INTRODUCTION
## About The Project -
## Scope
## About the Organization - 
<p>
    Edulyt India is an early age start-up working towards reducing the Gap between Education & 
Employment, founded in 2015 with a mission to train fresh graduates. Disrupting the education 
management sector mainly focused on the field of Analytics. 
Our core area of working is in Data Analytics for BFSI domain. 
Our team is working on basic AI tools to make the world a better easier place to live. Our core 
expertise lies in making the Graduates industry ready. We are highly skilled and trained in 
delivering training to aspiring Graduates. </p>


# DATASET INFO
<div class="w3-container">
  <table class="w3-table-all w3-card-4">
    <tr>
      <th>COLUMN NAME</th>
      <th>DATA TYPE</th>
      <th>TABLE</th>
      <th>DESCRIPTION</th>
    </tr>
    <tr>
      <td>Sl No:</td>
      <td>integer</td>
      <td>Customer Acqusition</td>
      <td>Count of rows</td>
    </tr>
    <tr>
      <td>Customer</td>
      <td>string</td>
      <td>Customer Acqusition</td>
      <td>Name of Customer</td>
    </tr>
    <tr>
      <td>Age</td>
      <td>decimal</td>
      <td>Customer Acqusition</td>
      <td>Age of Customer</td>
    </tr>
    <tr>
      <td>City</td>
      <td>string</td>
      <td>Customer Acqusition</td>
      <td>Customer's City</td>
    </tr>
    <tr>
        <td>Credit Card Product</td>
        <td>string</td>
        <td>Customer Acqusition</td>
        <td>Types of Credit Cards</td>
    </tr>
    <tr>
        <td>Limit</td>
        <td>integer</td>
        <td>Customer Acqusition</td>
        <td>Credit Card Limit</td>
    </tr>
    <tr>
        <td>Company</td>
        <td>string</td>
        <td>Customer Acqusition</td>
        <td>Name of the Company</td>
    </tr>
    <tr>
        <td>Segment</td>
        <td>string</td>
        <td>Customer Acqusition</td>
        <td>Customer Occupation</td>
    </tr>    
    <tr>
      <td>Sl No:</td>
      <td>integer</td>
      <td>Spend</td>
      <td>Count of rows</td>
    </tr>
    <tr>
      <td>Costomer</td>
      <td>string</td>
      <td>Spend</td>
      <td>Name of Customer</td>
    </tr>
    <tr>
      <td>Month</td>
      <td>date</td></td>
      <td>Spend</td>
      <td>Date</td>
    </tr>
    <tr>
      <td>Type</td>
      <td>string</td>
      <td>Spend</td>
      <td>Types of Expenses</td>
    </tr>
    <tr>
        <td>Amount</td>
        <td>decimal</td>
        <td>Spend</td>
        <td>Spend of Customer</td>
    </tr>
    <tr>
      <td>SL No:</td>
      <td>integer</td>
      <td>Repayment</td>
      <td>Count of rows</td>
    </tr>
    <tr>
      <td>Costomer</td>
      <td>string</td>
      <td>Repayment</td>
      <td>Name of Customer</td>
    </tr>
    <tr>
      <td>Month</td>
      <td>date</td>
      <td>Repayment</td>
      <td>Credit Card Payment Date</td>
    </tr>
    <tr>
        <td>Amount</td>
        <td>decimal</td>
        <td>Repayment</td>
        <td>Credit Card Payment Amount</td>
    </tr>
  </table>
</div>


# DATA ANALYTICS PROCESS
<img src="Data_Analytics_Process.png" alt="Data Analytics Process" width="500" height="400">

# METHODOLOGY
<h2>Loading Dataset</h2> 
<p>In this project we will use “Credit Banking Dataset”.
First, we will load data from an Excel file using the Pandas.ExcelFile() function, the data is available in three worksheets. The names of the worksheets are - 
    <ul>
        <li>Customer Acquisition</li>
        <li>Spend</li>
        <li>Repayment</li>
    </ul>
Then we will read data from different sheets using read_excel() function and store the data in a DataFrame object.</p>

<h2>Basic Data Analysis</h2>
<ul>
    <li>Look at the top/bottom 5 records of data.</li>
    <li>Check various attributes of data like shape (rows and columns), columns, datatype.</li>
    <li>Checking data types of all columns.</li>
    <li>Consize summary of dataframe.</li>
    <li>Check descriptive statistics of numerical variables.</li> 
    <li>Missing data :- Initial intuition</li>
    <li>Data Cleaning
                <ol type = "1">
                    <li>Create a copy of base data for manupulation & processing.</li>
                    <li>Converting the date into year and month columns</li>
                    <li>Rename Costomer column as Customer</li>
                    <li>Invalid / Missing data</li>
                    <li>Invalid value Treatment</li>
                    <li>Feature Binning</li>
                    <li>Remove columns not required for processing.</li>
                </ol>
     </li>
</ul>
<h2>Merging Data</h2>
<ul>
    <li>Merge Customer and Spend , Customer and Repayment</li>
    <li>Merge Customer , Spend, Repayment dataset</li>
</ul>
<h2>EDA(Exploratory data analysis) - Data Exploration</h2>
<ol type="1">
    <li>Plot distibution of individual predictors.
        <ul>
            <li>Univariate Analysis</li>
            <li>Bivariate Analysis</li>
        </ul>
    </li>
    <li>Convert all the categorical variables into dummy variables.</li>
    <li>Build a corelation of all predictors.</li>
</ol>

# ACTIONABLE INSIGHTS
<h4>In this project we have getting the following insights:-</h4>
<ul>
    <li>We have analysed that A13, A22, A39, A40, A41, A42, A45, A48, A60, A61 these are 
        top 10 monthly spenders.</li>
    <li>In the month of January, the spending is high.</li>
    <li>We have analysed that A22, A40, A41, A3, A45, A47, A48, A49, A60, A61 these are 
        top 10 monthly repay customers.</li>
    <li>In the month of January, the repay amount is high.</li>
    <li>Middle-aged customers are more likely to spend.</li>
    <li>About 53 percent of the Amount is being paid by middle-aged customers.</li>
    <li>Customers that having Normal Salary are spending more, followed by Salaried_Pvt and then self- 
        Employed</li>
    <li>Customers that having age 49.29 are spending more.</li>
    <li>Govt is most profitable segment</li>
    <li>A16, A18, A20, A23, A3, A30, A35, A42, A46, A5, A51, A58, A61 these are the 
        customers who spending but not repaying in the month of December.</li>
    <li>Some of the customers who only spend and repayment in the month of January,February, March, April.
        </li>
    <li>2.9% interest is calculated for any due amount of the customer</li>
    <li>Customers who's monthly spend is more than the limit we imposed a 2% of penalty of credit limit.</li>
    <li>Customers whose repayment is more than the spend then we give them a credit of 2% of their credit 
       limit in month billing.</li>
    <li>There are some negative values ​​present in the Monthly_Bank_Profit column. These negative values ​​mean          that the bank has suffered a loss.</li>
    
</ul>




      
 








             

