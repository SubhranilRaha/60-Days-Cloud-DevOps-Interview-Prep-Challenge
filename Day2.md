20 Interview Questions & Answers
1. What is cloud computing?
Answer: Cloud computing means accessing compute resources such as servers, storage, networking, and software over the internet. The cloud provider manages the physical infrastructure, while customers consume the resources as needed.

2. Why did companies move from traditional data centers to cloud?
Answer: Traditional data centers require hardware procurement, manual setup, maintenance, 24/7 monitoring, and large upfront investment. Cloud provides faster provisioning, easier scalability, pay-per-use pricing, and managed infrastructure.

3. What is the difference between a physical server and a cloud VM?
Answer: A physical server is dedicated hardware that you own or lease, while a cloud VM is a virtual machine created on a provider's physical infrastructure. Cloud VMs can usually be created, resized, and removed much faster.

4. What is IaaS?
Answer: IaaS stands for Infrastructure as a Service. It provides infrastructure such as virtual machines, CPU, memory, storage, and networking. The customer manages the operating system and everything above it.

5. What is PaaS?
Answer: PaaS stands for Platform as a Service. The provider manages the infrastructure and platform/runtime, allowing the customer to focus more on deploying and running applications.

6. What is SaaS?
Answer: SaaS stands for Software as a Service. It provides ready-to-use software over the internet. The user consumes the application without managing the underlying infrastructure or platform.

7. What is a public cloud?
Answer: A public cloud is an environment where cloud resources are provided by a third-party provider and can be accessed over the internet. AWS, Azure, and GCP are common examples.

8. What is a private cloud?
Answer: A private cloud is dedicated to a specific organization. Access and infrastructure are controlled by that organization, often with additional network and security controls.

9. What is hybrid cloud?
Answer: Hybrid cloud combines private and public cloud environments. For example, sensitive systems can remain in a private environment while scalable application workloads run in a public cloud.

10. How do you select a cloud region?
Answer: A major factor is latency. I would test latency from the customer locations to available regions and select a suitable region with low latency. I would also consider compliance, availability, cost, and disaster recovery requirements.

11. Why should primary and DR infrastructure not be placed in the same region?
Answer: A regional disaster such as a major power failure, flood, or other outage could affect both environments. Geographic separation reduces the risk of losing both primary and DR infrastructure at the same time.

12. What is the difference between internal and external IP?
Answer: An internal IP is used for private communication inside the cloud network or VPC. An external IP is reachable from outside the private network, subject to firewall and security rules.

13. What is SSH and which port does it use?
Answer: SSH stands for Secure Shell and is commonly used to securely connect to Linux servers remotely. The standard SSH port is TCP 22.

14. Why is Ubuntu commonly used?
Answer: Ubuntu is open-source, widely adopted, has strong community support, and is commonly used for cloud and web workloads. For enterprise-specific requirements, organizations may choose distributions such as RHEL.

15. What is an LTS version?
Answer: LTS means Long-Term Support. An LTS release receives long-term maintenance and security updates, making it suitable for stable production environments.

16. How can you create a cloud VM?
Answer: A VM can be created through the cloud console, CLI, SDK/script, Infrastructure as Code such as Terraform, or APIs. In AWS, CloudFormation is another Infrastructure as Code option.

17. What is Infrastructure as Code?
Answer: Infrastructure as Code, or IaC, means defining infrastructure using code or configuration files instead of manually creating resources. Terraform is a common example.

18. How do you check the Docker version?
Answer: Use docker -v or docker --version.

19. How do you check running Docker containers?
Answer: Use docker ps. It displays currently running containers.

20. What is port mapping in Docker?
Answer: Port mapping connects a port on the host machine to a port inside the container. For example, mapping VM port 3000 to container port 3000 allows users to access the application through the VM's IP and port 3000.

20 Scenario-Based Questions & Answers
1. Your website suddenly receives traffic from 100 users to 10,000 users. What would you do?
Answer: I would first monitor CPU, memory, network, and application metrics. Then I would use load balancing and horizontal scaling/auto-scaling to add capacity. I would also check database and other dependent services because scaling only the web servers may not solve the complete bottleneck.

2. Your application is hosted in Mumbai, but most customers are in Singapore. What would you investigate?
Answer: I would measure latency from the customer locations to different cloud regions. If business and compliance requirements allow it, I would evaluate deploying the workload closer to the users, such as Singapore, to reduce network latency.

