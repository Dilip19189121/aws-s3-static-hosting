# 🌐 AWS S3 Static Website Hosting

This project demonstrates how to host a static website using **Amazon S3**. It includes a simple HTML landing page, image assets, and documentation to guide deployment.

---

## 📁 Folder Structure

```
├── index.html          # Main webpage
├── Assets/             # Image files used in the site
└── Docs/               # Project summary and setup instructions
```

---

## 🚀 How to Deploy on AWS S3

1. **Create an S3 bucket**  
   - Disable “Block all public access”  
   - Enable static website hosting

2. **Upload project files**  
   - Maintain folder structure (Assets, Docs, etc.)

3. **Set index.html as the entry point**

4. **Apply public-read bucket policy**
   ```json
   {
     "Version": "2012-10-17",
     "Statement": [{
       "Sid": "PublicReadGetObject",
       "Effect": "Allow",
       "Principal": "*",
       "Action": "s3:GetObject",
       "Resource": "arn:aws:s3:::your-bucket-name/*"
     }]
   }
   ```

5. **Access your site**  
   - Use the endpoint URL from the hosting section

---

## 📄 Documentation

Detailed setup instructions and project summary are available in the `Docs/` folder.

---

## 🏷️ Tags

`AWS` `S3` `Static Hosting` `Cloud Deployment` `HTML` `Portfolio Project`

---

## 📌 Author

Built by Palli Dilip — passionate about cloud engineering, automation, and modular documentation.
