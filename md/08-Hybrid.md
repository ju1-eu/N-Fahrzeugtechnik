---
title: 'Hybrid'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!-----------------------------
Dozent: 
# 
## 
Quelle: Schmidt S. 87 ([ schmidt:2015:klima]).
Leistungsverzweigter Hybrid S. 52 ([ schmidt:2021:hybrid]).
Antriebskonzepte S. 1000 ([ reif:2022:boschkraftfahrtechnisches]).
ju 2-9-22
+------------------------------>

**Was ist ein Hybridfahrzeug? Hybrid-Vehicle (HV)** ist mit mindestens zwei unterschiedlichen Energiewandlern und -speichern für den Antrieb des Fahrzeuges  ausgestattet.

Beispiel: Verbrennungsmotor und Kraftstofftank & E-Motor und HV-Batterie

# Arten von Hybriden


1. **Micro-Hybrid:** Regeneratives Bremsen, Start-Stopp

1. **Mild-Hybrid:** Regeneratives Bremsen, Start-Stopp, Drehmomentunterstützung

1. **Full-Hybrid:** Regeneratives Bremsen, Start-Stopp, Drehmomentunterstützung, Elektrisches Fahren

1. **Plug-in-Hybrid:** Regeneratives Bremsen, Start-Stopp, Drehmomentunterstützung, Elektrisches Fahren, Steckdosenaufladung

**Boosten** Drehmomentunterstützung (Verbrennungsmotor unterstützen)

**Rekuperation** Regeneratives Bremsen (Bremsenergierückgewinnung $\to$ Batterie Laden)

# Antriebskonzepte

Leistungsverzweigter Hybrid S. 52 ([@schmidt:2021:hybrid])
und Antriebskonzepte S. 1000 ([@reif:2022:boschkraftfahrtechnisches]).

E-Maschine = **MG1 / MG2** (E-Motor / Generator), **V-Motor** (Verbrennungsmotor), **Planetengetriebe** (Planetenradsätze und Lamellenkupplung), Getriebe, Achsantrieb, Inverter (Pulswechselrichter)

1. **Serieller Hybrid** 
    - Antrieb: durch E-Motor
    - Verbrennungsmotor wird im Drehzahlfenster betrieben (mechanisch nicht mit Antriebstrang verbunden)
    - Serieller Energiefluss
        1. V-Motor $\to$ Generator $\to$ Inverter $\leftrightarrow$ HV-Batterie
        2. Inverter $\leftrightarrow$ E-Motor $\leftrightarrow$ Achsantrieb
    - Nachteil: schlechter Wirkungsgrad ($3\text{x}$ mehr Leistung reinstecken!)
    - Beispiel: Range-Extender (Reichweitenverlängerung)

1. **Paralleler Hybrid** 
    - Antrieb: durch E-Motor oder V-Motor (mechanisch mit Antriebstrang verbunden) oder beide parallel
    - *eine Kupplung zwischen E-Maschine $\parallel$ Getriebe - Achsantrieb*
    - Energiefluss: 
        1. V-Motor $\to$ Achsantrieb
        1. Batterie $\leftrightarrow$ Inverter $\leftrightarrow$ MG $\leftrightarrow$ Achsantrieb
    - *zwei Kupplungen zwischen V-Motor $\parallel$ E-Maschine $\parallel$ Getriebe - Achsantrieb*
    - Energiefluss: 
        1. V-Motor $\to$ Achsantrieb
        1. Batterie $\leftrightarrow$ Inverter $\leftrightarrow$ MG $\leftrightarrow$ Achsantrieb

1. **Leistungsverzweigter Hybrid**
    - Antrieb: durch zwei E-Motoren und V-Motor (mechanisch mit Antriebstrang verbunden)
    - Nachteil: aufwändiges Getriebe 
    - Leistungsverzweigung (Planetengetriebe) 
    - V-Motor (Drehmoment aufteilen)
        1. Teil $\to$ MG1 als Generator 
        1. Teil $\to$ Fahrzeugantrieb
    - V-Motor + E-Motor $\to$ Fahrzeugantrieb
    - Schub- u. Bremsphase: Generator $\to$ Rekuperation
