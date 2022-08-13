---
title: 'Keywords'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!-----------------------------+
ju 8-2-22
Gemischbildung
+------------------------------>

# Gemischbildungssysteme 

sollen für jeden Betriebszustand des Motors ein Kraftstoff-Luft-Gemisch herstellen, das in der *Menge ausreichend* ist und im Motor möglichst *vollständig verbrannt* wird.

# Betriebszustände

- **Kaltstart** 
  - Kraftstoff kondensiert an kalten Saugrohr- und    Zylinderwänden 
  - $\to$ sehr fettes Gemisch (bis $\lambda = 0,3$) nötig
- **Warmlauf** 
  - Kondensationsverluste verringert sich 
  - $\to$ Kraftstoffmenge wird temperaturabhängig verringert
- **Leerlauf** 
- **Übergang, Beschleunigung** 
  - beim Öffnen der Drosselklappe magert das Gemisch kurzzeitig ab 
  - $\to$ kurzzeitig mehr Kraftstoff einspritzen
- **Teillast** 
- **Volllast** 
  - maximale Motorleistung bei voll geöffneter Drosselklappe 
  - $\to$ Anreicherung des Gemisches auf $\lambda = 0,85 \dots 0,95$
- **Schubabschaltung**
  - Drosselklappe geschlossen bei hoher Drehzahl (Bergab fahren oder Fuß vom Gas bei hoher Geschwindigkeit) 
  - $\to$ keine Einspritzung von Benzin bis Drosselklappe wieder geöffnet

# Mischungsverhältnis

beschreibt die *Zusammensetzung des Kraftstoff-Luft-Gemisches*. Man unterscheidet ein theoretisches und ein praktisches Mischungsverhältnis.

1. **Theoretisches Mischungsverhältnis** (stöchiometrisches Verhältnis): 
   - zur *vollständigen Verbrennung* von $1~kg$ Super werden $14,7~Kg$ Luft benötigt 

2. **Praktisches Mischungsverhältnis**
   - weicht je nach Betriebszustand vom theoretischen Verhältnis ab 
   - *Fettes Gemisch* (Luftmangel): z. B. $1:13$
   - *Mageres Gemisch* (Luftüberschuss): z. B. $1:16$

# Luftverhältnis

$\lambda$ ist das Verhältnis zwischen der tatsächlich der Verbrennung zugeführten Luftmasse und der zur vollständigen Verbrennung theoretisch erforderlichen Luftmasse

- Luftverhältnis $\lambda = \frac{\text{zugeführte Luftmasse in [kg]}} {\text{theoretische Luftmasse in [kg]}}$

- Beim theoretischen Mischungsverhältnis $1:14,7$ ist $\lambda = 1$

- $\lambda = \frac{16~kg}{14,7~kg} > 1$ (mager)

**Mischungsverhältnisse für Super**

![Mischungsverhältnis](images/skizze/Mischungs-Luftverhaeltnis.pdf){width=60%}

# Gemischzusammensetzung

1. **Homogenes Gemisch** 
   - im gesamten Brennraum ist die Gemischzusammensetzung gleich
   - Einspritzung im Ansaugtakt
   - braucht Zeit für eine gleichmäßige Durchmischung des Kraftstoff-Luft-Gemisches

2. **Heterogenes Gemisch**
   - im Brennraum gibt es Bereiche unterschiedlicher Gemischzusammensetzung (**Schichtladung**)
     - Fettes Gemisch in der Nähe der Zündkerze ($\lambda = 1$)
     - Mageres Gemisch im äußeren Bereich ($\lambda > 1,3$)
     - späte Einspritzung während des Verdichtungstaktes
   - Saugrohrklappe geschlossen
   - man kann sehr mager fahren, um Sprit zu sparen

**Ort der Gemischbildung** 

1. **Äußere Gemischbildung** Kraftstoff wird in das Saugrohr eingespritzt
   - Homogenes Gemisch

2. **Innere Gemischbildung** Kraftstoff wird direkt in den Brennraum eingespritzt
   - Heterogenes Gemisch
     - späte Einspritzung während des Verdichtungstaktes kurz vor Zündung
     - Kraftstoff und Luft kann sich nicht gleichmäßig vermischen
   - Homogenes Gemisch
     - Einspritzung zu Beginn des Ansaugtaktes

3. **Kombi aus äußere und innere Gemischbildung** 

# Leistungsregelung

1. **Quantitätsregelung**  Motoren mit äußerer Gemischbildung und homogenem Gemisch
   - Je nach Lastzustand ändert sich die Drosselklappe und damit die angesaugte Luftmenge.
   - Die Zusammensetzung des Gemisches muss dabei nahezu gleich bleiben ($\lambda = 1$)

