---
title: 'Füllungsoptimierung-II'
author: 'Jan Unger'
date: \today
subject: "Markdown"
keywords: [Markdown,Latex,HTML,PDF,Pandoc,Shell-Script]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!----------------------------+
Dozent: Marc Limburg
Thema:  Füllungsoptimierung-II
Fachbuch ([@brand:2020:fachkundeKfz] S. 243)
Fachbuch ([@respondeck:2019:servicetechniker] S. 142)
Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 281)
# 
##
ju 10-4-22
+------------------------------>
# Wie beschreiben Sie die Dynamische Aufladung?

**Ausgangslage** Ansaugen, Volumenvergrößerung, Druckdifferenz

Die **einströmenden Frischgase** werden am geschlossenen Ventil **reflektiert** und an der bereits im Ansaugrohr stehenden Luftmasse (Außenluft) erneut reflektiert und  bewegt sich wieder auf das EV zu und wenn jetzt das Ventil öffnet können die Frischgase schneller in den Zylinder einströmen, weil die **Massenträgheit** einer ruhenden Luftmasse nicht überwunden werden muss.

Wir machen uns hier die **kinetische Energie** der sich bereits **in Bewegung gesetzten Luftmasse** zunutze, sodass der Beginn des Einströmens kein Losbrechmoment der Luftmasse darstellt, sondern eine schon in sich bewegten Luftmasse/Luftsäule zu nutzen und lässt damit das **Einströmen schneller beginnen** und dadurch wird ein besserer Füllungsgrad erreicht (Frischgasanteil steigt, mehr Kraftstoff $\to$ mehr Leistung und Drehmoment).

## Schwingsaugrohr

Variante

1. **Schaltsaugrohr** einfaches umschalten zwischen

    - **lange Saugrohrlänge** und großes Sammlervolumen, große Massen (sind träge)
      - **unteren Drehzahlbereich**
      - Klappe geschlossen 

    - **kurze Saugrohrlänge**, kleine Massen (sind agiler)
      - **oberen Drehzahlbereich** 
      - Klappe offen
      - Gassäule kann direkt aus dem Luftsammler in Richtung EV strömen

2. **Stufenlos regelbare Sauganlage**

## Resonanzsaugrohr

Beim Resonanzsaugrohr wird nicht der Weg (Saugrohrlänge) den die Luftsäule durchlaufen muss, sondern deren Geschwindigkeit verändert. Dies erreicht man durch Drehzahlabhängigen zu- und wegschalten einer zusätzlichen Luftmasse im Ansaugrohr.

1. Im **oberen Drehzahlbereich** ist die Luftmasse $M_2$ durch die **Resonanzklappe** vom Saugrohr getrennt. 

    - Die **bewegte Luftmasse** entspricht einer relativ **kleinen Masse** $M_1$.
    - Wodurch sie sehr **agil** ist und mit einer hohen Frequenz vom EV zur stehenden Außenluft zurück **reflektiert** werden kann.

2. Im **unteren Drehzahlbereich** wird die **Resonanzklappe** geöffnet und damit die **zusätzliche Luftmasse** $M_2$ aktiviert. 

    - Dadurch wird die Gesamtmasse $M_1 + M_2$ im Saugrohr erhöht,  wodurch die **Geschwindigkeit der Luftsäule** abnimmt. 
    - Sodass sie die längere Zeit zwischen zwei Ventilöffnungen bei geringerer Drehzahl zur Verfügung steht, um das EV nach ihrer **Reflexion** mit der Außenluft wieder zu erreichen.



## Resonanz- und Schwingsaugrohr (keine Prüfung)

Bei einem 6-Zylinder-Reihenmotor werden die *Zylindergruppen 1, 2, 3* und *4, 5, 6* getrennt und damit hat man immer ein Ventil, was sich öffnet und in der anderen Gruppe eins, was sich schließt.

1. Im **unteren Drehzahlbereich** ist die Umschaltklappe geschlossen: 

    - Bei der Befüllung der Zylinder 1, 2 und 3 wirkt der Raum vor den Zylindern 4, 5 und 6 als Resonanzraum und umgekehrt. 
    - Resonanzaufladung, hier schwingen die Luftmassen von rechts nach links.

