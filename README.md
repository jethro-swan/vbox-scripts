### VirtualBox headless management scripts

Some extremely simple scripts to create and manage headless VirtualBox VM.

(Adapted from scripts originally provided by Bob Hutchinson https://github.com/arwystli)

#### Create a VirtualBox VM

vbox_install <name of VM> <RDP port> <memory allocation>
e.g.
```
vbox_install crun15 3445 8192
```

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
