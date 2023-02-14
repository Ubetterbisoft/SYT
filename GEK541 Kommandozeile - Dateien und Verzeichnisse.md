# GEK541 Kommandozeile - Dateien und Verzeichnisse

Verfasser: Rajic Dejan

Datum: 21.11.2022

## Einführung 

Da Linux in sehr vielen Anwendungsbereichen sehr gefragt ist,  wird nun der richtige Umgang damit Nähergebracht. Insbesondere wird man sich die Kommandozeile ansehen.

### Detaillierte Aufgabenbeschreibung

Starte deine virtuelle Maschine oder verbinde dich mit einer Konsole auf einen Linux-Rechner. Du kannst auch die grafische Oberfläche deines  Linux-Systems nutzen. 

* **Welche Möglichkeiten gibt es die Kommandozeile zu  öffnen?** 
  
  * Windowstaste oder Grafisch die Dash auswählen (obere linke ecke) und auf Terminal Emulator Klicken
  * Strg + Alt + T
  
* **Was ist ein terminal emulator und wo kommt dieser zum Einsatz?**
  
  * [1]**Terminalemulationen simulieren Terminals anderer, meist entfernter, Computer**. Sie bilden eine Schnittstelle zur Dateneingabe und Steuerung eines entfernten Computers.
  
  

## Grundanforderungen

* **Grundbefehle**
  * cd: change directory, man wechselt in ein anderes Verzeichniss
  * cat: common, alternate spellings or phrasings ,[2] Der Befehl cat **liest die mit dem Parameter Datei angegebenen Dateien nacheinander und schreibt sie in die Standardausgabe**
  * echo: Wiederholt das was man ihm zu wiederholen gegeben hat(wie ein echo)
  * ls: list, gibt eine Liste von Datein aus 
  * rmdir: remove directory, löscht ein Verzeichnis
  * man: manuel, gibt eine liste mit allen befehlen für das Terminal aus
  * exit: beendet ein programm oder schließt das Terminal
  * login: wechselt den Benutzer
  * mkdir: make directory, erstellt ein verzeichnis

### Verlassen des Terminals

* **Wie kann man das Terminal nun verlassen?**
  * exit Befehl
*  **Wie kann der Befehl auch durch eine Tastenkombination aufgerufen werden?**
  * Alt + f4
* **Wo liegt der Unterschied zu dem naheliegenden `logout`?** 
  * Man wird aus dem terminal abgemeldet. Die Tastenkombination ist Strg+D
* **Was passiert wen man mittels ssh auf ssh auf einem Server verbunden ist?**
  * man kann den server fernsteuern. Wenn man beschließt das Terminal zu schließen wird das Terminal zwar geschlossen, jedoch nicht die Verbindung zum  SSH Server

### Absoluter / relativer Verzeichnisbaum

* **Wo liegt der Unterschied zu absoluten Pfaden und relativen Pfaden?**
  * Ein absoluter Pfad ist immer der komplette Pfad. Er beginnt also immer in Wurzelverzeichnis /. Ein relativer Pfad beginnt immer im aktuellen Verzeichnis.
* **Wie heißt der Befehl, der einen den aktuellen Ort mitteilt?**
  * Der Befehl heist: pwd
    * Beispiel: ``$ pwd``
      Output: /home/user/Documents
* **Was ist das Heimverzeichnis?** 
  * [3] Das **Homeverzeichnis** ist der Ort, an dem Benutzer ihre Daten ablegen können und an dem  Programme ihre benutzerspezifischen Einstellungen hinterlegen. Und nur hier  sollten Benutzer ihre Daten speichern.
* **Wie gelangt man dorthin?**
  * ``$ cd /home/``
* **In welchem Verzeichnis liegen die meisten Benutzer-Befehle unter Linux?**
  * Die meisten Befehle befinden sich in Form von Programmen in  Verzeichnis bin/
  * Dieses Verzeichnis lässt sich mithilfe von ``$ cd /bin/ erreichen``
* **Wo liegt der Unterschied zu absoluten Pfaden? Und was sind `.` und `..`?**
  * [4]**Ein absoluter Pfad ist immer der komplette Pfad.** **Er beginnt also immer in Wurzelverzeichnis /.** **Ein relativer Pfad beginnt immer im aktuellen Verzeichnis**.
  * Wenn man einen Absoluten Pfad nutzt kann man direkt in alle Verzeichnisse gelangen. Bei einem relativen pfad geht dies nicht.



## Befehle, Dateien und die Pipe