2. Im **oberen Drehzahlbereich** ist die Umschaltklappe geöffnet: 

    - Die Luft wird direkt angesaugt (kurzer Ansaugweg und hohe Frequenz der Gassäule).  
    - Für jeden einzelnen Zylinder lässt man diese Reflexionsphase durchlaufen.

# Fremdaufladung

Die Frischluft wird von einem Gebläse angesaugt und vor verdichtet und mit einem Überdruck an den Motor geliefert.

## Abgasturbolader

Das **Turbinenrad** wird durch den Abgasstrom (bis zu $320.000~min^{-1} = 5.333~s^{-1}$) beschleunigt. Dieses Turbinenrad ist über eine **Welle** mit dem **Verdichterrad** verbunden, das die Frischluft ansaugt und auf bis zu $2,2~bar$ verdichtet und an den Motor liefert.

**Was versteht man unter Laufzeug?** Kombi von Turbinenrad, Welle und Verdichterrad.

### Turbolader mit Bypass für Ladedruckbegrenzung

**Warum Ladedruck begrenzen?**

- Klopfgrenze
- Mechanische Überbelastung von Bauteilen 

Ladedruckbegrenzung $\to$ Ladedruckregelventil (**Wastegate**) oder Bypassklappe


<!---->
### VTG-Lader (Variable Turbinengeometrie, meist bei Dieselmotoren)

Konstanten Ladedruck und eine konstante Drehmomentkurve über einen nahezu gesamten Drehzahlbereich. 

Beim VTG-Lader sind vor dem Turbinenrad Leitschaufeln angeordnet, die den Einlassquerschnitt abhängig von der Drehzahl anpassen.

1. Im **unteren Drehzahlbereich** 

    - d.h. bei einem kleinen Abgasstrom
    - verstellen wir die **Leitschaufeln** so, dass der **Querschnitt** klein ist
    - bei einer verhältnismäßig großen **Strömungsgeschwindigkeit**
    - hier trifft der gesamte **Abgasstrom**
    - auf das äußere Ende meines **Turbinenrades**, die wirksame Fläche wird größer
    - großen **Hebelarm** und damit mehr Drehmoment


2. Im **oberen Drehzahlbereich**

    - verstellen wir die **Leitschaufeln** so, dass der **Querschnitt** groß ist
    - hier trifft der gesamte **Abgasstrom**
    - auf die Mitte meines **Turbinenrades**, die wirksame Fläche wird kleiner
    - und damit haben wir den **gleichen Ladedruck** wie im unteren Drehzahlbereich

Damit der VTG-Lader auch in **Ottomotoren** eingebaut werden kann, muss darauf geachtet werden, das die verbauten Materialien eine dementsprechende thermische Belastbarkeit aushalten kann, um eben einen reibungslosen Ablauf zu gewährleisten. Dieselmotoren haben eine geringere Abgastemperatur.

### Registeraufladung (Stufenaufladung)

- Mitte 90er-Jahre, Audi RS2 und Porsche
- kleiner und großer Turbolader sind in Reihe
- Regelklappen für Abgasstromseite und Frischluftseite
- Ladedruckbegrenzung $\to$ **Wastegate** (Bypassventil) stufenlose Ansteuerung über SG

1. **unteren Drehzahlbereich**: 

    - Regelklappen geschlossen
    - **kleiner Turbo** 
        - bei einem kleinen Abgasstrom
        - kommt schneller auf Drehzahl, agiler
        - Warum? Durch geringere Massenträgheit
        - bestimmt Ladedruck
    - **großer Turbo** 
        - dreht schon mal mit und arbeitet als Vorverdichter für den kleinen Lader

2. **mittleren Drehzahlbereich**: 

    - Regelklappen öffnen synchron 
    - verhindert Drossel Wirkung

3. **oberen Drehzahlbereich**: 

    - Regelklappen voll offen
    - **kleiner Turbo** läuft ohne Wirkung
    - **großer Turbo** bei einem großen Abgasstrom, max. Fördern

Herstellername *Twin-Turbo* - Bezeichnung nicht geschützt! 


### Doppelaufladung

