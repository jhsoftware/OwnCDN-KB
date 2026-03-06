---
Category: 1
---
# Can I run my own AWS S3 instance with OwnCDN ?

For the most commonly used S3 features - yes, you can basically turn your Windows computer into an S3 server.

OwnCDN does NOT implement the full S3 API (very extensive), but it does implement enough of it to work perfectly with a large number of applications that support "S3 compatible storage".

You can choose to use the "File System" service type to serve and add/update/remove files directly from the Windows file system.

Or, you can use the "Storage" service type to serve and add/update/remove files in a local database (SQLite), which provides the added benefits of live replication and versioning (enabling point-in-time restore).

