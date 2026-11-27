# Backup and restore

A backup is a snapshot of the database file, not server sync. Everything runs
locally.

## Create a backup

1. Open **Settings**, then **Backup & Restore**.
2. Tap **Create backup**.
3. Choose a location in the system file dialog.
4. Wait for the success message.

The backup uses `VACUUM INTO`, so the resulting file is consistent even while
the database is in use. Do not copy the open database file by hand.

## Restore a backup

1. Open **Backup & Restore**.
2. Tap **Restore from file**.
3. Pick a `.sqlite` backup file.
4. Confirm.

What the app does:

1. Reads the file into a temporary folder.
2. Validates the SQLite content, integrity, and schema version.
3. Creates a safety snapshot of the current database.
4. Closes the database and replaces it with the backup file.
5. Removes sidecar files, opens the database, and runs migrations.
6. Reloads the data providers.

If restore fails after the replacement, the app restores the safety snapshot.
Files that are not AturMyDuit backups, or have a newer schema, are rejected.

## Backup history

The Backup page shows successful and failed attempts. Use this history to
confirm that the latest backup was actually created.

## Recommendations

- Back up regularly, for example at the end of every month.
- Keep a copy in another storage location, not only on the phone.
- Use a name you can recognize. The app uses the pattern
  `aturmyduit-backup-YYYYMMDD-HHmmss.sqlite`.
- Never upload a backup to a public issue. It contains all your financial data.
- Backups are not encrypted yet. Store them somewhere safe.
