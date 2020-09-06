# AWSECSRoot
切换root权限并开启密码ssh登录root账户

```
sudo passwd root

su

sudo sed -i '/PasswordAuthentication/d;/PermitRootLogin/d' /etc/ssh/sshd_config

echo "PasswordAuthentication yes" >> /etc/ssh/sshd_config

echo "PermitRootLogin yes" >> /etc/ssh/sshd_config

sudo /sbin/service sshd restart
```

