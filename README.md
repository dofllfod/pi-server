# Pi Server
Fast, headless setup for a Raspberry Pi server based on Ubuntu 20.04 LTS.

## Getting started

- Download the Raspberry Pi [image](https://ubuntu.com/download/raspberry-pi) for Ubuntu Server 20.04 LTS
- Flash the image to an sd-card, e.g. with [Etcher](https://www.balena.io/etcher/)
- Configure the file `user-data` with hostname, timezone, username, password and ssh-key
- After completion open the boot section on the sd-card and add the files `user-data` and `ssh`
- Insert the sd card and start the Pi; this may take some time as the system updates itself
- Access the Pi with `ssh -i <SSH_KEY> <USERNAME>@<HOSTNAME>`

## Notes 

- This setup only works with an ethernet connection
- WIFI can be configured with the file `network-config`
- This approach requires a reboot after the first start and is therefore incompatible with cloud-init