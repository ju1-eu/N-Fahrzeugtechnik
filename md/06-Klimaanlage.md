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
ju 20-8-22 Klimaanlage
+----------------------------------------------------->

# Aktive und Passive Sicherheit

**Aktive Sicherheit** Maßnahmen zur Vermeidung von Unfällen

- *Beispiele:* ABS, ESP, Klima, Scheibenwischer, ACC (adaptive Geschwindigkeitsregelung)

*Klima*: die Raumtemperatur wird runtergekühlt, Aufmerksamkeit steigt und der Pollenfilter bewirkt eine geringere Allergie last für Allergiker.

**Passive Sicherheit** Maßnahmen zur Minderung von Unfallfolgen

- *Beispiele:* Airbag (Fahrer-, Beifahrer-, Kopf- und Seitenairbags), Gurtstraffer, Batterietrennschalter (Kurzschluss, Brandgefahr), Motorhaubenaufsteller



**Airbag löst nach** ca. $15 - 50~ms$ aus (Zündung -- Entfaltung), Crashsensoren: max. $30^\circ$ Aufprallwinkel zur Längsachse

**Gurtstraffer zieht Gurt nach** ca. $20 - 25~ms$ bis zu $15~cm$ ein.

\newpage
# Aufbau und Funktionsweise einer Klimaanlage

**Luftgütesensor:** misst Schadstoffe in der Außenluft (Frischluft vs. Innenraumluft)

**Wärme** vs. **geringe, hohe Wärme, Wärmeentzug** (Kälte gibt es in der Physik nicht)

**Enthalpie** Element, das eine bestimmte Wärmeenergie hat

## Komponenten 

1. **Magnetkupplung** Verbindung zwischen Riemenscheibe und Antriebswelle
    - Spaltmaß: $0,4 - 0,6~mm$

1. **Kompressor** Kältemittel verdichten
    - Taumelscheibenverdichter (Förderleistung variieren) 
    - Flügelzellenverdichter 
    - Spiralverdichter (Hybrid- und Elektrofahrzeuge) 
    - Kompressor mit variablem Hub und externer Regelung (PWM-Signal)

1. **Trockner** flüssiges Kältemittel wird entfeuchtet und gefiltert, beruhigen, Sammler


1. **Expansionsventil** regelt Kältemittelzufluss zum Verdampfer, um zu verhindern, dass der Kompressor flüssiges Kältemittel ansaugt (Flüssigkeitsschlag)


1. **Druckschalter und Überdruckventil** Schutz der Klimaanlage
    - Kühlerlüfter / Kondensatorgebläse
        - EIN: $\sim 16~\text{bar}$, AUS: $\sim 10~\text{bar}$
    - Magnetkupplung
        - Druckschalter: Druck zu niedrig $\sim 2~\text{bar}$, Druck zu hoch $\sim 28~\text{bar}$
    - Verdampfersonde / Vereisungssensor
        - Vereisungsschutz EIN $> +4^\circ \text{C}$, AUS  $< 0^\circ \text{C}$

## Funktion des Kältemittels

Kältemittel nimmt Energie auf und gib sie wieder ab bei Änderung seines Aggregatzustandes.

Bei geringem Druck und niedriger Temperatur verdampft Kältemittel. Der Siedepunkt kann durch Druckänderung verschoben werden. Erhöht man den Druck, dann steigt die Verdampfungstemperatur.

Beispiel: R134a

- Atmosphärische Druck: ca. $1~\text{bar} \to$ Siedepunkt: ca. $-26^\circ \text{C}$
- Überdruck: ca. $15~\text{bar} \to$ Siedepunkt: ca. $55^\circ \text{C}$

**Verdampfer** verdampfen, Energie aufnehmen (*Wärme_zu*) aus der Umgebung wird Wärme entzogen. Notwendig, wenn man eine Flüssigkeit verdampfen möchte. (flüssig $\to$ gasförmig)

vs.

**Kondensator** kondensieren, Energie abgeben (*Wärme_ab*) an die Umgebung (gasförmig $\to$ flüssig)

**Wärmepumpe** Heizen (PTC) und Kühlen

\newpage
## Erkläre den Kältemittelkreislauf 

<!--Klimakreislauf-1 vgl. abb.-->
![Klimakreislauf](images/Skizze/Klimakreislauf-1.pdf){width=70%}

1. **Kompressor** (Gasverdichter, gasförmig, Verdichten, Druck steigt) saugt das abgekühlte gasförmige Kältemittel an und verdichtet es. Druck und Temperatur steigt (Druckanstieg). Das Kältemittel erwärmt sich, wird aber nicht komplett flüssig. Deshalb schieben wir es durch den Kondensator.


1. **Kondensator** (Verflüssiger, Kondensieren) hier wird das Kältemittel von der Umgebungsluft durchströmt und abgekühlt. Aggregatzustand wechsel von gasförmig $\to$ flüssig (Druck ist konstant). Kältemittel wird flüssig, wenn es den Kondensator verlässt.
    

1. **Expansionsventil** (Dosiereinheit, Druckminderer, Drossel, Expandieren, flüssig) Kältemittel expandiert durch die Drossel (Druck abfall) und lässt bedarfsgerecht eine bestimmte definierte Menge Kältemittel durch Strömen.


