---
title: "Conclusion and Future Development"
date: 2025-05-25
weight: 4
chapter: false
pre: " <b> 4. </b> "
---

## 📌 Conclusion and Future Development

### 🔍 Conclusion

By deploying and comparing the model using Amazon EC2, S3, and RDS with other deployment methods (such as shared hosting, traditional VPS, or PaaS platforms like Heroku), it is clear that AWS offers significant advantages in scalability, flexibility, and resource management.  
EC2 provides powerful and flexible computing capabilities, S3 offers stable and scalable object storage, while RDS simplifies database management with built-in features such as automatic backups, security, and scalability.  
However, costs may be higher if resources are not optimized and usage is not monitored regularly.

### 🚀 Future Development

In the future, the deployment process can be enhanced by integrating a CI/CD pipeline using AWS-native services such as:
- **AWS CodePipeline**
- **AWS CodeBuild**
- **AWS CodeDeploy**

These services allow automation of the build, test, and deployment processes, reducing manual operations and speeding up feature releases.  
Moreover, adopting **Infrastructure as Code (IaC)** with AWS CloudFormation or Terraform will improve automation, ensure consistency across environments, and align with modern DevOps practices.

---

### 📊 Deployment Comparison Table

| Criteria                         | AWS (EC2 + S3 + RDS)         | VPS / Shared Hosting       | Heroku / Vercel / PaaS     |
|----------------------------------|-------------------------------|-----------------------------|-----------------------------|
| Performance                      | High                          | Medium / Limited            | Depends on plan             |
| Scalability                      | Excellent (Auto Scaling)      | Manual                      | Good (plan-based)           |
| System Management                | Self-managed (more control)   | Limited access              | Fully managed               |
| Configuration Flexibility        | Very flexible                 | Limited                     | Limited                     |
| CI/CD Integration with AWS       | Deep integration (CodeBuild…)| Difficult or unavailable    | Built-in integration        |
| Cost                             | Pay-as-you-use                | Low                         | Free / Expensive (based on plan) |
| Suitable for large applications  | ✅                             | ❌                           | ❌ / Moderate               |
| Suitable for learning / MVP      | ✅ (with Free Tier)            | ✅                           | ✅                          |

---
