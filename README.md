# ssh-enable
SSH enable, to get access to communicate with another SBC .


As root, edit the sshd_config file in /etc/ssh/sshd_config: nano /etc/ssh/sshd_config  

Add a line in the Authentication section of the file that says  

PermitRootLogin yes.  

This line may already exist and be commented out with a "#". In this case, remove the "#".

# Authentication: 
#LoginGraceTime 2m 
PermitRootLogin yes 
#StrictModes yes 
#MaxAuthTries 6 
#MaxSessions 10  

 

Save the updated /etc/ssh/sshd_config file.  

Restart the SSH server: service sshd restart 

//i followed these steps to establish a connection, correct me if am wrong
