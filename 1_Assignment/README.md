# Virtualization

Team: Gabrielle Viray (012340068)

## Steps to Complete the Assignment

### Initial Steps(Setup)
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
   4. Build Kernel Environment following the guide: https://wiki.ubuntu.com/Kernel/BuildYourOwnKernel<br>
      ```
      sudo apt-get install libncurses-dev gawk flex bison openssl libssl-dev dkms libelf-dev libudev-dev libpci-dev libiberty-dev autoconf
      ```
    
   5. Download "Makefile" and "cmpe283-1.c" from canvas.
      a. Make
      ```make```
      b. Insert module
      ```sudo insmod ./cmpe283-1.ko```
      c. Display messages
      ```dmesg```

### Implementation
  1.  In cmpe283-1.c, I added 4 Control MSRs below:
      - Primary Proccessor-Based Control
      - Secondary Proccessor-Based Control
      - Exit Control
      - Entry Control
  2. In Ubuntu terminal:<br>
      a. Make<br>
      ```
      make
      ```
      b. Unload module<br>
      ```
      sudo rmmod cmpe283-1
      ```
      c. Insert module<br>
      ```
      sudo insmod ./cmpe283-1.c
      ```
      d. Display messages<br>
      ```
      dmesg
      ```
      
## References
1. https://wiki.ubuntu.com/Kernel/BuildYourOwnKernel
2. https://www.intel.com/content/dam/www/public/us/en/documents/manuals/64-ia-32-architectures-software-developer-vol-3c-part-3-manual.pdf
