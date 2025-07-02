---
title: "Download Source Code and Package into JAR File"
date: 2025-05-25
weight: 4
chapter: false
pre: " <b> 2.4 </b> "
---

### Download Source Code and Package into JAR File

In this step, we will download the source code and package it into a JAR file. This is an important preparation step before deploying the source code to S3.

1. Go to the [GitHub repository interface](https://github.com/chianhluvC/LTUDJavaNhom12).
2. Click **Download Zip**.

![jar](/images/2.prerequisite/031-jar-step1.png)

3. After downloading, open the `application.properties` file and configure it as follows:

```properties
spring.datasource.url= ----urlRDSdatabase----
spring.datasource.username= -----yourUsername----
spring.datasource.password= ----yourPassword-----
```

  + The url should be taken from the RDS database that was previously created.
  + The username and password were also defined during the initial RDS setup.

![jar](/images/2.prerequisite/032-jar-step2.png)

4. Package the project into a JAR file. You can refer to [this guide](https://sarangsurve.medium.com/create-a-jar-file-in-intellij-idea-5c876ca06689) for detailed instructions on how to package into a JAR file.
  
![jar](/images/2.prerequisite/033-jar-step3.png)


Now that we’ve completed downloading the source code and packaging it into a JAR file, in the next step, we will proceed to configure Route53.