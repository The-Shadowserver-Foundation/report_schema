## Upcoming changes

**NOTE** 
  * *The CSV field order is not static.  Please utilize the CSV header for field order.*
    
---

### 2025-08-04 

The mapping of the 'source' field in the blocklist report which is currently mapped to 'extra.source' will be changed to 'extra.source_name'.

This change is necessary to avoid conflicts with the elasticsearch mapping of the 'extra.source' field where it is commonly an object instead of a string. 
