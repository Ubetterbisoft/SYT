# GEK412 Analoge Signale - Kapazität und Induktivität

### Autor: Dejan Rajic

### Datum: 04.04.2022

## Einführung

Diese Ausarbeitung entstand im Rahmen eines schulischen Arbeitsauftrages. Es werden Informationen bezüglich Kapazität und Induktivität in diesem Dokument weitervermittelt und erklärt.

## Voraussetzungen

- Grundverständnis von Strom, Spannung und Zeit
- mathematisches Verständnis von Funktionen
- Grundverständnis von sinusförmigen Wechselgrößen



## Grundanforderungen

* Welche Kenndaten gibt es bei den Kondensator und den Spulen?
  * Kondensator: Kapazität, maximalen Spannung und Toleranz, Material des Dielektrikums
  * Spulen: Anzahl der Windungen, Durchmesser des Leiters, die Spulenlänge, Art des Kernmaterials, Induktivität in Henry und Maximale Strombelastbarkeit
* Welche Prinzipien stehen hinter diesen beiden Bauteilen?
  * A: Legt man an einen **Kondensator** im Gleichstromkreis eine Spannung an, so lädt er sich auf. Verbindet  man die Anschlüsse miteinander, so entlädt er sich. Durch den **Kondensator** hindurch fließt aber kein Strom. Er bildet im Gleichstromkreis einen unendlich großen Widerstand.
  * A: In einer **Spule** ist der  Leitungsdraht in sehr vielen Windungen übereinander gewickelt. Jede  einzelne Wicklungsschleife wirkt wie ein kreisförmiger Leiter. Die  einzelnen Magnetfelder, die jede der Wicklungsschleifen umgeben,  überlagern sich zu einem intensiven Gesamtfeld.
* Welche verschiedenen Bauformen gibt es?
  * A: Drehkondensatoren, Trimmkondensatoren, Plattenkondensator, Keramikkondensatoren, Elektrolytkondensatoren
  * A: Zylindrische Spule, Ringkernspule
* Wie berechnet man die Auf- und Entladezeit eines Kondensators?
  * t(volleladezeit) = C * R * 5 

#### Schaltung Tinkercad:

Baue eine Schaltung auf (z.B. mittels Tinkercad), die über einen  100kΩ Widerstand einen 10µF Elektrolytkondensator auflädt. Parallel dazu lege einen Kreis mit Taster oder Schiebeschalter und einer roten LED  mit einem Vorwiderstand von 4,7kΩ. Das ganze versorge bitte mit einer  Spannung von 30V. Beschreibe deine Beobachtung? Was musst du beim  Kondensator beachten? Verwende zur Analyse und Begründung deiner  Annahmen das Oszilloskop bzw. das Multimeter!

