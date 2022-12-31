---
title: 'Gemischbildung-Diesel'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!-----------------------------
![ , Quelle: Europa-Verlag](images/CR/.png){width=70%}
Bosch S. ([@reif:2022:boschkraftfahrtechnisches]).
$850^\circ\text{C}$
ju 18-12-22 Gemischbildung-Diesel
+------------------------------>

**1892** erfand "Rudolf Diesel" den Motor, der heute PKW, LKW, Busse, Schiffe, Panzer, Baumaschinen,
Landmaschinen und Gabelstapler antreibt und der auch stationär zur Stromerzeugung
eingesetzt wird.

# Eigenschaften Dieselmotor 

1. Selbstzündung (Kompressionszündung)
1. Innere Gemischbildung (Brennraum)
1. Qualitative Gemischregulierung (Die eingespritzte Kraftstoffmenge reguliert die Leistung des Motors.)
1. Heterogenes Gemisch (Das Gemisch aus Luft und Kraftstoff ist im Brennraum nicht gleichmäßig verteilt.)
1. Hohes Luftverhältnis (Luftüberschuss, d.h. das Verhältnis von Luft zu Kraftstoff ist sehr groß.)
1. Zündwilliger Kraftstoff (hoch siedend, hohe Cetanzahl)

# Warum gibt es einen Klopfsensor beim Diesel?

Einspritzüberwachung (früher Nadelbewegungssensor): Einspritzbeginn, Zündbeginn, wie sauber ist die Verbrennung?

**Was ist ein Klopfsensor?** (am Motorblock verbaut)
Piezo-Element: wenn die seismische Masse in Schwingung gerät, wird durch die Bewegung eine Spannung erzeugt und im SG verarbeitet. Eine klopfende Verbrennung wird durch eine ungewöhnlich große Schwingung im Motor erkannt.

# Welche Arten von Dieselmotoren gibt es?

- Direkteinspritzung (erste 1988 Audi)
- Indirekte Einspritzung (Vorkammer und Wirbelkammer)
    - kugelförmig - Vergrößerung der Oberfläche - Wärmeverluste $\to$ kompensieren durch hohe Drücke und Temperaturen
    - Vorverbrennung $\to$ weiche Verbrennung
- Saugrohreinspritzung
- Turbo aufgeladen

# Warum haben wir eine höhere Verdichtungsendtemperatur als die Selbstentzündungstemperatur?

Das Gemisch muss sich schlagartig und schnell genug entzünden und sauber genug durchbrennen.

Gay-Lussac - Faktor 2 S. 193 ([@brand:2020:fachkundeKfz]) Erwärmt man das Gas um $273~K$, so dehnt es sich auf das doppelte aus. Verhindert man die Ausdehnung beim Verdichten, so verdoppelt sich der Druck.

- Verdichtungsverhältnis: $14 - 27:1$
- Verdichtungsendtemperatur (Lufttemperatur): $600 - 900^\circ\text{C}$
- Verdichtungsenddruck: $30 - 55~\text{bar}$
- Selbstzündungstemperatur (untere Grenze) $220^\circ\text{C}$ (im Mittel) bei ca. $350^\circ\text{C}$ Quelle: Bosch S. 562 ([@reif:2022:boschkraftfahrtechnisches]).
- Verbrennungshöchstdruck: $200~\text{bar}$
- Druck beim Öffnen des Auslassventils: $4 - 6~\text{bar}$
- Abgastemperatur: $550 - 750^\circ\text{C}$

**vgl. Otto-Saugmotor**

- Verdichtungsverhältnis: $7-12:1$
- Verdichtungsendtemperatur (Lufttemperatur) $400 - 500^\circ\text{C}$
- Verdichtungsenddruck: $18~\text{bar}$
- Selbstzündungstemperatur (im Mittel) $500^\circ\text{C}$ Quelle: Bosch S. 562 ([@]reif:2022:boschkraftfahrtechnische)
- Verbrennungshöchstdruck: $30 - 60~\text{bar}$
- Druck beim Öffnen des Auslassventils: $3 - 5~\text{bar}$
- Abgastemperatur: $900^\circ\text{C}$

Ein **Arbeitsspiel** läuft in zwei Kurbelwellenumdrehungen ab $720^\circ\text{KW}$ (Kurbelwinkel). Die **vier Takte des Arbeitsspieles** sind Ansaugen, Verdichten, Arbeiten und Ausstoßen. **Ein Takt** ist zwischen UT und OT.

**Ottomotor / Saugrohreinspritzung** 

