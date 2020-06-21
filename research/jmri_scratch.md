# Setting up JMRI on Raspberry Pi

 - pi 4
 - raspian OS

Based on [instructions](https://www.jmri.org/install/Raspbian.shtml) on JMRI website.

# JMRI Install

So there are several installs for different versions of raspian, need to find out what mine is.

```
pi@raspberrypi:~/Desktop/git_repos/ho_train/research $ cat /etc/os-release
PRETTY_NAME="Raspbian GNU/Linux 10 (buster)"
NAME="Raspbian GNU/Linux"
VERSION_ID="10"
VERSION="10 (buster)"
VERSION_CODENAME=buster
ID=raspbian
ID_LIKE=debian
HOME_URL="http://www.raspbian.org/"
SUPPORT_URL="http://www.raspbian.org/RaspbianForums"
BUG_REPORT_URL="http://www.raspbian.org/RaspbianBugs"
```

Hmm, ok, it looks like Raspian has done some serious upgrades since this page was written.  We'll have to play this by ear a bit.

But first, let's take a look at whether we have java installed.

```
pi@raspberrypi:~/Desktop/git_repos/ho_train/research $ which java
/usr/bin/java
pi@raspberrypi:~/Desktop/git_repos/ho_train/research $ java -version
openjdk version "11.0.3" 2019-04-16
OpenJDK Runtime Environment (build 11.0.3+7-post-Raspbian-5)
OpenJDK Server VM (build 11.0.3+7-post-Raspbian-5, mixed mode)
```

Ok, like OS, I am several versions ahead of what is referenced on site.  Well, let's download the latest linux version and see how it goes.

```
/home/pi/Downloads/JMRI.4.18+R37ad3d0.tgz
```



 