* **Wie könnte man aber nun die Ausgabe von ls -l /etc/* in eine Datei umleiten?**

  * Mit ls -l /etc/* > ausgabe.txt oder ls -l /etc/* >> ausgabe.txt

    

* **Wo ist dabei der Unterschied zu > und >> ?**

  * Mit > wird die Ausgabe des Befehls in eine Datei gespeichert und der eigentliche Inhalt gelöscht.

  * Mit >> wird die Ausgabe des Befehls ans Ende einer Datei angefügt.

    

* **Und wenn das in die eine Richtung geht, kann man auch aus einer Datei Befehle bestimmte**
  **Informationen übergeben?**

  * Ja das geht mit <

* **Schreibe in eine Datei namens ~/Hallo.txt den Text "Hallo Welt!". Welcher Befehl bietet**
  **sich dafür an? Was bedeutet die ~ ?**

  * echo "Hallo Welt!" > ~/Hallo.txt

## Fragestellungen

* **Wo bekommt man Unterstützung für einen Befehl?**
  * Um Hilfe zu bekommen macht man ein -h oder --help nach dem Befehl
  * Beispiel: ls -h
* **Wo liegt der Unterschied zwischen der Übergabe von einem oder zwei Bindestrichen bei der**
  **Verwendung von Optionen? (z.B. sudo -h und sudo --help )**
  * Mit nur einem - sind die Optionen einfach kürzer gestaltet. Sie sind hier mit nur einem Buchstaben verwendbar.
  * Mit zwei -- müssen die Optionen länger als ein Buchstabe sein.
  * Beispiel: $ ls -h ist das Selbe wie $ ls --help
* **Welche Funktionsweise hat die $PATH -Variable? Wie wird sie verwendet und wie ist sie unter**
  **Linux aufgebaut? Wie ist $PATH unter Windows aufgebaut?**
  * In der $Path Variable werden einige Pfade gespeichert. Diese Pfade dienen als
    Installationsverzeichnisse. So muss nicht immer ein Installationsverzeichnis angegeben
    werden. Unter Linux kann man sich die Path Variable mit echo path ausgeben lassen.
    Hier sind die Pfade durch Doppelpunkte getrennt.
  * In Windows werden die in $PATH gespeicherten Variablen nach ausführbaren Dateien
    durchsucht. Diese Dateien können dann ohne Angabe des Pfades ausgeführt werden.
    Man kann diese in Windows mit PATH ausgeben lassen. Hier werden die Pfade, anders
    als in Linux, durch Semikolons getrennt, angezeigt.
* **Wie kann die $PATH Variable angepasst werden? Wann kommt die Anpassung zur**
  **Anwendung?**
  * Man fügt Pfade zu $PATH hinzu wenn man bestimmte Executables ausführen möchte
    ohne jedes Mal den Pfad angeben zu müssen.
  * Man kann pfade zu $PATH hinzufügen indem man folgendes ausführt: export
    PATH=$PATH: ORDNER
* **Woran erkennt man einen relativen Pfad (im Gegensatz zu einem absoluten)?**
  * Ein absoluter Pfad hat immer ein / vor dem Pfad
  * Beispiel: /home/dejan/ <- absolut; dejanr/ <- relativ
* **Nenne zwei Arten, wie man das home Verzeichnis des aktuellen Benutzers ermitteln kann.**
  **Wo liegt dieses üblicherweise?**
  * Man kann das home Verzeichnis des aktuellen Users mithilfe von echo ~ òder echo
    $HOME ermitteln.
  * Normalerweise befindet sich das home Verzeichnis eines Users in /home/
* **Ein Benutzer möchte seinen Download-Ordner archivieren und tut dies mittels cp**
  **Downloads/ backup . Warum funktioniert das nicht und was sollte er stattdessen aufrufen?**
  * Mit cp Downloads/ backup/ kann der Download Ordner nicht archivirt werden, da der
    Befehl cp stadndardmäßig nur Dateien kopieren kann. Um mit dem Befehl ganze
    Ordner zu kopieren muss man -R hinzufügen.
  * Um den Downloads Ordner richtig zu archivieren muss man cp -R Downloads/
    backup/ nutzen.

## Quellen

[1]"Terminalemulation, Terminalemulator - Software und Anbieter", *Softguide.de*, 2022. [Online]. Available: https://www.softguide.de/software/emulation. [Accessed: 17- Oct- 2022].

[2]"IBM Documentation", *Ibm.com*, 2022. [Online]. Available: https://www.ibm.com/docs/de/aix/7.2?topic=c-cat-command. [Accessed: 17- Oct- 2022].

[3]"Homeverzeichnis › Wiki › ubuntuusers.de", *Wiki.ubuntuusers.de*, 2022. [Online]. Available: https://wiki.ubuntuusers.de/Homeverzeichnis/. [Accessed: 17- Oct- 2022].

[4]C.  Piazzi, "Aufbau und Umgang mit der Verzeichnisstruktur unter Linux", *Modius - Techblog*, 2022. [Online]. Available:  https://www.modius-techblog.de/linux/aufbau-und-umgang-mit-der-verzeichnisstruktur-unter-linux/. [Accessed: 17- Oct- 2022].

[5] Aufbau und Umgang mit der Verzeichnisstruktur unter Linux [Online]. Available: https://www.modius-techblog.de/linux/aufbau-und-umgang-mit-der-verzeichnisstruktur-unter-linux/ [Accessed: 21.11.2022] 