# Intro

This repo has an example of a service to be run on a linux system under Raspberry Pi, it also works under Orange Pi and similar embedded platforms.

There are two important files in this repo:

* service.py
    -which contains ther service to be run.
* daemonize.sh
    -which allows to daemonize the service and make it start after system startup.

daemonize.sh should be copy into /etc/init.d/

## Service

Service.py is a normal python script with a loop that runs for ever.

## Install

With root privileges:

```sh
$ /etc/init.d/daemonize start
```