3. Your primary cloud region goes down. What should happen?
Answer: A properly designed DR architecture should allow traffic or workloads to be restored in a separate region. The exact recovery approach depends on the application's RTO, RPO, data replication design, and business requirements.

4. Your company says customer data must remain inside India. How would this affect region selection?
Answer: Data residency becomes a mandatory constraint. I would select an appropriate Indian region or regions that satisfy the requirement, and then evaluate latency, availability, cost, and DR options within the allowed geographic boundaries.

5. A new VM is created, but you cannot SSH into it. What would you check?
Answer: I would check whether the VM is running, whether it has the expected IP address, whether port 22 is allowed by firewall/security rules, whether routing is correct, and whether the SSH key or credentials are valid.

6. Your Docker container is running, but users cannot access the application.
Answer: I would check docker ps, confirm the application is listening on the expected container port, verify host-to-container port mapping, and then check cloud firewall/security rules and whether the VM's external IP is reachable.

7. A physical server takes several days to replace after hardware failure. How would cloud help?
Answer: Cloud allows a replacement VM or infrastructure to be provisioned through a console, CLI, API, or IaC. This can reduce provisioning time significantly, assuming the required images, data, networking, and automation are already prepared.

8. Your company has sensitive workloads but also needs public-cloud scalability. Which model could fit?
Answer: A hybrid-cloud model could fit. Sensitive workloads can remain in a controlled private environment while scalable workloads use public cloud resources, depending on security, networking, compliance, and application architecture.

9. Your cloud bill is high because servers are idle after a temporary sales event. What would you investigate?
Answer: I would review resource utilization and identify idle or oversized resources. Then I would consider auto-scaling, scheduled scaling, right-sizing, and shutting down non-production resources when they are not required.

10. You need to create 50 identical VMs. Would you create them manually?
Answer: I would avoid manual creation at that scale. I would use Terraform or another automation/IaC approach so the infrastructure is repeatable, version-controlled, and easier to manage.

11. A developer wants the application to create a VM automatically after a user submits a request. How can this be implemented?
Answer: The application can call a cloud API or service through an authenticated backend workflow. The developer handles application-side API integration, while the cloud/DevOps engineer provides the required infrastructure, permissions, networking, and automation design.

12. Your company wants production stability but a new OS version has been released. Would you upgrade immediately?
Answer: I would not upgrade production immediately without validation. I would test the new version in a POC or non-production environment, verify application compatibility and automation, and then plan a controlled migration.

13. Your application works inside the VM but not from the internet. What could be wrong?
Answer: The application may be listening only on localhost, the required host/container port may not be mapped, or cloud firewall/security rules may block the port. I would validate each layer from the application to the network.

14. You have a primary region and a DR region, but both are geographically close. What concern do you have?
Answer: A large regional or geographic event could potentially affect both environments. I would evaluate greater geographic separation while considering latency, data residency, replication capability, and recovery objectives.

15. A container exits immediately after starting. How would you troubleshoot?
Answer: I would first check docker ps -a to see the container status and then inspect logs using docker logs <container-name-or-id>. I would verify the image, startup command, environment variables, dependencies, and application errors.

16. Your VM has an external IP, but the application is still unreachable on port 3000. What would you check?
Answer: I would verify that the application is listening on port 3000, confirm Docker port mapping, check the VM's firewall/security rules, and verify that the cloud network allows inbound TCP traffic on port 3000.

17. Your company wants a ready-to-use email application without managing servers. Which cloud service model matches this requirement?
Answer: SaaS is the closest match because the user consumes a ready-made application without managing the underlying infrastructure or platform.

18. Your team wants a managed database instead of maintaining the database server OS and patches. Which service model is this closest to?
Answer: This is generally a PaaS-style managed service because the provider manages much of the underlying infrastructure and platform while the customer focuses on using the database service.

19. Your team wants complete control over the OS, installed packages, and server configuration. Which model would you choose?
Answer: IaaS would provide the required level of control because the team receives a VM and manages the operating system and software installed above the infrastructure layer.

20. During a production incident, someone suggests putting everything in one region because it has the lowest latency. What else should you consider?
Answer: Latency is important, but it should not be the only factor. I would also evaluate high availability, disaster recovery, compliance/data residency, service availability, cost, data replication, and the application's RTO/RPO before finalizing the architecture.
