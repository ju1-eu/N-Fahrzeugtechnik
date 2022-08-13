---
title: 'Klimaanlage'
author: 'Jan Unger'
date: \today
subject: "Markdown"
keywords: [Markdown,Latex,HTML,PDF,Pandoc,Shell-Script]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!--------------------------------------------------+
Dozent: Marc Limburg
Thema:  Loesung -- Betriebs- und Hilfsstoffe
Fachbuch ([@brand:2020:fachkundeKfz] S. 243)
Fachbuch ([@respondeck:2019:servicetechniker] S. 142)
Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 281)
FS ([@bell:2020:formelsammlung] S. 32 - 37)
^\circ\text{C}
#
## 
ju 27-6-22 Klimaanlage
+----------------------------------------------------->

# Aktive und Passive Sicherheit

**Aktive Sicherheit** Maßnahmen zur Vermeidung von Unfällen

- *Beispiele:* ABS, ESP, Klima, Scheibenwischer, ACC (adaptive Geschwindigkeitsregelung)

**Passive Sicherheit** Maßnahmen zur Minderung von Unfallfolgen

- *Beispiele:* Airbag (Fahrer-, Beifahrer-, Kopf- und Seitenairbags), Gurtstraffer, Batterietrennschalter (Kurzschluss, Brandgefahr), Motorhaubenaufsteller



**Airbag löst nach** ca. $15 - 50~ms$ aus (Zündung -- Entfaltung), Crashsensoren: max. $30^\circ$ Aufprallwinkel zur Längsachse

**Gurtstraffer zieht Gurt nach** ca. $20 - 25~ms$ bis zu $15~cm$ ein.

# Aufbau und Funktionsweise einer Klimaanlage

**Luftgütesensor:** misst Schadstoffe in der Außenluft (Frischluft vs. Innenraumluft)

**Wärme** vs. **negative Wärme** (Kälte)

**Enthalpie** Element, das eine bestimmte Wärmeenergie hat

**Komponenten**

1. **Magnetkupplung** Verbindung zwischen Riemenscheibe und Antriebswelle
    - Spaltmaß: $0,4 - 0,6~mm$

1. **Kompressor** Kältemittel verdichten
    - Taumelscheibenverdichter (Förderleistung variieren) 
    - Flügelzellenverdichter 
    - Spiralverdichter (Hybrid- und Elektrofahrzeuge) 
    - Kompressor mit variablem Hub und externer Regelung (PWM-Signal)

1. **Trockner** Kältemittel trocknen, filtern, beruhigen, Sammler


1. **Expansionsventil** regelt Kältemittelzufluss zum Verdampfer, um zu verhindern, dass der Kompressor flüssiges Kältemittel ansaugt (Flüssigkeitsschlag)


1. **Druckschalter und Überdruckventil** Schutz der Klimaanlage
    - Kühlerlüfter / Kondensatorgebläse
        - EIN: $\sim 16~\text{bar}$, AUS: $\sim 10~\text{bar}$
    - Magnetkupplung
        - Druckschalter: Druck zu niedrig $\sim 2~\text{bar}$, Druck zu hoch $\sim 28~\text{bar}$
    - Verdampfersonde / Vereisungssensor
        - Vereisungsschutz EIN $> +4^\circ \text{C}$, AUS  $< 0^\circ \text{C}$

**Funktion**

Kältemittel nimmt Energie auf und gib sie wieder ab bei Änderung seines Aggregatzustandes.

Bei geringem Druck und niedriger Temperatur verdampft Kältemittel. Der Siedepunkt kann durch Druckänderung verschoben werden. Erhöht man den Druck, dann steigt die Verdampfungstemperatur.

Beispiel: R134a

- Atmosphärische Druck: ca. $1~\text{bar} \to$ Siedepunkt: ca. $-26^\circ \text{C}$
- Überdruck: ca. $15~\text{bar} \to$ Siedepunkt: ca. $55^\circ \text{C}$

**Verdampfer** verdampfen, Energie aufnehmen, *Wärme_zu*, aus der Umgebung wird Wärme entzogen. Notwendig, wenn man eine Flüssigkeit verdampfen möchte. (flüssig $\to$ gasförmig)

vs.

**Kondensator** kondensieren, Energie abgeben, *Wärme_ab* an die Umgebung (gasförmig $\to$ flüssig)

**Wärmepumpe** Heizen (PTC) und Kühlen

# Kältemittelkreislauf 

<!--Klimakreislauf-1 vgl. abb.-->
![Klimakreislauf](images/Skizze/Klimakreislauf-1.pdf){width=50%}

1. **Kompressor** (Gasverdichter, Komprimieren, Druck steigt, gasförmig) der kalte Dampf (gasförmig) wird abgesaugt und verdichtet. Dadurch steigt Druck und Temperatur des Gases.

    - Umlauf des Kältemittels
    - Fördermenge beeinflusst Kälteleistung


