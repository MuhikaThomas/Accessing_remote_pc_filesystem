[In this case i am using Debian]
* HOW TO ENABLE TELNET IN Debian

Open the terminal [ctrl + alt + t]
Run the following commands

#sudo apt-get install xinetd telnetd

The Telnet service is started automatically once the installation is done. And you can either run telnet serverip or use a Telnet client (PuTTy, SecureCRT, etc.) to access this server.

#telent "serverip"

To change the port (default is 23), edit the /etc/services file with your favorite text editor. Find out and change the number in the line below:

telnet        23/tcp

To apply changes, you have to restart the service by running the command below:
#sudo /etc/init.d/xinetd restart 




[Mossein King]
