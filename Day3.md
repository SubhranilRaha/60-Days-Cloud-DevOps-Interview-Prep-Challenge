30 DevOps Basic Tools Interview Questions & Answers

These questions are based on the DevOps toolchain covered in the session: planning, coding, Git/GitHub, build, artifact management, testing, CI/CD, containers, IaC, configuration management, and monitoring. The focus is on understanding what each tool does and where it is used.

1. What is Jira and why is it used in DevOps?

Answer: Jira is a project and issue tracking tool. Teams use it to create tickets, stories, tasks, bugs, and epics and to track their progress.

Use Case: A Scrum team creates a ticket for a new application feature, assigns it to a developer, and tracks it from development to completion.

2. What is Git?

Answer: Git is a distributed version control system used to manage source code and track changes made by developers.

Use Case: A developer changes application code, runs git add, git commit, and git push to save the change and share it with the remote repository.

3. What is GitHub?

Answer: GitHub is a cloud-based platform for hosting Git repositories and collaborating on source code.

Use Case: Multiple developers work on the same project, create branches, push code, review changes, and maintain commit history in GitHub.

4. What is the difference between Git and GitHub?

Answer: Git is the version control tool that runs locally, while GitHub is a remote platform that hosts Git repositories and provides collaboration features.

Simple Example: Git is the tool you use on your laptop; GitHub is the online place where your repository is stored and shared.

5. What is Maven?

Answer: Maven is a build and dependency management tool commonly used for Java projects.

Use Case: A Java application contains many dependencies. Maven downloads the required dependencies, compiles the code, runs tests, and packages the application into an artifact such as a JAR or WAR.

6. What is Nexus?

Answer: Nexus is an artifact repository used to store and manage build artifacts with versioning.

Use Case: Jenkins creates app-1.0.jar. Instead of keeping the artifact only on the Jenkins server, it can be uploaded to Nexus so other environments or pipelines can retrieve the exact version.

7. What is Selenium?

Answer: Selenium is a browser automation tool commonly used for UI and functional testing of web applications.

Use Case: After deployment, an automated Selenium test opens the website, enters login credentials, clicks buttons, and verifies that the expected page is displayed.

8. What is JMeter?

Answer: JMeter is used mainly for load and performance testing.

Use Case: Before production deployment, a team wants to test how an application behaves when thousands of users send requests at the same time.

9. What is Jenkins?

Answer: Jenkins is an open-source automation server widely used to implement CI/CD pipelines.

Use Case: A developer pushes code to GitHub. Jenkins detects the change, builds the application, runs tests, creates an artifact, and can deploy it to an environment.

10. What is CI?

Answer: Continuous Integration means frequently integrating code changes into a shared repository and automatically building and testing those changes.

Use Case: Every developer push triggers an automated build and test process so integration problems are found early.

11. What is CD?

Answer: Continuous Delivery or Continuous Deployment is the automated process of moving validated application changes toward or into deployment environments.

Use Case: After successful testing, a pipeline promotes the application from Dev to QA and then to Production according to the organization's release process.

12. What is Docker?

Answer: Docker is a containerization platform used to package an application with its dependencies into a portable container image.

Use Case: If an application works on a developer laptop but fails on a server because of dependency differences, Docker can package the application environment consistently.

13. What is a Docker image?

Answer: A Docker image is a packaged, immutable template used to create containers.

Use Case: A team builds myapp:v1 once and uses the same image in Dev, QA, and Production.

14. What is Kubernetes?

Answer: Kubernetes is a container orchestration platform used to deploy, manage, scale, and automate containers at large scale.

Use Case: A company has hundreds or thousands of containers and needs automatic scheduling, scaling, service discovery, and recovery.

15. What is the difference between Docker and Kubernetes?

Answer: Docker is commonly used to build and package container images, while Kubernetes manages and orchestrates containers across a cluster.

Simple Example: Docker helps package the application; Kubernetes helps run and manage many copies of that application.

16. What is Terraform?

Answer: Terraform is an Infrastructure as Code (IaC) tool used to provision and manage infrastructure using configuration files.

Use Case: Instead of manually creating 20 AWS resources, Terraform can define the infrastructure as code and create it consistently.

17. Why is Terraform useful in a multi-cloud environment?

