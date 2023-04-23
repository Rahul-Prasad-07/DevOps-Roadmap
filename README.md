# DevOps-Bootcamp

## Concepts & Hands on Demos
- Operating system : Linux
- Version Control : Git
- Build Tools : Npm & Gradle
- Artifact repository manager : Npm repository
- CI/CD : Jenkins
- Cloud - laas : AWS
- Infrastructure Provisioning : Terraform
- Go Lang Programming : Go Lang
- Container : Docker
- Container orchestration : Kubernetes
- Configuration managment : Ansible
- Monitoring : Promothes


## Cloud Platform
- Aws
- Digital Ocen
- Linod

## Complete DevOps Pipeline

Test --> Build --> Deploy --> Configure --> Monitor

## Software Development Life cycle

Plan --> Implement --> Test --> Deploy --> Maintain 

- programming
- software testing
- operation
 - build application
 - run on server
 - upgrade existing software 

### development 
- programming
- test framework
- database
- version control

### operation
- os, mostly Linux
- command line 
- scripting
- monitoring tools

## Waterfall vs Agile

## Operating system

### Intro to operating system 
- what is operating system?
- how it is constructed ?
- how os differ from each other ?

### Virtualization
- what virtualization and virtual machine?
- why virtualization is useful
- hypervisor 
- how virtualization works 
- why companies adopting virtualization?



### Linux file system
- linux vs windows
- what is binary
- /bin, /sbin, /lib, /usr, /user/local,/opt, /root, /etc, /dev, /var, /var/catch, /var/log, /tmp, /media, /mnt, 
- interaction with root 

### Main linux command
- Intro to command line
- GUI vs CLI
- pwd, ls, cd, mkdir, touch(file name), rm(file name), rm -r, clear, cd /- root folder, 

### Package Manager
- how to install software on linux?
- what is software package?
- download, install or update software from repository
- where do i get pakage manager?
- in ubuntu: APT - advance package tool
- sudo apt search openjdk
- copy command: Swift+ Ctrl+ c 
- paste command: Swift+ Ctrl+ v
- APT-GET & APT( we use this )
- Updating package: sudo apt update 
- where do these packages come from ? 
  - remote repository
  - package manager fetch from it
- you need alternative ways to install software
 - ubuntu software center 
 - snap package manager 
 - add repository: add-apt-repository
- package manager fot other linux distros
  - Debian based 
    - ubuntu, debian,int : APT & APT-GET
  - Red hat based 
    - RHEL, centOS, Fedora : YUM



### Vim Editor
- how to edit or write a file in CLI? 
 - built-in text editor in linux 'VI or VIM'
- why not just use GUI editor
  - small modification can be faster 
  - faster to create and edit at same time
  - support multiple format
  - when working on remote server

  - Git CLI : writing git commit messages
  - Display kubernetes configuration file
  - quickly editing one line or chat in file

- working with vim editor
   - Command Mode 
     - this is default mode
     - you can't edit text
     - whatever you type is interpreted as command 
     - navigate, search, delate, undo etc 
 
   - Insert Mode 
     - allows you to enter text
 
 
   - To switch command mode to insert mode type : i key 
   - press esc key for switching command mode
   - to save & quit vim : ( :wq ) key 
   - delete next 10 line : type d10
   - for undo : type u 
   - Type A : jump to end of line ans switch to insert mode
   - type 12G : go to line 12
   - type /pattern : search pattern 
   - type :%s/old/new : replace olf with new thorughtout the file 

### User & permission
- User accounts 
- Groups & ownership & file permission
- Linux commands for managing users and thier permission


- 3 Users category
  - superuser account
    - Root user : unrestricted permission
  - User account
    - a regular user we create to login
  - service account
    - relevant for linux distros & each service will get its own user, eg. mysql user will start mysql application
    - best practices for security
    - don't run service with root user

- why multiple standard users?
  - shared computer like in schools 
- how does it work ?
- centrally managed user permission in windows & that's one of the reason companies and school refer windows system
- multiple user in linux 


- multiple users on server 
  - for linux having multi-user is important for Servers 
  - usually teams administer a server 
- why not just use shard server ? 
  - they need non root user 
  - permission per team member 
  - traceability: who did what on system? 
  - admin create user with permission 

### Groups & permission
- How to manage permission?
- 2 level permission
  - User level : give permission to user directly 
  - Group level : group users into linux group & give permission to that group.this the way to go,if you manage multiple users.

- we have different groups like 
  - Devops team or group 
  - Admin team or group
  - Devloper teams or group
users are added to the group & permission for that group 
    

### Shell scripting
### Environment variables
### Networking
### SSH - Secure Shell






