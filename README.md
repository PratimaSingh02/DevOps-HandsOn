Comprehensive list of projects to practice DevOps concepts
1. Linux Servers - Vagrant 
- Setup website using Apache2 (HTTP server) on CentOS VM
- Setup LAMP/Wordpress on Ubuntu VM
- Setup both using VM provisioning- Automating the tasks
- Setup VM automation locally with Vprofile project
- Systemctl, systemd and creation of config file in /etc/systemd/system/ for services(Apache Tomcat 10)
- Deploying Java based Multi-tier webapp on local VMs using Vagrant. Services: Mariadb(MYSQL), Memcached(Database cache), RabbitMQ(Queueing agent), Apache Tomcat(Java servlet container), NGINX(Frontend load balancer)
- Bash Script. Websetup on remote host using SSH command. Setting up ssh-keys on CentOS and Ubuntu
  
2. Jenkins:
- Jenkins installation on EC2 instance (JDK required)
- Jenkins installation on docker container
- Jenkins jobs. Creating first Freestyle job
- Installing tools like maven, JDK on Jenkins server
- Installing plugins and updating the configuration in System Global settings
- Artifact versioning using Environment variables and parameters passed to the job.
- Continuous Integration Pipeline using Declarative Pipeline. Here we also setup sonarQube for code analysis, Nexus for uploading artifact, on AWS EC2. Also integrating with Slack for post build notifications.
- Deploying the Vprofile app on AWS ECS by using AWS ECR for storing the docker image of this app.
- Agents in Jenkins. How to add agents. Run job on a node/agent.
- Authentication and Authorization on Jenkins for multiple users.

3. GitHub Actions
- Workflows, Jobs, Steps, Runner (mainly Ubuntu), Action(reusuable automation code) YAML
-  Use cases: CI/CD, Testing, Code analysis, etc
- Environment (dev, QA, staging, production), secrets and variables
- Defining variables in the workflow (main.yml)
- Triggers: Push, Pull request, workflow dispatch (schedule)
- CI/CD: Building, testing, scanning the vprofile app. Building, tagging and publish the docker image to Amazon ECR using avaialble actions and code. Storing IAM access keys for ECR in secrets.

4. GitLab
- GitLab Introduction: SCM, CICD, Security, Registry & Repository, Monitoring & Analaytics, Project & Team management
- Users, Groups, Projects
- Connect local system to GitLab with ssh keys
- Runners, Executors (Docker and Shell)
- CI Pipeline
- Triggers & Rules
- Code scanning stage with Trivy 
- Build and publish docker image on GitLab Container Registry
- DevSecOps: Shift Left approach, SAST, DAST, SCA, IAST, API security
- Enterprise level tools for implementing DevSecOps
- Implement SAST in GitLab Pipeline using SonarCloud(SaaS)
- Add quality gates to SAST job in the pipeline to fail the build if quality gate fails. Set thresholds in quality gate to pass/fail.
- Software Composition Analysis using Snyk. Criteria to integrate Snyk with GitLab Pipeline.
- Dynamic Application Security Testing (DAST) using OWASP ZAP tool
- Reporting the results on JIRA
- DAST and SAST analyzers by GitLab Premium

5. Containerization with Docker
- What is containerization? How is it different from virtualization?
- Docker engine, docker CLI, docker compose
- Docker commands
- Multistage Dockerfile in YAML
- Containerizing Vprofile app on ubuntu VM and pushing the docker images to dockerhub registry
- Containerizing an EMart application that uses Angular(Client), Nginx(Loadbalancer), NodeJS(API), Java(BooksAPI), MongoDB(NoSQL db), MySQL- using docker compose

3. Kubernetes (K8s)
- What is K8s?
- K8s basic architecture: master and worker nodes
- Master processes: KubeAPI, Controller Manager, Scheduler
- ETCD: Cluster brain
- Worker processes: Kubelet, Container Runtime Environment (CRE), Kube Proxy
- KubeCTL: Command line utility to connect to K8s API server (KubeAPI)
- K8s components: Deployments, Pods, Service, ConfigMap, Secret
- Using Minikube to create one-node cluster. We use Docker as our virtualization driver
- KubeCTL basic commands
- Writing K8s configuration files for deployment, service
- Setting up MongoDB and MongoExpress using K8s components with configuration files
