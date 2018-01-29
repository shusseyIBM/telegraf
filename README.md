# Telegraph only to remote Influxdb

Home project to monitor different devices

## Quick Start

To start the container the first time launch:

```sh
docker run -d \
  --name telegraf \
  -p 22022:22 \
  -p 8125:8125/udp \
  shussey/telegraf:latest
```

You can replace `latest` with the desired version listed in changelog file.

To stop the container launch:

```sh
docker stop telegraf
```

To start the container again launch:

```sh
docker start telegraf
```

## Mapped Ports

```
Host		Container		Service

22022		22				sshd
```
## SSH

```sh
ssh root@localhost -p 22022
```
Password: root

