# aws_study-+
```
#!/bin/bash
echo 'Port (포트 번호)' >> /etc/ssh/sshd_config
systemctl restart sshd
sed -i "s/PasswordAuthentication no/PasswordAuthentication yes/g" /etc/ssh/sshd_config
echo "<AMI 이름>:<비밀번호>" | chpasswd
systemctl restart sshd
```
