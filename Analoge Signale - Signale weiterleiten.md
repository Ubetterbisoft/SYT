# Analoge Signale - Signale weiterleiten

### Autor: Dejan Rajic

### Datum: 30.05.2022

## Einführung

In der Signalverarbeitung ist eine Weiterleitung von Informationen sehr wichtig. Auf welche Art und Weise können Informationen weitergeleitet werden und welche Medien bieten sich dafür an? Wie können mehrere Nutzer gleichzeitig an einer Leitung angeschlossen sein ohne Störungen bei der Übertragung zu verursachen. Diese und viele weitere Fragen werden in der folgenden Dokumentation beantwortet.

## Projektbeschreibung

In der folgenden Dokumentation werden wichtige und interessante Fragen über die Datenverarbeitung und Weiterleitung von Signalen beantwortet und behandelt. Die Dokumentation entstand im rahmen einer Schulischen Ausarbeitung. Ich habe die jeweiligen Fragen die in den verschiedenen Gliedern (Detailierte Aufgabenbeschreibung, Fragestellungen beim Abgabegespräch und die Erweiterten Fragestellungen) so gut  ich konnte mit meinen aktuellen Wissen beantwortet. Die Informationen auf die ich mich in dieser Ausarbeitung beziehe stehen sind alle in der Rubrik Quellen ersichtlich.



## Theorie

##### Welche verschiedenen Arten von Übertragungsmedien werden heutzutage verwendet um über weite Strecken Signale und Informationen zu versenden und zu empfangen ?

* Kupferkabel, Luft (Drahtlos) und Lichtwellenleiter

##### Wann werden diese bevorzugt eingesetzt und was sind deren Haupteigenschaften?

* A: Bei der drahtlosen Datenübertragung werden elektromagnetische Wellen genutzt, um ohne ein Medium über kleinere Strecken Daten zu übertragen. Die drahtlose Datenübertragung wird aufgrund der Inkonsistenz der Bandbreite und der Reichweite fast nur für mobile Geräte ohne verpflichtenden Netzwerkkabelanschluss wie Smartphones, Laptops, Radios usw. genutzt. Mit der neuen 5G Technologie ist es möglich Geschwindigkeiten von bis zu 10GBits/Sekunde zu erzielen. Die elektromagnetischen Wellen werden mittels einer Antenne erzeugt und aufgenommen.

* A: Licht wird für Lichtwellenleiter verwendet. Lichtwellenleiter haben höhere übertragungsraten. Beim verlegen von Modernen Internetleitungen werden sie benutzt. Optische Signale aus Licht wandern durch das Kabel anstatt wie beim Kuper die Elektronen

* Kupferkabel Ist das am meisten verwendete Übertragungsmedium. Grundsätzlich gibt es zwei verschiedene Arten, die am meisten verwendet werden: Koaxialkabel, Patchkabel und Twisted-Pair Kabel. Koaxialkabel werden meist als Sekundär- und Tertiärverkabelung genutzt.
  Patchkabel dienen zur Verbindung von Endgeräten. Kupferkabel werden nicht über längere Strecken verwendet, da die Geschwindigkeit ziemlich
  schnell abfällt.

  

##### Welche Geschwindigkeiten werden dabei erzielt?

* [2]Funk: Mit der neuen 5G Technologie ist es möglich Geschwindigkeiten von bis zu 10GBits/Sekunde zu
  erzielen.
* [3]Mit Kupferkabeln können maximale Geschwindigkeiten von mehreren GBits/Sekunde erreicht
  werden
* [4]Licht: Mit Lichtwellenleitern können Übertragungsgeschwindigkeiten von bis zu mehreren
  Terabits/Sekunde erreicht werden.

##### Wie wird ein Medium für mehrere Teilnehmer eingesetzt?

* [5]Weil ein Medium in vielen Fällen von beiden Seiten benutzt wird gibtes verschiedene Methoden zur gleichzeitigen Verwendung. Darunter Zählen Simplex, Halbduplex, Duplex, Symmetrische und asymmetrische Übertragung

##### Welche Vermittlungstechniken stehen dabei zur Verfügung?

* Leitungsvermittlung
* Paketvermittlung

##### Was versteht man unter Duplexing und asymmetrischerr bzw. symmetrischer Übertragung?

