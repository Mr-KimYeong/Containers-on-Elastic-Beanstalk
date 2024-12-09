Docker and AWS Elastic Beanstalk Project
Project Overview
This project demonstrates the use of Docker for containerizing applications and deploying them on AWS Elastic Beanstalk. The project covers various aspects of Docker, including containerization, creating custom Docker images, and deploying applications to the cloud.

What is Docker?
Docker is a platform for containerizing applications, ensuring consistent environments. It isolates applications, making them portable, lightweight, and efficient. In this project, Docker was used to containerize, build, and deploy an application on AWS.

What is AWS Elastic Beanstalk?
AWS Elastic Beanstalk is a service that simplifies the deployment of cloud applications by managing the underlying infrastructure. Users can upload their code, and Elastic Beanstalk handles everything needed to get it running.

Key Steps and Learnings
Understanding Containers and Docker
Containers are packages that contain an application and all its dependencies, ensuring consistent and portable environments.

A container image is a blueprint for containers, providing instructions on what to include, such as application code, libraries, and dependencies.

Docker lets you run containers, making it easy for engineers to build, test, and deploy applications.

Running an Nginx Image
Nginx is a web server used for handling web traffic smoothly and efficiently.

Command used: docker run -d -p 80:80 nginx

Creating a Custom Image
The Dockerfile contains the set of instructions needed to build a Docker image.

Example Dockerfile:

Dockerfile
FROM nginx:latest
COPY index.html /usr/share/nginx/html/
EXPOSE 80
Command used to build the custom image: docker build -t my-web-app .

Running My Custom Image
Encountered an error when port 80 was already occupied by nginx.

Resolved by stopping the container using the port.

Deploying on Elastic Beanstalk
AWS Elastic Beanstalk makes it easy to deploy cloud applications without managing infrastructure.

Deploying the custom image on Elastic Beanstalk took 6 minutes.

Key Insights
One unexpected aspect was how smoothly the integration between Docker and AWS services worked, despite the complexity of the deployment.

Project Duration
This project took approximately 3 hours to complete.

Tools and Technologies Used
Docker

AWS Elastic Beanstalk

Nginx

GitHub

Contact
Email: kimtheoyeongwhang@gmail.com

GitHub: Mr-KimYeong
