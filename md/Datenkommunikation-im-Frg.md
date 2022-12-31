---
title: 'Datenkommunikation im Fahrzeug'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!------------------------------------------------------------------------+
![ . (Bild: Kai Borgeest)](images/CAN/CAN-1.pdf){width=70%} 
(Bild: Kai Borgeest)
(Foto: Robert Bosch GmbH)
Quelle: S. 105 [@borgeest:2021:elektronik].
ju 18-12-22 Datenkommunikation im Fahrzeug
+-------------------------------------------------------------------------->
# Bordelektrik 

## Bordnetz

![Überblick über das Bordnetz. (Bild: Kai Borgeest)](images/CAN/CAN-1.pdf){width=70%}

**Leitungen**

Um eine unzulässige Erhitzung von Kabeln im normalen Betrieb zu verhindern, darf die zulässige Stromdichte S nicht überschritten werden.

$S = \frac{I}{A}$ (Stromdichte S, Strom I und dem Leitungsquerschnitt A) 

**grobe Richtwerte für zulässige Stromdichten**

- Dauerbetrieb $5~A/mm^2$ 
- kurzzeitige Stromspitzen $10~A/mm^2$


Wird die zulässige Stromdichte überschritten, führt die Verlustleistung $P_V$ in der Leitung zu einer Überhitzung und damit zum Schmelzen, zur Zersetzung oder zum Brennen des Isoliermaterials oder angrenzender Strukturen, bei erheblicher Überlast auch zum Schmelzen des Leiters. 

**Verlustleistung beim Strom I**

$P_v = I^2 \cdot R \quad R = \frac{\rho \cdot l}{A}$ (Kupferleitung $0,0185~\Omega mm^2/m$)

$I = \frac{P}{U}$

\newpage
**elektrischer Verbraucher 12-V-Bordnetz**

**Verbraucher**         | **Leistungsaufnahme P** | **Strom I**
------------------------|-------------------------|------------
Elektro-Kraftstoffpumpe | 250 W                   | 21
Heckscheibenheizung     | 200 W                   | 17
Innengebläse            | 120 W                   | 10
Kühlerventilator        | 120 W                   | 10
Abblendlicht            | 110 W                   | 9,2
Scheibenwischer         | 50  W                   | 4,2
Bremslicht              | 42  W                   | 3,5
Kennzeichenleuchte      | 30  W                   | 2,5
Standlicht              | 8   W                   | 0,7

**Elektro- und Hybridfahrzeugen**

Ab 60 V hat sich der Begriff Hochvoltkabel durchgesetzt. Hochvoltkabel haben eine geerdete Abschirmung, sind mechanisch besonders stabil und durch ihre orange Farbgebung auffällig gekennzeichnet. 

Hochvoltkomponenten werden durch eine ringförmige Niederspannungsleitung verbunden (HVIL, High Voltage Interlock Loop), die auf Unterbrechungen überwacht wird. Wird eine Unterbrechung durch Trennung einer Leitung oder Öffnung eines Gehäuses erkannt, führt dies zur Abschaltung des Hochvoltsystems.

**Klemmenbezeichnungen** (Auswahl)

**Nr.**  | **Bezeichnung**
---------|------------------------------------------------------------------
1        | Zündspule (gemeinsame Klemme)
4        | Zündspule (Hochspannungsausgang)
15       | Positive Batteriespannung, über Schlüsselschalter
30       | Positive Batteriespannung
31       | Negative Batteriespannung
50       | Anlasser (geschaltete Klemme)
54 -- 58 | Beleuchtung
81 -- 88 | Schalter und Relais
B+       | Positive Generatorklemme zur Batterie
B        | Negative Generatorklemme zur Batterie
D+       | Positive Klemme an Generator und Regler für Regelung und Leuchte
D        | Negative Klemme an Generator und Regler für Regelung und Leuchte
DF       | "Dynamo Feld", Klemme an Generator und Regler für Erregerwicklung
U, V, W  | Drehstromklemmen des Generators

\newpage
## Mehrspannungsbordnetzes

