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
  * Kondensator: Kapazität, maximalen Spannung und Toleranz
  * Spulen: Anzahl der Windungen, Durchmesser des Leiters und Art des Eisenkern
* Welche Prinzipien stehen hinter diesen beiden Bauteilen?
  * A: Legt man an einen **Kondensator** im Gleichstromkreis eine Spannung an, so lädt er sich auf. Verbindet  man die Anschlüsse miteinander, so entlädt er sich. Durch den **Kondensator** hindurch fließt aber kein Strom. Er bildet im Gleichstromkreis einen unendlich großen Widerstand.
  * A: In einer **Spule** ist der  Leitungsdraht in sehr vielen Windungen übereinander gewickelt. Jede  einzelne Wicklungsschleife wirkt wie ein kreisförmiger Leiter. Die  einzelnen Magnetfelder, die jede der Wicklungsschleifen umgeben,  überlagern sich zu einem intensiven Gesamtfeld.
* Welche verschiedenen Bauformen gibt es?
  * A: Drehkondensatoren und Trimmkondensatoren
  * A: Zylindrische Spule, Flache Spule und Rechteckige Spule.
* Wie berechnet man die Auf- und Entladezeit eines Kondensators?
  * t(volleladezeit) = C * R * 5 

#### Schaltung Tinkercad:

Baue eine Schaltung auf (z.B. mittels Tinkercad), die über einen  100kΩ Widerstand einen 10µF Elektrolytkondensator auflädt. Parallel dazu lege einen Kreis mit Taster oder Schiebeschalter und einer roten LED  mit einem Vorwiderstand von 4,7kΩ. Das ganze versorge bitte mit einer  Spannung von 30V. Beschreibe deine Beobachtung? Was musst du beim  Kondensator beachten? Verwende zur Analyse und Begründung deiner  Annahmen das Oszilloskop bzw. das Multimeter!

A:     ![grafik](https://user-images.githubusercontent.com/78872776/161542644-3c512e86-9512-41d8-9d29-264850c372a5.png) 

​	

## Theorie

- "induktive und kapazitive Widerstände erklären"
  - A:[1] Beim **induktiven Widerstand** wird elektrische Energie der Quelle in Energie des Magnetfeldes der Spule umgewandelt und umgekehrt. Beim kapazitiven **Widerstand** wird elektrische Energie der Quelle in Energie des elektrischen Feldes des Kondensators umgewandelt und umgekehrt.

### EK SYT4 Elektrotechnik und Elektronik | Wechselspannung | analoge Signale

#### Kapazität berechnen

- Einheiten **` A = Fläche[m2], d = Plattenwiderstand[m], epsilon = 8,85 * 10 hoch -12 [Permittirität][Farad/m2], c = Kapazität`**

- A: Kapazität berechnen: **``` c = A * epsilon/ d ```**

  

- "induktive und kapazitive Widerstände berechnen"

  





### Fragestellungen beim Abgabegespräch

### Grundlegend

- Was ist der Kondensator bzw. die Spule bei Gleichspannung?
- Was ist 𝜏 (Tau) und wie kommt dieser Wert zum Einsatz?
  - MIt Tau kann man die Zeit berechnen in der Elektronische Bauteile (LED´S) mithilfe eines Kondensators Leuchten können.
- Wie lange braucht ein 10µF Kondensator bei einer Versorgungsspannung von 30V mit einem Widerstand von 100kΩ bis er ca. zu 86% geladen ist?![grafik](https://user-images.githubusercontent.com/78872776/161539369-0e34183f-2088-4a2e-ba5e-31a6c0e617a1.png)



## Quellen

[1] Ohmsche, induktive und kapazitive Widerstände im ...https://www.lernhelfer.de › physik-abitur › artikel › ohms...](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwjb9IDItaL2AhWFSvEDHdVYAmUQFnoECBsQAw&url=https%3A%2F%2Fwww.lernhelfer.de%2Fschuelerlexikon%2Fphysik-abitur%2Fartikel%2Fohmsche-induktive-und-kapazitive-widerstaende-im&usg=AOvVaw3O6p-BTnRQax85zVopkXBg)

Rechnung:

https://www.lernhelfer.de/schuelerlexikon/physik/artikel/spule

https://www.elektronik-kompendium.de/sites/bau/0207221.htm

https://www.hobbyelektroniker.ch/grundlagen/kondensatoren/

https://www.elektroniktutor.de/bauteilkunde/c_bauf.html

https://www.elektronik-kompendium.de/sites/bau/0207221.htm

https://www.leifiphysik.de/elektrizitaetslehre/kondensator-kapazitaet/grundwissen/kondensator-und-kapazitaet
