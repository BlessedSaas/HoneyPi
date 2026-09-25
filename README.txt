HoneyPi iPhone Dashboard
=========================

Vorbereitet für Channel-ID: 3456325

1. Die Dateien auf einen HTTPS-Webspace legen (z. B. GitHub Pages, Cloudflare Pages oder eigener Webspace).
2. index.html in Safari auf dem iPhone öffnen.
3. Beim ersten Start Channel-ID und den READ API KEY aus ThingSpeak eintragen.
   Niemals den WRITE API KEY verwenden.
4. In Safari: Teilen -> Zum Home-Bildschirm.
5. Danach startet das Dashboard wie eine eigene App.

Funktionen
----------
- automatische Erkennung der HoneyPi-Messarten über die Field-Namen
- Waage und Gewichtsänderung in kg; DS18B20 in °C
- DHT11-Temperatur in der Box in °C und Luftfeuchtigkeit in %
- falls die Feldnamen nicht eindeutig sind: Feldzuordnung unter Einstellungen
- aktuelle Messwerte als Karten (leere Felder werden nicht als 0 angezeigt)
- Verlauf 24 h / 3 / 7 / 30 Tage
- Minimum, Durchschnitt und Maximum
- getrennte Diagramme für Gewicht und DS18B20-Temperatur
- automatische Aktualisierung alle 60 Sekunden
- Read API Key bleibt im lokalen Browser-Speicher des Geräts
- Channel-ID 3456325 ist bereits voreingestellt

Hinweis:
Eine PWA/Service-Worker-Funktion benötigt HTTPS (localhost ausgenommen). Die eigentlichen
ThingSpeak-Daten werden direkt im Browser über die ThingSpeak REST API geladen.

Aktualisierung einer bestehenden GitHub-Pages-Installation:
Alle Dateien dieses ZIPs im Repository ersetzen und die Änderungen committen.
Nach der Veröffentlichung die Seite am iPhone einmal neu laden. Die bestehenden
Channel-Einstellungen im Browser bleiben erhalten.
