
# vpick

It is a command-line tool designed for backing up and restoring mobile system information, enabling users to transfer system parameters from a physical device to a cloud-based phone.

# How to use

## 1 unpackage
1. adb push vpick-1.0.5.tar.gz /data/local/tmp/
2. adb shell tar -zxvf vpick-1.0.5.tar.gz
3. cd vpick-1.0.5
4. chmod 777 *.sh
## 2 install
./install.sh
reboot


after reboot, a process named vpkd is automatically pulled up, and the vpick command line tool is supported
## 3 uninstall
./uninstall.sh

## pick phone info from real phone
1.download release packages vpick-V1.0.5-win64.tar.gz
2.unpacke and enty it from cmd line
3.plugin your phone
4.exec adbdevices.bat #to show you phone's hardware serialno
5.exec setsn.bat <serialno> #to set target device
6.exec vpick.bat   # pick the phone's info
7.once finished, the target foulder "vpk" will open 
