##How to create a Git MD file and push it to Git Hub

###Steps:

1) Open Git Bash, In command window write:

2) cd datasciencecoursera - to change directory

3) touch HelloWorld.md - to create text file

4) git status - to get list of modified files, in this case HelloWorld.md

5) git add HelloWorld.md - to get your files ready for committing 

6) git status - to again find status

7) git commit -m 'Added HelloWorld.md'

8) git push -u origin master

9) Git Bash will ask you for your user name and password. 

10) Refresh your GitHub repository page and you will now see the required file there.

11) Click the file and manually add comments as described in the lecture slides.  
Ref: Danish Us Salam

##Common errors and workarounds/fixes

###when faced with this error:

Pushing to git@github.com:519ebayproject/519ebayproject.git
To git@github.com:519ebayproject/519ebayproject.git
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'git@github.com:xxxxxgit'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Merge the remote changes (e.g. 'git pull')
hint: before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

###do the following:

"git push -f" or try "git pull origin master".
Ref: R Hendry

###when faced with this error:

 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'git@github.com:xxxxxgit'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

###do the following:

It is likely that you have more than one master/repository.
Simply go into the master that you dont want to use(in the git bash command prompt) and type "rm -rf .git"
This should not remove the file but change it to a non-master repository.
Then try "pushing" the data again from the master file that you do want to use.

Ref: R Hendry
