# GEK621 Sensoren und Aktoren gemeinsam einsetzen

### Grundlegend

- **Wie funktioniert der eingesetzte Ultraschall-Entfernungssensors (HC-SR04)? Welche Faktoren sind dabei zu beachten?**

  - Der Sensor HC-SR04 dient der Entfernungsmessung im Bereich zwischen 2cm und 3m. Er benötigt nur 5V Spannung und <2mA. Nach Triggerung misst das Modul selbständig die Entfernung und wandelt diese in ein PWM Signal um. Ein Messintervall dauert 20ms, daher ergibt sich das nur 50 Messungen pro Sekunde getätigt werden können.
  - Bei diesem Sensor muss man auf die Temperatur der Luft achten, da sich die Laufzeiten um 3,4% unterscheiden. Bei Verwendung im Freien ist eine Temperaturkompensation zu berücksichtigen

- **Was ist ein Aktor? Was ist eine Regelgröße? Nenne Beispiele?**

  - Ein Aktor ist ein Bauelement das elektrische Signale in mechanische Bewegung oder in andere physikalische Größen umsetzt. Sie stellen das Gegenteil zu Sensoren dar, die auf mechanische Bewegung mit elektrischen Impulsen reagieren.
  - Rolltreppe
  - Elektromotor
  - Lautsprecher
  - LED
  - Eine Regelgröße für Aktoren ist eine Größe, die durch eine Regelung oder Steuerung beeinflusst wird, um die Aktorleistung zu optimieren oder zu  verbessern. Die Regelgröße kann je nach Art des Aktors variieren und  hängt davon ab, welche Leistung das System erreichen soll. Bei einem Elektromotor wäre das z.B die Drehzahl.

  

- **Wie funktioniert der Servo Motor? Worauf ist bei der Verwendung zu Achten?**

  - **Ein Servo** besteht aus einer Motorsteuerung, einem Elektromotor,  einem Getriebe und einem Potentiometer zur Positionsbestimmung.  Alle Komponenten sind in einem robusten Gehäuse untergebracht. Angeschlossen wird er über ein dreipoliges Kabel. Dabei handelt es  sich um zwei Versorgungsleitungen (Plus und GND) und um eine  Datenleitung. Bei einem  Servoantrieb wird die Drehposition der Motorwelle über einen  Drehwinkelsensor ermittelt. Diese aktuelle Position der Welle (bzw. des  Rotors) wird fortlaufend an den Servoregler übertragen. In der  Servoelektronik wird dann die aktuelle Rotorposition mit der  Sollposition verglichen.

  - **Montage und Einbau:** Servomotoren sind in der Regel empfindlicher als andere Motoren und erfordern eine sorgfältige Montage und Einbau. Es ist wichtig, dass der Servomotor richtig montiert und ausgerichtet wird, um Vibrationen und unerwünschte Belastungen zu minimieren.

    **Stromversorgung:** Servomotoren erfordern normalerweise eine präzise Stromversorgung mit einer stabilen Spannung und einer ausreichenden Stromversorgung. Es ist wichtig sicherzustellen, dass die Stromversorgung den Anforderungen des Servomotors entspricht und ausreichend dimensioniert ist.

    **Überlastschutz: Servomotoren** sind empfindlicher gegenüber Überlastungen und können bei Überlastung oder Blockierung beschädigt werden. Es ist wichtig, dass das System über einen Überlastschutz verfügt, um eine Beschädigung des Servomotors zu verhindern.

    

    

- **Was für ein Signal wird verwendet um einen Servo zu steuern? Wie ist das aufgebaut? Wo wird es noch verwendet?**

  - Im Servo wird typischerweise durch ein Signal namens PWM  (Pulsweitenmodulation) gesteuert. Das PWM-Signal ist eine Art  elektronisches Signal, das aus einer Serie von Impulsen besteht. Die  Breite jedes Impulses bestimmt, auf welchem Winkel sich der Servo  ausrichtet. Das Signal wird normalerweise von einem Mikrocontroller  erzeugt und an den Servo gesendet, der dann entsprechend ausgerichtet  wird. PWM-Signale werden nicht nur zur Steuerung von Servos verwendet, sondern auch in vielen anderen elektronischen Anwendungen wie z.B Motorsteuerung, LED-Steuerung und zur Regelung von Spannung und Strom.

- **Was muss bei der Verarbeitung der Sensordaten beachtet werden?**

  - Bei der Verarbeitung von Sensordaten ist es wichtig, auf Genauigkeit,  Signalverarbeitung, Datenanalyse, Datenvisualisierung und Datenschutz zu achten. Die Messungen sollten so genau wie möglich sein, und die Daten  müssen gefiltert und korrekt verarbeitet werden, um genaue Ergebnisse zu erzielen. Die Ergebnisse sollten in einer verständlichen Form  präsentiert werden, um eine leichte Interpretation zu ermöglichen.  Datenschutz- und Sicherheitsrichtlinien müssen eingehalten werden, um  die Vertraulichkeit der Daten sicherzustellen.

