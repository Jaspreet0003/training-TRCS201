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
?	Matches exactly one character	file?.txt
[ ]	Matches one character from the set	file[1-3].txt
[! ]	Matches one character not in the set	file[!0-9].txt
{a,b,c}	Matches any listed string	file{1,2}.txt
{1..5}	Matches a range of values	file{1..5}.txt

📝 Escaping Characters in Linux
In Linux, certain characters like *, $, ", ', &, etc., have special meanings in the shell. Escaping characters prevents the shell from interpreting them and treats them as plain text.

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

📌 Types of Quotes:
Type	Purpose	Example	Output
Single Quotes '	Preserves everything literally inside	echo '$HOME'	$HOME
Double Quotes "	Expands variables but preserves spaces, etc.	echo "My home is $HOME"	My home is /home/user
Backslash \	Escapes a single character	echo \$HOME	$HOME

💻 Hardware: Basics of Computer Components
Hardware refers to the physical, tangible components of a computer system — the parts you can touch, unlike software which is a set of programs and data.

📌 What is Computer Hardware?
It includes everything from the CPU to the monitor, keyboard, mouse, storage devices, and other peripherals.

🔧 Basic Computer Hardware Components:
Component	Function
CPU (Processor)	The brain of the computer, processes instructions
Motherboard	Connects and manages all hardware components
RAM (Memory)	Temporary storage for quick data access
Hard Drive / SSD	Long-term storage for files and programs
Power Supply Unit	Converts electricity to power the computer
Input Devices	Devices like keyboard, mouse, scanner
Output Devices	Devices like monitor, printer
Graphics Card (GPU)	Manages graphics and image rendering
