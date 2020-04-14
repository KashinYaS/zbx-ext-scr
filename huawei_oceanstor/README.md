hw_os_alarms - number of Alarms on a specific Huawei OceanStor 5500 or Dorado system except Storage pool out of space alarms.

hw_os_enclosuredisks - number of Bad disks in a specific Huawei OceanStor 5500 or Dorado enclosure.
Still works toooo long, usually near 3 seconds. Zabbix does not like such a time comsuming scripts.

hw_os_single_disk - snmpget wrapper for getting hwInfoDiskHealthStatus. In case of failed snmpget returns failed(2) value.
Cause hw_os_enclosuredisks is still slow, use a workaround - single Zabbix item for each disk. Check it rarely, because it does not use bulk get and may produce hundreds od snmpget's.
