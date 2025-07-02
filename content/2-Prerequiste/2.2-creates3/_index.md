---
title: "Create S3"
date: 2025-05-25
weight: 2
chapter: false
pre: " <b> 2.2 </b> "
---

### Create S3

In this step, we will create an S3 bucket.  
This prepares us for the next step, where we will upload the `.jar` file of the source code to S3.

1. Go to the [S3 Management Console](https://console.aws.amazon.com/s3/home)  
2. Click **Create bucket**

![s3](/images/2.prerequisite/011-s3-step1.png)

3. Under **Bucket type**, configure the following:  
   - Select **General purpose**  
   - Set the **Bucket name** to **mySpringbootApp**

![s3](/images/2.prerequisite/012-s3-step2.png)

4. In the **Bucket Versioning** section, choose **Disable**  
   In the **Default encryption** section, choose  
   **Server-side encryption with Amazon S3 managed keys (SSE-S3)**

![s3](/images/2.prerequisite/013-s3-step3.png)

5. Scroll down to the **Bucket Key** section:  
   - Select **Enable**  
   - Then click **Create bucket**

![s3](/images/2.prerequisite/014-s3-step4.png)

6. After creation, you will see the result as shown below:

![s3](/images/2.prerequisite/015-s3-step5.png)

Next, we will proceed to create and configure RDS.
