---
title : "Tạo RDS"
date: 2025-05-25 
weight : 3
chapter : false
pre : " <b> 2.3 </b> "
---

### Tạo RDS

Trong bước này chúng ta sẽ tiến hành tạo RDS. Đây là bước chuẩn bị khá là quan trọng cho việc triển khai dữ liệu lên RDS ở các phần phía sắp tới

1. Truy cập vào [giao diện quản trị dịch vụ RDS](https://console.aws.amazon.com/rds/home)
2. Click vào  **Databases**.  

![rds](/images/2.prerequisite/016-rds-step1.png)

3. Giao diện quản trị dịch vụ RDS sẽ xuất hiện, click vào **Create database**

![rds](/images/2.prerequisite/017-rds-step2.png)

4. Giao diện Create database sẽ xuất hiện
  + Phần Choose a database creation method click vào **Standard create**.
  + Phần Engine options click vào **MySQL**.
  
![rds](/images/2.prerequisite/018-rds-step3.png)

5. Kéo xuống thêm một đoạn 
  + Phần Templates click chọn Free tier.
  + Phần Availability and durability sẽ được tự động chọn là Single-AZ DB instance deployment (1 instance).

![rds](/images/2.prerequisite/019-rds-step4.png)

6. Tiếp tục kéo xuống một đoạn
  + Ở phần DB instance identifier nhập tên database của bạn.
  + Master username nhập là **admin**.
  + Ở phần Credentials management click chọn Self managed.

![rds](/images/2.prerequisite/020-rds-step5.png)

7. Tiếp tục kéo xuống thêm một đoạn
  + Nhập **Master password**.
  + Nhập **Confirm master password**.
  
![rds](/images/2.prerequisite/021-rds-step6.png)

8. Tiếp tục kéo xuống đoạn VPC
  + Phần Virtual private cloud (VPC) click chọn **Default VPC**.
  + Phần DB subnet group click chọn **default**.
  + Phần Public access click chọn **yes**.
  + Phần VPC security group (firewall) click chọn **Choose existing**.
  
![rds](/images/2.prerequisite/022-rds-step7.png)

9. Tiếp tục kéo xuống đoạn Database authentication
  + Phần Database authentication options click chọn **Password authentication**.
  + Phần Monitoring mặc định là **Database Insights - Standard**.
  
![rds](/images/2.prerequisite/023-rds-step8.png)

10. Kéo xuống đoạn cuối trang, click chọn vào **Create database**
  
![rds](/images/2.prerequisite/024-rds-step9.png)

11. Sau khi đã tạo xong, ở bảng hiện thị database sẽ có database vừa tạo với trạng thái là Available
  
![rds](/images/2.prerequisite/025-rds-step10.png)

12. Click chọn vào database vừa tạo để xem các thông số chi tiết, chú ý đến endpoint sẽ là đường link kết nối đến database của ứng dụng
  
![rds](/images/2.prerequisite/026-rds-step11.png)

13. Tiếp tục kéo xuống đoạn Connectivity & security và chúng ta có thể thấy ứng dụng chạy trên port 3306
  
![rds](/images/2.prerequisite/027-rds-step12.png)

14. Mở ứng dụng  MySQL Community, bạn có thể tải [ứng dụng](https://dev.mysql.com/downloads/)
  + Click chọn vào mục **Database**.
  + Click chọn **Connect to Database**.
  
![rds](/images/2.prerequisite/028-rds-step13.png)

15. Hộp thoại Connect to database sẽ xuất hiện
  + Phần Connection Method click chọn **Standard**.
  + Phần Hostname dán url của database vừa tạo trên rds.
  + Phần username nhập là **admin**.
  + Click chọn vào ok để tiến hành kết nối, sau đó nhập thêm mật khẩu của database vừa tạo vào.
  
![rds](/images/2.prerequisite/029-rds-step14.png)

16. Xuất hiện giao diện ứng dụng, có các thông tin của database vừa tạo
  
![rds](/images/2.prerequisite/030-rds-step15.png)


Vậy là chúng ta đã chuẩn bị xong phần về RDS, ở bước tiếp theo chúng ta sẽ chuyển qua bước tải source code và đóng gói thành file jar.