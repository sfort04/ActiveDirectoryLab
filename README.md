# ActiveDirectoryLab

This contains steps on how I set up a basic home lab running Active Directory.

# Download and install Oracle VirtualBox
https://www.virtualbox.org/wiki/Downloads'

# Download Windows 10 and Windows 2022 ISO files.

https://www.microsoft.com/en-us/software-download/windows10ISO

https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022

# Create a new virtual machine by clicking on "New" in VirtualBox, naming it "Domain Controller" and selecting the "Windows Server 2022" ISO file as the boot media.


# Configure the vm by giving it two network adapters: one for connecting to the internet and one for the private network.


# Install Server 2022 on the vm and assign an IP address for the internal network.
![image](https://github.com/user-attachments/assets/4a042dd4-1d78-444f-9d67-e2e6e83530df)


# Name the server and install Active Directory to create the domain.
![image](https://github.com/user-attachments/assets/895fb219-e7b5-4e0a-8f07-81801c264ff4)

# Configuring routing so that clients on the private network can access the internet through the domain controller.

# Set up DHCP on the domain controller.

# Run Powershell script to create 1000 users in Active Directory.

# Create a new vm named "Client" and install Windows 10.

# Connect the client machine to the private network and join it to the domain.

# Log into the client machine with a domain account.
