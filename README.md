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

    student-cloud-storage-001
    │
    ├── Cloud.pdf
    ├── Assignment.docx
    ├── Image.jpg
    └── Notes.pdf

---

### Part B – Launching an Amazon EC2 Instance

* **Step 1:** Type **EC2** in the AWS search bar.
* **Step 2:** Open the EC2 Dashboard.
* **Step 3:** Click **Launch instance**.
* **Step 4:** Enter the instance name: `CloudLabVM`
* **Step 5:** Select the operating system:
  * Amazon Linux 2023
  * Ubuntu Server
* **Step 6:** Select the instance type: `t3.micro`
* **Step 7:** Create a key pair:

| Parameter | Value |
| :--- | :--- |
| Key pair name | `CloudLabKey` |
| Key pair type | RSA |
| File format | `.pem` |

* **Step 8:** Download the `CloudLabKey.pem` file.
* **Step 9:** Configure the network settings:
  * [x] Allow SSH traffic (Port 22)
  * [x] Allow HTTP traffic (Port 80)
  * [x] Allow HTTPS traffic (Port 443)
* **Step 10:** Set the storage size: `8 GiB`
* **Step 11:** Click **Launch instance**.
* **Step 12:** Wait until the status changes:  
  `Pending` ➔ `Running`

---

### Connecting to the EC2 Instance

* **Step 1:** Open EC2.
* **Step 2:** Select the instance.
* **Step 3:** Click **Connect**.
* **Step 4:** Select **EC2 Instance Connect**.
* **Step 5:** Click **Connect**.
* **Step 6:** Execute the following command:

    echo "Hello AWS"

#### Output

    Hello AWS

---

### Stopping the EC2 Instance

* **Step 1:** Open EC2.
* **Step 2:** Select **Instances**.
* **Step 3:** Select the running instance.
* **Step 4:** Click **Instance state**.
* **Step 5:** Click **Stop instance**.

**Status Transition:**  
`Running` ➔ `Stopping` ➔ `Stopped`

---

### Logging Out of AWS

1. Click the profile icon in the upper-right corner.
2. Select **Sign out**.

---



### OUTPUT:

**Bucket Creation:**

<img width="1280" height="634" alt="Screenshot 2026-10-31 100716" src="https://github.com/user-attachments/assets/34401343-7987-4c6b-9d90-08593af6ea6e" />

**Uploading files to the bucket:**

<img width="1280" height="643" alt="Screenshot 2026-10-31 101222" src="https://github.com/user-attachments/assets/51fcbcdc-7936-46fc-9e78-b4b8af7b5345" />

**Launching instance:**

<img width="1280" height="689" alt="Screenshot 2026-10-31 102226" src="https://github.com/user-attachments/assets/0c432bcc-f3c2-42a4-ace0-2c39c9b57839" />

<img width="1280" height="692" alt="Screenshot 2026-10-31 102235" src="https://github.com/user-attachments/assets/857951a9-b4e4-4d4f-b190-308f7b9c1d95" />

**Connecting to the instance and the echo command:**

<img width="1280" height="692" alt="Screenshot 2026-10-31 102505" src="https://github.com/user-attachments/assets/467a2bae-b7ae-49ff-bff2-e29ef1f072ca" />

### Result
The Amazon S3 bucket was created successfully, files were uploaded, an EC2 instance was launched, and the virtual machine was connected successfully.
