# TCP/IP-Modell

Das **TCP/IP-Modell** ist ein praktisches Netzwerkmodell, das in der echten Welt verwendet wird – z. B. im Internet. Es besteht aus **4 Schichten**, die ähnliche Aufgaben wie das OSI-Modell übernehmen.

## Übersicht der 4 Schichten

|TCP/IP-Schicht|Entspricht OSI-Schicht(en)|Aufgabe (einfach erklärt)|
|---|---|---|
|Anwendung|OSI 5–7|Interaktion mit Programmen (z. B. Browser, E-Mail)|
|Transport|OSI 4|Zuverlässige Datenübertragung (z. B. TCP, UDP)|
|Internet|OSI 3|Routing und IP-Adressen|
|Netzzugang|OSI 1–2|Physische Verbindung und MAC-Adressen|

---

## Erklärung mit Beispielen

### **1. Netzzugangsschicht (Network Access Layer)**

**Was macht sie?**  
Stellt die physische Verbindung her und regelt, wie Daten über das Medium übertragen werden.

**Beispiele:**

- Ethernet
- WLAN
- MAC-Adresse
- Switches, Netzwerkkabel

---

###  **2. Internetschicht (Internet Layer)**

**Was macht sie?**  
Findet den Weg durch das Netzwerk und sorgt für Adressierung.

**Beispiele:**

- IP-Adresse (IPv4, IPv6)
- Router
- ICMP (z. B. für Ping)

---

### **3. Transportschicht (Transport Layer)**

**Was macht sie?**  
Zerlegt Daten in Pakete und sorgt für deren zuverlässige Übertragung.

**Beispiele:**

- TCP (z. B. für Webseiten, E-Mail)
- UDP (z. B. für Videos, Games)
- Portnummern (z. B. Port 443 für HTTPS)

---

###  **4. Anwendungsschicht (Application Layer)**

**Was macht sie?**  
Stellt die Schnittstelle zur Benutzeranwendung bereit.

**Beispiele:**

- HTTP (Webseiten)
- SMTP (E-Mail senden)
- FTP (Dateien übertragen)
- DNS (Domainnamen auflösen)
