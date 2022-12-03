# dotfiles
This is a dotfiles repository, for the use with an aliased git bare repo.

### Initialisation
`git init --bare ~/.dotfiles`

### Alias
`alias dotfiles='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'`

### Prevent showing untracked files
`dotfiles config --local status.showUntrackedFiles no`

### Add the repository folder to gitignore - prevent recursion
`echo ".dotfiles" >> .gitignore`

## Git cheat sheet

### Fetch remote branch and put it in local one
`git fetch <remote_repo> <remote_branch>:<local_branch>`

### Merge only one file from another branch
`git checkout -m <branch_name> <yourfilepath>`

