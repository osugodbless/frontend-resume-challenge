**CLOUD RESUME CHALLENGE - FRONT_END**

This project is a result of participation in the Cloud Resume Challenge, a structured initiative guiding cloud enthusiasts, developers, sys-admins etc., through the creation of a comprehensive full-stack project utilizing Amazon Web Services (AWS). This challenge offers flexibility, allowing individuals to tailor their journey according to their preferences and interests.

The frontend components of the project are housed within this repository, while the deployed portfolio website can be accessed through the provided link.

**Project Overview:**
The project is hosted on AWS and comprises an S3 bucket and a CloudFront distribution. Within the S3 bucket, essential files such as index.html, CSS, and app.js are stored, with app.js containing JavaScript code responsible for interacting with the API. Access to the S3 bucket is exclusively through the CloudFront distribution, as the bucket is not configured for direct access. Additionally, an Amazon certificate has been procured through the Amazon Certificate Manager to establish a secure connection between the custom domain and the CloudFront distribution.

**Deployment Strategy:**
The project adopts an "infrastructure as code" (IaC) approach, facilitated by AWS CDK (Cloud Development Kit). The repository includes the source code for the CDK application, enabling seamless deployment and management of AWS resources.

**Continuous Integration and Continuous Deployment (CI/CD):**
Automation is integral to the project's development lifecycle. GitHub Actions workflow orchestrates deployment processes by installing dependencies, configuring AWS credentials via OIDC (OpenID Connect), deploying the CDK application, and executing Cypress tests to ensure robustness and reliability.
