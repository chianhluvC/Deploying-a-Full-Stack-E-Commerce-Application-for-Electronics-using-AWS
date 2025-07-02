---
title: "Create RDS"
date: 2025-05-25
weight: 3
chapter: false
pre: " <b> 2.3 </b> "
---

### Create RDS

In this step, we will create an RDS instance.  
This is a crucial step in preparing to deploy our application data to RDS in the upcoming sections.

1. Go to the [RDS Management Console](https://console.aws.amazon.com/rds/home)  
2. Click on **Databases**

![rds](/images/2.prerequisite/016-rds-step1.png)

3. On the RDS dashboard, click **Create database**

![rds](/images/2.prerequisite/017-rds-step2.png)

4. On the Create database page:  
   - Under **Choose a database creation method**, select **Standard create**  
   - Under **Engine options**, choose **MySQL**

![rds](/images/2.prerequisite/018-rds-step3.png)

5. Scroll down to:  
   - **Templates**: select **Free tier**  
   - **Availability and durability**: will be automatically set to **Single-AZ DB instance deployment (1 instance)**

![rds](/images/2.prerequisite/019-rds-step4.png)

6. Scroll down to the database credentials section:  
   - Enter a **DB instance identifier**  
   - Set **Master username** to `admin`  
   - Under **Credentials management**, choose **Self managed**

![rds](/images/2.prerequisite/020-rds-step5.png)

7. Scroll down to the password section:  
   - Enter the **Master password**  
   - Re-enter it in **Confirm master password**

![rds](/images/2.prerequisite/021-rds-step6.png)

8. In the **Connectivity** section:  
   - **Virtual private cloud (VPC)**: choose **Default VPC**  
   - **DB subnet group**: choose **default**  
   - **Public access**: select **Yes**  
   - **VPC security group (firewall)**: choose **Choose existing**

![rds](/images/2.prerequisite/022-rds-step7.png)

9. Under **Database authentication**:  
   - Select **Password authentication**  
   - Monitoring defaults to **Database Insights – Standard**

![rds](/images/2.prerequisite/023-rds-step8.png)

10. Scroll to the bottom and click **Create database**

![rds](/images/2.prerequisite/024-rds-step9.png)

11. Once created, you will see your new database listed with the status **Available**

![rds](/images/2.prerequisite/025-rds-step10.png)

12. Click on the newly created database to view its details — take note of the **endpoint**, which is the URL your application will use to connect

![rds](/images/2.prerequisite/026-rds-step11.png)

13. Scroll down to **Connectivity & security** to see that the database runs on port **3306**

![rds](/images/2.prerequisite/027-rds-step12.png)

14. Open **MySQL Community** client. You can download it [here](https://dev.mysql.com/downloads/)  
   - Click **Database**  
   - Then click **Connect to Database**

![rds](/images/2.prerequisite/028-rds-step13.png)

15. In the **Connect to database** dialog:  
   - **Connection Method**: select **Standard**  
   - **Hostname**: paste the endpoint from your RDS instance  
   - **Username**: enter `admin`  
   - Click **OK**, then enter the master password when prompted

![rds](/images/2.prerequisite/029-rds-step14.png)

16. The MySQL client interface will now show the details of your newly created database

![rds](/images/2.prerequisite/030-rds-step15.png)

---

Now that we’ve finished setting up RDS, the next step is to download the source code and package it into a `.jar` file.
