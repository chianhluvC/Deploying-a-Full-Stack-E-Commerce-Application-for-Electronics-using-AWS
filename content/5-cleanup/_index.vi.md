+++
title = "Dọn dẹp tài nguyên  "
date = 2025
weight = 5
chapter = false
pre = "<b>5. </b>"
+++

Chúng ta sẽ tiến hành các bước sau để xóa các tài nguyên chúng ta đã tạo trong bài thực hành này.

#### Xóa EC2 instance

Truy cập [giao diện quản trị dịch vụ EC2](https://console.aws.amazon.com/ec2/v2/home)
  + Click **Instances**.
  + Click chọn instance cần xoá
  + Click **Instance state**.
  + Click **Terminate instance**, sau đó click **Terminate** để xác nhận.
  
![Clean](/images/5.clean/001-cleanstep1.png)

![Clean](/images/5.clean/002-cleanstep2.png)

#### Xóa S3 bucket

Truy cập [giao diện quản trị dịch vụ S3](https://s3.console.aws.amazon.com/s3/home)
  + Click chọn S3 bucket chúng ta đã tạo cho bài thực hành.
  + Click **Empty**.
  + Điền **permanently delete**, sau đó click **Empty** để tiến hành xóa object trong bucket.

![Clean](/images/5.clean/003-cleanstep3.png)

![Clean](/images/5.clean/004-cleanstep4.png)

![Clean](/images/5.clean/005-cleanstep5.png)

#### Xóa RDS

1. Truy cập vào [giao diện quản trị dịch vụ RDS](https://console.aws.amazon.com/rds/home)
  + Click chọn vào database cần xoá 
  + Click chọn vào **action**
  + Click **Delete**.

![Clean](/images/5.clean/006-cleanstep6.png)

2. Tại ô confirm, tích xác nhận vào điều khoản dịch vụ
  + Nhập **delete me** để tiến hành xóa các endpoints.
  + Click chọn **Delete** để tiến hành xoá
  
![Clean](/images/5.clean/007-cleanstep7.png)

![Clean](/images/5.clean/008-cleanstep8.png)
