git config --global user.email "bajpai.mahendra@gmail.com"
git config --global user.name "mahendra"
git config --global color.ui true
git config --global color.status auto
git config --global color.branch auto

#### --- Installation ---
    https://www.tutorialspoint.com/git/index.htm

	Command                     |    Description
--------------------------------|----------------------------
$	sudo apt-get install git	|	( Install )
$	git --version				|	( check version )
$	git config --list			|	( check configuration )


###  Show branch name in terminal ( paste below code at end of file /home/bajpai/.bashrc )
	parse_git_branch() {
	     git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
	}
	export PS1="\u@\h:\[\033[32m\]\w\[\033[33m\]\$(parse_git_branch)\[\033[00m\] $ "