1. **Kondensator** (Verflüssiger, Kondensieren) das unter hohen Druck stehende heiße Gas wird in den Kondensator gepresst. Durch den Fahrtwind / Lüfter wird das heiße Gas abgekühlt und verflüssigt. Je besser gekühlt wird, desto geringer der Druck. 
    
    -  Aggregatzustandswechsel: gasförmig $\to$ flüssig (Druck ist konstant)

    - **Trockner** flüssiges Kältemittel wird entfeuchtet und gefiltert.

1. **Expansionsventil** (Dosiereinheit, Druckminderer, Drossel, Expandieren, flüssig) Kältemittel expandiert (Druck sinkt) und regelt die Menge des Kältemittels zum Verdampfer.


1. **Verdampfer** (Verdampfen) warme Luft bringt das entspannte flüssige Kältemittel bei geringer Temperatur zum Verdampfen. Dabei entzieht das Kältemittel der Luft Wärme und kühlt sie ab.

    -  Aggregatzustandswechsel: flüssig $\to$ gasförmig (Druck ist konstant)

# Klimaservice

**Ruhedruck** (Motor aus)

- Kältemitteldruck abhängig von Umgebungstemperatur (Vgl. Dampftafel / Richtwerte [@schmidt:2015:klima] S. 120)

**Betriebsdruck** (Motor an im LL, Klima ON, max. Gebläse, Keine Umluft, Heizung OFF, Temp. LOW, $5 - 10~\text{Min.}$ laufen lassen)

- **Sollwerte** Quelle: Andreas Lamm [^1]
- ND $1 - 3~\text{bar}$
- HD $7 - 20~\text{bar}$
- Kühlung 
    - Außentemperatur $20^\circ \text{C} \to 2 - 8^\circ \text{C}$ **Ausströmtemperatur**
    - Außentemperatur $30^\circ \text{C} \to \, <15^\circ \text{C}$ Ausströmtemperatur

[^1]: <https://klimacheck.com/>

**Klimadiagnose** 

1. Betriebsdruck (Vgl. Sollwerte)
    - **Läuft Kondensatorlüfter?**
        - Wenn Defroster EIN, dann muss Lüfter laufen!
1. Ausströmtemperatur (Vgl. Sollwerte)
1. Zustand Kältemittel (Schauglas)

*Vgl. Diagnosetabelle*

|**Hochdruck**      | **Niederdruck** | **Ursache**
|-------------------|-----------------|----------------------------------------------------
|normal, zu hoch    | zu niedrig      | Expansionsventil, Filter, Kondensator
|normal, zu niedrig | zu hoch         | zu viel Kältemittel, Kompressor
|normal, zu niedrig | zu niedrig      | zu wenig Kältemittel, Magnetkupplung
|zu niedrig         | zu hoch         | zu viel Kältemittel, Kondensator, Kondensatorlüfter

Anhand der Leitungstemperaturen auf mögliche defekte im Kältemittelkreislauf schließen ([@schmidt:2015:klima] S. 115).

Übersicht über fehlerhafte Füllmengen und Komponenten die sich an den Druckmanometern widerspiegeln können ([@schmidt:2015:klima] S. 116 -- 117).


**Magnetkupplung am Kompressor prüfen**

1. Spannungsversorgung prüfen (Verkabelung, Sicherung, Relais)
    1. Magnetkupplung (Spannung am Verbraucher) Soll: $12~V$
    1. Masseanschluss (gegen Masse) Soll: $0~V$
    1. Relais (gegen Masse) Soll: $12~V$
    1. Druckschalter (gegen Masse) Soll: $12~V$
1. Temperatur- und Druckschalter, Steuergerät, Luftspalt


**Kondensatorlüfter prüfen**

- Sicherung, Relais, Verkabelung, Motor, Schwergängigkeit

**Klima-Service-Gerät**

- Vakuumzeit $\boxed{60~Min/kg \cdot \text{Kältemittelmenge [kg]}} \quad (1~h~\hat =~ 1~kg)$
- Füllung 
- Kompressor-Öl

Phasen 

1. **Absaugen** (von Kältemittel und Kompressoröl)
1. **Evakuieren** (Vakuum, Wasser entfernen, Dichtigkeit prüfen)
1. **Aufbereiten** (Kältemittel von Wasser und Öl trennen und wiegen)
1. **Auffüllen** (von Kältemittel und Kompressoröl)

**Verlust an Kältemittel** $[\%] \, \boxed{= \frac{\text{abgesaugte Menge}}{\text{Füllmenge}} \cdot 100} \quad \text{Beispiel: } \frac{180~g}{640~g} \cdot 100 = 28~\%$

Jährlich ca. $10~\%$ Verlust normal.