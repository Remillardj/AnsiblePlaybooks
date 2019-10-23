# Easy play to create sudo user

## What does it do?
1. Create a user by taking in public key
2. Setups wheel group
3. Appends user in wheel group for passwordless sudoing
4. manually creates home directory as Ansible says using `createhome=yes` is deprecated 

## Usage
```
ansible-playbook play_setup_sudo_user.yaml --extra-vars "user=<your desired username here> pubkey=<rsa pub key>"
```
