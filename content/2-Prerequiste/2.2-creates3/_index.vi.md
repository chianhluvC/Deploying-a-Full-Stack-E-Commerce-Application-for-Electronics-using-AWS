---
title : "Tạo S3"
date: 2025-05-25 
weight : 2 
chapter : false
pre : " <b> 2.2 </b> "
---

### Tạo S3

Trong bước này chúng ta sẽ tiến hành tạo S3. Đây là bước chuẩn bị cho phần triển khai file jar của source code lên S3, chúng ta sẽ gặp ở phần tiếp theo

1. Truy cập vào [giao diện quản trị dịch vụ S3](https://console.aws.amazon.com/s3/home)
2. Click vào  **Create bucket**.  

![s3](/images/2.prerequisite/011-s3-step1.png)

3. Ở mục Bucket type chúng ta sẽ chọn các cấu hình như sau
  + Click chọn General purpose.
  + Đặt tên Bucket name là **mySpringbootApp**.

![s3](/images/2.prerequisite/012-s3-step2.png)

4. Ở các mục Bucket Versioning click chọn **Disable** và mục Default encryption chọn **Server-side encryption with Amazon S3 managed keys (SSE-S3)**

![s3](/images/2.prerequisite/013-s3-step3.png)

5. Kéo xuống tới đoạn Bucket Key
  + Click chọn Enable.
  + Sau đó click chọn Create Bucket.

![s3](/images/2.prerequisite/014-s3-step4.png)

6. Sau khi tạo xong sẽ hiện kết quả như hình bên dưới

![s3](/images/2.prerequisite/015-s3-step5.png)


Tiếp theo chúng ta sẽ thực hiện tạo và cấu hình RDS.