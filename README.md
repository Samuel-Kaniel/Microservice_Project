# 🛠 Microservice_Project

## 📌 Project Overview

### 🤖 Clients:
- **Client **: Represents an external user or system interacting with our platform via the global web.

### 🌐 Internet:
- Represents the vast network of interconnected computers. Client engages with our services through this.

### 🚪 API Gateway:
- Positioned as the bridge between external requests and internal services.
- Serves as the primary access point, routing requests to the right destinations.
- 🔒 Employs OAuth2.0 for authentication, ensuring that incoming requests are both authenticated and permitted.

### ⚖ Load Balancer:
- Distributes incoming traffic across services to guarantee even load and optimal utilization of resources.

### 🧩 Microservices:
- **Payment-Service**: Manages all things related to payments.
- **Order-Service**: Overlooks order handling and processing.
- **Product-Service**: Maintains products and associated features.

### 🗃 Database:
- Each microservice has its dedicated database to ensure data integrity and separation.
  - Payment-Service uses a database symbolized by a 🍃 MongoDB.
  - Order-Service integrates with a database marked by a 🐘.
  - Product-Service employs a MySQL database.

### 🐳 Docker & Infrastructure:
- **Private Docker Registry**: A hub for storing and handling custom Docker images.
- **Pull Images**: Illustrates the process of extracting Docker images.
- **Eureka Server**: Assists microservices in registering and finding one another.
- **Microservices Register As Client**: Signifies the microservices registering themselves.
- **Config Server**: Supervises external properties across multiple settings.
- **Pull Environment Configuration**: Services retrieve essential configurations.

### 🔍 Monitoring & Tracing:
- **Sleuth**: Useful for tracking requests to ascertain their route and response times.
- **Distributed Tracing with Zipkin**: Gathers and displays traces over multiple services.

---

**🏛 Architecture Insight**: 
The architecture demonstrates how clients interact with microservices through an API Gateway. The services are containerized, likely leveraging Docker, and each communicates with its designated database. The design also emphasizes critical components like a private Docker registry, a microservices register, a configuration server, and a distributed tracing mechanism.

---

