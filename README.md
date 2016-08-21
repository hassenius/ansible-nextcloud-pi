# Ansible-Nexcloud-Pi

Installs [Nextcloud](https://nextcloud.com/) v9 and nginx on a raspberry pi. 

WARNING: Does not secure anything; passwords are silly defaults (overridable, see [defaults](defaults/main.yml)) and nginx listens on HTTP only. DO NOT expose this raspberry pi to the public internet, or ensure securing it beforehand.

Tested with a Raspberry Pi 2 and a fresh [Raspbian](https://www.raspberrypi.org/downloads/raspbian/) install (release 2016-05-27-raspbian-jessie).

Recommended to set `nextcloud_trusted_host` to the IP or hostname of your raspberry pi. 

## TODO:

- allow for https
- set up let's encrypt
- make non-default users/passwords mandatory
- use binary, not git clone
- add meta and register on ansible galaxy
- show basic playbook / link to one-step nextcloud-in-a-box instructions
- make generic enough for ubuntu/debian systems, not just raspberry pi
- kitchen tests
- travis

## Credits

* Some code taken and adapted from [https://github.com/shibby/nextcloud-vagrant](https://github.com/shibby/nextcloud-vagrant)
* Inspiration from [this article](http://ifahrentholz.de/2016/install-nextcloud-on-raspberry/)