- **Wie können Fehler bzw. Ausreißer erkannt und ausgebessert werden?**

  - Um Fehler oder Ausreißer in Sensordaten zu erkennen und zu korrigieren,  können Methoden wie statistische Analyse, Filterung, Kalibrierung,  Überprüfung von Grenzwerten und Machine Learning eingesetzt werden. Die  Wahl der Methode hängt von der Art der Daten und Anforderungen ab. Eine  sorgfältige Analyse der Daten ist wichtig, um genaue Ergebnisse zu  erhalten. Durch Hoch / Tiefpässe kann unerwünschtes Rauschen unterdrückt werden.

    

- **Wie kann Interpolation helfen Servo Bewegungen ruhiger zu machen?**

  - Interpolation kann helfen, Servo-Bewegungen ruhiger und flüssiger zu  machen, indem sie zwischen zwei oder mehr Punkten interpoliert, um eine  kontinuierliche Bewegung zu erzeugen. Durch die Verwendung von  Interpolationstechniken wie Linear- oder Spline-Interpolation können  abrupte Änderungen in der Servobewegung vermieden werden, was zu einer  sanfteren und natürlicheren Bewegung führt. Dies ist insbesondere bei  Servos wichtig, die in Anwendungen wie Robotik, CNC-Maschinen und  Automatisierung eingesetzt werden, um präzise und reibungslose  Bewegungen zu gewährleisten.

### Erweitert

- **Was ist eine Hysterese/ein Schmitt-Trigger?**
  - Ein Schmitt-Trigger ist eine **Schaltung mit Operationsverstärker, der als Komparator mit Hysterese arbeitet**. Hierbei macht man sich die Eigenschaften einer Kippschaltung zu nutze,  bei der die Ausgangsspannung bei bestimmten Eingangsspannungen schaltet.
  - Hysterese, auch Hysteresis, ist eine Änderung der Wirkung, die verzögert gegenüber einer Änderung der Ursache auftritt.
- **Was ist ein Regelkreis? Was sind mögliche Anwendungen dafür?**
  - Als Regelkreis wird der dynamische Wirkungsablauf zwischen Regler  und Regelstrecke zur Beeinflussung der Regelgröße y(t) in einem  geschlossenen System bezeichnet, bei dem diese Größe fortlaufend  gemessen und mit der Führungsgröße w(t) verglichen wird.
- **Wie funktioniert die Rückkopplung im Regelkreis?**
  - Ziel der negativen Rückkopplung ist die Stabilisierung einer bestimmten Größe innerhalb des Regelkreises. Eine negative Rückkopplung liegt immer dann vor, wenn das Endprodukt im  Regelkreislauf inhibitorisch, also hemmend, auf das Produkt wirkt,  welches am Anfang der Reaktionskette steht.

# Quellen

"Ultraschall Messmodul HC-SR04" mikrocontroller.net [online](https://www.mikrocontroller.net/attachment/218122/HC-SR04_ultraschallmodul_beschreibung_3.pdf)

“Was Sind Aktoren? smart home-lexikon,” *Was sind Aktoren? Smart Home-Lexikon*. [Online]. Available: https://www.wertgarantie.de/lexikon/technik/aktoren. [Accessed: 03-Mar-2023]. 

“Servomotor Einfach Erklärt!,” *CNC Blog*. [Online]. Available: https://www.precifast.de/servomotor-funktion-ansteuern-anschliessen/. [Accessed: 03-Mar-2023]. 

S. Hermann, “So Steuert man einen servo mit Arduino – Inklusive Code und schaltung,” *Arduino Tutorial*, 22-Jul-2021. [Online]. Available: https://starthardware.org/servo/. [Accessed: 03-Mar-2023]. 

“Servomotor,” *Wikipedia*, 07-Feb-2021. [Online]. Available: https://de.wikipedia.org/wiki/Servomotor. [Accessed: 03-Mar-2023]. 

“Pulsdauermodulation,” *Wikipedia*, 25-Oct-2022. [Online]. Available: https://de.wikipedia.org/wiki/Pulsdauermodulation. [Accessed: 03-Mar-2023]. 

A. Bekker, “Das 'warum', Das 'wann' und das 'wie',” *Die Analyse von Sensordaten in der Produktion*, 19-Jul-2022. [Online]. Available: https://www.scnsoft.de/blog/analyse-von-sensordaten. [Accessed: 03-Mar-2023]. 

B. S. GmbH, “Hysterese,” *Hysterese - SHKwissen*, 18-Dec-2019. [Online]. Available: https://www.haustechnikdialog.de/SHKwissen/586/Hysterese. [Accessed: 03-Mar-2023]. 

“Rückkopplung,” *Rückkopplung - Funktion, Aufgabe & Krankheiten | MedLexi.de*. [Online]. Available: https://medlexi.de/R%C3%BCckkopplung. [Accessed: 03-Mar-2023]. 