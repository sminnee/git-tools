# git-tools

This repository is a collection of extensions to git that I find useful.  You're welcome to submit your own via pull requests:

 * `git pull-all`: Pulls all branches from their remotes, whether you have them currently checked out or now.
 * `git feature list-unmerged`: List remote branches that haven't yet been merged back to origin/master.

## Installation

I like to keep stuff from Github in ~/Projects, so this is how I'd install it:

	cd ~/Projects
	git clone https://github.com/sminnee/git-tools.git
	cd git-tools
	sudo ./install /usr/local/bin
	
The install command will create symlinks in /usr/local/bin, rather than copying files, to make upgrading easier.

## Upgrade

Since the installation is done with symlinks, any changes to your checkout will be immediately available:

	cd ~/Projects/git-tools
	git pull
