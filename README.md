BurpSuite-MacOS
===============

Build a MacOS .app wrapper for a user provided BurpSuite jar. 
This will allow Burp Suite to function as a traditional Mac app, with standard behaviour as far as the dock/mission control goes.

Screenshot of what it looks like running in the dock:
![](https://i.cloudup.com/LmI3sxDnFP.png)

By default, the build script assumes you are using the Burp Suite Professional.app directory to store all burp peripherals, such as bapps, log files, tmp directory, etc, and will copy them from the previous install into the new build.

To remove this feature, comment out lines 67-88 in build.xml.

Version and shortversion in build.xml are set for the latest version of burp.

Build Instructions: 

```bash
$ git clone git@github.com:liftsecurity/BurpSuite-MacOS.git
$ cd BurpSuite-MacOS
$ echo export "JAVA_HOME=\$(/usr/libexec/java_home)" >> ~/.bash_profile
$ cp {Full Path to burpsuite_pro_x.jar} ./burpsuite.jar
$ ant bundle
```


# 编译BurpSuite破解版为Mac Applocation

## 一、为什么要把BurpSuite破解版编译为Mac Applocation

优雅的装逼

## 二、系统环境
### java
 安装步骤：
 
 。。。。不知道如何安装java，那就放弃吧！
### ant
#### 安装步骤

安装brew

```
https://brew.sh/
```
brew 执行安装命令

```
brew install ant

```
 


## 三、详细步骤
首先从github上下载代码：

```
git clone https://github.com/iusky/BurpSuite-MacOS
```

然后进入该目录,直接执行

```
ant bundle
```

然后会在当前目录下生成一个名字为

```
Burp Suite Professional.app
```
的应用，直接将该应用复制到应用目录即可使用

## 四、更改了哪些参数？

1、更改了build.xml文件里面的mainclassname,将其改为了burploader的启动函数
2、将burp破解版的程序拷贝到了当前目录
3、更改了icon图标

