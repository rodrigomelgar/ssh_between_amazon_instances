# ssh_between_amazon_instances
script to enable ssh between amazon instances


## Step 1. Created RSA public keypair on each of the machine:

    cd ~
    ssh-keygen -t rsa

Do not enter any paraphrase, instead just press [enter].

## Step 2. Suppressed warning flags in ssh-config file:

    sudo vim /etc/ssh/ssh_config
    StrictHostKeyChecking no
    UserKnownHostsFile=/dev/null

