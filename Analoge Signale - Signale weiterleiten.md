# Analoge Signale - Signale weiterleiten

### Autor: Dejan Rajic

### Datum: 30.05.2022

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

* Funk: Mit der neuen 5G Technologie ist es möglich Geschwindigkeiten von bis zu 10GBits/Sekunde zu
  erzielen.
* Mit Kupferkabeln können maximale Geschwindigkeiten von mehreren GBits/Sekunde erreicht
  werden
* Licht: Mit Lichtwellenleitern können Übertragungsgeschwindigkeiten von bis zu mehreren
  Terabits/Sekunde erreicht werden.

##### Wie wird ein Medium für mehrere Teilnehmer eingesetzt?

* Weil ein Medium in vielen Fällen von beiden Seiten benutzt wird gibtes verschiedene Methoden zur gleichzeitigen Verwendung. Darunter Zählen Simplex, Halbduplex, Duplex, Symmetrische und asymmetrische Übertragung

##### Welche Vermittlungstechniken stehen dabei zur Verfügung?

* Leitungsvermittlung
* Paketvermittlung

##### Was versteht man unter Duplexing und asymmetrischerr bzw. symmetrischer Übertragung?

* Beim Duplex kann gleichzeitig übertragen und empfangen werden. Von Vollduplex spricht man, wenn es zwei Leiter zur Übertragung gibt, wovon einer zum Empfangen dient und der andere zum Senden.
* Symmetrische und asymmetrische Übertragung Bei der symmetrischen Datenübertragung sind im Übertragungsmedium Adernpaare, die beide ein Signal tragen, wobei die eine Ader beispielsweise das Ursprungssignal trägt und die andere das gleiche, nur mit entgegengesetzter Polarität, wodurch sich die Störsignale gegenseitig auslöschen. Die Asymmetrische Übertragung ist entsprechend das Gegenteil, also wird hier keine Ader mit
  verkehrter Polarität verwendet

##### Welche Verfahren sind hier verbreitet?

* Simplex: 
  Bei Simplex ist eine Übertragung nur in eine Richtung möglich. Beispiele dafür sind Fernsehen
  und Radio.
* Halbduplex:
  Beim Halbduplex teilen sich die beiden Seiten einen Leiter. Um das Gefühl einer gleichzeitigen
  Übertragung zu erzeugen, wird der Leiter immer für einen kurze Zeit in eine Richtung genutzt,
  und kurz danach wieder in die andere
* Duplex: Beim Duplex kann gleichzeitig übertragen und empfangen werden. Von Vollduplex spricht man, wenn es zwei Leiter zur Übertragung gibt, wovon einer zum Empfangen dient und der andere zum Senden.

##### Wie kommen Hoch, Tief bzw. Bandpässe zur Anwendung?

![image-20220602151314074](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220602151314074.png) 

**Tiefpass: **

Dadurch dass der Kondensator parallel zu Ua liegt entscheidet der Spannungsabfall an ihm die Spannung Ua. Ist nun also eine hohe Frequenz vorhanden, so ist der Blindwiderstand relativ klein und es ist fast kein Spannungsabfall vorhanden und dadurch ist Ua ebenso klein. Sollte nun eine niedrige Frequenz vorliegen, so ist der Spannungsabfall groß und Ua ist entsprechen groß.



**Hochpass:** 

Ein ähnliches Prinzip beschreibt auch den Hochpass der Unterschied ist nur, dass der fixe Widerstand und der Kondensator vertauscht sind. Da gilt Ue =  Uc + UR ist bei einer hohen Frequenz UR groß und hat dadurch einen hohen Spannungsabfall und Ua ist entsprechend groß. Bei niedriger Frequenz ist UR kleiner und Ua folgend klein.

![image-20220602151525796](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220602151525796.png) 

**Bandpässe:** 

