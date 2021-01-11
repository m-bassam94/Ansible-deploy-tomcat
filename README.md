# ansible playbook that deploys tomcat to a vagrant vm

![alt text](https://github.com/m-bassam94/Ansible-deploy-tomcat/blob/master/screenshots/ansible-tomcat-3.png)


### setup ubuntu 18.04 server using vagrant

* vagrant up
* vagrant ssh
* vi .ssh/authorized_keys
* add your host's public key
* ip a and copy vm ip address
* add vm ip address to inventory

### ansible-playbook steps

* update all packages
* install jdk
* create tomcat user & group
* create /opt/tomcat directory
* download and extract tomcat
* change tomcat directory ownership & permissions
* create tomcat systemd service file
* reload systemd daemon
* start tomcat service
* change default port from 8080 to 9999
* restart tomcat service

![alt text](https://github.com/m-bassam94/Ansible-deploy-tomcat/blob/master/screenshots/ansible-tomcat-1.png)
![alt text](https://github.com/m-bassam94/Ansible-deploy-tomcat/blob/master/screenshots/ansible-tomcat-2.png)
