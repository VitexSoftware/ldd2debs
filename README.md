ldd2debs
========

Find packaging dependencies for binaries

```shell
ldd2debs /bin/bash
libc6
libtinfo6
```

Installation
------------

```shell
sudo apt install lsb-release wget apt-transport-https bzip2

sudo wget -O /usr/share/keyrings/vitexsoftware.gpg https://repo.vitexsoftware.cz/keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/vitexsoftware.gpg]  https://repo.vitexsoftware.cz  $(lsb_release -sc) main" | sudo tee /etc/apt/sources.list.d/vitexsoftware.list
sudo apt update

sudo apt install ldd2debs
        
```

(also Test/Example for https://github.com/VitexSoftware/BuildImages/)