Entstehen durch eine Kombination der beiden Pässe. Die Grenzfrequenz ist der Punkt, bei dem der Hochpass alle tieferen Frequenzen als die Grenzfrequenz dämpft und der Tiefpass alle Frequenzen höher als die Grenzfrequenz dämpft.

##### Wie kann zum Beispiel ein Tiefpass helfen das schnelle Drücken eines Tasters zu entschärfen?

Um das schnelle drücken eine Tasters zu dämpfen kann ein Tiefpass verwendet werden. Ist die Grenzfrequenz beispielsweise 4hz so ergibt sich daraus 

![image-20220602153517355](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220602153517355.png) 

R und C können verändert werden, solange das Produkt gleich bleibt Reelle Größen für dieses Beispiel wären: R=2*104Ω und C=2*10-5F=20μF

## Erweitert

**Wenn die Bandbreite und die Übertragungsqualität verbessert werden soll  müssen bestimmte Verfahren eingesetzt werden, um dies auch  kostensparend umsetzen zu können. Welche Multiplexing-Verfahren werden hier eingesetzt?**

* 

**In der Nachrichtentechnik wird der Begriff Modulation verwendet, um welche Vorgänge zu beschreiben?**

* Es beschreibt das Informationen in Elektrische Signale umgewandelt werden, damit man sie übertragen kann.

**Welche drei Parameter werden dabei angepasst?**

* Amplitude, Frequenz und Phase

**Welche Unterschiede werden bei analogen und digitalen Signalen getroffen?**

* Analoges Modulationssignal bedeutet, dass das Informationssignal eine  typisch analoge sinusförmige Signalform hat. Digitales Modulationssignal bedeutet, dass das Informationssignal eine typisch digitale  rechteckförmige Signalform hat. Es werden alle Werte die nicht 0 oder 1 sind weggelassen bei der digitalen.

**Wie berechnet man die Grenzfrequenz eines Tiefpassfilters?**

![image-20220602155113405](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220602155113405.png) 

**Baue eine Schaltung auf, die nur 1 kHz *"durchlässt"*, und höhere Frequenzen filtert. Verwende dabei Tinkercad zur Überprüfung deiner Berechnung.**

![image-20220602160508314](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220602160508314.png) 

## Fragestellungen

### Grundlegend

- Welche Medien werden zur Übertragung von Daten in der modernen  Telekommunikation verwendet? Was sind dabei die wichtigen  Charakteristika?
  - Bei der modernen Telekommunikation wird  in der Regel Kabel oder Funktechnik verwendet.
- Welche Übertragungsgeschwindigkeiten werden bei den einzelnen Medien erzielt?
- Welche Einteilungen gibt es bei der Vermittlungstechnik?
  - An wen die Nachricht geht
- Welche Duplexingarten gibt es? Wo liegen hier die Unterschiede?
  - 
  - Asymmetrische Übertragung
    - Downlink und uplink ist höher als das andere
  - Symmetrische Übertragung
    - Down & uplink sind gleich hoch
  - Simplex
    - nur eine Richtung Fernsehen
  - Vollduplex
    - Bei Vollduplex erfolgt die übertragung zur gleichen Zeit in beide Richtungen
  - Halbduplex
  - Echokompensation
    - man kann senden in beide richtungen auf der gleichen frequenz und das eigene signal wird als erwartetes eche abgezogen von dem was wird kriegen. man zieht das was wir gekrigt haben von dem was gesendet wurd ab.	
  - Dublexabstand 
    - Der Abstand zwischen Hin- und Rückkanal wird als Duplexabstand bezeichnet.
- Wie unterscheiden sich die einzelnen Frequenzfilter?

### Erweitert



# Quellen

https://www.elektronik-kompendium.de/sites/kom/0811081.htm

https://praxistipps.chip.de/2g-3g-4g-und-5g-einfach-erklaert_41254

https://www.swisscom.ch/de/magazin/digitalisierung-im-alltag/kupfer-auf-speed/

http://www.dsl-ratgeber.net/neuer-rekord-bei-glasfaser-737-terabit-pro-sekunde.html