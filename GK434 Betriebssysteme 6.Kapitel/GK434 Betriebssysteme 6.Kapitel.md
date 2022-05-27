## GK434 Betriebssysteme 6.Kapitel

### Verfasser: Dejan Rajic

### Datum: 27.05.2022



### Zusammenfassung:

#### 6.3 Dateisysteme mit Dateizuordnungstabellen

Ein Dateisystem ist eine Ablageorganisation auf einem Datenträger, das den Zugriff auf dessen Dateien organisiert. Es legt fest wie Daten auf einem Speichermedium gespeichert, gelesen, verändert oder gelöscht werden können. Es ist eine Schnittstelle zwischen Betriebssystem und Laufwerk.



Die Dateizuordnungstabelle (FAT) ist eine Tabelle fester Größen, die für jeden Cluster des Dateisystems einen Eintrag enthält, der angibt ob der Cluster frei, das Medium an dieser Stelle beschädigt oder der Cluster von einer Datei belegt ist. Das Ende der Datei wird mit EOF ( End-Of-File) gekennzeichnet. Die Nummer im Versionsnamen gibt die Länge der clusternummern an.

Die Konsistenz der FAT ist für die Funktionalität des Dateisystems sehr wichtig, deswegen wird immer eine Kopie der FAT erstellt damit man Datenverlust  verhindern kann. Es gibt mehrere Sektoren im FAT, den Bootsektor, Den reservierten Sektor, FAT, Das Stammverzeichnis und die eigentlichen Daten.

 Zwischen Dem Bootsektor und der ersten FAT können sich manchmal optionale reservierte Sektoren befinden die den Bootsektor dienen. Das Stammverzeichnis speichert von jeden Datei das jeweilige Verzeichnis durch einen Eintrag. Bei FAT12 und FAT16 haben hat das Stammverzeichnis immer eine feste Größe. Bei FAT32 ist sie variabel. Der letzte Bereich sind die eigentlichen Daten.

Häufig vorkommende Probleme bei Dateisystemen sind querverbundene oder verlorene Cluster. Diese entstehen wenn ein Eintrag auf den nächsten Cluster einer Datei nicht korrekt ausgesucht wurde und sich somit zwei Dateien miteinander verbinden und der originelle restliche Teil der ersten Datei verloren geht.

#### Fat12

Bei Fat12 sind Clusternummern 12 Bits lang. Es können maximal 2096 Cluster adressiert werden. Das entspricht einer maximalen Dateisystemgröße von 16 MB

#### Fat16

Bei FAT16 können 6.536 Cluster pro Dateisystem adressiert werden. Weil 12 Cluster aber schon reserviert sind beträgt die letztendliche effektive Zahl nur 65.524. die Clustergrößen können zwischen 512 und 256 Bytes variieren Die Partitionsgröße sind aufgrund der variablen Clustergrößen 31MB bis 16GB. FAT16 wird bei USB Sticks verwendet. 

#### FAT32

Da 4 Bits reserviert sind, können 268.435.456 Cluster adressiert werden. Die Cluster könne zwischen 512Bytes und 32 kB groß sein. Die maximale Dateigröße unter FAT 32 ist 4GB, weil nur 4 Bytes für die Angabe der Dateigröße zur Verfügung stehen. FAT32 wird auch wie FAT16 für mobile Datenträger verwendet mit einer Kapazität von mehr als 2GB.

#### VFAT

Mit VFAT könne Dateinamen bis zu einer Länge von 255 Zeichne realisiert werden. Es wird mit Unicode kodiert. Lange Dateinamen verteilt VFAT auf maximal 20 Pseudo-Verzeichniseinträge. Bei einem VFAT Eintrag haben die ersten vier Bits im Feld Dateiattribute den Wert 1. Es werden Groß/Kleinschreibung angezeigt aber wie bei den anderen FATS ignoriert. Es wird nur der verkürzte Nameangezeigt. Jeder Dateiname muss eindeutig sein. Alle Sonderzeichen und Punkte werden innerhalb des Dateinamens Gelöscht, alle Kleinbuchstaben werden in Großbuchstaben umgewandelt und es werden nur die ersten sechs Buchstaben beibehalten.

#### Journaling-Dateisysteme

Um bei Konsistenzprüfung die zu überprüfenden Daten einzugrenzen, für moderne Dateisysteme ein sogenanntes Journal ein. Dabei werden alle Schreibzugriffe vor ihrer Durchführung gesammelt. Ein Vorteil ist dabei, dass nach einem Absturz nur diejenigen Dateien(Cluster) und Metadaten ÜBERRÜFT werden müssen, die im Journal stehen. Ein Journal erhöht die Anzahl der Schreibzugriffe, weil Änderungen erst ins Journal geschrieben und danach durchgeführt werden. Es gibt verschiedene Journaling Konzepte wie z.B Metadaten-Journaling, vollständiges-Journaling und ordered Journaling.

Beim Metadaten Journaling erfasst das Dateisysteme im Journal Änderungen an den Metadaten. Vorteilhaft ist das die Konsistenzprüfung nur wenige Sekunden braucht. Nachteil ist, dass die Konsistenz der Metadaten nach einem Absturz garantiert ist.

Beim vollständigen Journaling erfasst das Dateisystem alle Änderungen an den Metadaten und alle Änderungen an den Clustern der Dateien im Journal. Dadurch ist die Konsistenz der Dateien garantiert. Nachteil ist , dass alle Schreibzugriffe doppelt ausgeführt werden .

Das Order-Journaling erfasst nur Änderungen an den Metadaten. Änderungen an den Clustern von Dateien werden erst im Dateisystem durchgeführt und danach die Änderungen an den Betreffenden Metadaten ins Journal geschrieben. Vorteil ist das es nur wenige Sekunden dauert und ähnlich hohe Schreib-Geschwindigkeit wie bei Metadaten-Journaling erreich,t, aber es ist garantiert das beim System Absturz alle nicht abgeschlossenen Transaktionen im Journal verloren gehen.

#### Extent-basierte Adressierung

Bei Dateisystemen die nach Adressierungsschema der Blockadressierung arbeiten gibt es ein Problem. Der Verwaltungsaufwand für die Informationen ist zu hoch. Dieses Problem wird durch die steigende Speicherkapazität immer schlimmer. Eine Lösung um dies Zu umgehen sind Extents. Bei Extent Basierter Adressierung adressieren die Inodes nicht einzelne Cluster, sondern bilden eine möglichst große Dateibereiche die zusammenhängen. Statt vieler einzelner Clusternummern erfordert dies Form nur drei werte. die erste Clusternummer des Bereichs in der Datei, die Größe des Bereichs in der Datei und die Nummer des ersten Clusters auf dem Speichergerät. Beispiele dafür wären JFS, XFS, Btrfs, NTFS und ext4