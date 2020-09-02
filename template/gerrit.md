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
