# Task: S3 Static Website Hosting

## Objective
Host a static website using Amazon S3 by enabling website hosting, uploading HTML files, configuring public access, and enabling versioning.

---

## Steps

### 1. Create S3 Bucket
- Created a new S3 bucket  
- Disabled Block Public Access (required for website hosting)  

---

### 2. Enable Static Website Hosting
- Enabled static website hosting from bucket properties  
- Set index document: `index.html`  

---

### 3. Upload Website Files
- Uploaded HTML file (`index.html`) to the bucket  

---

### 4. Configure Bucket Policy
- Added policy to allow public read access (`s3:GetObject`)  

---

### 5. Enable Versioning
- Enabled versioning from bucket properties  

---

## Output

- S3 bucket created successfully  
- Static website hosting enabled  
- HTML page accessible via S3 website endpoint  
- Public access configured correctly  
- Versioning enabled for object tracking  

---

## Screenshots

![Output](screenshots/image1.png)  
![Output](screenshots/image2.png)