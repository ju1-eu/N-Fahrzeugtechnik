---
title: 'Common-Rail-Einspritzung'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!-----------------------------
Quelle: Europa-Verlag SimKfz
![, Quelle: Europa-Verlag SimKfz](images/CR/.png){width=70%}

Quelle: Europa-Verlag Arbeitsblätter Kfz-Technik
ju 16-9-22 Common-Rail-Einspritzung
+------------------------------>


![Common Rail, Quelle: Europa-Verlag SimKfz](images/CR/Common-Rail.png){width=70%} 

**Bauteile und Aufgaben**

1. **Elektrische Kraftstoffpumpe** Kraftstoff zu Hochdruckpumpe fördern.
1. **Hochdruckpumpe** Kraftstoff unter Hochdruck in das Rail fördern.
1. **Rail** Hochdruck speichern und Verteilung des Kraftstoffs auf die Injektoren.
1. **Druckregelventil** den erforderlichen Hochdruck an jeden Betriebszustand anpassen.
1. **Raildrucksensor** Hochdruck erfassen und als elektrisches Signal an das Steuergerät weiterleiten.
1. **Injektor** Kraftstoff dosiert in den Brennraum spritzen


**Welche Ursachen kommen für den Leistungsverlust infrage?**

1. **Mechanische Fehler**
    - Kompressionsverlust durch Verschleiß der Ventile oder des Kolbens
    - Verschleiß der Hochdruckpumpe
1. **Fehler im hydraulischen System**
    - Undichtigkeit an Injektoren (schließt nicht korrekt, tropft nach, Düse ausgewaschen)
    - Undichte Leitungen am Rail
1. **Elektrische Fehler**
    - Sensoren defekt
    - Aktoren defekt
    - Leitungsunterbrechung
    - Masseschluss

**Laufruheregelung**, die einzelnen Zylinder bekommen mehr oder weniger Kraftstoff vom Steuergerät zugeteilt.

**Was muss beachtet werden beim Einbau eines neuen Injektors?**

- Fertigungstoleranz: muss im Steuergerät einprogrammiert werden
- Zahlen- und Buchstabencodes auf dem Injektor
- Steuergerät korrigiert entsprechend die Grundeinspritzmenge des jeweiligen Injektors.

**Erkläre den Spannungs- bzw. Stromverlauf eines intakten Injektors**

- Injektorspannung beträgt in der Anzugsphase ca. 80 V. Der Anzugstrom liegt dadurch bei ca. 20 A. Danach wird der Strom auf ca. 12 A begrenzt (Haltestrom), bei einer Spannung von 12 V bis 14 V.

**Wie entsteht die Injektorsspannung von 80 bis 100 V?**

- Beim Ausschalten der Magnetventile wird die entstehende Induktionsspannung genutzt, um im Steuergerät einen Kondensator aufzuladen.

\newpage
**Welche Druckregelungsarten gibt es?**

1. **Einsteller-Regelung**
    - **Druckregelung hochdruckseitig** (Druckregelung)
        - Hochdruckpumpe fördert die maximale Fördermenge unabhängig von Bedarf an Kraftstoff
        - Raildruck wird über ein Druckregelventil geregelt, nicht benötigter Kraftstoff fließt zurück in den Tank
        - **Nachteil:** Hochdruckpumpe ist konstant maximal belastet, dadurch 
            - geringere Nutzleistung
            - erhöhter Kraftstoffverbrauch, Schadstoffausstoß, Verschleiß 
            - unnötige Erwärmung des Kraftstoffs 
    - **Druckregelung niederdruckseitig** (Mengenregelung)
        - Raildruck wird über eine Zumesseinheit an der Hochdruckpumpe niederdruckseitig geregelt
        - Bedarfsregelung es gelangt nur so viel Kraftstoff zu Hochdruckpumpe wie benötigt wird für die Einspritzung
        - Zumesseinheit regelt die Zuflussmenge zur Hochdruckpumpe
            - Mengenregelventil unbestromt: voll offen für maximale Fördermenge
            - Mengenregelventil bestromt: verringert den Öffnungsquerschnitt für minimale Fördermenge       
        - Druckbegrenzungsventil verhindert zu hohen Raildruck bei Ausfall der Zumesseinheit
        - **Nachteil:** 
            - hohe Trägheit
            - Drucksteigerung erfordert zunächst eine Erhöhung des Niederdrucks, dadurch erhöhte Förderleistung der Hochdruckpumpe

