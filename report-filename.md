## Report Filename Format

While we recommend using an integration utilizing the [API](https://github.com/The-Shadowserver-Foundation/api_utils/wiki/API:-Reports-Query#reportslist) to obtain reports, we understand that legacy import mechanisms do exist.

Report filenames contain the report date, report type, and a variable number of additional details based on the organization and filters used to generate the report.

### Examples:

1. `2015-01-01-dns_openresolver-sample-asn.csv`
2. `2020-04-03-scan_ics-sample-asn-delayed.csv`
3. `2024-07-04-dns_openresolver-123-sample-asn.csv`

---

### Sample regular expression 1:

This regex matches just the report type.

| expression | group | match 
| --- | --- | --- |
| `^\d{4}-\d{2}-\d{2}-([^-]+)-.+\.csv$  ` | 1 | report type | 

| example | group | match |
| --- | --- | --- | 
| `2015-01-01-dns_openresolver-sample-asn.csv` | 1 | `dns_openresolver` | 
| `2020-04-03-scan_ics-sample-asn-delayed.csv` | 1 | `scan_ics` | 
| `2024-07-04-dns_openresolver-123-sample-asn.csv` | 1 | `dns_openresolver` |

---

### Sample regular expression 2:

This regex matches the report date and type.

| expression | group | match |
| --- | --- | --- | 
| `^(\d{4}-\d{2}-\d{2})-([^-]+)-.+\.csv$` | 1 | report date | 
| | 2 | report type | 

| example | group | match |
| --- | --- | --- | 
| `2015-01-01-dns_openresolver-sample-asn.csv` | 1 | `2015-01-01`
|   | 2 | `dns_openresolver` | 
| `2020-04-03-scan_ics-sample-asn-delayed.csv` | 1 | `2022-04-03` |
|   | 2 | `scan_ics` | 
| `2024-07-04-dns_openresolver-123-sample-asn.csv` | 1 | `2025-07-04` |
|   | 2 | `dns_openresolver` |

---

### Sample regular expression 3:

This regex matches the report date, type, and identifier.

| expression | group | match |
| --- | --- | --- | 
| `^(\d{4}-\d{2}-\d{2})-([^-]+)-(.+)\.csv$` | 1 | report date | 
| | 2 | report type | 
| | 3 | report identifier |

| example | group | match |
| --- | --- | --- | 
| `2015-01-01-dns_openresolver-sample-asn.csv` | 1 | `2015-01-01` |
|   | 2 | `dns_openresolver` | 
|   | 3 | `sample-asn` |
| `2020-04-03-scan_ics-sample-asn-delayed.csv` | 1 | `2022-04-03` |
|   | 2 | `scan_ics` | 
|   | 3 | `sample-asn-delayed` |
| `2024-07-04-dns_openresolver-123-sample-asn.csv` | 1 | `2025-07-04` |
|   | 2 | `dns_openresolver` |
|   | 3 | `123-sample-asn` |
