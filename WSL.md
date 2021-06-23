# WSL

## Install WSL
May require Windows Insider build from Dev stream eg. 21390

    wsl --install

## Setup WSL

### Cache cleanup alias

## Setup IDEs

### Install **Intellij**
```
cd ~/
export jb_version=2021.1.2
mkdir -p downloads && cd downloads
wget https://download-cdn.jetbrains.com/idea/ideaIU-$jb_version.tar.gz -O intellij.tar.gz
sudo mkdir -p /opt/intellij
sudo tar -xvzf intellij.tar.gz --strip-components=1 --show-transformed -C /opt/intellij
sudo echo "alias intellij=/opt/intellij/bin/idea.sh" >> ~/.bashrc && source ~/.bashrc
rm intellij.tar.gz
```

### Install **PyCharm**
```
cd ~/
export jb_version=2021.1.2
mkdir -p downloads && cd downloads
wget https://download.jetbrains.com/python/pycharm-professional-$jb_version.tar.gz -O pycharm.tar.gz
sudo mkdir -p /opt/pycharm
sudo tar -xvzf pycharm.tar.gz --strip-components=1 --show-transformed -C /opt/pycharm
sudo echo "alias pycharm=/opt/pycharm/bin/pycharm.sh" >> ~/.bashrc && source ~/.bashrc
rm pycharm.tar.gz
```
