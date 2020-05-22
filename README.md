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

# How to install and configure
1. Install Windows Application UPSMON Pro (you can find it in Windows folder or you can download it from official website);
2. Launch UPSMON PRO and enable Webserver;
3. Optional open port in firewall for UPSMON Pro Web, in my case I am opened 8000/tcp
4. On any host you can open following: URL - http://url_of_upsmonpro:8000/ups.txt, should be few lines with UPS params;
5. Install Zabbix Template from zabbix folder;
6. Assign Zabbix template to monitoring Host;
7. Add MACROS - {$URL} - in our case http://url_of_upsmonpro:8000/ups.txt
8. wait few minutes and you will get all data from UPSMON Pro to you Zabbix.

Have a nice usage!
