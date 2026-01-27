# 1️⃣ Thema / Auftrag

Einführung in IPv6 – Adressierung, Adresstypen und praktische Anwendung

**Auftrag:**
Ziel dieser Übung ist es, die Grundlagen von IPv6 zu verstehen, Unterschiede zu IPv4 zu erkennen und IPv6 in der Praxis anzuwenden. Dazu werden Theorie, aktuelle Statistiken sowie praktische Tests mit IPv6-Adressen durchgeführt.

## 2️⃣ Ausgangslage

IPv4 ist aufgrund der begrenzten Anzahl verfügbarer IP-Adressen weitgehend ausgeschöpft. Moderne Netzwerke benötigen eine Lösung, die eine nahezu unbegrenzte Anzahl an Adressen bietet und zukünftige Anforderungen wie Cloud-Dienste, mobile Endgeräte und IoT unterstützt.

IPv6 wurde entwickelt, um diese Einschränkungen zu beseitigen und eine langfristige Lösung für das Internet bereitzustellen.

## 3️⃣ Lernziele

- Ich verstehe den Aufbau und die Schreibweise von IPv6-Adressen
- Ich kenne die wichtigsten IPv6-Adress-Typen
- Ich kann IPv6 auf einem Client aktivieren
- Ich kann die IPv6-Konnektivität zwischen zwei Clients testen
- Ich kann den aktuellen Stand der IPv6-Nutzung beurteilen

## 4️⃣ Theorie / Fachwissen

**4.1 Was ist IPv6?**

- IPv6 ist die Weiterentwicklung von IPv4 und verwendet 128 Bit für die Adressierung. Dadurch stehen deutlich mehr IP-Adressen zur Verfügung als bei IPv4.

- IPv6 benötigt grundsätzlich kein NAT und vereinfacht dadurch den Netzwerkaufbau.

**4.2 Aufbau und Schreibweise von IPv6-Adressen**

IPv6-Adressen bestehen aus acht Blöcken mit je vier hexadezimalen Zeichen, getrennt durch Doppelpunkte.

Beispiel:

`2001:0db8:0000:0000:0000:0000:0000:0001`

Vereinfachte Schreibweise:

`2001:db8::1`

**4.3 IPv6-Adress-Typen**
Typ	Beschreibung
Global Unicast	Öffentlich routbare Adresse
Unique Local Address (ULA)	Private IPv6-Adresse
Link-Local	Lokale Kommunikation im selben Netzwerk
Multicast	Gruppenkommunikation
Loopback	Kommunikation mit dem eigenen Gerät

IPv6 kennt keinen Broadcast, dieser wird durch Multicast ersetzt.

## 5️⃣ Recherche / Vertiefung
**5.1 IPv6-Nutzung weltweit und in der Schweiz**

Die Statistiken von Google zeigen, dass der Anteil der IPv6-Nutzer weltweit stetig steigt. Auch in der Schweiz nimmt die Nutzung von IPv6 kontinuierlich zu.

Laut Cisco 6lab sind viele Schweizer Webseiten bereits über IPv6 erreichbar, insbesondere bei grossen Organisationen und Internet-Providern.

**5.2 Vergleich IPv4 vs. IPv6**
Merkmal	IPv4	IPv6
Adresslänge	32 Bit	128 Bit
Anzahl Adressen	ca. 4.3 Milliarden	sehr gross
Broadcast	Ja	Nein
NAT notwendig	Ja	Nein

## 6️⃣ Praxis / Durchführung
**6.1 IPv6 auf dem Client aktivieren**

Auf einem Windows-System kann IPv6 über die Netzwerkeinstellungen oder standardmässig automatisch verwendet werden. Alternativ können Informationen über IPv6 mit PowerShell angezeigt werden.

Beispiel:

Get-NetIPv6Protocol
Get-NetAdapter

**6.2 Variante 1 – Link-Local IPv6-Adresse**

Link-Local-Adressen werden automatisch generiert und beginnen mit fe80::. Sie ermöglichen die Kommunikation zwischen Geräten im selben Netzwerk ohne zusätzliche Konfiguration.

Ein Ping mit Link-Local-Adresse ist möglich, wenn das Interface angegeben wird.

**6.3 Variante 2 – Unique Local Address (ULA)**

ULA-Adressen befinden sich im Bereich fc00::/7 und dienen als private IPv6-Adressen für interne Netzwerke. Sie sind vergleichbar mit privaten IPv4-Adressen.

Beispiel:

fdf8:f535:82e4::/64

**6.4 Verbindungstest (Ping)**

Zwischen zwei Clients wird die IPv6-Konnektivität mit dem Ping-Befehl überprüft. Ein erfolgreicher Ping bestätigt die korrekte IPv6-Konfiguration.

## 7️⃣ Resultate / Beobachtungen

IPv6-Adressen wurden korrekt zugewiesen

- Die Kommunikation zwischen zwei Clients über IPv6 funktioniert
- Sowohl Link-Local als auch ULA-Adressen können verwendet werden
- IPv6 ist in modernen Betriebssystemen standardmässig aktiv

## 8️⃣ Schwierigkeiten / Erkenntnisse

- Die Schreibweise von IPv6 ist anfangs ungewohnt
- Link-Local-Adressen erfordern die Angabe des Interfaces
- IPv6-Subnetting ist einfacher als bei IPv4

## 9️⃣ Reflexion

Durch diese Übung habe ich gelernt, wie IPv6 aufgebaut ist und wie sich IPv6 von IPv4 unterscheidet. Besonders interessant fand ich, dass IPv6 ohne NAT auskommt und automatisch Link-Local-Adressen vergibt. IPv6 wird bereits heute aktiv genutzt und ist ein wichtiger Bestandteil moderner Netzwerke.

## 🔟 Fazit

IPv6 ist notwendig, um den steigenden Anforderungen moderner Netzwerke gerecht zu werden. Die Übung zeigt, dass IPv6 nicht nur theoretisch relevant ist, sondern auch praktisch einfach eingesetzt werden kann.
