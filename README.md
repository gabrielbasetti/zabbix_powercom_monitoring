# Zabbix Template for monitoring Powercom UPS throught UPSMON PRO Web
Complete solution to monitoring Powecom UPS device through the UPSMON PRO WEB

# Contact Info:
Created by Ilias Aidar - 23/05/2020
E-Mail: ilias@ilianapro.com
Telegram: @iSmartyPro 
OS: Windows

# Description:

To work this solution you have to install on Windows Host - UPSMON PRO 2.4 Appliction.

Zabbix template will grab data from UPSMON PRO WEB and store data in Zabbix.

# Items:
* Input, V
* Output, V
* Frequency, Hz
* Load, %
* Battery Level, %
* Temperatue, C

# Triggers:
* Battery is less than 50%;
* Battery is less than 20%;
* Input is less than 220V;
* Input is less than 200V;
* Input is less than 180V;
* Output is less than 200V;
* Temperature more than 30C;
* Temperature more than 35C.
