# Command Line Learning Notes

##Udacity Linux Command Line Basics

### Lesson 1 Get into the shell

A command-line interface or command language interpreter is a means of interacting with a computer programme where the user issues commands to the program in the forms of successive lines of text(command lines).

在使用终端（terminal）（终端以前是个硬件）与计算机交互以前，人们使用打孔卡把程序和数据放入计算机中。终端使用户直接向计算机程序中输入命令并立即获得回音。
command line interface 是可编程的。

shell的用处之一是管理server——地处很远的机器，且没有图形界面。首先要建立虚拟linux服务器。

**虚拟机（virtual machine）**是一个运行在windows或mac电脑上的程序，它可以运行一个不同的操作系统，我们将要在虚拟机中运行Ubuntu Linux server system.
	
	vagrant up // 运行虚拟机	
	
	vagrant ssh //log into the linux machine
	
	vagrant@vagrant-ubuntu-trusty-64:~$ Alice's tea party
	> //当输入 引号、圆括号、大括号时会break，此时输入对应的符号返回。在符号前面加\
	
	exit（ctr+D）//log out the linux machine
	
	ls //查看当前文件夹下的文件
	
	curl （地址）//从地址下载文件
	
#### Terminal vs Shell

terminal接收键盘input的命令，在显示器上显示结果，而处理命令的程序是shell。terminal中的命令默认是shell来运行，但可以用其他的程序如python interpreter来运行。
有很多不同的shell程序，linux和mac中默认的是GNU Bash, 还有其他的如TCSH，KSH，Seashell。也可以把shell命令写入文件，然后运行shell程序来执行文件——shell脚本。

### Lesson 2 Shell Commands

#### linux file names and contents

Linux 系统的file names 很灵活，不像windows一定有后缀名。

	install.sh //shell脚本
	supervisor.pem //秘钥
	
#### command history
	输入命令时按住上箭头，浏览之前输入过的命令

	history //列出所有命令历史
	
	ctrl+R //搜索命令历史