In Zukunft ist mit neuen Fahrzeugsystemen wie "Brake-by-Wire" oder "Steer-by- Wire" zu rechnen, die einen hohen Bedarf an elektrischer Energie haben. Damit steigen auch die Ströme im Bordnetz an und so quadratisch die Leitungsverluste.
Durch Einsatz einer höheren Bordnetzspannung kann die gleiche Leistung mit reduzierten Strömen übertragen werden. Je höher die Spannungen sind, umso geringer werden die Leitungsverluste.

![Struktur eines künftigen Mehrspannungsbordnetzes (Bild: Kai Borgeest)](images/CAN/CAN-2.pdf){width=70%}

Kombination aus einem 12-V-Netz für Kleinverbraucher und einem 48-V-Netz für Großverbraucher. Beide Netze werden über einen Schaltwandler (DC/DC) gekoppelt.

\newpage
## Energiemanagement (BMS)

1. Batterieüberwachung 
    - Eingriff in die Laderegelung 
    - Eingriff in das Motormanagement, um zum Aufladen der Batterie eine Mindestdrehzahl zu erzwingen. 
    - Ziele
        1. Bestimmung des Ladezustandes (State of Charge, SOC)
        1. Restlebensdauer der Batterie (State of Health, SOH)
        1. Funktionsfähigkeit der Fahrzeugfunktionen, vor allem des Startens (State of Function, SOF).

1. automatisch Verbraucher je nach Wichtigkeit und Leistungsbedarf abzuschalten oder auch wieder einzuschalten. 

1. Steuerung eines hybriden Antriebssystems


**Energiemanagement-Steuergerät / Bordnetzsteuergerät** benötigt von der Batterie Informationen über Temperatur, Spannung und Strom.

**Batterietyp** über Diagnosetester dem Energiemanagement mitteilen, welcher eingebaut wurde. 

**Fremdstartbolzen** der bei Starthilfe anstelle des Batterie-Minuspols zu verwenden ist, damit das Steuergerät den Fremdstart registriert und bei seinen Berechnungen berücksichtigt. 

**schweren Unfall** (Signal vom Airbag-Steuergerät) über ein Relais das Bordnetz spannungsfrei schaltet.

Bei großen Batterien für Hybrid- und Elektrofahrzeuge werden wesentliche Teile des Energiemanagements in die Batterie integriert.

\newpage
# CAN-Bus 

CAN-Bus war das erste digitale Bussystem.


![Ein kleiner Ausschnitt aus der Kommunikationsmatrix zwischen vier Steuergeräten (Bild: Kai Borgeest)](images/CAN/CAN-3.pdf){width=70%}

![Vier über einen Bus kommunizierende Steuergeräte (Bild: Kai Borgeest)](images/CAN/CAN-4.pdf){width=70%}


\newpage
**Transceiver** ein Kunstwort aus Transmitter/Receiver, also Sender/Empfänger

![Umsetzung des OSI-Modells durch die verwendeten Bauelemente. Der CAN-Controller erzeugt eine Nachricht mit dem gewünschten Inhalt und sendet sie über die Leitung Tx an den Transceiver. Wenn auf dem Bus eine Nachricht erscheint, schickt er diese über die Rx-Leitung an den CAN-Controller, der wiederum Teil eines Mikrocontrollers sein kann, aber nicht sein muss. Die Bezeichnungen CAN_H und CAN_L stehen für "CAN high" und "CAN low". (Bild: Kai Borgeest)](images/CAN/CAN-5.pdf){width=50%}

\newpage
## Spannungspegel und Störsicherheit

Zwei verdrillte Adern stellt einen sinnvollen Kompromiss zwischen Störfestigkeit und Kosten dar. Das Signal wird über beide Leitungen entgegengesetzt übertragen.

**logische 1** soll gesendet werden, wird der Tx-Eingang des Transceivers
vom Controller mit einer Spannung von z. B. 5 V angesteuert. Der untere PNP-Transistor
sperrt, der obere NPN-Transistor bekommt das invertierte Signal und sperrt ebenfalls. Der
Bus behält seine Ruhespannung von 2,5 V auf beiden Leitungen, die Spannungsdifferenz
zwischen den Busleitungen CAN_H und CAN_L ist 0. Die Sendeschaltung muss nicht
wie hier gezeigt mit NPN- und PNP-Transistoren aufgebaut werden, sondern kann auch
mit Feldeffekt-Transistoren (FET) realisiert werden.

