*******************************************************************************
*                    __    __      __  ___      _ __                          *
*             ____  / /_  / /_  __/  |/  /___ _(_) /                          *
*            / __ \/ __ \/ / / / / /|_/ / __ `/ / /                           *
*           / /_/ / / / / / /_/ / /  / / /_/ / / /                            *
*          / .___/_/ /_/_/\__, /_/  /_/\__,_/_/_/ Free                        *
*         /_/            /____/                                               *
* https://phlymail.com                            mailto:phlymail@phlylabs.de *
*******************************************************************************
* (c) 2001-2016 phlyLabs, Berlin                                              *
*******************************************************************************
*                                                                             *
*                     Installation und Konfiguration                          *
*                                                                             *
*******************************************************************************

Installationshinweise phlyMail Free
--------------------------------------------

Dieses Archiv enth�lt die Ordner 'phlymail' und 'Docs'.

'phlymail' enth�lt die Applikation phlyMail Free.

Kopieren Sie diesen Ordner in ein geeignetes Verzeichnis auf Ihrer Pr�senz /
Ihrem Webserver, wo Sie PHP ausf�hren k�nnen.

Richten Sie dann die MySQL-Datenbank ein, die Sie f�r phlyMail verwenden
m�chten. Die Tabellen werden durch den Installer angelegt.

Sobald Sie dies getan und die Zugriffsrechte korrekt vergeben haben (dabei ist
insbesondere darauf zu achten, da� sowohl die Zugriffsmaske per chmod
ausreichend gesetzt ist [wir empfehlen chmod -r 777 bzw.
chown -r <apacheuser>.<apachegroup>], als auch der Eigent�mer von PHP
Schreibrechte auf die Ordnerstruktur von phlyMail hat), k�nnen Sie den
Installer ausf�hren, der die Grundkonfiguration vornimmt.

Ein Hinweis zu Apache und mod_php (PHP l�uft als Modul und nicht als CGI):
-------------------------------------------------------------------------------
Achten Sie darauf, da� Sie den phlyMail-Ordner per chown auf den Nutzer und die
Gruppe �bertragen, unter denen der Apache l�uft. Dazu m�ssen Sie i.d.R.
root-Rechte haben bzw. Komandos per sudo ausf�hren k�nnen.
K�nnen Sie dies nicht tun, sollte es gen�gen, den phlyMail-Ordner per
chmod -r 777 f�r alle les- und schreibbar zu machen.
Beachten Sie aber, dass es im Allgemeinen ausreicht, die Struktur mit der Maske
755 bzw. 775 zu versehen. Je lockerer die Rechte vergeben werden, desto
unsicherer ist Ihre Installation.
-------------------------------------------------------------------------------

Der Aufruf des Installers erfolgt mit
https://ihre-domain.tld/pfad/zu/phlymail/installer.php

W�hrend der Installation werden der Pr�fix f�r die zu verwendenden
MySQL-Tabellen abgefragt. Sollte dies nicht mit bereits vorhandenen Tabellen in
der gew�hlten DB kollidieren, empfehlen wir, den vom Installer gemachten
Vorschlag zu �bernhemen.

Nach erfolgreicher Installation l�scht sich der Installer selbst und
phlyMail ist grunds�tzlich betriebsbereit.

Mit dem Installer wurde ein Administrator mit dem von Ihnen vergebenen
Usernamen und Pa�wort eingerichtet. Loggen Sie sich mit diesen Daten in die
Konfigurationsboerfl�che ein und nehmen Sie nun die Detailkonfiguration von
phlyMail vor:
https://ihre-domain.tld/pfad/zu/phlymail/config.php

Der Aufruf der Applikation erfolgt sp�ter mit:
https://ihre-domain.tld/pfad/zu/phlymail/index.php oder einfach nur
https://ihre-domain.tld/pfad/zu/phlymail/


Weitere M�glichkeiten
---------------------

Bitte beachten Sie auch: https://phlymail.com/forum/tipps-tricks-f28.html

Bei Problemen besuchen Sie bitte unser Forum unter https://phlymail.com/forum/

Viel Spa� w�nscht

Das Team von phlyLabs