- zwei gleich große/kleine Turbolader sind parallel im Verbund
- Ladedruckbegrenzung $\to$ **Wastegate** geöffnet

1. **unteren Drehzahlbereich**: Turbo 1 aktiv

2. **mittleren Drehzahlbereich**: Turbo 2 läuft an durch Öffnen eines Ventils, die vor verdichtete Luft wird zum Turbo 1 gefördert

3. **oberen Drehzahlbereich**: beide Turbo's aktiv


Herstellername *Bi-Turbo* - Bezeichnung nicht geschützt!

### Twin-Scroll-Lader 

Bei einem 4 Zylinder Motor werden die **Abgasströme** der *Zylinder 1 und 4* sowie der *Zylinder 2 und 3* in getrennten Kanälen zur Turbine geleitet. 

Durch Strömung-Impulse (Tick, Tick, ... immer abwechselnd kleiner und großer Kanal) entsteht eine Impulsaufladung auf die Turbinenschaufeln.

Vorteil: keine gegenläufigen Strömungen

1. **kleiner Kanal** leitet den Abgasstrom auf die Innenflächen der Turbinenschaufeln. 
    - schnelleres und sensibleres Ansprechverhalten des Laders 

2. **großer Kanal** leitet den Abgasstrom auf den Rand der Turbinenschaufeln. 
    - sorgt für höhere Drehzahl und Leistung des Turboladers

## Mechanische Lader

Der Antrieb erfolgt durch KW über Keilriemen.

### Schraubenkompressor (Roots-Lader, Kompressor)

Beim Schraubenkompressor verdichten zwei ineinander verdrillte Laderschaufeln/Rotoren die Luft Richtung Einlasskanal.

**Ladedruckregelung** erfolgt durch Bypassklappe oder Magnetkupplung (Kompressor kann entkoppelt werden, um unnötigen Kraftstoffverbrauch zu reduzieren)

**Lastwunsch** wird gesteuert durch den Fahrer über $\to$ Hauptdrosselklappe 

1. **Saugbetrieb / Teillast**

    - Bypassklappe offen, Drossel frei
    - Leer fördern lassen ($\to$ d.h. Überschüssige Luft wird auf die Saugseite des Laders gefördert)
    - hier herrscht Unterdruck

2. **Ladebetrieb / Volllast**

    - Bypassklappe geschlossen
    - voller Ladedruck

### Comprex-Lader (keine Serienreife, keine Prüfung)

Besteht aus einem rotierenden Röhrenkörper, der von der Kurbelwelle angetrieben wird. Beim Comprex-Lader schiebt Abgas die Frischluft in den Ansaugtrakt. Das erfordert eine präzise Abstimmung auf die Motorsteuerung.

**Hyprex-Lader**

Der Hyprex-Lader ist eine Weiterentwicklung des Comprex-Laders. Der Röhrenkörper wird durch einen elektronisch geregelten Elektromotor angetrieben.

### Kombi von Turbolader und Kompressor (VW bei den Twincharger-TSI-Motoren)

Hauptvorteile verknüpfen

- **Kompressor** (im unteren Drehzahlbereich $\to$ direktes Ansprechverhalten) 
- **Turbolader** (im oberen Drehzahlbereich $\to$ nahezu keine Leistungsentnahme vom Verbrennungsmotor)

## Elektrische Lader (eLader)

- Antrieb des Verdichterrads: 48 V Elektromotor
- unabhängig vom Abgasstrom und damit kein Turboloch
  - **unteren Drehzahlbereich** $\to$ elektrische Lader
  - **oberen Drehzahlbereich** $\to$ Abgasturbolader 


## Warum muss ich die Ladeluft kühlen?

**Was begrenzt den maximalen Ladedruck?**

Klopfgrenze, **wodurch tritt eine klopfende Verbrennung ein?** Ungewollte Glühzündung, **wodurch entsteht eine Glühzündung?** Durch zu viel Druck und Hitze.

Wenn ich dem System Hitze entziehe, kann ich mit dem Ladedruck höher gehen. Meine angesaugte Luftmasse hat eine höhere Dichte, ich kann gleichzeitig mehr davon reinpacken. Dadurch ist meine Leistungsfähigkeit noch mal gestiegen.