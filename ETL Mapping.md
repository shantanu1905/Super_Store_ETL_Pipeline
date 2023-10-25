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

### Mapping 2 (Loading data from staging table to fact & dimension table   )
![mapping 2](https://github.com/shantanu1905/Super_Store_ETL_Pipeline/assets/59206895/31473103-9fd2-41f5-95b4-3002639f64de)
![mapping 2 explaination](https://github.com/shantanu1905/Super_Store_ETL_Pipeline/assets/59206895/953b7f83-da3e-48f2-a668-5f0cb9d1a3bc)

### Actual ETL Mapping created in Informatica Intelligent Cloud Service 
![etl2](https://github.com/shantanu1905/Super_Store_ETL_Pipeline/assets/59206895/f8f845e8-f406-4359-8d26-94f3ce614268)



