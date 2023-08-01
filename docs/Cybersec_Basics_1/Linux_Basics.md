# Linux basics

### What is a Linux distribution?

> A linux distro is a type of linux version. Since linux is just the kernel, many types of operating systems can be
> built on top of it.

### What is a filesystem? Why is it useful?
### What is a partition?
### How does the ext4 filesystem work? What is a directory entry? What is an inode?
### How does permission management work in Linux?
### What does it mean if a file has the following permission settings: rwxr--r--?

> The owner of the files has full permission to the file (read, write, execute), the specified group only has read 
> permissions and anyone else also only has read permission.

### What is the octal representation of the permission settings above?
### What is SUID and SGID?
### Which command is used to change the permission settings on a file or directory?

> The ``chmod`` command is used.

### What is a symbolic link?
### What does the sudo command do? What can be configured in the /etc/sudoers file?

> The ``sudo`` command gives root privileges for the current command. It requires the user password.
> In the ``/etc/sudoers`` file we can give permission to users or groups of users to be able to use the ``sudo``
> command.

### What is the difference between sudo and su command?

> ``sudo`` give temporary root privileges to run the command as root users, while the ``su`` allows us to change into 
> whatever user we want (as long as the user exists).

### What is in /etc/passwd file?

> The ``/etc/passwd`` file holds all the passwords of the system users in a hashed form.

### What is in /etc/shadow file?
### What command is used to manage services in Linux?

> ``ps``, but it only shows the services of the current terminal. To get all the system's services we can use the 
> ``-aux`` options.

### How can you install a new package in Linux?

> There are many ways. We can user the ``software center`` for ease of use. In the command line we can install ``.deb`` 
> files with the ``sudo dpkg -i software.deb`` command. We can also use ``apt`` with the ``sudo apt install software`` 
> command. If we download the installer from a website, and it is packaged in a ``tar.gz`` format, we can use the 
> following commands to install:
> ```
> # use sudo if anywhere is needed
> tar -xzf package.tar.gz or tar -xjf package.tar.bz2 # unpack the package
> cd package # hop into the extracted directory
> ./configure
> make
> make install
> ```

### What absolute path is equivalent to this relative path: /var/log/./../../etc/passwd?
### Why is it problematic from a security point of view if a group of administrators uses the same root account for system maintenance?