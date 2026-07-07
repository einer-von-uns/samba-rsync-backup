# Samba rsync Backup

Automatisiertes rsync Backup-Skript von Ubuntu zu Rocky Linux.

## 🏴‍☠️ Die Mannschaft (Samba Users)
Alle Benutzer sind in der Linux-Gruppe `crew` organisiert und besitzen aus Sicherheitsgründen keinen SSH-Zugriff (`/sbin/nologin`).

* **marte5** (Kapt'n / Administrator)
* **amy** (Crew)
* **betty** (Crew)
* **bob** (Crew)
* **linda** (Crew)
* **tim** (Crew)

## 🗺️ Architektur
* **Quelle (Ubuntu Samba):** `10.10.10.17` -> `/home/beute/` (Eigentümer: `root:crew`, Rechte: `2770`)
* **Ziel (Rocky Linux VM):** `10.10.10.25` -> `/home/beute/` (User: `rockvm`)

## 🕒 Autopilot
Das Skript `backup.beute` wird jede Nacht um 02:00 Uhr via Cronjob ausgeführt.
