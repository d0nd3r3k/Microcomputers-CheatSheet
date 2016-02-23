# RaspberryPi Raspbian Configuration
---

## Install NodeJs

```
sudo mkdir /opt/node
```

```
wget http://nodejs.org/dist/v0.10.2/node-v0.10.2-linux-arm-pi.tar.gz
tar xvzf node-v0.10.2-linux-arm-pi.tar.gz
sudo cp -r node-v0.10.2-linux-arm-pi/* /opt/node
```

add Node.JS to your path variable:

```
nano /etc/profile
```

Add the following lines:

```
NODE_JS_HOME="/opt/node"
PATH="$PATH:$NODE_JS_HOME/bin"
```
Before:
```
export PATH
...
```


















