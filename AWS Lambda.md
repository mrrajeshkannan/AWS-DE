# AWS Lambda – Serverless Compute Service

What is AWS Lambda?
------------------
AWS Lambda is a serverless compute service that lets you run code without provisioning or managing servers. 

It automatically scales based on demand and charges only for execution time.

Lambda executes code in response to events from AWS services like S3, DynamoDB, API Gateway, and Kinesis, making it ideal for event-driven applications.

## Key Features of AWS Lambda:-
<b>Serverless Execution</b> – No need to manage servers or infrastructure.

<b>Event-Driven</b> – Automatically triggers based on AWS service events.

<b>Auto-Scaling</b> – Scales based on incoming requests.

<b>Multi-Language Support</b> – Python, Node.js, Java, Go, .NET, Ruby, etc.

<b>Pay-Per-Use Pricing</b> – Billed for execution time, not idle time.

<b>Seamless AWS Integration</b> – Works with S3, DynamoDB, API Gateway, etc.

<b>Security with IAM</b> – Uses IAM roles to control AWS resource access.


## How AWS Lambda Works
<b>Trigger/Event</b> → AWS service (e.g., S3, API Gateway, DynamoDB) triggers Lambda.

<b>Lambda Function Execution</b> → Runs the uploaded function code.

<b>Automatic Scaling</b> → Handles multiple requests in parallel.

<b>Result Processing</b> → Sends output to another AWS service or API response.
