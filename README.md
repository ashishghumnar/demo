Configure Merge tool in git p4Merge

$ got config --global diff.tool p4merge

git local states
---working directory - all files and folders in directorey (may or may not be on repo)
---staging area - modfified files gets into staging area
---repository or commit history --this is what to get to git repository

Remote stage 

create command alias 

git config --global --alias.<command-alias-name> <actual command>;

git add .gitignore file to ignore files

git add -u  -- to track updated files only
git add -A -- to track all changes like deleting , renaming etc

advance commands

like diffe , merge  

configure p4Merge for looking at diff

git diff (sho diff against head)
git difftool show diff in p4Merge
git diff <id> <id>
git diff <id> <id>

options passed to diff can be passed to difftool


Branching
	branch is timeline of commit
	branch names are labels
	
	we can create new branch from master --|master brach
		                                   |
                                           |-----create another brach from master| 
										   |                  |                  |
										   |                                     |
										   |                                     |
										   ||<-----------<--<--| Merge back to master
										   |
										   |-----create another brach from master| 
										   |                  |                  |
										   |                                     |
										   |                                     |
										   ||<-----------<--<--| Merge back to master
										
										
	Merge Type
		Fast Forward Merge
			Simplest Case if no additional changes on master branch
			
			automatic merge
			HEAD last comit of branch
			
			
-Changing Item one
-TestOne 		
