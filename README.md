# Raspberry Pi development notes

## Configuring wifi with Raspbian and Raspbian Lite

https://linuxhint.com/rasperberry_pi_wifi_wpa_supplicant/

- Create empty `ssh` file on root of SD card to enable SSH (username `pi` password `raspberry`).
- Create `wpa_supplicant.conf` file on root of SD card to add wifi:

```
country=US
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1

network={
ssid="YOUR_WIFI_SSID_NAME"
scan_ssid=1
psk="YOUR_WIFI_PASSWORD"
key_mgmt=WPA-PSK
}
```

## Hx711 load sensor (scale)

- tutorial: https://tutorials-raspberrypi.com/digital-raspberry-pi-scale-weight-sensor-hx711/
- 3d printable load cell mount: https://www.thingiverse.com/thing:2486831/comments
