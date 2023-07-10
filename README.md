# OAI_N310_Conf
### Building and Installing the USRP Open-Source Toolchain (UHD) on With Ubuntu 20.04
Using the following Link: https://kb.ettus.com/Building_and_Installing_the_USRP_Open-Source_Toolchain_(UHD_and_GNU_Radio)_on_Linux
1. Update and Install dependencies for UHD and GNU Radio.

```
sudo apt-get update
sudo apt-get -y install autoconf automake build-essential ccache cmake cpufrequtils doxygen ethtool fort77 g++ gir1.2-gtk-3.0 git gobject-introspection gpsd gpsd-clients inetutils-tools libasound2-dev libboost-all-dev libcomedi-dev libcppunit-dev libfftw3-bin libfftw3-dev libfftw3-doc libfontconfig1-dev libgmp-dev libgps-dev libgsl-dev liblog4cpp5-dev libncurses5 libncurses5-dev libpulse-dev libqt5opengl5-dev libqwt-qt5-dev libsdl1.2-dev libtool libudev-dev libusb-1.0-0 libusb-1.0-0-dev libusb-dev libxi-dev libxrender-dev libzmq3-dev libzmq5 ncurses-bin python3-cheetah python3-click python3-click-plugins python3-click-threading python3-dev python3-docutils python3-gi python3-gi-cairo python3-gps python3-lxml python3-mako python3-numpy python3-numpy-dbg python3-opengl python3-pyqt5 python3-requests python3-scipy python3-setuptools python3-six python3-sphinx python3-yaml python3-zmq python3-ruamel.yaml swig wget
```
#### Building and installing UHD from source code.
UHD is open-source, and is hosted on GitHub. You can browse the code online at the link below, which points to version 4.4.0.0, which is the the latest release at the time of this writing.

```
cd $HOME
mkdir workarea
cd workarea
git clone https://github.com/EttusResearch/uhd
cd uhd
git tag -l
git checkout v4.4.0.0 #For UHD 4.4.0.0
```
