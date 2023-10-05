# ansible-installation-and-playbook-template-examples

Detailed steps on how to install Ansible on a (RHEL/Centos Linux) control node and also various examples on common playbooks for installing different programs/utilities or automating manual tasks on multiple nodes

In the README file, you will find other details that include quality of life improvements and things that are not part of the main focus on this Github repo

When you are creating YAML inventory files, we need to customize our vimrc file to make our life easier
when editing YAML files, because YAML does not use tabs so we have to expand tabs to spaces and we reduce the indent level

cd /home

vim .vimrc

"sets the background to dark color
set bg=dark

"turns on syntax highlighting
syntax=on

"The autocmd will make it that it will affect YAML files
"Setlocal will set some local changes
"ai is autoident, it means if we hit the return key, we return to the last indent level
"ts is tab stop and in our case we set it to 2 spaces
"sw is shift width and we set it to 2, this is used for autoindent
"et is the expand tab so that when we hit the TAB key, those tabs are translated into spaces and stored as spaces into our file
autocmd FileType yaml setlocal ai ts=2 sw=2 et
