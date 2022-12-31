---
title: 'Motorsteuerung'
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
Thema:  Motorsteuerung
Fachbuch ([@brand:2020:fachkundeKfz] S. 243)
Fachbuch ([@respondeck:2019:servicetechniker] S. 142)
Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 281)
FS ([@bell:2020:formelsammlung] S. 32 - 37)
#
## 
ju 28-10-22
+----------------------------------------------------->

# Was ist ein Untengesteuerter Motor? 

Anordnung der Ventile

Fachbuch ([@brand:2020:fachkundeKfz] S. 242)

## Untengesteuerter Motor 

"stehende Ventile" (Ventilteller ist oben)

- Ungünstige Brennraumform, schlechter Wirkungsgrad
- *z. B. Harley-Davidson, Rasenmähermotoren*
- Flatheadmotor, sv-Motor

## Obengesteuerter Motor 

"hängende Ventile" (Ventilteller ist unten)

# Anordnung der Nockenwelle (Steuerungsbauarten)

Fachbuch ([@brand:2020:fachkundeKfz] S. 242)

<!--01_Anordnung-der-Nockenwelle_Skizze vgl. abb.-->
![Anordnung der Nockenwelle](images/Skizze/01_Anordnung-der-Nockenwelle_Skizze.pdf){width=60%}

## sv-Motor

- "side valves" seitlich stehende Ventile
- untengesteuerter Motor
- unten liegende Nockenwelle

## ohv-Motor

- "overhead valves" hängende Ventile
- obengesteuerter Motor
- unten liegende Nockenwelle
  
## ohc-Motor

- "overhead camshaft"
- Nockenwelle über Zylinderkopf 
  
## dohc-Motor

- "double overhead camshaft"
- zwei Nockenwellen über Zylinderkopf

## cih-Motor

- "camshaft in head"
- Nockenwelle im Zylinderkopf

# Arten von Nockenwellenantriebe

Fachbuch ([@brand:2020:fachkundeKfz] S. 247)

1. Steuerkette 
1. Zahnriemen 
1. Königswelle 
1. Stirnräder
1. Schubstangenmotoren

# Nenne Zahnriemen Merkmale (trocken laufend)

Fachbuch ([@brand:2020:fachkundeKfz] S. 247)

- geringe Masse 
- geräuscharmer Lauf 
- begrenzte Standzeit, begrenzte Belastbarkeit 
- Unterliegen einem Wartungsintervall
- braucht keine Schmierung
- kostengünstig in der Produktion
- Chemisch sensibel

# Ölbadzahnriemen Eigenschaften (nass laufend)

- mit Öl geschmierter Lauf 
- geringere Geräuschentwicklung
- geringere Reibung ($20~\%$ weniger als Steuerkette) 

**Ziel:** 

- Kontaktflächen der beweglichen Teile reduzieren $\to$ Emissionen
- Thermomanagement: Betriebstemperatur lange halten (BMW)

# Steuerkette Merkmale

1. Große Kräfte übertragen
2. eigentlich wartungsarm, aus praktischer Sicht leider problembehaftet
3. teuer in Konstruktion 
4. Steuerkette gilt als lauter
5. größere Masse als ein Riemen

# Stirnradantrieb

- Große Kräfte übertragen 
- wartungsfrei 
- schmale Bauform 
- teuer in Konstruktion 
- Dauerläufer (nicht problembehaftet)

# Königswelle

- wartungsfrei 
- leicht, weil hohl gebohrt, Hohlröhre 
- kleine Kräfte übertragen 
- teuer in Konstruktion und Herstellung

# Unterschied - Steuern und Regeln

**Steuern** Soll-Ist-Vergleich 

z. B. *Steuerkette*: Markierung soll auf OT stehen, alles in Ordnung, wenn nicht, dann defekt.

**Regeln** Soll-Ist-Vergleich mit der Option des Eingriffs 

z. B. Steuerrad Kapitän, *ABS Regelkreis*: SG erfasst Drehzahlsignal, 
Drehen alle Räder gleich schnell, alles okay. Dreht ein Rad schneller $\to$ aktiver Eingriff ins System.



# Nockenwellen - Herstellungsmöglichkeiten

## Gegossene Nockenwelle

- muss nachgearbeitet werden, Lagerstellen, partiell gehärtet 
- biegsam, flexibles Bauteil (Gusseisen mit Lamellen- o. Kugelgrafit)
- *Vorteil* kostengünstig in der Herstellung, weniger problembehaftet

(*Kaltverformen* je härter ein Material, um zu spröder.)

## Gebaute Nockenwelle

