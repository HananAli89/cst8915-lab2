# CST8915 Lab 2: 12-Factor Refactor of the Algonquin Pet Store

**Student Name**: Hanan Ali
**Student ID**: 041153451
**Course**: CST8915 Full-stack Cloud-native Development
**Semester**: Fall 2026

---

## Demo Video

🎥 [Watch Demo Video](https://www.youtube.com/watch?v=YOUR_VIDEO_ID)

---

## Service Repositories

| Service | Repository |
|---|---|
| Order Service (Node.js) | https://github.com/HananAli89/order-service |
| Product Service (Rust) | https://github.com/HananAli89/product-service |
| Store Front (Vue.js) | https://github.com/HananAli89/store-front |

---

Each component runs on its own Azure VM (Ubuntu 24.04):

| VM | Runs | Port | Inbound source (NSG) |
|---|---|---|---|
| rabbitmq-vm | RabbitMQ (backing service) | 5672 (AMQP), 15672 (optional UI) | order-vm public IP / my laptop IP |
| order-vm | order-service | 3000 | my laptop IP |
| product-vm | product-service | 3030 | my laptop IP |
| store-vm | store-front | 8080 | my laptop IP |

SSH (22) on all four VMs is limited to my laptop's IP.

---

## Reflection Questions

### 1. What changes did you make to the order-service and product-service to comply with the Configuration and Backing Services factors?



### 2. Why is it important to use environment variables instead of hard-coding configurations?



### 3. Why is it important to have separate repositories for each microservice?

---

## Challenges and Learnings

---

## Screenshots