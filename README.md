# AWSECSRoot
切换root权限并开启密码ssh登录root账户

以用户名centos登录
```
sudo passwd root

su

curl https://raw.githubusercontent.com/HXHGTS/AWSECSRoot/master/sshd_config_centos7 > /etc/ssh/sshd_config

/sbin/service sshd restart

```

[AWS官方说明](https://docs.aws.amazon.com/zh_cn/AWSEC2/latest/UserGuide/managing-users.html)

[AWS开启ipv6](https://docs.aws.amazon.com/zh_cn/vpc/latest/userguide/get-started-ipv6.html)
