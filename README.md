# install-mysql-redis-and-rabbitmq-with-ansible-on-docker

Before launching the vagrantfile, please read this file and do the next steps.
1. Install vagrant latest version on operating system (e.g windows)
2. Install a virtualization tool like virtualbox 
3. Copy the attached files to appropriate path (e.g: E:/vagrant/ansible)
-	Before launching the vagrantfiles, please change vagrantfiles and set the path of step 3 
4. Launch 3 virtual machines using vagrantfiles
5. Please configure ssh no password between 3 machines. (if it's required, change /etc/ssh/sshd_config file for enabling ssh connection)
-	Configure ssh no password on these ip addresses
o	Node1 to node1 : root@127.0.0.1
o	Node1 to node1 : root@10.1.1.11
o	Node1 to node2 : root@10.1.1.12
o	Node1 to node3 : root@10.1.1.13
6. for checking the rabbitMQ cluster state, by using browser, check the bellow address
-	127.0.0.1:15672
-	username: rabbit
-	password: rabbitPass
7. for checking the state of redis and mysql services, please connect to the container and check state of the services.

Notice: Mysql cluster, and RabbitMQ cluster are implemented on node1 and redis is implemented on node1, node2 and node3.
