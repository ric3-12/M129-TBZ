## 1. Ausgangslage / Umfeld

Das dargestellte Netzwerk gehört zu einem KMU (kleines bis mittleres Unternehmen) mit mehreren Abteilungen.
Das Unternehmen arbeitet standortübergreifend innerhalb eines Gebäudekomplexes bzw. Campus und benötigt:

stabile interne Kommunikation

logische Trennung der Abteilungen

einfache Erweiterbarkeit

klare Struktur für Administration und Fehlersuche

Das Netzwerk wurde mit Cisco Routern (2811) und Cisco Switches (2960) umgesetzt.

## 2. Ziel des Netzwerks

Ziel der Netzwerkarchitektur ist es:

die Abteilungen logisch voneinander zu trennen

Routing zwischen den Abteilungen zu ermöglichen

unterschiedlich große Netze effizient zu adressieren

ein realistisches KMU-Szenario abzubilden

## 3. Warum mehrere Subnetze?

Nicht jede Abteilung benötigt gleich viele Endgeräte.
Deshalb wurden unterschiedlich große Subnetze verwendet:

/26 → größere Abteilungen (bis 62 Hosts)

/27 → mittlere Abteilungen (bis 30 Hosts)

/28 → kleine Abteilungen / Spezialbereiche (bis 14 Hosts)

Vorteil:
Effiziente Nutzung von IP-Adressen und klare Struktur.

## 4. Rollen der Netzwerkgeräte
4.1 Switches (Cisco 2960)

Access-Switches für Endgeräte (PCs)

Verbinden Clients innerhalb einer Abteilung

Keine Routing-Funktion (Layer 2)

4.2 Router (Cisco 2811)

Routing zwischen den Subnetzen (Layer 3)

Jeder Router stellt das Default Gateway für seine Abteilung bereit

Verbindung zwischen den einzelnen Netzwerksegmenten

## 5. Routing-Konzept

Es wird statisches Routing eingesetzt.

Warum statisches Routing?

kleines bis mittleres Netzwerk

volle Kontrolle über Routing-Wege

einfach zu verstehen und zu dokumentieren

ideal für Schul- und Lernumgebungen

Jeder Router kennt:

seine direkt angeschlossenen Netze

statische Routen zu entfernten Netzen