## Severity Levels

| Level | Description |
| -- | --- |
| critical | Highly critical vulnerabilities that are being actively exploited, where failure to remediate poses a very high likelihood of compromise. For example, a pre-auth RCE or modification or leakage of sensitive data.
| high | End of life systems, systems that you can log into with authentication that are meant to be internal (SMB, RDP), some data can be leaked. Sinkhole events end up in this category.
| medium | Risk that does not pose an immediate threat to the system but can over time escalate to a higher severity. For example, risk of participating in DDoS, unencrypted services requiring login, vulnerabilities requiring MITM to exploit, attacker will need to know internal systems/infrastructure in order to exploit it.
| low | Deviation from best practice - little to no practical way to exploit, but setup is not ideal. For example, SSL POODLE reports may end up in this category.
| info | Informational only. Typically no concerns. However, this category includes the Device Identification report, which may include information on device types that should not be accessible on the public Internet, in which case the individual events in the report may be assigned higher severity levels. Review in accordance with your security policy.

        
## Default Severity Level by Report Type

| Report | Subject | Level |
| ---    | ---     | ---   |
| blocklist | Block Listed IP Addresses | low |
| compromised_account | Compromised Account | critical |
| compromised_website | Compromised Website | critical |
| compromised_website6 | IPv6 Compromised Website | critical |
| device_id | Device Identification | info |
| device_id6 | IPv6 Device Identification | info |
| event4_ddos_participant | DDoS Participant | high |
| event4_honeypot_brute_force | Honeypot Brute Force Events | critical |
| event4_honeypot_darknet | Darknet Events | high |
| event4_honeypot_ddos | Honeypot DDoS Events | critical |
| event4_honeypot_ddos_amp | Honeypot DDoS Amplification Events | info |
| event4_honeypot_ddos_target | Honeypot DDoS Target Events | info |
| event4_honeypot_http_scan | Honeypot HTTP Scanner Events | high |
| event4_honeypot_ics_scan | Honeypot ICS Scanner Events | critical |
| event4_honeypot_rdp_scan | Honeypot RDP Scanner Events | high |
| event4_honeypot_smb_scan | Honeypot SMB Scanner Events | high |
| event4_ip_spoofer | IP Spoofer Events | medium |
| event4_microsoft_sinkhole | Microsoft Sinkhole events | critical |
| event4_microsoft_sinkhole_http | Microsoft Sinkhole HTTP Events | critical |
| event4_sinkhole | Sinkhole Events | critical |
| event4_sinkhole_dns | Sinkhole DNS Events | info |
| event4_sinkhole_http | Sinkhole HTTP Events | critical |
| event4_sinkhole_http_referer | Sinkhole HTTP Referer Events | critical |
| event6_sinkhole | IPv6 Sinkhole Events | critical |
| event6_sinkhole_http | IPv6 Sinkhole HTTP Events | critical |
| event6_sinkhole_http_referer | IPv6 Sinkhole HTTP Referer Events | critical |
| malware_url | Malware URL | critical |
| population6_bgp | IPv6 Accessible BGP | medium |
| population6_http_proxy | IPv6 Accessible HTTP Proxy | low |
| population6_msmq | IPv6 Accessible MSMQ Service | medium |
| population_bgp | Accessible BGP | medium |
| population_http_proxy | Accessible HTTP Proxy | low |
| population_msmq | Accessible MSMQ Service | medium |
| sandbox_conn | Sandbox Connections | low |
| sandbox_url | Sandbox URL | low |
| scan6_activemq | IPv6 Accessible ActiveMQ Service | medium |
| scan6_bgp | IPv6 Open BGP | high |
| scan6_cwmp | IPv6 Accessible CWMP | medium |
| scan6_dns | IPv6 DNS Open Resolvers | medium |
| scan6_elasticsearch | IPv6 Open Elasticsearch Server | low |
| scan6_exchange | IPv6 Vulnerable Exchange Server | critical |
| scan6_ftp | IPv6 Accessible FTP Service | medium |
| scan6_http | IPv6 Accessible HTTP | info |
| scan6_http_proxy | IPv6 Open HTTP Proxy | medium |
| scan6_http_vulnerable | IPv6 Vulnerable HTTP | critical |
| scan6_ipp | IPv6 Open IPP | high |
| scan6_isakmp | IPv6 Vulnerable ISAKMP | low |
| scan6_ldap_tcp | IPv6 Open LDAP (TCP) Services | high |
| scan6_mqtt | IPv6 Open MQTT | medium |
| scan6_mqtt_anon | IPv6 Open Anonymous MQTT | high |
| scan6_mysql | IPv6 Accessible MySQL Server | high |
| scan6_ntp | IPv6 NTP Version | medium |
| scan6_ntpmonitor | IPv6 NTP Monitor | medium |
| scan6_postgres | IPv6 Accessible PostgreSQL Server | high |
| scan6_rdp | IPv6 Accessible RDP Report | high |
| scan6_slp | IPv6 Accessible SLP Service | high |
| scan6_smb | IPv6 Accessible SMB Service | high |
| scan6_smtp | IPv6 Accessible SMTP | info |
| scan6_smtp_vulnerable | IPv6 Vulnerable SMTP | critical |
| scan6_snmp | IPv6 Open SNMP | high |
| scan6_ssh | IPv6 Accessible SSH | low |
| scan6_ssl | IPv6 Accessible SSL | info |
| scan6_ssl_freak | IPv6 SSL/Freak Vulnerable Servers | low |
| scan6_ssl_poodle | IPv6 SSLv3/Poodle Vulnerable Servers | low |
| scan6_stun | IPv6 Accessible Session Traversal Utilities for NAT | medium |
| scan6_telnet | IPv6 Accessible Telnet Service | medium |
| scan6_vnc | IPv6 Accessible VNC Service | high |
| scan_activemq | Accessible ActiveMQ Service | medium |
| scan_adb | Accessible Android Debug Bridge | critical |
| scan_afp | Accessible Apple Filing Protocol | high |
| scan_amqp | Accessible AMQP | medium |
| scan_ard | Accessible Apple Remote Desktop | high |
| scan_bgp | Open BGP | high |
| scan_chargen | Open Chargen | medium |
| scan_cisco_smart_install | Accessible Cisco Smart Install | critical |
| scan_coap | Accessible CoAP | medium |
| scan_couchdb | Accessible CouchDB Server | high |
| scan_cwmp | Accessible CWMP | medium |
| scan_db2 | Open DB2 Discovery Service | high |
| scan_ddos_middlebox | Vulnerable DDoS Middlebox | medium |
| scan_dns | DNS Open Resolvers | medium |
| scan_docker | Accessible Docker Service | critical |
| scan_dvr_dhcpdiscover | Accessible DVR DHCPDiscover | high |
| scan_elasticsearch | Open Elasticsearch Server | high |
| scan_epmd | Accessible Erlang Port Mapper Daemon | high |
| scan_exchange | Vulnerable Exchange Server | critical |
| scan_ftp | Accessible FTP Service | medium |
| scan_hadoop | Accessible Hadoop Service | high |
| scan_http | Accessible HTTP | info |
| scan_http_proxy | Open HTTP Proxy | medium |
| scan_http_vulnerable | Vulnerable HTTP | critical |
| scan_ics | Accessible ICS | high |
| scan_ipmi | Open IPMI Report | high |
| scan_ipp | Open IPP | high |
| scan_isakmp | Vulnerable ISAKMP | low |
| scan_kubernetes | Accessible Kubernetes API Server | high |
| scan_ldap_tcp | Open LDAP (TCP) Services | high |
| scan_ldap_udp | Open LDAP Services | high |
| scan_mdns | Open mDNS Report | medium |
| scan_memcached | Open Memcached Server | high |
| scan_mongodb | Open MongoDB Service | high |
| scan_mqtt | Open MQTT | medium |
| scan_mqtt_anon | Open Anonymous MQTT | high |
| scan_mssql | Open MS-SQL Server Resolution Service | high |
| scan_mysql | Accessible MySQL Server | high |
| scan_nat_pmp | Vulnerable NAT-PMP Systems | high |
| scan_netbios | Open Netbios | high |
| scan_netis_router | Netcore/Netis Router Vulnerability Scan | critical |
| scan_ntp | NTP Version | medium |
| scan_ntpmonitor | NTP Monitor | medium |
| scan_portmapper | Open Portmapper Scan | medium |
| scan_postgres | Accessible PostgreSQL Server | high |
| scan_qotd | Open QOTD | medium |
| scan_quic | Accessible QUIC Report | info |
| scan_radmin | Accessible Radmin | high |
| scan_rdp | Accessible RDP Report | high |
| scan_rdpeudp | Accessible MS-RDPEUDP | high |
| scan_redis | Open Redis Server | high |
| scan_rsync | Accessible Rsync Service | medium |
| scan_sip | Accessible SIP | high |
| scan_slp | Accessible SLP Service | high |
| scan_smb | Accessible SMB Service | high |
| scan_smtp | Accessible SMTP | info |
| scan_smtp_vulnerable | Vulnerable SMTP | critical |
| scan_snmp | Open SNMP | high |
| scan_socks | Accessible SOCKS4/5 Proxy | medium |
| scan_ssdp | Open SSDP | high |
| scan_ssh | Accessible SSH | low |
| scan_ssl | Accessible SSL | info |
| scan_ssl_freak | SSL/Freak Vulnerable Servers | low |
| scan_ssl_poodle | SSLv3/Poodle Vulnerable Servers | low |
| scan_stun | Accessible Session Traversal Utilities for NAT | medium |
| scan_synfulknock | SYNful Knock | critical |
| scan_telnet | Accessible Telnet Service | medium |
| scan_tftp | Open TFTP Servers | medium |
| scan_ubiquiti | Accessible Ubiquiti Discovery Service | high |
| scan_vnc | Accessible VNC Service | high |
| scan_ws_discovery | Accessible WS-Discovery Service | medium |
| scan_xdmcp | Accessible XDMCP Service | high |
| spam_url | Spam URL | low |
