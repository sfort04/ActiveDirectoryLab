# ActiveDirectoryLab

This contains steps on how I set up a basic home lab running Active Directory.

# Download and install Oracle VirtualBox
[VirtualBox](https://www.virtualbox.org/wiki/Downloads)

# Download Windows 10 and Windows 2022 ISO files.
[Windows 10 ISO](https://www.microsoft.com/en-us/software-download/windows10ISO)

[Windows Server 2022](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022)

# Create a new virtual machine by clicking on "New" in VirtualBox, naming it "Domain Controller" and selecting the "Windows Server 2022" ISO file as the boot media.


# Configure the vm by giving it two network adapters: one for connecting to the internet and one for the private network.
![image](https://github.com/user-attachments/assets/04ca05f6-f6d8-4f7d-a7f6-02f603b3b061)


# Install Server 2022 on the vm and assign an IP address for the internal network.
![image](https://github.com/user-attachments/assets/4a042dd4-1d78-444f-9d67-e2e6e83530df)


# Name the server and install Active Directory to create the domain.
![image](https://github.com/user-attachments/assets/895fb219-e7b5-4e0a-8f07-81801c264ff4)
![image](https://github.com/user-attachments/assets/4dd40a50-0c1d-4870-a0a3-c6966efe97bd)


# Configuring routing so that clients on the private network can access the internet through the domain controller.
![image](https://github.com/user-attachments/assets/468f581b-5775-4a1b-9ba3-523faaa0310b)

![image](https://github.com/user-attachments/assets/d1b53f0d-a63d-4e8a-8558-e0023d1ae34e)

# Set up DHCP on the domain controller.
![image](https://github.com/user-attachments/assets/c8222b70-1d43-4a2e-bd7c-35ea3e3be1bb)

![image](https://github.com/user-attachments/assets/73c17982-41ab-46c7-a401-9c875b27e5a0)


# Run Powershell script to create 1000 users in Active Directory.
[Powershell Script](https://github.com/joshmadakor1/AD_PS)

![image](https://github.com/user-attachments/assets/cfb4b417-0dd9-40a2-8d6a-928c6313c4a8)
![image](https://github.com/user-attachments/assets/73cb9253-7b06-4ccc-87bc-3676904afc52)



# Create a new vm named "Client" and install Windows 10.

# Connect the client machine to the private network and join it to the domain.
![image](https://github.com/user-attachments/assets/bae1ef91-f588-4b6f-9d76-9d75b96eb48b)
![image](https://github.com/user-attachments/assets/d9925b2c-ad15-4e77-9cfb-f8ff31ada9dd)


# Verify connection to Internet and Domain Controller by using ping.
![image](https://github.com/user-attachments/assets/b6bb01ec-124f-4ff7-a631-a46b5d586c81)
![image](https://github.com/user-attachments/assets/8511367e-2b7b-40a3-93c7-ca113f20bfde)


# Log into the client machine with a domain account.
![image](https://github.com/user-attachments/assets/462ee3a8-9482-4215-84e3-3bbb92a592a9)

