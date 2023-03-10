# Zabbix-Aruba-CX
Aruba CX series monitoring template for Zabbix

Refer to Zabbix forum for discussion and other updates: https://www.zabbix.com/forum/zabbix-cookbook/446449-aruba-cx-template

Modification of Zabbix 6.0.4 built-in template HP Enterprise Switch SNMP.

Includes the following changes:
1. corrects temperature reading
2. gathers firmware release
3. gathers serial number
4. gathers CPU utilization

Known bugs and limitations:

1. CX series switches have multiple CPU cores, the CPU utilization gathers CPU 0 only
2. Firmware release is the currently running firmware, which may not be the firmware saved in the primary or secondary flash.

Tested/developed only on 6100. 

How to use:
1. Within zabbix, go to Configuration -> templates
2. Import template
3. Apply template to switches like any other

Revision 2 from Michael Webber includes better fan/power discovery and developed under 6.2

see https://www.zabbix.com/forum/zabbix-cookbook/446449-aruba-cx-template?p=449659#post449659

Jeff hacked a bit to support uploading to a 6.0 version system