1. Motor / Drosselklappe (fast geschlossen -- offen)
1. Ansaugen (geringe -- maximale Menge Kraftstoff-Luftgemisch)
1. Füllung (schlecht -- maximal)
1. Verdichtungshöchstdruck (gering -- maximal)
1. Zündung des Kraftstoff-Luftgemisches, nach der Verbrennung
1. Verbrennungshöchstdruck (gering -- maximal)
1. wirkt auf die Kolbenfläche und wird auf $\to$ Kolben $\to$ Pleuel $\to$ Kurbelwelle übertragen
1. Drehmoment an Kurbelwelle (gering -- maximal)
1. Drehzahl des Motors (gering -- maximal)

# Nageln

**Nageln** ist ein harter Motorlauf und entsteht durch zu großer Zündverzug, zum Beispiel beim Kaltstart des Motors (schlagartige Verbrennung), kann gemindert werden durch Voreinspritzung.

**Zu großer Zündverzug tritt ein ...**

1. kaltem Motor oder kalter Ansaugluft
1. schlechter Kompression
1. Kraftstoff mit zu niedriger Cetanzahl
1. tropfenden Injektoren

# Quantitätsregelung und Qualitätsregelung

**Quantitätsregelung** Ottomotor - Regulierung über die Gemischmasse, Drosselklappe (Lastzustand) Menge von Luftmasse (Luftmassenmesser) und Kraftstoffmasse, um das Ziel Lambda = 1 zu erreichen, wird die Kraftstoffmasse angepasst.

**Qualitätsregelung** Dieselmotoren - Regulierung über die Kraftstoffmasse, keine Drosselklappe (systembedingt) nahezu konstante gleiche Menge Luftmasse, aber die Größe der Kraftstoffmasse kann geändert werden in Abhängigkeit des Lastwunsches.

# Verbrennungsablauf beim Dieselmotor

**Verbrennung am Kraftstofftröpfchen** Ausgangslage: Dieseltropfen wird eingespritzt, Umgebungsluft $600 - 900^\circ\text{C}$, Kraftstofftröpfchen so gut wie möglich zu verdampfen.

Das Ziel ist ein zündfähiges Gemisch an der Außenlufttemperatur von selbst zu entzünden, da nur eine sehr geringe Zeit zwischen Einspritzzeit und kurz vor Ende des Verbrennungsprozesses besteht. Um die Kraftstofftröpfchen so klein wie möglich zu halten, werden sehr hohe Drücke und Temperaturen angestrebt.

**Unvollständige Verbrennung** (durch Sauerstoffmangel)

Wie kann das sein, wir haben doch Sauerstoffüberschuss?

Je größer der Kraftstofftropfen, desto größer ist der Bereich, wo Luftmangel herrscht.

**Ursachen für Partikel und Rußbildung** durch unvollständige Verbrennung

1. Kaltstart- und Warmlaufphase (kalter Motor hat geringere Kompression, Kondensationsverluste an Zylinderwand, Wärmeabgabe an Brennraumwände)
1. Volllastbetrieb (Kraftstoffüberschuss)
1. Sauerstoffmangel (verstopfter Luftfilter, defekter Turbolader, undichter Ladeluftkühler)
1. Defekte Injektoren (schlechtes Strahlbild, tropfen nach $\to$ mehr Kraftstoff)
1. Kompressionsverluste (Blow-by, Verdichtungstemperatur wird später erreicht)

# Was ist EDC? Nenne Aufgaben, Vorteile, Ziele und Merkmale

**EDC** (Electronic Diesel Control, elektronische Dieselsteuerung, Motorsteuerung), Kennfeld (Sollwerte) geregeltes elektronisches Einspritzsystem (Einspritzsteuerung)

**Motorsteuerung Aufgaben** (Auswahl)

1. Einspritzung des Kraftstoffes
    - zu jedem Zeitpunkt die gerade erforderliche Menge an Kraftstoff in die Zylinder des Motors einzuspritzen.
1. Regelung und Begrenzung von Drehzahl und Geschwindigkeit,
1. Regelung des Luftsystems (Abgasrückführung und Ladedruckregelung),
1. Abgasnachbehandlung,
1. Glühkerzensteuerung und Thermomanagement,
1. Zylinderabschaltung,
1. Diagnose,
1. Wegfahrsperre.

**Vorteile** bedarfsgerechte Regelung

**Ziele** Einspritzbeginn und Kraftstoffmenge exakt zu regeln

**Merkmale** Optimieren von Schadstoffen, Verbrauch, Drehmoment und Leistung, Laufruhe

