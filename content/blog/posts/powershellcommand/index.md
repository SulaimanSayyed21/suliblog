---
date: "2024-01-12"
draft: false
title: "Powershell commands"
categories:
  - "Programming Languages"
description: "The most used Powershell commands."
tags:
  - "bash"
  - "shell"
series:
  - "bash"
images:
  - "pscm.jpg"
featured: true 

authors: 
  - Sulaiman
---


# Essential PowerShell Commands

## Introduction:
PowerShell is a powerful scripting language and command-line interface (CLI) for Windows, designed to automate tasks and manage system configurations. It offers a rich set of commands that allow you to interact with the system, manage files, configure services, and perform administrative tasks. This guide provides an overview of the most commonly used PowerShell commands, organized into logical sections for easy reference. Whether you are new to PowerShell or looking to brush up on your skills, this guide will help streamline your workflow and improve your productivity.

---

## PowerShell vs Bash

While both PowerShell and Bash are command-line interfaces used for scripting and automation, they cater to different ecosystems and have unique characteristics:

- **Platform**:  
  - **Bash** is primarily used on Unix-based systems like Linux and macOS.
  - **PowerShell** is native to Windows, although it is now cross-platform and can be used on Linux and macOS as well.

- **Syntax and Piping**:  
  - **Bash** uses text-based output and pipes commands using `|`. It operates on strings and text by default.
  - **PowerShell** uses objects, which means you can pipe objects and interact with them more directly and flexibly compared to the text-based approach in Bash.

- **Commandlets vs Commands**:  
  - **PowerShell** has cmdlets (commands built specifically for PowerShell), whereas **Bash** relies on standard shell commands and utilities.

- **Scripting**:  
  - PowerShell scripts are more focused on object manipulation, while Bash scripts are often used for text processing and file management.

PowerShell is generally favored in Windows environments for system administration and automation, while Bash is the go-to tool for Unix/Linux system administration and scripting.

---

## File and Directory Commands

### `cd`
```powershell
cd [directory]


## File and Directory Commands

### `cd`
```powershell
cd [directory]
```
Changes the current working directory to the specified path.

#### Example:
```powershell
cd C:\Users\YourName\Documents
```

---

### `pwd`
```powershell
pwd
```
Prints the current working directory.

#### Example:
```powershell
pwd
```

---

### `mkdir`
```powershell
mkdir [directory_name]
```
Creates a new directory.

#### Example:
```powershell
mkdir Projects
```

---

### `ls`
```powershell
ls [path]
```
Lists the contents of a directory. Works similarly to `dir`.

#### Example:
```powershell
ls C:\Users\YourName
```

---

### `rm`
```powershell
rm [file_or_directory]
```
Removes files or directories.

#### Example:
```powershell
rm file.txt
```

---

### `cp`
```powershell
cp [source] [destination]
```
Copies a file or directory to a new location.

#### Example:
```powershell
cp file.txt C:\Users\YourName\Documents
```

---

### `move`
```powershell
move [source] [destination]
```
Moves a file or directory to a new location.

#### Example:
```powershell
move file.txt C:\Users\YourName\Documents
```

---

## System Commands

### `get-process`
```powershell
get-process
```
Lists all the running processes on the system.

#### Example:
```powershell
get-process
```

---

### `stop-process`
```powershell
stop-process -name [process_name]
```
Stops a running process by its name.

#### Example:
```powershell
stop-process -name notepad
```

---

### `get-service`
```powershell
get-service
```
Displays the status of services on the system.

#### Example:
```powershell
get-service
```

---

### `start-service`
```powershell
start-service [service_name]
```
Starts a specified service.

#### Example:
```powershell
start-service "wuauserv"
```

---

### `stop-service`
```powershell
stop-service [service_name]
```
Stops a specified service.

#### Example:
```powershell
stop-service "wuauserv"
```

---

### `shutdown`
```powershell
shutdown /s /f /t [time]
```
Shuts down or restarts the computer after a specified time (in seconds).

#### Example:
```powershell
shutdown /s /f /t 60
```

---

## Network Commands

### `test-connection`
```powershell
test-connection [host]
```
Checks network connectivity to a specified host.

#### Example:
```powershell
test-connection google.com
```

---

### `get-netipaddress`
```powershell
get-netipaddress
```
Displays IP address information of the computer.

#### Example:
```powershell
get-netipaddress
```

---

### `get-netadapter`
```powershell
get-netadapter
```
Displays network adapter information.

#### Example:
```powershell
get-netadapter
```

---

## User Management Commands

### `get-localuser`
```powershell
get-localuser
```
Lists all local user accounts on the system.

#### Example:
```powershell
get-localuser
```

---

### `new-localuser`
```powershell
new-localuser [username] -password [password]
```
Creates a new local user account.

#### Example:
```powershell
new-localuser "newuser" -password "password123"
```

---

### `set-localuser`
```powershell
set-localuser [username] -password [new_password]
```
Changes the password of a local user account.

#### Example:
```powershell
set-localuser "newuser" -password "newpassword456"
```

---

## File Content and Text Commands

### `get-content`
```powershell
get-content [file]
```
Displays the content of a file.

#### Example:
```powershell
get-content C:\Users\YourName\Documents\file.txt
```

---

### `set-content`
```powershell
set-content [file] [content]
```
Writes content to a file.

#### Example:
```powershell
set-content C:\Users\YourName\Documents\file.txt "New content"
```

---

### `add-content`
```powershell
add-content [file] [content]
```
Appends content to a file.

#### Example:
```powershell
add-content C:\Users\YourName\Documents\file.txt "Appended content"
```

---

### `select-string`
```powershell
select-string -pattern [pattern] -path [file]
```
Searches for a pattern in a file.

#### Example:
```powershell
select-string -pattern "error" -path C:\Logs\log.txt
```

---

## PowerShell Scripting and Automation

### `foreach`
```powershell
foreach ($item in $array) { 
    # Commands to run for each item 
}
```
Iterates over a collection (like an array) and performs actions on each item.

#### Example:
```powershell
foreach ($item in $array) { 
    echo $item 
}
```

---

### `if`
```powershell
if ($condition) { 
    # Commands to execute if condition is true 
}
```
Executes a block of code if the specified condition is true.

#### Example:
```powershell
if ($x -eq 5) { 
    echo "X is 5" 
}
```

---

### `function`
```powershell
function [function_name] {
    # Function body
}
```
Defines a function in PowerShell.

#### Example:
```powershell
function greet {
    echo "Hello, World!"
}
```

---
