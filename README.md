# macos atom python
## References
* https://brew.sh
* https://atom.io
* https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup
* https://stackoverflow.com/questions/52522565/git-is-not-working-after-macos-update-xcrun-error-invalid-active-developer-pa

## macOS
### Install
* System Preferences > Software Update
  * Install macOS Monterey 12.0.1
### Configure
```
xcode-select --install
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
git config --global user.name "Mona Lisa"
git config --global user.email mona@lisa.tld
git config --global init.defaultBranch main
```

## Python3
### Install
```
brew install pyenv
pyenv install -1
pyenv install 3.10.0
```
### Configure
#### pyenv
```
pyenv global 3.10.0
pyenv version
cat ~/.zshrc
echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.zshrc
cat ~/.zshrc
PATH=$(pyenv root)/shims:$PATH
python --version
echo 'PATH=$(pyenv root)/shims:$PATH' >> ~/.zshrc
python --version
which python
```
#### pip
```
python3 -m pip install --upgrade pip
```
#### setuptools
```
python3 -m pip install --upgrade setuptools
```
## Code
### Create repo
```
mkdir -p ~/Projects/git/hub/bachmeb/macos-atom-python
cd $_
pwd
git init
```
### Add project to Atom
* File > Add Project Folder
  *  ~/Projects/git/hub/bachmeb/macos-atom-python

### Create python code
* Select project name > a
  * ./hello.py
```
print('hello')
```
### Run python in script window
* Packages > Script > Run Script
> ```
> hello
> [Finished in 0.43s]
### Run python code in Terminal
```
python hello.py
```
> ```
> hello
