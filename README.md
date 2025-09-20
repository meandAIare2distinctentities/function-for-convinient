# Github from scratch 
- `git --version`: check your Github version.
- `cd yourfolder`: move your directory to another folder.
- `git add .`: if you create a new file on your local machine but do not use this statement, Github doesn't know about this file, so we have to apply this one to tell Git to track all the changes of these files (update a file, create a new file,...).
- `git status`: check your Github status (if it's red color, your file hasn't been tracked, use `git add .`, otherwise, green color).
- `git config --global user.email "vun67774@gmail.com"`, `git config --global user.name "vusanov"`: before using `git commit...` below, we need to verify author identity through two statements above.
- `git commit -m "some messages" -m "some decriptions"`: use to add some messages and descriptions for files we just created.

# Before performing operations such as push, pull, we need to prove to Github that you are the owner of your account, this is done by using SSH keys, for convinience, just follow these steps:
- Step 1: Open terminal.
- Step 2: Paste this text `ssh-keygen -t rsa -b 4096 -C "vun67774@gmail.com"`.
- Step 3: Enter file in which to save the key (/c/Users/YOU/.ssh/id_ALGORITHM):[Press enter] (type in your fav name, exp: gitkey).
- Step 4: Enter passphrase (empty for no passphrase).
- Step 5: Enter same passphrase again.
`gitkey` and `gitkey.pub` will be generated for you.
`cat gitkey/gitkey.pub`: totally show your created SSH keys.

`git push origin main`: push all your updated files to Github.com. 