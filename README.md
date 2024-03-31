Project Title: Sparkify ETL Data Warehouse on Amazon Redshift

Overview:
This project involves building an ETL (Extract, Transform, Load) pipeline to construct a data warehouse on Amazon Redshift for Sparkify, a music streaming startup. The source data is stored in JSON format within S3 buckets and comprises song data (metadata about songs and artists) and log data (simulated app activity logs).

The project includes scripts to create tables, execute the ETL process, and define SQL queries for table manipulation. Additionally, a configuration file is provided to specify cluster and authentication details.

Datasets:

Song data: s3://udacity-dend/song_data
Log data: s3://udacity-dend/log_data
Schema:
The data warehouse schema consists of:

Fact Table: songplays
Dimension Tables: users, songs, artists, time
Project Structure:

create_tables.py: Script to drop and recreate tables.
etl.py: Script to perform ETL operations (extract, transform, load).
sql_queries.py: Contains SQL queries for table creation, data insertion, etc.
dhw.cfg: Configuration file containing cluster, IAM role, and S3 bucket information.
How to Run:

Execute create_tables.py to create database tables.
Run etl.py to perform ETL operations and load data into the Redshift database.
Instructions:

Clone the repository to your local machine.
Ensure you have Python installed.
Install required dependencies (e.g., boto3, psycopg2).
Modify dhw.cfg to include your Redshift cluster and IAM role details.
Run create_tables.py to set up the database tables.
Execute etl.py to perform the ETL process and load data into Redshift.
Additional Notes:

Ensure appropriate permissions and access policies are set for AWS resources.
Monitor Redshift cluster performance during data loading and querying.
Consider optimizing ETL process for efficiency and scalability.
Document any issues encountered and resolutions implemented for future reference.




