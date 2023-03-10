
# Virtualization & Linux Fundamental
## Introduction

virtualization is the first journey to learn about cloud technology, learning is like this:
1. Virtualization

2. Linux Directory Hierarchy

3. Linux basic commands

## Cloud research
### Virtualization Concept
What Is Virtualization?

Virtualization is a process based on software or virtualization, representation of something, be it virtual applications, servers, storage space, and connections. Virtualization is one way to reduce IT costs while increasing efficiency for all types.
In this condition I learned about two types of virtualization, like this:

#### 1. Virtual Machine

Virtual Machines (VMs) are computing resources that use software, not a physical computer, to run programs and deploy applications. One or more virtual "guest" machines running on a physical "host" machine. Each virtual machine runs its own operating system and functions independently from other VMs, even though they are all running on the same host. This means, for example, that a virtual MacOS virtual machine can run on a physical PC.

![server](https://user-images.githubusercontent.com/121140952/210730524-5a947385-b484-45a1-9160-535130f3d1da.png)


#### 2. Hardware Virtualization

Hardware virtualization is a method used to create virtual versions of a physical desktop and an operating system, it uses a virtual machine manager (VMM) called a hypervisor to provide abstract hardware to multiple guest operating systems, which can then share physical hardware resources with more efficient.

![hard](https://user-images.githubusercontent.com/121140952/210731304-ec7e7841-b56a-4192-a465-188930ebebaa.png)


### Linux Hierarchy Directory

The root directory, represented by “/”, is the top level directory on the system. It contains files and subdirectories that are essential for system functioning.
For example:

• the /etc directory contains configuration files for the system.

• The /var directory holds variable data such as log files.

• /root directory is the home directory for the root user.

• /home is where the user's home directory is usually located.

• /bin contains the binary files required at system boot.

•	And many others.

![HIRARKI](https://user-images.githubusercontent.com/121140952/210732707-a6cee91f-12df-4628-abdd-63d15ef47005.png)


#### Linux basic commands

Actually, the Linux command is an application that is not equipped with a GUI display so that in order to be able to run various basic Linux commands and other commands, a Linux shell or terminal based on the CLI (command line interface) is required.

  • View the active folder address: $ pwd

  • Move to the user's home folder: $ cd

  • Move folder: $ cd destination folder. Example of moving to the /usr folder: $ cd /usr

  • Move to parent folder : $ cd .. [double colon]. The example is now in the /home/user/Documents/Data1/Data1a folder. If you want to go up one level to the Data1 folder, type $ cd ..

  • View the contents of the folder: $ ls

  • Create a folder : $ mkdir foldername

  • Create/edit files using a text editor: $ nano filename.txt or $ vi filename.txt

  • View the contents of a text file: $ cat filename.txt or $ more filename.txt

• Copy files/folders : $ cp source file destination folder

• Rename file/folder : $ mv original filename new filename

• Moving files/folders : $ mv source destination

• Delete file : $ rm filename

• Delete folder : $ rm -rf folder

• Clear the screen : $ clear

• View command history: $ history

• Create file : $ touch new filename

• And there are many other commands

## Next Steps

✍️ Describe what you think you think you want to do next.

## Social Proof

 https://cahblitaran.blogspot.com/
