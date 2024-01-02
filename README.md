# ETL-Testing-


# ELT Testing Tutorial

![ELT Testing Tutorial](https://static.javatpoint.com/tutorial/etl-testing/images/etl-testing.jpg)

ELT Testing tutorial provides basic and advanced concepts of ELT Testing. Our ELT Testing tutorial is designed for beginners and professionals.

ETL tools extract the data from all the different data sources, transforms the data and (after applying joining fields, calculations, removing incorrect data fields etc.) and loads it into a data warehouse.

ETL testing is done to ensure that the data has been loaded from a source to destination after business transformation is accurate. It also involves the verification of data at various stages that used between source and destination

![ELT Testing Tutorial](https://static.javatpoint.com/tutorial/etl-testing/images/etl-testing2.png)

## ETL (Extraction, Transformation and Loading) Testing

ETL testing is done before data is moved to production data warehouse systems. It is also called as table balancing or product reconciliation. ETL testing is different from Database testing in terms of its scope and the steps followed during this testing.

ETL testing is to ensure that the data which has been loaded from a source to destination after transformation is accurate. It involves the verification of data at various stages, which is used between source and destination.

![ETL Testing Introduction](https://static.javatpoint.com/tutorial/etl-testing/images/etl-testing-introduction.png)

## Process for ETL testing

Like other testing process, ETL testing also go through some testing processes.

![ETL Testing Introduction](https://static.javatpoint.com/tutorial/etl-testing/images/etl-testing-introduction2.png)

ETL testing performed in five stages.

1. ETL testing identifies data sources and requirements.
2. Data recovery
3. Implement dimensional modeling and business logic.
4. Build and populate data
5. Build reports

## Types of ETL testing

The types of ETL testing are:

**1. New Data Warehouse Testing:** It is built and verified from the core. In this testing, the input is taken from the customer's requirement and different data sources. However, the new data warehouse is built and verified with the help of ETL tools.

**Here are the responsibilities which are played by different groups:**

- **Business Analyst:** Business Analyst gathers and documents the requirements.
- **Infrastructure People:** These people set up the test environment.
- **QA Testers:** QA Testers develop test plans and test scripts and then execute these test plan and scripts.
- **Developers:** Developers perform the unit test for each module.
- **Database Administrator:** Database Administrator test for the performance and also for the stress.
- **Users:** Users do functional testing, which includes UAT (User Acceptance Testing).

**2. Production Validation Testing:** This testing is done on data when data is moved to production systems. Informatica Data Validation option provides the automation of ETL testing and management capabilities to ensure that the data do not compromise production systems.

**3. Source to Target Testing (Validation):** This type of testing is done to validate the data values transformed the expected data values.

**4. Application Upgrade:** This type of ETL testing is automatically generated, which saves the test development time. This type of testing checks the extracted data from an older application are precisely same as the data in a new application.

**5. Metadata Testing:** Metadata testing includes the measurement of types of data, length of data, and check index/constraint.

**6. Data Accuracy Testing:** This testing is done to ensure that the data is accurately loaded and transformed as expected.

**7. Data Transformation Testing:** Data transformation testing done in many cases. It cannot be achieved by writing one source SQL query and comparing the output with the target. Multiple SQL queries need to be run for each row to verify the transformation rules.

**8. Data Quality Testing:** Data Quality Tests includes syntax and reference test. To avoid any error due to date or order number during business process data quality is done. **Syntax tests:** It will report dirty data, based on invalid character, character pattern, incorrect upper or lower case order, etc. **Reference Tests:** It will check the data according to the data model.

**For Example**, Customer ID data quality testing includes number check, date check, precision check, date check, etc.

**9. Incremental ETL Testing:** This testing is done to check the data integrity of old and new data when the new data added. Incremental testing verifies that the system processes correctly even after the insertion and updating the data during an incremental ETL process.

**10. GUI/Navigation Testing:** This testing is done to check the navigation or GUI aspects of the front end reports.

**11. Migration Testing:** In this testing, the customer has an existing data warehouse, and ETL is performing the job. But customers are looking for tools to improve efficiency. It includes these steps:

- **Design and validation tests**
- **Setting up the test environment**
- **Executing the validation test**
- **Reporting the bugs**

**12. Change Requests:** In this case, data added to an existing data warehouse. There might be condition arises where customers require to change the present business rule, or they can integrate new rule.

**13. Report Testing:** The final result of the data warehouse, **reported testing**. Repots should test by validating the data, layout in the report. Reports are an essential resource for creating vital business decisions.

## Tasks performed in ETL Testing

Tasks involved in ETL testing are:

- Understanding of data, used for reporting
- Data Model Reviewing
- Mapping of the source to target
- Checks the data in the source data
- Validation of packages and schema
- In the target system, data verification should be done
- Verification of aggregation rules and data transformation calculation
- Data comparison between the target system and data source
- For the target system, quality and data integrity should be examined.
- Performance testing of data.

## Differences between the ETL and the Database Testing

ETL and database testing involve data validation, but both are not same. ETL testing is usually performed on data in a data warehouse, whereas, database testing is performed on transactional systems. Data comes into the transactional database from different applications.

### Operations performed in ETL Testing

ETL testing involves the following operations:

- Validation of data movement from source to the target system.
- Data count verification in the source and target system.
- ETL testing verifies the transformation, extraction as per requirement and expectation.
- ETL testing verifies if table relations join and keys are preservers during the transformation.

### The operation performed in Database Testing

Database testing focuses on data accuracy, the correctness of data, and valid values.

Database testing performs the following operations:

- Database testing focuses on verification of the column in a table that has valid data values.
- To verify whether the primary or foreign key is maintained, database testing is used.
- Database testing verifies if the data is missing in the column. Here, we check that are there any null values in columns which should have a valid value?
- We verify the accuracy of data in columns.

**For example**, the Number of month's column shouldn't have a value greater than 12.

|Function|ETL Testing|Database Testing|
|---|---|---|
|**Primary Goal**|ETL testing is performed for data extraction, transformation and loading for BI reporting.|Database testing is performed to validate and integrate the data.|
|**Business Need**|ETL testing used for information, forecasting, and analytical reporting.|This testing is used to integrate the data from multiple applications and server impact.|
|**Applicable System**|ETL testing contains historic data that cannot be used in business flow environment.|ETL testing contains the transactional system where the flow of business occurs.|
|**Modeling**|The multidimensional method is used.|ER method is used.|
|**Database Type**|ETL testing is applied to OLAP systems.|Database testing is used in OLTP system.|
|**Data Type**|ETL uses the de-normalized data with fewer joins, more indexes, and aggregations.|The database uses normalized data with joins.|
|**Common Tools**|QuerySurge, Informatica, etc. tools are used.|QTP, Selenium tools are used in database testing.|

## ETL performance Testing

ETL performance testing is used to ensure if an ETL system can handle an expected load of multiple users and transactions. Performance testing involves server-side workload on the ETL system.

### How to perform ETL testing performance?

Here are the following steps which are followed to test the performance of ETL testing:

**Step 1:** Find the load which transformed in production.

**Step 2:** New data will be created of the same load or move it from production data to a local server.

**Step 3:** Now, we will disable the ETL until the required code is generated.

**Step 4:** We will count the needed data from the database table.

**Step 5:** We will note down the last run of ETL and enable the ETL. It will get enough stress to transform the entire load which has created and run it.

**Step 6:** After the completion of ETL, we will count the created data.

**Essential performance that should be noted:**

- Find out the total time taken to transform the load
- Find out the performance that has been improved or dropped.
- We will check if the entire expected load is extracted and transferred.

## Data Accuracy in ETL Testing

In ETL Testing, we focus on data accuracy to ensure whether the data is accurately loaded to the target system as per our expectations.

**Here are the steps which should be followed to perform the data accuracy are:**

**Value Comparison:** In value comparison, we compare the data in the source and target system with minimum or no transformation. ETL testing can be possible by using various ETL tools. For example, Source Qualifier Transformation in Informatica.

Expression Transformation can also be performed in data accuracy testing. Set of operators can be used in SQL statements to check the data accuracy in the source and the target systems.

**Check the columns of critical data:** Critical Data columns can be checked by comparing the distinct values in the source and the target system.

[](https://www.javatpoint.com/etl-testing#)[](https://www.javatpoint.com/etl-testing#)[](https://www.javatpoint.com/etl-testing#)

1. SELECT cust_name, order_id, city, count(*)  FROM customer GROUP BY cust_name, order_id, city;  

## ETL testing in data transformation

It is quite complex to perform the data transformation because it cannot be achieved by writing a single SQL query and comparing the output with the target. To do the ETL testing for Data Transformation, we have to write multiple SQL queries for each row to verify the transformation rules.

To perform the successful ETL testing for data transformation, we have to pick the sufficient and sample data from the source system to apply the transformation rule.

**The significant steps to perform ETL testing for data transformation are:**

**Step 1.** The first step is to create a scenario for input data and the expected results. Now we will validate ETL testing with the business customer. ETL testing is the best approach to gather the requirements during designs and can be used as a part of testing.

**Step 2.** The second step is to create the test data according to the scenario. ETL developer will automate the entire process of populating the datasets with the scenario spreadsheet permit versatility and mobility for the reason that the situation is changed.

**Step 3.** Utilize the data profiling and the results will compare the range and submission of values in each field between the source and the target data.

**Step 4.** We will validate the accurate processing of ETL generated fields. For example, Surrogate keys.

**Step 5.** We will validate the data types within the warehouse that are the same as specified in the data model or design.

**Step 6.** Scenarios of data will be created between tables which test the referential integrity.

**Step 7.** We will validate the parent to child relationship in the data.

**Step 8.** And at the end, we will perform **lookup transformation**. Lookup query should be straight without any data gathering and expected to return only one value as per the source table. We can directly join the lookup table in the source qualifier. If this is not a case, we will write a query which will join the lookup table with the main table in the source and will compare the data in the corresponding column in the target.

## ETL Test Cases

**_The objective of ETL testing is to assure that the loaded data from source to destination after business transformation is accurate._**

ETL testing applies to different tools and databases in the information management industry.

During the ETL testing performance, two documents always used by the ETL tester which are:

**1. ETL mapping sheets:** ETL mapping sheets contain all the information of the source and destination tables, which includes every column and their lookup in the reference table. ETL tester needs to be comfortable with SQL queries as ETL testing may involve writing big queries with multiple joins to validate the data at any stage of ETL. ETL mapping sheets provide significant help when we write queries for data verification.

**2. DB Schema of Source (Target):** It should be kept accessible to verify any detail in mapping sheet.

## ETL Test Scenarios and Test Cases:

|ETL Test Scenario|ETL Test Cases|
|---|---|
|**Mapping doc validation**|We will verify the mapping document whether the ETL information provided or not. Log change should maintain in every mapping doc.|
|**Validation**|- We will validate the target and source table structure with the corresponding mapping doc.<br>- The data type of source and target table should be the same.<br>- Length of the data type of both source and target should be the same.<br>- We will verify the data field type, and formats which are specified.<br>- The length of the source data type should not be less than the length of the target data type.|
|**Constraint Validation**|The constraint should be defined for a specific table as per our expectation.|
|**Data Consistency Issues**|- Data Type and length of a particular attribute may vary in files or tables through the semantic definition.<br>- Misuse of integrity constraint.|
|**Completeness Issues**|- Here, we have to be ensure that all the expected data is loaded into the target table.<br>- In this scenario, record counts will be compared between source and target.<br>- We will check the rejected records.<br>- Data should not be truncated in the column of the truncated table.<br>- Will check the boundary value analysis.<br>- We will compare unique values of critical fields between the data loaded in warehouse and source data.|
|**Correctness Issues**|- This scenario is used to correct the data, which is misspelled or inaccurately recorded.<br>- To correct the data, that is null, non-unique, and out of range.|
|**Transformation**|- This scenario is used to check the transformation.|
|**Data Quality**|- This scenario is used to check the number and validate it.<br>- Data Check: This scenario will follow the date format, and it should be same for all the records.<br>- Precision check<br>- Data check<br>- Null check|
|**Null Validate**|- This scenario will verify the null values, where "Not null" values are specified for a specific column.|
|**Duplicate Check**|- In this scenario, we will check the validation of unique key, primary key, and any other column should be unique as per business requirement having any duplicate rows.<br>- We will check if any duplicate values exist in any column which is extracted from multiple column sources and combine them into one column.<br>- As per the client requirements, we need to ensure that there are no duplicates in a combination of multiple columns with target only.|
|**Date Validation**|- Date values are using many areas in development to know the row creation date.<br>- Identify the existing records as per the ETL development perspective.<br>- Sometimes on the date values, the updates and inserts are generated.|
|**Data Cleanness**|- The unnecessary column should be removed before loading into the staging area.|

## Types of ETL Bugs

  
![ETL Testing Introduction](https://static.javatpoint.com/tutorial/etl-testing/images/etl-test-cases.png)  

|Types of ETL Bugs|Description|
|---|---|
|**User Interface Bugs**|These bugs are related to the Graphical User Interface of an application such as, color, font style, navigation, spelling check, etc.|
|**Input-Output Bugs**|In this type of bug, the application starts taking invalid values, and the valid values are rejected.|
|**Boundary value analysis bug**|These bugs check for the minimum and maximum values.|
|**Calculation Bugs**|Calculation bugs show the mathematical errors, and most of the time the final output is wrong.|
|**Load Condition Bugs**|These types of bugs don't allow multiple users. It does not allow the data which is user accepted.|
|**Race Condition Bugs**|In this kind of bugs, the system will not run properly. It starts crashing or hanging.|
|**Equivalence Class Partitioning bugs**|This type of bug results invalid or invalid types.|
|**Version Control Bugs**|These types of bugs usually occur in Regression Testing and do not give any information on versions.|
|**Hardware Bugs**|In this type of bug, the device will not respond to the application as expected.|
|**Help Source Bugs**|This bug will result as the mistakes in the help documents.|

## Responsibility of ETL tester

ETL tester is responsible for validating the data sources, applying transformation logic, and loading the data in the target table, extraction of data.

The responsibilities of ETL tester are:

**Verify the table in the source system.** It involves the following types of operation:

- Count Check
- Data Type check
- Reconcile records with source data
- Ensure no spam data is loaded
- Remove duplicate data
- Check all the keys are in place

**Apply Transformation Logic**

Transformation logic is applied before loading the data. It involves the following operations:

- Transformation logic is applied before and after checking the record of the count.
- Validation of data flow from the staging area to the intermediate table.
- Check the data threshold validation; for example, the age value should not be more than 100.
- Check the surrogate key

**Data Loading**

Data is loaded from the staging area to the target systems. It involves the following operations:

We will check if the aggregate values and calculated measures loaded in the fact table.

- During the loading of the data, we will check the modeling views based on the target table.
- We will check, if the CDC has been applied to the incremental load table.
- Check the data dimension table and review the history of the table.
- Check the reports of BI which are based on the loaded fact and dimension table as per the expected results.

## Testing of ETL Tools

ETL testers are required to test the test cases and tools as well. It involves the following operations:

- Test the ETL tool and its functions
- Test the ETL Data Warehouse system
- Create, design and execute the test cases and test plan
- Test the flat file data transfer

## Advantages of ETL Testing

Benefits of ETL testing are given below:

1. ETL testing can extract or receive data from any data sources at the same time.
2. ETL can load the data from heterogeneous sources to a single generalized (frequent)\ different target at the same time.
3. ETL can be able to load different types of the goal at the same time.
4. ETL can be able to extract required business data from various sources and can be needed load business data into the different target as the desired format.
5. ETL can perform any data transformation according to the business.

## Disadvantages of ETL Testing

Disadvantages of ETL testing are given below:

1. One of the main disadvantages of ETL testing is that we must be a data-oriented developer or database analyst to use it.
2. When we need a fast response, it is not ideal for real-time or on-demand access.
3. ETL testing will take months to put on any place.
4. It is challenging to keep the data in the changing requirement.

heading:

ETL testers are required to test the test cases and tools as well. It involves the following operation:

- Test the ETL tool and its function
- Test the ETL Data Warehouse system
- Create, design and execute the test cases and test plan
- Test the flat file data transfer
## Production Validation Testing

To perform Analytical Reporting and Analysis, the data in your production should be correct. This testing is done on the data that is moved to the production system. It involves data validation in the production system and comparing it the with the source data.

## Source-to-target Count Testing

This type of testing is done when the tester has less time to perform the testing operation. It involves checking the count of data in the source and the target systems. It doesn’t involve checking the values of data in the target system. It also doesn’t involve if the data is in ascending or descending order after mapping of data.

## Source-to-target Data Testing

In this type of testing, a tester validates data values from the source to the target system. It checks the data values in the source system and the corresponding values in the target system after transformation. This type of testing is time-consuming and is normally performed in financial and banking projects.

## Data Integration / Threshold Value Validation Testing

In this type of testing, a tester validates the range of data. All the threshold values in the target system are checked if they are as per the expected result. It also involves integration of data in the target system from multiple source systems after transformation and loading.

**Example** − Age attribute shouldn’t have a value greater than 100. In the date column DD/MM/YY, the month field shouldn’t have a value greater than 12.

AD

## Application Migration Testing

Application migration testing is normally performed automatically when you move from an old application to a new application system. This testing saves a lot of time. It checks if the data extracted from an old application is same as per the data in the new application system.

AD

## Data Check and Constraint Testing

It includes performing various checks such as data type check, data length check, and index check. Here a Test Engineer performs the following scenarios − Primary Key, Foreign Key, NOT NULL, NULL, and UNIQUE.

AD

## Duplicate Data Check Testing

This testing involves checking for duplicate data in the target system. When there is a huge amount of data in the target system, it is possible that there is duplicate data in the production system that may result in incorrect data in Analytical Reports.

Duplicate values can be checked with SQL statement like −

Select Cust_Id, Cust_NAME, Quantity, COUNT (*) 
FROM Customer
GROUP BY Cust_Id, Cust_NAME, Quantity HAVING COUNT (*) >1;

Duplicate data appears in the target system due to the following reasons −

- If no primary key is defined, then duplicate values may come.
- Due to incorrect mapping or environmental issues.
- Manual errors while transferring data from the source to the target system.

## Data Transformation Testing

Data transformation testing is not performed by running a single SQL statement. It is time-consuming and involves running multiple SQL queries for each row to verify the transformation rules. The tester needs to run SQL queries for each row and then compare the output with the target data.

## Data Quality Testing

Data quality testing involves performing number check, date check, null check, precision check, etc. A tester performs **Syntax Test** to report invalid characters, incorrect upper/lower case order, etc. and **Reference Tests** to check if the data is according to the data model.

## Incremental Testing

Incremental testing is performed to verify if Insert and Update statements are executed as per the expected result. This testing is performed step-by-step with old and new data.

## Regression Testing

When we make changes to data transformation and aggregation rules to add new functionality which also helps the tester to find new errors, it is called Regression Testing. The bugs in data that that comes in regression testing are called Regression.

## Retesting

When you run the tests after fixing the codes, it is called retesting.

## System Integration Testing

System integration testing involves testing the components of a system individually and later integrating the modules. There are three ways a system integration can be done: top-down, bottom-up, and hybrid.

## Navigation Testing

Navigation testing is also known as testing the front-end of the system. It involves enduser point of view testing by checking all the aspects of the front-end report − includes data in various fields, calculation and aggregates, etc.
