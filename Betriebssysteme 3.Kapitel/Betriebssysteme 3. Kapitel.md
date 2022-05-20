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
  logischer Entwurf von Rechentechnik, maschinennahe Programmierung. Auch Betriebssysteme fallen unter die technische Informatik, weil das Betriebssystem steuert die Aufgaben des Computers.
* **Theoretische Informatik: **Untersuchung der mathematischen Grundlagen der
  Information, ihre Darstellung und effiziente Verarbeitung.
* **Angewandte Informatik: **Angewandte Technik, Praxis und Theorie der
    Informatik in anderen wissenschaftlichen und gesellschaftlichen Bereichen



**Fasse die Kernfunktionalitäten von Betriebssystemen kurz und prägnant zusammen**.

* Daten in verschiedenen Datenspeichern wie z.B (Cache,Hauptspeicher,etc.) und Hardwarekomponenten werden Verwaltet.  Es werden Funktionalitäten zur Interprozesskommunikation unterschiedlicher Benutzergruppen bereitgestellt.



 **Zeichne einen kleinen Zeitstrahl (auf einem [Grafiz](https://elearning.tgm.ac.at/mod/folder/view.php?id=238414)) über die Entwicklung der Computersysteme** **Beschreibe kurz jede dieser Generationen**.



![index](https://user-images.githubusercontent.com/78872776/169475301-b7af82ff-2072-4f62-8d9f-19b1b6280684.jpg)





**Monolithischer Kernel**:

Ein Vorteil des monolithischen Kernels ist, dass er schon alle Funktionen eines Betriebssysteme erbringt. Es lässt sich auch hervorheben, dass weniger Prozesswechsel nötig sind, dadurch ist die Ausführgeschwindigkeit und Stabilität besser. Jedoch kann man nicht separate Komponenten des Kerns neu starten, in dem Falle kann es sein das das gesamte Betriebssystem abstürzt. Das dauernde Kompilieren und Übersetzen kann man auch zu den Nachteilen Zählen.

**Mikro Kernel**:

Nur die nötigsten Funktionen zur Speicher- und Prozessverwaltung sowie zur Synchronisation und Interprozesskommunikation. Gerätetreiber, Treiber für
Dateisysteme  laufen mit allen verbleibenden Funktionalitäten als sogenannte Dienste oder auch Server
außerhalb des Kerns im Benutzermodus. Diese Architektur hat die geringste Ausführungsgeschwindigkeit, weil es die meisten Prozesswechsel aufzeigt.

**Hybride Kerne:**

Enthält Aspekte von einem monolithischen Kern und einem minimalen kern, wird auch Makro Kernel genannt. Sie enthalten aus Geschwindigkeitsgründen Komponente die außerhalb der minimalen Kerne liegen. Im Vergleich zum minimalen Kern haben sie eine höhere Geschwindigkeit um zum
monolithischen Kern eine höhere Stabilität.

## Fragestellungen

-  In welchem/n Teilgebiet(e) der Informatik befindet sich das Thema der Betriebssysteme?
  - Die Betriebssysteme gehören in das Teilgebiet der praktischen Informatik wo auch die
    Steuerungssysteme und Programmiersprachenentwicklung dazugehört.
-  Welche Arten von Betriebssysteme gibt es und wie unterscheiden sie sich? Nenne Beispiele für jede Art?
  - Stapelbetrieb und Dialogbetrieb:
    Der Stapelbetrieb ist eine Betriebsart, bei der das Programm mit allen Eingabedaten vollständig vorliegen muss, bevor die Abarbeitung beginnen kann. Üblicherweise ist Stapelbetrieb interaktionslos.
    Beim Dialogbetrieb können mehrere Benutzer gleichzeitig über Dialogstationen an einem Großrechner arbeiten (Linux, DOS,Unix).
  - Einzelprogrammbetrieb und Mehrprogrammbetrieb:
    Beim Einzelprogrammbetrieb kann zu jedem Zeitpunkt nur ein einziges Programm laufen. Mehrere Programme können im Mehrprogrammbetrieb gleichzeitig mit dem Computer arbeiten.
  - Einzelbenutzerbetrieb und Mehrbenutzerbetrieb:
    Der Computer steht im Einzelbenutzerbetrieb immer nur einem einzigen Benutzer zur Verfügung. Beim Mehrbenutzerbetrieb können mehrere Benutzer gleichzeitig mit dem Computer arbeiten. Die Leistung wird zwischen den Nutzern aufgeteilt(Linux, Mac OS X).
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

[1] "Betriebssysteme Kompakt Springer Buch". 2020. Available at: TGM-Elearning: Hier können
Sie sich anmelden [Accessed 19 May 2022].
[2] De.wikipedia.org. 2022. Betriebssystem - Wikipedia. [online] Available at: Betriebssystem –
Wikipedia [Accessed 19 May 2022].
[3] www.tinohempel.de. 2022. Informatik und deren Teilgebiete - Tinohempel. [online] Available
at: Informatik und deren Teilgebiete [Accessed 19 May 2022].

[4] www.sawakinome.com. 2022. Unterschied zwischen GNU und Unix - Sawakinome. [online]
Available at: Unterschied zwischen GNU und Unix [Accessed 19 May 2022].


