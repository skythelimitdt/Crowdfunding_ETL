# Crowdfunding_ETL

ETL Mini Project: [Completed Assignment](https://github.com/skythelimitdt/Crowdfunding_ETL/blob/main/ETL_Mini_Project_AWright_EYildirim.ipynb)

ERD Diagram: ![ERD.png](https://github.com/skythelimitdt/Crowdfunding_ETL/blob/main/ERD.png)


For the ETL mini project, we will work on building an ETL pipeline using Python, Pandas, and either Python dictionary methods or regular expressions to extract and transform the data. We used both Python dictionary method and regular expressions to extract and transform the data. 
After transforming the data, we will create four CSV files and use the CSV file data to create an ERD and a table schema. Finally, we’ll upload the CSV file data into a Postgres database.

# Requirements

# Category DataFrame is Created
- The DataFrame contains a "category_id" column that has entries going sequentially from "cat1" to "catn", where n is the number of unique categories
- The DataFrame has a "category" column that contains only the category titles
- The category DataFrame is exported as **category.csv** - Category CSV File: [category.csv Completed Assignment](https://github.com/skythelimitdt/Crowdfunding_ETL/blob/main/Resources/category.csv)

# Subcategory DataFrame is Created
- The DataFrame contains a "subcategory_id" column that has entries going sequentially from "subcat1" to "subcatn", where n is the number of unique subcategories
- The DataFrame contains a "subcategory" column that contains only the subcategory titles
- The subcategory DataFrame is exported as **subcategory.csv** - Subcategory CSV File: [subcategory.csv Completed Assignment](https://github.com/skythelimitdt/Crowdfunding_ETL/blob/main/Resources/subcategory.csv)

# Campaign DataFrame is Created
- The DataFrame has the following columns:
    - A "cf_id" column
    - A "contact_id" column
    - A "company_name" column
    - A "description" column
    - A "goal" column that is a **float** data type
    - A "pledged" column that is a **float** data type
    - An "outcome" column
    - A "backers_count" column
    - A "country" column
    - A "currency" column
    - A "launch_date" with the UTC times converted to the **datetime** format
    - An "end_date" with the UTC times converted to the **datetime** format
    - A "category_id" column that contains the unique identification numbers matching those in the "category_id" column of the category DataFrame
    - A "subcategory_id" column that contains the unique identification numbers matching those in the "subcategory_id" column of the subcategory DataFrame
- The campaign DataFrame is exported as **campaign.csv** - Campaign CSV File: [subcategory.csv Completed Assignment](https://github.com/skythelimitdt/Crowdfunding_ETL/blob/main/Resources/campaign.csv)


# Contacts DataFrame is Created
- The DataFrame has the following columns:
    - A "contact_id" column
    - A "first_name" column
    - A "last_name" column
    - An "email" column
- The contacts DataFrame is exported as **contacts.csv**

# Crowdfunding Database is Created
- A database schema labeled, **crowdfunding_db_schema.sql** is created - Crowdfunding_db Schema: [crowfunding_db_schema.sql Completed Assignment](https://github.com/skythelimitdt/Crowdfunding_ETL/blob/main/crowfunding_db_schema.sql)
- A **crowdfunding_db** is created using the **crowdfunding_db_schema.sql** file
- The database has the appropriate primary and foreign keys and relationships
- Each CSV file is imported into the appropriate table without errors
- The data from each table is displayed using a **SELECT*** statement
