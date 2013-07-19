# Darts

**Darts** is a web app for calculating scores, tracking history and assiting with multiple darts games.

## Requirements

* VirtualBox - Free virtualization software [Downloads](https://www.virtualbox.org/wiki/Downloads)
* Vagrant - Tool for working with virtualbox images [Vagrant Home](https://downloads.vagrantup.com)
* Git - Source Control Management [Downloads](http://git-scm.com/downloads)

## Installation

- Clone darts repo   
  `git clone https://github.com/JJCLane/darts.git`  
  `cd darts`
- Run vagrant   
   `vagrant up`
- Wait while it pulls in everything necessary (this can take a while the first time)


## Usage

- Navigate to [http://localhost:8080](http://localhost:8080)
- SSH access (use putty for Windows see below)   
   `vagrant ssh`
- Shut down virtual machine   
   `vagrant halt`


### SSH access (Windows putty)

- Locate ssh private key   
   `C:\Users\example_user\.vagrant.d\insecure_private_key`
- Load ssh private key in [puttygen](http://the.earth.li/~sgtatham/putty/latest/x86/puttygen.exe)   
   Select all files if you cannot find it
- Click `Save private key`   
   Press `Yes` if it asks about saving without a password  
   Save it anywhere (though the same folder makes sense)
- Open [putty](http://the.earth.li/~sgtatham/putty/latest/x86/putty.exe) and enter details displayed when using ssh command   
   `vagrant ssh`
- In the left categories section navigate to   
   `Connection > SSH > Auth`
- Click on browse and select the private key generated earlier
- Now you can connect by pressing open at the bottom
- If you would like this to be saved for next time   
   Navigate back to `Session`  
   Give it a name  
   Click on save
