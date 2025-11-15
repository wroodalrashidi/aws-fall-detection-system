# 🧠 AWS Fall Detection System

A cloud-based fall detection system built using **AWS Rekognition**, **Lambda**, **S3**, and **SNS**.  
When a video or image is uploaded, the system automatically detects if a fall has occurred and sends an alert via email or SMS.

---

## 🚀 Features
- Automatic fall detection using **Amazon Rekognition**
- Event-driven workflow with **AWS Lambda**
- Notifications via **Amazon SNS**
- Optional logging with **DynamoDB**
- Simple web dashboard hosted on **S3**

---

## 🏗️ Architecture
![Architecture Diagram](architecture/fall-detection-architecture.png)

**Workflow:**
1. A video or image is uploaded to **Amazon S3**
2. **AWS Lambda** is triggered
3. Lambda analyzes the file using **Amazon Rekognition**
4. If a fall is detected → **SNS** sends an alert
5. Logs are optionally saved to **DynamoDB**
6. A web dashboard (on **S3**) shows recent alerts

---

## 🧩 AWS Services Used
- **Amazon S3** – Stores uploaded videos and images  
- **AWS Lambda** – Handles detection logic and triggers  
- **Amazon Rekognition** – Performs image/video analysis  
- **Amazon SNS** – Sends alert notifications  
- **Amazon DynamoDB (optional)** – Saves detection logs  

---

## 🧪 How to Run
1. Upload an image or short video to your S3 bucket.  
2. Wait for Lambda to process the file.  
3. Check your email/SMS for alerts.  

---

## 👥 Team Members
- *Wrood Alrashidi*  
- *Seba Alwosais*

---

## 📄 License
This project is part of the **AWS Cloud Computing Course (Fall 2025)** at Kuwait University.
