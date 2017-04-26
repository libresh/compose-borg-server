# borg-server

A borg server for libre.sh.

## Getting started

```
cd /system
git clone https://github.com/indiehosters/borg-server borg-servername
cd borg-servername
vi docker-compose.yml #replace things between XX
vi authorized_keys_example #add your ssh public key
mv authorized_keys_example authorized_keys
libre enable
libre start
```
