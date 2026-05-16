


### Installing drivers

https://discourse.ubuntu.com/t/how-to-install-newer-nvidia-driver-when-software-updates-wont-let-you/69352


```
ubuntu-drivers devices

ubuntu-drivers list

sudo ubuntu-drivers install nvidia-driver-595-open
sudo ubuntu-drivers autoinstall
```




### Network issue

#### 20260516

Network config is fine, but lost all network devices.

* Check status: `nmcli general status`


Bring back network: Use GRUIB to boot into older kernel using advanced boot options on boot.
```
sudo apt update
sudo apt upgrade
sudp apt dist-install
uda # my alias
sudo ubuntu-drivers autoinstall
uname -r # get dist version
```
Before robooting 6.17.0-23-generic