---
title : "Cấu hình EC2 và kết nối tới S3"
date: 2025-05-25 
weight : 2 
chapter : false
pre : " <b> 3.2. </b> "
---


1. Truy cập vào EC2 đã tạo và click copy địa chỉ Public IPv4 address

![ec2deploy](/images/3.deploy/014-ec2-deploy2.png)

2. Mở CMD truy cập vào thư mục chứa keypair EC2 và thực hiện đoạn code sau để SSH tới EC2
  
```cmd
ssh -i "your-keypair.pem" ec2-user@<EC2-PUBLIC-IP>
```

![ec2deploy](/images/3.deploy/017-ec2-deploy5.png)

3. Copy đường dẫn tới file jar đã tải lên ở S3
![ec2deploy](/images/3.deploy/018-ec2-deploy6.png)

4. Cấu hình đường dẫn

![ec2deploy](/images/3.deploy/019-ec2-deploy7.png)


5. Click chọn vào biểu tưởng copy để copy đường dẫn

![ec2deploy](/images/3.deploy/020-ec2-deploy8.png)

6. Nhập lệnh theo đoạn code bên dưới để tiến hành tải file jar từ S3 về EC2

```cmd
pwd 'links3'
```

![ec2deploy](/images/3.deploy/021-ec2-deploy9.png)

7. Đợi đến khi tải xong và sẽ có thông báo hiện thị 100% trên CMD

![ec2deploy](/images/3.deploy/022-ec2-deploy10.png)

8. Nhập lệnh theo đoạn code bên dưới để tiến hành đổi tên file

```cmd
mv 'namefile' newName
ls
```

![ec2deploy](/images/3.deploy/023-ec2-deploy11.png)


9. Tiến hành cài đặt java 22 bằng đoạn lệnh bên dưới

```cmd
sudo yum install java-22
ls
```

![ec2deploy](/images/3.deploy/024-ec2-deploy12.png)

10. Đợi gói java 22 cài đặt vào EC2

![ec2deploy](/images/3.deploy/025-ec2-deploy13.png)


11. Tiến hành các bước sau để chạy ứng dụng web
  + Kiểm tra phiên bản java
  + Chạy ứng dụng
  
 ```cmd
java -version
java -jar DASpring.jar
ls
``` 

![ec2deploy](/images/3.deploy/026-ec2-deploy14.png)

12. Xem các thông tin của ứng dụng đang chạy

![ec2deploy](/images/3.deploy/027-ec2-deploy15.png)

13. Cài đặt thêm port cho inbound rules
   + Click add Rule
   + Click chọn Custom TCP 
   + Nhập port 8080
   + Click chọn Anywhere
   + Click vào Save rules

![ec2deploy](/images/3.deploy/028-ec2-deploy16.png)

 Vậy là bạn đã hoàn tất các bước triển khai ứng dụng E-Commerce Full-Stack chuyên về điện tử bằng AWS. Ở phần kế tiếp chúng ta sẽ thực hiện test web vừa triển khai lên AWS.
