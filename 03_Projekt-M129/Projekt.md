# Projekt_Modul_129

In Diesem Modul werde ich als Projekt ein kleines Netzwerk Bauen:

![Cisco File](Pictures/Screenshot 2024-01-29 195531.png)

Zuerst habe ich mit der Grobplannung angefangen das habe ich auf Draw.io gemacht:

![Draw Io](/99_Media/Draw.io.png)

Danach habe ich die Grobplannung von Draw.io in Cisco umgesetzt:

---


Danach habe ich die IP Adressen zuteilung und die Routingtabellen erstellt und habe die in Cisco umgesetzt:

[Routing Tabellen](https://gitlab.com/leonur-/projekt_modul_129/-/blob/main/Routing%20Tabellen.md?ref_type=heads)


Danach habe ich alles Konfiguriert und mit dem Ping command getestet. Alle Gateways eingetragen und das und auf dem Cisco File noch alles Aufgeschrieben.

Ping Commands:
![Cisco File](/99_Media//Erster_ping.png)
![Cisco File](/99_Media//Zweiter_ping.png)


------------------

# Static Routing

In diesem Projekt lag der Schwerpunkt hauptsächlich auf dem Einsatz von Static Routing.

Static Routing beschreibt ein Verfahren zur Weiterleitung von Datenpaketen in Computernetzwerken, bei dem die Routing-Tabelle manuell eingerichtet wird. Dabei legt der Netzwerkadministrator fest, welchen Weg Datenpakete von der Quelle bis zum Ziel nehmen. Im Unterschied zum dynamischen Routing, bei dem Router automatisch Routing-Informationen austauschen und selbstständig den optimalen Pfad berechnen, erfordert Static Routing eine vollständige manuelle Konfiguration.

Die Routen werden beim statischen Routing von Hand erstellt und gepflegt. Dazu gehören die Definition von Zielnetzwerken und Subnetzen sowie die Angabe des jeweiligen nächsten Hops. Diese Einträge bleiben konstant und ändern sich nur, wenn der Administrator sie gezielt anpasst.

Static Routing eignet sich besonders für kleine Netzwerke oder überschaubare Netzwerkstrukturen, in denen sich die Topologie nur selten verändert. Es stellt eine einfache, stabile und gut kontrollierbare Methode zur Verkehrssteuerung dar und reduziert den Netzwerk-Overhead, da keine regelmäßigen Routing-Updates ausgetauscht werden müssen.

Dennoch bringt Static Routing auch Nachteile mit sich. Es ist nur eingeschränkt skalierbar und kann bei häufigen Änderungen der Netzwerktopologie oder bei großen Netzwerken schnell unübersichtlich und ineffizient werden. In solchen Szenarien ist dynamisches Routing meist die bessere Lösung, da es sich automatisch an Veränderungen anpasst.

Zusammenfassend bietet Static Routing eine zuverlässige und leicht verständliche Möglichkeit zur Steuerung des Datenverkehrs, insbesondere in Netzwerken mit stabiler Struktur, in denen Vorhersehbarkeit und Kontrolle im Vordergrund stehen.

