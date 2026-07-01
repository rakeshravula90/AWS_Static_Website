# AWS Static Website Hosting on Amazon S3 with CloudFront

## Project Overview

This project demonstrates how to deploy a static website on **Amazon Web Services (AWS)** using **Amazon S3** for storage and static website hosting, and **Amazon CloudFront** as a Content Delivery Network (CDN) to improve performance and content delivery.

The website consists of static web assets including **HTML**, **CSS**, **JavaScript**, images, and supporting libraries. Since the website does not require any server-side processing or database connectivity, Amazon S3 provides a simple, scalable, and cost-effective hosting solution.

---

## Project Objectives

The primary objectives of this project are:

* Create an Amazon S3 bucket.
* Configure the bucket for Static Website Hosting.
* Upload all website files to the S3 bucket.
* Configure bucket permissions using an IAM-compatible S3 Bucket Policy.
* Create an Amazon CloudFront distribution.
* Access the website through both the S3 Website Endpoint and the CloudFront Distribution URL.
* Demonstrate successful deployment with screenshots.

---

## AWS Services Used

| AWS Service       | Purpose                                            |
| ----------------- | -------------------------------------------------- |
| Amazon S3         | Stores and hosts the static website files          |
| Amazon CloudFront | Delivers website content globally with low latency |
| IAM Bucket Policy | Grants public read access to website objects       |

---

## Technologies Used

* HTML5
* CSS3
* JavaScript
* Bootstrap
* Font Awesome
* jQuery
* Amazon S3
* Amazon CloudFront

---

## Project Folder Structure

```text
AWS_Static_Website/

├── index.html
├── README.md
├── README.txt
│
├── css/
│   └── Website stylesheets
│
├── img/
│   └── Website images
│
├── vendor/
│   ├── bootstrap/
│   ├── jquery/
│   └── fontawesome-free/
│
└── screenshots/
    ├── 01-Bucket-Creation.png
    ├── 02-Permissions-Tab.png
    ├── 03-Uploaded-Files.png
    ├── 04-Static-Website-Hosting.png
    ├── 05-Bucket-Policy.png
    ├── 06-CloudFront-Distribution.png
    └── 07-CloudFront-Website.png
```

---

## Deployment Steps

### Step 1 – Create an Amazon S3 Bucket

* Created a new S3 bucket.
* Selected an AWS Region.
* Configured the bucket for website hosting.
* Disabled Block Public Access as required for public website hosting.

---

### Step 2 – Upload Website Files

Uploaded all project files to the S3 bucket, including:

* HTML
* CSS
* JavaScript
* Images
* Bootstrap libraries
* jQuery
* Font Awesome

---

### Step 3 – Enable Static Website Hosting

Configured:

* Static Website Hosting: **Enabled**
* Index Document: **index.html**

AWS generated a unique S3 Website Endpoint for accessing the website.

---

### Step 4 – Configure Bucket Policy

Applied a Bucket Policy allowing public read access (`s3:GetObject`) to all website files.

This ensures visitors can access the website through the S3 Website Endpoint.

---

### Step 5 – Configure Amazon CloudFront

Created a CloudFront Distribution using the S3 bucket as the origin.

CloudFront provides:

* Faster content delivery
* Reduced latency
* Global edge caching
* HTTPS support

---

### Step 6 – Verify Deployment

Successfully verified that the website is accessible through:

* Amazon S3 Static Website Endpoint
* Amazon CloudFront Distribution URL

---

## Website URLs

### Amazon S3 Website Endpoint

```text
http://YOUR-S3-WEBSITE-ENDPOINT
```

### Amazon CloudFront Distribution URL

```text
https://YOUR-CLOUDFRONT-DOMAIN
```

> Replace the above URLs with your actual S3 Website Endpoint and CloudFront Distribution URL.

---

## Screenshots Included

The repository contains screenshots demonstrating each deployment step:

* Website Files
* S3 Bucket Creation
* Uploaded Files
* Static Website Hosting Configuration
* Bucket Policy
* CloudFront Distribution
* Website Access via CloudFront

---

## Learning Outcomes

Through this project, I gained practical experience in:

* Static website hosting on AWS
* Amazon S3 configuration
* Bucket permissions and policies
* CloudFront CDN configuration
* Website deployment
* AWS Management Console
* Content delivery optimization

---

## Future Improvements

Potential enhancements include:

* Registering a custom domain using Amazon Route 53
* Securing the website with an SSL/TLS certificate using AWS Certificate Manager (ACM)
* Automating deployment using AWS CodePipeline
* Implementing CI/CD workflows with GitHub Actions
* Monitoring website performance using Amazon CloudWatch
