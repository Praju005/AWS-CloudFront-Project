# ☁️ AWS CloudFront Website Project

A **static portfolio website** for my sweet shop, designed using **HTML & CSS**, and securely deployed on **AWS S3 + CloudFront**.  
This project highlights **real-world AWS skills** in static website hosting, CDN distribution, and HTTPS configuration.

---

## 🏗️ AWS Architecture

```plaintext
+-------------------+
|   User Browser    |
+-------------------+
          |
          v
+-------------------+         +-------------------+
|   CloudFront CDN  | <-----> |   AWS Edge Cache  |
| (HTTPS + Caching) |         +-------------------+
+-------------------+
          |
          v
+-------------------+
|   S3 Bucket       |
| (Private Hosting) |
| + OAI/OAC Access  |
+-------------------+

✨ The bucket is **private** – only CloudFront can fetch objects via **Origin Access Identity (OAI)** or **Origin Access Control (OAC)**, ensuring secure access.  

---

## 🚀 Features  

- 🖼️ **Attractive Portfolio** – Hero, Menu, Gallery, and Contact sections  
- 📦 **Hosted on AWS S3** – Reliable static website hosting  
- 🌍 **CloudFront Integration** – Global content delivery + HTTPS  
- 🔒 **Secure Setup** – No public bucket policy, OAI/OAC used  
- 🌐 **Scalable** – Supports custom domains via **Route53 + ACM**  

---

## 🛠️ Tech Stack  

- **Frontend**: HTML, CSS  
- **Hosting**: Amazon S3 (Static Website Hosting)  
- **CDN & HTTPS**: AWS CloudFront with OAI/OAC  
- **Domain Management (Optional)**: Route53  

---

## 📝 Deployment Steps  

### 1️⃣ Create S3 Bucket  
- Name: `sweet05`  
- Keep it **private**  

### 2️⃣ Upload Files  
- Upload `sweet_shop_portfolio.html`  

### 3️⃣ Setup CloudFront  
- Origin: S3 bucket  
- Restrict Bucket Access ✅ Yes  
- Use **OAI/OAC** for security  
- Redirect **HTTP → HTTPS**  

### 4️⃣ Access Website  
- CloudFront URL → `https://dXXXXXXXX.cloudfront.net`  

### 5️⃣ (Optional) Add Custom Domain  
- Configure with **Route53 + SSL Certificate (ACM)**  

---

## 🎯 Learnings from this Project  

✔️ Hosting static websites securely on **AWS S3**  
✔️ Configuring **CloudFront distributions** with OAI/OAC  
✔️ Enabling **HTTPS + caching** for performance  
✔️ Mapping **custom domains** with Route53  

---

## 👨‍💻 Author  

**Prajakta Pandaram**  
📌 *AWS | Cloud Projects  

