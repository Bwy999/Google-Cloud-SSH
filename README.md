# 使用 Termius 登录 Google Cloud

**1.设置 root 密码**

- 先从浏览器打开 Google Cloud 控制台ssh连接服务器

- 输入代码 sudo -i，进入Root

- 输入代码 passwd ，输入新密码，然后回车，然后再重复一次密码，回车。**(输入密码的时候不会显示出来）**


**2.开启 Google Cloud SSH 权限**

- CentOS/Debian 系统，输入以下两条命令

    sed -i 's/PermitRootLogin no/PermitRootLogin yes/g' /etc/ssh/sshd_config

    sed -i 's/PasswordAuthentication no/PasswordAuthentication yes/g' /etc/ssh/sshd_config

- Ubuntu 系统，输入以下两条命令

    sed -i 's/#PermitRootLogin prohibit-password/PermitRootLogin yes/g' /etc/ssh/sshd_config

    sed -i 's/PasswordAuthentication no/PasswordAuthentication yes/g' /etc/ssh/sshd_config

**3.重启服务器**

   - reboot

**4.Terminus iOS 客户端设置**


**5.完成✅**



