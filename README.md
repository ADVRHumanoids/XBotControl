# XBotControl
XBotControl framework: XBotCore + OpenSoT + CartesI/O

**XBotCore** slides available [here](https://www.dropbox.com/s/ojwruiax6r2k53z/XBotCore_Tutorial_IROS_19.pdf?dl=0).

**OpenSoT** slides available [here](https://docs.google.com/presentation/d/1kwJsAnVi_3ADtqFSTP8wq3JOGLcvDV_ypcEEjPHnCEA/edit#slide=id.p).

**CartesI/O** slides available [here](https://docs.google.com/presentation/d/1bmeKwGsyhoEIW_Wd05ITrp71J0FMkANDNeZTTDXzfJ4/edit#slide=id.p).

XBotControl Tutorial available at https://github.com/ADVRHumanoids/tutorial_iros2018

# Install

Supported Operating System: **Ubuntu 16.04**

Since XBotControl comes with built-in ROS support, you should first install and configure ROS kinetic as described here http://wiki.ros.org/kinetic/Installation/Ubuntu


Download the release version you want to install from https://github.com/ADVRHumanoids/XBotControl/releases

For example, if I want to install XBotControl 1.0.1 I will do the following:

```
wget https://github.com/ADVRHumanoids/XBotControl/releases/download/v1.0.1/XBotControl_1.0-1.deb
sudo apt-get install gdebi # utility that lets you install local deb packages resolving and installing its dependencies.
sudo gdebi XBotControl_1.0-1.deb
```

# Configure

First of all source the XBot setup.bash

```
. /opt/xbot/build/install/share/xbot/setup.bash
```

You can check that the sourcing has effect in your bash terminal by echoing the $XBOT_ROOT env variable.

```
echo $XBOT_ROOT
```

The answer should be:

```
/opt/xbot/build/install/share/xbot
```

Remember to source in each of the terminal you are using or to put the source command in your .bashrc

Later on you can set YOUR_CONFIG_YAML (e.g. /home/embedded/configs/my_robot.yaml): this is going to be used in the following XBotCore executions.

```
set_xbot_config YOUR_CONFIG_YAML
````


# Uninstall

```
sudo dpkg -P xbotcontrol
```

