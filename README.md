# lazylab_forensics
lazylab was ransomed! this repo contains forensic artifacts.

LazyLab (https://github.com/BoredHackerBlog/lazylab) was ransomed.

This repo contains forensics artifacts.

Be careful with the files. This repo does contain actual malware and ransomware!!

Zip password: infected

Lab was ransomed on Aug 24th. 

## Lab setup

- DC - 192.168.200.11
- Workstation - 192.168.200.12
- Splunk - 192.168.200.10:8000

## Users
- mscott - Admin, DA
- jim - admin, admin on workstation1
- pam - admin, admin on workstation1
- dwight - admin on workstation1
- vagrant - default account on all machines. should be ignored. used for intial setup/deployment

## Evidence
- Splunk logs include sysmon logs - install splunk, extract the logs in default db folder.
- Memory dumps were collected after the systems were ransomed - UPDATE: Memory dumps can't be read by volatility for some reason. You can ignore them.
- Systems were shutdown and rebooted before KAPE collection and artifact collection happened
- Systems were shutdown and rebooted again before raw evtx files were collected


## Files
- dc1_artifacts.zip - malware, kape (parsed), and other artifacts from dc1
- workstation1_artifacts.zip - malware, kape (parsed), and other artifacts from workstation1
- dc1_logs.zip - evtx logs from dc1
- workstation1_logs.zip - evtx logs from workstation1
- splunk_logs_db.zip - splunk logs. install splunk (free) and add the files to default/db folder. (/defaultdb/db folder. i believe its under /var/lib/splunk maybe?)
- Memory dumps can be found here: https://github.com/BoredHackerBlog/lazylab_forensics/releases
