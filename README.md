# Introduction

The project contains templates and pipelines related to Palo Alto NG firewall scenarios

## firewall.json

The template *firewall.json* creates a single Palo Alto NG firewall.

### Prerequisites

A storage account with a fileshare for bootstrapping the firewall must exist and contain the following folders: config, content, license, software.  A plugins folder is optional.

### Parameters

The following parameters are required:

|Name|Restricted|Value(s)|Default Value
|---------|---------|---------|---------|
|adminUsername|no||sfcadmin|
|bootstrapFileShare|no|||
|bootstrapStorageAccount|no|||
|environment|yes|prod,dev,sandbox|dev |
|fwName|no||null|
|location|yes|westus,westus2,westus3|westus3|
|paSku|yes|byol,bundle1,bundle2,vmseries-flex|byol|
|paVersion|yes|9.0.9,9.1.0,10.0.9,10.1.6,latest| |
|paOffer|yes|vmseries1,vmseries-flex|vmseries1|
|paVmSize|yes|Standard_DS3_v2,Standard_DS4_v2,Standard_DS5_v2|Standard_DS3_v2|
|subnetPrefix|no||null|

Parameters required at runtime

- adminPassword

---
