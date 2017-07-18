## Synopsis

This is a splunk app that contains the volume definitions for splunk data volumes. 

## Code Example

Volume definitions stored in the ../local/indexes.conf file 

```

# One Volume for Hot and Cold
[volume:primary]
path = /data/primary
maxVolumeDataSizeMB = 5000000

#
# This could be your cold storage volume
[volume:secondary]
path = /data/secondary
maxVolumeDataSizeMB = 5000000
```

## Motivation

This app allows the splunk administrator to manage all data volumes in one location.

## Installation

This app should be placed in /opt/splunk/etc/apps (or wherever $SPLUNK_HOME is) and modified accordingly for volume/disk size.