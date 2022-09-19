*Personal notes, open to corrections!

# Git Notes 

## Command Line Keys

I am using [Hyper](https://hyper.is/) terminal. 

To navigate: 
```php 
~ % ls     # List - prints what is inside of the folder
~ % cd     # Change directory 
~ % cd..   # Back one level 
~ % ls -a  # Shows also hidden files
▼▲         # Use  to scroll through previous commands 
```
To manage Files: 
```php
~ % mkdit                    # Creates new folder (Makes new directory)
~ % touch Name.txt           # Creates new txt file 
~ % open Name.txt            # To open file
~ % open -a AppName Name.txt # To specify what app you want to open the file with 
~ % rm Name.txt              # Delete file (Not directory!)
~ % pwd.                     # Entire path (to where you are)
~ % rm*                      # To delete all the files in directory 
~ % rm -r NameOfDirectory/   # Removes directory 
```

## Git Commands


**Create your file** --> There is a **Working Directory** (Where our file is created and where you initiate your git) --> **Staging Area** (Git Index - for a set of changes that are to be committed together) --> **Repository** --(Git Checkout)--> **Working Directory** 

```php
~ % git init                   #Initialize empty Git repository in the current location 
~ % git add Filename           # Adds File to staging area to start tracking changes 
~ % git status.                # Status 
~ % git rm -- cached <File>... # To unstage ( ?????????) 
~ % git commit -m "Message"    # Commit (Message in present tense) 
~ % git log                    # to see what commits you have made
~ % git add .                  # To add all files in the directory 
~ % git diff                   # To check what was modified 
~ % git checkout FileName.txt  # To rollback to the last version 
```
## Steps
*Name stands for name of directory

- **~ % mkdir Name** *Create new folder (directory):*
       
- **~ % cd Name** *Move to this new directory:*
- **~ % git init** *Initialize git repository:*
- **~ % touch FileName** *Create new file in the directory:*
- **~ % open FileName** *To open the file:*
- **~ % git add FileName** (or **.** for all the files) *Add the file to staging area:*
- **~ % git commit -m "Message"** *Commit:*
- **~ % git status** *Check status:*
- **~ % git log** *Check what commits you've made:*
- **~ % git diff** *Check what was modified:*
- **~ % git checkout** *To rollback:*

## Remote Repositories 
(Stored on someone's else computer/server) 






"...or push an existing repository from the command line" --(copy repository address)--> 
```php
~ % git  remote add origin URLOfRepository #Here you literally told git that you created the remote repository somewhere on the Internet
```
***Origin** - name of your repository 



```php
~ % git push -u origin master # Push our local repository to the remote repository 
```
***master** - name of branch 

***-u** - links local and remote (u-option) 

## Contributing
Pull requests are very welcome. I acknowledge the possibility of some uncertainties and mistakes I might have made. Please, feel free to correct me, I will be really grateful! 
