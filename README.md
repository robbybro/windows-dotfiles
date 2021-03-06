# Bash for Windows Dotfiles and Setup Instructions

These dotfiles are meant to work on Bash for Windows, providing tmux and powerline support, as well as some nice plugins. It's basically a heavily modified version of my [dotfiles for Linux](https://github.com/robbybro/dotfiles) which are in turn a lightly modified version of [anstosa's dotfiles for linux](https://github.com/anstosa/dotfiles)

## Warning - These are pretty experimental, use at your own risk

## On Thar Being Dragons
Don't edit any of your dotfiles with a windows editor. Do it all in the Linux shell. You will break everything. [Here's why](https://github.com/Microsoft/BashOnWindows/issues/904)

## Instructions
1. Clone repo: git clone git@github.com:robbybro/windows-dotfiles.git ~/.dotfiles
2. [OPTIONAL] Backup existing dotfiles
3. Install dotfiles: ~/.dotfiles/install.sh (you may need to `chmod +x install.sh`)
4. [RECOMMENDED] Restart or source ~/.bashrc in all open terminals

## What this thing does 
1. [Install tmux 2.3+ for correct utf-8 compatibility](https://gist.github.com/P7h/91e14096374075f5316e). If that fails, check [here](https://launchpad.net/~pi-rho/+archive/ubuntu/dev) for the lastest version of tmux-next for your distro.
2. [Install powerline](http://powerline.readthedocs.io/en/master/installation/linux.html). Don't forget to patch the fonts or [install pre-patched fonts](https://github.com/powerline/fonts)!
3. Install a bunch of vim plugins
4. configure a bunch of git shortcuts 

## Tips
1. [tmux displaying wrong colors?](http://askubuntu.com/questions/125526/vim-in-tmux-display-wrong-colors) run `tmux-next -2`
2. [Run Zsh instead of bash](http://www.howtogeek.com/258518/how-to-use-zsh-or-another-shell-in-windows-10/)
3. [Set up Bash for Windows inside of VS Code](https://code.visualstudio.com/docs/editor/integrated-terminal)\
4. [Bash for Windows FAQ](https://msdn.microsoft.com/en-us/commandline/wsl/faq)
5. [Get Mongodb Running](https://github.com/Microsoft/BashOnWindows/issues/796#issuecomment-238048520)
6. [Install Nodejs on Bash for Windows](https://aigeec.com/installing-node-js-on-windows-10-bash/)
7. [Get Webpack running on Bash for Windows](https://github.com/Microsoft/BashOnWindows/issues/468)

## Also note there are tons of problems getting webpack and webpack watch to work. Looking into [virtualization and building via docker](https://medium.com/@andyccs/webpack-and-docker-for-development-and-deployment-ae0e73243db4#.7iqk98om2)