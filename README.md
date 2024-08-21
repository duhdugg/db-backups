# db-backups

🚧 Work In Progress 🚧

## Dependencies

- borg
- fuzzel (optional, for wayland desktop gui)
- fzf (for cli)
- postgres commands:
    * createdb
    * pg_dump
    * pg_restore
    * psql
- zstd

## Initialize the borg repo

```bash
BACKUP_DIR="/usr/local/bak/db-backups"
sudo mkdir -p $BACKUP_DIR
sudo chown $USER $BACKUP_DIR
borg init -e none $BACKUP_DIR
```
