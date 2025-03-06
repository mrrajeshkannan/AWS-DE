AWS S3 (SIMPLE STORAGE SERVICE)
-------------------------------
Amazon S3 (Simple Storage Service) is a key component in modern data engineering workflows, offering scalable, durable, and cost-effective storage. 

1️⃣ Data Engineering & ETL Pipelines.

2️⃣ Big Data Analytics & Machine Learning.

3️⃣ Application Development & Hosting.

4️⃣ Security & Compliance.

📌 Real-World Example: Data Pipeline Using S3:-
-----------------------------------------------
1️⃣ Raw Data Collection: API data is stored in s3://raw-data-bucket/.

2️⃣ ETL Processing: AWS Glue processes and transforms the data.

3️⃣ Processed Data Storage: Data is saved in s3://processed-data-bucket/ in Parquet format.

4️⃣ Analytics & Querying:


Athena queries the processed data.
Snowflake or Redshift ingests the data for reporting.



1. How to create a bucket in S3.
2. How to upload a file in S3.
3. How to enable versioning in S3.
4. How to access S3 bucket file.


## 1. How to create a bucket in S3.
1️⃣ Using AWS Management Console
Steps:
Sign in to the AWS Management Console.

Navigate to S3 service.

Click on "Create bucket".

Enter a Bucket name (must be globally unique).

Select an AWS Region (choose the closest for better performance).

Block Public Access (Recommended: Keep all public access blocked unless needed).

Choose Bucket Versioning (Enable if you want to track object versions).

Encryption (Optional): Choose between SSE-S3, SSE-KMS, or SSE-C.

Click Create bucket.

✅ Your S3 bucket is now created!


## Questions :- 

Question 1:-   S3 is global service but why do we require region selection?

    Ans:Because for low latency and faster performance

Question 2:- S3 CAn we upload 10 TB data at once it allows unlimited data?

    Ans: No at a time it will accept upto 5 TB data we can saprate into parts.

Question 3 : - How many Bucket we can create in 1 aws account ?

    Ans: 100 bucket we can create if we want more we have to raice ticket to AWS.



