# Super_Store_ETL_Pipeline


## About Project 
This project centres around the efficient handling and transformation of data. Specifically, we're tasked with the comprehensive upload of Superstore data into Snowflake, implementing an ETL pipeline in IICS (Informatica intelligent cloud services) for data refinement, and structuring the data into three fundamental components: location dimension table, date dimension table, and a fact table and developing a user-friendly Power BI dashboard that empowers data visualization and presentation. In an age where data insights drive crucial decision-making, our endeavour serves to provide a streamlined, accessible, and insightful approach to data management. 

## References Used
Download Dataset from below link *Superstore Sales Dataset*
https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting

## Dimension & Fact Table Schema 
![er-diagram](https://github.com/shantanu1905/Super_Store_ETL_Pipeline/assets/59206895/e2d19afc-69e9-49c0-9a64-52fba8b11aa6)

## Table Defination 
View Table defination from below link *Fact & Dimension Tables* <br>
https://github.com/shantanu1905/Super_Store_ETL_Pipeline/blob/main/fact_and_dimension_table.md

## ETL Mappings 
I have created my all ETL mapppings/data pipeline in *informatica intelligent cloud services*, you can use any ELT tool as per your need.

Components used in ETL mapping : 

- **Source:** It is used to define the origin of your data. This could be a flat file, a database table, an API, or any other source from which you want to extract data. 
- **Target:** This component in IICS is responsible for specifying the destination where the transformed data will be loaded. This can be a database table, a flat file, a cloud-based data warehouse, or any other repository. 
- **Lookup Transformation:** It is used to perform lookups on data in your ETL process. It allows you to compare data in the source to data in another reference source, typically using a key field. This is often used to enrich or filter data during transformation.  
- **Expression Transformation:** It is used for performing transformations on data. You can use this component to create calculated fields, apply conditional logic, or perform various data manipulation tasks. It's a versatile tool for modifying data as it passes through the ETL pipeline. 
- **Sequence Generator:** It is often used to generate sequential values in your ETL process. This can be handy for creating surrogate keys or unique identifiers for records as they are loaded into the target system. You can define the starting value, increment, and other properties of the sequence.

### Mapping 1 (Data from Flat file loading to  Staging area)

![Mapping 1](https://github.com/shantanu1905/Super_Store_ETL_Pipeline/assets/59206895/f8bdb280-2be3-41fe-914a-560d1eaee125)




