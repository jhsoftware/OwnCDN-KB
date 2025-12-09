---
category: 1
refs: 8
---
# How to back up OwnCDN

You can always shut down OwnCDN and make a full copy of all the files in the [data folder](/kb/8). This can be restored directly on a new setup of OwnCDN if needed.

The `.db` files are SQLite databases, which can also be backed up "live" (without shutting down OwnCDN), using SQLite utilities.

## Configuration data

The full OwnCDN configuration is stored in the
`OwnCDN.config.json` file in the [data folder](/kb/8).

If you only want to back up the configuration (and not the data), just make a copy of this file.

## Storage service data

The best way to back up data in OwnCDN [Storage services](https://owncdn.com/docs/storage-service-type) is through the built-in live replication to another remote OwnCDN instance.

## File system service

Data served by OwnCDN [File system services](https://owncdn.com/docs/file-system-service-type) needs to backed up in the same way you would any other files - using your normal back up software and procedures.

## Other service types

The data stored by other service types is generally cached data with some other primary storage location. So the backing up these should not be critical (depending on your usage).


