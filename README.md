# Installation
### Download and change folder
```
cd ~
git clone https://github.com/overtninja/dotfiles.git

cd dotfiles
```
### Run install
```
./install.sh
```

# Uninstallation

### Change to dotfiles folder
```
cd ~/dotfiles
```

### Run uninstaller
```
./uninstall.sh
```
- - - -
# Cool tools

You should really [check this guys project out](https://github.com/adrienverge/yamllint) if you're writing Ansible or Salt.

I add this alias to my `~/.bashrc`

    alias yams='find . -type f -name "*.yml*" -exec yamllint -f parsable {} \; | sed "s|\./||g" | egrep -v "(\.kitchen/|\[warning\])"'

Inside of one of my ansible projects I can then run

    yams
