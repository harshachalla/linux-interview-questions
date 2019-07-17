# linux-interview-questions

**1) What is Linux?** 
* Linux is an operating system based on UNIX and was first introduced by Linus Torvalds.
* It is based on the Linux Kernel and can run on different hardware platforms manufactured by Intel, MIPS, HP, IBM Etc..

**2) What is the difference between UNIX and LINUX?**
* Unix originally began as a propriety operating system from Bell Laboratories, which later on spawned into different commercial versions.
* Linux is free, open source and intended as a non-propriety operating system for the masses.

**3) What is BASH?**
* BASH is short for Bourne Again SHell. It was written by Steve Bourne as a replacement to the original Bourne Shell (represented by /bin/sh).

**4) What is Linux Kernel?**

* The Linux Kernel is a low-level systems software whose main role is to manage hardware resources for the user.
* It is also used to provide an interface for user-level interaction.

**5) What is LILO?**

* LILO is a boot loader for Linux. 
* It is used mainly to load the Linux operating system into main memory so that it can begin its operations.

**7) What is the advantage of open source?**

* Open source allows you to distribute your software, including source codes freely to anyone who is interested. 
* People would then be able to add features and even debug and correct errors that are in the source code.
* They can even make it run better and then redistribute these enhanced source code freely again.
* This eventually benefits everyone in the community.

**10) What is the basic difference between BASH and DOS?**

The key differences between the BASH and DOS console lie in 3 areas:

- BASH commands are case sensitive 
 * while DOS commands are not;

- Under BASH, / character is a directory separator and \ acts as an escape character. 
* Under DOS, / serves as a command argument delimiter and \ is the directory separator


**12) Describe the root account.**

* The root account is like a systems administrator account and allows you full control of the system.
* Here you can create and maintain user accounts, assigning different permissions for each account.
* It is the default account every time you install Linux.

**13) What is CLI?**

* CLI is short for Command Line Interface.
* This interface allows the user to type declarative commands to instruct the computer to perform operations.
* CLI offers greater flexibility.

**15) How do you open a command prompt when issuing a command?**

* To open the default shell (which is where the command prompt can be found), press **Ctrl-Alt-F1**.
* This will provide a command line interface (CLI) from which you can run commands as needed.

**16) How can you find out how much memory Linux is using?**

* From a command shell, use the **"concatenate"** command: **cat /proc/meminfo** for memory usage information. 
* You should see a line starting something like Mem: 64655360, etc.
* This is the total memory Linux thinks it has available to use.

* You can also use commands

```free - m

vmstat

top

htop```
to find current memory usage