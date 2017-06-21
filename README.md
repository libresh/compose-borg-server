# borg-server

A borg server for libre.sh.

## Getting started

```
cd /system
git clone https://github.com/indiehosters/borg-server borg-servername
cd borg-servername
cp .env.sample .env
vi .env #add your ssh public key
libre start
libre enable
```

## List backups

```
docker-compose exec borg bash
cd /backups
borg list my_backup
```

## Restore a backup

```
docker-compose exec borg bash
mkdir destination
cd destination
borg extract /backups/my_backup::ARCHIVE
```
