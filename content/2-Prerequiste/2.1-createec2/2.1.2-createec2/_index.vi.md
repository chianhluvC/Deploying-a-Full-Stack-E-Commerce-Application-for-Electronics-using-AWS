---
title : "Tạo EC2"
date: 2025-05-25 
weight : 2
chapter : false
pre : " <b> 2.1.2 </b> "
---

#### Tạo EC2

1. Truy cập vào [giao diện quản trị dịch vụ EC2](console.aws.amazon.com/ec2/home)
  + Click **Instances**.
  + Click **Launch instances**.

![EC2](/images/2.prerequisite/003-createec2.png)

2. Tại trang **Launch instance**
  + Tại mục **Name and tags** điền tên của EC2 là **MyElectronicShop**.
  + Click Quick Start chọn **Amazon Linux**.
  
![EC2](/images/2.prerequisite/004-selectoptionec2.png)

3. Kéo xuống đoạn Amazon Machine Image (AMI), click chọn **Amazon Linux 2023 kernel-6.1 AMI**
  
![EC2](/images/2.prerequisite/005-selectoptionec2step1.png)

4. Tiếp tục kéo xuống đoạn Key pair, click chọn **Create new key pair**
  + Điền Key pair name là **ElectronicShopKeypairEC2**.
  + Chọn Key pair type là **RSA**.
  + Chọn Private key file format là .pem.
  + Click Create key pair.

![EC2](/images/2.prerequisite/006-selectoptionec2step2.png)

5. Kéo xuống phần Network settings và cấu hình như sau
  + Click chọn Create security group ở phần **Firewall (security groups)**.
  + Click chọn Allow SSH traffic from.
  + Tuỳ chọn của Allow SSH traffic from là Anywhere.
  + Click chọn Launch instance.
  
![EC2](/images/2.prerequisite/007-selectoptionec2step3.png)

6. Sau khi tạo thành công chúng ta quay lại Instances
  + Sẽ thấy trạng thái Instance state là running.
  + Click vào Instance ID để xem thông số chi tiết EC2 vừa tạo.
  
![EC2](/images/2.prerequisite/008-selectoptionec2step4.png)

![EC2](/images/2.prerequisite/009-selectoptionec2step5.png)

7. Kéo xuống thêm một đoạn click vào mục Security, để xem các thông số về Inbound rules và Outbound rules.

![EC2](/images/2.prerequisite/010-selectoptionec2step6.png)


