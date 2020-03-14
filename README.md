### VirtualBox headless management scripts

Some extremely simple scripts to create and manage headless VirtualBox VM (adapted from scripts originally provided by Bob Hutchinson https://github.com/arwystli).

In due course the intention is to combine these into a single script with a rich set of options, but for the time being they work as needed.

### Install VBoxManage and the VirtualBox Extension Pack

The download page for Linux versions is at https://www.virtualbox.org/wiki/Linux_Downloads

After installing VBoxManage download the VirtualBox Extension Pack from https://www.virtualbox.org/wiki/Downloads and install it following the instructions at https://www.virtualbox.org/manual/ch01.html#intro-installing which is necessary to provide the RDP interface necessary for installation.

### The scripts

#### Create a VirtualBox VM

vbox_install <name of VM> <RDP port> <memory allocation>
e.g.
```
vbox_install crun15 3445 8192
```
  
You will need to download appropriate .iso files and edit this script to point to the correct location.

(This script will be modified in due course to allow selection of OS and version as parameters.)

#### Save the execution state of a running VM

e.g.
```
savevm crun15
```

#### Stop VM without saving state

e.g.
```
stopvm crun15
```

#### Start VM (whether or not state has been saved)

e.g.
```
startvm crun15
```

#### Restart VM

e.g.
```
restartvm crun15
```

#### List running VM

e.g.
```
listvm
```

#### Show information about VM

e.g.
```
showinfovm crun15
```

#### Unregister and delete a VM

e.g.
```
deletevm crun15
```