1. **Verdampfer** (Verdampfen) dadurch wird ein Aggregatzustand wechsel von  flüssig $\to$ gasförmig (Druck ist konstant) gewährleistet. Die durch den Verdampfer strömende Umgebungsluft runterkühlen und in den Innenraum einströmen lassen. Dabei entzieht das Kältemittel der Umgebungsluft Wärme und kühlt sie ab.


\newpage
## Kunde bemängelt, Klimaanlage kühlt nicht richtig

**Es wurde beispielsweise nur 100 g Kältemittel abgesaugt. Kann die Klimaanlage wieder befüllt werden?**

Nicht befüllen $\to$ wir machen uns strafbar.

Kältemittel absaugen und mit Stickstoff auf Undichtigkeit prüfen.

**Verlust an Kältemittel** $[\%] \, \boxed{= \frac{\text{abgesaugte Menge}}{\text{Füllmenge}} \cdot 100} \quad \text{Beispiel: } \frac{180~g}{640~g} \cdot 100 = 28~\%$

Jährlich ca. $10~\%$ Verlust normal.

## Was ist der Unterschied zwischen intern und extern geregelte Klimakompressoren?

**Intern**, die Stellung der Taumelscheibe und damit die Fördermenge wird durch ein Regelventil bestimmt. Kann bei Bedarf über eine Magnetkupplung entkoppelt und damit komplett ausgeschaltet werden.

*Nachteil:* "kaputt stehen" eine Klimaanlage nimmt Schaden, wenn sie nicht regelmäßig eingeschaltet wird (Dichtungen, Schmierung)

**Extern** keine Magnetkupplung, mit Überlastschutz, Anlage läuft immer, aber Fördermenge wird runtergeregelt auf ca. $2~\%$

*Nachteil:* Reibung

## Kältemittel R744 - Problem bei hohen Außentemperaturen

Klima funktioniert schlecht bei zu hohen Außentemperaturen $> 35^\circ\text{C}$. Kältemittel wird nicht genug runtergekühlt.

## Warum sollte man eine Klimaanlage spülen und welche Möglichkeiten gibt es?

Bei Verunreinigungen, Beispiel  Kompressor schaden.

- Sieb Einsätze
- Formiergas, Stickstoff, mit Kältemittel (Quelle: Andreas Lamm) 

**Offene Anlage** Trockner erneuern oder Anlage verschließen.

## Desinfizieren einer Klimaanlage

- Ozongeräte (24h)
- Spray (geringe Wirkung)

## Warum läuft aus der Klimaanlage Wasser bei heißem Wetter?

- **Sommer** schwüles Wetter hat eine hohe Luftfeuchtigkeit 
- **Winter** kalte Luft hat eine geringe Luftfeuchtigkeit

## Welche Kältemittelöle gibt es und wo ist der Unterschied?

Herstellerangaben befolgen - Typenschild auf dem Klimakompressor

- **PAG-Öle** hygroskopisch
- **POE-Öle** Polyester-Öl, elektrisch isolierendes Klimakompressoröl

\newpage
# Klimaservice

**Ruhedruck** (Motor aus)

- Kältemitteldruck abhängig von Umgebungstemperatur (Vgl. Dampftafel / Richtwerte [@schmidt:2015:klima] S. 120)

**Betriebsdruck** (Motor an im LL, Klima ON, max. Gebläse, keine Umluft, Heizung OFF, Temp. LOW, $5 - 10~\text{Min.}$ laufen lassen)

- **Sollwerte** Quelle: Andreas Lamm [^1]
- ND $1 - 3~\text{bar}$
- HD $7 - 20~\text{bar}$
- Kühlung 
    - Außentemperatur $20^\circ \text{C} \to 2 - 8^\circ \text{C}$ **Ausströmtemperatur**
    - Außentemperatur $30^\circ \text{C} \to \, <15^\circ \text{C}$ Ausströmtemperatur

[^1]: <https://klimacheck.com/>

## Klimadiagnose

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

Anhand der Leitungstemperaturen auf mögliche Defekte im Kältemittelkreislauf schließen ([@schmidt:2015:klima] S. 115).

Übersicht über fehlerhafte Füllmengen und Komponenten, die sich an den Druckmanometern widerspiegeln können ([@schmidt:2015:klima] S. 116 -- 117).

## Magnetkupplung und Kondensatorlüfter prüfen

**Magnetkupplung am Kompressor prüfen**

1. Spannungsversorgung prüfen (Verkabelung, Sicherung, Relais)
    1. Magnetkupplung (Spannung am Verbraucher) Soll: $12~V$
    1. Masseanschluss (gegen Masse) Soll: $0~V$
    1. Relais (gegen Masse) Soll: $12~V$
    1. Druckschalter (gegen Masse) Soll: $12~V$
1. Temperatur- und Druckschalter, Steuergerät, Luftspalt


**Kondensatorlüfter prüfen**

- Sicherung, Relais, Verkabelung, Motor, schwergängig

## Klima-Service-Gerät

- Vakuumzeit $\boxed{60~Min/kg \cdot \text{Kältemittelmenge [kg]}} \quad (1~h~\hat =~ 1~kg)$
- Füllung 
- Kompressor-Öl

Phasen 

1. **Absaugen** (von Kältemittel und Kompressoröl)
1. **Evakuieren** (Vakuum, Wasser entfernen, Dichtigkeit prüfen)
1. **Aufbereiten** (Kältemittel von Wasser und Öl trennen und wiegen)
1. **Auffüllen** (von Kältemittel und Kompressoröl)

