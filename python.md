# Python venv

## Installation

```
$ pip3 install virtualen
$ pip3 install virtualenvwrapper
```

edit .bashrc

```
# Virtualenvwrapper settings:

export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3
export WORKON_HOME=$HOME/.virtualenvs
export VIRTUALENVWRAPPER_VIRTUALENV=/home/jimc/.local/bin/virtualenv
source ~/.local/bin/virtualenvwrapper.sh
```

## Use

### create a virtual environment in Python3 and activate it immediately:

```
$ mkvirtualenv name_of_your_env
```

### deactivate the environment

```
$ deactivate
```

### To list all available virtual environments use the command workon or lsvirtualenv:

```
$ workon

$ lsvirtualenv
```

### To activate one specific environment use workon + name of your environment:

```
$ workon name_of_your_env
```

### Rmvirtualenv will remove a specific virtual environment located in your .virtualenv directory.

```
$ rmvirtualenv name_of_your_env
```

### Cpvirtualenv will copy the existing virtual environment to a new virtual environment and activate it.

```
$ cpvirtualenv old_virtual_env new_virtual_env
```
