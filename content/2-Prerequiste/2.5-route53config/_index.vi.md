---
title : "Cấu hình Route 53"
date: 2025-05-25 
weight : 5
chapter : false
pre : " <b> 2.5 </b> "
---

### Cấu hình Route 53

Trong bước này chúng ta sẽ tiến hành tải cấu hình Route 53. Đây là bước cuối cùng của phần chuẩn bị này

1. Truy cập vào [giao diện trang quản lý domains](https://console.aws.amazon.com/route53/domains/home)
2. Click vào  **Register domains**.  

![route53](/images/2.prerequisite/034-route53-step1.png)

3. Giao diện trang quản lý domains sẽ xuất hiện
  + Phần Check availability for a domain nhập tên domain cần tạo, sau đó nhấn **Search**
  + Sau khi tìm thấy domain phù hợp nhấn **Select**
  + Cuối cùng nhấn Proceed to checkout
  
![route53](/images/2.prerequisite/035-route53-step2.png)

4. Ở phần Pricing nhấn **Next**
  
![route53](/images/2.prerequisite/036-route53-step3.png)

5. Tiến hành xem lại các thông tin trước khi Submit
  
![route53](/images/2.prerequisite/037-route53-step4.png)

6. Kéo xuống cuối cùng của trang, tích vào ô đồng ý với điều khoản dịch vụ và Click **Submit**
  
![route53](/images/2.prerequisite/038-route53-step5.png)

7. Sau khi tạo thành công, chúng ta sẽ thấy thông tin domain vừa tạo
  
![route53](/images/2.prerequisite/039-route53-step6.png)

8. Click chọn vào domain vừa tạo để xem chi tiết các thông số
  
![route53](/images/2.prerequisite/040-route53-step7.png)

Chúng ta đã chuẩn bị xong phần cấu hình Route53, ở phần sau chúng ta sẽ tới các bước triển khai.