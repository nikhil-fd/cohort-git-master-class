# VCS (Version Control Sysytem)
- Version control means, we write code in a separate file in 50 line or 100 line or many more. so to track this code like when you modify or replace or insert or delete code such thing controlled by VCS and VCS is made by Git and Git is developed by Linus Torvalds who is owner of Linux Operating Systen and GIT.
### 1️⃣First created a repository/folder for a Project
- Then goto that folder directory through git bash command line.
- Now we need to do version control to this project folder/repository. so use command below👇
```git
git init
```
- After use command "git init" then it will initiate/initialize version control to this project folder or file.

### 2️⃣Then all file will become U (means UNTRACKED)
- So we need to do TRACKED the file using below command👇
```git
git add <filename>
```
- The above command will TRACK to a single individual file.
- The below command can TRACK to all file.👇
```git
git add .
```
- The below command will show all details regarding all file like which file MODIFIED or UNTRACK or TRACK etc.👇
```git
git status
```
### 3️⃣Then All file become A (means INDEX ADDED)
- Now we need to commit theses file with a message. use below command.👇
```git
git commit -m "explained how git works"
```
- After used commit it creates a individual HASH or (id).
### To track the history of project file use👇
```git
git log
```
### To track what modified in a file and when modified like add or delete👇
- use "git diff" just after modified data and symbol will be M(blue color) means befor use command add.
```git
git diff <filename>
```
- To track all file modification use👇
```git
git diff
```
### how to execute a file or render the data of a file use👇
```git
cat <filename>
```
### Below command can render hash file data
- goto project folder - cd .git/objects/70 
```git
git cat-file -p <hash>
```




