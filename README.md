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

**8) What is the basic difference between BASH and DOS?**

The key differences between the BASH and DOS console lie in 3 areas:

- BASH commands are case sensitive 
 * while DOS commands are not;

- Under BASH, / character is a directory separator and \ acts as an escape character. 
* Under DOS, / serves as a command argument delimiter and \ is the directory separator


**9) Describe the root account.**

* The root account is like a systems administrator account and allows you full control of the system.
* Here you can create and maintain user accounts, assigning different permissions for each account.
* It is the default account every time you install Linux.

**10) What is CLI?**

* CLI is short for Command Line Interface.
* This interface allows the user to type declarative commands to instruct the computer to perform operations.
* CLI offers greater flexibility.

**11) How do you open a command prompt when issuing a command?**

* To open the default shell (which is where the command prompt can be found), press **Ctrl-Alt-F1**.
* This will provide a command line interface (CLI) from which you can run commands as needed.

**12) How can you find out how much memory Linux is using?**

* From a command shell, use the **"concatenate"** command: **cat /proc/meminfo** for memory usage information. 
* You should see a line starting something like Mem: 64655360, etc.
* This is the total memory Linux thinks it has available to use.

* You can also use commands

```free - m

vmstat

top

htop
```

to find current memory usage


**13) What is the maximum length for a filename under Linux?**

* Any filename can have a maximum of 255 characters.
* This limit does not include the path name, so therefore the entire pathname and filename could well exceed 255 characters.

**14) What is the pwd command?**

* to find **present work directory**

**15) What are environmental variables?**

* Environmental variables are global settings that control the shell's function as well as that of other Linux programs.
* Another common term for environmental variables is global shell variables.

**16) What are the different modes when using vi editor?**

* There are 3 modes under vi:- Command mode – this is the mode where you start in
* - Edit mode – this is the mode that allows you to do text editing
* - Ex mode – this is the mode wherein you interact with vi with instructions to process a file


**17) What is grep command?**

* grep a search command that makes use of pattern-based searching.
* It makes use of options and parameters that are specified along with the command line and applies this pattern in searching the required file output.

**18) What are the contents of /usr/local?**

* It contains locally installed files.
* This directory matters in environments where files are stored on the network.
* Specifically, locally-installed files go to /usr/local/bin, /usr/local/lib, etc.). Another application of this directory is that it is used for software packages installed from source, or software not officially shipped with the distribution.


**19) How do you terminate an ongoing process?**

* Every process in the system is identified by a unique process id or pid.
* Use the kill command followed by the pid to terminate that process.
* To terminate all process at once, use kill 0.

**20) Write a command that will look for files with an extension "c", and has the occurrence of the string "apple" in it.**

```
 Find ./ -name "*.c" | xargs grep –i "apple"
```

**21) Write a command that will display all .txt files, including its individual permission.**

```
ls -al *.txt
```

**22) Write a command that will do the following:**

-look for all files in the current and subsequent directories with an extension c,v
-strip the,v from the result (you can use sed command)
-use the result and use a grep command to search for all occurrences of the word ORANGE in the files.

```
Find ./ -name "*.c,v" | sed 's/,v//g' | xargs grep "ORANGE"
```

**23) What is the command to calculate the size of a folder?**

* To calculate the size of a folder uses the command **du –sh folder1.**

**24) How can you find the status of a process?**

* Use the command

```
ps ux
```
**25) How can you check the memory status?**

You can use the command

* **free -m** to display output in MB

* **free -g** to display output in GB

**26) How can you append one file to another in Linux?**

* To append one file to another in Linux you can use command **cat file2 >> file 1.** 
* The operator >> appends the output of the named file or creates the file if it is not created.
* While another command **cat file 1 file 2 > file 3** appends two or more files to one.

**27) Explain how you can find a file using Terminal?**

* To find a file you have to use a command, 
```
find . –name "process.txt" .
```
 It will look for the current directory for a file called process.txt.

**28) Explain how you can create a folder using Terminal?**

* To create a folder, you have to use command **mkdir.** It will be something like these: ~$ mkdir Guru99

**29) Explain how you can view the text file using Terminal?**

* To view the text file, go to the specific folder where the text files are located by using the command cd and then type less filename.txt.

```
less filename.txt
```

**30) Explain how to enable root logging in Ubuntu?**

* The command which enables root logging is

```
#sudo sh-c 'echo "greater-show-manual-login=true" >>/etc/lightdm/lightdm.conf'
```