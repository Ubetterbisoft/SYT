# GK 314 Virtualisierung

### Autor: Dejan Rajic

### Datum: 3.3.2022

## Einführung

In dieser Dokumentation werden wichtige Tatsachen und Informationen zu Virtuellen Maschinen beschrieben und angeführt. Die Beweggründe dieser Dokumentation und dieser Aufgabe sind Schulischer Natur. Das hier herangeführte Wissen ist hauptsächlich auf die Theorie reduziert.

## Theorie

#### Aufgaben-/Fragestellung: VirtualBox

* Was ist der Unterschied zwischen NAT und Netzwerkbrücke in den Netzwerkeinstellung der VirtualBox?

  * Beim NAT hat man nur als Gast zugriff auf ein externes Netzwerk.
  * Bei der Netzwerkbrücke hat man als Gast zugriff auf andere Geräte und ein externes Netzwerk. Und der Host hat zugriff auf den Gast

* Was ist der Host-Key und wie kommt dieser zum Einsatz?
  * Das ist die Taste welche den User zum Host zurück bringt. Der Host-Key ist die Rechte Strg Taste

* Wie lässt sich die Gasterweiterung unter Linux installieren und warum wird diese benötigt?

  * Damit die VM richtig skalliert wird. Copy und Paste wird aktiviert. Mann kann mehrere Desktops haben.  Man kann auch Windows gleichzeitig auf Mac laufen lassen, dabei kann man Windows auf einen Anderen Desktop parralel oder in einem Desktop in einem Fenster laufen lassen.

  

#### Allgemeine Fragestellungen  - Virtualisierung, Simulation, Emulation : 

- Was ist der Unterschied zwischen Emulation, Simulation und Virtualisierung? Wo kommt was zum Einsatz?
  - Die Emulation ist die Nachahmung der Funktion eines Computers
  - Die Simulation ist die Nachbildung von realen Szenarien wie z.B Ausbildung, Unterhaltung etc.
  - Virtualisierung ist die die Simulation oder Emulation als Software.
- Was macht Containering(wie zB. Docker) und wo kommt es zum Einsatz? Was sind die Vor- und Nachteile?
  - Ist eine abgespeckte Form von einer Virtual-Machine die nur Programme ausführt.
  - [1]**Docker Container** sind  eine Art light-Version von Virtuellen Maschinen. Während Virtuelle  Maschinen die Hardware eines Rechners, also den Prozessor, die  Festplatte, usw. virtualisieren, virtualisieren **Docker Container** das Betriebssystem. Dies wird auch Container Virtualisierung genannt.
  - Vorteil: Geringer Ressourcenverbrauch
  - Vorteil: Sehr skallierbarr
  - Vorteil: Sehr flexibel einsetzbar für Microservices
  - Nachteil: Es kann nie so schnell sein wie eine richtige Virtual Machine
  - Nachteil: Generelle Sicherheitsprobleme
  - Nachteil: Komplizierter in Einrichtung und Verwaltung
- Was macht ein "cycle accurate" Emulator?
  - Ein Emulator der so schnell läuft wie das System selbst
- Was wird mit Thinkcad simuliert?
  - 3D Konstruktionen und Geometrie

​		

#### Fragestellung BASH in der VM:

- Was ist die Bash?

  - Born again shell
  - Ist eine Commandline Interface

- Wie sind die Bash-Befehle aufgebaut? Was ist ein Argument? Was ist eine Option?

  - Nach einem Befehl kann man Argumente und Funktionen setzen.
  - Ein Argument kommt nach dem Befehl und der Befehl kann mit dem Inhalt des Arguments arbeiten
  - Eine Option ist das wo ein - davorsteht, damit kann man sagen, was der Befehl machen soll

- Wie kann ich die Dokumentation zu einem Bash-Befehl finden?

  - Mit `man ls`  und  `-h`

- Mit welchem Befehl kann ich den Inhalt von einem Ordner abfragen? Was ist  dabei der Unterschied von relativen und absoluten Pfad?

  - Mit `ls` .
  - [2] Der **absolute Pfad** bezieht sich immer auf ein Stammverzeichnis des Servers (Root).
  - [2]  Der **relative Pfad** zeigt die Struktur des Verzeichnisses an.

- Wie wird ein Software-Update mit der Bash durchgeführt? Was ist der Befehl dafür?

  - `sudo apt update`

- Welche sind die wichtigsten Befehle?

  - cd

  - mkdir

  - touch

  - pwd

  - nano

  - vim

  - rm

  - mv

    

# Quellen

[1] Was sind Docker Container - in 90 Sekunden - Systempilot 

https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwirxrjI9qH2AhW1RfEDHcdmAZAQFnoECA4QAw&url=https%3A%2F%2Fsystempilot.net%2Fdocker-container%2F&usg=AOvVaw0t1VzqToPYxspqIP0uJnb4

[2] [Was ist der Unterschied zwischen dem absoluten und  relativen Pfad 

https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwjJjPH0_qH2AhW4SfEDHevyAagQFnoECAsQAw&url=https%3A%2F%2Ffaq.swizzonic.ch%2Fist-der-unterschied-zwischen-dem-absoluten-und-relativen-pfad%2F&usg=AOvVaw1mcrSm0a7iqNu2mw6sizbj

 Unterschied zu NAT und Netzwerkbrücke: https://www.thomas-krenn.com/de/wiki/Netzwerkkonfiguration_in_VirtualBox