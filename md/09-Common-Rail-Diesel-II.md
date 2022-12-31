---
title: 'Common-Rail-System'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!-----------------------------
Quelle: Europa-Verlag
ju 5-10-22 Common-Rail-System
+------------------------------>

# Bauteile und Aufgaben eines Common-Rail Systems

<!--CR-6 vgl. abb.-->
![Common-Rail System, Quelle: Europa-Verlag](images/Diesel/Diesel-6.pdf){width=70%}

1. **Hochdruckpumpe** Kraftstoff unter Hochdruck in das Rail fördern.
1. **Raildruckregelventil** den erforderlichen Hochdruck an jeden Betriebszustand anpassen.
1. **Rail** Hochdruck speichern und Verteilung des Kraftstoffs auf die Injektoren.
1. **Raildrucksensor** Hochdruck erfassen und als elektrisches Signal an das Steuergerät weiterleiten.
1. **Injektor** Kraftstoff dosiert in den Brennraum spritzen
1. Saugrohrtemperaturfühler
1. Bremspedalschalter
1. **Vorförderpumpe,** Kraftstoff zu Hochdruckpumpe fördern.

**Laufruheregelung**, die einzelnen Zylinder bekommen mehr oder weniger Kraftstoff vom Steuergerät zugeteilt.

# Welche Ursachen kommen für den Leistungsverlust infrage?

1. **Mechanische Fehler**
    - Kompressionsverlust durch Verschleiß der Ventile oder Kolben
    - Verschleiß der Hochdruckpumpe
1. **Fehler im hydraulischen System**
    - Undichtigkeit an Injektoren (schließt nicht korrekt, tropft nach, Düse ausgewaschen)
    - Undichte Leitungen am Rail
1. **Elektrische Fehler**
    - Sensoren defekt
    - Aktoren defekt
    - Leitungsunterbrechung
    - Masseschluss

# Was muss beachtet werden beim Einbau eines neuen Injektors?

- Fertigungstoleranz: muss im Steuergerät einprogrammiert werden
- Zahlen- und Buchstabencodes auf dem Injektor
- Steuergerät korrigiert entsprechend die Grundeinspritzmenge des jeweiligen Injektors.

\newpage
# Welche Druckregelungsarten gibt es? (Prüfung)

<!--CR-2 vgl. abb.-->
![CR-Einsteller- und Zweistellerregelung, Quelle: Europa-Verlag](images/Diesel/Diesel-2.pdf){width=80%}


1. **Einsteller-Regelung**
    - **Druckregelung hochdruckseitig** über ein **Druckregelventil** (DRV)
        - Hochdruckpumpe fördert die maximale Fördermenge unabhängig von Bedarf an Kraftstoff
        - Raildruck wird über ein **Druckregelventil** geregelt, nicht benötigter Kraftstoff fließt zurück in den Tank
        - **Vorteil**
            - schneller Druckaufbau möglich
            - bei Lastwechsel agil
        - **Nachteil:** Hochdruckpumpe ist konstant maximal belastet, dadurch 
            - geringere Nutzleistung
            - erhöhter Kraftstoffverbrauch, Schadstoffausstoß, Verschleiß 
            - unnötige Erwärmung des Kraftstoffs 
    - **Druckregelung niederdruckseitig** (Mengenregelung) über eine **Zumesseinheit** (ZME)
        - **Zumesseinheit** regelt die Zuflussmenge zur Hochdruckpumpe
        - **Bedarfsregelung**, d.h. es gelangt nur so viel Kraftstoff zu Hochdruckpumpe wie für die Einspritzung benötigt wird 
        - **Druckbegrenzungsventil** verhindert zu hohen Raildruck bei Ausfall der Zumesseinheit
        - **Vorteil**
            - bedarfsgerechte Förderung
            - geringe Leistungsaufnahme der Pumpe
        - **Nachteil:** 
            - hohe Trägheit
            - Drucksteigerung erfordert zunächst eine Erhöhung des Niederdrucks, dadurch erhöhte Förderleistung der Hochdruckpumpe

