Comprehensive list of projects to practice DevOps concepts
1. Linux Servers - Vagrant 
- Setup website using Apache2 (HTTP server) on CentOS VM
- Setup LAMP/Wordpress on Ubuntu VM
- Setup both using VM provisioning- Automating the tasks
- Setup VM automation locally with Vprofile project
- Systemctl, systemd and creation of config file in /etc/systemd/system/ for services(Apache Tomcat 10)
- Deploying Java based Multi-tier webapp on local VMs using Vagrant. Services: Mariadb(MYSQL), Memcached(Database cache), RabbitMQ(Queueing agent), Apache Tomcat(Java servlet container), NGINX(Frontend load balancer)
- Bash Script. Websetup on remote host using SSH command. Setting up ssh-keys on CentOS and Ubuntu
- Jenkins:
1. Jenkins installation on EC2 instance (JDK required)
2. Jenkins installation on docker container
3. Jenkins jobs. Creating first Freestyle job
4. Installing tools like maven, JDK on Jenkins server
5. Installing plugins and updating the configuration in System Global settings
6. Artifact versioning using Environment variables and parameters passed to the job.
7. Continuous Integration Pipeline using Declarative Pipeline. Here we also setup sonarQube for code analysis, Nexus for uploading artifact, on AWS EC2. Also integrating with Slack for post build notifications.