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

Then extract and by (my best understanding of) convention, move to `/opt` directory.

To execute, go to `/opt/JMRI` and enter `./PanelPro` or `./DecoderPro`, per instructions.  Ok, tried it it works, now what is the next step?  Probably need to learn a bit more about the software, and then tackle actually trying to connect the **z21** box.

# Exploring JMRI basics

Based on example in JMRI [setup page](https://www.jmri.org/help/en/html/setup/index.shtml), I am starting with the **DecoderPro** program.

 - asks me to set active profile, chose default "My JMRI Railroad"
 - started wizard
  - changed default owner from `root` to `pi`
  - selected Roco and Z21 from dropdown list in  wizard
   - IP configuration stuff came up, which I don't want to deal with right now
   - so switched to **Z21 Simulator** for now

Ok, program came up with instructions on how to get started.





