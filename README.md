# Deploying 2048 Game with Docker on AWS Elastic Beanstalk

## Introduction
This README provides instructions on how to deploy the 2048 game using Docker containers and AWS (Amazon Web Services) Elastic Beanstalk. The 2048 game is a popular web-based game where players slide numbered tiles on a grid to combine them and create a tile with the number 2048.

## Prerequisites
Before proceeding, ensure you have the following:
- An AWS account
- Docker installed on your local machine

## Getting Started
1. Clone the GitHub repository containing the 2048 game source code:
   ```bash
   git clone https://github.com/gabrielecirulli/2048.git
2. Navigate to the project directory:
   ```bash
   cd 2048
3. Create a Dockerfile
4. Build the Docker Image:
   ```bash
   docker build -t 2048-game .
5. Run the Docker container:
   ```bash
   docker run -d -p 80:80 2048-game
6. Access the game in your browser by visting http://localhost

## Deploying to AWS Elastic Beanstalk
1. Open the AWS Management Console and navigate to Elastic Beanstalk.
2. Click on "Create Application" and provide a name for your application (e.g., "2048-game").
3. Choose "Docker" as the platform.
4. Upload your Dockerfile and other necessary files.
5. Configure additional settings as needed (e.g., environment variables, instance type).
6. Click on "Create Application" to deploy your game to AWS Elastic Beanstalk.
7. Once the deployment is complete, access your game using the provided URL.

## Cleaning Up
After you have finished testing or showcasing the game, make sure to clean up your resources to avoid incurring unnecessary charges. Delete the application and environment from AWS Elastic Beanstalk.

## Conclusion
Congratulations! You have successfully deployed the 2048 game using Docker containers and AWS Elastic Beanstalk.
