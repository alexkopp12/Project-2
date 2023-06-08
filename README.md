# Project 2: Crowdfunding


## Project Participants
* Savannah Porter
* Andrew Skorupa
* Mohamed Abou elkhier
* Alex Kopp


## Task Leads:
1. Savannah
2. Alex
3. Andrew
4. Mohamed


## Goals/ Tasks

### 1. Create the Category and Subcategory DataFrames
Extract and transform the crowdfunding.xlsx Excel data to create a category DataFrame that has the following columns:

* A "category_id" column that has entries going sequentially from "cat1" to "catn", where n is the number of unique categories
* A "category" column that contains only the category titles

![image](https://github.com/SavannahWithAnH/Project-2/assets/126124356/164608f9-f52c-4dec-9182-c4d33259af0c)

Export the category DataFrame as category.csv and save it to your GitHub repository.

Extract and transform the crowdfunding.xlsx Excel data to create a subcategory DataFrame that has the following columns:

* A "subcategory_id" column that has entries going sequentially from "subcat1" to "subcatn", where n is the number of unique subcategories
* A "subcategory" column that contains only the subcategory titles

![image](https://github.com/SavannahWithAnH/Project-2/assets/126124356/e8bcfe79-24a1-4dc6-9428-6accb4a0f5d4)

Export the subcategory DataFrame as subcategory.csv and save it to your GitHub repository.


### 2. Create the Campaign DataFrame
Extract and transform the crowdfunding.xlsx Excel data to create a campaign DataFrame has the following columns:

* The "cf_id" column
* The "contact_id" column
* The "company_name" column
* The "blurb" column, renamed to "description"
* The "goal" column, converted to the float data type
* The "pledged" column, converted to the float data type
* The "outcome" column
* The "backers_count" column
* The "country" column
* The "currency" column
* The "launched_at" column, renamed to "launch_date" and with the UTC times converted to the datetime format
* The "deadline" column, renamed to "end_date" and with the UTC times converted to the datetime format
* The "category_id" column, with unique identification numbers matching those in the "category_id" column of the category DataFrame
* The "subcategory_id" column, with the unique identification numbers matching those in the "subcategory_id" column of the subcategory DataFrame

![image](https://github.com/SavannahWithAnH/Project-2/assets/126124356/a41de922-6bb9-41a2-aa76-3710624449e6)

Export the campaign DataFrame as campaign.csv and save it to your GitHub repository.


### 3. Create the Contacts DataFrame
Choose one of the following two options for extracting and transforming the data from the contacts.xlsx Excel data:

* Option 1: Use Python dictionary methods.
* Option 2: Use regular expressions.

If you chose Option 1, complete the following steps:

Import the contacts.xlsx file into a DataFrame.
Iterate through the DataFrame, converting each row to a dictionary.
Iterate through each dictionary, doing the following:
Extract the dictionary values from the keys by using a Python list comprehension.
Add the values for each row to a new list.
Create a new DataFrame that contains the extracted data.
Split each "name" column value into a first and last name, and place each in a new column.
Clean and export the DataFrame as contacts.csv and save it to your GitHub repository.
If you chose Option 2, complete the following steps:

Import the contacts.xlsx file into a DataFrame.
Extract the "contact_id", "name", and "email" columns by using regular expressions.
Create a new DataFrame with the extracted data.
Convert the "contact_id" column to the integer type.
Split each "name" column value into a first and a last name, and place each in a new column.
Clean and then export the DataFrame as contacts.csv and save it to your GitHub repository.

![image](https://github.com/SavannahWithAnH/Project-2/assets/126124356/a1afc0a5-9770-45bd-a881-ab0e6534fff6)


### 4. Create the Crowdfunding Database

* Inspect the four CSV files, and then sketch an ERD of the tables by using QuickDBDLinks to an external site..
* Use the information from the ERD to create a table schema for each CSV file.
  Note: Remember to specify the data types, primary keys, foreign keys, and other constraints.
* Save the database schema as a Postgres file named crowdfunding_db_schema.sql, and save it to your GitHub repository.
* Create a new Postgres database, named crowdfunding_db.
* Using the database schema, create the tables in the correct order to handle the foreign keys.
* Verify the table creation by running a SELECT statement for each table.
* Import each CSV file into its corresponding SQL table.
* Verify that each table has the correct data by running a SELECT statement for each.
