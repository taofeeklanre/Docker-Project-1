## Project-4: Host a Dynamic Website on AWS Platform with Docker, ECR, and ECS
Welcome to this project, where we dive into the world of containerization and orchestration on AWS. This project guides you through leveraging Docker, Amazon Elastic Container Registry (ECR), and Amazon Elastic Container Service (ECS) to host a dynamic website. By containerizing your application and deploying it on ECS, you'll achieve scalability, reliability, and ease of management. Join us on this journey to unlock the power of containerized deployments on AWS!

## Project Structure

Part 1: Pre-requisites / Requirements

Part 2: Create Project Infrastructure in AWS, Docker, Dockerfile, Docker Image, and Others

Part 3: Create Application Load Balancer, ACM, ECS, Record Set in Route 53, and Others

Cleanup

Contributing

License

Contact

Project Overview

### Introduction
What is Docker and Containerization?
Docker is a powerful tool used for containerization, which serves as a lightweight alternative to full machine virtualization. Containers allow you to package an application along with its dependencies into a standardized unit for software development. This ensures that the application runs consistently across different computing environments.

## Why Use Docker and Containers for Hosting a Website?

1. Deploying a website on a traditional EC2 instance involves managing various dependencies, libraries, and configurations, which can be complex and error-prone. Docker containers encapsulate your application and its environment, making it portable and easy to deploy. Benefits of using containers include:

2. Consistency: Ensures applications run the same way across different environments, reducing compatibility issues.
   
3. Isolation: Each container operates independently, preventing changes or issues in one container from affecting others.
   
4. Resource Efficiency: Containers share the host OS kernel, reducing overhead and improving resource utilization compared to traditional virtual machines.
   
5. By leveraging Docker, ECS, and ECR, you can simplify the deployment process, improve scalability, and enhance the overall management of your dynamic website on AWS.


## Objectives
Building on our previous series, "PROJECT-2: Hosting a Dynamic Website on AWS-LAMP Stack Framework," this project explores the use of Docker containers, ECS, and ECR to streamline deployment, improve scalability, and enhance management of dynamic websites on AWS. These technologies offer greater flexibility, allowing developers to package applications and dependencies into lightweight, portable containers that can be easily deployed and managed in the AWS cloud.

By the end of this project, you will have a comprehensive understanding of how to leverage Docker, ECS, and ECR to build and deploy dynamic websites on AWS efficiently.

### Part 1: Pre-requisites / Requirements

Before you begin, ensure you have the following:

1. GitHub Account: Sign up for a free GitHub account.
2. SSH Key Pairs: Generate SSH key pairs for secure access.
3. Git Installation: Install Git on your computer. Download Git
4. Visual Studio Code: Install Visual Studio Code for code editing.
5. Docker Hub Account: Create a Docker Hub account.
6. Virtualization Enabled: Ensure virtualization is enabled on your computer.
7. Docker Installation: Download and install Docker on your computer.

#### Part 2: Create Project Infrastructure in AWS, Docker, Dockerfile, Docker Image, and Others
1. Building a Three-Tier AWS Network VPC from Scratch

2. Set up a Virtual Private Cloud (VPC) with public, private, and database subnets.
   
3. Create NAT Gateways

4. Configure NAT Gateways for internet access in private subnets.

5. Create Security Groups in AWS

6. Define security groups to control inbound and outbound traffic.

7. Set Up MySQL RDS Instance in AWS

8. Launch a MySQL database instance using Amazon RDS.

9. Create EC2 Instance Connect Endpoint
## Architecture Reference Diagram
![Project Endpoint]


10. Configure EC2 instance connectivity.

12. Register a New Domain Name in Route 53

13. Use Amazon Route 53 to register and manage your domain.

14. Create Repository to Store the Application Codes

15. Initialize a Git repository for your application code.

16. Add the Application Code to the GitHub Repository

17. Push your application code to GitHub.

18. Create a Repository to Store the Dockerfile

