# ansible-nginx

For docker image test machine
```sh
echo 'root:P@ssw0rd' | chpasswd
sed -i 's/PermitRootLogin no/PermitRootLogin yes/' /etc/ssh/sshd_config
sed 's@session\s*required\s*pam_loginuid.so@session optional pam_loginuid.so@g' -i /etc/pam.d/sshd
apt-get update
apt-get install -y net-tools
apt-get install -y openssh-server
service ssh on
service ssh start
```