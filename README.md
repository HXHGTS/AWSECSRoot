# AWSECSRoot
切换root权限并开启密码ssh登录root账户

```
sudo passwd root

su

sudo vi /etc/ssh/sshd_config

PasswordAuthentication yes

PermitRootLogin yes

sudo /sbin/service sshd restart
```

