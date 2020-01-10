# my hass to main hass bridge

1. zwave over mqtt
2. bluetooth over mqtt

## TODO
3. slimme meter over mqtt
4. More generic bluetooth bridge:
    - find a method to get it all instead of per item


## /boot/config.txt
add:
```
enable_uart=1
dtoverlay=pi3-miniuart-bt
core_freq=250
```

## How to enable SSH
- format usb drive with fat
- rename drive to "CONFIG"
- copy ssh pubkey to root of drive with the name authorized_keys
- insert usb (maybe reboot)
- ```ssh -i ~/.ssh/pubkey -p 22222 root@ip.of.raspberry```
