# Experiment No. 2

## CLOUD STORAGE CREATION (S3) AND LAUNCHING AN EC2 INSTANCE IN AWS

### Aim
To create an Amazon S3 (Simple Storage Service) bucket for cloud storage and launch a virtual machine using Amazon EC2 (Elastic Compute Cloud) in the AWS Management Console.

---

### Objectives
After completing this experiment, students will be able to:
* Understand AWS Cloud Storage (Amazon S3).
* Create and manage S3 buckets.
* Upload and organize files in cloud storage.
* Launch an EC2 virtual server.
* Connect to an EC2 instance.
* Understand cloud computing infrastructure services.

---

### Software Requirements
* Laptop/Desktop
* Internet Connection
* AWS Academy Learner Account / AWS Free Tier Account
* Modern Web Browser (Chrome/Edge)

---

### Theory

#### Amazon S3 (Simple Storage Service)
Amazon S3 is an object storage service provided by AWS that stores unlimited amounts of data with high durability and availability.

**Features:**
* Unlimited Storage
* 99.999999999% (11 9's) durability
* High Availability
* Secure Storage
* Versioning
* Lifecycle Management
* Encryption

---

### Part A – Creating an Amazon S3 Bucket

* **Step 1:** Open the AWS console.  
  *URL:* `https://aws.amazon.com/console/`
* **Step 2:** Log in using the following method:
  * Click **Sign in using root user email**.
  * Enter the registered email address.
  * Enter the AWS password.
  * Complete the verification process.

#### Output

* **Step 3:** Type **S3** in the search box.
* **Step 4:** Click **Amazon S3**.
* **Step 5:** Click **Create bucket**.
* **Step 6:** Enter the following details:

| Parameter | Value |
| :--- | :--- |
| Bucket type | General purpose |
| Bucket name | `student-cloud-storage-001` |
| AWS Region | Asia Pacific (Mumbai) |

* **Step 7:** Leave the remaining settings unchanged.
* **Step 8:** Click **Create bucket**.
* **Step 9:** Click **Upload**.
* **Step 10:** Upload the following files:
  * PDF file
  * Word document
  * Image file

**Example Structure:**
```text
student-cloud-storage-001
│
├── Cloud.pdf
├── Assignment.docx
├── Image.jpg
└── Notes.pdf
