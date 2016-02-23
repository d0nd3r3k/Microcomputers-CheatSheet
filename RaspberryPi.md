## RaspberryPi - Raspbian Configuration
---

### Install Node.js from source

```
sudo mkdir /opt/node
```

```
wget http://nodejs.org/dist/v0.10.2/node-v0.10.2-linux-arm-pi.tar.gz
tar xvzf node-v0.10.2-linux-arm-pi.tar.gz
sudo cp -r node-v0.10.2-linux-arm-pi/* /opt/node
```

add Node.js to your PATH env-variable:

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

### Install Node.js with apt-get

```
apt-get install nodejs
```

Note: this will most likely install an earlier version of Node.js on the rPi.

### Update Node.js using [n](https://github.com/tj/n)

```
sudo npm cache clean -f
sudo npm install -g n
sudo n stable
```

```
node -v
```

[source](http://web.archive.org/web/20150604015623/http://davidwalsh.name/upgrade-nodejs)












