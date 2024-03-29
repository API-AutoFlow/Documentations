---
layout: default
title: OS Command
parent: System
grand_parent: Internal Actions
---
# OS Command
Single-line Operating System (OS) command.

## Properties
```yaml
Command: operating system command
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
There are 3 ways to run multiple shell commands in one line:

1. Use `;`
No matter the first command cmd1 run successfully or not, always run the second command cmd2:
```
$ cd ~/Documents; ls
```
no matter cd to ~/Documents successfully, run ls

2. Use `&&`

Only when the first command cmd1 run successfully, run the second command cmd2:
```
$ cd ~/Documents && ls
```
run ls only after cd to ~/Documents

3. Use `||`

Only when the first command cmd1 failed to run, run the second command cmd2:
```
$ cd ~/Documents || ls
```
if failed cd to ~/Documents, `ls` will run
