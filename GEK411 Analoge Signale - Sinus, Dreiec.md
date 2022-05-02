# GEK411 Analoge Signale - Sinus, Dreieck, Rechteck und Sägezahn

### Autor: Dejan Rajic

### Datum: 3.3.2022

## Einführung

In dieser Dokumentation wird erläutert wie man analoge und digitale Signale unterscheiden und erklären kann. Ebenso werden sinusförmige Wechselgrößen und deren mathematische Zusammenhänge erklären in diesem Kapitel ein großer Bestandteil sein. Man kann nicht alles mit Gleichstrom lösen. Wir schauen uns an wie die Änderung von Zuständen für die Informationsweitergabe in verschiedenen Umgebungen umgesetzt werden kann.

## Theorie

### Detaillierte Aufgabenbeschreibung

Erkläre kurz, welche verschiedenen Arten von Informationen du im Alltag häufig benutzt. Wie können diese elektrisch verarbeitet werden?

A:` Unter alltägliche informationen versteht man z.B sehen (Optisch), hören(Akustisch) und tasten bzw fühlen(Wärme). Analoge und Digitale Informationen. Um ein Analoges Signal in ein digitales umzuwandeln, muss man einen Sensor an das digitale gerät anschließen und die konstanten analogen Werte zu bestimmten zeiten abtasten. Diese können dann digital dargestellt werden. Dadurch ergibt sich ein kleiner teil an informationen die nicht mehr benutzt werden.  `

#### Analog:

Analoge signale kommen in der natur vor bzw "echten Welt" vor. Ein Beispiel wäre das Quecksilber Termomether. Analoge signale sind konstant (die kurve ist rund). Es können unendlich viele werte dazwischen angenommen werden.

#### Digital:

Digitale signale kommen bei Computern vor. Diese sind diskret das bedeutet, dass die Kurve eckig ist. Der Wert der Y-Achse kann nur zu bestimmten zeitpunkten abgetastet werden. Es können keine Werte zwischen zwei punkten  angenommen werden.

#### Klassifizierung von Signalen:

Kenndaten periodischer Signale:

* Periodendauer
* Frequenz
* Amplitude
* Gleichwert
* Gleichrichtwert
* Effektivwert
* Crestfaktor
* Formfaktor

