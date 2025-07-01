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

