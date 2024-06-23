# Home Lab for Cybersecurity

## Introduction
This project provides a detailed guide to set up a home lab for cybersecurity practice. The lab will include VirtualBox, Windows 10, Metasploitable, and Kali Linux. By following these steps, you'll create a safe environment to test and enhance your cybersecurity skills.

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

![VirtualBox Installation](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/virtualbox_download-1.png)

#### Step 2: Install VirtualBox
- Run the installer and follow the installation instructions.
- Accept all default settings unless you have specific requirements.

![VirtualBox Installation](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/virtualbox_download-2.png)

### 2. Download Windows 10 ISO
#### Step 1: Download Windows 10 ISO
- Go to the [Microsoft Windows 10 download page](https://www.microsoft.com/en-us/software-download/windows10ISO).
- Select the version and click on "Confirm".
- Choose the language and click on "Confirm".
- Select either the 32-bit or 64-bit download.

![Windows 10 ISO Download](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/windows10_download-1.png)

![Windows 10 ISO Download](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/windows10_download-2.png)

![Windows 10 ISO Download](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/windows10_download-3.png)

![Windows 10 ISO Download](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/windows10_download-4.png)

![Windows 10 ISO Download](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/windows10_download-5.png)

![Windows 10 ISO Download](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/windows10_download-6.png)

### 3. Set Up Virtual Machine for Windows 10
#### Step 1: Create a New Virtual Machine
- Open VirtualBox and click on "New".
- Enter the name, type (Microsoft Windows), and version (Windows 10).

![Create VM](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/create_vm-1.png)

![Create VM](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/create_vm-2.png)

![Create VM](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/create_vm-3.png)

![Create VM](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/create_vm-4.png)

![Create VM](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/create_vm-5.png)

#### Step 2: Configure the Virtual Machine
- Allocate memory (at least 2GB recommended).
- Create a virtual hard disk (VDI, dynamically allocated, 50GB).

![Configure VM](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/configure_vm-1.png)

![Configure VM](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/configure_vm-2.png)

![Configure VM](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/configure_vm-3.png)

![Configure VM](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/configure_vm-4.png)

![Configure VM](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/configure_vm-5.png)

![Configure VM](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/configure_vm-6.png)



#### Step 3: Install Windows 10
- Select the newly created VM and click "Start".
- Browse to the Windows 10 ISO file and start the installation.
- Follow the on-screen instructions to complete the installation.

![Install Windows 10](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/configure_vm-4.png)

### 4. Download and Set Up Kali Linux
#### Step 1: Download Kali Linux ISO
- Go to the [Kali Linux download page](https://www.kali.org/downloads/).
- Download the ISO file.

![Kali Linux Download](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/kali_download-1.png)

![Kali Linux Download](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/kali_download-2.png)

![Kali Linux Download](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/kali_download-3.png)

#### Step 2: Create a New Virtual Machine
- Open VirtualBox and click on "New". Follow the same steps we followed in the Windows 10 installation
- Enter the name, type (Linux), and version (Debian 64-bit).

![Create VM](https://github.com/AkshayPatel03/Project_screenshots/blob/004658c2938996397df90e3f1db6e881c5c801d5/home-lab-for-cybersecurity/create_vm-1.png)


#### Step 3: Configure the Virtual Machine
- Allocate memory (at least 2GB recommended).
- Create a virtual hard disk (VDI, dynamically allocated, 20GB).

#### Step 4: Install Kali Linux
- Select the newly created VM and click "Start".
- Browse to the Kali Linux ISO file and start the installation.
- Follow the on-screen instructions to complete the installation.

![Install Kali Linux](https://github.com/AkshayPatel03/Project_screenshots/blob/c7c0575a44b62ea79eeca4b01c4a2be9799a4e7e/home-lab-for-cybersecurity/Install_KaliLinux-1.png)

### 5. Download and Set Up Metasploitable
#### Step 1: Download Metasploitable
- Go to the [SourceForge Metasploitable download page](https://sourceforge.net/projects/metasploitable/files/Metasploitable2/).
- Download the Metasploitable ZIP file.

![Metasploitable Download](https://github.com/AkshayPatel03/Project_screenshots/blob/c7c0575a44b62ea79eeca4b01c4a2be9799a4e7e/home-lab-for-cybersecurity/metasploitable_download-1.png)

![Metasploitable Download](https://github.com/AkshayPatel03/Project_screenshots/blob/c7c0575a44b62ea79eeca4b01c4a2be9799a4e7e/home-lab-for-cybersecurity/metasploitable_download-2.png)

#### Step 2: Create a New Virtual Machine
- Open VirtualBox and click on "New". 
- Enter the name, type (Linux), and version (Other Linux 32-bit). Follow the same steps we followed in the Windows 10 installation

#### Step 3: Configure the Virtual Machine
- Allocate memory (at least 512MB recommended).
- Use an existing virtual hard disk and select the Metasploitable VMDK file.

#### Step 4: Start Metasploitable
- Select the newly created VM and click "Start".

![Start Metasploitable](https://github.com/AkshayPatel03/Project_screenshots/blob/c7c0575a44b62ea79eeca4b01c4a2be9799a4e7e/home-lab-for-cybersecurity/Insatall_Metasploitable_VM-1.png)




### 6. Testing the Lab Setup
- Ensure all VMs can communicate with each other.
- Test basic scenarios such as scanning with Nmap from Kali Linux to Metasploitable.

#### Example Test:
1. **Scan Metasploitable from Kali Linux:**
   - Open a terminal in Kali Linux.
   - Run `nmap -p- [Metasploitable_IP]` to scan all ports of the Metasploitable VM.

![Nmap Scan](images/nmap_scan.png)

## Conclusion
Congratulations on setting up your home lab! You now have a safe environment to practice various cybersecurity techniques. Use this lab to explore different tools, perform penetration testing, and improve your cybersecurity skills.

## Next Steps
- Explore different tools in Kali Linux.
- Perform various attacks on Metasploitable and analyze the results.
- Document your findings and experiments.

