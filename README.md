# AWS-Banking-Solution
This CloudFormation project deploys a banking app on AWS, utilizing S3 for data, Lambda for logic, API Gateway for APIs, RDS for databases, and DynamoDB for NoSQL storage. It's parameterized for flexibility, offering a scalable and secure financial platform.
Project Description:

The provided CloudFormation code represents a banking application built on Amazon Web Services (AWS) infrastructure, aiming to deliver a secure and scalable financial platform. This cloud-native application leverages multiple AWS services to ensure efficient functionality.

Key Components:

Amazon S3 Bucket (bankingS3bucket): This AWS S3 bucket serves as the data store for the banking application. It's used to manage and store banking-related data, such as account balances and transaction history.

AWS Lambda Function (Lambdafunction): The Lambda function is the core backend logic of the application. It interacts with the S3 bucket to retrieve banking data and responds to API requests. Written in Python, it converts data formats and handles data retrieval efficiently.

Amazon API Gateway (bankingRESTAPI): The API Gateway enables the creation of RESTful APIs, exposing the banking functionalities to external applications or users. It serves as the entry point for interacting with the application.

AWS Identity and Access Management (IAM) Role (LambdaExecutionRole): This IAM role is assumed by the Lambda function, allowing it to access AWS resources securely. It's granted permissions to interact with the S3 bucket and execute necessary actions.

Amazon RDS Database (RDSInstance): The RDS instance provides relational database storage. It's configured to support structured data storage, retrieval, and management. Currently configured for MySQL, it can be adapted for other database engines.

Amazon DynamoDB Table (DynamoDBTable): DynamoDB is utilized to store unstructured or semi-structured data, offering flexibility for various application needs.

AWS API Gateway Deployment (APIDeployment): This resource manages the deployment of the API Gateway. It allows you to create different stages for your API, such as development, testing, and production.

AWS Lambda Permission (LambdaInvokePermission): This permission allows the API Gateway to invoke the Lambda function securely.

Parameterized Configuration:

The CloudFormation template incorporates parameterized configuration, enabling customization during deployment. Users can specify parameters such as S3 bucket name, Lambda runtime, API stage, and more, making the application flexible and adaptable to different use cases.

Overall, "BankingApp-AWS" is a cloud-native banking application that harnesses AWS services to deliver secure, scalable, and customizable financial services, from data storage and retrieval to API-driven interactions. It showcases the power of cloud computing in modernizing traditional financial systems.
