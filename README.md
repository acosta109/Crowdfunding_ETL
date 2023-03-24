ETL (Extract, Transform, Load) is a process of moving data from one or more sources, transforming it to fit the target schema, and loading it into a destination database or data warehouse. In Python, you can perform ETL using various libraries and tools. 

Extract: The first step is to extract data from the source. You can use various libraries and tools to extract data, such as Pandas, Requests, and Beautiful Soup.  In this case, it was excel files that we extracted the data from.

Transform: Once you have extracted the data, you need to transform it to fit the target schema. You can use libraries like Pandas and NumPy to perform various transformations such as cleaning, filtering, merging, and aggregating data.

Load: Finally, you need to load the transformed data into the destination database or data warehouse. 


In this case, it was excel files that we extracted the data from.  

we extracted data in the following order
1. crowdfunding.xlsx and we transformed the data by making two CSV's named category.csv and subcategory.csv
2. next we copied the crowdfunding.xlsx into a campaign.csv for all data related to the campaign minus the category and sub-category
3. Finally, we went to contacts.xlsx to transform the data from having "contact_id" into having multiple columns of 'contact_id', 'first_name', 'last_name', and 'email'



After we did our ETL, we related all the tables with the name 'crowdfunding_db_schema.sql' and uploaded to postgres SQL under the name "crowdfunding_db" and included SELECT * statements of each table 

![](campaign%20SQL%20query.png)
