# zabbix-yum
List available updates from yum in zabbix using zabbix-sender

Files come in two parts:
> Template - To be imported into Zabbix interface and then assigned to the machine you wish to monitor

> yum-updates.sh - To be run on the machine that you wish to monitor

# Template
The template contains the items for collecting the data and also triggers with differing warning types, dependant on the count of differing updates available.

# yum-update.sh
The script will run yum updates and collect the amounts of different updates available. Then uses the zabbix_sender to send the data to the server

# Pre-reqs
1. Zabbix 'ServerActive' Address
2. zabbix-sender installed
