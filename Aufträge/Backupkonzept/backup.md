# Mein Backup Konzept

## Inhaltsverzeichnis

- [Nextcloud](#nextcloud)
- [Andere Backup Möglichkeiten](#andere-backup-möglichkeiten)
    - [NAS (Network Attached Storage)](#nas)
    - [Macrium Reflect](#macrium-reflect)

## Nextcloud

Ich betreibe einen eigenen Server der auf Ubuntu läuft, diese besitzt über Drei 1TB SSD Platten die auf **RAID 5** laufen und somit im Fall eines Festplatten ausfalls die Daten wiederhergestellt werden können. Auf dem Server läuft eine **Nextcloud** Instanz der die Daten auf dem Server speichert und mit dem Internet synchronisiert. Die Daten werden auf dem Server verschlüsselt gespeichert und können nur mit dem richtigen Passwort entschlüsselt werden. Durch die ständige synchronisation der Daten auf dem Server und dem Internet sind die Daten immer auf dem neusten Stand und können von überall abgerufen werden. Die Daten sind wiederrum auf mehreren Geräten gespeichert und können auch beim Ausfall des Servers darauf zugegriffen werden.

*Links*: [Nextcloud](https://nextcloud.com/), [Ubuntu](https://ubuntu.com/)

![Nextcloud](https://upload.wikimedia.org/wikipedia/commons/thumb/6/60/Nextcloud_Logo.svg/1200px-Nextcloud_Logo.svg.png)

![Ubuntu](x_resources/ubuntu.png)

# Andere Backup Möglichkeiten

## NAS 

Ein **NAS Server** (eigener Server mit TrueNAS oder Fertigsysteme z.B von Synology) eignen sich auch sehr gut als eine Backup Möglichkeit. Sie lassen sich einfach als Netzwerklaufwerk einbinden und können somit auch als Speicherort für Backups verwendet werden. Durch erstellen von **RAID** Systemen bieten sie auch eine gewisse Sicherheit gegen Datenverlust.

- **NAS** = Network Attached Storage

![TrueNAS](https://pbs.twimg.com/profile_images/1445829681270251525/ykuR5Gtl_400x400.png)
- [TrueNAS](https://www.truenas.com/)

![Synology](x_resources/synology.png)

- [Synology](https://www.synology.com/de-de)

## Macrium Reflect

**Macrium Reflect** ist eine Backup Software. Sie bietet die Möglichkeit, Backups von ganzen Festplatten oder einzelnen Partitionen zu erstellen. Die Backups können auf einem externen Speichermedium oder auf einem Netzwerklaufwerk gespeichert werden. 

Folgende Möglichkeiten bietet Macrium Reflect:
- **Image Backup**: Erstellen eines Abbilds einer Festplatte oder Partition
- **File and Folder Backup**: Erstellen eines Backups von einzelnen Dateien oder Ordnern
- **Clone**: Kopieren einer Festplatte oder Partition auf eine andere Festplatte oder Partition
- **Rescue Media**: Erstellen eines bootfähigen USB-Sticks oder einer bootfähigen CD/DVD, um ein Backup wiederherzustellen

![Macrium Reflect](x_resources/macrium.png)

- [Macrium Reflect](https://www.macrium.com/reflectfree)