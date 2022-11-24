# Demo

Description

#### Clone the repo
Clone this repo into my machine using VS terminal.
->Folder-Name `git clone SSH | HTTPS`

+ When cloning the repo there will be a hidden folder : `.git` 
to see it type the cmd : `ls` (short of ls -la)

+ Try now to change the README.md file, and add a new file index.html for example.
+ to see what has been updated : `git status`
this will tell us that the README.md file has been updated, and the new index.html file is `Untracked`, meaning git doesn't know about this file yet.
+ to made the changes into git and track the untracked files we use : `git add .`
+ now we need to commit files into github : `git commit -m "Added index.html" -m "Some desc for desc box"`
+ this last command just saved the files locally. To do it remotally : `git push`
+ we need to prove to github that we're the owner of our accound : 
to connect locally to remotlly : 

1- Generate the SSH 
```
ssh-keygen -t rsa -b 4096` -C "email@example.com"
> the name of the file to save the SSH key, name it for example : testkey
```

2- Search for that file : `ls | grep testkey`
```
testkey (use to tell github that i'm the owner)
testkey.pub (its OK to others to see this)

> to see the public key : cat testkey.pub
to copy it just highlight it :)
or use the command to make you copy : pbcopy < FILE_FILE (./testkey.pub)

```


3- go to github/settings/SSH and GPG keys> Click on : `new SSH key`
4- Adding the SSH key to the ssh-agent: wwe need to make sure that the local CLI knows about the just generated key, we need to modify the `~/.ssh/config` check this link : 
[SSH key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#adding-your-ssh-key-to-the-ssh-agent)


+ Now we need to push the work into github : 
`git push origin master`
-> origin : an option that stands for the location  of our git repo.

--- 










---
This crash course from : [FreeCodeCamp](https://www.youtube.com/watch?v=RGOj5yH7evk)





