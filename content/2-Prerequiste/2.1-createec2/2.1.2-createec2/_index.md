---
title: "Create EC2"
date: 2025-05-25
weight: 2
chapter: false
pre: " <b> 2.1.2 </b> "
---

#### Create EC2

1. Go to the [EC2 Management Console](https://console.aws.amazon.com/ec2/home)  
   - Click **Instances**  
   - Click **Launch instances**

![EC2](/images/2.prerequisite/003-createec2.png)

2. On the **Launch instance** page:  
   - Under **Name and tags**, enter the EC2 name as **MyElectronicShop**  
   - In the **Application and OS Images (Amazon Machine Image)** section, choose **Amazon Linux** under Quick Start

![EC2](/images/2.prerequisite/004-selectoptionec2.png)

3. Scroll to the **Amazon Machine Image (AMI)** section, and select  
   **Amazon Linux 2023 kernel-6.1 AMI**

![EC2](/images/2.prerequisite/005-selectoptionec2step1.png)

4. Scroll to the **Key pair (login)** section and click **Create new key pair**  
   - Enter the Key pair name as **ElectronicShopKeypairEC2**  
   - Choose Key pair type: **RSA**  
   - Choose Private key file format: **.pem**  
   - Click **Create key pair**

![EC2](/images/2.prerequisite/006-selectoptionec2step2.png)

5. Scroll to the **Network settings** section and configure as follows:  
   - Click **Create security group** under **Firewall (security groups)**  
   - Choose **Allow SSH traffic from**  
   - For **Allow SSH traffic from**, select **Anywhere**  
   - Click **Launch instance**

![EC2](/images/2.prerequisite/007-selectoptionec2step3.png)

6. After successfully launching the instance, go back to the **Instances** section:  
   - You will see the **Instance state** as `running`  
   - Click on the **Instance ID** to view detailed information about the created EC2

![EC2](/images/2.prerequisite/008-selectoptionec2step4.png)

![EC2](/images/2.prerequisite/009-selectoptionec2step5.png)

7. Scroll down to the **Security** tab to view details about **Inbound rules** and **Outbound rules**

![EC2](/images/2.prerequisite/010-selectoptionec2step6.png)
