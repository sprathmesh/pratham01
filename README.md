# pratham01
This is my self information project
DevOps Portfolio Project - Personal Website with Docker and Kubernetes
This project is a personal portfolio website for Prathmesh Shinde, a DevOps & AWS Enthusiast. It showcases Prathmesh's skills, experience, and provides links to his GitHub, LinkedIn, Docker Hub, and downloadable CV.

The website is built using Nginx, containerized with Docker, and deployed in a Kubernetes cluster.

Features
Responsive web design with HTML and CSS.
Nginx serves as the web server inside a Docker container.
Kubernetes configuration for deployment and service management.
Custom NodePort service for external access.
Includes links to social profiles and downloadable CV.
Directory Structure
bash
Copy
Edit


steps:----------------

Docker Setup
Build and Run the Docker Container
bash
Copy
Edit
docker build -t prathmesh-portfolio:latest .
docker run -d -p 8085:80 prathmesh-portfolio
Access the website at http://localhost:8085.

Kubernetes Setup
Apply Deployment and Service
bash
Copy
Edit
kubectl apply -f pratham-deployment.yaml
kubectl apply -f pratham-service.yaml
Port Forwarding for Access on Port 8080
bash
Copy
Edit
kubectl port-forward service/pratham-service 8080:30080
Access the website at http://<Node-IP>:8080.

Technology Stack
Nginx: Web server to serve static content.
Docker: Containerization of the website.
Kubernetes: Deployment and Service management.
HTML/CSS: Frontend development.
Future Improvements
Add a contact form with email integration.
Implement CI/CD pipeline for automated deployment.
Convert the project into a Helm chart for easier deployment.
Connect with Me
GitHub
LinkedIn
Docker Hub
Email Me
License
This project is for educational purposes only. Feel free to use it as a reference.


