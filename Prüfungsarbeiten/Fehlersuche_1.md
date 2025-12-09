# Dokumentation – Analyse und Korrektur der Routingfehler (Cisco)
*(Ich-Perspektive)*

## 1. Einleitung

In dieser Aufgabe habe ich die Routingkonfiguration in einer Cisco-Netzwerkumgebung analysiert.  
Mir wurden zwei konkrete Fehlermeldungen angezeigt:

- **Fehler in RIB (Präfixlänge) bei Router RT01**  
- **Fehler in RIB (Next Hop) bei Router RT02**

Mein Ziel war es, herauszufinden, warum diese Einträge falsch sind und wie man sie in Cisco Packet Tracer richtig korrigiert.

## 2. Fehleranalyse

### 2.1 Fehler bei RT01 – falsche Präfixlänge

In der Routingtabelle von RT01 war eine Route zum Netz **192.168.3.0** eingetragen, allerdings mit einer **falschen Subnetzmaske**.

**Falscher Eintrag:**
```
192.168.3.0/29 via 10.120.80.1
```

Das Netz 192.168.3.0 wird in der Topologie jedoch als **/24-Netz** genutzt.  
Durch die falsche Präfixlänge konnte RT01 Pakete in dieses Netz nicht korrekt weiterleiten.

### 2.2 Fehler bei RT02 – falscher Next Hop

In RT02 befand sich folgender ungültiger Routingeintrag:

**Falscher Eintrag:**
```
10.40.40.0/24 via 127.0.0.1
```

Die Adresse **127.0.0.1** ist die interne Loopback-Adresse und niemals ein gültiger Next Hop.

Der richtige Weg zum Netz 10.40.40.0/24 führt über Router RT03.  
RT03 besitzt auf der Verbindung zu RT02 die Adresse:

```
10.20.20.2
```

## 3. Vorgehen zur Korrektur in Cisco Packet Tracer

### 3.1 Allgemeiner Hinweis

In Cisco Packet Tracer können **statische Routen nicht direkt bearbeitet** werden.  
Ich musste daher:

1. den falschen Eintrag **löschen**  
2. den korrekten Eintrag **neu hinzufügen**

### 3.2 Korrektur bei RT01

**Schritte:**

1. Router anklicken  
2. **Config → Routing → Static**  
3. Falsche Route auswählen  
4. **Remove** klicken  
5. Korrekte Werte eintragen:

```
Network: 192.168.3.0
Mask:    255.255.255.0
Next Hop: 10.120.80.1
```

6. **Add** bestätigen

### 3.3 Korrektur bei RT02

**Korrekte Route eingetragen:**

```
Network: 10.40.40.0
Mask:    255.255.255.0
Next Hop: 10.20.20.2
```

Damit zeigt RT02 korrekt auf RT03.

## 4. Ergebnis

Nach der Anpassung beider Routingtabellen funktionierte das endgeräteübergreifende Routing wieder vollständig.  
Alle Netzwerke ließen sich erfolgreich anpingen, und die Fehlerhinweise im Packet Tracer waren behoben.

## 5. Reflexion

Diese Aufgabe hat mir gezeigt, wie wichtig korrekte Präfixlängen und Next-Hop-Adressen bei statischem Routing sind. Ich habe gelernt:

- eine falsche Subnetzmaske kann ein ganzes Netz isolieren  
- ein Next Hop muss immer eine gültige Router-IP sein  
- statische Routen müssen bei Fehlern gelöscht und neu hinzugefügt werden  

Diese Erkenntnisse helfen mir, Routingfehler schneller zu erkennen und sicher zu beheben.
