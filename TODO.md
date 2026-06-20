
### Permissions with ssh

I think its a user issue. I think that if I redo it with --become-user theprimeagen it will work better.
remove all become_user root

sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
 <https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim>'

### NVIM

bad order of tasks.

### Ansible pull

no vault
make it clone
--become-user theprimeagen
-t install . I just keep forgetting this...
example

Create ~/.vault_pass.txt put your password

ansible-playbook -t install local.yml -vvv --ask-become-pass

ansible-playbook -t dotfiles local.yml -vvv --ask-become-pass

uv tool install "vectorcode[lsp,mcp]<1.0.0" --python python3.13

Open Alacritty.app once, then go to System Settings → Security & Privacy → General and click “Open Anyway” for Alacritty.

- clone it with https then change remote to ssh once ssh is up.
