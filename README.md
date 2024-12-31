
# 📝 **Scalable Campus Visit Survey Platform: Microservices Architecture on AWS **

This project implements a **Survey Form API** using **Spring Boot**, with deployment on **Kubernetes** managed via **Rancher** and CI/CD using **Jenkins**.

## 📚 **Project Overview**

- **Backend:** Java Spring Boot
- **Database:** AWS RDS MySQL
- **Containerization:** Docker
- **Orchestration:** Kubernetes (via Rancher)
- **CI/CD:** Jenkins

## ⚙️ **Setup & Deployment Steps**

### **1. Spring Boot API Setup**
- Endpoints:
   - `GET /api/surveys` – Fetch all surveys
   - `GET /api/surveys/{id}` – Fetch survey by ID
   - `POST /api/surveys` – Create new survey
   - `PUT /api/surveys/{id}` – Update survey by ID
   - `DELETE /api/surveys/{id}` – Delete survey by ID

### **2. Build & Push Docker Image**
```bash
docker build -t survey-backend:v1 .
docker tag survey-backend:v1 your-dockerhub-username/survey-backend:latest
docker push your-dockerhub-username/survey-backend:latest
```

### **3. Kubernetes Cluster Setup via Rancher**
- Setup Rancher on AWS EC2
- Deploy 3 replica pods using Rancher UI

### **4. CI/CD Pipeline using Jenkins**
- Automated builds and deployment triggered on `git push`

## 🧩 **Architecture Overview**
- Java Spring Boot Backend
- AWS RDS MySQL Database
- Docker Containerization
- Kubernetes Cluster Managed via Rancher
- CI/CD with Jenkins

## 📜 **Documentation**
For detailed steps, refer to the full documentation: [SWE645_HW3_Report](SWE645_HW3_Report.pdf)


## 🤝 **Contributing**
Feel free to fork this repository and submit pull requests.