Answer: Terraform supports many cloud providers through providers, so infrastructure can be managed using a common IaC workflow.

Use Case: An organization uses AWS for one workload and GCP for another. Terraform can be used to manage infrastructure for both.

18. What is Ansible?

Answer: Ansible is an automation and configuration management tool used to perform repetitive operational tasks across servers.

Use Case: An administrator needs to install Python and security patches on 200 servers. Ansible can automate the same task across all servers.

19. What is Prometheus?

Answer: Prometheus is a monitoring and metrics collection system. It collects and stores time-series metrics.

Use Case: Prometheus collects CPU, memory, request count, and application metrics from servers or Kubernetes workloads.

20. What is Grafana?

Answer: Grafana is a visualization and dashboard tool used to display metrics and monitoring data.

Use Case: Prometheus stores CPU and memory metrics, while Grafana displays them in dashboards so engineers can quickly understand system health.

21. What is CloudWatch?

Answer: Amazon CloudWatch is an AWS monitoring and observability service used for metrics, logs, alarms, and monitoring AWS resources.

Use Case: An AWS team monitors EC2 CPU utilization and creates an alarm when CPU remains above a defined threshold.

22. What is Splunk?

Answer: Splunk is primarily a logging and data analysis platform. It can also support monitoring and alerting.

Use Case: Application logs from multiple servers are centralized in Splunk so engineers can search errors and investigate incidents.

23. What is Helm?

Answer: Helm is a package manager for Kubernetes. It helps package and manage Kubernetes application configurations using charts.

Use Case: A complex Kubernetes application contains multiple manifests. A Helm chart can package them together and make installation and upgrades easier.

24. What is GitLab CI?

Answer: GitLab CI is a CI/CD capability integrated into GitLab.

Use Case: When code is pushed to a GitLab repository, a pipeline can automatically build, test, scan, and deploy the application.

25. What is an artifact in DevOps?

Answer: An artifact is a build output produced by the build process, such as a JAR, WAR, executable, package, or container image.

Use Case: A Java build produces application.jar, which is then stored in an artifact repository and used for deployment.

26. What is the purpose of a CI/CD pipeline?

Answer: A CI/CD pipeline automates the flow from source code to build, testing, packaging, and deployment.

Use Case: Instead of manually performing ten deployment steps, Jenkins executes the same repeatable process every time code is approved.

27. Why do we need version control?

Answer: Version control keeps a history of code changes and enables collaboration, comparison, rollback, and accountability.

Use Case: If a new release introduces a bug, the team can identify the change and roll back to a known working version.

28. What is the difference between release and deployment?

Answer: A release is the process of moving a version toward another environment or making a version available, while deployment is the actual act of placing and running the application in the target environment.

Example: Moving v2.0 from Dev to QA is part of the release flow; installing and running v2.0 on QA servers is deployment.

29. Why do DevOps teams use automation?

Answer: Automation reduces repetitive manual work, improves consistency, saves time, and reduces human error.

Use Case: Instead of manually patching 200 servers every week, Ansible can perform the same operation consistently.

30. Why should a DevOps engineer understand tools by category instead of memorizing many tools?

Answer: Different companies use different products, but the underlying DevOps requirement remains similar.

Example: One company may use Jenkins, another GitLab CI, and another GitHub Actions. The important knowledge is understanding CI/CD concepts and how the selected tool implements them.

30 DevOps Scenario-Based Interview Questions & Answers

These questions focus on which tool to use, why to use it, and when to use it. In an interview, first identify the problem, then select the appropriate DevOps category and tool.

1. Developers are pushing code manually and the team wants automatic builds and tests. Which tool will you use?

Answer: Use Jenkins for CI/CD automation.

Why: Jenkins can connect with GitHub, trigger pipelines when code changes, build the application, run tests, and produce artifacts.

Use Case: GitHub push → Jenkins → Maven build → tests → artifact.

2. A Java developer has to compile the code and download project dependencies automatically. Which tool will you use?

Answer: Use Maven.

Why: Maven handles Java build lifecycle and dependency management.

Use Case: mvn clean package can clean the project, compile the code, run tests, and create the JAR/WAR artifact.

3. Your company has 300 developers working on the same application. How will you manage source code?

Answer: Use Git with GitHub.

