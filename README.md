# NodeJS Serverless Chat Application with AWS, Snort, and Splunk Security

Welcome to the NodeJS Serverless Chat Application project! This application leverages various AWS services to create a scalable and secure chat platform. In addition, it incorporates Snort for network intrusion detection and Splunk for monitoring and analysis.

## Overview

This project showcases the integration of the following AWS services:

0. **IAM (Identity and Access Management)**
   - Manages access permissions for AWS services.
   - Policies defined for DynamoDB, Lambda, and Cognito.

1. **AWS Cognito**
   - Handles user signup/authentication with token generation.
   - Tokens used for user identification and API calls through API Gateway.

2. **AWS Lambda**
   - Core functionality for executing API requests triggered by user actions.
   - Integrates with Cognito, API Gateway, and DynamoDB.

3. **API Gateway**
   - Manages API methods (GET and POST) and their responses.
   - Acts as a bridge between the frontend and Lambda functions.

4. **DynamoDB**
   - NoSQL database for quick response times and caching.
   - Securely stores chat data.

5. **CloudFront**
   - Optimizes performance with edge locations.
   - Auto-generates SSL certificates for HTTPS connections.
   - Converts HTTP/2 requests to HTTP/3 for improved speed.
   - Caches and delivers content stored in S3 quickly.

6. **AWS S3**
   - Stores HTML, CSS, Bootstrap, and JavaScript files.
   - Deploys API's JavaScript SDK file.

7. **CloudWatch**
   - Monitors and logs metrics and events in the AWS environment.

8. **EC2 (Elastic Compute Cloud)**
   - Secures the VPC with a Network Intrusion Detection System (NIDS) using Snort.
   - Scans inbound traffic, drops malicious packets, and alerts administrators.

## Security Measures

- **Snort (NIDS) on EC2**
  - Scans inbound traffic for network intrusion detection.
  - Drops malicious packets using predefined rules.
  - Alerts administrators about potential attacks.

- **Splunk**
  - Monitors and analyzes logs for enhanced security intelligence.
  - Provides insights into application and network activities.

## Deployment

1. Configure IAM roles with appropriate policies.
2. Set up Cognito for user authentication and token generation.
3. Implement Lambda functions to handle API requests.
4. Configure API Gateway to manage methods and responses.
5. Set up DynamoDB for efficient and secure chat data storage.
6. Utilize CloudFront for edge optimization, SSL certificate generation, and content caching.
7. Store frontend files in S3, including the deployed API's JavaScript SDK file.
8. Enable CloudWatch for comprehensive monitoring.
9. Deploy an EC2 instance with Snort for network intrusion detection.

## Getting Started

1. Clone this repository:

   ```bash
   git clone https://github.com/Eldrago12/WhisperWave.git
   ```

2. Follow the deployment steps mentioned above.

3. Customize the application as needed.

4. Test and enjoy your secure and scalable serverless chat application!

## Contributors

- Sirshak Dolai (https://github.com/Eldrago12)

## License

This project is licensed under the [MIT License](LICENSE).

Feel free to contribute and improve the project! If you have any questions or suggestions, please open an issue or pull request.
