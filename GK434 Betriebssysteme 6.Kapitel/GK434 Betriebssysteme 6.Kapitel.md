## GK434 Betriebssysteme 6.Kapitel

### Zusammenfassung:

#### 6.3 Dateisysteme mit Dateizuordnungstabellen

Ein Dateisystem ist eine Ablageorganisation auf einem Datenträger, das den Zugriff auf dessen Dateien organisiert. Es legt fest wie Daten auf einem Speichermedium gespeichert, gelesen, verändert oder gelöscht werden können. Es ist eine Schnittstelle zwischen Betriebssystem und Laufwerk.



Die Dateizuordnungstabelle (FAT) ist eine Tabelle fester Größen, die für jeden Cluster des Dateisystems einen Eintrag enthält, der angibt ob der Cluster frei, das Medium an dieser Stelle beschädigt oder der Cluster von einer Datei belegt ist. Das Ende der Datei wird mit EOF ( End-Of-File) gekennzeichnet. Die Nummer im Versionsnamen gibt die Länge der clusternummern an.

Die Konsistenz der Fat ist für die Funktionalität des Dateisystemes sehr wichtig, deswegen