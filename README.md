📌 Project Description

This project showcases an end-to-end DevOps implementation of a full-stack application using Docker, Docker Compose, CI/CD, and Nginx. The frontend and backend are containerized with separate Dockerfiles, and MongoDB is configured as the database either directly on the VM or using the official MongoDB Docker image.

The application is deployed on an Ubuntu virtual machine (AWS/Azure) using Docker Compose for multi-container orchestration. A CI/CD pipeline is implemented using GitHub Actions to automatically build Docker images, push them to Docker Hub, and redeploy updated containers whenever changes are pushed to the repository.

Nginx is configured as a reverse proxy to route traffic and expose the complete application through port 80. This project demonstrates containerization, automated deployment, and production-style infrastructure setup in a cloud environment.
