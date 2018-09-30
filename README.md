# XBotControl
XBotControl framework: XBotCore + OpenSoT + CartesI/O

# Install

Download the release version you want to install from https://github.com/ADVRHumanoids/XBotControl/releases

For example, if I want to install XBotControl 1.0.0 I will do the following:

```
wget https://github.com/ADVRHumanoids/XBotControl/releases/download/1.0.0/XBotControl_1.0-0.deb
sudo apt-get install gdebi # utility that lets you install local deb packages resolving and installing its dependencies.
sudo gdebi XBotControl_1.0-0.deb
```

# Configure

```
. /opt/xbot/build/install/share/xbot/setup.bash
set_xbot_config YOUR_CONFIG
```

# Uninstall

```
sudo dpkg -P xbotcontrol
```

# Try it with no installation!

Thanks to our collaboration with [The Construct Sim LTD](http://www.theconstructsim.com/), you are able to run the XBotControl framework on your browser using ROS Development Studio at this [link](https://rds.theconstructsim.com/tc_projects/use_project_share_link/b1c6f2c1-2964-4d52-90e7-ae267383a9b6).
