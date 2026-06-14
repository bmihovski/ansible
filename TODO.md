
### Permissions with ssh

All members of the sudo group to execute any commands using passwordless sudo, change the configuration with visudo to:
%sudo   ALL=(ALL:ALL) NOPASSWD:ALL

### Ansible pull

no vault
make it clone
--become-user theprimeagen
-t install . I just keep forgetting this...
example

## Set Ansible vault password

Create ~/.vault_pass.txt put your password

## Install software dependencies

ansible-playbook -t install local.yml -vvv --ask-become-pass

## Apply apps configuration

ansible-playbook -t dotfiles local.yml -vvv --ask-become-pass

pipx install vectorcode

- clone it with https then change remote to ssh once ssh is up.

### Setup zsh at system level

Add the shell to system configuration

```shell
sudo sh -c "echo /home/linuxbrew/.linuxbrew/bin/zsh >> /etc/shells"
```
