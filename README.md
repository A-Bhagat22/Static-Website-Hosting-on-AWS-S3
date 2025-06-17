# Project 01 – Static Website Hosting on AWS S3

This project demonstrates how to host a fully static website using AWS S3. It includes steps like bucket creation, static hosting configuration, public access setup, and uploading HTML/CSS files to host a working frontend website.

---

## 🚀 Tech Stack / Tools Used

- **AWS S3** – For file storage and static hosting
- **IAM** – For setting bucket policy (public access)
- **HTML/CSS/JS** – Frontend code (Neogym template)
- **Git & GitHub** – For version control and project showcase

---

## 📁 Folder Structure
01-s3-static-website-hosting/
├── index.html
├── css/
├── js/
├── images/
├── fonts/
└── README.md


---

## ✅ Steps Performed

1. Created a new S3 bucket with a unique name
2. Enabled **static website hosting**
3. Uploaded all static files (HTML, CSS, JS, images)
4. Added a **bucket policy** to allow public read access
5. Accessed site using the S3 static site URL

---

## 🔗 Live Demo

👉 [Click here to view website](http://neogym-static-site-apoorva.s3-website-us-east-1.amazonaws.com/)

---

## 🧠 What I Learned

- Hosting a frontend-only site using S3 without any server
- Handling static asset folders (css, js, images)
- Managing S3 permissions and bucket policies
- Understanding S3 static website URLs and access rules

---

## 📌 Commands & Notes

- Bucket Policy Used:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::neogym-static-site-apoorva/*"
    }
  ]
}

