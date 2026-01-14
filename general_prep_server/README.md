
# install ansible 
## might need to install python and/or pip
    sudo apt update
    sudo apt install pipx
    pipx ensurepath
    sudo pipx ensurepath --global # optional to allow pipx actions with --global argument
    pipx install --include-deps ansible


# running a playbook

    ansible-playbook -i hosts.yml daily_backups.yml --ask-vault-pass

# creating a encrypted secret
    ansible-vault encrypt_string 'password' --name 'sshfs_password'



# exmple of pinging a host 
    ping example

    ansible all -m ping -v


    list all hosts
    ansible all --list-hosts -i ?????



