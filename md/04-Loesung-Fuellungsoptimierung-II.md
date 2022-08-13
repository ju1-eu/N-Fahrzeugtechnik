---
title: 'L-Füllungsoptimierung-II'
author: 'Jan Unger'
date: \today
subject: "Markdown"
keywords: [Markdown,Latex,HTML,PDF,Pandoc,Shell-Script]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!-----------------------------+
Dozent: Marc Limburg
Thema:  Lösung - Füllungsoptimierung-II
Fachbuch ([@brand:2020:fachkundeKfz] S. 243)
Fachbuch ([@respondeck:2019:servicetechniker] S. 142)
Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 281)
FS ([@bell:2020:formelsammlung] S. 32 - 37)
#
##
ju 5-5-22
+----------------------------------------------------->

**1) Nennen Sie Möglichkeiten zur Leistungssteigerung eines Verbrennungsmotors.**

In der mir verfügbaren Zeit möglichst viel Kraftstoff und Luft in den Zylinder zu bekommen. Dieses Kraftstoff-Luft-Gemisch wird zur Verbrennung gebracht und soll meinen Kolben effektiv nach unten treiben.

Mögliche Systeme

1. Einventiltechnik $\to$ Mehrventiltechnik 
1. Saugmotor $\to$ Fremdaufladung 
1. Steuerzeiten $\to$ variable Steuerzeiten (Nachladeeffekt nutzen) 
1. Ventiltrieb $\to$ variable Ventiltrieb (unterschiedliche Nockenprofile und Ventilöffnungszeiten) 
1. Dynamische Aufladung (Strömungsenergie der bereits bewegten Luftmasse nutzen innerhalb meines Ansaugsystems) 
1. Motordrehzahl anheben $\to$ z. B. Honda (kleinen Hubraum und hohe Drehzahl) 
1. Hubraum vergrößern 
1. Zündung optimieren

**2) Definieren Sie Dynamische Aufladung und Fremdaufladung**

**a) Dynamische Aufladung**

Die dynamische Aufladung erfolgt ausschließlich durch Nutzung der kinetischen Energie der Gassäule im Ansaugtrakt. Wird das EV geschlossen, kommt es zur Reflexion und an der bereits im Ansaugrohr stehenden Luftmasse (Außenluft) erneut reflektiert und  bewegt sich wieder auf das EV zu.
Im Idealfall soll die Gassäule wieder vor dem EV stehen, wenn diese gerade öffnet. 

Erreichbar ist diese durch

1. dynamische Ansaugwege
    - lange Wege für niedrige Drehzahlen 
    - kurze Wege für hohe Drehzahlen 

2. Resonanzsaugrohr - durch Änderung der Luftgeschwindigkeit durch zuschaltbare Luftmassen 
    - Resonanzklappe offen, zusätzliche Luftmasse aktiviert, das erhöht die Gesamtmasse im Saugrohr, wodurch die Geschwindigkeit der Luftsäule abnimmt (Massenträgheit) $\to$ für niedrige Drehzahlen 
    - Resonanzklappe geschlossen, die bewegte Luftmasse ist gering, sehr agil und mit hoher Frequenz vom EV zu stehenden Außenluft und zurück reflektiert $\to$ für hohe Drehzahlen


**b) Fremdaufladung**

Die Frischluft wird von einem Gebläse angesaugt und vor verdichtet und mit einem Überdruck an den Motor geliefert. Füllungsgrad auf bis zu 160\% erreicht werden können.

Systeme: Abgasturbolader, eLader, Kompressor

**3) Welche Möglichkeiten bieten Schaltsaugrohre?**

Sie ermöglichen eine bedarfsgerechte Änderung der Ansaugwege. Diese Maßnahme bewirkt eine Erhöhung der Zylinderfüllung und somit eine Steigerung des Drehmoments bzw. Motorleistung. Die Laufdauer der Luftsäule ändert sich mit der Frequenz. 

**Schaltsaugrohr** einfaches umschalten zwischen

- **lange Saugrohrlänge** und großes Sammlervolumen, große Massen (sind träge)
    - **unteren Drehzahlbereich**
    - Klappe geschlossen 

- **kurze Saugrohrlänge**, kleine Massen (sind agiler)
    - **oberen Drehzahlbereich** 
    - Klappe offen
    - Gassäule kann direkt aus dem Luftsammler in Richtung EV strömen

**4) Wie ist grundsätzlich die Wirkungsweise eines Abgas-Turboladers?**

Das **Turbinenrad** wird durch den Abgasstrom beschleunigt. Dieses Turbinenrad ist über eine **Welle** mit dem **Verdichterrad** verbunden, das die Frischluft ansaugt und auf bis zu $2,2~bar$ verdichtet und an den Motor liefert.

**5) Was bedeutet das Kürzel VTG in Verbindung mit Fremdaufladung?**

Variable Turbinengeometrie

**Beschreiben Sie das Verhalten dieses Laders in Abhängigkeit zur Drehzahl.**

$\boxed{\uparrow M = \sim F \cdot \uparrow r}$

1. Bei **niedriger Drehzahl** mit geringer Abgasmenge wird durch die Leitschaufelstellung ein kleiner Eintrittsquerschnitt bemessen und der Abgasstrom auf den äußeren Rand des Turbinenrades geleitet. Hierdurch wird das Abgas beschleunigt und trifft zudem auf einen langen Hebelarm. Am Turbinenrad entsteht ein großes Moment, die Turbinendrehzahl und der Ladedruck steigen.

