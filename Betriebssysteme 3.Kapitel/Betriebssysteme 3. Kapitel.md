# GK433 Betriebssysteme 3. Kapitel

## Einführung

Die Entwicklung und der Einsatz von Betriebssystemen sind  ein wichtiger Teil der Informatik. Da Betriebssysteme auch seit mehr als fünfzig Jahre im täglichen Einsatz sind, haben diese auch eine bereits  lange Geschichte in der Informatik. Diese Themen und der grundlegende  Aufbau von Betriebssystemen sind Teil dieses Moduls und auch des dritten Kapitels des Buchs "Betriebsysteme kompakt"!



## Ziele

Es wird im Buch "Betriebssysteme Kompakt" darum gehen die Grundlagen und Funktionalitäten von Betriebssystemen zu verstehen. 

## Detaillierte Aufgabenstellung

**Beschreibe jedes der Teilgebiete der Informatik:**

* **Praktische Informatik**: Formulierung von Algorithmen als Programme, Betriebssysteme,
  Steuerungssystemen, Programmiersprachenentwicklung

* **Technische Informatik: **Untersuchung des funktionellen Aufbaus der Hardware,
  logischer Entwurf von Rechentechnik, maschinennahe Programmierung.
  Betriebssysteme gehören auch ein bisschen zur technischen Informatik aufgrund der
  Aufgabe, dass Betriebssysteme auch den Computer steuern.

* **Theoretische Informatik: **Untersuchung der (meist) mathematischen Grundlagen der
  Information, ihre Darstellung und effiziente Verarbeitung.

* **Angewandte Informatik: **Anwendung von technischer, praktischer und theoretischer
  Informatik in anderen Wissenschaften und Gesellschaftsbereichen

  

**Fasse die Kernfunktionalitäten von Betriebssystemen kurz und prägnant zusammen**.

* Verwaltung von Hardwarekomponenten und Daten in verschiedenen Datenspeichern(Cache, Hauptspeicher...) als auch Verwaltung von Prozessen, Bereitstellung von Funktionalitäten zur Interprozesskommunikation unterschiedlicher Benutzergruppen.



 **Zeichne einen kleinen Zeitstrahl (auf einem [Grafiz](https://elearning.tgm.ac.at/mod/folder/view.php?id=238414)) über die Entwicklung der Computersysteme** **Beschreibe kurz jede dieser Generationen**.

Die Geschichte der Betriebssysteme reicht zurück bis in die 1950er-Jahre. **Zeichne einen kleinen Zeitstrahl (auf einem [Grafiz](https://elearning.tgm.ac.at/mod/folder/view.php?id=238414)) über die Entwicklung der Computersysteme**! Am Gang zwischen H127 und H129 befindet sich ein Zeitstrahl der  Informatik, der als Inspiration und Unterstützung helfen kann und im  Buch gibt es einen Überblick über die fünf Generationen der Computer. **Beschreibe kurz jede dieser Generationen**.

Jedes Betriebssystem hat als zentralen Bestandteil einen  Betriebssystemkern oder im englischen auch Kernel genannt. Die Struktur  und Architektur von einem Kernel können unterschiedlich aufgebaut sein.  Die drei verschiedenen Architekturen sind der monolithischem Kernel,  Mikrokernel und Hybridkernel. Schreibe eine **kurze Zusammenfassung über die drei Betriebssystemekerne**. Gerne kannst du dafür auch eine grafische Darstellung in Form von einen [Grafiz](https://elearning.tgm.ac.at/mod/folder/view.php?id=238414) machen.



## Fragestellungen

-  In welchem/n Teilgebiet(e) der Informatik befindet sich das Thema der Betriebssysteme?
  - Die Betriebssysteme gehören in das Teilgebiet der praktischen Informatik wo auch die
    Steuerungssysteme und Programmiersprachenentwicklung dazugehört.
-  Welche Arten von Betriebssysteme gibt es und wie unterscheiden sie sich? Nenne Beispiele für jede Art?
  - Stapelbetrieb und Dialogbetrieb:
    Der Stapelbetrieb ist eine Betriebsart, bei der das Programm mit allen Eingabedaten vollständig vorliegen muss, bevor die Abarbeitung beginnen kann. Üblicherweise ist Stapelbetrieb interaktionslos.
    Beim Dialogbetrieb können mehrere Benutzer gleichzeitig über Dialogstationen an einem Großrechner arbeiten.
  - Einzelprogrammbetrieb und Mehrprogrammbetrieb:
    Beim Einzelprogrammbetrieb kann zu jedem Zeitpunkt nur ein einziges Programm laufen. Mehrere Programme können im Mehrprogrammbetrieb gleichzeitig mit dem Computer arbeiten.
  - Einzelbenutzerbetrieb und Mehrbenutzerbetrieb:
    Der Computer steht im Einzelbenutzerbetrieb immer nur einem einzigen Benutzer zur Verfügung. Beim Mehrbenutzerbetrieb können mehrere Benutzer gleichzeitig mit dem Computer arbeiten.
-  Was bedeutet die Speichereinheiten in Betriebssysteme (8-bit, 16-bit, 32-bit, ...)?
  - Ein Betriebssystem kann nur so viele Speichereinheiten ansprechen, wie der Adressraum zulässt. So kann ein 64-Bit-Betriebssystem mehr Speicher ansprechen als eines mit 32-Bit.
-  Was macht Echtzeitbetriebssysteme so besonders? Was sind die Vor- und Nachteile?
  -  Echtzeitbetriebssysteme bieten Mehrprogrammbetrieb und haben zusätzlich Echtzeitfunktionen für die Einhaltung von Deadlines.
  -  Regelt alle aufgaben in genauen Taktschritten
  -  Weiche Betriebssysteme = Laptops
  -  harte Betriebssysteme = Datacenters
  -  Vorteil: Gut für Systeme geeignet die Dauerbetrieb erfordern, oder bei denen Ausfallzeiten nicht hinnehmbar sind.
  -  Nachteil: Teuer, aufwändiger, schwierig

-  Was ist das Konzept hinter verteilten Betriebssystemen?
  - Es steuert Prozesse auf mehreren unabhängigen Computern, wobei die einzelnen Knoten verborgen bleiben. Es erscheint als ein einziger großer Computer.
-  Das Betriebssystem Plan 9 wird gerne als Unix-Nachfolger gesehen. Was  ist ein wichtiges Grundprinzip hinter dem Plan-9 Betriebssystem?
  - Everything in a File, Sollte Nachfolger von Unis sein, wird nicht mehr umgesetzt
-  Was ist der Unterschied zwischen GNU/Linux und einem Unix-Betriebssystem?
  - Gnu/Linux ist open Source, man läd sich alle Werkzeuge selbst runter. Es hat eine eigene Shell, die GNU, verwendet jedoch den UNIX-ähnlichen Kernel
    
  - Unix ist closed Source, enthält Standardmäßig viele Werkzeuge. Das UNIX besteht aus der Shell und dem Kernel und könnte für sich alleine funktionieren

## Quellen