**logischen 0** leiten beide Transistoren, also wenn der Controller
das Signal am Tx-Eingang auf 0 V legt. In diesem Falle wird die Spannung auf CAN_H
erhöht, die Spannung auf CAN_L gesenkt. 

- **CAN_H** oder "CAN high" für Anhebung 
- **CAN_L** oder "CAN low" für Absenkung

\newpage
**High-Speed-CAN**

- 3,5 V auf dem CAN_H und 
- 1,5 V auf CAN_L
- Ruhespannung von 2,5V wird über hohe Widerstände (einige 10 -- 100 $k\Omega$) auf beide CAN-Leitungen gelegt, damit sich die Spannung auf den Busleitungen beim Durchschalten der Transistoren verändern kann. 

![Elektrische Ansteuerung und Auswertung des CAN-Busses im Transceiver (vereinfacht). Links ist der Sender, rechts daneben der Empfänger eingezeichnet. Ganz rechts ist klein die Erzeugung des Ruhepotentials von 2,5V (in vielen Highspeed-CAN-Transceivern integriert) angedeutet (Bild: Kai Borgeest)](images/CAN/CAN-6.pdf){width=50%}

Der Empfänger vergleicht die Spannungen auf CAN_H und CAN_L. Bei einer logischen 1 liegen beide CAN-Leitungen auf 2,5 V, die Differenz ist 0. Der nachfolgende Inverter erzeugt aus dieser 0 wieder eine 1. Bei einer logischen 0 ist zwischen den Spannungen eine Differenz von 2 V vorhanden. Wenn die Differenzspannung einen sicheren Minimalwert (z. B. 1 V), überschreitet, wird dies zunächst durch eine 1 signalisiert, aus welcher der Inverter wieder die ursprüngliche 0 erzeugt.

**Low-Speed-CAN** 

- Ruhespannung und rezessive Spannung
    - 5 V am CAN_L
    - 0 V am CAN_H 

- dominante Spannung am 
    - 1,4 V oder kleiner CAN_L 
    - 3,6 V oder größer am CAN_H

**Ist eine der beiden Leitungen defekt**, kann sie abgeschaltet werden (Fault
Tolerant CAN). Der symmetrische Betrieb wird dann verlassen, indem die verbleibende
Leitung gegen Masse betrieben wird.

**Wake-Up** (Aufwecken) Low-Speed-CAN-Transceiver können in einen Bereitschaftszustand gehen, in dem der Sendeteil abgeschaltet ist, der Empfangsteil aber bereit bleibt, um ein  durch Kommunikation auf dem Bus oder Aktivierung eines Pins zu ermöglichen.

**Energieeinsparung** wird ein Teilnetzbetrieb (Partial Networking), bei dem Steuergeräte, die gerade keine Funktion erfüllen, ihren Energieverbrauch reduzieren, immer wichtiger. Dieser benötigt ein selektives Aufwecken einzelner Busteilnehmer.

\newpage
## Wellenwiderstand und Abschluss

**Wellenwiderstand** sagt aus, welchen fiktiven Widerstand ein Signal am Eingang einer Leitung "sieht" und damit, welchen Strom die Quelle in die Leitung einspeist. Ist eine Kenngröße jeder Leitung, also jedes Leiterpaares.

Wird eine Leitung nicht mit ihrem Wellenwiderstand abgeschlossen, kommt es zu Reflexionen des Signals an ihren Enden. 

1. **Leitung an den Enden offen zu lassen**
    - kann vorkommen, wenn am Ende der Leitung sich ein Steuergerät befindet, dessen Transceiver einen hohen Eingangswiderstand hat (was durchaus üblich ist). In diesem Falle käme es zu einer Reflexion, das Signal würde die Leitung wieder zurücklaufen und sich mit anderen hinlaufenden Signalen überlagern. Damit würden andere Steuergeräte am Bus im schlimmsten Fall einen undefinierten Datenzustand empfangen, die Kommunikation auf dem Bus kann zusammenbrechen.

