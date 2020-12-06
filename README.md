# BPC-UIN_dcnn_example

## Clone GIT repository

First update repositories.
```
$ sudo apt-get update
```

Try, if the git is installed on your system
```
$ git --version
```

If not, install it by 
```
$ sudo apt install git
```

Now move to the directory, where you want to clone (download) the repository, and type
```
$ git clone https://github.com/adamek727/BPC-UIN_dcnn_example.git
```

Now the new "BPC-UIN_dcnn_example" directory was created with all the files inside.


## Installing virtual environment

For Mac and Windows, please see official installation documentation. 

For Linux follows the tutorial below.

Choose your distribution: [anaconda](https://www.anaconda.com/products/individual)


Download the anaconda installation script. (In future the name of the install script will be different. Change it to the current version.)
```
$ cd /tmp
$ wget https://repo.anaconda.com/archive/Anaconda3-2020.02-Linux-x86_64.sh
```

Run installation script.
```
$ bash Anaconda3-2020.02-Linux-x86_64.sh
```

At the end of installation the following messages may apear:

```
Do you wish the installer to initialize Anaconda3
by running conda init? [yes|no]
```

```
installation finished.
Do you wish the installer to prepend the Anaconda3 install location
to PATH in your /home/user/.bashrc ? [yes|no]
```
TyFor both type yes.

Test the installation:
```
$ source ~/.bashrc
$ conda info
```
You should get the conda info output. CG!


## Creating virtual environmnet

Build the virtual environment from the yaml file.
```
$ conda env create -f requirements.yml
```
This process takse several minutes. 

If the build was successful, activate the environment by
```
$ conda activate bpc-uin-dcnn
```

Now the bash should look like 
```
(bpc-uin-dcnn) my_pc@my_account:~/BPC-UIN_dcnn_example $
```
That means, we are now using the tools intalled in the virtual environment sandbox. CG!

## Running examples

In the directory, that where the example files are (fully.connected.ipynb and dcnn.ipynb), run Jupyter.
```
$ jupyter notebook
```

The web browser should open.

[Jupyter](https://jupyter.org/) is a tool for python prototyping. It runs the web server, and allows you to execute Python code in a separated blocks.

In the web page select the fully_connected of the dcnn example file

By pressing the Shit + Enter, you can execute the code. Feel free to modify the code, and to experiment with the NNs.

## Next Step

More Keras tutorials: [Here](https://keras.io/examples/)

If you are interested in NNs more, see the [Pytorch](https://pytorch.org/), the powerfull framework to work with complex NNs.
