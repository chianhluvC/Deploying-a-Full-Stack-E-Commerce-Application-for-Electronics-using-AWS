---
title : "Configuring EC2 and Connecting to S3"
date: 2025-05-25 
weight : 2 
chapter : false
pre : " <b> 3.2. </b> "
---


1. Access the created EC2 instance and click Copy the Public IPv4 address

![ec2deploy](/images/3.deploy/014-ec2-deploy2.png)

2. Open CMD, navigate to the directory containing the EC2 keypair, and execute the following code to SSH into the EC2 instance:
  
```cmd
ssh -i "your-keypair.pem" ec2-user@<EC2-PUBLIC-IP>
```

![ec2deploy](/images/3.deploy/017-ec2-deploy5.png)

3. Copy the S3 object URL of the uploaded JAR file
![ec2deploy](/images/3.deploy/018-ec2-deploy6.png)

4. Configure the file path

![ec2deploy](/images/3.deploy/019-ec2-deploy7.png)


5. Click the Copy icon to copy the path

![ec2deploy](/images/3.deploy/020-ec2-deploy8.png)

6. Enter the command below to download the JAR file from S3 to EC2

```cmd
pwd 'links3'
```

![ec2deploy](/images/3.deploy/021-ec2-deploy9.png)

7. Wait for the download to complete. A 100% progress notification will appear in CMD

![ec2deploy](/images/3.deploy/022-ec2-deploy10.png)

8. Run the following command to rename the file

```cmd
mv 'namefile' newName
ls
```

![ec2deploy](/images/3.deploy/023-ec2-deploy11.png)


9. Install Java 22 using the command below

```cmd
sudo yum install java-22
ls
```

![ec2deploy](/images/3.deploy/024-ec2-deploy12.png)

10. Wait for Java 22 to be installed on the EC2 instance

![ec2deploy](/images/3.deploy/025-ec2-deploy13.png)


11. Proceed with the following steps to run the web application
  + Verify the Java version
  + Launch the application
  
 ```cmd
java -version
java -jar DASpring.jar
ls
``` 

![ec2deploy](/images/3.deploy/026-ec2-deploy14.png)

12. Check the running application’s details

![ec2deploy](/images/3.deploy/027-ec2-deploy15.png)

13. Add a port to the inbound rules in the EC2 security group.
   + Click add Rule
   + Select "Custom TCP" from the rule type dropdown
   + Enter port 8080 in the port range field
   + Set source to "Anywhere" (0.0.0.0/0 for IPv4)
   + Click "Save rules" to apply the changes

![ec2deploy](/images/3.deploy/028-ec2-deploy16.png)

Congratulations! You’ve completed deploying the E-Commerce Full-Stack application (specializing in electronics) on AWS. In the next section, we’ll test the deployed web application.
