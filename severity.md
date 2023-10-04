# Severity

| Level | Description |
| -- | --- |
| critical | Highly critical vulnerabilities that are being actively exploited, where failure to remediate poses an very high likelyhood of compromise.
| high | End of life systems, internal systems that you can log into with authentication that are meant to be internal (SMB, RDP), some data can be leaked. Drone/sinkhole events end up in this category.
| medium | Risk of participating in DDoS, unencrypted services requiring login, vulnerabilities requiring MITM to exploit, attacker will need to know internal systems/infrastructure in order to exploit it.
| low | Deviation from best practice - little to no practical way to exploit, but setup is not ideal.
| info | Informational only. However, this category includes the Device Identification report, which may include information on device types that should not be accessible on the public Internet. Review in accordance with your security policy.
        