Why: Git provides version control, branches, commits, merging, and history, while GitHub provides centralized remote collaboration.

Use Case: Developers create branches, commit changes, push to GitHub, and collaborate through pull requests.

4. A developer accidentally introduces a bug and you need to identify who changed the code. Which tool will help?

Answer: Use Git and the GitHub repository history.

Why: Git records commits, authors, timestamps, and changed files.

Use Case: Inspect commit history, identify the change, and revert or fix the problematic commit.

5. Your application works on the developer laptop but fails in QA because the environment is different. Which tool can help?

Answer: Use Docker.

Why: Docker packages the application and its dependencies into an image so the same packaged application can move across environments.

Use Case: Build one image and promote the same image from Dev → QA → Production.

6. You have 1,000 containers and need automatic scheduling, scaling, and management. Which tool will you use?

Answer: Use Kubernetes.

Why: Kubernetes is designed for container orchestration at scale.

Use Case: Kubernetes can manage replicas, services, scheduling, health checks, and scaling.

7. You need to create 50 cloud VMs repeatedly without manually creating them from the console. Which tool will you use?

Answer: Use Terraform.

Why: Terraform lets you define infrastructure as code and provision it repeatedly.

Use Case: Write Terraform configuration once and use it to create the required infrastructure consistently.

8. Your company uses AWS, Azure, and GCP. You want a common Infrastructure as Code approach. Which tool can you consider?

Answer: Use Terraform.

Why: Terraform supports multiple cloud providers through providers.

Use Case: Manage infrastructure across AWS, Azure, and GCP using code and a common workflow.

9. You need to install Python on 200 Linux servers. Would you do it manually?

Answer: No. Use Ansible.

Why: Ansible can execute the same configuration task across many servers.

Use Case: Create a playbook that installs Python and run it against the required hosts.

10. Your organization needs weekly patching on hundreds of servers. Which tool would you choose?

Answer: Use Ansible for configuration and operational automation.

Why: Repetitive patching tasks can be automated and made consistent.

Use Case: Schedule or trigger an Ansible job to apply approved patches across server groups.

11. Your Kubernetes cluster is running but you don't know whether CPU and memory usage is increasing. Which tools would you use?

Answer: Use Prometheus and Grafana.

Why: Prometheus collects metrics and Grafana visualizes them.

Use Case: Create dashboards for node CPU, memory, pod resource usage, and application metrics.

12. You are running only AWS infrastructure and want native monitoring. Which tool can you use?

Answer: Use CloudWatch.

Why: CloudWatch integrates directly with AWS services and provides metrics, logs, and alarms.

Use Case: Monitor EC2 CPU utilization and create an alarm for abnormal usage.

13. Application logs are spread across 100 servers and engineers need centralized log search. Which tool can you use?

Answer: Splunk can be used for centralized log collection and analysis.

Why: Engineers can search and analyze logs from multiple systems in one place.

Use Case: Search application errors across multiple servers during incident troubleshooting.

14. Your website suddenly receives 10,000 users instead of 100. What should you investigate first?

Answer: Use monitoring tools such as Prometheus/Grafana for Kubernetes environments or CloudWatch for AWS environments.

Why: First understand CPU, memory, request rate, latency, errors, and other system metrics before deciding what action is required.

Use Case: Identify whether the issue is capacity, application performance, database load, or another bottleneck.

15. You need to test whether an application can handle thousands of simultaneous requests. Which tool should you use?

Answer: Use JMeter.

Why: JMeter is designed for load and performance testing.

Use Case: Generate controlled traffic and measure response time, throughput, and error rate.

16. You want to automatically test the login functionality of a web application through a browser. Which tool should you use?

Answer: Use Selenium.

Why: Selenium automates browser interactions.

Use Case: Open the login page, enter username/password, click Login, and validate the expected result.

17. Your Java build creates a JAR file and you need to store different versions centrally. Which tool should you use?

Answer: Use Nexus or another artifact repository such as JFrog Artifactory.

Why: Artifact repositories store build outputs and their versions separately from source code.

Use Case: Store app-1.0.jar, app-1.1.jar, and app-2.0.jar and retrieve a specific version during deployment.

18. Your team wants to deploy the same application to Dev, QA, and Production. What should you package and promote?

Answer: Package the application into a versioned artifact or container image and promote the same build through environments.

