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
