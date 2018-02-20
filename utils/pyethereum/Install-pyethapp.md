# Extended pyethapp deployment instructions

Using as reference https://github.com/ethereum/pyethapp

## Ubuntu

Installing base libraries

```
sudo apt-get install virtualenv virtualenvwrapper
sudo apt-get install build-essential automake pkg-config libtool libffi-dev libgmp-dev python-dev
```

Loading virtual env wrapper configuration
```
source /usr/share/virtualenvwrapper/virtualenvwrapper.sh
```

Create pyethapp virtualenv

```
mkvirtualenv pyethapp
```

Checking we are using the pyethapp env
```
workon
```

Installing the pyethapp library, default version (1.5.0) failed in my case. Digging into forums last version recommended is 1.5.1a0
```
pip install pyethapp==1.5.1a0
```

Creating new account
```
pyethapp account new
```

Private key is in ~/.config/pyethapp/keystore

Joining the network
``
pyethapp run
```

Instructions about how to run the application can be found on https://github.com/ethereum/pyethapp/wiki/The_Console