1. **Zweisteller-Regelung** (**Druckregelung nieder- und hochdruckseitig**)
    - **Vorteil**
        - geringe Leistungsaufnahme der Hochdruckpumpe bei konstant hohen Drücken
        - hohe Agilität bei geringen Drücken
    - **Motorstart und Warmlaufphase** hochdruckseitig geregelt
        - Kraftstoff soll sich erwärmen und damit fließ- und zündfähiger zu machen
    - **betriebswarmer Motor: Leerlauf / Teillast** Zweisteller-Betrieb
        - große Sprünge des Raildrucks sind wahrscheinlich (Motor im Leerlauf / Teillast $\to$ Lastwunsch des Fahrers: Volllast)
    - **hohen Motorlast** niederdruckseitig geregelt
        - große Steigerungen des Raildrucks nicht möglich und deshalb ist die Trägheit vernachlässigbar



**Druckregelventil** Druckerfassung durch Membransensor am Rail (Raildrucksensor)

Ansteuerung: PWM-Signal (Raildruck wird größer, wenn Tastverhältnis größer wird), wenn Magnetventil bestromt: dadurch wird die Schließkraft der Ventilnadel erhöht oder gesenkt. Dementsprechend wird der Raildruck erhöht oder gesenkt.

1. **unbestromt / stromlos** Raildruck etwa $100~\text{bar}$
    - Motor abstellen, Ventilfeder hält Druckregelventil geschlossen, verhindert ein Leerlaufen des Rails

1. Magnetventil bestromt, Lastzustände:
    - **Motorstart** Raildruck $> 250~\text{bar}$ 
        - Wie hoch ist der Druck im Rail bei Motorstart?
    - **Leerlauf** Raildruck etwa $400~\text{bar}$
    - **Vollast** Raildruck etwa $2000~\text{bar}$ 

**Warum lässt sich ein Fahrzeug mit defektem Druckregelventil nicht mehr starten?**

Durch die im Druckregelventil verbaute Feder verbleibt im Rail ein Restdruck von ca. 100 bar. Da für einen sicheren Motorstart der Druck im Rail mind. 250 bar betragen muss, ist ein Motorstart nicht möglich.

\newpage
### Injektoren

Injektoren vs. Einspritzdüsen: haben keinen festen Öffnungsdruck, sondern öffnen und schließen unter dem jeweiligen variablen Einspritzdruck.

Kraft = Druck x Fläche


**Wie werden Piezoinjektoren angesteuert?**

SG $\to$ Spannung anlegen $\to$ Längenänderung, bleibt in Position bis Kurzschluss $\to$ abschließende Spannung.



**Erklären Sie die Funktionsweise eines Magnetspuleninjektors im geschlossenen und geöffneten Zustand.**

![Injektor mit Magnetventil, Quelle: Europa-Verlag SimKfz](images/CR/Wirkungsweise-Magnetventilinjektors.png){width=40%} 

- **Magnetventil unbestromt - geschlossenen Zustand** dann wirkt im Ventilsteuerraum auf der Stirnfläche des Ventilsteuerkolbens und auf der Druckschulter der Düsennadel gleicher Kraftstoffkochdruck. Einspritzventil ist geschlossen.

- **Magnetventil bestromt - geöffneten Zustand,** dann wird der Rücklauf geöffnet. Über die Ablaufdrossel entweicht mehr Kraftstoff, als über die Zulaufdrossel abfließen kann. Es kommt zum Druckabfall im Ventilsteuerraum. Der Druck auf die Druckschulter der Düsennadel kann die Düse öffnen. Düsennadel öffnet die Düse.

**Erklären Sie die Funktionsweise eines Injektors mit Piezoventil**

Piezoinjektoren erlauben hohe Schaltgeschwindigkeiten und damit viele Teileinspritzungen.

- Piezo-Aktormodul wird bestromt und dehnt sich aus.
- Über den hydraulischen Koppler findet eine Hubvergrößerung statt.
- Öffnet das Servoventil und damit den Rücklauf.
- Über die Ablaufdrossel fließt Kraftstoff aus dem Ventilsteuerraum ab.
- Über die Zulaufdrossel kann weniger Kraftstoff in den Ventilsteuerraum zufließen. Es kommt zum Druckabfall.
- Der Druck auf die Druckschulter der Düsennadel öffnet die Düsennadel des Injektors. Einspritzbeginn.

