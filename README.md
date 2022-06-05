# Data-Engineer-Assignment-BeZen
#### The notebook is about an assignment given by Ben zen and has 4 problems.

**In the data analysis first install the required libraries:**
    
    1. !pip install pandas
    
    2. !pip install numpy
    
    3. !pip install matplotlib
    
    4. !pip install seaborn
    
    5. !pip install regex


**The dataset is present in rar file and to work with this, we can use multiple options:**
    
    1. Extract rar file using external tools like Zip Extracter, UnRAR and RAR viewer etc.
    
    2. Using patool library extract the dataset into yiur system.
    
    3. Use GoogleColab and upload the rar file and then call the csv file from it.

**For this assignment I have used Jupyter Notebook.**

**After reading the csv file into a dataframe using pandas library, we see some basic attributes of the dataset like shape and info.**
**Dataset Link - https://drive.google.com/file/d/1AVg8ENuzzvmBWhzFRUgT1os7E8IO78Tq/view**

**A short descripton of the dataset**

    ● UUID (Primary Key)

    ● Price (String)

    ● Price_unfiltered (String)

    ● Product Type

    ● Category

    ● Level 1 -> This is just a classification of a product.

**Then handeled the missing values in the dataset carefully and properly by assuming that the analysis won't be hindered if I remove the missing data.**

### Problem 1 - Products Without Prices.
**First I cleaned the columns of the data.**
**Then created a new data frame having product types which do ot have price value in the price_string column.**

### Problem 2 - Counts of Products Without and With Prices for each Product Type, Category, and Level 1
**To calculate counts of products without prices I used isnull() and with prices I used notnull().**
**Calculating each category is similar to one another for with and without prices respectively.**
**Created new columns for each required classfication of the data and its price tags.**

### Problem 3 - Format the price and separate it into currency and value column.
**Here The price_string is converted into the required format, e.g  '$81.00'.**
**Assuming that the currency is US Dollars, I've created the currency column with currency as 'USD'.**

### Problem 4 - Categories with Average Price of Product.
**Using groupby method, I created a new dataframe for the aggregated price of product and saved it in currency format.**
