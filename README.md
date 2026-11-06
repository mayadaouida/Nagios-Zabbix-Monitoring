\# Nagios and Zabbix Monitoring Project



\## Project Overview

This project demonstrates the implementation of an infrastructure monitoring environment using \*\*Nagios Core\*\* and \*\*Zabbix\*\* on Ubuntu 22.04 virtual machines.



The environment was deployed using \*\*Vagrant\*\* and \*\*Oracle VirtualBox\*\*.



\## Project Objectives

\- Monitor host availability and service status.

\- Monitor Linux system resources.

\- Configure remote monitoring between monitoring and target hosts.

\- Validate monitoring results through both web interfaces.



\## Technologies Used

\- Ubuntu 22.04 LTS

\- Vagrant

\- Oracle VirtualBox

\- Nagios Core 4.5.9

\- NRPE 4.0.3

\- Zabbix 7.0

\- MariaDB

\- Apache Web Server



\## Infrastructure



| Machine | IP Address | Role |

|---|---|---|

| monitor01 | 192.168.56.17 | Nagios and Zabbix monitoring server |

| web01 | 192.168.56.11 | Remote Linux host monitored by Nagios |



\## Nagios Implementation

\- Installed and configured Nagios Core.

\- Configured host and service monitoring.

\- Monitored local services and system resources.

\- Configured NRPE on the remote host.

\- Verified remote NRPE connectivity.

\- Confirmed that the remote host and CPU Load service were reporting correctly.



\## Zabbix Implementation

\- Installed Zabbix Server, Frontend, Agent, and MariaDB.

\- Configured the Zabbix database and frontend.

\- Added `monitor01` as a monitored host.

\- Linked the \*\*Linux by Zabbix agent\*\* template.

\- Verified agent connectivity and collected monitoring data.



\## Validation

The implementation was tested using:

\- Nagios web interface and service status.

\- NRPE connectivity test.

\- Zabbix agent connectivity using `zabbix\_get`.

\- Zabbix Latest Data to verify collected metrics.



\## Screenshots



\### Nagios Services

!\[Nagios Services](Screenshots/Nagios-Services.jpeg)



\### Zabbix Latest Data

!\[Zabbix Latest Data](Screenshots/Zabbix-Latest-Data.jpeg)



\## Repository Structure

```text

Nagios-Zabbix-Monitoring/

├── README.md

├── Vagrantfile

├── .gitignore

├── Screenshots/

│   ├── Nagios-Services.jpeg

│   └── Zabbix-Latest-Data.jpeg

├── nagios/

└── zabbix/

```



\## Conclusion

This project demonstrates the deployment of two monitoring solutions and the configuration of local and remote Linux host monitoring. Both Nagios and Zabbix were successfully tested through their respective interfaces.