2. **Qualitätsregelung** Motoren mit innerer Gemischbildung und heterogenem Gemisch
   - Bei geöffneter Drosselklappe wird verschieden viel Kraftstoff eingespritzt. Die angesaugte Luftmenge bleibt dabei nahezu gleich
   - Die Zusammensetzung des Gemisches im Brennraum ändert sich somit je nach Lastzustand.

# Arten der Benzineinspritzung

**Vergaser**

Luft wird angesaugt vom Motor, vor der Drosselklappe gibt es eine Verengung, durch die Verengung erhöht sich die Strömungsgeschwindigkeit der angesaugten Luft (Venturi-Rohr). Der Kraftstoff im Vergaser gelangt über eine Düse in Tropfenform in das Ansaugluftgemisch. Durch die hohe Strömungsgeschwindigkeit der angesaugten Luft wird der Kraftstoff mitgerissen. 

Vorzerstäubung, Feinzerstäubung $\to$ Kraftstoff-Luft-Gemisch

Die Luftdurchflussmenge wird über Luftdruck (Luftdichte) und Temperatur gemessen. Daraus wird die Düsengröße berechnet und damit die Kraftstoffmenge.

**Indirekte Einspritzung**

*Einzelpunkteinspritzung*

- vor der Drosselklappe befindet sich ein Einspritzventil
- die angesaugte Luft wird mit Kraftstoff versetzt, sodass ich hier ein Gemisch gebildet habe
- Gemischzusammensetzung war nicht so genau, durch unterschiedliche Ansaugwege

| **#**                  | **Beschreibung**                 |
|------------------------|----------------------------------|
| Art der Einspritzung   | **SPI = Single Point Injection** |
| Ort der Einspritzung   | Indirekt - vor der Drosselklappe |
| Gemischzusammensetzung | homogen                          |

*Mehrpunkteinspritzung*

- die angesaugte Luft strömt durch die Drosselklappe in das Verteilerrohr
- Kraftstoffverteilerrohr mit einzelne Einspitzventilen, die direkt in das Saugrohr einspritzen
- Gemischzusammensetzung ist gleich (gleiche Ansaugwege)


| **#**                  | **Beschreibung**                 |
|------------------------|----------------------------------|
| Art der Einspritzung   | **MPI = Multi Point Injection**  |
| Ort der Einspritzung   | Indirekt - vor das Einlassventil |
| Gemischzusammensetzung | homogen                          |


**Direkte Einspritzung**

| **#**                  | **Beschreibung**                |
|------------------------|---------------------------------|
| Art der Einspritzung   | **MPI = Multi Point Injection** |
| Ort der Einspritzung   | Direkt - in den Zylinder        |
| Gemischzusammensetzung | homogen oder heterogen          |

# Öffnung der Einspritzventile

- Simultane Einspritzung 
- Sequenzielle Einspritzung 
- Zylinderselektive Einspritzung


# Zündanlage

**Zündanlage mit Unterbrecherkontakt**

Bat. 12 V $\to$ Zündspannung 40.000 V

Batterie - 30 - Zündschalter - 15 - Zündspule

- 1 - Unterbrecherkontakt - Masse wird geschaltet durch Nocken
  - geschlossen - in Primärspule baut sich Magnetfeld auf
  - offen - Magnetfeld bricht zusammen, es wird eine Spannung in der Sekundärspule indiziert - Spannung geht weiter an den Zündverteiler
- 4 - Zündverteiler - Zündkerze - Zündfunken - Masse

**Zündanlage mit Einzelfunkzündspule**

- Eingabe - Wann soll gezündet werden?
  - Positionsgeber an Nockenwelle und Fahrpedal
- Verarbeitung erfolgt im Steuergerät
  - Kennfeld - abhängig von Drehzahl und Last wird ein Zündwinkel berechnet
- Ausgabe an Zündspule

# Sensoren und Aktoren

| **#**                   | **Sensoren**                 | **Aktoren**                |
|-------------------------|------------------------------|----------------------------|
| **Zentraleinspritzung** | Drehzahlgeber                | Drosselklappenansteller    |
|                         | Motortemperaturfühler        | Regenerierventil           |
|                         | Lufttemperaturfühler         | Einspritzventil            |
|                         | Drosselklappenpotentiometer  |                            |
|                         | Lambdasonde                  |                            |
|                         | OT-Geber                     |                            |
| **MED - Motronic**      | Luftmassenmesser             | Kraftstoffpumpe            |
|                         | Saugrohrdrucksensor          | E-Gas Stellmotor           |
|                         | Differenzdrucksensor         | Lambdasondenheizung        |
|                         | Fahrpedalsensor              | NOx-Sensorheizung          |
|                         | NOx-Sensor                   | Tankentlüftungsventil      |
|                         | Abgastemperatursensor        | Abgasrückführventil        |
|                         | Saugrohrklappenpotentiometer | Kraftstoffdruckregelventil |
|                         |                              | Saugrohrklappenventil      |