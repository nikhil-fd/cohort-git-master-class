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
- NOTE: TRACK means STAGE
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
#### 👌Through a single command can do add & commit
```git
git commit -am "put your task ralated msg"
```
- After used commit it creates a individual HASH or (id).
### To track the history of project file use👇
```git
git log
```
- Below cmd gives all commit in 1 line
```git
git log --oneline
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
### Below command can render hash file data which hash created after commit.
- 1st after use commit -m cmd then do git log and you get hash code.
- 2nd after get hash code copy that code and note down the starting 2 digit of that hash code that 2digit number name's 1 folder will be created in directory .git/two digit folder name. open that 2digit name folder here you get that hash code. 
- 3rd now go back to directory .git and from here run below cmd then it will open that hash code and we can see the committed msg details.👇
```git
NIKHIL DAS@nikhil-pc MINGW64 /d/cohort_git_github/.git (GIT_DIR!)     
$ git cat-file -p db0ae0
b0c248611572ba6b87e4d8062b656536bd
```
```git
git cat-file -p <hash>
```
- check "type" by -t👇
```git
git cat-file -t <hash>
```
⏳NOTE: In real time scenario developers should not visit .git repository again and agian. They work everything without touch .git repository. This way is pritty good.
## 4️⃣At first time if your project folder is not placed in github then follow below.
- goto github--then create a repository--give repo name--give description--select public--then click create
- After this goto vs code editor--goto project folder path in gitbash--then write below cmd--it will push your project folder to gitgub's newely created repository. 
```git
git remote add origin <repository/folder url>
```
## 5️⃣After added repository in github then push project folder from vscode editor to github.
- When 1st time push any project folder then use below cmd👇
```git
git push -u origin main
```
- Once push project folder to github then whenever any changes occured in your project file then push file to github by below cmd👇
```git
git push
```
### NOTE:⏳
- In company there is a "main" branch or some company would keep it's name as "production" or "live" branch.
- when task assigned to multiple developers then individual/private "branch" is being created under "main" branch per individual task as a ticket number.
- After task completed then the private branch directly not merged with main branch because the "main" branch is direct connected in production. 
- So if the private branch has any bugs and it merge with "main" branch then it will be impacted live business. so nobody don't do like this.
- After task completed in private branch then this task is being reviewed by review team if everything is perfect then the private branch will merge with "main" branch then automatically you work will reflect in production.

#### Create Directory/Folder and File through gitbash cmd
- for directory/folder creation
```git
mkdir <foldername>
```
- To crate ".html", ".css", ".js" ".txt" file inside a folder
```git
touch <filename.html>
```
## 6️⃣Create branch & navigate 1 branch to another branch & merge branch from private to main
- check currently you are on which branch
```git
git branch
```
- it will crate a new branch only but won't navigate to that branch automaticaly👇
```git
git branch "branch-name"
```
- navigate 1 branch to another branch👇
```git
git checkout <branchname>
```
- It will crate a new branch and simonstanonsly will be navigate to that branch👇
```git
git checkout -b <branch-name>
```
#### merge branch from "private" to "main" branch
- 1st switch branch from private to main branch.👇
```git
git checkout main
```
- then use below cmd👇
```git
git merge <private-branch-name>
```
```text
press q -- to exit from git command
```


## EXTRA:
- You can install a extension i.e. "git lens" for better git code visualizaion.






