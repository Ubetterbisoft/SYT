# GK431 Betriebssysteme 1.Kapitel

## Autor: Dejan Rajic

## Veröffentlicht: 29.03.2022

## Ziele

Zusammenfassen des Vorworts, Inhaltsverzeichnisses und die Einleitung des Buches "Betriebssysteme kompakt".

## Zusammenfassung

### Vorwort

Das Buch "Betriebssysteme kompakt" wurde geschrieben um dem Leser einen Überblick über die wichtigsten Aufgabenbereiche und Kernfunktionalitäten von Betriebssystemen zu geben. Die Programmbeispiele sind in der Programmiersprache C geschrieben und in den Betriebssystemen Debian GNU/Linux getestet. Betriebssysteme sind Schnittstellen zwischen der Hardware eines Computers und seinen Benutzern und deren Softwareprozessen. 

### Inhaltsverzeichnis

Im zweiten Kapitel werden die Repräsentationen von Zahlen, Datei und Speichergrößen und Informationsdarstellungen behandelt.

 Im dritten Kapitel finden sich Informationen bezüglich der Einordnung der Betriebssysteme in die Informatik, Positionierung und Kernfunktionalitäten von Betriebssystemen sowie ihre Entwicklung, diese kann man in ihre einzelnen Generationen einteilen. Betriebsarten sowie nähere Informationen zu  8/16/32/64 Bit-Betriebssystemen, Echtzeitbetriebssysteme, Verteilte Betriebssysteme, Architektur des Betriebssystemkerns und dem Schichten Modell werden ausführlich beschrieben. 

Das 4.te Kapitel behandelt die Grundlagen der Rechnerarchitektur welche man in folgende Rubriken unterteilen kann: Von-Neumann-Architektur, Ein-/Ausgabegeräte, Digitale Datenspeicher, Speicherhierarchie und RAID. 

Im Kapitel 5 widmet man sich der Speicherverwaltung. Themen wie Konzepte zu Speicherverwaltung, Speicheradressierung in der Praxis und Seitenersetzungsstrategien werden näher durchleuchtet. 

Da das 6. Kapitel Dateisysteme beschreibt, ist es nicht verwunderlich, dass die Technische Grundlagen der Dateisysteme, Blockadressierung bei Linux-Dateisystemen, Dateisysteme mit Dateizuornungstabellen, Journaling-Dateisysteme, Extent-basierte Adressierung, Copy-on-Write, Datenzugriffe mit einem Cache beschleunigen und die Defragmentierung  erklärt werden. 

Die Systemaufrufe im 7. Kapitel, kann man in Benutzermodus/Kernelmodus, Systemaufrufe/Bibliotheken und den Ablauf eines Systemaufrufs einteilen.

Bei der Prozessorverwaltung im 8. Kapitel sind die Prozesskontexte, Prozesszustände, die Struktur eines Prozesses im Speicher, das erzeugen von Prozessen mit fork, das ersetzen von Prozessen mit exec und der Prozesswechsel mit dem Scheduling von Prozessen äußerst wichtig hervorzuheben.

Die Interprozesskommunikation des 9. Kapitels enthält Kritische Abschnitte und Wettlaufsituationen, die Synchronisation von Prozessen, die Kommunikationen von Prozessen und die Kooperation von Prozessen

Im 10. und letztem Kapitel wird über die Virtualisierung geschrieben. Partitionierung, Hardware-Emulation, Anwendungs-Virtualisierung, Vollständige-Virtualisierung , Para-Virtualisierung und die Betriebssystem-Virtualisierung sind hierbei keine Fremdwörter

### Einleitung des Buches

Das Ziel des Buches ist es , den Leser ein grundlegendes Wissen über die Funktionsweise von Betriebssystemen und deren Komponenten zu vermitteln. Technische Vorkenntnisse sind nicht notwendig. In den Kapiteln 2 und 3  wird man in die Grundlagen der Informationstechnik und Betriebssysteme eingeführt. Mann muss zuers die notwendigsten Hardwarekomponenten verstehen, um die Arbeitsweise von Betriebssystemen nachvollziehen zu können. Kapitel 4 beschäftig sich mit der Grundlage der Rechnerarchitektur, kurz gesagt in welchen Verhältnissen die einzelnen Komponenten zueinander stehen. Das 5. Kapitel beschreibt die Speicherverwaltung und wie Caches und der Hauptspeicher verwalten werden. Das 6. Kapitel beschreibt die technischen Grundlagen von Dateisystemen. Kapitel 7 beschreibt die Arbeitsweise von Systemaufrufen. Die Prozessverwaltung ist eine der schwierigsten punkte, darauf fokussiert sich Kapitel 8. Im 9. Kapitel beschreibt man die Interprozesskommunikation. Im 10. Kapitel gibt es eine kurze Einführung in ein paar Virtualisierungskonzepten.

## Fragestellungen

* Versuche in einem kurzen Merksatz zu erklären, was ein Betriebssystem ist?
  * A: Ein Betriebssystem ist die Schnittstelle zwischen der Hardware eines Computers und seinen Benutzern und deren Softwareprozessen.

* Warum verwenden wir Betriebssysteme?
  * Um den Betrieb eines Computers zu steuern

*  Welche Betriebssysteme kennst du und mit welchen Betriebssystemen hast du schon gearbeitet?
  * A: Welche kennst du?
    * Windows
    * Linux
    * MacOS
    * Raspbarian
    * Android
  * A: Mit welchen hast du schon gearbeitet
    * Windows
    * Linux
    * Raspbarian
    * Android

* Für welche Art von Rechner wurden die ersten Betriebssysteme erfunden?
  * A: Für Großraumrechner wie dem System/360 

# Quellen

[1]"Was ist ein Betriebssystem?", *Datacenter-insider.de*, 2022. [Online]. Available: https://www.datacenter-insider.de/was-ist-ein-betriebssystem-a-682406/. [Accessed: 29- Mar- 2022].

[2]"Was ist ein Betriebssystem?", *It-business.de*, 2022. [Online]. Available: https://www.it-business.de/was-ist-ein-betriebssystem-a-673192/. [Accessed: 29- Mar- 2022].

[3]C.  Baun, *Betriebssysteme kompakt*, 2nd ed. Frankfurt am Main: Springer Verlag, 2020.