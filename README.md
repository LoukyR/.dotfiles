# dotfiles repo

The different config files that help be get up and running.


## Atlassian suggestion

https://www.atlassian.com/git/tutorials/dotfiles

https://news.ycombinator.com/item?id=11071754

## Toubleshooting slow boot time

Literally just check this:
```
sudo systemd-analyze blame
``` 

Will output how long services take to boot.

Used this source https://askubuntu.com/questions/1217252/boot-process-hangs-at-systemd-networkd-wait-online
Remove this service that should (as per source) only be enabled on server platform. 
```
systemctl disable systemd-networkd.service
```
