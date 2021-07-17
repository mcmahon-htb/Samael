# Samael

Bash script to automate the tasks of setting up an environment for and starting enumeration of a machine in the [hack the box](https://hackthebox.eu) labs

## Arguments

```
-i <ip_address> - The ip address of the machine on htb
-n <name> - The name of the htb machine
```

## Features

### Environment Variables
* Adds the ip address to an environment vairable named after the machine. For example if the machine name is Love and the ip address is 10.129.4.6 the environment variable will be $LOVE=10.129.4.6
* Adds this environment variable to the ~/.bashrc script so it will persist when you open new terminals or tmux panes

### Hosts file
* Adds an entry to the hosts file so it can be accessed with hostname.htb

### File and Folder Creation
* Creates the folders
  * ~/my_data/machines/$machine/ 
  * ~/my_data/machines/$machine/enum
* Creates a report.md template file in the $machine folder

### Starts a tmux session
* New tmux session is created, the session name is the machine name
* 

### Nmap Scan
* runs an nmap scan


### Open in Firefox
* Opens machinename.htb in two firefox tabs, one for http, one for https

