## Ohmyzsh

- doesn't work because of the user.
- also you cannot re-install it or else it breaks.
  - had to put a little file exist protector

### Permissions with ssh

I think its a user issue. I think that if I redo it with --become-user theprimeagen it will work better.
remove all become_user root

sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
 https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'

### NVIM

bad order of tasks.

### Ansible pull

no vault
make it clone
--become-user theprimeagen
-t install . I just keep forgetting this...
example

ansible-playbook -t install local.yml -vvv --ask-become-pass

- clone it with https then change remote to ssh once ssh is up.
