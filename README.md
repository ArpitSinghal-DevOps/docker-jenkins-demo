# docker-jenkins-demo
Hands-on practices on 25/12/2025 from linode account in Local system. 

🔥 **Project Title
CI/CD Pipeline for Automated Docker Deployment using Jenkins**

🧠 Project Summary (CV ke liye – 2–3 lines)
Designed and implemented an end-to-end CI/CD pipeline using Jenkins and Docker to automatically build and deploy a containerized web application on a Linux server. Integrated GitHub for source control and resolved real-world permission and port-conflict issues during deployment.

🛠️ Tools & Technologies Used
Jenkins (CI/CD Automation)

Docker (Containerization)

Git & GitHub (Version Control)

Linux (Ubuntu on Linode)

Nginx (Web Server)

Bash / Shell Commands

⚙️ Project Architecture (Simple Explainable)
Developer pushes code to GitHub repository

Jenkins pulls the latest code automatically

Jenkins builds Docker image using Dockerfile

Existing container is stopped and removed

New Docker container is deployed on the server

Application is accessible via browser on a custom port

🔁 CI/CD Workflow (Step-by-Step)
Code committed and pushed to GitHub

Jenkins job triggered manually (later extendable to webhook)

Jenkins executes shell commands

Docker image built from Dockerfile

Old container removed safely using || true

New container launched on available port

Website deployed automatically without manual intervention

🧩 Key Features
Automated build and deployment process

Dockerized application for consistent runtime

Jenkins Freestyle Job configuration

Permission handling for Jenkins-Docker integration

Port conflict handling during deployment

Real-world Linux service troubleshooting

🚧 Challenges Faced & Solutions (INTERVIEW GOLD)
Jenkins service startup failure → Resolved by fixing Java version and port conflicts

Docker permission denied error → Solved by adding Jenkins user to Docker group

Port already in use issue → Fixed by changing container port mapping

Container cleanup failure → Handled safely using docker stop || true

📈 Learning Outcomes
Hands-on experience with CI/CD pipelines

Practical understanding of Jenkins architecture

Docker container lifecycle management

Linux user permission and service management

Debugging real production-like issues

DevOps mindset for automation and reliability
