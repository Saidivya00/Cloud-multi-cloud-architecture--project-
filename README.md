# 🌐 Multi-Cloud Architecture Project – AWS & GCP Integration

This project showcases the design and implementation of a **multi-cloud architecture** that distributes services across two major cloud providers — **Amazon Web Services (AWS)** and **Google Cloud Platform (GCP)**. It focuses on building interoperability, improving fault tolerance, and demonstrating platform-agnostic cloud deployment.

---

## 🎯 Objective

To design a multi-cloud system where services run on both AWS and GCP, communicate securely, and operate seamlessly together. The setup demonstrates cross-cloud communication, monitoring, and failover capabilities.

---

## 🛠️ Tools & Services Used

### ☁️ AWS:
- **EC2** – Host REST API Server  
- **RDS (MySQL)** – Primary Database  
- **CloudWatch** – Monitoring and Alerts  

### ☁️ GCP:
- **Cloud Functions** – Trigger on request  
- **Cloud Storage** – Store processed assets  
- **Pub/Sub** – Messaging between services  
- **Cloud Monitoring** – Metrics and Logs  

---
---

## 🔄 Interoperability Overview

| Feature               | AWS                          | GCP                         |
|----------------------|-------------------------------|------------------------------|
| Backend Service      | EC2 (Node.js)                 | Cloud Functions (Python)     |
| Messaging Layer      | API Calls (HTTPS)             | Pub/Sub                      |
| Data Storage         | RDS                           | GCP Storage                  |
| Monitoring           | AWS CloudWatch                | GCP Monitoring               |
| Communication Method | HTTPS, JSON Payloads          | Triggered Event Handler      |

---

## 🚀 Demo Walkthrough

1. **AWS EC2** hosts a Node.js API that processes user input.  
2. On submission, it sends an HTTP request to a **GCP Cloud Function**.  
3. The Cloud Function handles the request and publishes a message to **GCP Pub/Sub**.  
4. A secondary function subscribes to the topic and stores results in **Google Cloud Storage**.  
5. Both clouds are monitored using their native tools to log and alert on performance metrics.

---

## 📦 Deliverables

- ✅ Cloud resources deployed across AWS and GCP  
- ✅ Verified communication between services  
- ✅ Live monitoring dashboards on both platforms  
- ✅ Storage and message pipeline working across cloud providers  
- ✅ A working demo and this documentation

---

## 📌 Conclusion

This multi-cloud setup proves that services can be reliably distributed across platforms, ensuring **redundancy**, **platform independence**, and **resilience**. The project demonstrates practical implementation of modern cloud strategies used by enterprises for scalability and failover.

---