Why: Rebuilding separately for each environment can introduce differences.

Use Case: Build once, test the same artifact, and deploy the approved version.

19. Your Kubernetes application has 15 YAML files and installation is becoming difficult. Which tool can help package them?

Answer: Use Helm.

Why: Helm packages Kubernetes resources into reusable charts.

Use Case: Create a Helm chart containing Deployment, Service, ConfigMap, and other resources.

20. A company wants developers to push code and automatically run build, test, and deployment stages. What should you design?

Answer: Design a CI/CD pipeline using a tool such as Jenkins or GitLab CI.

Why: The pipeline automates the software delivery workflow.

Use Case: Git push → build → test → security checks → artifact → deployment.

21. Your Jenkins server builds an application, but the artifact disappears when the workspace is cleaned. What is missing?

Answer: A proper artifact management strategy is missing.

Why: Build artifacts should be stored in a repository such as Nexus instead of depending only on a Jenkins workspace.

Use Case: Jenkins builds the JAR and uploads it to Nexus with a version.

22. Two developers modify the same source file. How will you manage their changes?

Answer: Use Git branches and merging.

Why: Developers can work independently and then integrate their changes through a controlled merge process.

Use Case: Developer A works on feature/login; Developer B works on feature/payment; both eventually merge into the appropriate shared branch.

23. You want every code change to be tested before it can be merged. What approach should you use?

Answer: Use a CI pipeline integrated with Git.

Why: The pipeline can automatically build and run tests for every change.

Use Case: Pull request → CI build → unit tests → quality checks → approval → merge.

24. A company wants to recreate its entire cloud environment after a disaster. Which tool is useful?

Answer: Use Terraform for infrastructure provisioning.

Why: Infrastructure is defined as code and can be recreated from version-controlled configuration.

Use Case: Recreate networks, compute resources, databases, and other supported infrastructure from Terraform code.

25. You need to change the configuration of 500 Linux servers consistently. Which tool is appropriate?

Answer: Use Ansible.

Why: Ansible is designed for configuration management and operational automation.

Use Case: Update configuration files, install packages, restart services, and verify server state across a server group.

26. Your Kubernetes application is running, but users report slow responses. Which tools and data would you check?

Answer: Start with Prometheus and Grafana for metrics and inspect application logs using the organization's logging platform, such as Splunk.

Why: Metrics can reveal CPU, memory, request rate, latency, and resource saturation, while logs can provide application-level errors.

Use Case: Correlate high latency with resource usage and application errors before deciding on remediation.

27. Your AWS EC2 server's CPU suddenly reaches 95%. Which tool can alert you?

Answer: Use CloudWatch.

Why: CloudWatch can collect EC2 metrics and create alarms.

Use Case: Configure an alarm when CPU utilization crosses an agreed threshold for a defined period.

28. Your team is manually copying JAR files from one server to another for every release. What should you change?

Answer: Introduce CI/CD and artifact management using tools such as Jenkins and Nexus.

Why: Jenkins can automate the build/release process and Nexus can centrally store versioned artifacts.

Use Case: Git push → Jenkins build → Nexus upload → deployment pipeline retrieves the approved artifact.

29. Your organization is using many different DevOps tools. How should you decide which tool to learn or introduce?

Answer: Start with the DevOps category and business requirement, then select a tool that fits the environment.

Why: Tools change between organizations, but categories such as source control, CI/CD, containers, IaC, automation, testing, and monitoring remain.

Example: If the requirement is Infrastructure as Code, evaluate Terraform or a cloud-native IaC tool rather than randomly selecting a tool.

30. During an interview, you are asked: "Which tool should I use and why?" What is the best way to answer?

Answer: Do not answer only with a tool name. Explain the problem, category, tool, reason, and use case.

Interview Format

Problem: What problem are we solving?

Category: Which DevOps category does it belong to?

Tool: Which tool would you use?
Why: Why is that tool suitable?

Use Case: How would you implement it?

Alternative: Mention an alternative when relevant.
Example:

"If I need to automate infrastructure provisioning across AWS and GCP, I would consider Terraform because it provides an Infrastructure as Code approach and supports multiple cloud providers. I would keep the Terraform code in Git and use CI/CD to validate and apply infrastructure changes through a controlled workflow."
