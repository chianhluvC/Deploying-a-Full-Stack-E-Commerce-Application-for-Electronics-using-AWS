---
title : "Triển khai source lên S3"
date: 2025-05-25 
weight : 1 
chapter : false
pre : " <b> 3.1. </b> "
---


1. Truy cập vào bucket đã tạo và click chọn upload

![s3deploy](/images/3.deploy/001-s3-deploy1.png)

2. Tại trang upload
  + Click chọn **Add files**.
  + Sau đó tải lên file đã đóng gói ở phần trước

![s3deploy](/images/3.deploy/002-s3-deploy2.png)

3. Sau khi chọn file, thông tin file cần tải lên sẽ được hiện thị

![s3deploy](/images/3.deploy/003-s3-deploy3.png)

4. Sau đó click vào **Upload** để tải file lên

![s3deploy](/images/3.deploy/004-s3-deploy4.png)


5. Sau khi tải file thành công sẽ có trạng thái là Succeeded 

![s3deploy](/images/3.deploy/005-s3-deploy5.png)

6. Click vào file vừa tải để xem thông số các chi tiết

![s3deploy](/images/3.deploy/006-s3-deploy6.png)

7. Xem các quyền của bucket chứa file đã tải lên 

![s3deploy](/images/3.deploy/007-s3-deploy7.png)

8. Click vào file vừa tải lên, sau đó click vào permissions để xem các quyền với file vừa tạo

![s3deploy](/images/3.deploy/008-s3-deploy8.png)


9. Click chọn vào Object action ở bên phải

![s3deploy](/images/3.deploy/009-s3-deploy9.png)


10. Sau đó chọn vào Share with a presigned URL

![s3deploy](/images/3.deploy/010-s3-deploy10.png)


11. Giao diện Share with a presigned URL sẽ xuất hiện
  + Click chọn Minutes
  + Điền **45** vào Number of minutes
  + Click vào create presigned URL

![s3deploy](/images/3.deploy/011-s3-deploy11.png)

12. Thông báo sẽ xuất hiện, sau đó click vào Copy presigned URL để lưu đường dẫn tới file vừa tạo

![s3deploy](/images/3.deploy/012-s3-deploy12.png)


 Vậy là bạn đã xong bước đầu tiên của phần triển khai web lên AWS.

