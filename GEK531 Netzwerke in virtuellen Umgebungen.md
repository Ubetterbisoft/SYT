# GEK531 Netzwerke in virtuellen Umgebungen

## Grundanforderungen

* **Recherchiere in welchen grundlegenden Eckpunkten sich die möglichen  Netzwerkkonfigurationen unterscheiden. Gib auch zumindest jeweils ein  Einsatzgebiet an, wo der jeweilige Modus Sinn macht. Dokumentiere auch  mithilfe von Netzwerkdiagrammen bzw. Bildern und versuche nicht nur eine Quelle zu finden!**

1. NAT (Network Address Translation ) PORTS!

   1. [1] NAT wird häufig verwendet, um aufgrund der Knappheit öffentlicher  IP-Adressen mit privaten IP-Adressen im Internet zu kommunizieren. Z.b ein Unternehmen will nicht mit jeder Ip-Adresse eines Mitarbeiters mit dem Internet kommunizieren sondern mit nur einer einzigen. Somit werden viele Globale IPv4 Adressen eingespart

   2. [3]Netzplan von Nat:![grafik](https://user-images.githubusercontent.com/78872776/193265250-737fb7f2-0dab-4df4-be2d-ea58a94e7705.png) 

      

2. Bridged (Network - Hardware) Max-address

   1. [2]Wenn zwei NAT-Geräte seriell verbunden werden (z. B. wenn ein Modem mit integrierten  NAT-Fähigkeiten mit einem Router verbunden wird, der ebenfalls ein  NAT-Gerät ist) sollte man den Modem im **Bridge**-**Modus** konfigurieren, um Konflikte zu vermeiden.
   2. [3]![grafik](https://user-images.githubusercontent.com/78872776/193265669-6cb8316c-5bcf-46b6-b283-ecabdbf86ffb.png)

3. Host - Only
   * Die Host Only Konfiguration lässt nur Host Systeme und VM'S mit anderen VM'S kommunizieren
   * [3]<img src="https://user-images.githubusercontent.com/78872776/193266227-218d660f-58d3-4996-b6fc-e69dc81bc947.png" alt="grafik"  /> 

4. Internes Netzwerk

   1. [3]Nur virtuelle Maschinen, die dem gleichen internen Netzwerk angehören,  können untereinander kommunizieren. Eine Kommunikation über die Grenzen  des virtuellen Netzwerkes hinaus ist nicht möglich.
   2. ![grafik](https://user-images.githubusercontent.com/78872776/193267135-b51058ba-7124-42cd-bd9e-8507603259a7.png) 

* Konfiguriere nun deine virtuelle Maschine so, dass du sie von deinem  Host-System per ping-Befehl erreichen kannst, allerdings andere Geräte  im Netzwerk von der virtuellen Maschine nichts sehen.
  * Host-only:
    * Ich pinge von der Hostmaschine aus die VM: erfolgreich<img src="https://user-images.githubusercontent.com/78872776/193268876-9bd5779e-9cf8-4108-a2a4-3a6022fbd487.png" alt="grafik" style="zoom:200%;" />  
    
      
  
* Sobald du dich mit deiner virtuellen Instanz ins Internet verbinden  kannst, mache ein Systemupdate deiner Linux Installation mittels `sudo apt update; sudo apt upgrade`. Was geschieht bei diesen zwei Befehlen?

  * Damit ich ins Internet komme muss ich NAT als Netzwerkadapter konfigurieren, weil es mit Host-Only nicht möglich ist.
  * update:![grafik](https://user-images.githubusercontent.com/78872776/193333530-684cff54-7818-4ff7-bbe1-173915f98274.png) 
  * upgrade:
  * sudo apt update aktualisiert die Paketliste
  * sudo apt upgrade updated die Pakete dann wirtklich

  

* Beantworte auch noch die übrigen Fragestellungen weiter unten und gib  die erstellte Dokumentation als PDF auf Moodle ab und melde dich zu  einem Abgabegespräch!

## Fragestellungen

- Welche drei gängigen Konfigurationsarten gibt es bei der Netzwerkkonfiguration von virtuellen Maschinen?

  - Bridged
  - NAT
  - Host-Only

  

- Wann verwende ich welche Netzwerkkonfiguration?

  - Bridged: Die VM bekommt direkten Zugriff auf  die physikalische Netzwerkkarte, die Ip-Adresse wird ihr vom Netzwerk zugewiesen. 
  - NAT: Es wird eine virtuelle Netzwerkkarte erstellt, es entsteht ein eigenes Netzwerk für die VM's. Portweiterleitungen sind möglich.
  - Host-Only: Es ist so wie Nat nur ist es vom äuseren Netzwerk abgeschottet. Es kann nur mit Hostsystem und anderen VM's im lokalen netz kommuniziert werden.

  

- Welche Auswirkungen auf die an die VM vergebene IP-Adresse hat der jeweilige Modus?

  - Nat -> private IP-Adresse vom Hypervisor
  - Bridged -> über DHCP
  - Host-Only -> auch IP-Adresse über Hypervisor

  

- Wie können externe Netzwerkknoten auf die Gast-Instanz zugreifen?

  - Bridged: Mit der IPAdresse die die VM vom Netzwerk zugewiesen bekommen hat
  - NAT: Mit der Originalen IP-Adresse des Hostsystems
  - Host Only: Bei Host Only ist gar kein zugriff auf das Internet möglich

  

- Was muss das Host-System starten, damit eine automatische IP-Vergabe in der Gast-Instanz zustande kommen kann? Wie kann man das auch manuell lösen?

  - Ein DHCP server muss gestartet werden damit eine automatische IP vergeben wird
  - Manuell kann man es auch statisch vergeben

  

- Wo werden die virtuellen Netzwerkdevices verwaltet?

  - Der Hypervisor verwaltet die virtuellen Netzwerkdevices

  

- Wie kann ein bestimmtes Netzwerkinterface bei der *Bridged* Variante ausgewählt werden?

  - ![image-20220930204921670](C:\Users\draji\AppData\Roaming\Typora\typora-user-images\image-20220930204921670.png)
  - Unter erweitert 




# Quellen

[1]S.  Luber, "Was ist NAT (Network Address Translation)?", *Ip-insider.de*, 2022. [Online]. Available:  https://www.ip-insider.de/was-ist-nat-network-address-translation-a-663954/. [Accessed: 30- Sep- 2022].

[2]"Szenarien, in denen Sie Ihr Modem im Bridge-Modus konfigurieren müssen", *NETGEAR KB*, 2022. [Online]. Available:  https://kb.netgear.com/de/22280/Szenarien-in-denen-Sie-Ihr-Modem-im-Bridge-Modus-konfigurieren-m%C3%BCssen-1479991075149?language=de. [Accessed: 30- Sep- 2022].

[3]R.  Nockmann, "VirtualBox Netzwerkkonfiguration - Nocksoft", *Nocksoft*, 2022. [Online]. Available: https://nocksoft.de/tutorials/virtualbox-netzwerkkonfiguration/. [Accessed: 30- Sep- 2022].