1. **Zweisteller - Regelung** (**Druckregelung nieder- und hochdruckseitig**)
    - Zusammenspiel von Zumesseinheit (ZME) und Druckregelventil (DRV) 
    - **Vorteile**
        - geringe Leistungsaufnahme der Hochdruckpumpe bei konstant hohen Drücken
        - hohe Agilität bei geringen Drücken
    - **Kaltstart / Motorstart und Warmlaufphase** (angesteuert: **DRV**) "Druckregelung hochdruckseitig geregelt"
        - Schneller Druckaufbau möglich. Bessere Kraftstoffvorwärmung. Verzicht auf Kraftstoffheizung möglich.
        - Kraftstoff soll sich erwärmen, um ihn damit fließ- und zündfähiger zu machen
    - **betriebswarmer Motor: Leerlauf / Teilllast / Schub** (angesteuert: **DRV und ZME**) "Zweisteller-Betrieb"
        - große Sprünge des Raildrucks sind wahrscheinlich (zwischen Motor im Leerlauf / Teillast und $\to$ Lastwunsch des Fahrers bei Volllast)
        - Raildruckregelung bei reduzierter Leistungsaufnahme der Pumpe
    - **hohen Motorlast** (angesteuert: **ZME**) "Druckregelung niederdruckseitig geregelt"
        - große Steigerungen des Raildrucks nicht möglich und deshalb ist die Trägheit vernachlässigbar
        - Reduzierter Leistungsaufnahme der Pumpe. Gesamte Kraftstoffmenge der Pumpe wird eingespritzt.

\newpage
**Schaltstellung der Zumesseinheit an der Hochdruckpumpe in Bezug auf die Fördermenge.**

<!--CR-3 vgl. abb.-->
![CR-Zumesseinheit, Quelle: Europa-Verlag](images/Diesel/Diesel-3.pdf){width=80%}

1. **Zumesseinheit unbestromt**: Maximale Fördermenge
1. **Zumesseinheit bestromt**: verringert den Öffnungsquerschnitt für minimale Fördermenge  

**Druckregelventil** Druckerfassung durch Membransensor am Rail (Raildrucksensor)

<!--CR-8 vgl. abb.-->
![CR-Druckregelventil (DRV), Quelle: Europa-Verlag](images/Diesel/Diesel-8.pdf){width=30%}

*Ansteuerung:* Das Steuergerät taktet das Druckregelventil mit einem PWM-Signal an. Dadurch wird die Schließkraft der Ventilnadel erhöht oder gesenkt. Dementsprechend wird der Raildruck erhöht oder gesenkt.


1. **Magnetventil unbestromt / stromlos** Raildruck etwa $100~\text{bar}$
    - Motor abstellen, Ventilfeder hält Druckregelventil geschlossen, verhindert ein Leerlaufen des Rails

1. **Magnetventil bestromt** Raildruck bei verschiedene Lastzuständen:
    - **Motorstart** Raildruck $> 250~\text{bar}$ (Wie hoch ist der Druck im Rail bei Motorstart?)
    - **Leerlauf** Raildruck etwa $400~\text{bar}$
    - **Volllast** Raildruck etwa $2000~\text{bar}$ 

\newpage
**Warum lässt sich ein Fahrzeug mit defektem Druckregelventil nicht mehr starten?**

<!--CR-4 vgl. abb.-->
![CR-DRV Motor aus, Quelle: Europa-Verlag](images/Diesel/Diesel-4.pdf){width=30%}

Durch die im Druckregelventil verbaute Feder verbleibt im Rail ein **Restdruck** von ca. 100 bar. Da für einen **sicheren Motorstart** der Druck im Rail mind. 250 bar betragen muss, ist ein Motorstart nicht möglich.

Ist die **ZME** defekt, übernimmt das **DRV** die Druckregelung.

\newpage
# Injektoren

**Unterschied zwischen Injektoren und Einspritzdüsen** haben keinen festen Öffnungsdruck, sondern öffnen und schließen unter dem jeweiligen variablen Einspritzdruck.

Kraft = Druck x Fläche


## Erklären Sie die Funktionsweise eines Magnetventil-Injektor im geschlossenen und geöffneten Zustand.

<!--CR-7 vgl. abb.-->
![CR-Magnetventil-Injektor, Quelle: Europa-Verlag](images/Diesel/Diesel-7.pdf){width=30%}

1. Rücklauf
1. Magnetventil
1. Zulauf von dem Rail
1. Ventilsteuerraum
1. Druckschulter
1. Zulaufdrossel
1. Düsennadel
1. Abflussdrossel


- **Magnetventil unbestromt - geschlossenen Zustand** dann wirkt im Ventilsteuerraum auf der Stirnfläche des Ventilsteuerkolbens und auf der Druckschulter der Düsennadel gleicher Kraftstoffdruck. Einspritzventil ist geschlossen.

