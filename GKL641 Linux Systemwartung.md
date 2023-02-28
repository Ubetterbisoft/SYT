# GKL641 Linux Systemwartung

## 1. Installation von Webdienst

Welche Distribution verwendest du?

* Xubuntu

Welches Release ist in `/etc/apt/sources.list` eingetragen? Wie lange wird dieses Release noch mit Updates unterstützt? 

* Xubuntu 22.04.1 LTS_Jammy jellyfish_- Release amd64 (20220809.1)

Wie lange wird dieses Release noch mit Updates unterstützt?

* Bis April 2027

Was muss nach dem *End-of-life-date (EOL)* getan werden, um die installierte Distribution weiter verwenden zu können?

* Man muss die installierte Distribution aktualisieren, oder falls es keine Updates mehr gibt muss man die Distribution ändern

Welche Seite erscheint, wenn du danach auf deinem host die URL http://localhost:8080 ansurfst?

* Es kommt die Seite die wir in einer SYT Theorie Stunde eingerichtet haben. Darauf Steht der Vorname Nachname Klasse in einem <h1> -tag geschrieben

![grafik](https://user-images.githubusercontent.com/78872776/218975059-cc352ab9-5b26-4dea-b7bd-d500e9e980a4.png)

![grafik](https://user-images.githubusercontent.com/78872776/218975297-2effff6d-78d6-42a1-8894-79af4fa72cec.png)

![grafik](https://user-images.githubusercontent.com/78872776/220550286-597dc11d-2bcf-4437-b52b-02cbcb257f47.png)

![grafik](https://user-images.githubusercontent.com/78872776/220551880-ddb6a6c7-a180-4048-9f69-6173f568ac80.png)

## 2. Dienste verwalten

Verwende die befehle `systemctl stop apache2`, `systemctl start apache2` und `systemctl restart apache2` und verifiziere ob der Webserver funktioniert oder nicht.

#### Stop:

![grafik](https://user-images.githubusercontent.com/78872776/220553457-09062414-0535-41b9-b0a1-acc6296e5112.png)



![grafik](https://user-images.githubusercontent.com/78872776/220553807-26c26c1e-b843-4473-a058-45d06fc63cb4.png)

Der Webserver wurde erfolgreich nach Eingabe des Passworts und Befehls gestoppt.

![image-20230222084700201](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20230222084700201.png)

#### Start:

![grafik](https://user-images.githubusercontent.com/78872776/220554203-5c7929d0-6e7b-4b08-913f-1f4183594269.png)

![grafik](https://user-images.githubusercontent.com/78872776/220555856-59b6862a-548c-4871-b9af-b696664d0626.png)



wurde erfolgreich wieder gestartet

#### Restart:

![grafik](https://user-images.githubusercontent.com/78872776/220554827-67d556c4-f82f-456d-8b56-2c12c00e00ae.png)

Die HTML Datei wurde geändert und der Server restarted. Mit dem Restart wurden die Änderungen übernommen.

![grafik](https://user-images.githubusercontent.com/78872776/220555388-ebec56b8-3880-4ed3-af97-4d94ead6ed7b.png)



#### Status:

![grafik](https://user-images.githubusercontent.com/78872776/220555856-59b6862a-548c-4871-b9af-b696664d0626.png)

`systemctl statusapache2` gibt den Status des Webservers an

#### Dienste automatisch starten:

![grafik](https://user-images.githubusercontent.com/78872776/220558256-accdc25b-a020-4687-9003-942f8c1110dd.png)

Dabei wird unter `/etc/systemd/system/service-name` eine Verlinkung erstellt. Alles was in dem Pfad ist wird als prozess ausgeführt

## 3. Arbeitsspeicher und Systemresourcen

Du kannst dir unter Linux laufende Prozesse mit dem Kommando `ps` anzeigen lassen. Per default zeigt `ps` allerdings immer nur Prozesse, die unter deinem aktuellen Benutzer in  der aktuellen Konsole laufen. Wie viele Prozesse sind das bei dir?

* ![grafik](https://user-images.githubusercontent.com/78872776/220559723-34032089-fd95-4192-9fb1-dac61c1ef152.png)
* Es werden zwei Prozesse bash und ps ausgeführt

Um alle am System laufenden Prozesse anzeigen zu lassen, verwende die Option `ps ax`. Dies zeigt dir alle laufenden Prozesse von allen Benutzern. Wie viele  Prozesse verwendet der Apache Webserver? Wie kannst du dir zu den  Prozessen den Benutzer anzeigen lassen, unter dem sie laufen?

* ![grafik](https://user-images.githubusercontent.com/78872776/220560576-306811fe-2c3f-4841-8f1a-d65f77783d4e.png)

  Es werden drei Prozesse vom Webserver ausgeführt

* ![grafik](https://user-images.githubusercontent.com/78872776/220561337-e4d84724-b899-4815-b804-bafa3a83dab4.png)mit ps aux werden zu den Prozessen alle Benutzer angezeigt

  ![grafik](https://user-images.githubusercontent.com/78872776/220561724-8e9662da-bc6e-47ac-a4c0-4a1c398b7a88.png)

​				rot eingekreist die Benutzer

Um laufend die aktuellen Prozesse anzeigen zu lassen, gibt es das Tool `top`. Zu diesem gibt es aber eine komfortable Alternative namens `htop`. Installiere es auf deinem System und rufe `htop` auf. Zusätzliche zu den laufenden Prozessen siehst du oben am  Bildschirm noch weitere Systemanzeigen. Welche sind das? Warum zeigt `htop` z.B. für den Apache-Webserver mehr Prozesse an als `ps`?

![grafik](https://user-images.githubusercontent.com/78872776/220562602-7ff2a138-96c2-4bdb-932a-2102d820c258.png)



* SWP ist für den Auslagerungspeicher
* CPU zeigt die CPU Auslastung an
* MEM zeigt die Arbeitsspeicher Auslastung an

![grafik](https://user-images.githubusercontent.com/78872776/220564350-83459254-6d63-4cc9-badd-44998bfbe7ea.png)

Die Grünen Einträge sind Threads und keine Prozesse, desshalb werden mehr angezeigt als mit ps aux. Bei ps aux werden keine Threads angezeigt



Mittels `htop` lassen sich auch Prozesse beenden. Starte in einem neuen Reiter die Ausgabe von Zufallsbytes mit dem Befehl `cat /dev/urandom`. Finde diesen neuen, laufenden Prozess in `htop` und beende diesen mittels den möglichen Funktionen im Prozessbetrachter.

![grafik](https://user-images.githubusercontent.com/78872776/220565336-9c3d32dd-f90a-497d-8280-e4823df36d64.png)

![grafik](https://user-images.githubusercontent.com/78872776/220566298-0608cc6d-f88a-4ebd-ab59-9334cd7b2f51.png)

den Prozess auswählen, f9 drücken und anschließend im linken menü SIGKILL auswählen, damit wird der Prozess gekillt

## 4. Festplattenplatz

Recherchiere in der Manpage zu `du`, was diese beiden Optionen (-s, -c) bewirken und führe `sudo du -sch /var/log/*` aus. Was sagt dir die Ausgabe?

* -s "--sumarize", gibt nur eine Summe für jedes Argument an
* -c ""  gibt eine Gesamtsumme aus.
* Die Ausgabe zeigt mir alle Dateien die den Speicherplatz im Verzeichnis `sudo du -sch /var/log/*` verbrauchen und gibt sie im Human readable Format an.

![grafik](https://user-images.githubusercontent.com/78872776/220576472-68ecd968-cba7-48e9-b351-25a267186aef.png)

Mittels `df` lässt sich der noch freie Speicherplatz anzeigen (auch hier wird `-h` verwendet, um lesbare Größeneinheiten anzeigen zu lassen). Das Kommando `df -h <verzeichnis>` gibt dabei den für `<verzeichnis>` noch freien Speicherplatz an, das heißt, den freien Speicherplatz der Partition, auf der `<verzeichnis>` liegt. Was bewirkt ein Aufruf von `df -h` ohne Angabe eines Verzeichnisses?

* df -h gibt den Speicherplatz in menschenlesbarer Form auf allen Partitionen des Systems an ( also den verfügbaren Speicherplatz auf der gesamten VM)
* ![grafik](https://user-images.githubusercontent.com/78872776/220577730-19ef09b2-78ee-49e8-91ac-510ef3fcd00b.png)

## 5. Logdaten

Du kennst ja schon den Befehl `systemctl status` aus der  vorherigen Teilaufgabe. Du hast bemerkt, dass mit der Übergabe des  Service-Namen nur ein Teil der Logging-Information angezeigt wird. Wie  lassen sich nun alle Logdaten zu einem Service mittels `systemd` anzeigen? Wie unterscheiden sich diese Informationen zu denen im Verzeichnis `/var/log`?

* Um alle Logdaten zu einem Service mittels systemd anzuzeigen, kann der Befehl `"journalctl -u SERVICE_NAME"` verwendet werden. Dies zeigt alle Logeinträge für den angegebenen Service-Namen an. Wenn  der Befehl ohne Angabe eines Service-Namens verwendet wird, werden alle  Logeinträge für alle Services angezeigt
* Die Logdaten, die von systemd gesammelt werden, unterscheiden sich von  denen im Verzeichnis /var/log, da sie vom systemd-Journald-Dienst  gesammelt werden, anstatt von den individuellen Protokolldateien der  Dienste. Das Systemd-Journal ist ein zentralisiertes  Protokollierungssystem, das mehrere Protokolldatenquellen in einem  einzigen Protokoll vereint. Dies ermöglicht eine einfache und  zentralisierte Verwaltung von Protokolldaten sowie die Möglichkeit,  Protokolldaten auf einfache Weise nach bestimmten Kriterien zu  durchsuchen und zu filtern.
* ![grafik](https://user-images.githubusercontent.com/78872776/220581981-9ee5e6c2-7a89-4893-bbfc-9d96ca4eb81c.png)

Der englische Name *Journal*  lässt auf ein Protokoll oder Tagebuch schließen, wie kann dieses  durchsucht werden? Finde den Filter, der nur Logeinträge für das heutige Datum anzeigt!

* Um das Systemd-Journal zu durchsuchen, kann der Befehl "journalctl" verwendet werden. Um nur Logeinträge für das heutige Datum anzuzeigen, kann der Filter "- -since=today" verwendet werden. Der vollständige Befehl würde dann lauten:

  `"journalctl --since=today"`

## 6. Netzwerkverbindungen

Mit dem Kommando `netstat` lassen sich verschiedene Daten des Netzwerksubsystems anzeigen, wie z.B. die Routingtabellen `netstat -r` oder offene Sockets `netstat -l`. Da Sockets unter Unix-Systemen auch sehr häufig zur  Interprozesskommunikation zwischen Prozessen auf demselben Rechner  eingesetzt werden, ist die Ausgabe hier oft sehr unübersichtlich. Um  alle (und nur die) tcp-Verbindungen anzeigen zu lassen, werden oft die  Optionen `netstat -talp` zusammen verwendet. Führe dieses  Kommando in deiner VM aus, nachdem du die Webseite aus dem ersten  Schritt oben vom Host aus aufgerufen hast, und erkläre die Ausgabe. Wie  funktioniert dies für das Protokoll UDP?

* Konkret bedeutet dies, dass der Befehl "netstat -talp" alle offenen  TCP-Verbindungen anzeigt, sowohl zu lokalen als auch zu entfernten  Hosts, einschließlich der Listening-Sockets. Zusätzlich werden für jede  Verbindung der Prozessname und die Prozess-ID angezeigt.
* Die Ausgabe zeigt für jede TCP-Verbindung die lokale IP-Adresse und den  Port, die IP-Adresse und den Port des entfernten Hosts, den  Verbindungsstatus (z.B. "LISTEN" für Listening-Sockets oder  "ESTABLISHED" für aktive Verbindungen), sowie den Prozessnamen und die  PID, die die Verbindung geöffnet hat.
* ![grafik](https://user-images.githubusercontent.com/78872776/220582922-fdfcc724-bbf9-4cc1-b3b7-4f5c9812fecf.png)

* Die Optionen "-u" und "-a" werden verwendet, um UDP-Verbindungen und  alle Verbindungen anzuzeigen, auch wenn sie nicht mit einer Prozess-ID  verknüpft sind.
* ![grafik](https://user-images.githubusercontent.com/78872776/220584433-354f7668-28cf-4b0a-9b10-75061bda1698.png)

## 7. Automatisierung und Task-Scheduler

Um das vorliegende System am laufenden Stand zu halten ist es möglich  automatische Updates durchführen zu lassen. Dies kann über verschiedene  Möglichkeiten geschehen (z.B. `unattended-upgrade`). Konfiguriere das automatische Upgrade von Security-Updates in deiner VM. Was sind dabei die wichtigsten *Default* Einstellungen?

1. Nur Sicherheitsupdates: Unattended-upgrade aktualisiert standardmäßig nur die Pakete, für die Sicherheitsupdates verfügbar sind. Dies kann geändert werden, um auch andere Pakete zu aktualisieren.
2. Zeitplan: Der Befehl ist standardmäßig so konfiguriert, dass er jeden Tag um 6 Uhr morgens ausgeführt wird. Dieser Zeitplan kann angepasst werden, um den Bedürfnissen des Benutzers zu entsprechen.
3. E-Mail-Benachrichtigungen: Unattended-upgrade kann so eingestellt werden, dass es dem Benutzer eine E-Mail sendet, wenn Updates installiert wurden oder wenn ein Fehler aufgetreten ist.
4. Systemneustart: Wenn ein Paket ein Update erfordert, das einen Neustart des Systems erfordert, wird dies standardmäßig nicht automatisch durchgeführt. Der Benutzer muss den Neustart manuell durchführen. Dies kann geändert werden, um den Neustart automatisch durchzuführen.
5. Verhalten bei Konflikten: Wenn es bei der Aktualisierung von Paketen zu Konflikten kommt, wird standardmäßig das beibehalten, was bereits installiert ist. Dies kann geändert werden, um die aktualisierte Version zu installieren oder um den Benutzer zu fragen, welche Version installiert werden soll.

![grafik](https://user-images.githubusercontent.com/78872776/220586187-9710a966-ba4a-496e-8a78-d1a7b5179345.png)

--------------------------------------

Wiederkehrende Aufgaben (Tasks) können mit dem Dienst `cron` oder auch dem `systemd.timer` durchgeführt werden. Definiere einen Prozess, der dir die Information  über deine Festplatten-Auslastung jeden Tag um 06:00 in der Früh in eine Datei speichert, die in das Verzeichnis `/var/log/harddisk/` als `20230212-0600.log` (nach dem aktuellen Datum) gespeichert wird . Kleiner Tipp, du kannst  ein Bash-Script schreiben, welches von den oben genannten Diensten  aufgerufen wird und teste dein Script bevor du die Timer einsetzt.

* Bash Skript: ![grafik](https://user-images.githubusercontent.com/78872776/220610363-4fcdce5a-4743-4c59-a90c-5afb4173047f.png)

*  Als rootuser den Befehl crontab -e ausführen und letzte weise Zeile eingeben um das Skript immer um 06:00 auszuführen![grafik](https://user-images.githubusercontent.com/78872776/220615882-bee99b47-0e7c-4a41-a505-81282876b0cb.png)

  

![grafik](https://user-images.githubusercontent.com/78872776/220616714-f1aa9984-cc0d-4c23-96a4-688e1a276df7.png)

die Log files werden nach vorgegebenen Schema erstellt immer mit dem aktuellen datum erstellt