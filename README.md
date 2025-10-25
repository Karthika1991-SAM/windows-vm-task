# Windows VM Creation on AWS

## 📘 Project Description
This project demonstrates how to create a **Windows Virtual Machine (VM)** on **Amazon Web Services (AWS)** using **EC2**, connect to it using **Remote Desktop Protocol (RDP)**, and verify the system details.

---

## 🧰 Tech Stack
- **AWS EC2 (Windows AMI)**
- **AWS CLI**
- **RDP (Remote Desktop Protocol)**
- **Windows PowerShell / Command Prompt**

---

## ⚙️ Steps to Reproduce

### 1️⃣ Create a Windows EC2 Instance
- Log in to the [AWS Management Console](https://aws.amazon.com/console/).
- Navigate to **EC2 → Instances → Launch Instance**.
- Choose **Windows Server AMI** (e.g., Windows Server 2022 Base).
- Select an instance type (e.g., `t3.micro`).
- Configure:

  - Enable **Auto-assign Public IP**
  - Add a **Security Group Rule** to allow **RDP (Port 3389)**.
- Create or select an **existing key pair**.
- Launch the instance.

---

### 2️⃣ Connect to the Instance via RDP
- From the EC2 dashboard, select your instance.
- Click **Connect → RDP client**.
- Download the **RDP file** and **get the Administrator password** (using your key pair).
- Open the RDP file in Windows, enter the credentials, and connect.

---

### 3️⃣ Verify System Info
Once connected:
1. Open **Command Prompt (CMD)**.
2. Run the command:
   ```bash
   systeminfo