A:     ![grafik](https://user-images.githubusercontent.com/78872776/161542644-3c512e86-9512-41d8-9d29-264850c372a5.png) 

A: Der Kondensator hat sich voll aufgeladen und nimmt keine Energie mehr auf.

## Fragestellungen beim Abgabegespräch

### Grundlegend

- Was ist der Kondensator bzw. die Spule bei Gleichspannung?
  - Der **Kondensator** wirkt wie eine Sperre für den Gleichstrom.
  - Das Verhalten einer **Spule** im Gleichstromkreis ist somit vergleichbar mit dem Aufladen eines  Kondensators an einer Gleichspannungsquelle. Im Unterschied zum  Kondensator speichert die **Spule** die zugeführte Energie im Magnetfeld und der Kondensator im elektrischen Feld.

- Was ist 𝜏 (Tau) und wie kommt dieser Wert zum Einsatz?
  - Bei der **Zeitkonstanten** Tau  handelt sich um die Zeit, die ein Kondensator benötigt, um über den  Widerstand auf 63,2 % ( e-Funktion) der angelegten Spannung aufgeladen  zu werden. 5 Tau entspricht einer vollen Ladung.
- Wie lange braucht ein 10µF Kondensator bei einer Versorgungsspannung von 30V mit einem Widerstand von 100kΩ bis er ca. zu 86% geladen ist? ![grafik](https://user-images.githubusercontent.com/78872776/161539369-0e34183f-2088-4a2e-ba5e-31a6c0e617a1.png)
  - Nachdem 1 Farat und 1 Ohm = Tau = 1s
  - A:  2* 10mikrofarad * 100kohm = 2* tau , und zwei tau sind 86% Ladung demnach ist die dauer Ladung 2s lang


### Erweiterungen

#### Kapazität berechnen

- Einheiten **` A = PlattenFläche[m2], d = Plattenabstand[m], epsilon(Permittivität) = 8,85 * 10 hoch -12 [Permittirität][Farad/m2], c = Kapazität`**

- A: Kapazität berechnen: **``` c = A * epsilon/ d ```**

  

- "induktive und kapazitive Widerstände berechnen"

  - induktiv: xL(induktiver Widerstand) = ```2* pi * f * L``
  - kapazitiv: xc(kapazitiver Widerstand) = ```- 1 / 2 * pi * f * C``

  

- "induktive und kapazitive Widerstände erklären"

  - A:[1] Beim **induktiven Widerstand** wird elektrische Energie der Quelle in Energie des Magnetfeldes der Spule umgewandelt und umgekehrt. Beim kapazitiven **Widerstand** wird elektrische Energie der Quelle in Energie des elektrischen Feldes des Kondensators umgewandelt und umgekehrt.

- Wo liegen dabei die Unterschiede in der Leistungsaufnahme?

  - Der elektrische Widerstand der Spule ist im Wechselstromkreis wesentlich größer als im Gleichstromkreis. Ursache dafür ist die Selbstinduktion. Beim Kapazitven Widerstand hingegen, er verhindert nicht mehr den Stromfluss, sondern wirkt im Wechselstrom wie ein Widerstand weil er sich ständ auf und entläd.

## Quellen

[1] Ohmsche, induktive und kapazitive Widerstände im ...https://www.lernhelfer.de › physik-abitur › artikel › ohms...](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwjb9IDItaL2AhWFSvEDHdVYAmUQFnoECBsQAw&url=https%3A%2F%2Fwww.lernhelfer.de%2Fschuelerlexikon%2Fphysik-abitur%2Fartikel%2Fohmsche-induktive-und-kapazitive-widerstaende-im&usg=AOvVaw3O6p-BTnRQax85zVopkXBg)



[1]"Spule in Physik | Schülerlexikon | Lernhelfer", *Lernhelfer.de*, 2022. [Online]. Available: https://www.lernhelfer.de/schuelerlexikon/physik/artikel/spule. [Accessed: 05- May- 2022].

[2]"Spule / Spulen / Induktivität", *Elektronik-kompendium.de*, 2022. [Online]. Available: https://www.elektronik-kompendium.de/sites/bau/0207221.html. [Accessed: 05- May- 2022].https://www.hobbyelektroniker.ch/grundlagen/kondensatoren/

[3]D.  Mietke, "Kondensatoren in einer Typenübersicht", *Elektroniktutor.de*, 2022. [Online]. Available: https://www.elektroniktutor.de/bauteilkunde/c_bauf.html. [Accessed: 05- May- 2022].

[4]"Spule / Spulen / Induktivität", *Elektronik-kompendium.de*, 2022. [Online]. Available: https://www.elektronik-kompendium.de/sites/bau/0207221.htm. [Accessed: 05- May- 2022].

[5]"Spule / Spulen / Induktivität", *Elektronik-kompendium.de*, 2022. [Online]. Available: https://www.elektronik-kompendium.de/sites/bau/0207221.htm. [Accessed: 05- May- 2022].https://www.leifiphysik.de/elektrizitaetslehre/kondensator-kapazitaet/grundwissen/kondensator-und-kapazitaet

[6]*Youtu.be*, 2022. [Online]. Available: https://youtu.be/tTzkMqCkUf4?t=392. [Accessed: 05- May- 2022].

[7]*Youtu.be*, 2022. [Online]. Available: https://youtu.be/CAEqq7J9Ce4. [Accessed: 05- May- 2022].

[8]2022. [Online]. Available: https://de.universaldenker.org/formeln/458. [Accessed: 05- May- 2022].
