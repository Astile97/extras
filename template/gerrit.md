# Submitting Patches To PixysOS Gerrit

We love new patches! Here is how you can add your patch..

First,  register at https://gerrit.pixysos.com/

Then, open a terminal and generate the ssh keys

```bash
#At this point you may as well configure your git email and user id
git config --global review.corvusrom.com.username <username you registered with>
git config --global review.corvusrom.com.email <your email you registered with>

#Then to generate SSh keys
ssh-keygen -t rsa -C "your@email.com"
```
After genrating the ssh key go to ```home/root "~/.ssh" ``` and open ```"id_rsa.pub"``` and copy the whole key and paste it in SSH Keys in PixysOS Gerrit. 

To do that, go to settings (icon in the top right corner next to user-icon) "SSH Keys" section on the left side and then paste it on "ADD NEW SSH KEY" and save it.

To Submit your first patch,go to the directory of the repo,
```bash
cd PROJECT - Eg:- cd frameworks/base Here, the repo would be PixysOS/frameworks_base
```
Now perform the changes you need to submit, and commit it.
```bash
git add .
git commit -m "your commit message that is understandable"

And save it <Ctrl X, then press Y to save and press Enter>
```

After this, the next step is to sumbit your patch to PixysOS Gerrit.
```bash
git push ssh://<username>@gerrit.pixysos.com:29418/<project> HEAD:refs/for/<branch>

example 
git push ssh://superman@gerrit.pixysos.com:29418/PixysOS/frameworks_base HEAD:refs/for/ten
```

Things you need here are your Username,Project name and the branch you committed the change!
