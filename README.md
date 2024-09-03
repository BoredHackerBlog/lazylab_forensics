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
- Memory dumps were collected after the systems were ransomed
- Systems were shutdown and rebooted before KAPE collection and artifact collection happened
- Systems were shutdown and rebooted again before raw evtx files were collected
