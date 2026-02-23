# 🐦 Birds Gallery Website using Amazon S3 & CloudFront

## 📌 Topic Overview
This project demonstrates how to host a static website using **Amazon S3** and deliver it securely and globally using **Amazon CloudFront**.  
The website displays bird images through an HTML page while following AWS best practices such as keeping the S3 bucket private and serving content through a CDN.

This project is suitable for beginners learning **AWS storage, CDN, and cloud security fundamentals**.

---

## 🛠️ Technologies Used
- **Amazon S3** – Object storage for HTML and image files  
- **Amazon CloudFront** – Content Delivery Network (CDN)  
- **HTML & CSS** – Static website design  
- **Origin Access Control (OAC)** – Secure access between CloudFront and S3  
- **GitHub** – Source code version control  

---

## Architecture
User → CloudFront → Private S3 Bucket


## Features
- Secure public access
- CDN caching
- AWS Free Tier friendly



🔐 Security Best Practices

- S3 bucket is NOT public
- Only CloudFront can read objects from S3
- HTTPS enabled via CloudFront


💰 Cost Considerations

- Uses AWS Free Tier
- Pay-as-you-go model
- No cost for small traffic



## ⚙️ Project Steps

### 1️⃣ Create S3 Bucket
- Created a private Amazon S3 bucket  
- Uploaded the following files:
  - `birds.html`
  - `peacock.jpg`
  - `jpgparrots.jpg`
- Enabled **Block Public Access**

### 2️⃣ Configure CloudFront
- Created a CloudFront distribution  
- Set the S3 bucket as the origin  
- Enabled **Origin Access Control (OAC)**  
- Updated the S3 bucket policy to allow access **only from CloudFront**

### 3️⃣ Access the Website
- Website accessed using the CloudFront URL:

https://<cloudfront-domain>/birds.html



