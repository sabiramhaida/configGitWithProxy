# How to config git with proxy
## Introduction 
This readme if you need to configure git to use proxy

### Show current configuration

To see the current configuration of all `http` sections

```
git config --global --get-regexp http.*
```

If you are in a locally cloned repository folder then you drop 
the `--global` and see all current config:

```
git config --get-regexp http.*
```

### Configure the proxy 

You can configure in your user `~/.gitconfig` file using the `--global` switch, or local to a repository in its `.git/config` file.

#### Setting a global proxy

Configure a global proxy if all access to all repos require this proxy

```
git config --global http.proxy http://proxyUsername:proxyPassword@proxy.server.com:port
```

