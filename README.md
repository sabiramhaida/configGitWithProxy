# How to config git with proxy
## Introduction 
This readme if you need to configure git to use a proxy

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
