# Building a Kali Linux Home Lab in VMware

## 1.Objective
The goal of this project was to safely deploy a Klai Linux virtual machine inside VMware Workstation

## 2. Tools & Technologies Used
**Hypervisor: VMware Workstation Pro
** Operating System: Kali Linux (64-bit installer ISO)
**Host System: Windows 11 / macos

## 3. Step-by-step Implementation

### Step 1: Resource Allocation
* Created a new Virtual Machine in VMware.
*  Allocated **2 CPU Cores**, **8GB RAM** and **30GB of Virtual Disk Space** to ensure smooth performance.
*  Configured the Network Adapter to **NAT** for safe, isolated internet access.

<img width="1918" height="1006" alt="image" src="https://github.com/user-attachments/assets/dd236e98-bfbe-4728-87b2-7b183a20a15b" />


  ## Step 2: OS Installation & Configuration
  * Booted the VM using the Kali ISO.
  * Selected the **Graphical Install** option.
  * Configured the default system language, keyboard layout and hostname (" Kali-lab").

    ## Step 3: Post-Install Hardening & Updates
    Once the Kali Linux fully loaded, I opended the terminal and run the following commands to ensure the system was           secure and up to date:
    \'\'\'bash
    sudo apt update && sudo apt upgrade -y
    \'\'\'
    * Verified that VMware Tools were running correctly for clipboard sharing and screen scaling.

      <img width="1918" height="915" alt="image" src="https://github.com/user-attachments/assets/1073dda3-5f40-40c6-983e-05b7fb5412e0" />

   
      ## Step 4: Key Takeaways & Challenges
      **Resource Management:** Learnt how to balance RAM allocation between my host machine and the VM so neither system         crashes.
      **Network Isolation:** Understood the difference between NAT, Bridged and Host networking modes, choosing NAT to           keep my lab environment separate from my home network. Bridge to connect directly to my physical home router and           Host only to create a private neteork that exists between my physical host computer and the VM.
    


    
  
