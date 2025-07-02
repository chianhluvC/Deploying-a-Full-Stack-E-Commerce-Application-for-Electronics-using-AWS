+++
title = "Clean Up Resources"
date = 2025
weight = 5
chapter = false
pre = "<b>5. </b>"
+++

We will follow the steps below to delete the resources created during this practical exercise.

#### Delete EC2 Instance

Go to the [EC2 Management Console](https://console.aws.amazon.com/ec2/v2/home)  
  + Click **Instances**  
  + Select the instance you want to delete  
  + Click **Instance state**  
  + Click **Terminate instance**, then click **Terminate** to confirm

![Clean](/images/5.clean/001-cleanstep1.png)

![Clean](/images/5.clean/002-cleanstep2.png)

#### Delete S3 Bucket

Go to the [S3 Management Console](https://s3.console.aws.amazon.com/s3/home)  
  + Select the S3 bucket created during this exercise  
  + Click **Empty**  
  + Type **permanently delete**, then click **Empty** to remove all objects in the bucket  

![Clean](/images/5.clean/003-cleanstep3.png)

![Clean](/images/5.clean/004-cleanstep4.png)

![Clean](/images/5.clean/005-cleanstep5.png)

#### Delete RDS

1. Go to the [RDS Management Console](https://console.aws.amazon.com/rds/home)  
   + Select the database you want to delete  
   + Click **Actions**  
   + Click **Delete**

![Clean](/images/5.clean/006-cleanstep6.png)

2. In the confirmation section, check the box to acknowledge the service terms  
   + Enter **delete me** to confirm deletion of the endpoints  
   + Click **Delete** to proceed

![Clean](/images/5.clean/007-cleanstep7.png)

![Clean](/images/5.clean/008-cleanstep8.png)
