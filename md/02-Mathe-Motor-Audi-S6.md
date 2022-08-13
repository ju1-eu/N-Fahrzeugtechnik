---
title: 'M-Motorberechnung'
author: 'Jan Unger'
date: \today
subject: "Markdown"
keywords: [Markdown,Latex,HTML,PDF,Pandoc,Shell-Script]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!---------------------------------------------------+
Dozent: Marc Limburg
Thema:  Mathe - Motorberechnung
Fachbuch ([@brand:2020:fachkundeKfz] S. 243)
Fachbuch ([@respondeck:2019:servicetechniker] S. 142)
Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 281)
FS ([@bell:2020:formelsammlung] S. 32 - 37)
#
## 
ju 15-4-22
+----------------------------------------------------->

# Motorberechnung - siehe Datenblatt Audi S6

Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 32 - 33)
FS ([@bell:2020:formelsammlung] S. 32 - 37)

**Aufgabe 1a Zylinderhubraum**

geg: $V_H = 4172~cm^3, z = 8$

ges: $V_h$

Formel: $V_H = V_h \cdot z \to V_h = \frac{V_H}{z}$

Lösung: $V_h =  521,5~cm^3$


**Aufgabe 1b Bohrung**

geg: $s = 9,3~cm, V_h =  521,5~cm^3$

ges: $d$

Formel: $V_h = \frac{\pi \cdot d^2}{4} \cdot s \to d = \sqrt\frac{V_h \cdot 4}{\pi \cdot s}$

Lösung: $d =  8,4497~cm = 84,4969~mm$


**Aufgabe 1c Verdichtungsraum**

geg: $\epsilon = 11 : 1, V_h =  521,5~cm^3$

ges: $V_c$

Formel: $V_c = \frac{V_h}{\epsilon - 1}$

Lösung: $V_c =  52,15~cm^3$


**Aufgabe 1d Hubraumleistung in KW**

geg: $P_{eff} = 250~KW, V_H = 4172~cm^3 = 4,172~l$

ges: $P_H$

Formel: $P_H = \frac{P_{eff}}{V_H}$

Lösung: $P_H =  59,9233 KW/l$

*spezifische Leistung* ($\to$ Literleistung, bessere Vergleichbarkeit)

Umrechnungsfaktor $\boxed{1~PS = 0,735~KW \quad 1~KW = 1,36~PS}$

$\frac{81,4~PS/l}{1,36} = 59,85~KW$

**Aufgabe 1e**

geg: $M = 420~Nm, n = 3400~U/min$

ges: $P_{eff}$

Formel: $P_{eff} = \frac{M \cdot n}{9550}$

Lösung: $P_{eff} =  149,5288~KW$


**Aufgabe 1f Effektiven Kolbendruck bei maximaler Leistung**

geg: $P_{eff} = 250~KW, V_H = 4,172~l, n = 7000~U/min$

ges: $p_{eff}$

Formel: $p_{eff} = \frac{1200 \cdot P_{eff}}{V_H} \cdot n$

Lösung: $p_{eff} =  10,2726~bar$


**Aufgabe 1g mittlere Kolbengeschwindigkeit bei maximaler Leistung**

geg: $s = 0,093~m, n = 7000~U/min$

ges: $v_m$

Formel: $v_m = \frac{s \cdot n}{30}$

Lösung: $v_m =  21,7~m/s$

(*Standard* $v_m: \quad$ Otto = $9 - 16~m/s$, Diesel = $8 - 14~m/s$, zwei Nullpunkte: OT, UT)

**Aufgabe 2 Motortyp nach Art der Motorsteuerung**

- "double overhead camshaft" (dohc) 
- zwei Nockenwellen über Zylinderkopf

**Aufgabe 3 Hub-Bohrung-Verhältnis**

Hub > Bohrung, $s > d$, $93~mm > 84,5~mm$ Langhuber

*oder*

$\alpha = \frac{s}{d} = \frac{93}{84,5} = 1,1$

$\boxed{\alpha > 1 \quad \text{Langhuber}, \alpha = 1 \quad \text{Quadrathuber}, \alpha < 1 \quad \text{Kurzhuber}}$

**Aufgabe 4 elastischer Bereich**

Drehzahlbereich vom Maximalen Drehmoment zur Maximalen Leistung: $3400 - 7000~U/min$

