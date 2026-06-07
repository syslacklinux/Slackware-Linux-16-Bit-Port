<img width="1920" height="1280" alt="Slackware 16 Bit Logo" src="https://github.com/user-attachments/assets/92b26044-1698-445c-baac-fd47a1023d0f" />

# Slackware-Linux-16-Bit-Port
This is a port of Slackware to 16 Bit
Based On ELKS

Installation

Build ELKS images
On a modern Linux machine
git clone https://github.com/jbruchon/elks.git
cd elks
make

Write floppy image

    Insert a real floppy disk.

    Use dd to write the image:

    sudo dd if=elks.img of=/dev/fd0 bs=512

Boot hardware from floppy

    Insert the floppy into your vintage PC.

    Power on; ELKS should boot into its shell.

    Login as root (no password).

Install to HDD

    Partition the HDD using DOS tools or ELKS utilities.

    Format with FAT or MINIX (mkfs.minix).

    Copy ELKS system files from floppy to HDD.

    Adjust boot sector or use a bootloader (ELKS includes simple boot code).

    Reboot with HDD as primary boot device.


Login as root then vi /etc/issue Then Change ELKS 0.7.0 To Slackware 15.0 8086 then esc then :wq

Preview

<img width="735" height="464" alt="Screenshot From 2026-06-02 11-55-39" src="https://github.com/user-attachments/assets/75432b00-0ef3-4ad6-8258-243a4f0fc343" />
