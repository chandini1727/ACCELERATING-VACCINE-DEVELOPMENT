# ACCELERATING_VACCINE_DEVELOPMENT
## Project Overview
This project focuses on building a cloud-based data pipeline to support vaccine development teams by enabling efficient data storage, cleaning, transformation, and analytics. Additionally, a static website was developed to facilitate scientific collaboration, data visualization, and virtual meetings for stakeholders.

The pipeline leverages AWS services to process large volumes of vaccine-related data, perform analytics (e.g., efficacy analysis, adverse event monitoring, batch quality control), and provide interactive dashboards for real-time insights. The static website enhances collaboration by offering a user-friendly interface for scientists to view data, conduct meetings, and share findings.
# Video demo 
🙎‍♀️https://drive.google.com/file/d/1iYHnBt3Z46atf1bDoUhp-VRvJV1U00pH/view?usp=drive_link

# Working Process
The project was executed through the following steps:

- **Collaboration with Vaccine Teams:**
Identified critical data types, volumes, and sources through workshops with scientists.
Defined key use cases: efficacy analysis, adverse event monitoring, and batch quality control.
- **Infrastructure Design:**
Designed a scalable AWS data lake using S3 for efficient storage and partitioning.
Ensured compliance with HIPAA and GDPR using AWS tools for encryption, access control, and monitoring.
- **Data Processing:**
Cleaned and transformed data using AWS Glue and stored it in AWS Redshift for high-performance analytics.
Created specialized data marts for focused analysis, such as vaccine efficacy modeling.
- **Visualization:**
Integrated Redshift data marts with Power BI to develop interactive dashboards and reports for real-time insights.
- **Static Website:**
Built a static website for scientific collaboration, enabling data visualization and virtual meetings.

## Implementation
The data pipeline was implemented using AWS services with the following steps:

- **1. Creating S3 Bucket**
Navigated to the S3 console, created a bucket with a suitable name, and configured it for data storage.
- **2. Creating EC2 Instances**
Launched EC2 instances via the EC2 console, selecting appropriate AMIs, instance types, and key pairs for compute resources.
- **3. Data Cleaning with AWS Glue**
Database Creation: Added a database in AWS Glue for organizing data.
Crawler Setup: Configured crawlers to scan S3 data sources and populate the Glue Data Catalog.
- **ETL Job:**
Created an ETL job to remove duplicates and transform data.
Uploaded ETL scripts to S3 and configured job properties (e.g., data sources, transformations, bookmarks).
Ran the job to process and clean data.
- **4. Viewing Cleaned Data**
Accessed the S3 bucket, selected parquet files, and used S3 Select to query cleaned data with SQL.
- **5. Data Analytics and Visualization**
Transformed cleaned data into AWS Redshift for high-performance analytics.
Integrated Redshift with Power BI to create dashboards for vaccine development teams.
- **6. Static Website**
Developed a static website hosted on AWS S3 for scientific collaboration.
Features include data visualization, meeting scheduling, and stakeholder communication.
## Technologies Used
- **1.AWS S3:** Scalable storage for the data lake.
- **2.AWS EC2:** Compute resources for processing tasks.
- **3.AWS Glue:** Data cleaning and ETL processes.
- **4.AWS Redshift:** High-performance data warehousing for analytics.
- **5.Power BI:** Interactive dashboards and real-time reporting.
- **6.HTML/CSS/JavaScript:** Static website for scientific collaboration.
- **7.AWS IAM:** Security and access control for compliance with HIPAA and GDPR.

