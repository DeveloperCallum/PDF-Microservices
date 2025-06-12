# Problem
PDFs are widely used for extractionRequest storage and data sharing, yet extracting structured information, especially tables, can be **challenging and time-consuming**. Many organisations struggle to retrieve tabular data efficiently for further processing, often relying on manual methods or third-party tools that don't always give enough flexibility or in house tools to complete the extraction.

### Motivation for building this project:
1. **Learn How to Build Microservices** – By designing a modular system that processes PDFs, extracts tables, and serves structured data, I will explore the principles of **service decomposition, scalability, and communication**.
2. **Understand the Technology Choices** – Implementing messaging, REST APIs, and worker queues will give hands-on experience with **asynchronous processing, event-driven architecture**, and the practical trade-offs in system design.

   
# Project Planning
![image](https://github.com/user-attachments/assets/c16095ed-a0df-4354-b6e8-6b138e5e76c6)

![image](https://github.com/user-attachments/assets/71c252f1-958d-43e5-837f-9a8a253c1d15)

![image](https://github.com/user-attachments/assets/66bb2d82-43d4-4bb3-b074-7aad67935814)

## Network Arch
![image](https://github.com/user-attachments/assets/067c915d-8d19-43a9-aba7-55542f880e85)

# Client flow diagram
![image](https://github.com/user-attachments/assets/e0447144-513f-4db6-b518-a69a4bcafd43)

# Communication
<img width="1154" alt="Screenshot 2025-06-12 at 21 55 56" src="https://github.com/user-attachments/assets/caaa936e-4327-43a7-b45a-6afa5905763e" />


---
TODO
- Font-end
- Finish Express Integration; Proxying complete, service is fully working. Need to allow the API to provide status API.
- Change the worker service to allow for processing of pdf to images, also allow nodes to disable specific job types.
- error endpoint for frontend clients.

# How to setup
1. `clean compile install` Main libary, followed by Worker Libary.
2. `clean compile package` Worker-Management-Service and Worker  Service.
3. `docker compose up --build` inside the PDF-Microservices-File-Configurations/Job Service
This will start up the job service.

To start the backend-server,
run `docker compose up --build` inside the PDF-Microservices-Backend-Service.

# Postman documentation
[Go to documentation](https://.postman.co/workspace/PDF-Microservice~cbd44020-3a7a-4ef1-8fb5-64fe1cbd164d/collection/7115964-f555d23a-1981-4ebf-b333-07510ff52cf0?action=share&creator=7115964)
