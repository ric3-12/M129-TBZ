# Netzwerkgrundlagen & Netzwerkkomponenten

Dieses Merkblatt vertieft Punkt **1 der Modulbeschreibung** und ist so aufgebaut, dass du es direkt in deiner Dokumentation verwenden kannst.

---

# 📘 1. Anforderungen für ein neues Netzwerk & Netzwerkkomponenten

Beim Aufbau eines neuen Netzwerks müssen technische, organisatorische und sicherheitsrelevante Punkte berücksichtigt werden. Die folgenden Kapitel decken alle erforderlichen Grundlagen ab.

---

## ✔ 1.1 Wichtige Normierungsstellen (IEEE, ISO) & deren Standards

### **IEEE – Institute of Electrical and Electronics Engineers**

Die IEEE definiert Standards für Netzwerk- und Kommunikationstechnologien.
Wichtige Standards:

* **IEEE 802.3 (Ethernet)** → physikalische & Data-Link-Protokolle für LAN
* **IEEE 802.11 (WLAN)** → Wireless LAN
* **IEEE 802.1Q (VLAN)** → Tagging für virtuelle Netzwerke

### **ISO – International Organization for Standardization**

* Bekannt für das **OSI-Schichtenmodell**, welches die Netzwerkkommunikation beschreibt.
* Dient als Grundlage für Netzwerkdesign, Fehlersuche und Analyse.

### Warum Standards wichtig sind

* Herstellerunabhängigkeit
* Interoperabilität zwischen Geräten
* Sicherheit durch definierte Protokolle
* Skalierbarkeit & Erweiterbarkeit

---

## ✔ 1.2 Wichtige LAN-Technologien & deren Einsatzgebiete

| Technologie                   | Standard        | Einsatzzweck                                    |
| ----------------------------- | --------------- | ----------------------------------------------- |
| **Ethernet (Kupfer/LWL)**     | IEEE 802.3      | Kabelgebundene Firmennetze, Serveranbindungen   |
| **WLAN**                      | IEEE 802.11     | Mobile Geräte, flexible Netzwerke               |
| **VLAN**                      | IEEE 802.1Q     | Netztrennung, Sicherheitszonen                  |
| **PoE (Power over Ethernet)** | IEEE 802.3af/at | Stromversorgung über LAN-Kabel für Kameras, APs |

### Funktionsweise grundsätzlich

* Ethernet arbeitet mit **Frames & MAC-Adressen**.
* WLAN nutzt Funkkanäle, Verschlüsselung (WPA3).
* VLANs ermöglichen mehrere logische Netze auf derselben Hardware.

---

## ✔ 1.3 Funktionen von Switch und Router

### **Switch (Layer 2)**

* Verarbeitet **MAC-Adressen**
* Verbindet Geräte innerhalb **eines** Netzwerks
* Arbeitet Frame-basiert
* Lerneffekt: Switch baut MAC-Adress-Tabelle auf
* Verhindert unnötigen Traffic (Unicast, Broadcast, Multicast)

### **Router (Layer 3)**

* Verbindet **mehrere Netzwerke** miteinander
* Arbeitet mit **IP-Adressen**
* Bestimmt Routen mithilfe von Routingtabellen
* Setzt NAT, DHCP, ACLs ein

### Unterschied Switch vs. Router

* Switch = Kommunikation **im gleichen IP-Netz**
* Router = Kommunikation **zwischen verschiedenen IP-Netzen**

---

## ✔ 1.4 Switch-Features & Zusatzfunktionen

### **Manageable vs. unmanaged Switches**

* *Unmanaged*: Plug-and-Play, keine Konfiguration möglich
* *Managed*: VLAN, SNMP, QoS, Monitoring möglich

### **Stackable Switches**

* Mehrere Switches als „ein Gerät“ verwaltbar
* Vorteile: Skalierbarkeit, hohe Verfügbarkeit

### **Auto-Negotiation**

* Automatische Geschwindigkeit/Modus (10/100/1000 Mbit/s, Full-Duplex)

### **Spanning-Tree-Protokoll (STP)**

* Verhindert Netzwerkschleifen
* Sorgt für Redundanz
* Varianten: RSTP, MSTP

---

## ✔ 1.5 Sicherheit bei Switches & Routern

### Switch-Sicherheit

* **Port-Security** (MAC-Adressbegrenzung)
* **VLANs** zur Netztrennung
* **BPDU Guard** gegen fehlerhafte STP-Geräte

### Router-Sicherheit

* SSH statt Telnet
* ACLs (Access Control Lists)
* Firewall-Funktionen
* Sichere Managementvorgänge: Benutzerrechte, Logging

---

## ✔ 1.6 Symbole in Netzwerkschemata

| Symbol | Bedeutung         |
| ------ | ----------------- |
| ◯ →↔   | Router            |
| ▭▭▭    | Switch            |
| 🔒🧱   | Firewall          |
| 🖥️    | PC/Client         |
| 📡     | WLAN Access Point |
| 🗄️    | Server            |

Diese Symbole erleichtern das Skizzieren von Netzwerkdiagrammen für Projekte oder Prüfungen.

---

Wenn du möchtest, erstelle ich dir jetzt:

* **Merkblatt 2 (Subnetting & Adressschema)**
* **Merkblatt 3 (Router/Switch Konfiguration + Beispiele)**
* **Zusätzliche Grafiken oder Tabellen**

Sag mir einfach: *"Bitte Merkblatt 2"* oder *"Alle weiteren bitte erstellen"*!
