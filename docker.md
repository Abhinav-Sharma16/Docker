### Docker

Docker is a platform that helps developers build, share and run applications with the containers.
Docker basically works for problems like:

### Problem 1
```
 At Developer end:
	Developer made an application which uses services like node, java,etc. That application runs perfectly at developers end. Developer send that application to Testing team for final check before producion phase.

 At Tester end: 
	Tester insatlled that application after around 6months or lets take it as a year. We all know services update their versions with some minor bug fixes and improvements. When the tester 
installed the application it installed with updated version of it services because of which it start creating some issues in application.  
```

### Problem 2
``` 
 At developer and tester end:
	Developer made an application which uses services like node, java,etc. Now that application working perfectly at developer's end. Simultaneously tester also installed that application in same time with 
same version of services as developer was using. Now it will send it to servers for production.

 At Server's end: 
	Servers got the application after like a year. Servers are all ways stays up to date. Again problem occurs that services got latest versions which results in issues in application.
```

There are many more problem occurs for which now almost every company either big or small uses docker.

### Container
A docker container have everything about the project like liberaries, runtime, tools, wuth sepcification version, code.

### Docker installation on Linux

Docker Desktop on Linux runs a Virtual Machine (VM) which creates and uses a custom docker context, desktop-linux, on startup.
This means images and containers deployed on the Linux Docker Engine (before installation) are not available in Docker Desktop for Linux.

### General System Requirements:
To install Docker Desktop successfully, your Linux host must meet the following general requirements:

    > 64-bit kernel and CPU support for virtualization.
    > KVM virtualization support. Follow the KVM virtualization support instructions to check if the KVM kernel modules are enabled and how to provide access to the KVM device.
    > QEMU must be version 5.2 or later. We recommend upgrading to the latest version.
    > systemd init system.
    > Gnome, KDE, or MATE Desktop environment.
    	>> For many Linux distros, the Gnome environment does not support tray icons. To add support for tray icons, you need to install a Gnome extension. For example, AppIndicator
    > At least 4 GB of RAM.
    > Enable configuring ID mapping in user namespaces, see File sharing.
    > Recommended: Initialize pass for credentials management.

### KVM virtualization support

Docker Desktop runs a VM that requires KVM support
The kvm module should load automatically if the host has virtualization support. To load the module manually, run:
```
# modprobe kvm
```
Depending on the processor of the host machine, followwing command will used:
```
# modprobe kvm_intel	//Intel Processors

# modprobe kvm_amd	//AMD Processors
```

