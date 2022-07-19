# Raspberry Pi-Wetterstation
## Info
Mithilfe dieses Repositories wird ein Raspberry Pi 3B und verschiedener Sensorik eine vollfunktionale lokale Wetterstation.

Hierbei werden mittels der Sensoren BMP180 und DHT11 
- Lufttemperatur
- Luftdruck
- Luftfeuchtigkeit
- Höhe

erfasst.

In den Ordnern Bilder, Software, Hardware und Dokumentation finden sich verschiedene Ressourcen und Informationen zum Projekt.

## Vorbereitung der Komponenten

Unterstützende Bilder finden sich im Ordner Bilder

### Pinbelegung
#### DHT11

Von Raspberry Pi >> DHT11

 - Pin 1 auf 3.3V
 - Pin 6 auf GND
 - Pin 7 (GPIO 4) auf D4

#### BMP180

Von Raspberry Pi >> BMP180

 - Pin 4 auf 5V
 - Pin 9 auf GND
 - Pin 3 auf D2
 - Pin 5 auf D1

## Installation
Es wird ein vollständig eingerichteter Raspberry-Pi 3, sowie Root-Rechte vorausgesetzt. __Es wird Raspberry Pi OS in der 64-Bit Variante empfohlen.__

Dem RPi ___muss___ eine statische IP-Adresse im Netzwerk vergeben werden!

In `Software/Pi/` führe das Installationsscript aus:

`sudo ./install.py`

Nach der Installation werden alle Dienste vollautomatisch bei Systemstart ausgeführt.

## FAQ
### Wie ändere ich die Netzwerkkonfiguration des PIs?

Um die Host-Adresse zu ändern, führe das Script zum erneuten Kompilieren des Servers aus.
In `Software/Pi`:

`sudo ./rebuild_server.sh`

### Wie führe ich ein Update für die Applikation durch?

Siehe: __Wie ändere ich die Netzwerkkonfiguration des PIs?__
