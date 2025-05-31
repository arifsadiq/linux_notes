### Define the boot process of Linux

Booting process: First BIOS loads the boot loaders, then boot loaders loads the kernel, then kernel mount the file systems and drivers installation will takes place and in it will be loaded.

Boot process takes place in 4 scenes with 4 main characters.

#### Scene 1
When the computer is switched on, it automatically invokes BIOS ( a ROM chip embedded in the motherboard). 
The BIOS will start the processor and perform a POST [Power On Self Test] to check whether the connected device are ready to use and working properly.
Once the POST is completes BIOS will jump to a specified location in RAM and check for the booting device.
The boot sector is always the first sector of the hard disk and BIOS will load the MBR into the memory.

#### Scene 2
Here the bootloader takes the control of the booting process. GRUB is the main bootloader commonly available.
It will help the user to select various boot options. Depending on the selected boot option, the kernel is loaded.

#### Scene 3
After kernel is loaded the kernel will take control of the booting process and it will initialize all the hardwares including I/O processors 
etc. Kernel then creates a root device and mounts the partitions.

#### Scene 4
INIT is loaded.

