# PROJECT 1

# ☁️ Cloud-Based Static Website Deployment Using AWS

This project consists of building and deploying a personal static website (portfolio) using core AWS services, with a focus on scalability, global availability, and low cost.

## 📌 Project Overview

- **Goal**: Host a personal website on the cloud using secure and modern infrastructure.
- **Type**: Static Website
- **Cloud Provider**: AWS
- **Infrastructure as Code**: No
- **Deployment**: Manual (via file upload to S3)

---

## 🔧 Services and Technologies Used

| Service                           | Purpose                                            |
| --------------------------------- | -------------------------------------------------- |
| **Amazon S3**                     | Storage and hosting of static site files           |
| **AWS CloudFront**                | Content delivery using global CDN with low latency |
| **AWS Route 53**                  | DNS management with custom domain                  |
| **AWS Certificate Manager (ACM)** | SSL certificate creation for HTTPS via CloudFront  |
| **IAM**                           | Access and permission management for AWS services  |

---

## 🌐 Solution Architecture

```plaintext
User
  ↓
CloudFront (HTTPS with SSL)
  ↓
S3 Bucket (HTML/CSS files)
  ↘
Route 53 (Custom domain management)
```

---

## 🔒 Security and Best Practices

- S3 bucket policy allows only controlled public read access.
- HTTPS enabled using a free ACM certificate.
- Direct access to the S3 bucket is blocked—content served only through CloudFront.
- Project follows AWS recommended practices for static website hosting.

---

## 🚀 Deployment Steps

1. Creat an S3 bucket named after the domain and configure for static website hosting.
2. Upload static website files (HTML and CSS).
3. Creat a CloudFront distribution pointing to the S3 bucket.
4. Generate an SSL certificate in ACM for your custom domain.
5. Set up a hosted zone in Route 53 and route traffic to the CloudFront distribution.
6. Test the website using the custom HTTPS domain.

---

## 📎 Live Website

🌐 [vivaldosantana.com](https://vivaldosantana.com)

---

## 🧠 Lessons Learned

- How to configure S3 for static website hosting
- Integrating S3 with CloudFront for global delivery
- Using ACM for secure HTTPS access
- Managing DNS with Route 53
- Applying AWS security and permission best practices

---

## 📫 Contact

- GitHub: [github.com/vivaldosantanawebdev](https://github.com/vivaldosantanawebdev)
- LinkedIn: [linkedin.com/in/vivaldo-santana](https://www.linkedin.com/in/vivaldo-santana/)
