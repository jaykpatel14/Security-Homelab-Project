This guide will walk you through the process of installing PfSense, an open-source firewall and router platform, on VMware Workstation 17. PfSense offers a wide range of features such as firewall, VPN, traffic shaping, and more, making it a versatile solution for securing your network.

Prerequisites

Before you begin, ensure you have the following:

VMware Workstation 17 installed on your computer.
PfSense ISO: Downloaded from the PfSense website.

Installation Steps
Follow these steps to install PfSense on VMware Workstation 17:

Create a New Virtual Machine:

Open VMware Workstation and click on "File" > "New Virtual Machine."
Select "Typical" and click "Next."
Choose "Installer disc image file (iso)" and browse to the location of the downloaded PfSense ISO.
Click "Next" and specify the guest operating system as "FreeBSD" and version as "FreeBSD 64-bit."
Enter a name for the virtual machine and specify the location to save it.
Set the disk size according to your requirements and choose "Store virtual disk as a single file."
Click "Finish" to create the virtual machine.


Customize Virtual Machine Settings:

Before powering on the virtual machine, customize its settings.
Go to "Edit virtual machine settings."
Under the "Hardware" tab, ensure that the virtual machine has at least three network adapters (NICs) configured. Assign one adapter to "Nat" mode for WAN connectivity and second one to VMnet 1 and third one to VMnet 2

Optionally, adjust other settings such as CPU, memory, and display according to your preferences.

Install PfSense:

Power on the virtual machine.
PfSense will boot from the ISO image. Follow the on-screen instructions to proceed with the installation.
When prompted, select "Standard Kernel" and proceed with the installation as guided.
Configure Network Interfaces:

During installation, PfSense will detect the network interfaces. Assign the interfaces accordingly for WAN and LAN connectivity based on your network setup.
Configure IP addresses for the WAN and LAN interfaces as per your network configuration.
Complete Installation:

Once the installation is complete, the virtual machine will reboot.
PfSense will boot from the installed disk.
Access PfSense Web Interface:

Open a web browser on your host machine and enter the IP address assigned to the LAN interface of the PfSense virtual machine.
Log in with the default credentials (username: admin, password: pfsense).
Follow Initial Setup Wizard:

The PfSense initial setup wizard will guide you through configuring basic settings such as the WAN and LAN interfaces, DNS, and admin password.
Follow the wizard to complete the initial configuration of PfSense.
Explore PfSense Dashboard:

Once the initial setup is complete, you'll be redirected to the PfSense dashboard.
From here, you can explore the various features and settings of PfSense and begin configuring firewall rules, VPNs, and more.
Congratulations! You have successfully installed PfSense on VMware Workstation 17 and can now start configuring it to secure your network. Refer to the PfSense documentation for detailed information on advanced configurations and features.





