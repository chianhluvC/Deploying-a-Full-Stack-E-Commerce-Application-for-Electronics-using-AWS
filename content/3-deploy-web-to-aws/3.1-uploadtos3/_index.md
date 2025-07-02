---
title: "Deploy Source to S3"
date: 2025-05-25
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---

1. Go to the created bucket and click **Upload**.

![s3deploy](/images/3.deploy/001-s3-deploy1.png)

2. On the upload page:  
   + Click **Add files**.  
   + Then upload the packaged file from the previous section.

![s3deploy](/images/3.deploy/002-s3-deploy2.png)

3. Once the file is selected, its information will be displayed.

![s3deploy](/images/3.deploy/003-s3-deploy3.png)

4. Then click **Upload** to start uploading the file.

![s3deploy](/images/3.deploy/004-s3-deploy4.png)

5. Once the upload is successful, the status will be **Succeeded**.

![s3deploy](/images/3.deploy/005-s3-deploy5.png)

6. Click on the uploaded file to view detailed properties.

![s3deploy](/images/3.deploy/006-s3-deploy6.png)

7. View the permissions of the bucket that contains the uploaded file.

![s3deploy](/images/3.deploy/007-s3-deploy7.png)

8. Click on the uploaded file, then click on **Permissions** to view its access settings.

![s3deploy](/images/3.deploy/008-s3-deploy8.png)

9. Click **Object actions** on the right side.

![s3deploy](/images/3.deploy/009-s3-deploy9.png)

10. Then select **Share with a presigned URL**.

![s3deploy](/images/3.deploy/010-s3-deploy10.png)

11. The **Share with a presigned URL** screen will appear:  
   + Select **Minutes**.  
   + Enter **45** in the Number of minutes field.  
   + Click **Create presigned URL**.

![s3deploy](/images/3.deploy/011-s3-deploy11.png)

12. A notification will appear. Click **Copy presigned URL** to save the link to the uploaded file.

![s3deploy](/images/3.deploy/012-s3-deploy12.png)

You’ve now completed the first step of deploying your web application to AWS.
