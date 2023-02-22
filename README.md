-# gitworkflow.github.io
-Git team Workflow lab for NXP



### Git Configuration

Install Git VCS tools

	sudo apt-get install vim git
	sudo apt-get install vim git

Configure User name and email address

	git config --global user.name "User Name"
	git config --global user.email "user.email@nxp.com"

Personalize preferred text editor

	git config --global core.editor vim
	git config --global color.ui true
	git config --global push.default upstream
	git config --global merge.conflictstyle diff3





### Git aliases (Optional)

Feature that can make your Git experience simpler, easier, and more familiar

	git config --global alias.s "status -s"
	git config --global alias.l "log --oneline"
	git config --global alias.lp "log -p"
	git config --global alias.hreset "reset HEAD"
	git config --global alias.tree "log --oneline --decorate --all --graph"
	git config --global alias.d "diff"
	git config --global alias.a "add"
	git config --global alias.uncommit "reset HEAD^"
	git config --global alias.rst "git reset --hard"
	git config --global alias.last 'log -1 HEAD'

Reference: https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases





### Git Workflow

Fork a template project

	git clone <repo>
	git checkout -b <local_branch> <remote_working_branch>

repo: git@github.com:malonso1/gitworkflow.git

remote branch: main



Personalize Git

	cd <repo>
	cp -v git/git-completion.bash ~/.git-completion.bash
	cp -v git/git-prompt.sh ~/.git-prompt.sh
	cat -v git/bash_profile >> ~/.bashrc
	cd ~
	bash

