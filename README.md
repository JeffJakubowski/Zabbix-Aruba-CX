# Zabbix-Aruba-CX
Aruba CX series monitoring template for Zabbix

Modification of Zabbix 6.0.4 built-in template HP Enterprise Switch SNMP.

Includes the following changes:
1. corrects temperature reading
2. gathers firmware release
3. gathers serial number
4. gathers CPU utilization

Known bugs and limitations:

1. CX series switches have multiple CPU cores, the CPU utilization gathers CPU 0 only
2. Firmware release is the currently running firmware, which may not be the firmware saved in the primary or secondary flash.
