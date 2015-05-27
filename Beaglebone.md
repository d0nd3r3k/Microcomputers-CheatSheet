ssh root@192.168.7.2
passwd
adduser foo
usermod -a -G sudo foo
visudo
exit

ssh foo@192.168.7.2
