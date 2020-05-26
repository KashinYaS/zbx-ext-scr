Scripts for Cisco devices:
- cisco_bgp_nei - get BGP neighbor IP and OID's suffix. Use this as LLD key "cisco_bgp_nei["{HOST.CONN}","{IPADDRESS}","{$SNMP_COMMUNITY}"]" {#VALUE} is a IPv4 BGP neighbor's IP, and {#INDEX} is a suffix suitable for OID and Key fields
- cisco_nexus_zone_count - get VSAN with ID=$4 zone count. Useful to keep VSAN's symmetry. For VSAN 10 Zabbix item will be cisco_nexus_zone_count["{HOST.CONN}","{IPADDRESS}","{$SNMP_COMMUNITY}","10"]
- cisco_asa_local_ip_count - count local IP addresses that match regexp $4. May be used to monitor Local IP pool exhaust.
