# Project – Spring Boot + Terraform + AWS

This project demonstrates basic integration between **Spring Boot**, **Docker**, **Terraform**, and **AWS EC2**.  
The application exposes a single REST endpoint `GET /time` that returns the **current date and time**.  
The infrastructure is provisioned using **Terraform**, which creates an EC2 instance and runs the Docker image published on **Docker Hub**.

---

## Architecture

```text
[User] ---> [AWS EC2] ---> [Docker Container: Spring API]
                     ↑
                 [Terraform]
