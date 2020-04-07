# Ansible_Web_app_flask_with_HAPROXY

Solution for Udemy Course Ansible Advanced

Architecture :

2 Web Servers 
1 Database Server
1 Proxy Server

All targets are running under Debian 9.

Purpose of the playbook : Setup a a flask application with HTTP load balancing

- Install python dependencies on all servers
- Install mysql dependencies on db server
- Create mysql database and user on db server
- Install git on web servers
- Retrieve web app from github (Thanks to mmumshad for the python app)
- Launch flask services
- Install haproxy service on proxy server
- Push haproxy.cfg to proxy server from haproxy.j2 template
- Edit haproxy.cfg to add web_servers IP Address
- Edit haproxy file in /etc/default to enable it
- Start Haproxy

Result :

![HA PROXY STATS ](https://github.com/mrRobotSAS/Ansible_Web_app_flask_with_HAPROXY/blob/master/Screenshots/HAPROXY.png)
