# Terminal Commands
pwd - To get path of working directory

ls - To list all files and directories of working directory

mkdir _DirectoryName_ - To make directory of name _DirectoryName_

rmdir _DirectoryName_ - To remove directory of name _DirectoryName_

cd _DirectoryName_ - To open the directory of name _DirectoryName_

cat _FIleName_ - To make file of name _FileName_

rm _FIleName_ - To remove file of name _FileName_\

rm -rf .git - To remove .git file (undo git init)

echo -e "_Text_" >> _FileName_ - To add _Text_ to the end of the file of name _FileName_

echo -e "_Text_" > _FileName_ - To clear and add (overwrite) _Text_ to the file of name _FileName_

more _FileName_ - To display content of the file of name _FileName_

more ./-file00 - To display content of the file of name -file00 (Example for file with name starting with -)

more ./* - To display content of all files on the directory (Use * instead of name to run any command for all the files/directories)

cp -r _ExistingFile/DirectoryName_ _CreatedFile/DirectoryName_ - To create a copy of _ExistingFile/DirectoryName_ as _CreatedFile/DirectoryName_ in the working directory

file _FileName_ - To display file type

find <Parameters> - To display files that satisfy certain conditions (like size, type, permissions, have certain text in them)



# Git Commands

git init - Initialise git (start saving versions)

git config --global user.name "_username_" - To set username

git config --global user.email "_email_" - To set email

git config --list - To list all configurations

git status - Shows changes that are not committed

git add _FileName_ - Include _FileName_'s changes to be updated in the next commit

git add _DirectoryName_ - Include _DirectoryName_'s changes to be updated in the next commit

git add . - Include all files/directories' changes to be updated in the next commit

git commit -m "_Message_" - Commits changes in the files added

git log - Lists history of all commits made

git checkout HEAD~1 - Go to the previous version of the directory

git checkout master - Go to the latest version of the directory

git branch _BranchName_ - Create a branch of name _BranchName_

git checkout _BranchName_ - Go to the branch of name _BranchName_

## Merging Branches:
* git checkout master

* git merge _BranchName_ - To merge _BranchName_ to selected branch/master

Then add and commit


## Merge Conflict:
Go to the file and correct the conflict manually, then add and commit



# GitHub Commands
git remote add _RemoteName_ _RepoURL_ - Add remote to local repository (_RemoteName_ can be anything but is generally origin or upstream)

git remote remove _RemoteName_ -  Remove remote

git push _RemoteName_ _BranchName_ - Push commits of _BranchName_ to remote repository

git push _RemoteName_ - Push commits of all branches to remote repository

git fetch _RemoteName_ _BranchName_ - Downloads changes to local repository

git merge _RemoteName_/_BranchName_ - To merge _BranchName_ of remote to local repository (Similar to git merge _BranchName_)

git pull _RemoteName_ _BranchName_ - Merge changes to local repository (It is like combination of previous two, fetch and merge commands)

git clone _RepoURL_ - Clone the repository from remote to local repository



.gitignore - Add file names in this files to make then non trackable for git

<fileName>.sh file - Type commands in <fileName>.sh file to be able to run those commands in the terminal
