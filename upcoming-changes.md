## Upcoming changes

The following schema changes are planned for November 18 2023:

| report | change |
| --- | --- |
| * all * |remove: sic
|sandbox_connection|remove: host; add: city, hostname, naics, sector, region, sha1, sha256
|sandbox_dns| remove: md5hash, type; add: md5, request_type, sha1, sha256
|sandbox_url| remove: host; add: city, hostname, naics, port, region, sector, /'ssha1, sha256
|scan_chargen| remove: size (already has response_size)
|scan_db2| remove: size; add: response_size
|scan_ldap| remove: size; add: response_size
|scan_ntpmonitor| remove: size; add: response_size
|scan_rdp| remove: bluekeep_vulnerable, cve20190708_vulnerable (replaced with tag)
|scan_sip| add: naics, sector
|scan_smb| remove: smb_implant, smbv1_support (replaced with tag)
|scan_smtp| add: auth_ssl_response, auth_tls_response, cert_expiration_date, cert_expired, cert_issue_date, cert_length, cert_serial_number, cert_valid, cipher_suite, freak_cipher_suite, freak_vulnerable, handshake, issuer_business_category, issuer_common_name, issuer_country, issuer_email_address, issuer_given_name, issuer_locality_name, issuer_organization_name, issuer_organization_unit_name, issuer_postal_code, issuer_serial_number, issuer_state_or_province_name, issuer_street_address, issuer_surname, jarm, key_algorithm, md5_fingerprint, raw_cert, raw_cert_chain, self_signed, sha1_fingerprint, sha256_fingerprint, sha512_fingerprint, signature_algorithm, ssl_version, sslv3_supported, subject_business_category, subject_common_name, subject_country, subject_email_address, subject_given_name, subject_locality_name, subject_organization_name, subject_organization_unit_name, subject_postal_code, subject_serial_number, subject_state_or_province_name, subject_street_address, subject_surname, tlsv13_cipher, tlsv13_support, validation_level
|scan_tftp| remove: size; add: response_size
|scan_ubiquiti| remove: size; add: response_size
|scan_xdmcp| remove: size; add: response_size
|url_malware| remove: host; add: hostname
|url_spam| remove: host, md5; add: hostname, port

The following schema changes are planned for November 25 2023:

* The `severity` field will be added to all reports.

* The `hostname_source` field will be added to all scan and population reports.
  