# Was sind die Hauptsteuergrößen eines jeden Motors?

Last und Drehzahl (Fahrpedalwertsensor, Drehzahlsensor der Kurbelwelle)

**Korrektursteuergrößen** anpassen der Grundeinspritzzeiten (abhängig vom Motor)

Einspritzbeginn, $NO_\text{x}-\text{Wert}$, Motortemperatur, Fahrgeschwindigkeit, AGR-Rate, Ladedruck, Ansauglufttemperatur, Kraftstofftemperatur, usw.

# Einspritzsysteme

1. **Reiheneinspritzpumpe**
    - Einspritzdruck bis etwa 1300 bar
    - Mengenregelung und Förderbeginn (Fliehkraftregler)
1. **Axialkolben-Verteilereinspritzpumpe** (VE)
    - Einspritzdruck bis etwa 1400 bar
    - Mengenregelung (Verschieben des Regelschiebers) und Förderbeginn (hydraulische Spritzversteller), Drehzahl (Fliehkraftregler)
1. **Radialkolben-Verteilereinspritzpumpe** (VP44)
    - Einspritzdruck bis etwa 1900 bar
1. **Pumpe-Düse System mit Magnetventil**
    - Einspritzdruck bis etwa 2200 bar
1. **Pumpe-Düse System mit Piezoventil**
1. **Pumpe-Leitung-Düse System** (PLD, Nfz)
1. **Common-Rail System**

## Pumpe-Leitung-Düse System 

Pro Zylinder ein Pumpenelement und eine Einspritzdüse. Einspritzdruck bis etwa 1800 bar. Eine elektrisch geregelte Voreinspritzung ist aufgrund der Trägheit des Systems nicht möglich (Länge der Kraftstoffwege). Um eine Voreinspritzung realisieren zu können, kommen spezielle Einspritzdüsen zum Einsatz. Die sogenannten Zweifeder-Düsenhalter (kleine Feder - Voreinspritzung, große Feder - Haupteinspritzung).


\newpage
## Pumpe-Düse System mit Magnetventil 

**Erkläre die Vorgänge - Befüllen, Voreinspritzung, Haupteinspritzung eines PDE**

**Befüllen** bei ablaufenden Einspritznocken wird der Pumpenkolben nach oben gezogen und der Hochdruckraum wird mit Kraftstoff befüllt. Solange Magnetventil offen ist, fließt der Kraftstoff durch den Hochdruckraum in den Rücklauf ab. (kühlende Wirkung)

Bei auflaufenden Nocken wird der Pumpenkolben nach unten gedrückt. Das *Magnetventil* ist geschlossen und verschließt Kraftstoff Vor- und Rücklaufleitung. Es baut sich ein Hochdruck auf.

**Voreinspritzung** (Beginn) bei etwa 180 bar ist der Druck größer als die Düsen-Federkraft. Durch das Einspritzen des Kraftstoffs haben wir einen kurzen Druckabfall und die Düsennadel schließt (Ende).

Der Ausweichkolben hat seine schräge Druckschulter freigegeben (große Fläche, große Kraft), wodurch er nach unten gedrückt wird und spannt die Düsenfeder vor.

*Magnetventil* öffnet und der überschüssige Kraftstoff entweicht in die Vor- und Rücklaufleitung.

**Haupteinspritzung** der Druck steigt weiter und drückt bei etwa 300 bar die Düsennadel nach oben (Ende). Durch den Druckabfall schließt die Düsennadel.

**Nachteile des Pumpe-Düse Systems mit Magnetventil** 

1. Druckerzeugung ist abhängig von Einspritznocken zum Pumpenkolben
1. Druck ist nicht konstant, sondern 300 bis 2200 bar (Kraftstofftröpfchengröße)
1. Hohe Kräfte können auf den Zahnriemen wirken
1. Keine Nacheinspritzung (zu Regeneration von DPF)
1. Kein mehrmaliges Vorspritzen möglich

\newpage
<!--CR-5 vgl. abb.-->
![Pumpe-Düse System, Quelle: Europa-Verlag](images/Diesel/Diesel-11.pdf){width=70%}

1. Drallkanal
1. Füllkanal
1. Auslasskanal
1. Einlassnockenwelle
1. Kraftstoffrücklauf
1. Auslassnockenwelle mit Einspritznocken 
1. Kolbenfeder
1. Einspritznocke
1. Rollenkipphebel
1. Ausweichkolben
1. Pumpenkolben
1. Magnetventil PDE
1. Einstellschraube Spielausgleich PDE
1. Kraftstoffzulauf
1. Hochdruckraum

