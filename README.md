# macos atom python
## References
* https://brew.sh
* https://atom.io
* https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup

## Brew
### Install
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Git
### Install
```
brew install git
```
### Configure
```
git config --list --show-origin
```
```
git config --global user.name "Mona Lisa"
```
```
git config --global user.email mona@lisa.tld
```
```
git config --global init.defaultBranch main
```

## Python3
### Install
```
brew install python
```
### Configure
#### pip
```
python3 -m pip install --upgrade pip
```
#### setuptools
```
python3 -m pip install --upgrade setuptools
```

## Atom
### Install
### Configure
#### Script
```
apm install script
```
#### Terminal
```
apm install platformio-ide-terminal
```
