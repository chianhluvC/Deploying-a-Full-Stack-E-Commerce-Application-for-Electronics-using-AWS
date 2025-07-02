---
title : "Tải source code và đóng gói thành file jar"
date: 2025-05-25 
weight : 4
chapter : false
pre : " <b> 2.4 </b> "
---

### Tải source code và đóng gói thành file jar

Trong bước này chúng ta sẽ tiến hành tải source code và đóng gói thành file jar. Đây là bước chuẩn bị quan trọng cho việc triển khai source code lên S3

1. Truy cập vào [giao diện trang repo github](https://github.com/chianhluvC/LTUDJavaNhom12)
2. Click vào  **Download Zip**.  

![jar](/images/2.prerequisite/031-jar-step1.png)

3. Tải về mở file application.properties tiến hình cấu hình như sau
  
  ```properties
  spring.datasource.url= ----urlRDSdatabase----
  spring.datasource.username= -----yourUsername----
  spring.datasource.password= ----yourPassword-----
  ```
  + Phần url lấy ở database RDS đã tạo trước đó.
  + User và password cũng được tạo lúc ban đầu tạo database RDS.

![jar](/images/2.prerequisite/032-jar-step2.png)

4. Đóng gói thành file jar, tham khảo [đường dẫn sau](https://sarangsurve.medium.com/create-a-jar-file-in-intellij-idea-5c876ca06689) để đóng gói thành file JAR.
  
![jar](/images/2.prerequisite/033-jar-step3.png)


Vậy là chúng ta đã chuẩn bị xong phần tải source code và đóng gói thành file jar , ở bước tiếp theo chúng ta sẽ chuyển qua cấu hình Route53.