# git_tips_tricks

Repo for Github and Git tips and tricks

tips and tricks for using git


# Setting Up First Time

1. Add user name and email

git config --global user.name "Fisrt Last"

git config --global user.email "your_email@example.com"


# Generate SSH key

1. ssh-keygen -t rsa -b 4096 -C "your_email@example.com"


# Add SSH key to ssh agent

1. eval $(ssh-agent -s)
2. ssh-add ~/.ssh/id_rsa

# Add SSH key to github account

1. cat ~/.ssh/id_rsa.pub







## Connecting to Github with SSH

### Checking for existing SSH keys
1. Open Git Bash.

2. Enter ls -al ~/.ssh to see if existing SSH keys are present:

$ ls -al ~/.ssh

# Lists the files in your .ssh directory, if they exist
Check the directory listing to see if you already have a public SSH key. By default, the filenames of the public keys are one of the following:

id_rsa.pub
id_ecdsa.pub
id_ed25519.pub
If you don't have an existing public and private key pair, or don't wish to use any that are available to connect to GitHub, then generate a new SSH key.

If you see an existing public and private key pair listed (for example id_rsa.pub and id_rsa) that you would like to use to connect to GitHub, you can add your SSH key to the ssh-agent.

## Unset email

git config --global --unset-all user.name

