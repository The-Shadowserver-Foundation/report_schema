## Completed changes

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


  
