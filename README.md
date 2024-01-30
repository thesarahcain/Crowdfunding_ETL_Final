# Project 2

### Background
## 
For the ETL mini project, you will work with a partner to practice building an ETL pipeline using Python, Pandas, and either Python dictionary methods or regular expressions to extract and transform the data. 
After you transform the data, you'll create four CSV files and use the CSV file data to create an ERD and a table schema. Finally, you’ll upload the CSV file data into a Postgres database.
Since this is a one-week project, make sure that you have done at least half of your project before the third day of class to stay on track.
Although you and your partner will divide the work, it’s essential to collaborate and communicate while working on different parts of the project. Be sure to check in with your partner regularly and offer support.

### Create the Category and Subcategory DataFrames
## 
Extract and transform the crowdfunding.xlsx Excel data to create a category DataFrame that has the following columns:
- "category_id" column that has entries going sequentially from "cat1" to "catn", where n is the number of unique categories
- "category" column that contains only the category titles
The following image shows this category DataFrame:

(replace with our screenshot of chart) 

Extract and transform the crowdfunding.xlsx Excel data to create a subcategory DataFrame that has the following columns:
- "subcategory_id" column that has entries going sequentially from "subcat1" to "subcatn", where n is the number of unique subcategories
- "subcategory" column that contains only the subcategory titles
The following image shows this subcategory DataFrame:

(replace with our image when done) 

### Create the Campaign DataFrame
## 
Extract and transform the crowdfunding.xlsx Excel data to create a campaign DataFrame has the following columns:
- The "cf_id" column
- The "contact_id" column
- The "company_name" column
- The "blurb" column, renamed to "description"
- The "goal" column, converted to the float data type
- The "pledged" column, converted to the float data type
- The "outcome" column
- The "backers_count" column
- The "country" column
- The "currency" column
- The "launched_at" column, renamed to "launch_date" and with the UTC times converted to the datetime format
- The "deadline" column, renamed to "end_date" and with the UTC times converted to the datetime format
- The "category_id" column, with unique identification numbers matching those in the "category_id" column of the category DataFrame
- The "subcategory_id" column, with the unique identification numbers matching those in the "subcategory_id" column of the subcategory DataFrame
  The following image shows this campaign DataFrame:
(insert our image when done)

### Create the Contacts DataFrame
## 
Choose one of the following two options for extracting and transforming the data from the contacts.xlsx Excel data:

Option 1: Use Python dictionary methods.

Option 2: Use regular expressions
##!!!!!!!!!!!!!!!!!!!!!!!! SIDE NOTE: UPDATE AND FINISH INSTRUCTIONS HERE DEPENDING ON THE OPTION YOU CHOOSE!!!!!!!!!!!!!!!!!!!!!!!!!!!

### Create the Crowdfunding DataBase
## 
- Inspect the four CSV files, and then sketch an ERD of the tables by using QuickDBDLinks to an external site..
- Use the information from the ERD to create a table schema for each CSV file.
- Note: Remember to specify the data types, primary keys, foreign keys, and other constraints.
- Save the database schema as a Postgres file named crowdfunding_db_schema.sql, and save it to your GitHub repository.
- Create a new Postgres database, named crowdfunding_db.
- Using the database schema, create the tables in the correct order to handle the foreign keys.
- Verify the table creation by running a SELECT statement for each table.
- Import each CSV file into its corresponding SQL table.
- Verify that each table has the correct data by running a SELECT statement for each.

### References 
## 
Below are URL addresses of websites that were referenced when writing this code: 