**Einspritzvorgang**

1. Nockenhub wird über den Rollenkippebel auf den Pumpenkolben übertragen
1. **Magnetventil angesteuert** und verschließt Kraftstoffzulauf und -rücklauf
1. Druckaufbau im Hochdruckraum beginnt
1. Bei ca. 180 bar ist der Druck größer als die Federkraft. **Voreinspritzung beginn**
1. Ausweichkolben öffnet Ausgleichsraum, kurzer Druckabfall. **Voreinspritzung ende**
1. Bei ca. 300 bar überwindet der Kraftstoffdruck die Kraft der vorgespannten Feder. **Haupteinspritzung beginn**
1. **Magnetventil nicht angesteuert** und öffnet den Kraftstoffzulauf und -rücklauf.


**steile Flanke des Einspritznockens** bewirkt einen schnellen Druckanstieg.


## Pumpe-Düse System mit Piezoventil 

**Piezoelektrische-Effekt** (direkt), übt man auf einen Piezokristall Druck aus, so erzeugt dieser eine Spannung. 

*Verformung* durch Druck / Krafteinfluss

*Anwendung:* Klopfsensor, Drucksensor (Click-Feuerzeug)

**Reziproker Piezoelektrischer-Effekt** (invers) legt man an einen Piezokristall eine Spannung an, so verformt er sich. Die Längenänderung ist proportional zur angelegten Spannung. 

*Verformung* durch Spannungseinfluss

*Anwendung:* Injektor

Kfz: Steuerspannung 110-150 V, max. Ausdehnung 0,15 \%

Piezoventil ersetzt Magnetventil (Trägheit - Magnetventil bewegt sich zeitversetzt, weil der Magnetfeldaufbau gehemmt wird, durch Gegeninduktion)

**Piezoventil (Piezoaktor)** besteht aus Piezoaktormodul und Übersetzermodul (kl. Hebelwerk)

Die Längenausdehnung eines Piezokristalls liegt bei maximal 0,15 \% (sehr gering). Werden, bis zu 500 Piezokristalle in Reihe geschaltet ist die Gesamtausdehnung des Piezoaktormodul etwa 0,04 mm. Zum Erreichen der erforderlichen Ventilöffnung von 0,1 mm wird ein kleines Hebelwerk, sogenannte Übersetzermodul zwischen Piezoaktormodul und hydraulischen Ventil geschaltet.

**Piezoventil geschlossen**, die Verbindung zwischen Hochdruckraum zur Vor- und Rücklaufleitung ist unterbrochen. Hochdruck kann sich aufbauen und es wird eingespritzt.

**Piezoventil offen**, die Verbindung zwischen Hochdruckraum zur Vor- und Rücklaufleitung ist wieder hergestellt. Hochdruck entweicht und der Einspritzvorgang ist beendet.



# Einspritzventile 

- Ein- und Zweifeder-Düsenhalter
- Loch- und Zapfendüsen

**Prüfen:** Öffnungsdruck, Strahlbild

# Glühsysteme

**Aufgabe von Starthilfsanlagen**

1. Anspringen des kalten Dieselmotors erleichtern 
1. runden und stabilen Leerlauf zu sorgen
1. Schadstoffemissionen zu senken

**Arten von Glühstiftkerzen**

1. **Selbstregelnde Glühstiftkerzen**
    - *Aufbau:* Heizwendel, Regelwendel, Keramikstift, Ringspalt
    - *Nennspannung:* 11,5 V
    - *Vorglühzeit:* 2 -- 7 s
    - *Glühtemperatur:* $850^\circ\text{C}$
    - *Leistungsaufnahme:* 100 W
    - *Regelung der Glühkerzenstromaufnahme:* Durch das PTC-Verhalten der Regelwendel wird die Stromaufnahme nach erreichen der Glühtemperatur begrenzt.
1. **Elektronisch geregelte Glühstiftkerzen**
    - *Aufbau:* Heizwendel, Regelwendel, Keramikstift, Ringspalt
    - *Nennspannung:* 5 -- 8 V
    - *Vorglühzeit:* 1 -- 2 s
    - *Glühtemperatur:* $1000^\circ\text{C}$
    - *Regelung der Glühkerzenstromaufnahme:* Die Glühkerzen werden pulsweitenmoduliert kurzfristig mit Überspannung von bis zu 11 V betrieben.
1. **Drucksensorglühstiftkerzen** (PSG, Pressure Sensor Glow Plug, Brennraumdruckgeber)
    - Einspritzzeitpunkt und Druckverlauf ermitteln
