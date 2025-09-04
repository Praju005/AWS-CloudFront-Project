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
✨ The bucket is private – only CloudFront can fetch objects via Origin Access Identity (OAI)/Origin Access Control (OAC), ensuring security.

🚀 Features
🖼️ Attractive Portfolio – Hero, Menu, Gallery, and Contact sections

📦 Hosted on AWS S3 – Reliable static website hosting

🌍 CloudFront Integration – Global content delivery + HTTPS

🔒 Secure Setup – No public bucket policy, OAI/OAC used

🌐 Scalable – Can be mapped with a custom domain via Route53

🛠️ Tech Stack
Frontend: HTML, CSS

Hosting: Amazon S3 (Static Website Hosting)

CDN & HTTPS: AWS CloudFront with OAI/OAC

Domain Management (Optional): Route53

📝 Deployment Steps (AWS)
Create S3 Bucket

Name: sweet05

Keep it private

Upload Files

Upload sweet_shop_portfolio.html

Setup CloudFront

Origin: S3 bucket

Restrict Bucket Access: ✅ Yes

Use OAI/OAC for security

Redirect HTTP → HTTPS

Access Website

Use CloudFront URL → https://dXXXXXXXX.cloudfront.net

(Optional) Add Custom Domain

Configure Route53 + SSL certificate via ACM

📂 Project Structure
bash
Copy code
sweet05/
│── sweet_shop_portfolio.html   # Website file
│── README.md                   # Documentation
📸 Screenshots
Homepage

🎯 Learnings from this Project
Hosting static websites securely on AWS S3

Configuring CloudFront distributions with OAI/OAC

Enabling HTTPS and caching for better performance

Mapping custom domains with Route53
----------------
👨‍💻 Author
Prajakta Pandaram








Ask ChatGPT
