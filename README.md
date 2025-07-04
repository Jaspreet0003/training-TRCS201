# training-TRCS201
in this repository i will share what i have done on daily basis
the day started with introduction of linux 
it is a open and free source (not paid)
learned difference of linux over windows

downloaded mainly three softwares-

*1.virtual box*

*2.visual c++*

*3.ubuntu 24.04.02*
# DAY 2: 
We began the second day by quickly going over all the topics discussed on Day 1. This helped reinforce the concepts and set the tone for the new topics.

After the recap, we moved on to an important part of the operating system: the Kernel. The Kernel is the main part of an operating system, responsible for managing all critical resources such as memory, processor time, and input/output devices. It acts as the central unit that connects the system software to the hardware.

Following that, we explored the concept of the Shell. The Shell acts as a middle layer between the user and the Kernel. It receives commands from the user, interprets them, and then passes them to the Kernel to perform the requested operations.

Our teacher explained these concepts in a very clear and engaging manner, using a simple diagram to illustrate the flow of interaction:
![Image](https://github.com/user-attachments/assets/95f51467-59c3-4265-9ccd-06041f96bc22)

# FILE SYSTEM STRUCTURES -



# BELOW ARE FEW COMMANDS THAT WE PRACTISED-- 


![Image](https://github.com/user-attachments/assets/e0ed84d9-0a9f-42bf-9dd3-09ec73426040)

![Image](https://github.com/user-attachments/assets/6e33c465-9502-4594-ad4c-c2cc42aeb4a2)

![Image](https://github.com/user-attachments/assets/e76545b7-bdd8-4504-a2ee-73295dd320ab)

![Image](https://github.com/user-attachments/assets/a134e9e1-2f03-4fa3-b560-ba3ce3c0db57)

# DAY3

We began by revisiting the concepts covered on the previous days to refresh our understanding. After the revision, we moved on to several new topics:

⸻

💻 Dual Boot Setup

Dual booting allows a system to have two operating systems installed simultaneously. During startup, the user can choose which OS to boot into. This is particularly useful for switching between different environments (e.g., Windows and Linux).

⸻

📀 Understanding ISO Files

An ISO file in Linux represents an exact copy of the data from an optical disk (like a CD or DVD) packaged in a single file using the ISO 9660 standard. It is commonly used for OS installation and software distribution.

⸻

🔧 Bare Metal Installation

This refers to installing an operating system directly onto a physical machine’s hardware, without the use of any virtualization technology. It’s often used for setting up servers or fresh systems from scratch.

⸻

🖥 Virtualization: VMware vs VirtualBox
	•	VMware: A professional-grade virtualization solution, widely used in enterprises. Known for high performance, stability, and advanced features.
	•	VirtualBox: A free and open-source tool ideal for personal use, development, and testing. While it lacks some enterprise features, it’s easy to use and supports various operating systems.

⸻

💾 Disk Partitioning Schemes

Partitioning splits a hard drive into separate sections, each behaving like an independent disk. This helps in organizing data and running multiple OSes.

Main Types of Partitioning:
	•	MBR (Master Boot Record)
	•	Supports up to 4 primary partitions
	•	Maximum disk size: 2 TB
	•	Works with BIOS systems
	•	Considered outdated and less flexible
	•	GPT (GUID Partition Table)
	•	Supports over 128 partitions
	•	Can handle disks larger than 2 TB
	•	Designed for UEFI systems
	•	Offers better scalability and redundancy

⸻

🔐 Permissions and Shell Scripting

🔸 File & Directory Permissions
	•	chmod (change mode): Used to set or modify permissions for files and folders.

Examples:
	•	chmod +x script.sh → Grants execute permission to the script
	•	chmod 444 file.txt → Sets file to read-only for all users


# BELOW ARE 3 PROGRAMS THAT WE PRACTISED BASED ON SHELL PROGRAMMING-

![Image](https://github.com/user-attachments/assets/b45d7982-b46b-4e21-bdbb-f51dd5620097)

![Image](https://github.com/user-attachments/assets/e3827eac-a844-4985-aa18-96a7b09dd720)

![Image](https://github.com/user-attachments/assets/2c33a5e9-7bc4-4250-a5e4-cf5ce1955bd4)

![Image](https://github.com/user-attachments/assets/fd625118-0f31-452e-bfdd-65036ef9c2d0)

![Image](https://github.com/user-attachments/assets/e1bb167f-32bd-4c4b-a3ee-c53ddb755b10)

![Image](https://github.com/user-attachments/assets/21671c31-3e0b-4230-8f2e-fdecbaf7b36a)

## DAY 4

📦 File Compression Using Commands
File compression is the technique of reducing the size of one or more files by encoding the data more efficiently. It helps save storage space, makes file transfers faster, and simplifies file management.

![Screenshot 2025-06-30 112658](https://github.com/user-attachments/assets/14e13dad-7387-4809-b221-a906b52e8333)


📌 Purpose:
📂 Save Storage Space: Reduce the disk space used by files.



🚀 Faster Data Transfer: Smaller files take less time to upload and download.



📑 Simplified File Management: Makes handling multiple files easier by compressing them into single archives.



📦 What is GZIP (GNU Zip)?


Gzip is a popular command-line tool in Linux that compresses files to save space without losing any data. It creates compressed files with a .gz extension.


🔧 Syntax:
bash


Copy


Edit


gzip filename.txt


👉 Compresses filename.txt to filename.txt.gz and removes the original file.

🔧 To Decompress a File:


bash


Copy


Edit


gunzip filename.txt.gz


👉 Restores the original file and deletes the compressed version.



🔧 Compress Without Deleting the Original:


Use the -k option:

bash


Copy


Edit


gzip -k file.txt
👉 This creates a compressed file while keeping the original.



🐧 Wildcards in Linux


Wildcards are special characters used in Linux commands to represent one or more characters in file or directory names. They allow working with multiple files at once without listing them individually.

![Screenshot 2025-06-30 113327](https://github.com/user-attachments/assets/b5a826db-5546-4789-8eb7-098a18e25f28)


📌 Example:


bash
Copy
Edit
ls *.txt
👉 Lists all files ending with .txt.

✅ Common Wildcard Commands:


bash


Copy


Edit


rm *.log           # Removes all .log files  
cp *.jpg images/   # Copies all .jpg files to images/ folder  
mv report?.txt old/ # Moves files like report1.txt, report2.txt to old/
📊 Wildcard Symbols:


Wildcard	Description	Example


*	Matches zero or more characters	*.txt

*	
?	Matches exactly one character	file?.txt


[ ]	Matches one character from the set	file[1-3].txt


[! ]	Matches one character not in the set	file[!0-9].txt


{a,b,c}	Matches any listed string	file{1,2}.txt


{1..5}	Matches a range of values	file{1..5}.txt



📝 Escaping Characters in Linux


In Linux, certain characters like *, $, ", ', &, etc., have special meanings in the shell. Escaping characters prevents the shell from interpreting them and treats them as plain text

![Screenshot 2025-06-30 113738](https://github.com/user-attachments/assets/686ce126-a92e-446c-837d-3efd219bfe8a)


📌 Why Use Escaping?


To handle characters such as:

ruby
Copy
Edit
*, ?, |, &, <, >, $, ", ', \, etc.


and ensure they appear or work as normal characters.



🔧 Common Escaping Methods:


Method	Effect	Example
\	Escapes the next character	echo \$HOME → $HOME
'...'	Treats everything inside as literal text	'*.txt' → *.txt
"..."	Allows variables to expand, protects others	"Hello $USER" → expands
\ (newline)	Continues command to next line	echo "Hello \ (newline)`

📖 Examples:


bash
Copy
Edit
touch MyFile.txt


ls MyFile.txt



echo \$HOME        # Prints $HOME


📝 Quoting in Linux


Quoting controls how the shell processes special characters and variables.

![Screenshot 2025-06-30 114826](https://github.com/user-attachments/assets/e6af38ce-3dea-4193-be5b-1ef33521bdd6)


📌 Types of Quotes:


Type	Purpose	Example	Output


Single Quotes '	Preserves everything literally inside	echo '$HOME'	$HOME


Double Quotes "	Expands variables but preserves spaces, etc.	echo "My home is $HOME"	My home is /home/user


Backslash \	Escapes a single character	echo \$HOME	$HOME



💻 Hardware: Basics of Computer Components


Hardware refers to the physical, tangible components of a computer system — the parts you can touch, unlike software which is a set of programs and data.



📌 What is Computer Hardware?


It includes everything from the CPU to the monitor, keyboard, mouse, storage devices, and other peripherals.


## 🖥️ Basic Computer Hardware Components

| Component              | Description                                      |
|:----------------------|:-------------------------------------------------|
| **CPU (Processor)**     | The brain of the computer, processes instructions |
| **Motherboard**         | Connects and manages all hardware components      |
| **RAM (Memory)**        | Temporary storage for quick data access           |
| **Hard Drive / SSD**    | Long-term storage for files and programs          |
| **Power Supply Unit**   | Converts electricity to power the computer        |
| **Input Devices**       | Devices like keyboard, mouse, scanner             |
| **Output Devices**      | Devices like monitor, printer                     |
| **Graphics Card (GPU)** | Manages graphics and image rendering              |

Motherboard-

![mother board](https://github.com/user-attachments/assets/e2113f78-5d2c-4b32-8b63-aa1ec2168c5f)

## 📖 What is a Motherboard?

A **motherboard** is the primary printed circuit board (PCB) inside a computer. It acts as the **central hub** that connects all the components of a computer together — including the CPU, RAM, storage, and peripheral devices.

---

## 📦 Functions of a Motherboard

✅ Provides electrical connections for all components  
✅ Hosts essential system components like CPU and RAM  
✅ Facilitates data communication between hardware devices  
✅ Provides slots and ports for peripherals and storage devices  
✅ Manages power distribution to components  

---

## 📌 Basic Components of a Motherboard

| Component         | Description                                                   |
|:------------------|:--------------------------------------------------------------|
| **CPU Socket**       | Slot where the processor is installed                         |
| **RAM Slots (DIMM)** | Slots for memory modules (RAM)                                |
| **Chipset**          | Controls data flow between CPU, memory, and peripherals        |
| **BIOS/UEFI Chip**   | Contains firmware to start and configure hardware              |
| **Expansion Slots**  | (PCI, PCIe) for adding graphics cards, sound cards, etc.       |
| **SATA Ports**       | Connect hard drives, SSDs, and optical drives                  |
| **Power Connectors** | Supply power to the motherboard and components                 |
| **USB/Audio Ports**  | Connect external devices like keyboard, mouse, speakers, etc.  |

---

## 🖥️ Types of Motherboards (Form Factors)

| Type       | Size and Use                                                         |
|:------------|:---------------------------------------------------------------------|
| **ATX**       | Standard size for desktops; most common and expandable               |
| **Micro-ATX** | Smaller than ATX; fewer expansion slots                              |
| **Mini-ITX**  | Compact size for small PCs and home theater systems                   |




## DAY 5 

🛠️ Common PC Issues and Troubleshooting Solutions

Today, we discussed frequent problems users face with personal computers and how to resolve them. Below is a categorized summary, with each issue followed by its likely cause and recommended solution.

⸻

🔧 System Performance & Maintenance Issues

• C Drive Full / PC Slowing Down

The C: drive holds system-critical files and OS data. Avoid saving personal data here. To fix:
	•	Use Disk Cleanup
	•	Delete unnecessary files (like %temp%, temp, and prefetch)
	•	Move files to D: or E: drives
	•	Uninstall programs you don’t use

• Computer Running Slowly

Often caused by too many startup apps or limited RAM.
	•	Open Task Manager → disable unused startup apps
	•	Delete junk and temp files
	•	Remove unneeded software

• Fragmented Hard Disk (HDD Only)

Fragmentation affects performance on HDDs (not SSDs).
	•	Run “Defragment and Optimize Drives” via Windows search

• Excess Temporary/Junk Files

Generated during app usage; they slow down the system over time.
	•	Use Disk Cleanup
	•	Manually delete %temp%, temp, and prefetch files

• Slow Startup Time

Usually from too many startup programs or services.
	•	Use Task Manager > Startup tab to disable non-essential apps

⸻

💻 Software-Related Issues

• App Freezing or Crashing

This may happen due to:
	•	Corrupted installations
	•	Low memory
Fix: Force close via Task Manager, then update or reinstall the application.

• Installation Errors

Causes may include:
	•	Lack of admin rights
	•	Wrong version (32-bit vs 64-bit)
Fix: Right-click and choose “Run as Administrator”, ensure correct version is used.

• Windows Update Fails

This happens if update cache gets corrupted.
Fix:
	•	Run Windows Update Troubleshooter
	•	Clear contents from C:\Windows\SoftwareDistribution

⸻

🖨️ Hardware & Peripheral Issues

• Printer Not Working

Check for:
	•	Driver issues
	•	Connection errors
Fix: Restart both printer and PC, check cables, and reinstall drivers if necessary.

• External Drive Not Showing

New or unformatted drives may not appear.
Fix:
	•	Go to Disk Management
	•	Assign a drive letter
	•	Format the drive (if required)

• Random Restarts / Overheating

Often due to:
	•	Blocked fans or dust
	•	Old thermal paste
Fix: Clean air vents and CPU fan, apply new thermal paste if needed, use cooling pads.

⸻

🌐 Network & Security Problems

• Internet Connected but Not Working

Usually caused by:
	•	DNS errors
	•	Outdated network drivers
Fix:
	•	Restart router
	•	Use Windows Network Troubleshooter
	•	Run ipconfig /flushdns in Command Prompt

• Antivirus Slowing System Down

Too many antivirus programs cause system lag.
Fix: Stick to one reliable antivirus (like Windows Defender), and disable non-essential scans.

⸻

👤 Login & Display Issues

• Forgot Password

Local account: Reset using another admin account or boot in Safe Mode
Microsoft account: Use Microsoft’s password recovery tool online

• Poor Graphics Performance

Caused by:
	•	Old GPU drivers
	•	High resource usage
Fix:
	•	Update drivers (from NVIDIA/AMD website)
	•	Close background apps while gaming or designing

⸻

💥 Blue Screen of Death (BSOD)

What Is It?

![IMG_4271](https://github.com/user-attachments/assets/c919fe10-08ab-4404-8003-03b25da7d48a)


The BSOD (Blue Screen of Death) is a critical error screen that forces Windows to shut down to prevent damage. It’s often caused by low-level hardware or driver issues.

Common Causes
	•	Faulty device drivers
	•	Corrupt system files
	•	Incompatible or failing hardware (RAM, GPU, HDD)
	•	Overheating
	•	BIOS issues or overclocking
	•	Malware

⸻

🧠 How to Analyze BSOD
	1.	Check the Stop Code
Example: CRITICAL_PROCESS_DIED, IRQL_NOT_LESS_OR_EQUAL
	2.	Use Reliability Monitor
Find it in the Start menu to see system events before crash
	3.	View Minidump Files
Stored at C:\Windows\Minidump\. Analyze using:
	•	BlueScreenView (NirSoft)
	•	WinDbg
	•	WhoCrashed
	4.	Check Event Viewer
Run eventvwr.msc to view detailed logs leading to the crash


## 🧰 Steps to Fix a BSOD

| 🔢 Step | 🛠️ Action |
|--------|-----------|
| 1. | **Update Drivers** — Use Device Manager to update GPU, chipset, and network drivers. |
| 2. | **Uninstall Recent Software** — Remove apps or drivers installed before the BSOD started. |
| 3. | **System File Checker** — Run `sfc /scannow` in Command Prompt (admin mode). |
| 4. | **Check RAM** — Use Windows Memory Diagnostic tool. |
| 5. | **Scan for Malware** — Use Windows Defender or Malwarebytes. |
| 6. | **Reset Overclocking** — Revert BIOS settings to default. |
| 7. | **System Restore** — Roll back to a previous restore point. |
| 8. | **Update Windows** — Ensure Windows is up to date with patches and security updates. |

---

## 🛡️ Prevention Tips

- Don’t install untrusted software or drivers.
- Create a restore point before major system changes.
- Keep drivers and antivirus up to date.
- Regularly clean hardware (fans, vents) to avoid overheating.


## DAY 6

### 1. 🔐 Safe Mode
Safe Mode is a diagnostic startup mode that loads only essential system drivers and services. It helps isolate and fix issues caused by third-party apps or drivers.

#### ✅ How to Access Safe Mode (Windows):
- Press `Win + R`, type `msconfig`, go to **Boot** > Check **Safe boot**, then restart.
- Or, force reboot 3 times to trigger Windows Recovery, then go to:
  `Troubleshoot > Advanced Options > Startup Settings > Restart > Select 4 or 5`.

---

### 2. 🧰 Recovery Tools
Windows and other OS platforms offer built-in recovery tools for restoring or fixing your system.

#### 🛠️ Common Tools:
- **System Restore** – Roll back to a previous working state.
- **Startup Repair** – Fixes boot issues automatically.
- **Command Prompt** – Advanced troubleshooting via commands.
- **Reset This PC** – Reinstalls Windows (with or without keeping files).

---

### 3. 🛠️ OS Repair Methods
When system files are corrupt or missing, these tools can help:

- `sfc /scannow` – Scans and repairs system files.
- `chkdsk /f /r` – Checks and fixes hard drive errors.
- `DISM /Online /Cleanup-Image /RestoreHealth` – Repairs Windows image.

---

### 4. 🦠 Virus & Malware Symptoms
Common signs your PC might be infected:

- Slow performance
- Unexpected pop-ups or ads
- Programs opening/closing on their own
- Disabled antivirus/firewall
- High CPU or disk usage
- Unknown applications installed

---

### 5. 🧹 Basic Malware Removal Steps

#### Step-by-step:
1. **Boot into Safe Mode with Networking**
2. **Uninstall suspicious programs** from Control Panel or Settings
3. **Run antivirus scans** using tools like:
   - Windows Defender
   - Malwarebytes
   - HitmanPro
4. **Delete temp files** using `Disk Cleanup`
5. **Reset browser settings** (Chrome/Edge/Firefox)
6. **Update OS and antivirus definitions**



# 🔌 RJ45 Networking Essentials

This repository provides essential information about **RJ45 connectors**, including wiring standards, cable types, and usage in networking. RJ45 is the most common connector used for Ethernet networking.

---

## 📘 What is RJ45?

**RJ45 (Registered Jack 45)** is an 8-pin connector used primarily in Ethernet networking. It connects computers, routers, switches, and other network devices using twisted-pair cables.

---

## 🧷 Pinout Standards

There are two main wiring standards used in RJ45 connectors:

### 2. T568B Standard (Most Common):

Pin
Wire Color
Function
1
Orange/White
TX+
2
Orange
TX-
3
Green/White
RX+
4
Blue
—
5
Blue/White
—
6
Green
RX-
7
Brown/White
—
8
Brown
—


## 🛠️ How to Crimp an RJ45 Connector

1. Strip about 1 inch of outer insulation.
2. Untwist and arrange the wires based on the T568B or T568A standard.
3. Trim the wires evenly.
4. Insert the wires into the RJ45 plug.
5. Use the crimping tool to press the connector.
6. Test the cable for connectivity.


## 📷 Diagram

![IMG_5017](https://github.com/user-attachments/assets/44df9483-4573-4309-b067-d3d64359c7b8)


## DAY 7


Networking Fundamentals

🖥️ What is a Host?



A host is any device connected to a network that can send or receive data. This includes:
	•	Desktop and Laptop Computers
	•	Servers
	•	Smartphones
	•	Network Printers
	•	IP Cameras
	•	IoT Devices (e.g., smart TVs, smart bulbs)

⸻

🌐 What is a Network?

A network is a collection of two or more interconnected devices that share data and resources. These devices communicate via wired (Ethernet cables) or wireless (Wi-Fi) methods.

Key Functions of a Network:
	•	📁 File and Data Sharing
	•	🖨️ Shared Resource Access (e.g., printers, internet)
	•	🗣️ Communication (emails, voice/video calls)
	•	🛠️ Centralized or decentralized control over devices

⸻

🌍 Understanding IP Addressing

An IP address (Internet Protocol address) is a unique numerical label assigned to each device on a network. It ensures devices can be identified and communicate on a local or global scale.

🔢 Types of IP Addresses:
	1.	Public IP Address
	•	Assigned by your Internet Service Provider (ISP)
	•	Used for communication over the internet
	2.	Private IP Address
	•	Used within a private LAN (Local Area Network)
	•	Not routable on the internet
	•	Common in homes and offices

⸻

🔑 Key Properties of IP Addresses:

1. Uniqueness
	•	Each device on a network must have a distinct IP address.
	•	Duplicate IPs cause conflicts and disrupt communication.

Example: Two devices cannot share the same IP like 192.168.1.10.

2. Universality
	•	IP addressing standards (IPv4/IPv6) are globally recognized.
	•	Enables cross-border device communication and interoperability.

⸻

IPv4 (Internet Protocol Version 4)
	•	Address Size: 32 bits
	•	Format: 4 decimal-separated groups (octets)
	•	Range per octet: 0 to 255
	•	Example: 192.168.1.1

🧮 Address Space:
	•	Total combinations: 2³² = 4,294,967,296
	•	This space is limited and nearing exhaustion.

⸻

IPv6 (Internet Protocol Version 6)
	•	Address Size: 128 bits
	•	Format: 8 groups of 4 hexadecimal digits
	•	Separator: Colons (:)
	•	Example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

🧮 Address Space:
	•	Total combinations: 2¹²⁸ = 340 undecillion
	•	Sufficient for the expanding number of internet-enabled devices.


## 📊 IPv4 vs IPv6 Comparison Table

| Feature               | IPv4                              | IPv6                                  |
|------------------------|------------------------------------|----------------------------------------|
| **Address Length**     | 32 bits (4 blocks)                | 128 bits (8 blocks)                    |
| **Address Format**     | Decimal, separated by dots        | Hexadecimal, separated by colons       |
| **Example**            | 192.168.0.1                       | 2001:0db8:85a3:0000:0000:8a2e:0370:7334 |
| **Address Space**      | ~4.3 billion addresses            | ~340 undecillion addresses             |
| **Configuration**      | Manual or via DHCP                | Auto-configuration (SLAAC) or DHCPv6   |
| **Security**           | Optional (IPSec not mandatory)    | Built-in IPSec support                 |
| **Header Complexity**  | Simple and small                  | More complex and larger                |
| **Broadcast Support**  | Supports broadcast                | No broadcast; uses multicast instead   |
| **Fragmentation**      | Done by both sender and routers   | Handled only by the sender             |

IP Address Notations

1. Binary Format
	•	IPs are internally processed in binary (0s and 1s).
	•	32-bit binary IPs are divided into 4 groups (octets).

Example: 11000000.10101000.00000001.00000001
(Binary format of 192.168.1.1)

2. Dotted Decimal Notation
	•	Human-readable format for IPv4.
	•	Converts each 8-bit binary octet into a decimal number (0–255).

Example:
Binary: 11000000.10101000.00000001.00000001
Decimal: 192.168.1.1


## 🧩 Classful Addressing in IPv4

In classful addressing, IPv4 addresses are divided into five categories (Class A to Class E), based on the first few bits of the address. Each class has a specific IP range, default subnet mask, and intended use.

### 📚 IP Address Classes Overview

| Class | Starting Bits | IP Address Range       | Default Subnet Mask   | Number of Hosts       | Usage                            |
|-------|----------------|-------------------------|------------------------|------------------------|----------------------------------|
| A     | 0              | 1.0.0.0 – 126.255.255.255 | 255.0.0.0 ( /8 )       | ~16 million per network | Very large networks              |
| B     | 10             | 128.0.0.0 – 191.255.255.255 | 255.255.0.0 ( /16 )     | ~65,000 per network     | Medium-sized networks            |
| C     | 110            | 192.0.0.0 – 223.255.255.255 | 255.255.255.0 ( /24 )   | 254 per network         | Small networks (LANs)           |
| D     | 1110           | 224.0.0.0 – 239.255.255.255 | Not applicable          | Not for host use        | Multicasting                    |
| E     | 1111           | 240.0.0.0 – 255.255.255.255 | Not applicable          | Not for host use        | Experimental / Research         |



![IMG_4329](https://github.com/user-attachments/assets/7ba371eb-97d0-457a-a4c1-819d0cecdd90)


### 🔎 Notes:

- **Class A** is used by large organizations with a vast number of devices.
- **Class B** is allocated to medium-sized networks like universities.
- **Class C** is common in small businesses or home networks.
- **Class D** is reserved for multicast groups (used in streaming, conferencing).
- **Class E** is reserved for future or experimental purposes and not assigned to devices.

> ⚠️ Classful addressing is now mostly obsolete and replaced by CIDR (Classless Inter-Domain Routing), but it’s important for understanding IPv4 fundamentals.


## 📡 Unicast vs Broadcast vs Multicast

In computer networking, data can be transmitted in different modes depending on the number of recipients. Below is a comparison of **Unicast**, **Broadcast**, and **Multicast** communication methods.

### 🔁 Communication Types Comparison

| Mode       | Description                                                 | Destination Type           | Example Use Case                      |
|------------|-------------------------------------------------------------|----------------------------|----------------------------------------|
| **Unicast**   | Sends data from one sender to one specific receiver         | One-to-One                 | Web browsing, downloading a file       |
| **Broadcast** | Sends data from one sender to **all devices** on the network | One-to-All (same network)  | ARP request, DHCP discover             |
| **Multicast** | Sends data from one sender to **multiple selected receivers** | One-to-Many (group)        | Video streaming, IPTV, webinars        |

### 📌 Summary

- **Unicast**: Point-to-point communication; most common in daily internet use.
- **Broadcast**: Reaches all devices on the local network; limited to LANs.
- **Multicast**: Targets specific groups; reduces unnecessary network traffic.

> 🧠 Tip: Multicast requires receivers to "join" a multicast group using protocols like IGMP.


# 🧱 Networking Essentials: Subnetting, MAC, DNS, CIDR

This section explores important concepts in computer networking, including **Subnetting**, **Subnet Masks**, **MAC Addresses**, **DNS**, and **CIDR**. These are critical for understanding how networks are organized, addressed, and managed.

---

## 🔄 Subnetting

**Subnetting** is the process of dividing a larger network into smaller, manageable subnetworks (subnets). It improves performance, security, and IP address utilization.

### ⚙️ Why Use Subnetting?

- Efficient IP address management  
- Reduces broadcast traffic  
- Enhances network performance  
- Improves security and isolation

### 🧮 Example:

Given IP: `192.168.1.0/24`  
You can create 4 subnets using a /26 mask:  
- Subnet 1: `192.168.1.0/26`  
- Subnet 2: `192.168.1.64/26`  
- Subnet 3: `192.168.1.128/26`  
- Subnet 4: `192.168.1.192/26`  

---

## 🧠 Subnet Mask

A **Subnet Mask** is used to determine the network and host portions of an IP address.

### 📌 Common Subnet Masks:

| Subnet Mask        | CIDR Notation | Hosts per Subnet |
|--------------------|---------------|------------------|
| 255.0.0.0          | /8            | 16,777,214        |
| 255.255.0.0        | /16           | 65,534            |
| 255.255.255.0      | /24           | 254               |
| 255.255.255.192    | /26           | 62                |
| 255.255.255.248    | /29           | 6                 |

### ✨ How It Works:

For IP `192.168.1.10` with mask `255.255.255.0`:
- Network part: `192.168.1`
- Host part: `10`

---

## 🔐 MAC Address (Media Access Control)

A **MAC address** is a unique identifier assigned to a network interface card (NIC). It operates at the **Data Link Layer (Layer 2)** of the OSI model.

### 📋 Format:

- Consists of 6 pairs of hexadecimal numbers  
- Example: `00:1A:2B:3C:4D:5E`

### 🧬 Characteristics:

- Hardware-level address
- Fixed at the time of manufacture
- Used for local network communication

---

## 🌍 DNS (Domain Name System)

The **Domain Name System (DNS)** translates human-friendly domain names into IP addresses.

### 🕸️ How It Works:

When you type `www.example.com`, DNS translates it into an IP like `93.184.216.34`.

### 📑 DNS Components:

- **DNS Resolver**: Client-side tool that queries DNS servers  
- **Root Server**: Top-level DNS servers  
- **TLD Server**: Handles top-level domains like `.com`, `.org`  
- **Authoritative Server**: Contains actual IP info for domains

---

## 📏 CIDR (Classless Inter-Domain Routing)

**CIDR** replaces traditional class-based IP addressing. It allows more flexible allocation of IP addresses using **prefix notation**.

### 🧾 CIDR Notation:

Format: `IP_address/Prefix_length`  
Example: `192.168.0.0/24`  
This means the first 24 bits are for the network, and the remaining 8 are for host addresses.

### 📚 Benefits of CIDR:

- Efficient IP allocation  
- Reduces routing table size  
- Supports VLSM (Variable Length Subnet Masking)

---

## 🧮 CIDR to Subnet Mask Conversion Table

| CIDR | Subnet Mask         | Hosts per Subnet |
|------|---------------------|------------------|
| /8   | 255.0.0.0           | 16,777,214        |
| /16  | 255.255.0.0         | 65,534            |
| /24  | 255.255.255.0       | 254               |
| /26  | 255.255.255.192     | 62                |
| /30  | 255.255.255.252     | 2                 |

---

## 📌 Summary

| Concept       | Description                                      |
|---------------|--------------------------------------------------|
| Subnetting    | Divides a network into smaller logical subnets   |
| Subnet Mask   | Identifies network and host parts of an IP       |
| MAC Address   | Unique physical address for network interfaces   |
| DNS           | Translates domain names to IP addresses          |
| CIDR          | Classless method to represent IP ranges          |

---

## DAY 8

## 📥 DHCP (Dynamic Host Configuration Protocol)

**DHCP** is an application-layer network protocol used to **automatically assign IP addresses** and other configuration settings to devices (clients) on a network.

### 📌 Why DHCP is Important:
- Manual IP configuration is time-consuming and error-prone, especially on large networks.
- DHCP automates the process and ensures every device gets a valid and unique IP address.

### 🔄 DHCP Workflow (DORA Process):
| Step | Description |
|------|-------------|
| **Discover** | The client sends a broadcast request to locate a DHCP server. |
| **Offer** | The DHCP server responds with an available IP and configuration options. |
| **Request** | The client requests the offered configuration. |
| **Acknowledgement** | The server confirms and assigns the IP address to the client. |

### 🧩 Other DHCP Configurations:
- **Subnet Mask**
- **Default Gateway**
- **DNS Servers**
- **Lease Time** – how long the IP is valid

### 💡 Note:
DHCP uses **UDP ports 67 (server) and 68 (client)**.

---

## 🧪 Networking Commands

These are essential CLI tools used to test and configure networks.

### 🔹 `ping` Command

Used to test **connectivity between two devices** (your computer and a remote host).

#### ✅ Purpose:
- To check if a host is reachable
- Measure latency (round-trip time)
- Diagnose packet loss

#### 🔧 Syntax:
```bash
ping <hostname or IP>

🧾 Sample Output:

PING google.com (142.250.64.78): 56 data bytes
64 bytes from 142.250.64.78: icmp_seq=0 ttl=117 time=23.345 ms


## 🔹 traceroute / tracert Command

Used to track the path packets take to reach a remote server. Helpful in diagnosing where delays or failures occur.

✅ Purpose:
	•	View intermediate routers or hops
	•	Identify slow or dropped hops
	•	Discover routing issues


🔹 ifconfig Command

Used on Linux/Unix-based systems to view and configure network interfaces.

✅ Displays:
	•	IP address
	•	Subnet mask
	•	MAC address
	•	Status (UP or DOWN)


## 🔍 What Does “64 Bytes” Mean in ping?

When you run a ping command, you’ll often see lines like:

64 bytes from 8.8.8.8: icmp_seq=1 ttl=56 time=10.2 ms


## 📘 Explanation:
	•	64 bytes refers to the size of the ICMP reply packet sent back by the destination.
	•	This includes 56 data bytes + 8 bytes of ICMP header (varies by OS).
	•	In Linux, 64 bytes is the default size; in Windows, it might show 32 bytes.


♻️ Loopback Address

The loopback address is used to send network traffic to the same device (itself) for testing purposes.

🧾 Loopback IP:
	•	IPv4: 127.0.0.1
	•	IPv6: ::1

🔹 Uses:
	•	Software testing
	•	Checking if TCP/IP stack is working
	•	Hosting local servers (web dev, database)

💡 Note:

Packets sent to 127.0.0.1 never leave the device or enter the network.

⸻

🔌 Ethernet

Ethernet is a family of networking technologies used for wired local area networks (LANs).

🧷 Key Characteristics:
	•	Uses Cat5e/Cat6 cables
	•	Defined by the IEEE 802.3 standard
	•	Data is sent in frames
	•	Speeds range from 10 Mbps to 100 Gbps+

🔐 Advantages:
	•	Stable, consistent performance
	•	More secure (physical access required)
	•	Minimal interference or congestion

🔧 Components:
	•	NIC (Network Interface Card)
	•	Switches
	•	Routers
	•	Cables (Cat5e, Cat6, etc.)


## 🌐 Comparison: Ethernet vs Wi-Fi vs LAN vs WAN vs Internet

This section compares five key terms in networking, often confused or interchanged. Understanding the difference helps in designing, configuring, and troubleshooting networks efficiently.

| Term      | Type         | Description                                                                 | Scope/Range         | Examples / Use Cases                              |
|-----------|--------------|-----------------------------------------------------------------------------|---------------------|---------------------------------------------------|
| **Ethernet**  | Wired Technology | Physical medium using cables for data transmission (IEEE 802.3 standard)   | Local (Room/Building) | Office computers, gaming consoles, switches       |
| **Wi-Fi**     | Wireless Technology | Wireless local connectivity using radio signals (IEEE 802.11 standard)     | Local (~30–100 m)    | Smartphones, laptops, smart TVs                   |
| **LAN**       | Network Type    | Local Area Network that connects devices in a small physical area          | Limited to building   | Home network, School/Office network               |
| **WAN**       | Network Type    | Wide Area Network connecting multiple LANs over long distances             | City to Global        | Corporate branches, cellular networks             |
| **Internet**  | Global Network  | Interconnection of millions of WANs and LANs globally                      | Worldwide             | Web browsing, email, video streaming              |

---

### 🧠 Summary

- **Ethernet** and **Wi-Fi** are methods of connecting to a **LAN**.
- **LANs** can be connected over long distances using **WANs**.
- The **Internet** is a global network made up of interconnected LANs and WANs.