1. **Leitung an den Enden kurz zuschließen** 
    - kommt nur bei Fehlern vor



**High-Speed-CAN** an beiden Enden mit je einem Widerstand von nominal
120 $\Omega$ abgeschlossen, dies entspricht näherungsweise dem Wellenwiderstand der
verdrillten 2-Draht-Leitung. Um Störströme gezielt abzuleiten, werden oft zwei Widerstände
zu 60 $\Omega$ in Reihe geschaltet und der Knoten zwischen den beiden Widerständen
über einen Kondensator von wenigen nF auf Masse gelegt. 

Zweckmäßigerweise wird man diese beiden Widerstände nicht direkt
in den Kabelbaum einbauen, sondern in die an beiden Busenden sitzenden Steuergeräte.

**Low-Speed-CAN** üblich, in jedem Knoten Widerstände jeweils gegen Masse und Versorgungsspannung vorzusehen. Hersteller empfehlen Gesamtabschlusswiderstände des Netzwerkes (Parallelschaltung aller einzelnen Abschlüsse) zwischen 100 $\Omega$ und darüber. Der optimale Abschlusswiderstand steigt also mit der Anzahl der elektrisch parallel geschalteten Knoten im Netzwerk.

\newpage
## Verbindung von Steuergeräten

![CAN-Bus mit sternförmiger Anbindung (passiver Stern) (Bild: Kai Borgeest)](images/CAN/CAN-7.pdf){width=50%}


1. **passive Stern**
    - wird häufig in der Nähe des Armaturenbretts realisiert, evtl. existieren auch mehre Sternpunkte. 
    - Vorbildlich hat z. B. Audi beim A6 und beim A8 die Sternpunkte realisiert. Sämtliche Zugänge treffen sich an den beiden Seiten des Armaturenbrettes, die Verbindungen erfolgen über Brückenstecker.

1. **aktiver Stern** bei dem sich ein weiteres Gerät im Sternpunkt befände, um jede Verzweigung mit einem eigenen Transceiver anzusteuern.
    - Gateway (aktiver Stern) eines Oberklasse-Fahrzeugs mit vier High-Speed-Transceivern (HS) und einem Low-Speed-Transceiver (LS) für den langsameren Komfort-CAN. Eine CPU (Mikrocontroller) kann gezielt Nachrichten aufarbeiten und an andere Busse weiterleiten.

    1. High-Speed-Transceivern (HS)
        - Antriebs-CAN
        - Kombi-CAN
        - ACC-CAN
        - Diagnose-CAN

    1. Low-Speed-Transceiver (LS)
        - Komfort-CAN

![Gateway (aktiver Stern) eines Oberklasse-Fahrzeugs mit vier High-Speed-Transceivern (HS) und einem Low-Speed-Transceiver (LS) für den langsameren Komfort-CAN. Eine CPU (Mikrocontroller) kann gezielt Nachrichten aufarbeiten und an andere Busse weiterleiten. (Bild: Kai Borgeest)](images/CAN/CAN-8.pdf){width=50%}

Inzwischen ist es üblich, in einem Fahrzeug mehrere elektrisch getrennte CAN-Busse
zu haben, die sich auch in ihren Datenraten unterscheiden können, aber nicht müssen. Verbunden sind diese dann über einen aktiven Sternpunkt, der auch als Gateway bezeichnet
wird. Während bei Systemen von geringer Komplexität (bis ca. 5 Steuergeräte
im Fahrzeug) evtl. auf ein Gateway verzichtet wird, besitzen Systeme von mittlerer
bis hoher Komplexität (ab ca. 50 Steuergeräte im Fahrzeug) auf jeden Fall eines. Das
Gateway kann eine zusätzliche Funktion eines möglichst zentralen Steuergerätes, z. B.
des Kombiinstruments sein, mit zunehmender Komplexität verwendet man als Gateway
ein eigenständiges Gerät, welches nur diese Aufgabe verrichtet.



