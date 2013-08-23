# Terminate Dead Session
A script that users can load on remote systems as a back up to kill rogue processes

## Purpose 
Tool to help a Sys Ad with maintaing a system with rogue processes. Main idea is you can't get to the box with conventional methods but you can remote in. This becomes a valuable script in those cases with it being easily modifiable.

## Get the Script
Download via GitHub 
or
```bash
$ curl -L https://raw.github.com/pasqualedagostino/tds/master/tds.sh > tds.sh
```
then
```bash
$ chmod +x /path/to/tds.sh
```
## Usage
Remote into the system and run the command with no arguments. It is currently configured to kill rogue processes for the current user but could be modified for other users ( keep this in mind if you are running as root! ). Also be sure to check syntax for your distro
```bash
$ ssh username@host "bash -c ./tds.sh"
```
or
```bash
$ ./tds.sh
```
