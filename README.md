# small_org_network_design

The different departments in our organization are as follows:
•	Managing Director
•	Sales
•	Accounting
•	Purchasing
•	Advertising

Considering security and better functionality, we have divided the original network into several parts, in turn creating several subnets. Each department has an assigned VLAN containing all devices belonging to that department.
The initial IP address 192.168.1.0/24 will be divided into subnets.

For all the devices, the Subnet Mask is 255.255.255.224.
 
The server present in VLAN 50 has been set up as a DNS server (Local DNS). It hosts the web-page www.cleanplanet.com, and all the computers access this webpage by reaching the IP address of the server 192.168.1.130.

To communicate between departments, all traffic must pass through the Internal Router. We have used Router-on-a-stick technique to achieve this.

We also have an SSH-enable router which is connected to an Additional Server. The admin can remotely access this router by entering a pre-set password. SSH is typically used to log in to a remote machine and execute commands, but it also supports tunnelling, and file transfer using the associated SSH file transfer (SFTP) or secure copy (SCP) protocols. SSH uses the client-server model.

