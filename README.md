# Home Lab for Cybersecurity

## Introduction

Welcome to my home lab setup! This project demonstrates my proficiency in creating and utilizing a secure environment for practicing various cybersecurity techniques. I use this lab to explore different tools, perform penetration testing, and continuously enhance my cybersecurity skills. The lab will include VirtualBox, Windows 10, Metasploitable, and Kali Linux.

## Requirements

### Hardware

- A computer with at least 8GB of RAM (16GB recommended)
- At least 100GB of free disk space

### Software

- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
- [Windows 10 ISO](https://www.microsoft.com/en-us/software-download/windows10ISO)
- [Kali Linux ISO](https://www.kali.org/downloads/)
- [Metasploitable](https://sourceforge.net/projects/metasploitable/files/Metasploitable2/)

## Setup Guide

### 1. Download and Install VirtualBox

#### Step 1: Download VirtualBox

- Go to the [VirtualBox download page](https://www.virtualbox.org/wiki/Downloads).
- Download the appropriate version for your operating system.

![VirtualBox Installation](images/virtualbox_download-1.png)

#### Step 2: Install VirtualBox

- Run the installer and follow the installation instructions.
- Accept all default settings unless you have specific requirements.

![VirtualBox Installation](images/virtualbox_download-2.png)

### 2. Download Windows 10 ISO

#### Step 1: Download Windows 10 ISO

- Go to the [Microsoft Windows 10 download page](https://www.microsoft.com/en-us/software-download/windows10ISO).
- Select the version and click on "Confirm".
- Choose the language and click on "Confirm".
- Select either the 32-bit or 64-bit download.

![Windows 10 ISO Download](images/windows10_download-1.png)

![Windows 10 ISO Download](images/windows10_download-2.png)

![Windows 10 ISO Download](images/windows10_download-3.png)

![Windows 10 ISO Download](images/windows10_download-4.png)

![Windows 10 ISO Download](images/windows10_download-5.png)

![Windows 10 ISO Download](images/windows10_download-6.png)

### 3. Set Up Virtual Machine for Windows 10

#### Step 1: Create a New Virtual Machine

- Open VirtualBox and click on "New".
- Enter the name, type (Microsoft Windows), and version (Windows 10).

![Create VM](images/create_vm-1.png)

![Create VM](images/create_vm-2.png)

![Create VM](images/create_vm-3.png)

![Create VM](images/create_vm-4.png)

![Create VM](images/create_vm-5.png)

#### Step 2: Configure the Virtual Machine

- Allocate memory (at least 2GB recommended).
- Create a virtual hard disk (VDI, dynamically allocated, 50GB).

![Configure VM](images/configure_vm-1.png)

![Configure VM](images/configure_vm-2.png)

![Configure VM](images/configure_vm-3.png)

![Configure VM](images/configure_vm-4.png)

![Configure VM](images/configure_vm-5.png)

![Configure VM](images/configure_vm-6.png)

#### Step 3: Install Windows 10

- Select the newly created VM and click "Start".
- Browse to the Windows 10 ISO file and start the installation.
- Follow the on-screen instructions to complete the installation.

![Install Windows 10](images/configure_vm-4.png)

### 4. Download and Set Up Kali Linux

#### Step 1: Download Kali Linux ISO

- Go to the [Kali Linux download page](https://www.kali.org/downloads/).
- Download the ISO file.

![Kali Linux Download](images/kali_download-1.png)

![Kali Linux Download](images/kali_download-2.png)

![Kali Linux Download](images/kali_download-3.png)

#### Step 2: Create a New Virtual Machine

- Open VirtualBox and click on "New". Follow the same steps we followed in the Windows 10 installation
- Enter the name, type (Linux), and version (Debian 64-bit).

![Create VM](images/create_vm-1.png)

#### Step 3: Configure the Virtual Machine

- Allocate memory (at least 2GB recommended).
- Create a virtual hard disk (VDI, dynamically allocated, 20GB).

#### Step 4: Install Kali Linux

- Select the newly created VM and click "Start".
- Browse to the Kali Linux ISO file and start the installation.
- Follow the on-screen instructions to complete the installation.

![Install Kali Linux](images/Install_KaliLinux-1.png)

### 5. Download and Set Up Metasploitable

#### Step 1: Download Metasploitable

- Go to the [SourceForge Metasploitable download page](https://sourceforge.net/projects/metasploitable/files/Metasploitable2/).
- Download the Metasploitable ZIP file.

![Metasploitable Download](images/metasploitable_download-1.png)

![Metasploitable Download](images/metasploitable_download-2.png)

#### Step 2: Create a New Virtual Machine

- Open VirtualBox and click on "New".
- Enter the name, type (Linux), and version (Other Linux 32-bit). Follow the same steps we followed in the Windows 10 installation

#### Step 3: Configure the Virtual Machine

- Allocate memory (at least 512MB recommended).
- Use an existing virtual hard disk and select the Metasploitable VMDK file.

#### Step 4: Start Metasploitable

- Select the newly created VM and click "Start".

![Start Metasploitable](images/Insatall_Metasploitable_VM-1.png)

#### Step 5: Network Adapter Options in VirtualBox

VirtualBox provides several network adapter options that you can use to configure networking for your virtual machines (VMs). Each option serves different purposes and is suitable for various scenarios. Below is a summary of the network adapter options along with their use cases, pros, and cons:

#### How to crete NAT Network and check Host-Only Network Adapter

![NAT Example](images/Network_adaptor_option-1.png)

![NAT Example](images/Network_adaptor_option-2.png)

![NAT Example](images/Network_adaptor_option-3.png)

![NAT Example](images/Network_adaptor_option-4.png)

##### 1. NAT (Network Address Translation)

- **Use When**: You need your VM to access the internet but don't require direct access from the host or other VMs.
- **Pros**: Simple setup, provides internet access.
- **Cons**: VM not directly accessible from the host or other VMs.

##### 2. NAT Network

- **Use When**: Multiple VMs need internet access and communication with each other, but not with the host.
- **Pros**: Allows VMs to communicate internally and access the internet.
- **Cons**: VMs are not accessible from the host.

![NAT Example](images/Network_adaptor_VM-1.png)

![NAT Example](images/Network_adaptor_VM-2.png)

##### 3. Bridged Adapter

- **Use When**: You need the VM to appear as a separate device on your physical network, accessible from the host and other devices.
- **Pros**: VM is accessible from the host and other devices on the network, provides internet access.
- **Cons**: Setup may be more complex depending on network configuration.

##### 4. Internal Network

- **Use When**: VMs need to communicate with each other but should be isolated from the host and external networks.
- **Pros**: VMs can communicate internally, complete isolation.
- **Cons**: No internet access, not accessible from the host.

##### 5. Host-Only Adapter

- **Use When**: VMs need to communicate with the host and each other in an isolated network environment.
- **Pros**: VMs can communicate with the host and each other.
- **Cons**: No internet access, isolated from external networks.

##### 6. Generic Driver

- **Use When**: Advanced configurations requiring specific or custom networking setups.
- **Pros**: Highly customizable.
- **Cons**: Requires advanced knowledge to configure.

##### 7. Not Attached

- **Use When**: VM does not need network access, for isolated testing or specific security requirements.
- **Pros**: Complete isolation.
- **Cons**: No network communication at all.

##### Choosing the Right Adapter

- **Internet Access**: NAT or NAT Network.
- **VM to VM Communication**: NAT Network, Internal Network, or Host-Only Adapter.
- **Host and VM Communication**: Bridged Adapter or Host-Only Adapter.
- **Isolation**: Internal Network, Host-Only Adapter, or Not Attached.

##### 6. Testing the Lab Setup

- Ensure all VMs can communicate with each other.
- Test basic scenarios such as scanning with Nmap from Kali Linux to Metasploitable.

#### Example Test:

1. **Scan Metasploitable from Kali Linux:**
   - Open a terminal in Kali Linux.
   - Run `nmap -p- 192.168.10.5` to scan all ports of the Metasploitable VM.

![Nmap Scan](images/connection_test-1.png)

![Nmap Scan](images/connection_test-2.png)

![Nmap Scan](images/connection_test-3.jpg)

![Nmap Scan](images/connection_test-4.png)

![Nmap Scan](images/connection_test-5.png)

## Conclusion

Congratulations on setting up the home lab! This environment is perfect for practicing various cybersecurity techniques in a safe and controlled setting. Using this lab, I will explore different tools, perform penetration testing, and continuously improve my cybersecurity skills. This project not only enhances my learning but also showcases my ability to create and manage complex technical environments.

## Next Steps

- Explore different tools in Kali Linux.
- Perform various attacks on Metasploitable and analyze the results.
- Document your findings and experiments.
