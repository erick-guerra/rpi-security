# rpi-sec to do list

Finish installation script

Adjust camera settings if dark

Fix white balance

Measure and tweak power consumption:
  - Lower CPU speed?
  - Enable iwconfig power management?

Handle file open errors (camera photos and config file)

Use jesse lite distro?

Take photo then check for MACs, then delete if required.

Implement some form of LED status

Add init script

Change import order to stop delay when doing first start. Import scapy and slow modules inside functions.

Use a pushbullet channel?


A separate thread does photo processing:
  - monitor photo list
  - if new photo, then check for MACs
  - if no macs, then send notification and archive photo
  - continue to check for MACs at a higher frequency
  - continue to process photos as they come
  - rate limit notifications?
  - clean up old photos?

~~Log message on alarm state transition~~

~~Have debug mode or to syslog mode.~~

~~Disable alarm by sending push from phone~~

~~Tidy logging to show which thread is logging~~

~~use scan_interval from config file if there~~

~~Remove _ping_ip and _find_mac_in_arp_table~~