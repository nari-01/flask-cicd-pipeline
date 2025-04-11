##Flask CI/CD Pipeline using Jenkins and Docker

This project demonstrates how to build a **CI/CD pipeline** for a Python Flask application using **Jenkins**, **Docker**, and **GitHub Webhooks**, deployed on an **AWS EC2 instance**.

---

##Tools & Technologies

- Python 3.10
- Flask
- Docker
- Jenkins (on EC2)
- GitHub Webhooks
- AWS EC2 (Ubuntu)

---

##CI/CD Pipeline Flow

1. Code pushed to GitHub
2. GitHub Webhook triggers Jenkins
3. Jenkins:
   - Clones the repo
   - Builds Docker image from `Dockerfile`
   - Removes any existing container
   - Runs a new container exposing the Flask app on port 5001
4. App accessible at:
http://54.177.92.61:5001
