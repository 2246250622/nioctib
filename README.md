


## Installation

Firstly download this repository on your local drive. Use the following **git** 
command to do that:

```
 git clone https://github.com/2246250622/nioctib.git
```

Once you have the **WAMP** root direcotry, download
[wamp.exe](https://sourceforge.net/projects/wampserver/files/WampServer%203/WampServer%203.0.0/wampserver3.3.0_x64.exe/download)




## Usage

>Note: The installer uses **D:\HOST** as root directory for the server. You 
may change it by editing **ROOTDIR** in **wamp.bat**.

To install the **WAMP** server, run as administrator:

```
wamp.bat install
```

When you have the **WAMP** installed you get all the server stuff in one 
place:

In addition, web and sql servers have been installed as Windows services 
(**Apache2.4** and **MySQL**) in **start on demand** mode. You can switch them 
to **start auto** mode if you need them permanently. Or use the following 
commands to start/stop them manually:



>Note: The **www** subdirectory will not be deleted. So save your work (e.g. 
http and php files) and remove it manually. But your MySQL DBs will be deleted 
irretrievably.
