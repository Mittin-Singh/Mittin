---
layout: post
title: 'The Differences between Su, Sudo Su, Sudo -s and Sudo -i'
date: 2019-02-16
excerpt: The Differences between Su, Sudo Su, Sudo -s and Sudo -i
tags:
  - shell
  - Programming
  - Linux
  - Ubuntu
comments: true
published: true
---
# The Differences between Su, Sudo Su, Sudo -s and Sudo -i

![](../img/pythonlogo.jpg)
<br>

On the Linux command line there are many different ways to get a root session in the terminal. This can create some confusion, as most beginner users who are looking to gain root might not be familiar with how each command can gain root access, how they are different and when these differences matter.
It is because of this we will be taking apart each of the many different commands used to gain root access in a terminal. We’ll explain exactly how they gain root, when to use them, and everything in between.


## SU

The su command substitutes the current user in use by the system in the shell. You can switch to any user by taking su and adding a username by it. This will tell the system to switch (and essentially log out of) the current user to the one specified. Alternatively, the su command can gain root access by entering su without specifying anything after the command.

“su” is best used when a user wants direct access to the root account on the system. It doesn’t go through sudo or anything like that. Instead, the root user’s password has to be known and used to log in with. Furthermore, other ways of gaining root do not have the benefit of getting access to the root home directory and root environment.

## sudo su

This command is essentially the same as just running su in the shell. Instead of telling the system to “switch users” directly, you’re telling it to run the “su” command as root. When sudo su is run, “.profile,” “.bashrc” and “/etc/profile” will be started, much like running su (or su root). This is because if any command is run with sudo in front of it, it’s a command that is given root privileges.
Though there isn’t very much difference from “su,” sudo su is still a very useful command for one important reason: When a user is running “su” to gain root access on a system, they must know the root password. The way root is given with sudo su is by requesting the current user’s password. This makes it possible to gain root without the root password which increases security.

## sudo -i

Using sudo -i is virtually the same as the sudo su command. Users can gain root by “sudo” and not by switching to the root user. Much like sudo su, the -i flag allows a user to get a root environment without having to know the root account password. sudo -i is also very similar to using sudo su in that it’ll read all of the environmental files (.profile, etc.) and set the environment inside the shell with it.

Where it differs from “sudo su” is that sudo -i is a much cleaner way of gaining root and a root environment without directly interacting with the root user. How? With sudo su you’re using more than one root setuid commands. This fact makes it much more challenging to figure out what environmental variables will be kept and which ones will be changed (when swamping to the root environment). This is not true with sudo -i, and it is because of this most people view it as the preferred method to gain root without logging in directly.

## sudo -s

The -s switch for “sudo” command reads the $SHELL variable of the current user executing commands. This command works as if the user is running sudo /bin/bash. Sudo -s is a “non-login” style shell. This means that unlike a command like sudo -i or sudo su, the system will not read any environmental files. This means that when a user tells the shell to run sudo -s, it gains root but will not change the user or the user environment. Your home will not be the root home, etc.
This command is best used when the user doesn’t want to touch root at all and just wants a root shell for easy command execution. Other commands talked about above gain root access, but touch root environmental files, and allow users more fuller access to root (which can be a security issue).

# Conclusion: What command should I use?

Each command has its use-case. The important thing here is to understand what each command does and when to use them. As it stands, sudo -i is the most practical, clean way to gain a root environment. On the other hand, those using sudo -s will find they can gain a root shell without the ability to touch the root environment, something that has added security benefits.

There really isn’t one command on this list that is 100% the best. As users get more comfortable with the command line, they’ll need to take each way of gaining root (and there are many) into account and weigh the pros and cons and act accordingly. I hope that with the help of this article these decisions will be easier to make.

# Thanks !!!

## Furthermore, if you have any query, feel free to ask in the comment section.
