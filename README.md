# WSL-Linux-Drive-Installer
script and guide about how to mount drives with linux filesystem on windows using wsl

# Summary
* Prerequisites
* Hard-drive installation
* Donation

# Prerequisites
* Linux subsystem on windows
* WSL2
 
# Hard-drive installation

To install the hard drive you have to run the following command in powershell:
```

GET-CimInstance -query "SELECT * from Win32_DiskDrive"

```

search for the first column your device. Before mounting the device, make sure that you have wsl2 in your enviroment:
```
wsl --version

```

It should show you wsl version: 2, if not then set wsl as the following:
```
wsl --set-default-version 2

```

Then you need to mount the device on wsl:
```

wsl --mount <value first column> --bare

```

This will mount the device. Run your linux distro on wsl and then check the device running:
```
lsblk

```

When you have found the device, use the **mount** command in the /mnt folder.

# Donation

If you did find this guide usefull, please donate me at the following paypal address:

```
https://www.paypal.me/francescodisales
```

Or if you want to donate in cryptocurrencies, you can donate at the following Monero address:

```
4B9WQivaHfd3miDfPKEfCianocGpBx9d8FXycz2vmNW3aBDVKHgkBd9Gmapt4RBVEpTwnehujsiUBBehUiLvnEHs7VFstCC
```





