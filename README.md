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

- User mangement in practice
 - access control files 
   - /etc/password : stored user account info & everyone can read it but root user can only change the file.
   - /etc/shadow 
   - /etc/group
    

### Shell scripting
### Environment variables
Till now you have coverd 
 - Basic linux commands 
 - Basic Shell scripting
 - You can have multiple users on linux os and Windows os
 
In the environment module
  - Each users have its own env
  - Each user can configure it's own env/account by setting pref 
  - these os configuration should be isolted from the user environment 
Where does os store all these configurations?
--> Environment Variables & its usecases 
  - Os store infro about env
  - we can create our own env variables
  - variables store information
  - You can see it all env by runng **printenv** command
  
Why would we want to create own env?
 - App has to be connected with databse and severs .. for that we need credential to loggin 
 - we cant write our credential in our open code 
 - set data as env vars on server 
 - by creating these env vars, we make thrm avilable in the environment 
 - all apps and processes can now access these env vars
 - what is you have write creditials for 1000000 of servers and databse : that's where this concept make process easier and more flexible
 
How to create Env variables 
- export DB_USERNAME = dbuser by exporting it is avaible in whole system
- export DB_PASSWORD = password

How ro delate env?
- unset (name of env)

If u are using BASH, you can delcare variables in the **~/.bashrc** file

How persist env variables ?
- user specific env variables file --> `./bashrc
- for system --> /etc/environment

Add custom command/Prorgram



Commands 
- printenv USER
- printenv | grep USER
- echo $USER --> Rahul Prasad
- printenv | grep DB --> all results of env with db starting
- wq:
- source .bashrc
- vim /etc/environment
- /user/bin/ls -l
- echo $PATH


### Networking
- How does computer network works?
- How does computer connect to internet?
- what is an ip address and port?
- what is dns? 

 - Lan 
 - Ip
 - switch
 - router & wan 
 - gateway: ip address of router 
 - subnet & subnetting : process of dividing one network into two or more network
 - CIDR bloks : classless inter domain routing

Any device needs 3 pecies of data for communication : 
 - Ip address
 - subnet
 - gateway

How to make sure ip address doesn't overlap ? 
 - NAT : network address transition
 - router changes ips 



 
### SSH - Secure Shell

- Intro to SSH
 - SSH is network protocol that gives user a secure way to access computer over the internet
 - SSH refers also the suite of utilities that implement that protocol
 - ebcyrpted data communication : That means we need to authenticate 
   - 2 ways to authenticate
     - Username and Password
       - Admin create user on remote server
       - User can then connect with username and password
     - SSH Key Pair : without typing pass
       - more secure
       - Client create an SSH key pair : public key + Private key
       - keys are simply encyrpted values
       - Private key = secret key. is stored securely on the client machine
       - Public key = Can be shared. like with the remote server
       - concept like in web3
       - in development : all team members create their ssh key and admin store it on the server and they can connect.
       - If the public key of the person is not registerd on the remote server, they cannot connect to it.
      
   - SSH for services 
      - u can also add users on the remoter server for another services
      - Another services can be another app like jenkins to connect with server, to copy fs or execute some commands thier
      - example
      - Create jenkins user on app server
       - create ssh key pair on jenkins server
       - add public ssh key to authorized_key on app server
       - This way we can allow jenkins to automatically connect over ssh to over ssh to our app sever and execute stuff on cli
       
- Firewall and Port 22
 -  when one machine needs to connect with another machine then the communication must be allowed throgh **Firewall rule**.
 -  Other wise by default it's Bloked
 -  **SSH Authentication** comes after the connection : first connection must be allowed and then auth can be varified by server.
 -  Firewall always configure the **ports** where the server is accessable and that the port is always open for app.
 -   So what port and which app that run on server to accept our ssh req --> most os has SSH sevices runs by defalt on machine,
 -   By defallt that ssh server runs on port 22
 -   In firewall rule we allow access on port 22
 -   SSH is powerfull and needs to be restricted to specific ip addresses

- SSH in Action --> DEMO
  - Create Remote Server on cloud platform(digital ocen)
  - Generate SSH key pair on our laptop to access without password
  - Copy bash script file to the remoter server
  - Execute script file on remote server