2. Bei **hohen Drehzahlen** mit entsprechend größere Abgasmenge wird durch die Leitschaufel ein großer Einlassquerschnitt eingestellt und der Abgasstrom relativ nah an das Zentrum des Turbinenrades geleitet. Die höhere Abgasgeschwindigkeit in Verbindung mit dem größeren Abgasvolumen kompensiert den kleinen Hebelarm am Turbinenrad. Wodurch der Ladedruck konstant bleibt.

**6) Warum werden VTG-Lader nur bei Dieselmotoren verwendet?**

Die Abgastemperatur bei Ottomotoren ist im Volllastbereich bis zu 1000 °C (im Vergleich Dieselmotor bis ca. 800 °C) zu hoch. Die Temperatur am Verstellmechanismus darf 850 °C nicht übersteigen, da dieser sonst ausfallen könnte. 

*Ergänzung,* dies gilt nicht für moderne VTG-Lader mit Molybdän beschichteten Verstellmechanismus. Diese sind für den Einsatz im Ottomotor geeignet.

**7) Beschreiben Sie Aufbau und Wirkungsweise der Doppel- und Registeraufladung**

**a) Doppelaufladung**

- zwei gleich große/kleine Turbolader sind parallel im Verbund
- Ladedruckbegrenzung $\to$ **Wastegate** geöffnet

1. **unteren Drehzahlbereich**: Turbo 1 aktiv

2. **mittleren Drehzahlbereich**: Turbo 2 läuft an durch Öffnen eines Ventils, die vor verdichtete Luft wird zum Turbo 1 gefördert

3. **oberen Drehzahlbereich**: beide Turbo's aktiv

**b) Registeraufladung**

- kleiner und großer Turbolader sind in Reihe
- Regelklappen für Abgasstromseite und Frischluftseite
- Ladedruckbegrenzung $\to$ **Wastegate** (Bypassventil) stufenlose Ansteuerung über SG

1. **unteren Drehzahlbereich**: 

    - Regelklappen geschlossen
    - **kleiner Turbo,** geringe Massenträgheit
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

**8) Welchen Vorteil erreicht man durch die Ladeluftkühlung?**

Eine bessere Zylinderfüllung durch höhere Luftdichte. 
Durch Senkung der Ladelufttemperatur z. B. 120 °C auf 70 °C (ca.  50 °C abkühlen) niedrige Verbrennungstemperatur, Selbstentzündungstemperatur wird später erreicht, geringere Klopfneigung und dadurch höhere Ladedrücke.

**Innere Kühlung**

1. durch die Temperatur der angesaugten Luftmasse wird das innere des Zylinders gekühlt
2. Kraftstoff wird flüssig in den Zylinder eingespritzt und fängt an, an der umgebenen Wärme gasförmig zu werden. Durch den Aggregatzustands wechsel von flüssig in gasförmig entsteht ein Druckverlust und dadurch entziehen wir der Umgebungsluft Wärme.

**9) Was versteht man unter "Downsizing"?**

Verkleinerung der Verbrennungsmotoren (Hubraum und Zylinderzahl) bei gleicher Leistung.

**Warum macht man das?** Durch Verringern des Hubraums oder wegfallen einzelne Zylinder verringern wir die Reibungsverluste und damit einen geringeren Verlust der erzeugten Leistung. Um Kraftstoff zu sparen.

**10) Wodurch ist die Leistungssteigerung durch Aufladung eines Otto-Motors begrenzt?**

Ladedruck kann nicht unbegrenzt erhöht werden. **Warum?**
Durch die Klopfgrenze des Kraftstoff-Luft-Gemisches. 
Lädt man einen Ottomotor zu stark auf, kommt es zu einer ungewollten Kompressionszündung, der sogenannten klopfenden Verbrennung.

Klopfgrenze, **wodurch tritt eine klopfende Verbrennung ein?** Ungewollte Glühzündung, **wodurch entsteht eine Glühzündung?** Durch zu viel Druck und Hitze.

**11) Wassereinspritzung**

**Aufbau:** Wassertank, Einspritzdüsen

**Sinn?**

- dem Brennraum die Temperatur entziehen
- dadurch Klopfneigung reduzieren 
- Ladedruck erhöhen 
- Leistung ausschöpfen

**Kompensieren der Außentemperatur** z. B. 40 °C

- durch mehr Wasser Einspritzen 
- wird vom Motorsteuergerät überwacht 
- Last/Drehzahl abhängig 
- Ansaugluft 25 °C zusätzlich runterkühlen 
- 8 \% höhere Leistung und gleichzeitig 8 \%  Kraftstoffeinsparung

**Vorteil**

Die Temperaturen von $\to$ Kolbenboden, Ventile, Katalysator, Lader entlasten.

**Einspritzung - Zerstäubung** unter einem hohen Druck möglichst fein zerstäuben (Mehrlochdüse) Tröpfchenbildung (Kugeloberfläche).
Je feiner ich zerstäube, umso höher ist die Wahrscheinlichkeit, dass ich einen vollständigen Verdunstungsprozess habe, der dazu führt, dass ich im Idealfall keinerlei Rußbildung erzeuge.
Bei bestimmten Lastzuständen, hohen Einspritzdruck und kurzer Einspritzzeit habe ich das Problem, dass die Tröpfchengröße ansteigt und so zu einer Entstehung von Ruß kommt.