# installing-Kali-on-Mac-OS-M1


### Steps:

1. **Install UTM:**
   - Download and install UTM from the official website: [UTM Download](https://mac.getutm.app/)
   - **Important Step:** Grant full-disk access to UTM in your Mac OS system settings under Security & Privacy.

2. **Download Kali Linux ISO for ARM64:**
   - Download the Kali Linux ISO for ARM64 architecture from the official Kali Linux website.

3. **Setup Virtual Machine in UTM:**
   - Open UTM and create a new virtual machine.
   - Choose "Linux" as the operating system.
   - Browse and select the downloaded Kali Linux ISO.
   - Allocate RAM, enable hardware OpenGL virtualization, and set storage to at least 64GB.
   - **Important Step:** Add a new serial device in the virtual machine settings.
   - Save the virtual machine.

4. **Installation Process:**
   - Start the virtual machine and open the graphical installer.
   - Select language, keyboard, and timezone preferences.
   - Proceed with the installation, setting hostname, domain name, and user credentials.
   - Choose the partition method "Guided - use entire disk" and complete the installation.

5. **Post-Installation Setup:**
   - Once installation is complete, close the installation windows.
   - Remove the serial device and eject the ISO file from the virtual CD/DVD drive in UTM settings.
   - Restart the virtual machine and access Kali GNU/Linux.

6. **First Steps on Kali Linux:**
   - Run the following commands in the terminal:
     ```
     sudo apt-get update
     sudo apt-get upgrade
     sudo apt-get autoremove
     sudo apt-get clean
     ```
