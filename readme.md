Item Catalog


#### 1-Use a terminal
we recommend using the Git Bash terminal that comes with the Git software. If you don't already have Git installed, download Git from 
git-scm.com.

### 2-install virtual box from this link
Install the platform package for your operating system. You do not need the extension pack or the SDK. You do not need to launch VirtualBox after installing it; Vagrant will do that.

https://www.virtualbox.org/wiki/Download_Old_Builds_5_1

### 3-Install Vagrant
Vagrant is the software that configures the VM and lets you share files between your host computer and the VM's filesystem. Download it from 
https://www.vagrantup.com/downloads.html

. Install the version for your operating system.


### 4-Download the VM configuration
There are a couple of different ways you can download the VM configuration.

You can download and unzip this file: 
https://s3.amazonaws.com/video.udacity-data.com/topher/2018/April/5acfbfa3_fsnd-virtual-machine/fsnd-virtual-machine.zip
This will give you a directory called FSND-Virtual-Machine. It may be located inside your Downloads folder.

Note: If you are using Windows OS you will find a Time Out error, to fix it use the new Vagrant file configuration:
https://s3.amazonaws.com/video.udacity-data.com/topher/2019/March/5c7ebe7a_vagrant-configuration-windows/vagrant-configuration-windows.zip

to replace you current Vagrant file.
to start the program navigate to its folder using
cd <path>
    
 Change to this directory in your terminal with cd. Inside, you will find another directory called vagrant. Change directory to the vagrant directory:
 
Start the virtual machine
From your terminal, inside the vagrant subdirectory, run the command vagrant up. This will cause Vagrant to download the Linux operating system and install it. This may take quite a while (many minutes) depending on how fast your Internet connection is.

When vagrant up is finished running, you will get your shell prompt back. At this point, you can run vagrant ssh to log in to your newly installed Linux VM!

Next You Should Install python, but don't worry... it's already installed in the vm

first Launch Vagrant using Git
```
$  Vagrant up 
```
---------------
Login to Vagrant
```
$ Vagrant ssh
```
---------------
Change directory to /vagrant
```
$ Cd /vagrant
```
---------------
Initialize the database
```
$ Python database_setup.py
```
---------------

Populate the database with some initial data
```
$ Python lotsofdata.py
```
---------------
Launch application
```
$ Python final.py
```
---------------
Open the browser and go to http://localhost:5000

JSON endpoints:-
Returns JSON of all Catagories With Their Items
```
/category/JSON
```

Returns JSON of Only Categories
```
/category/only/JSON
```
Returns JSON of All Items Of Specific Category
```
/category/<int:category_id>/item/JSON
```
 ------------------------------------------------
 
 ### Refrences :
 stackoverflow.com
 udacity.com