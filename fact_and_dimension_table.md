# Table Defination 
All tables listed below are created in snowflake.


### STG_SUPERSTORE_SALES_DATA (Staging Area/Table)
```

create or replace TABLE STG_SUPERSTORE_SALES_DATA (
	ROW_ID NUMBER(38,0) NOT NULL,
	ORDER_ID VARCHAR(20) NOT NULL,
	ORDER_DATE DATE NOT NULL,
	SHIP_DATE DATE NOT NULL,
	SHIP_MODE VARCHAR(255) NOT NULL,
	CUSTOMER_ID VARCHAR(255) NOT NULL,
	CUSTOMER_NAME VARCHAR(255) NOT NULL,
	SEGMENT VARCHAR(255) NOT NULL,
	COUNTRY VARCHAR(255) NOT NULL,
	CITY VARCHAR(255) NOT NULL,
	STATE VARCHAR(255) NOT NULL,
	POSTAL_CODE NUMBER(38,0) NOT NULL,
	REGION VARCHAR(255) NOT NULL,
	PRODUCT_ID VARCHAR(255) NOT NULL,
	CATEGORY VARCHAR(255) NOT NULL,
	SUB_CATEGORY VARCHAR(255) NOT NULL,
	PRODUCT_NAME VARCHAR(255) NOT NULL,
	SALES FLOAT NOT NULL,
	QUANTITY NUMBER(38,0) NOT NULL,
	DISCOUNT FLOAT NOT NULL,
	PROFIT FLOAT NOT NULL,
	primary key (ROW_ID)
);

```
### FACT_SALES (Fact Table)

```
create or replace TABLE FACT_SALES (
	ROW_ID NUMBER(38,0) NOT NULL,
	DATE_ID NUMBER(38,0),
	LOCATION_ID NUMBER(38,0),
	ORDER_ID VARCHAR(50),
	SHIP_MODE VARCHAR(50),
	CUSTOMER_ID VARCHAR(50),
	CUSTOMER_NAME VARCHAR(50),
	PRODUCT_ID VARCHAR(50),
	PRODUCT_NAME VARCHAR(255),
	CATEGORY VARCHAR(50),
	SUB_CATEGORY VARCHAR(50),
	SALES FLOAT,
	QUANTITY NUMBER(38,0),
	DISCOUNT FLOAT,
	PROFIT FLOAT,
	SEGMENT VARCHAR(20),
	STATUS NUMBER(30,0),
	primary key (ROW_ID)
);

```
### DIM_DATE (Dimension Table)

```
create or replace TABLE DIM_DATE (
	DATE_ID NUMBER(38,0) NOT NULL,
	ORDER_DATE DATE,
	SHIP_DATE DATE,
	STATUS NUMBER(30,0),
	primary key (DATE_ID)
);

```

### DIM_LOCATION (Dimension Table)
```
create or replace TABLE DIM_LOCATION (
	LOCATION_ID NUMBER(38,0) NOT NULL,
	COUNTRY VARCHAR(50),
	CITY VARCHAR(50),
	STATE VARCHAR(50),
	POSTAL_CODE NUMBER(38,0),
	REGION VARCHAR(10),
	STATUS NUMBER(30,0),
	primary key (LOCATION_ID)
);

```