- **Magnetventil bestromt - geöffneten Zustand,** dann wird der Rücklauf geöffnet. Über die Ablaufdrossel entweicht mehr Kraftstoff, als über die Zulaufdrossel abfließen kann. Es kommt zum Druckabfall im Ventilsteuerraum. Der Druck auf die Druckschulter der Düsennadel öffnet die Düse.

**Ansteuerung eines Magnetventil-Injektors (Spannungs- und Stromverlauf)**

Die Injektorspannung / Boosterspannung beträgt in der Anzugsphase ca. 100 V. Der Anzugsstrom liegt dadurch bei ca. 20 A. Danach wird der Strom auf ca. 13 A begrenzt (Haltestrom), bei einer Spannung von 12 -- 14 V (Batteriespannung). 

**Wie entsteht die Injektorspannung / Boosterspannung bis ca. 100 V?**

Beim Ausschalten der Magnetventile wird die entstehende Selbstinduktionsspannung genutzt, um im Steuergerät einen Kondensator aufzuladen.

\newpage
## Erklären Sie die Funktionsweise eines Piezoinjektor

Piezoinjektoren erlauben hohe Schaltgeschwindigkeiten und damit viele Teileinspritzungen.

<!--CR-1 vgl. abb.-->
![CR-Piezoinjektor, Quelle: Europa-Verlag](images/Diesel/Diesel-1.pdf){width=30%}

1. Zulaufdrossel
1. Piezo-Aktormodul
1. Rücklauf
1. Hydraulischer Koppler
1. Düsennadel
1. Ablaufdrossel
1. Zulauf mit Raildruck
1. Servoventil

**Einspritzvorgang**

1. Piezo-Aktormodul wird bestromt und dehnt sich aus
1. Über den hydraulischen Koppler findet eine Hubvergrößerung statt.
1. Der hydraulischen Koppler öffnet das Servoventil und damit den Rücklauf.
1. Über die Ablaufdrossel fließt Kraftstoff aus dem Ventilsteuerraum ab.
1. Über die Zulaufdrossel kann weniger Kraftstoff in den Ventilsteuerraum zufließen. Es kommt zum Druckabfall.
1. Der Druck auf die Druckschulter der Düsennadel öffnet die Düsennadel des Injektors. Einspritzbeginn.


**Hydraulische Koppler vergrößert den Weg des Piezo-Aktormoduls auf das Servoventil**

<!--CR-9 vgl. abb.-->
![CR-Piezoinjektor - hydraulicher Koppler, Quelle: Europa-Verlag](images/Diesel/Diesel-21.pdf){width=30%}

Er besteht aus zwei Kolben mit unterschiedlichen Durchmessern. Das Piezo-Aktormodul drückt mit kleinem Hub auf den großen Kolben, dadurch wird der kleine Kolben mit einem großen Hub bewegt.

**Reziproker Piezoelektrischer-Effekt** (invers) legt man an einen Piezokristall eine Spannung an, so verformt er sich. Die Längenänderung ist proportional zur angelegten Spannung. Bleibt in Position bis Kurzschluss.

*Verformung* durch Spannungseinfluss

*Anwendung:* Injektor

**Ansteuerung eines Piezoinjektors** 110 -- 150 V bei ca. 13 A, Piezoaktormodul dehnt sich aus (am Ende vergleichbar mit geladenen Kondensator) *Injektor offen:* Stromaufnahme null *Injektor geschlossen:* SG schaltet Spannung ab und schließt Stromkreis über Widerstand kurz. Piezoaktormodul entlädt sich und zieht sich zusammen.

Piezoventil ersetzt Magnetventil (Grund: durch Trägheit $\to$ Magnetventil bewegt sich zeitversetzt, weil der Magnetfeldaufbau gehemmt wird, durch Gegeninduktion)

**Piezoventil (Piezoaktor)** besteht aus Piezoaktormodul und Übersetzermodul (kl. Hebelwerk)

Die Längenausdehnung eines Piezokristalls liegt bei maximal 0,15 \% (sehr gering). Werden, bis zu 500 Piezokristalle in Reihe geschaltet ist die Gesamtausdehnung des Piezoaktormodul etwa 0,04 mm. Zum Erreichen der erforderlichen Ventilöffnung von 0,1 mm wird ein kleines Hebelwerk, sogenannte Übersetzermodul zwischen Piezoaktormodul und hydraulischen Ventil geschaltet.

