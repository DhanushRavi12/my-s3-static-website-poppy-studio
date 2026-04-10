# 🚀 AWS S3 Static Website Hosting (Poppy Studio)

## 📌 Project Overview
This project demonstrates how to host a static website using AWS S3.  
A real-world HTML template (Poppy Studio) was deployed and made publicly accessible over the internet.

---

## 🔧 Technologies Used
- AWS S3
- HTML, CSS, JavaScript
- Bucket Policy
- Static Website Hosting

---

## ⚙️ Architecture
User → Internet → S3 Bucket → Static Website

---

## 🚀 Steps Performed

### 1️⃣ Created S3 Bucket
- Bucket name: `my-static-website-poppy-studio`
- Region: ap-south-1
- Disabled Block Public Access

### 2️⃣ Uploaded Website Files
- index.html  
- CSS & JavaScript files  
- images folder  

### 3️⃣ Enabled Static Website Hosting
- Enabled static hosting  
- Index document: index.html  

### 4️⃣ Configured Bucket Policy
- Allowed public read access using policy  

---

## 🔐 Bucket Policy

To make the website publicly accessible, the following policy was applied:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Principal": "*",
      "Action": [
        "s3:GetObject"
      ],
      "Resource": "arn:aws:s3:::my-static-website-poppy-studio/*"
    }
  ]
}




## 👨‍💻 Author

**Dhanush R**  
🚀 AWS & DevOps Enthusiast  

📧 r.dhanushravii1202@gmail.com  
📞 +91 9080414681  

🔗 LinkedIn: https://www.linkedin.com/in/dhanush-ravi-934784232/  
💻 GitHub: https://github.com/DhanushRavi12
