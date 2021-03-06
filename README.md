# Zabbix Iostat Monitoring
Zabbix 5.2+ template for monitor iostat output, alerts for high disk utilization and etc  
Test enviroment:  
* Ubuntu Server 20
* iostat 12.5.4
* jq-1.6

# Install
Only 2 dependencies needed to run this template:
* **sysstat**
* **jq**

You can install these tools from your system package manager, for example:  
  
Ubuntu:  
`apt install sysstat jq`   
CentOS:  
`yum install sysstat jq`  

I recommend using the latest sysstat package because old versions of iostat contain some bugs with JSON output  
If your system has sysstat older than 12.5.4, I suggest compiling sysstat from [source code](https://github.com/sysstat/sysstat) (with no extra options to make this template works)
