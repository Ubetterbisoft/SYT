

## Detaillierte Aufgabenbeschreibung

### 1. Der erste Container

![grafik](https://user-images.githubusercontent.com/78872776/228447985-dbc035db-fca0-4246-b8d3-68588ced288e.png)

![grafik](https://user-images.githubusercontent.com/78872776/228448329-45c6b745-18d7-420f-b9c6-0e9f1cca5613.png) 

* Wie kann dann der Dienst gestartet bzw. gestoppt werden?
  * Mit systemcl start oder stop, lässt sich der Dienst starten oder beenden

Liste dir nun alle aktiven und passiven Container in deinem System mit dem Befehl `docker ps -a` auf und analysiere den Output!

![grafik](https://user-images.githubusercontent.com/78872776/228449729-70e80532-4c74-462f-9a9c-61834ad97dbf.png)

* Es sind die Images hello-world enthalten und intelligent euclid. intelligent euclid ist inaktiv, hello-world active

### 2. Fertige Images und deren Einstiegspunkte

![grafik](https://user-images.githubusercontent.com/78872776/228453587-83e67db8-e4e6-4984-88b0-e9486aa1ba3b.png)

unter dem link http://localhost:3001/ghost gelangt man zum admin panel

![grafik](https://user-images.githubusercontent.com/78872776/228454396-f7ffa81e-27c1-48ed-a89a-e7a6a8da12ee.png)

Mann muss einfach einen neuen Post erstellen und den Instructions folgen

### 3. Images verwalten

![grafik](https://user-images.githubusercontent.com/78872776/228455539-d8473b94-ae6b-4fc5-9397-601d518d7473.png)



* Welche Informationen werden dabei angezeigt? 
  * Der Name des Repositorys, der Tag, die Image ID, das Erstellungsdatum des Images und die Speichergröße

Will man ein Image nur  herunterladen (ohne es gleich in einem Container zu verwenden), kann der Befehl `docker pull` verwendet werden.

![grafik](https://user-images.githubusercontent.com/78872776/228457694-1bb7f953-61a2-4041-a698-7a56db18a21f.png)

Prune:

Mit der Zeit und nach einigen Updates kann es zu einem doch recht großen Speicherverbrauch kommen. Um nicht benutzte Images nicht immer händisch entfernen zu müssen, bietet Docker eine kleine Option an: `docker image prune -a`

![grafik](https://user-images.githubusercontent.com/78872776/228458177-a0f53f1e-c5b3-45be-bb36-9c10a1c0e47c.png)

Um jedoch gezielt ein Image zu entfernen kann der Befehl `docker rmi hello-world:latest` eingegeben werden. Was passiert, wenn ein Container jedoch noch dieses Image benötigt? Welche anderen Optionen hat `docker image` noch zu bieten?

![grafik](https://user-images.githubusercontent.com/78872776/228458807-0386ba5f-731a-481c-8606-9c2b901012ce.png)

Wenn das image noch benötigt wird, erhält man eine fehlermeldung welche das löschen verhindert