# Master Clock Accuracy Monitor

Public mirror of a home ESP8266 that watches the hourly sync-contact pulse from a
Self Winding Clock Co. master clock and logs its offset from real (NTP) time.

- **Dashboard:** https://w1jgc.github.io/master-clock-monitor/
- **Raw data:** [`log.csv`](log.csv) — `utc_iso,offset_ms,pulse_ms` (positive offset = clock fast)

`log.csv` is refreshed roughly every 15 minutes by a cron job on my laptop that
pulls it from the device on my LAN and pushes here. The device itself is not
exposed to the internet. New data points only appear at the top of each hour.
