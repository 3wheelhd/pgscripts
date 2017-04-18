This directory contains scripts to accomplish postgresql backups.

Some knowledge of the postgresql backup process is assumed.

The backup script consists of two files:
	pg_backup.config - The main configuration file. This should be the only file which needs modifications.
	pg_backup.sh - The normal backup script which will go through each database and save a gzipped and/or a custom format copy of the backup into a date-based directory.

The location of the backups is configurable by changing the value of BACKUP_DIR in the pg_backup.config script.