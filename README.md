# BPC-UIN_dcnn_example

## Installing virtual environment

For Mac and Windows, please see official installation documentation. 

For Linux follows the tutorial below.

Choose your distribution: [anaconda](https://www.anaconda.com/products/individual)

Update repositories and install curl tool.
```
$ sudo apt-get update
$ sudo apt-get install curl
```

Download the anaconda installation script. (In future the name of the install script will be different. Change it to the current version.)
```
$ cd /tmp
$ curl –O https://repo.anaconda.com/archive/Anaconda3-2020.02-Linux-x86_64.sh
```

Run installation script.
```
$ bash Anaconda3-2020.02-Linux-x86_64.sh
```

At the end of installation the following message will apear:
```
installation finished.
Do you wish the installer to prepend the Anaconda3 install location
to PATH in your /home/user/.bashrc ? [yes|no]
```
Type yes.

Test the installation:
```
$ source ~/.bashrc
$ conda info
```
You should get the conda info output. CG!


## Creating virtual environmnet

