# WAMP

**WAMP** project is an auto-installer for WAMP server units (Apache, MySQL, PHP) 
on 32/64-bit Windows platforms.

It's useful if you need to have installed bunch of "**Apache 2.4 + MySQL 5.6 + 
PHP 5.6**" on your Windows system quickly. Only **Windows 7, Vista, 8/8.1, 10, 
Server 2008, Server 2012, Server 2016** are supported.


## Installation

Firstly download this repository on your local drive. Use the following **git** 
command to do that:

```
 git clone https://github.com/codedim/WAMP
```

Once you have the **WAMP** root direcotry, download
[wamp.zip](https://drive.google.com/file/d/0B_8B-dFXY5lBazJHS1ZWV1hjdzQ/view?usp=sharing&resourcekey=0-B3WT1M-la3JmziQxOJVtmg)
(77M) and unzip it to **WAMP\distrib** subdirectory. From now you must to have 
the following structure of files:

```
 WAMP\
      |___ wamp.bat
      |___ README.md
      |___ distrib\
                   |___ config.php
                   |___ index.php
                   |___ unzip.exe
                   |___ WAMPx64.zip
                   |___ WAMPx86.zip
```

The **wamp.zip** consists of command line **unzip.exe** application and two 
corresponding archives: **WAMPx64.zip** and **WAMPx86.zip**. The **wamp.bat** 
script will select appropriate zip-file automatically.
	
>Note: Each zip-file has a minimal set of necessary files to start WAMP server 
up. You may build your own kit with different versions of units, extended set 
of files and modules and so on.


## Usage

>Note: The installer uses **D:\HOST** as root directory for the server. You 
may change it by editing **ROOTDIR** in **wamp.bat**.

To install the **WAMP** server, run as administrator:

```
wamp.bat install
```

When you have the **WAMP** installed you get all the server stuff in one 
place:

```
 D:\HOST\
         |___ apache\
         |___ log\
         |___ mysql\
         |___ php\
         |___ tmp\
         |___ www\
```

In addition, web and sql servers have been installed as Windows services 
(**Apache2.4** and **MySQL**) in **start on demand** mode. You can switch them 
to **start auto** mode if you need them permanently. Or use the following 
commands to start/stop them manually:

```
wamp.bat start
wamp.bat stop
```

To uninstall the server, run:

```
wamp.bat uninstall
```

>Note: The **www** subdirectory will not be deleted. So save your work (e.g. 
http and php files) and remove it manually. But your MySQL DBs will be deleted 
irretrievably.