Es gibt kontinuierliche und diskontinuierliche Signale. Das bedeutet das es sich vier typen daraus ergeben.
* Analog-Kontinuierlich: ` Der Wert ist kontinuirlich und kann zwischen zwei Punkten jeden erdenklichen Wert annehmen`
  * ![grafik](https://user-images.githubusercontent.com/78872776/165945531-3153f13d-8a1a-411a-9bb3-ff36bd7117d1.png)


* Diskret-Kontinuierlich: `Die Y Achse also den Wert kann man nur zwischen definierten Punkten nehmen, jedoch kann man ihn nur zu jeder Zeit abfragen`
  * ![grafik](https://user-images.githubusercontent.com/78872776/165945661-d2cd6009-ce1a-41fd-8ceb-8cef19366546.png) 

* Analog-Diskontinuierlich: `Die Y Achse kann jeden Wert annehmen, die Zeit also die x-Achse nur bestimmte Werte in einen vorgegebenen Takt`
  * ![grafik](https://user-images.githubusercontent.com/78872776/165945811-581c7a51-4c67-4438-8c4e-2fbaba7815a2.png) 

* Diskret-Diskontinuierlich: `Der wert wird nur zu Bestimmten definierten Punkten in einen Vorgegebenen Takt ermittelt.`
  * ![grafik](https://user-images.githubusercontent.com/78872776/165945896-c8883be3-6017-4e7f-b1da-1139aec177e9.png) 


#### Genauere Analyse des Sinus

Der Sinus ist eine Analog-konstante Funktion bei der die Periodizität ein Pi ist. Die Sinusfunktion kommt überall häufig vor, wie zum Beispiel bei dem Wechselstrom. Man kann die Zeit in Sekunden angeben da der Wechselstrom in Eurupa eine Netzfrequenz von 50 Hz hat. In Sekunden wären das 50 Schwingungen in einem Diagramm.



 ## Fragestellungen beim Abgabegespräch

- Was ist der Unterschied zwischen Gleich- und Wechselspannung?

  - A: Bei der Gleichspannung läuft der Strom immer in die gleicher Richtung, bei der Wechselspannung Wechselt er immer die Richtung

- Was ist ein Signal? Welche Arten von Signalen gibt es?

  - A: Ein Signal ist ein Zeichen mit einer bestimmten Bedeutung, welches Informationen weitergeben soll

- Was ist die Kreisfrequenz und wie wird diese berechnet?

  ```
  ω = 2 · π · f
  
  Sie ist ein Maß dafür, wie schnell eine Schwingung abläuft.
  ```

- Was bedeutet der Begriff Effektivwert und wie kann er berechnet werden?

 ```
Unter dem Effektivwert wird in der Elektrotechnik der quadratische Mittelwert einer zeitlich veränderlichen physikalischen Größe verstanden.

Mann kann den Effektivwert bei einem Sinusförmigen Signal ausrechnen:
U(effektivwert) = U'(Amplitude/Spitzenwert) / wurzel von 2
 ```
Die Allgemeine Formel:

![image-20220303143606683](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220303143606683.png) 

* Wie wird die Wellenlänge "Lamda" berechnet?

​	` Lamda = c(Lichtgeschwindigkeit) / f(frequenz)` 

## Erweiterte Kompetenz

### Berechnung Analog Kontinuierlich (Sinus)

![image-20220303145444183](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220303145444183.png) 

`Ueff = U´ / Wurzel von 2 = 5 / Wurzel von 2 = 1,41 V `

### Berechnung Rechtecks Spannung

![image-20220303145822282](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220303145822282.png) 

`Ueff = U´`

`Ueff = 5V`

### Berechnung Dreiecks Spannung

![image-20220303145945684](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220303145945684.png) 

`Ueff = U´ / Wurzel von 3 = 5 / Wurzel von 3 = 2,88 V `

### Berechnung Sägezahn Spannung

![image-20220303150131479](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220303150131479.png) 

`Ueff = U´ / wurzel von 3 = 2,88 V`

#### Fragen:

* Wieso ist bei der Wechselspannung der Sinus so weit verbreitet? 
  * Spannung und Stromstärke müssen nicht unbedingt den zeitlichen Verlauf einer Sinusfunktion besitzen. Allerdings ist sinusförmige Wechselstrom  technisch am weitesten verbreitet, da er bei der Stromgewinnung in  Wechselstromgeneratoren entsteht.

​	

* Welche  Gründe gibt es für den Einsatz der Wechselspannung in der  Energietechnik?
  * Muss elektrische Energie über große Entfernungen übertragen werden, wird **Wechselstrom** eingesetzt, weil dieser sich einfach auf hohe Spannungen transformieren lässt.



* Welche Signalform wird bei digitalen Übertragungsarten oft gewählt und wieso?
  * Analog diskontinuirlich, damit man eine größere Bandbreite an Werten einholen kann.

​	

* Welche Rolle spielt dabei der Crestfaktor
  * Der Scheitelfaktor oder Crest-Faktor beschreibt in der  Elektrotechnik das Verhältnis von Scheitelwert zu Effektivwert einer  Wechselgröße und ist immer größer oder gleich eins

# Quellen

* "Systemtechnik Theorie Unterlagen" elearning; zuletzt besucht 2020-02-15; [online](https://elearning.tgm.ac.at/course/view.php?id=1939)

* "Was ist der Unterschied zwischen analogen und digitalen Daten?" Digi4all - youtube; zuletzt besucht 2020-02-15; 

* Elektrotechnik in 5 Minuten - Klassifikation von Signalen" Alexander Stöger

* Elektrische Signale" elektroniktutor.de; zuletzt besucht 2020-02-15; [online](https://elektroniktutor.de/signalkunde/signdef.html)

* "Kenndaten periodischer Signale" elektroniktutor.de; zuletzt besucht 2020-02-15

* Digitale und analoge Signale – ein Vergleich" elektroniktutor.de; zuletzt besucht 2020-02-15

* Effektivwert" studyflix.de; zuletzt besucht 2020-02-15