- zwei unterschiedliche Materialien, 
- Nocken (aus Einsatz-, Vergütungs- o. Nitrierstahl) auf ein Stahlrohr geschrumpft 
- *Problem* Nocken können sich verdrehen 
- *Vorteil* Gewichtsreduzierung, Nocken ist belastbarer 
- *Nachteil* Aufwand
- Material V4A (hohl gebohrt)

# Nockenformen

Fachbuch ([@brand:2020:fachkundeKfz] S. 246)

<!--02_Nockenformen_Skizze vgl. abb.-->
![Nockenformen](images/Skizze/02_Nockenformen_Skizze.pdf){width=60%}

## spitzer Nocken (tagenden Nocken)

- langsames Öffnen / Schließen der Ventile
- kurze Zeit voll geöffnet  
- geringe Füllung 
- stabiler Leerlauf 
- weicher und komfortorientierte Drehzahlbereich
- nicht als hochdrehender, hochbelasteter Motor geeignet
  
## steiler Nocken (scharfer Nocken, Kreisbogen Nocken)

- schnelles Öffnen / Schließen der Ventile
- bleibt längere Zeit voll geöffnet 
- hoher Füllungsgrad, bei hohen Drehzahlen 
- im Leerlauf teilweise unrunder Lauf, da "inneres AGR" entstehen kann 
  (große Ventilüberschneidung $\to$ Abgase in Ansaugtrakt)
  Abhilfe: Leerlaufdrehzahl erhöhen (750 $\to$ 950 U/min.)
- Leistungsmotoren, hohe Drehzahlen
  
## unsymmetrischer Nocken

- *flach* langsameres öffnen der Ventile
- *steil* schnelles schließen der Ventile
- längeres offen halten der Ventile
- vereinigt beide Varianten

(*Ziel bei hohen Drehzahlen*: Ventile schnell öffnen (Nocken) / schließen (Ventilfeder) $\to$  gute Füllung, hohen Wirkungsgrad erreichen.)

# Arten von Ventilbetätigung

Fachbuch ([@brand:2020:fachkundeKfz] S. 247, 242)

<!--03_Arten-von-Ventilbetaetigung_Skizze vgl. abb.-->
![Arten von Ventilbetätigung](images/Skizze/03_Arten-von-Ventilbetaetigung_Skizze.pdf){width=60%}


## Rollenschlepphebel, Schlepphebel, Schwinghebel 

- einarmige Hebel
- geringe Reibung zwischen Nocken und Schlepphebel durch Nockenrolle (nadelgelagert)

## Kipphebel

zweiarmige Hebel

## direkt

Nockenwelle - Hydrostößel - Ventil

# Welche Beanspruchung ist das Ventil ausgesetzt?

## Mechanische Beanspruchung des Ventils

- Ziehen (Ventilfeder, schließen, Ventilsitz)
- Druck (Nocken, öffnen) 
- Torsion (verdrehen) 
- Biegen 

## Chemische Beanspruchung

Schwefel im Kraftstoff $\to$ Korrosion

## Thermische Belastung

Auslassventil bis $900^\circ\text{C}$


# Ventilspielausgleich

**Wofür?** Temperaturänderung (Motor Kaltstart, temperaturbedingte Längenänderung des Ventils ausgleichen)

**Zu kleines Ventilspiel** (Nachteile)

- Ventil öffnet früher und schließt später
- Ventil ist länger auf
- kann dadurch nicht genügend Wärme abgeben über Ventilsitz
- Ventilteller wird immer weiter einer höheren thermischen Belastung unterzogen und dadurch erhöhter Verschleiß
- Am Ende ist das Ventil einer Hochtemperaturkorrosion unterworfen (Verbranntes Ventil)


**zu großes Ventilspiel** (Nachteile)

- Ventil öffnet zu spät, geht nicht ganz auf und schließt zu früh
- Ventil ist kürzer auf
- Klappergeräusche und erhöhter Verschleiß, *Warum?* durch großes Ventilspiel, liegt nicht am Nockengrundkreis auf (Nocken schlägt auf Ventil)
- Hieraus können folgen: schlechte Zylinderfüllung und die  maximale erreichbare Leistung sinkt

## definiertes Ventilspiel 

Wartung notwendig

## Hydraulischer Ventilspielausgleich

**ablaufender Nocken** (ohne Belastung)

- Entspannung des Systems 
- Spielausgleichsfeder drückt Druckbolzen nach oben bis Stößel am Nocken anliegt 
- Kugelventil öffnet sich, Raumvergrößerung im Arbeitsraum (Unterdruck)
- Durch den Systemdruck strömt frisches Öl von außen ein und der Arbeitsraum wird befüllt 

**auflaufender Nocken** (mit Belastung)

