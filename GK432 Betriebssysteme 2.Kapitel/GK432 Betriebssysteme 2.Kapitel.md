# GK432 Betriebssysteme 2.Kapitel

### Autor: Dejan Rajic

### Veröffentlicht: 04.04.2022

## Zusammenfassung Kapitel 2

Im zweiten Kapitel geht es um die Grundlagen der Informationstechnik. Bits, die Repräsentation von Zahlen, Datei / Speichergrößen und die Informationsdarstellung werden dabei gut erklärt.

#### Bits

 Ein Bit ist die kleinstmögliche Einheit einer digitalen Information. Den Wert eines oder mehrerer Bits nennt man Zustand. Er wird durch zwei Zustände dargestellt (an und aus). Jedes zusätzliche Bit verdoppelt die Anzahl der möglichen darstellbaren Zustände.

#### Repräsentation von Zahlen

Für die IT sind die wichtigsten Stellenwertsysteme das Dezimal, Dual, Oktal und Hexadezimalsystem. Das Dezimalsystem verwendet als Basis die Zahl 10. Jede Ziffer D an der Stelle i hat den Wert D * 10 hoch i, zum Beispiel **2013 = 2 * 10 hoch 3 + 0 * 10 hoch 2 +1 10 hoch 1 + 3 * 10 hoch 0**. Beim Dualsystem verwendet man als Basis die Zahl 2. Zahlen werden nur mit den Ziffern der Werte Null und Eins dargestellt. Bei der Umwandlung von Dualzahlen in Dezimalzahlen werden die Ziffern mit ihren Stellenwertigkeiten ausmultipliziert und Ergebnisse addiert. Um eine Dezimalzahl in ein Dualzahl umzuwandeln, muss man die Dezimalzahl durch die Basis 2 dividieren und das Ergebnis der Division wird in der nächsten Runde erneut durch die Basis dividiert. Dies wiederholt man bis das Ergebnis der Division Null ist. Die Reste werden dann von unten nach oben als eine Zahl aufgeschrieben. Das Oktalsystem verwendet als Basis 8 und kann Gruppen von 3 Bits mit einem Zeichen darstellen. Bei der Umwandlung von Dualzahlen in Oktal zahlen wird die Bit kette vom niederwertigsten Bit beginnend in Dreiergruppen unterteilt. Jede Dreiergruppe entspricht einer Stele der Oktalzahl. Die Umwandlung von Oktal in binär funktioniert genau gleich nur umgekehrt. Das Hexadezimalsystem verwendet die Zahl 16. die Darstellung positiver Zahlen erfolgt mit 16 Ziffern und Buchstaben (0-9, A - F). Ein Zeichen kann eine Gruppe von 4 Bits darstellen. Die Umwandlung von Dual in Hexadezimal ist analog zu der des Oktalsystems, nur wird die Dualzahl in viererblöcke unterteilt. Die Umwandlung ist genau gleich, nur andersrum.

#### Datei und Speichergrößen 

Eine Datei ist eine beliebig lange Folge von Bytes und enthölt inhaltlich zusammengehörende Daten. Da sich die Größenordnungen der meisten Dateien in riesigen Bereichen befindet, gibt es verschiedene Größenordnungen. Es werden Zweierpotenzen von Bytes genutzt. Hier ein Paar Beispiele.

| Name      | Bytes     |
| --------- | --------- |
| Kilobyte  | 2 hoch 10 |
| Megabyte  | 2 hoch 20 |
| Terabyte  | 2 hoch 30 |
| Gigabyte  | 2 hoch 40 |
| Terabyte  | 2 hoch 50 |
| Exabyte   | 2 hoch 60 |
| Zettabyte | 2 hoch 70 |
| Yottabyte | 2 hoch 80 |

Beim Kaufen von USB Speichermedien werden jedoch Dezimal- Präfixe als Angabe benutzt. Mit jeder weiteren Maßeinheit (PB, EP, ZB) wächst der Kapazitätsunterschied zwischen Zweierpotenzen und Zehnerpotenzen weiter an.

#### Informationsdarstellung

Die ACII Kodierung ist eine 7-Bit Teichenkodierung welche 256 Zeichen umfasst. Es gibt auch nicht sichtbare Zeichen wie z.B Backspace, Carriage Return welche auch als Steuerzeichen bezeichnet werden. Um Probleme durch unterschiedliche Zeichenkodierungen in Zukunft zu vermeiden, wurde Unicode entwickelt. Diese wird laufend erweitert und soll in Zukunft alle bekannten Schriftzeichen enthalten. Der beliebteste Standard ist UTF-8. Um einen Text zu kodieren, werden die einzelnen Zeichen zu einer Zeichenkette (String) aneinandergefügt. Die Zeichen werden alle durch die Dezimalzahlen der Zeichennummern der ASCII-Tabelle ersetzt. Mann kann sie auch als hexadezimal angeben. Anschließend werden sie in Dualzahlen  konvertiert und man erhält eine Bitfolge

## Fragestellungen

-  Welche Beispiele fallen dir ein um ein Bit zu erklären? Was kann eine Datenmenge von 1 Bit darstellen?
  - A: Zwei Zustände (an, aus). Zum Beispiele Lampe an, Tür offen oder Tür zu.
-  Wo kommt das Oktalsystem zum Einsatz?
  - A:Oktalzahlen werden heute noch  bei der Darstellung von Dateizugriffsrechten unter Unix verwendet, wo je drei Bit die Rechte einer Benutzerklasse darstellen
-  Wo wird das Hexadezimalsystem verwendet? 
  - A: Um eine Farbe darzustellen. Für jede Farbe wird ein Byte genommen. ein Byte kann man als Bit schlecht lesen, desshalb benutzt man das hexadezimal System
-  Was war der ursprüngliche Einsatz der ASCII-Kodierung? 
  - A: Sie wurde ursprünglich für Fernschreiber benutzt.
-  Was ist der Unterschied zwischen der ASCII- und der Unicode-Kodierung?
  - A: Unicode ist eine Erweiterung von ASCII und es enthält Chinesische, Japanische und Sonderzeichen.
-  Was macht das Unicode-Konsortium? 
  - A: einmal im Jahr beschließt es welche neuen Zeichen im Unicode aufgenommen werden.

# Quellen

 [1]  Wikipedia contributors, „Oktalsystem“, *Wikipedia, The Free Encyclopedia*. [Online]. Verfügbar unter: https://de.wikipedia.org/w/index.php?title=Oktalsystem&oldid=216330785. 

[3] C. Baun, *Betriebssysteme kompakt*, 2nd ed. Frankfurt am Main: Springer Verlag, 2020.
