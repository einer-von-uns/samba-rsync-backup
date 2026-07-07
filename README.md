# Samba rsync Backup

Automatisiertes rsync Backup-Skript von Ubuntu zu Rocky Linux.

## Architektur
* **Quelle (Ubuntu Samba):** `10.10.10.17` -> `/home/beute/`
* **Ziel (Rocky Linux VM):** `10.10.10.25` -> `/home/beute/` (User: `rockvm`)

## Autopilot
Das Skript `backup.beute` wird jede Nacht um 02:00 Uhr via Cronjob ausgeführt.
