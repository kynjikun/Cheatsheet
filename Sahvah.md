CHEAT SHEET
----

*Login*
```
ssh -I <path to PEM key> <username>@<ip address>
```

*Upgrade Server* (centOS)
 
```
sudo yum update && sudo yum upgrade -y
```

Create Directory
```
mkdir <name>
```

Create file
```
touch <filename>.<extension>
```

Delete
```
rm <filname>.<extension>
```

Copy 
```
cp <filename> <directoryname>/.
```

Copy to another name
```
cp <filename> <name>
```

Rename
```
mv <filename>.<extension> <filename>.<extension>
```

Move
```
mv <filename>.<extension> <directoryname>
```

Current Path
```
pwd
```

Edit File
```
vim
```

Vim Commands
```
: <- every vim commands starts with
: set mouse=nicr <- enable 
:?<text> <- search
:w <- save file
:q <- exit file
:wq <-save  and exit file
```
Change File Permission (Read,Write,Execute)     
```
r=1
w=2
x=4
chmod <rwx><rwx><rwx> <filename>.<extension>
```

Apply Permission to all files with a directory
```
Chmod <permission mask e.g 777> -R <directoryname>/
```

Volume Status
```
df -h
```

extract
```
tar xzvf <filaname>.tar.gz
```
compress
```
tar czvf <filaname>.tar.gz /directory
```
######_______________________________________#####
######_______________________________________#####

#Update Server
######login to Server
```
ssh <user>@<ip address> -p <portnum> 
```

######display list of accounts
```
ls /home
```
######login as 
```
sudo su - <user>
```
######find Directory to update
```
cd <directory>
```
######fetCh update from git
```
git fetch
```
######Check Branch currently On
```
git branch
```
######apply fetched Update from git
```
git pull
```
######compile the file
```
./activator stage
```
######Check Process to Kill(PID)
```
netstat -tuplen
```
######Kill Process
```
kill <PID num> 
	or 
kill `cat target/universal/stage/RUNNING_PID`
```
#######sometime
```
Sudo rm <PIDpath>
```
#######Start Server and Daemonize
```
./activator start -J-server
	**ctrl + D**
```
	 
#_____________________
#_____________________



#Setting up Server centOS

Install net tools
```
 sudo yum install net-tools -y
```

Upgrade server
```
 sudo yum upgrade -y
```
Install Basic app
```
 Sudo yum install git vim wget -y
```






