# Software

In diesem Ordner finden sich alle Skripte, Ressourcen und Apps, die während der Installation oder während der tatsächlichen Bereitstellung der App gebraucht werden

Die Webapp basiert auf einem responsiven __VueJS-Frontend__ und einem regulären __PHP-Backend__, das mit der Datenbank auf dem Raspberry kommuniziert, die gewünschten Daten abholt und diese dem Frontend als API bereitstellt.

Diese Dreiecksbeziehung kommt durch Sicherheitsbedenken zustande, da der Client niemals direkt zugriff auf die serverseitigen Daten haben sollte.

Ein einfaches __Python-Script__ regelt die Erhebung der Daten der Sensoren. Dieses  wird einfach bei jedem Boot als Systemdienst gestartet und fügt bei jedem vollständigen Datensatz circa alle zwei Sekunden einen neuen Eintrag in die __MYSQL-Datenbank__ ein.

## Installation
`sudo ./Pi/install.sh`