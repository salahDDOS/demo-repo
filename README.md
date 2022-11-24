# Demo

Description

### Clone the repo
Clone this repo into my machine using VS terminal.
->Folder-Name `git clone SSH | HTTPS`

+ When cloning the repo there will be a hidden folder : `.git` 
to see it type the cmd : `ls` (short of ls -la)

+ Try now to change the README.md file, and add a new file index.html for example.
+ to see what has been updated : `git status`
this will tell us that the README.md file has been updated, and the new index.html file is `Untracked`, meaning git doesn't know about this file yet.
+ to made the changes into git and track the untracked files we use : `git add .`