- Kugelventil schließt sich, es baut sich Druck im System auf
- durch die Inkompressibilität von Flüssigkeiten $\to$ starre Verbindung
- Nocken wird auf den Stößel auflaufen können, ohne Spiel zu haben und das Ventil betätigen 
- *Warum Ringspalt?* (Wärmeausdehnung des Öls ausgleichen)
- dadurch wird "Öl" durch den kleinen Ringspalt gepresst (definierte Ölmenge) 

**Bemerkung** Wärmeeintrag: "Je wärmer das Öl, umso dünnflüssiger."
Erfordert die *richtige Öl-Viskosität* (Zähflüssigkeit, Temperaturabhängig, Fließverhalten), sind an diese Ringspalte angepasst. 

*falsche Öl-Viskosität* ein Klappern oder Aufpumpen der Hydrostößel $\to$ darf nicht sein sonst Thermische Überlast, Hochtemperaturkorrosion $\to$ verbrannte Ventile

Fachbuch ([@brand:2020:fachkundeKfz] S. 245)

<!--04_Ventilspielausgleich_Skizze vgl. abb.-->
![Ventilspielausgleich](images/Skizze/04_Ventilspielausgleich_Skizze.pdf){width=60%}


# Drehzahlverhältnis zwischen Kurbelwelle zu Nockenwelle?

2:1

# Was steuert die Motorsteuerung?

Den Zeitpunkt und die Dauer des Ansaugens der Frischgase und den Zeitpunkt und die Dauer des Ausstoßes der Abgase.

Öffnen und Schließen der Ventile.

**Voraussetzung** 

1. Einspritzung des Kraftstoffs (Energieträger)
2. Eine Zündung, die diese Energie, gebunden im Kraftstoff, in chemische Energie, in Wärmeenergie umwandelt (Wärmekraftmaschine)

Druck wird über eine Fläche in Kraft und Drehmoment übertragen, an die Kurbelwelle übergeben, läuft durch das Getriebe - Achswellen - Reifen auf die Straße und wir haben Vortrieb.

# Dreiventiltechnik mit zwei Zündkerzen

Fachbuch ([@brand:2020:fachkundeKfz] S. 243)

Fachbuch ([@respondeck:2019:servicetechniker] S. 142)

## Zusammenfassung


<!--05_Dreiventiltechnik_Skizze vgl. abb.-->
![Dreiventiltechnik](images/Skizze/05_Dreiventiltechnik_Skizze.pdf){width=20%}

Wir haben bei **drei Ventilen** einen großen Ein- und Auslassquerschnitt.

Durch die Anordnung ist eine Unterbringung von **zwei Zündkerzen** möglich, sodass zwei Zündkerzen in der Nähe der Zylinderwand entstehen in deren Umgebung zwei Flammfronten. Somit kann bereits niedergeschlagener Kraftstoff noch verdampfen und verbrannt werden.

Durch zwei Zündkerzen findet die Verbrennung schneller statt. Dadurch wird der maximale Kolbendruck früher erreicht und ein hohes Drehmoment erreicht. Wir nähern uns einer Gleichdruckverbrennung (Isobar).

**Klopfneigung** wird durch zwei Zündkerzen verringert. Da geringere Wärmeeintrag in die noch nicht verbrannten Gase stattfindet. 

**Abgastemperatur** ist niedriger, dadurch geringerer NOx-Ausstoß trotz geringer HC und CO-Werte.

Dank nur **einem Abgasrohr** geringere Wärmeverluste. "light off point" des Katalysators wird schneller erreicht.



## Warum sind das zwei Einlassventile und ein Auslassventil?

**Vorteil** 

- kleine Massen 
- zwei kleine Ventile $\to$ große Einlassquerschnitte 
- höhere Drehzahlen 
- gute Füllung und Zylinderspülung
  
**Nachteil** 

- mehr Teile $\to$ größere Reibungsverluste 
- Verschleiß und Ausfallwahrscheinlichkeiten

**Ein großes Ventil** hat eine Massenträgheit.

- Masse in Ruhelage (Ventil offen), Losbrechmoment  $\to$ höchste Kraft, Masse in Bewegung (Federkraft: Ventil schließen)
- Ansaugventil möglichst lange offen lassen (Kolben und Ventil kommen sich sehr nahe)
- *Ziel:* bestimmte Drehzahl erreichen (Wie schnell kann dieser Wechsel vollzogen werden?)

## Zylinderspülung bei Ventilüberschneidung

Mit dem Ausstoß der Abgase ziehen wir einen kleinen definierten Frischgasanteil mit, um den Zylinder zu spülen und möglichst wenig inertes Gas (AGR) zu gewährleisten.

## Nachladeeffekt beim Ansaugen

