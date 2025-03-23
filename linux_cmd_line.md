# Installation
- `apt install` <package_name>
- `apt install` <package.deb>





## Keyrings

## sources list

## http tools


## Shell settings

- Configuring the commandline `PS` variable with `git` branch. Copy paste the code below to `.bashrc`
  ```
  parse_git_branch() {
    git branch 2>/dev/null | grep '*' | sed 's/* / (/;s/$/)/'
  }

  export PS1="\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\W\[\033[01;33m\]\$(parse_git_branch)\[\033[00m\]\$ "
  ```
