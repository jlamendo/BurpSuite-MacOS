BurpSuite-MacOS
===============

Build a MacOS .app wrapper for a user provided BurpSuite jar. 
This will allow Burp Suite to function as a traditional Mac app, with standard behaviour as far as the dock/mission control goes.

Screenshot of what it looks like running in the taskbar:
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
