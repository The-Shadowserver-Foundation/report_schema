## Report Filename Format

Report filenames contain the report date, report type, and a variable number of additional details based on the organization and filters used to generate the report.

### Examples:

1. `2015-01-01-dns_openresolver-sample-asn.csv`
2. `2020-04-03-scan_ics-sample-asn-delayed.csv`
3. `2024-07-04-dns_openresolver-123-sample-asn.csv`

---

### Sample regular expression 1:

| expression | group | match 
| --- | --- | --- |
| `^\d{4}-\d{2}-\d{2}-([^-]+)-.+\.csv$  ` | 1 | report type | 

| example | group | match |
| --- | --- | --- | 
| 1 | 1 | `dns_openresolver` | 
| 2 | 1 | `scan_ics` | 
| 3 | 1 | `dns_openresolver` |

---

### Sample regular expression 2:

| expression | group | match |
| --- | --- | --- | 
| `^(\d{4}-\d{2}-\d{2})-([^-]+)-.+\.csv$` | 1 | report date | 
| | 2 | report type | 

| example | group | match |
| --- | --- | --- | 
| 1 | 1 | `2015-01-01`
| 1 | 2 | `dns_openresolver` | 
| 2 | 1 | `2022-04-03` |
| 2 | 2 | `scan_ics` | 
| 3 | 1 | `2025-07-04` |
| 3 | 2 | `dns_openresolver` |
