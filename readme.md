DevOps Project: Automated CI/CD Pipeline
Objective
Automate the build, test, and deployment process for a simple web application.
Use GitHub Actions for CI/CD, Docker for containerization, and optionally deploy the container to a cloud server.



Deploy to a Cloud Server
Example: Deploy to AWS EC2 with Docker

SSH into your EC2 instance:

bash
ssh -i your-key.pem ec2-user@your-instance-ip

Install Docker:

bash
sudo yum update -y
sudo amazon-linux-extras install docker
sudo service docker start
sudo usermod -a -G docker ec2-user


Pull the Docker image:

bash
docker pull <your-dockerhub-username>/vscode-devops-app:latest


Run the container:


bash
docker run -d -p 80:5000 <your-dockerhub-username>/vscode-devops-app:latest