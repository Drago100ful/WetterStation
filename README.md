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
