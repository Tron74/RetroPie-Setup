RetroPie-Setup 4.6 for RockPro64
==============

General Usage
-------------

Original RetroPie 4.6 Shell script modified to work on RockPro64 running Ubuntu (Armbian 20.02.1 Bionic) with many emulators and games, using EmulationStation as the graphical front end.

This script is designed for use on Raspbian on the Raspberry Pi, OSMC on the Vero4K or Ubuntu on the ODroid-C1 or a PC, and now for RockPro64.

To run the RetroPie Setup Script make sure that your APT repositories are up-to-date and that Git is installed:

```shell
sudo apt-get update
sudo apt-get dist-upgrade
sudo apt-get install git
```

Then you can download the latest RetroPie setup script with

```shell
cd
git clone --depth=1 https://github.com/RetroPie/RetroPie-Setup.git
```

The script is executed with 

```shell
cd RetroPie-Setup
sudo ./retropie_setup.sh
```

When you first run the script it may install some additional packages that are needed.

Binaries and Sources
--------------------

On the Raspberry Pi, RetroPie Setup offers the possibility to install from binaries or source. For other supported platforms only a source install is available. Installing from binary is recommended on a Raspberry Pi as building everything from source can take a long time.

For more information visit the blog at https://retropie.org.uk or the repository at https://github.com/RetroPie/RetroPie-Setup.

Wiki
----

You can find useful information about several components or for several frequently asked questions in the [wiki](https://github.com/RetroPie/RetroPie-Setup/wiki) of the RetroPie Script. If you think that there is something missing, you are invited to add it to the wiki.


Thanks
------

This script just simplifies the usage of the great works of many other people that enjoy the spirit of retrogaming. Many thanks go to them!

# Information for RockPro64

Requirements:

# Core
```shell
sudo apt install libusb-1.0-0-dev libavcodec-dev libavformat-dev libavdevice-dev
sudo cp ./rock64-addon/usr / -r
sudo cp ./rock64-addon/opt / -r
sudo cp ./rock64-addon/etc / -r
```

# Emulator - main  - mupend64plus
```shell
apt-get install libxmu-dev libxmu-headers freeglut3-dev libxext-dev libxi-dev
```

# Driver - snesdev
```shell
apt install make libconfuse-dev
```