Einlassventile werden erst nach Durchschreiten des unteren Totpunktes geschlossen.
Frischgase strömen trotz aufwärtsgehendem Kolben in den Zylinder nach.
Die Kinetische Energie der einströmenden Frischgase ist größer, als die Druckzunahme durch aufwärts gehenden Kolben.

## Warum zwei Zündkerzen?

Zündkerze ist in der Nähe der Zylinderwand, zwei Flammenfronten entstehen.

1. **Vollständige Verbrennung**
   - niedergeschlagener Kraftstoff verdampft (an Zylinderwandung und Feuersteg) und der Verbrennung zugeführt
2. **schnellerer Verbrennungsablauf**
   - Schnelleres erreichen des maximalen Verbrennungsdruckes. Die Temperatur kann schneller konstant gehalten bzw. in Druck umgewandelt und über die Fläche des Kolbens in Kraft und Drehmoment auf die Kurbelwelle übertragen werden.
   - Drehmoment = Kraft (max. Kolbendruck) x Hebelarm (90° stehende Kurbelwellenzapfen = Hebelarm am größten)

## Innermotorisch entstehen geringere Schadstoffe

1. **HC** geringer Ausstoß unverbrannter Kohlenwasserstoffe, durch weniger niedergeschlagener Kraftstoff
2. **CO** geringer, durch vollständige Verbrennung
3. **NOx** ist reduziert, durch schnelleren Verbrennungsablauf $\to$ zwei Zündkerzen, Abgastemperatur ist niedriger

## Wann entsteht NOx?

Durch hoher Druck und hohe Temperatur.

## Zusammenhang zwischen HC und CO vs. NOx

Es gibt zwei Zündgrenzen "fett" und "mager".

1. **HC und CO** entsteht durch unvollständige fette Verbrennung
   - Senken: durch Abmagern 
   - Verbrennungsspitzentemperatur: geringer
2. **NOx** entsteht durch magere Verbrennung
   - Senken: durch anfetten
   - Verbrennungsspitzentemperatur: ansteigen

## Schadstoffe 

1. **HC** unverbrannte Kohlenwasserstoffe 
   - Verdampft am Ende der Verbrennung und wird dem Abgas zugeführt
2. **CO** Kohlenmonoxid
   - schwerer als Luft (Grube), bindet Hämoglobin im Blut
   - keine vollständige Verbrennung
3. **NOx** Stickoxide

## Was ist AGR?

Platzhalter Gas (inertes Gas) nimmt nicht an der Verbrennung teil, soll den Umgebungssauerstoff fernhalten

AGR-Rate ist am größten in Teillast (80 Km/h auf der Landstraße)

Ziel: Aus großen Motor $\to$ kleinen Motor machen, viel Abgas und geringe Menge Kraftstoff einspritzen

*Problem* "Luftmenge ist da und kein Kraftstoff Einspritzen"  $\to$ magere Verbrennung $\to$ thermische Belastung und Anstieg NOx

*Luftmassenmesser* misst angesaugte Luftmasse und Sauerstoffgehalt $\to$ AGR-Rate $\to$ Kraftstoffmenge berechnen

Ziel: homogen - Magerbetrieb (über den kompletten Zylinder)

## Wie entsteht Ruß?

Kraftstoff wird an heißen Luft eingespritzt, zündfähiges Kraftstoff-Luft-Gemisch bildet sich

*einzelne Kraftstofftröpfchen* 

- fangen von außen an zu verdunsten, entzünden, Verbrennung ist zu kurz (nicht vollständig)
- innen: Verbrennung von Kohlenwasserstoff ohne Sauerstoff

## Was fördert die Klopfneigung?

Unkontrollierte, unerwünschte Verbrennung (Glühzündung, klingende, klopfende Verbrennung)

entzündet sich selbst an etwas glühenden, z. B. Ölkohle, Masseelektrode (Zündkerze)

Wärme braucht Zeit zum Wirken. 

1. **Wärmeeintrag gering:** geringe Klopfneigung, geringe thermische Belastung, schneller Verbrennungsablauf 
2. **Wärmeeintrag hoch:** klopfende Verbrennung

## Ein Auslassventil - ein Abgasrohr

Abgas verliert weniger Wärmeenergie.

1. ab ca. 450 °C "light off point" des Katalysators: min. $50~\%$ der Abgase konvertiert in nicht Schadstoffen

2. ab ca. 650 °C altert der Katalysator exponentiell und thermische Belastung

**Thermodynamik - warme Luft strömt** schneller, weniger Rückstau.

Das unter Druck stehende Abgas verlässt den Zylinder mit Überschall (Auspuffgeräusch). 
**Schallgeschwindigkeit** ca. 343 m/s (z. B. Blitz $\to$ Donner, drei Sekunden zählen $\to$ ca. 1 km Entfernung)

