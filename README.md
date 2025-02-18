# Startr

This project is part of a collection of projects and tools maintained by openco.

Development of these tools requires the use of git, a text editor (I recommend Code and when you are ready Vim).

All steps work best in a Debian based Linux distribution such as Ubuntu or Elementary OS.



## Setting up your Build Environment 

You will need to have git and the following packages installed. Installing things in Debian based systems is quick with a package manager. Open your terminal and enter the following two commands:

`sudo apt-get update` #This updates your package manager's directory of programs

`sudo apt-get install git git-flow zlib1g-dev` # This installs git, git-flow, and zlib1g-dev

> Note: the command `sudo` allows you to run a command as the `root` or Admin user. On linux systems the root user is a special user account used for system administration. The name root may have originated because root is the only user account with permission to modify the root directory of a Unix system. This directory was originally considered to be root's home directory, but the UNIX Filesystem Hierarchy Standard now recommends that root's home be at /root.



## Create your ssh key:

It's simpler to work with repos if you have your ssh key setup. 

```
username@username-computername:~$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/home/username/.ssh/id_rsa):                     
Created directory '/home/username/.ssh'.
Enter passphrase (empty for no passphrase): 
```

If you are not dealing with a high sercurity project and you trust your computer you can put no passphrase.

## find your public ssh key 

To show your ssh key use command  `cat /home/username/.ssh/id_rsa.pub`

## Keep your projects clean

Choose or make a directory for your local repos.

I recomend ~/Documents/Projects

## Clone this and other repos you are working on

Fork and Clone the folowing repos to your machine

* https://github.com/opencoca/lt2d_school
* https://github.com/opencoca/lt2d_school_admin
* https://github.com/opencoca/simpleweb
* https://github.com/opencoca/startr

> Note: our team uses master repos with submodules. If work on many projects with our team ask your supervisor if you're eligable for access to parent repos

To clone a repo to directory of your choosing by using the following command
`git clone git@github.com:username/project.git` (found by clicking dropdown on download)

## Some Basic Git Commands

'''cat .git/config
git pull
git status 
git diff
git add README.md 
git status
git commit
git config --global user.email "yourname@something.com"
git config --global user.name "YourName"
git commit
fg
git push'''


## USE PYENV and PIPENV

Pyenv lets you easily switch between multiple versions of Python. It's simple, unobtrusive, and follows the UNIX tradition of single-purpose tools that do one thing well. **Pipenv** is a tool that aims to bring the best of all packaging worlds (bundler, composer, npm, cargo, yarn, etc.) to the Python world. Pipenv and Pyenv work well together allowing you to work on projects that  have differing needs.

https://github.com/pyenv/pyenv-installer

### Pyenv Install:

```source-shell
$ curl https://pyenv.run | bash
```

`pyenv.run` redirects to the install script in this repository and the invocation above is equivalent to:

$ curl -L https://github.com/pyenv/pyenv-installer/raw/master/bin/pyenv-installer | bash

Restart your shell so the path changes take effect:

```
source-shell
$ exec $SHELL
```

You can now begin using pyenv.

> If you need, `export USE_GIT_URI` to use `git://` instead of `https://` for git clone.

### Pipenv Install:

Pipenv is primarily meant to provide users and developers of applications with an easy method to setup a working environment. 

Install pipenv using python's pip

`pip install --user pipenv`



# License
Copyright 2019–2021 12787326 Canada Inc.

Licensed under the AGPLv3: https://opensource.org/licenses/agpl-3.0
