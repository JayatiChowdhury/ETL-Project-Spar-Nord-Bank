Spar Nord Banks have to refill the ATMs when the money goes below a specific threshold limit.This depends on the activity and the area where a particular ATM is located as well as the weather, day of the week, etc.
In this project, Spar Nord Bank is trying to observe the withdrawal behavior and the corresponding dependent factors to optimally manage the refill frequency. Apart from this, some other business insights also have to be drawn from the data.like-
----Top 10 ATMs where most transactions are in the ’inactive’ state
----Number of ATM failures corresponding to the different weather conditions recorded at the time of the transactions
----Top 10 ATMs with the most number of transactions throughout the year
----Number of overall ATM transactions going inactive per month for each month
----Top 10 ATMs with the highest total amount withdrawn throughout the year
----Number of failed ATM transactions across various card types
----Top 10 records with the number of transactions ordered by the ATM_number, ATM_manufacturer, location, weekend_flag and then total_transaction_count, on weekdays and on weekends throughout the year
----Most active day in each ATMs from location "Vejgaard"

The project task was to build a batch ETL pipeline - first, to ingest transactional data from RDS into HDFS (using AWS EC2) via Sqoop; next, to transform the data using PySpark (using AWS EC2) to create relevant dimension and fact tables (Data Mart); next, to upload these tables into AWS S3 buckets; finally, load them from S3 into AWS Redshift tables. Lastly, I performed analytical queries on the loaded data, to answer business questions.
