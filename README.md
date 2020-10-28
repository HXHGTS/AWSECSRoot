# AWSECSRoot
切换root权限并开启密码ssh登录root账户

```
sudo passwd root

su

sed -i '/PasswordAuthentication/d;/PermitRootLogin/d' /etc/ssh/sshd_config

echo "PasswordAuthentication yes" >> /etc/ssh/sshd_config

echo "PermitRootLogin yes" >> /etc/ssh/sshd_config

/sbin/service sshd restart
```

[AWS官方说明](https://docs.aws.amazon.com/zh_cn/AWSEC2/latest/UserGuide/managing-users.html)