* [1]Beim Duplex kann gleichzeitig übertragen und empfangen werden. Von Vollduplex spricht man, wenn es zwei Leiter zur Übertragung gibt, wovon einer zum Empfangen dient und der andere zum Senden.
* [1]Symmetrische und asymmetrische Übertragung Bei der symmetrischen Datenübertragung sind im Übertragungsmedium Adernpaare, die beide ein Signal tragen, wobei die eine Ader beispielsweise das Ursprungssignal trägt und die andere das gleiche, nur mit entgegengesetzter Polarität, wodurch sich die Störsignale gegenseitig auslöschen. Die Asymmetrische Übertragung ist entsprechend das Gegenteil, also wird hier keine Ader mit
  verkehrter Polarität verwendet

##### Welche Verfahren sind hier verbreitet?

* [5]Simplex: 
  Bei Simplex ist eine Übertragung nur in eine Richtung möglich. Beispiele dafür sind Fernsehen
  und Radio.
* Halbduplex:
  Beim Halbduplex teilen sich die beiden Seiten einen Leiter. Um das Gefühl einer gleichzeitigen
  Übertragung zu erzeugen, wird der Leiter immer für einen kurze Zeit in eine Richtung genutzt,
  und kurz danach wieder in die andere
* Duplex: Beim Duplex kann gleichzeitig übertragen und empfangen werden. Von Vollduplex spricht man, wenn es zwei Leiter zur Übertragung gibt, wovon einer zum Empfangen dient und der andere zum Senden.

##### Wie kommen Hoch, Tief bzw. Bandpässe zur Anwendung?

![image-20220603100225347](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220603100225347.png) 

**Tiefpass: **

[5]Dadurch dass der Kondensator parallel zu Ua liegt entscheidet der Spannungsabfall an ihm die Spannung Ua. Ist nun also eine hohe Frequenz vorhanden, so ist der Blindwiderstand relativ klein und es ist fast kein Spannungsabfall vorhanden und dadurch ist Ua ebenso klein. Sollte nun eine niedrige Frequenz vorliegen, so ist der Spannungsabfall groß und Ua ist entsprechen groß.



**Hochpass:** 

[5]Ein ähnliches Prinzip beschreibt auch den Hochpass der Unterschied ist nur, dass der fixe Widerstand und der Kondensator vertauscht sind. Da gilt Ue =  Uc + UR ist bei einer hohen Frequenz UR groß und hat dadurch einen hohen Spannungsabfall und Ua ist entsprechend groß. Bei niedriger Frequenz ist UR kleiner und Ua folgend klein.

![image-20220603100314876](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220603100314876.png) 

**Bandpässe:** 

[5]Entstehen durch eine Kombination der beiden Pässe. Die Grenzfrequenz ist der Punkt, bei dem der Hochpass alle tieferen Frequenzen als die Grenzfrequenz dämpft und der Tiefpass alle Frequenzen höher als die Grenzfrequenz dämpft.

![image-20220603100402257](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220603100402257.png) 

##### Wie kann zum Beispiel ein Tiefpass helfen das schnelle Drücken eines Tasters zu entschärfen?

Um das schnelle drücken eine Tasters zu dämpfen kann ein Tiefpass verwendet werden. Ist die Grenzfrequenz beispielsweise 4hz so ergibt sich daraus 

 

R und C können verändert werden, solange das Produkt gleich bleibt Reelle Größen für dieses Beispiel wären: R=2*104Ω und C=2*10-5F=20μF

## Erweitert

**Wenn die Bandbreite und die Übertragungsqualität verbessert werden soll  müssen bestimmte Verfahren eingesetzt werden, um dies auch  kostensparend umsetzen zu können. Welche Multiplexing-Verfahren werden hier eingesetzt?**

* Raummultiplexverfahren
* Zeitmultiplexverfahren
* Frequenzmultiplexverfahren
* Codemultiplexverfahren

**In der Nachrichtentechnik wird der Begriff Modulation verwendet, um welche Vorgänge zu beschreiben?**

* Es beschreibt das Informationen in Elektrische Signale umgewandelt werden, damit man sie übertragen kann.

**Welche drei Parameter werden dabei angepasst?**

* Amplitude, Frequenz und Phase

**Welche Unterschiede werden bei analogen und digitalen Signalen getroffen?**

* Analoges Modulationssignal bedeutet, dass das Informationssignal eine  typisch analoge sinusförmige Signalform hat. Digitales Modulationssignal bedeutet, dass das Informationssignal eine typisch digitale  rechteckförmige Signalform hat. Es werden alle Werte die nicht 0 oder 1 sind weggelassen bei der digitalen. Bei der Analogen Modulation werden Analoge Signale in Digitale umgewandelt. Bei der Digitalen Modulation

