# jenkins area

- [持续集成 Jenkins 视频教程全集（22P）| 1 小时从入门到精通](https://www.bilibili.com/video/av59639803/)
- [pipeline 视频教程](https://www.bilibili.com/video/av56547404/)
- [pipleline git commit trigger](https://blog.csdn.net/qq_30758629/article/details/93353437)
- [pipeline/getting-started](https://jenkins.io/zh/doc/book/pipeline/getting-started/)

## 安装&配置

- [macOS Jenkins安装&配置](https://www.jianshu.com/p/9dc3b45fbbec)
- [Creating & Managing multiple users in Jenkins](https://medium.com/@anusha.sharma3010/creating-managing-multiple-users-in-jenkins-b68ba7dc0810)

1. Create First Admin User
    - Username: nate
    - Password: 1234
    - Confirm password: 1234
    - Full name: Nate Xu
    - E-mail address: nate.xu@everbridge.com

2. default admin password

```
sudo less /Users/Shared/Jenkins/Home/secrets/initialAdminPassword
```

## 常用命令

[HOW TO: Start, Stop, Restart or Reload Jenkins – Mac OSx](http://damien.co/general/how-to-start-stop-restart-or-reload-jenkins-mac-osx-8022)


### How to Stop, Restart Jenkins – Common URL options URL’s to stop or restart Jenkins

`http://[jenkins-server]/[command]` where [command] can be

- exit shutdown jenkins

- restart restart jenkins

- reload to reload the configuration

### Terminal and Kill Process

```bash
ps -e | grep jenkins

53 ?? 0:02.51 /usr/bin/java -jar /Applications/Jenkins/jenkins.war 392 ttys000 0:00.00 grep jenkins

$ sudo kill 53
```

### Terminal and Start / Stop daemon

You want to use launchctl to start and stop Jenkins.

- Start Jenkins: `sudo launchctl load /Library/LaunchDaemons/org.jenkins-ci.plist`

- Stop Jenkins: `sudo launchctl unload /Library/LaunchDaemons/org.jenkins-ci.plist`

### How to change default port on Jenkins from default to custom on Mac (OS X EL Captain)

- http://regeda.net/2016/07/06/how-to-change-default-port-on-jenkins-from-default-to-custom-on-mac/


## 卸载

```bash
$/Library/Application\ Support/Jenkins/Uninstall.command
```
https://stackoverflow.com/questions/44005592/how-to-uninstall-jenkins-on-mac-completely?rq=1
