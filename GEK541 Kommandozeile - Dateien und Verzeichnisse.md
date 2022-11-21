# GEK541 Kommandozeile - Dateien und Verzeichnisse

Verfasser: Rajic Dejan

Datum: 21.11.2022

## Einführung 

Da Linux in sehr vielen Anwendungsbereichen sehr gefragt ist,  wird nun der richtige Umgang damit Nähergebracht. Insbesondere wird man sich die Kommandozeile ansehen.

### Detaillierte Aufgabenbeschreibung

Starte deine virtuelle Maschine oder verbinde dich mit einer Konsole auf einen Linux-Rechner. Du kannst auch die grafische Oberfläche deines  Linux-Systems nutzen. 

* Welche Möglichkeiten gibt es die Kommandozeile zu  öffnen? 
  * Windowstaste oder Grafisch die Dash auswählen (obere linke ecke) und auf Terminal Emulator Klicken
  * Strg + Alt + T
* Was ist ein **terminal emulator** und wo kommt dieser zum Einsatz?
  * [1]**Terminalemulationen simulieren Terminals anderer, meist entfernter, Computer**. Sie bilden eine Schnittstelle zur Dateneingabe und Steuerung eines entfernten Computers.
* Was ist der Unterschied zwischen Befehl, Option

### Grundanforderungen

* Grundbefehle
  * cd: change directory, man wechselt in ein anderes Verzeichniss
  * cat: common, alternate spellings or phrasings ,[2] Der Befehl cat **liest die mit dem Parameter Datei angegebenen Dateien nacheinander und schreibt sie in die Standardausgabe**
  * echo: Wiederholt das was man ihm zu wiederholen gegeben hat(wie ein echo)
  * ls: list, gibt eine Listevon Datein aus 
  * rmdir: remove directory, löscht ein Verzeichnis
  * man: manuel, gibt eine liste mit allen befehlen für das Terminal aus
  * exit: beendet ein programm oder schließt das Terminal
  * login: wechselt den Benutzer
  * mkdir: make directory, erstellt ein verzeichnis

### Verlassen des Terminals

* Wie kann man das Terminal nun verlassen?
  * exit
*  Wie kann der Befehl auch durch eine Tastenkombination aufgerufen werden?
  * Alt + f4
* Wo liegt der Unterschied zu dem naheliegenden `logout`? 
  * Man wird aus dem terminal abgemeldet
* Was passiert wen man mittels ssh auf ssh auf einem Server verbunden ist?
  * man kann den server fernsteuern

### Absoluter / relativer Verzeichnisbaum

* Wo liegt der Unterschied zu absoluten Pfaden und relativen Pfaden?
  * **Ein absoluter Pfad ist immer der komplette Pfad.** **Er beginnt also immer in Wurzelverzeichnis /.** **Ein relativer Pfad beginnt immer im aktuellen Verzeichnis**.
* Was ist der unterschied zwischen . und .. ?
  * 

* Wie heißt der Befehl, der einen den aktuellen Ort mitteilt?
  * 

* Was ist das Heimverzeichnis? 
  * [3] Das **Homeverzeichnis** ist der Ort, an dem Benutzer ihre Daten ablegen können und an dem  Programme ihre benutzerspezifischen Einstellungen hinterlegen. Nur hier  hat der einzelne Benutzer volle Schreib- und Leserechte. Und nur hier  sollten Benutzer ihre Daten speichern.
* Wie gelangt man dorthin?
  * cd ~
* In welchem Verzeichnis liegen die meisten Benutzer-Befehle unter Linux?
  * root
* Wo liegt der Unterschied zu absoluten Pfaden? Und was sind `.` und `..`?
  * [4]**Ein absoluter Pfad ist immer der komplette Pfad.** **Er beginnt also immer in Wurzelverzeichnis /.** **Ein relativer Pfad beginnt immer im aktuellen Verzeichnis**.

## Quellen



[1]"Terminalemulation, Terminalemulator - Software und Anbieter", *Softguide.de*, 2022. [Online]. Available: https://www.softguide.de/software/emulation. [Accessed: 17- Oct- 2022].

[2]"IBM Documentation", *Ibm.com*, 2022. [Online]. Available: https://www.ibm.com/docs/de/aix/7.2?topic=c-cat-command. [Accessed: 17- Oct- 2022].

[3]"Homeverzeichnis › Wiki › ubuntuusers.de", *Wiki.ubuntuusers.de*, 2022. [Online]. Available: https://wiki.ubuntuusers.de/Homeverzeichnis/. [Accessed: 17- Oct- 2022].

[4]C.  Piazzi, "Aufbau und Umgang mit der Verzeichnisstruktur unter Linux", *Modius - Techblog*, 2022. [Online]. Available:  https://www.modius-techblog.de/linux/aufbau-und-umgang-mit-der-verzeichnisstruktur-unter-linux/. [Accessed: 17- Oct- 2022].

[5] Aufbau und Umgang mit der Verzeichnisstruktur unter Linux [Online]. Available: https://www.modius-techblog.de/linux/aufbau-und-umgang-mit-der-verzeichnisstruktur-unter-linux/ [Accessed: 21.11.2022] 