**Wie berechnet man die Grenzfrequenz eines Tiefpassfilters?**

![image-20220603100542198](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220603100542198.png) 

**Baue eine Schaltung auf, die nur 1 kHz *"durchlässt"*, und höhere Frequenzen filtert**

<img src="C:\Users\draji\Downloads\tiefpass.PNG" alt="tiefpass" style="zoom: 33%;" /> 

Hochpass:

 <img src="C:\Users\draji\Downloads\hochpass.PNG" alt="hochpass" style="zoom:33%;" />

## Fragestellungen

### Grundlegend

- Wie unterscheiden sich die einzelnen Frequenzfilter?
  - Ein Hochpassfilter lässt nur Frequenzen durch die Höher sind als die Grenzfrequenz
  - Ein Tiefpassfilter lässt nur Frequenzen durch die Niedriger sind als die Grenzfrequenz
  - Ein Bandpassfilter dämpft alle Frequenzen die Niedriger und Höher als die Grenzfrequenz sin

### Erweitert

* Welche Multiplexing verfahren kommen in der modernen Telekommunikation zum Einsatz?

  * Raummultiplexverfahren
  * Zeitmultiplexverfahren
  * Frequenzmultiplexverfahren
  * Codemultiplexverfahren

* Welche Modulationsverfahren gibt es bei analogen und digitalen Übertragungsarten?

  * Frequenzanpassung
  * Mehrfachausnutzung des Übertragungsmediums
  * Erhöhung der Störsicherheit

* Was ist eine Grenzfrequenz und wie wird diese berechnet?

  * Die **Grenzfrequenz**  entspricht in der Elektro- und Nachrichtentechnik der Frequenz, ab der  die Amplitude eines Signals auf einen bestimmten Wert abfällt. 

  1. f=12⋅ π⋅R⋅C.
  2. R=12⋅ π⋅f⋅C.
  3. C=12⋅ π⋅f⋅R.



## Zusammenfassung

Abschließend lässt sich zusammenfassend sagen, dass Informationen übertragen werden müssen um von Punkt A zu Punkt B zu kommen. Dabei spielt die Auswahl des Übertragungsmediums eine entscheidende Rolle. Es gibt verschiedene Übertragungswege wie (Luft, Kabel, oder Licht). Jeder von ihnen hat seine Vor und Nachteile, sein es Kosten, Übertragungsgeschwindigkeit oder Reichweite. Ebenfalls kann man mit den verschiedenen Duplex varianten für ein gleichzeitiges Senden und Empfangen von Signalen sorgen. Bei der Symmetrischen  Synchronisation werden Adern paare im übertragungsmedium verwendet um Fehler mit einer entgegengesetzten Polarität zu vermeiden. Beim Symmetrischen wird keine entgegengesetzte Polarität verwendet. Tiefpässe lassen nur Frequenzen durch die unter einer Bestimmten Grenzlinie liegen. Hochpässe lassen sie nur durch wenn sie über der Grenzlinie liegen. 

# Quellen

[1]"Duplex und Duplexing (TDD FDD)", *Elektronik-kompendium.de*, 2022. [Online]. Available: https://www.elektronik-kompendium.de/sites/kom/0811081.htm. [Accessed: 03- Jun- 2022].

[2]"2G, 3G, 4G und 5G - einfach erklärt", *Praxistipps.chip.de*, 2022. [Online]. Available: https://praxistipps.chip.de/2g-3g-4g-und-5g-einfach-erklaert_41254. [Accessed: 03- Jun- 2022].

[3]"Kupferleitungen auf Speed | Swisscom Magazin", *Swisscom Magazin*, 2022. [Online]. Available:  https://www.swisscom.ch/de/magazin/digitalisierung-im-alltag/kupfer-auf-speed/. [Accessed: 03- Jun- 2022].

[4]"Neuer Rekord bei Glasfaser: 73,7 Terabit pro Sekunde - DSL-Ratgeber", *Dsl-ratgeber.net*, 2022. [Online]. Available:  http://www.dsl-ratgeber.net/neuer-rekord-bei-glasfaser-737-terabit-pro-sekunde.html. [Accessed: 03- Jun- 2022].

[5]"Übertragungstechnik", *Elektronik-kompendium.de*, 2022. [Online]. Available: http://www.elektronik-kompendium.de/sites/kom/1303291.htm. [Accessed: 03- Jun- 2022].

