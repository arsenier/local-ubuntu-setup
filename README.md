A personal ansible playbook to set up my local machine for ubuntu or any distro based on it

## Requirements:
- ansible (can be installed via `install_ansible.sh`)
- passwordless sudo, one way is to do `sudo visudo` and then add `username ALL=(ALL) NOPASSWD: ALL` at the end of the file

## Useful commands
- `ansible-playbook local.yml --ask-vault-pass` to apply changes locally
- `ansible-pull -U https://github.com/tanqhnguyen/local-ubuntu-setup.git --ask-vault-pass` to pull from git and apply changes at the same time
- `ansible-vault encrypt_string --ask-vault-pass <string>` to create a new encrypted string to use in the playbook