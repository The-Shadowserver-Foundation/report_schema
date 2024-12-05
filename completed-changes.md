## Completed changes

### The following schema changes were completed on Dec 5 2024:

* Revised 'http_agent' to be 'extra.http_agent' in the event_honeypot_http_scan, sandbox_url, and scan_sip reports.
* Added the scan_msrpc report.


### The following schema change was completed on Sep 24 2024:

* Added compromised_iot and compromised_iot6 reports.


### The following schema change was completed on July 29 2024:

*  Normalized the 'date' field in the scan_cwmp and scan6_cwmp reports to 'http_date'.


### The following schema changes were completed on June 14 2024:

IntelMQ 2024-06-14T14:44:58Z

* Added machine_name to the event4_microsoft_sinkhole_http, event6_microsoft_sinkhole_http, event4_sinkhole_http, and event6_sinkhole_http reports.
* Added hassh to the scan_ssh and scan6_ssh reports.
* Added first_seen_time, last_seen_time, and potential_exposure_time to the special report.


### The following schema changes were completed on Mar 20 2024:

IntelMQ 2024-03-20T21:53:18Z

* Added the scan_loop_dos report.


### The following schema changes were completed on February 8 2024:

IntelMQ 2024-02-08T15:10:57Z

* Added the 'extra.cve' field to the scan_http_vulnerable and scan6_http_vulnerable reports.


### The following schema changes were completed on February 6 2024:

IntelMQ 2024-02-06T15:00:11Z

* The 'classification.identifier' has been updated to describe the incident for the compromised_website6, population6_bgp, population6_msmq, population_bgp, population_msmq, scan6_activemq, scan6_bgp, scan6_cwmp, scan6_elasticsearch, scan6_ipp, scan6_mqtt, scan6_mqtt_anon, scan6_mysql, scan6_postgres, scan6_rdp, scan6_slp, scan6_smb, scan6_smtp, scan6_smtp_vulnerable, scan6_snmp, scan6_ssh, scan6_ssl, scan6_ssl_freak, scan6_ssl_poodle, scan6_stun, scan6_telnet, scan6_vnc, event_honeypot_ics_scan, and scan_http_vulnerable reports.
* The 'classification.taxonomy' and 'classification.type' have been changed to vulnerable/vulnerable-system for the population6_bgp, population_bgp, population6_msmq, population_msmq, scan6_mysql, scan_mysql, scan6_postgres, scan_postgres, scan_couchdb, scan_epmd reports.


### The following schema changes were completed on January 29 2024:

IntelMQ  2024-01-29T17:25:47Z

* The 'malware.name' is now mapped to 'infection' for the event4_microsoft_sinkhole, event4_microsoft_sinkhole_http, event6_sinkhole, event6_sinkhole_http, event6_sinkhole_http_referer, event_sinkhole, event_sinkole_dns, event_sinkhole_http, and event_sinkhole_http_referer reports.
* The 'classification.identifier' is now mapped to 'infection' for the event4_microsoft_sinkhole_http, event6_sinkhole_http, event6_sinkhole_http_referer, event_sinkhole_http, and event_sinkhole_http_referer reports.
* The 'classification.taxonomy', 'classification.type', and 'protocol.application' were changed for the event6_sinkhole_http_referer and event_sinkhole_http_referer reports.


### The following schema changes were completed on December 17 2023:

IntelMQ  2023-12-17T17:35:41Z

* Added scan_post_exploitation_framework report.


### The following IntelMQ changes were completed on December 12 2023:

IntelMQ  2023-12-12T16:26:32Z

* Corrected 'source.fqdn' from 'destination.fqdn' in sandbox_conn and sandbox_url reports.
* Added 'tag' to scan_vnc and scan_hadoop reports.


### The following schema changes were completed on November 25 2023:

IntelMQ  2023-11-22T00:13:50Z 

* The `severity` field will be added to all reports.

* The `hostname_source` field will be added to all scan and population reports.

---

### The following schema changes were completed on November 18 2023:

IntelMQ  2023-11-16T17:31:58Z 

| report | change |
| --- | --- |
| * all * |remove: sic
|sandbox_connection|remove: host; add: city, hostname, naics, sector, region, sha1, sha256
|sandbox_dns| remove: md5hash, type; add: md5, request_type, sha1, sha256
|sandbox_url| remove: host; add: city, hostname, naics, port, region, sector, ssha1, sha256
|scan_chargen| remove: size (already has response_size)
|scan_db2| remove: size; add: response_size
|scan_ldap| remove: size; add: response_size
|scan_ntpmonitor| remove: size; add: response_size
|scan_rdp| remove: bluekeep_vulnerable, cve20190708_vulnerable (replaced with tag)
|scan_sip| add: naics, sector
|scan_smb| remove: smb_implant, smbv1_support (replaced with tag)
|scan_tftp| remove: size; add: response_size
|scan_ubiquiti| remove: size; add: response_size
|scan_xdmcp| remove: size; add: response_size
|url_malware| remove: host; add: hostname
|url_spam| remove: host, md5; add: hostname, port

---


  