19. Set up a separate repository for Docker configuration.

20. Create a Personal Access Token

21. Generate a GitHub personal access token for authentication.

22. Create a Dockerfile for the Project

23. Write a Dockerfile to define your application's Docker image.

24. Add Build Arguments and Environment Variables to the Dockerfile

25. Configure build arguments and environment variables for flexibility.

26. Create a Script to Build the Docker Image

27. Develop a build script to automate Docker image creation.

28. Make the Script Executable

29. Modify script permissions to make it executable.

30. Build the Docker Image

31. Execute the build script to create your Docker image.

32. Install the AWS Command Line CLI

33. Install the AWS CLI for AWS operations.

34. Create an IAM User with Programmatic Access

35. Set up an IAM user with necessary permissions for AWS services.

36. Run the AWS Configure Command

37. Configure AWS CLI with your IAM credentials using aws configure.

38. Create a Repository in Amazon ECR with AWS CLI

39. Use AWS CLI to create an ECR repository for storing Docker images.

40. Push the Docker Image to the Amazon ECR Repository

41. Authenticate Docker to ECR and push your image.

42. Migrate Database File (Rentzone MySQL)

43. Import your MySQL database into the RDS instance.

### Part 3: Create Application Load Balancer, ACM, ECS, Record Set in Route 53, and Others
1. Creating an Application Load Balancer

2. Set up an Application Load Balancer to distribute traffic.

3. Registering for an SSL Certificate in Amazon Certificate Manager

4. Obtain an SSL certificate for secure HTTPS connections.

5. Creating an HTTPS Listener for the Application Load Balancer

6. Configure the load balancer to handle HTTPS traffic.

7. Adding Environment Variables to a File

8. Manage configuration through environment variables.

9. Creating an S3 Bucket to Store the Environment File

10. Use Amazon S3 to store and manage environment configuration files.

11. Creating an IAM Role for the ECS Task Definition

12. Define IAM roles for ECS tasks to access AWS resources securely.

13. Creating an ECS Cluster

14. Launch an ECS cluster to manage containerized applications.

15. Creating a Task Definition

16. Define how your Docker containers should run within ECS.

17. Creating an ECS Service

18. Deploy and manage your containers using ECS services.

19. Creating a Record Set in Route 53

20. Configure DNS settings to route traffic to your load balancer.

## Cleaning Up Your ECS Project

Remove resources to avoid unnecessary charges.
After completing the setup and deployment steps, your dynamic website will be accessible via the domain you registered. The website is hosted on AWS using Docker containers managed by ECS, ensuring scalability and reliability.

To access your website:

Open your web browser.
Navigate to your registered domain name (e.g., www.yourdomain.com).
Verify that the website is loading correctly and functions as expected.

Cleanup
To avoid incurring charges for the AWS resources used in this project, follow these cleanup steps:

Delete ECS Services and Clusters

Remove ECS services and clusters via the AWS Management Console.
Delete ECR Repositories

Remove Docker images and ECR repositories.
Terminate EC2 Instances

Stop and terminate any EC2 instances created.
Delete RDS Instances

Delete the MySQL RDS instance if no longer needed.
Remove S3 Buckets

Delete S3 buckets used for storing environment files.
Delete Load Balancers and SSL Certificates

Remove Application Load Balancers and associated SSL certificates.
Delete VPC and Related Networking Components

Remove the VPC, subnets, NAT gateways, and security groups.
Remove Domain Registration

If you no longer need the domain, delete it from Route 53.
Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

How to Contribute
Fork the repository.
Create a new branch (git checkout -b feature/YourFeature).
Commit your changes (git commit -m 'Add some feature').
Push to the branch (git push origin feature/YourFeature).
Open a pull request.
License
This project is licensed under the MIT License.

Contact
For any questions or inquiries, please contact:

Your Name
Email: your.email@example.com
GitHub: your-github-username
Happy deploying! 🚀
