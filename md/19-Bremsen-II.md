---
title: 'Bremsen II'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!------------------------------------------------------------------------+
![Bremsen, Quelle: Europa-Verlag](images/Bremsen/Bremsen-1.pdf){width=70%} 
ju 24-12-22  Bremsen II
--------------------------------------------------------------------------->

# Grundlagen der Fahrdynamikregelung

**Kammscher Reibkreis**, die größte auf die Straße übertragbare Kraft wird als Kreis dargestellt.

Die Kraft, die ein Rad maximal übertragen kann, setzt sich aus der Aufstandskraft des Rades und der Haftreibung zwischen Reifen und Fahrbahn zusammen.

- *Innerhalb des Kreises* Kräfte übertragen
- *Außerhalb des Kreises* Schlupf
- $F_\text{max} = F_N \cdot \mu_H$ (Antriebskraft, Bremskraft, Normalkraft, Haftreibungszahl)
- $\mu = 0,1$ Eis
- **stabilen Fahrzustand** Resultierende Kraft aus Umfangskraft und Seitenführungskraft muss innerhalb des Kreises liegen
- **durchdrehende oder blockierende Räder**
    - Umfangskraft max. und 
    - Seitenführungskraft 0
    - Fahrzeug ist nicht mehr lenkbar
- **max. Kurvengeschwindigkeit**
    - Seitenführungskraft max.
    - Fahrzeug kann weder gebremst noch beschleunigt werden (würde ausbrechen)

**Schlupf**

Das Verhältnis der Fahrgeschwindigkeit zu Radumfangsgeschwindigkeit oder das Verhältnis der tatsächlich zurückgelegten Wegstrecke zum dynamischen Abholumfang. (blockiert ein Rad, dann ist der Schlupf 100 \%)

**dynamischen Abrollumfang**

- Reifenaufstandsfläche = Latsch 
- Wenn sich das Rad dreht, verändert sich der Reifenumfang, als wenn das Fahrzeug steht. 
- Verlängerung des Weges durch Schlupf oder Verformung des Reifens.

**Typgenehmigung** für ABS nein und ESP ja


# ABS

**ABS-Arbeitsbereich**

**stabilen Bereich**, um ein ausreichendes Maß an Seitenführungskraft bereitstellen zu können. Zwischen 8 -- 35 \% Schlupf.

**ABS-Aufgaben**

- Erhalt der Seitenführungskraft durch Begrenzung der maximalen Bremskraft
- Vermeidung von Bremsplatten

**Maximale Bremskraft** Übergang von Haftreibung zur Gleitreibung

**ABS-Funktion**

- Erfassen der Raddrehzahlsignale, die miteinander verglichen werden
- weicht ein Rad ab und bei kritischen Schlupfwerten
- wird die Bremskraft begrenzt durch **3x Regelphasen**
- Regelzyklus 4 -- 10x pro Sekunde (10 Hz)

1. **Druck halten**
    - Einlassventil wird geschlossen und Druck an Radbremse konstant gehalten.
1. **Druck ablassen**
    - Auslassventil wird geöffnet und Bremsdruck wird gesandt.
1. **Druck aufbau**
    - Sinkt der Schlupf auf unkritischer Werte, öffnet das Einlassventil und wird mit maximaler Bremskraft verzögern.

**Regelungsarten des ABS**

1. **Select-Low-Regelung** (HA)
    - Das Rad mit der geringeren Bodenhaftung bestimmt den gemeinsamen Bremsdruck einer Achse.

2. **Individualregelung** (VA)
    - wird jedem Rad die maximale übertragbare Bremskraft zugeteilt. 
    - Unterschiedliche Bremskräfte wirken.
        - Ein Giermoment entsteht in Richtung des Rades mit der größeren Haftung. Kann durch Gegenlenken, ausgeglichen werden. (Vgl. Negativer Lenkrollradius)

**Negativer Lenkrollradius** (Lenkrollhalbmesser) an Vorderachse

Erzeugt ein automatisches Gegenlenken, d.h. der Reifen schwenkt nach innen an der Vorderachse.

**ABS-Sensoren** 

- Geschwindigkeit von ca. 6 km/h notwendig
- Induktiv-Sensor (Bosch: passiv)
    - Spule und Magnetfeld $\to$ Wechselspannung
- Hall-Sensor  (Bosch: aktiv)
    - eigene Spannungsversorgung 
    - Kabel kann 2-adrig sein (Masseleitung = Signalleitung)
    - Stromsignal an SG
    - Prüfen: Strommessung

**Regelkanäle von ABS**

1. 2 Kanal ABS-System (VA und HA)
1. 3 Kanal ABS-System (VA rechts + links und HA)
1. 4 Kanal ABS-System (4S4M, Sensoren und Modulatoren)

# ASR

Erfassung des Radschlupfs an den Antriebsrädern durch Abgleichen der Drehzahlsignale. Bei kritischen Schlupfwerten begrenzen der Antriebskraft durch Verringern des Motordrehmoments oder Bremseingriff.

# FDR / ESP

Fahrdynamische Prozesse erfassen und autonom regeln.

**Systeme**

1. (+) Antiblockiersystem (ABS)
1. (+) Elektronische Bremskraftverteilung (EBV)
1. (+) Antriebsschlupfregelung (ASR) mit Motorschleppmoment-Regelung (MSR)
1. (+) Giermomentregelung (GMR)
1. (=) Fahrdynamikregelsystem (FDR) = Elektronisches Stabilitätsprogramm (ESP)

**Komponenten**

1. Hydraulikeinheit
1. Lenkwinkelsensor
1. Tandem-Hauptzylinder mit Drucksensoren
1. Querbeschleunigungs- und Gierratensensor
1. Raddrehzahlsensor
1. Motormanagement

**Gierratenerfassung**

Erfassen der Drehbewegung des Fahrzeugs um seine eigene Hochachse mithilfe der Corioliskraft (Piezo-Element wird gestaucht oder gestreckt $\to$ SG).

**Bewegungen und Kräfte des Fahrzeugs**

1. Hochachse - Gieren (Schleudern, Drehbewegung)
    - Radlast, Kräfte durch Fahrbahnunebenheiten

1. Längsachse - Wanken (Kippbewegung)
    - Antriebskraft, Bremskraft, Reibungskraft

1. Querachse - Nicken (Drehbewegung)
    - Fliehkraft, Seitenwindkraft, Seitenführungskraft