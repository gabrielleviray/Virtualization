# Virtualization

Team: Gabrielle Viray (012340068)

## Initial Setup:
  1. Installed VMware Fusion and Ubuntu 20.04 ISO file.
  2. Create Virtual Machine with 200 GB of Disk Space and Enabled Virtualization.
  3. Download Linux Source Code from Github<br>
     a. Git install in Ubuntu terminal
     ```
     sudo apt-get install git
     ```
     b. Forked linux code from https://github.com/torvalds/linux and cloned to my repo.<br>
     c. Cloned linux repo<br>
     ```
     git clone https://github.com/gabrielleviray/linux.git
     ```
   4. Build Kernel Environment following the guide:https://wiki.ubuntu.com/Kernel/BuildYourOwnKernel
    ```
    sudo apt-get install libncurses-dev gawk flex bison openssl libssl-dev dkms libelf-dev libudev-dev libpci-dev libiberty-dev autoconf
    ```
   5. Download 'Makefile' and 'cmpe283-1.c' from canvas.
      a. ```make```
      b. ```sudo insmod ./cmpe283-1.ko
      c. ```dmesg```

## Implementation
  1. 
