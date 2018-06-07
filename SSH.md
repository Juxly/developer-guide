# SSH Keys

You will need an SSH key to access the code on bitbucket.

## Generate an SSH Key

1. ssh-keygen -t rsa -b 4096 -C "youremail@juxly.com"

2. Copy public key to clipboard `cat ~/.ssh/id_rsa.pub | pbcopy`

3. Add public key to bitbucket

4. Now you're ready to pull down some repos
