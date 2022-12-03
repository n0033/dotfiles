# dotfiles
This is a dotfiles repository, for usage with an aliased git bare repo.

### Initialisation
`git init --bare ~/.dotfiles`

### Alias
`alias dotfiles='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'`

### Prevent showing untracked files
`dotfiles config --local status.showUntrackedFiles no`

### Add the repository folder to gitignore - prevent recursion
`echo ".dotfiles" >> .gitignore`
