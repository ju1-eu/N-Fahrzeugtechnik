---
title: 'Füllungsoptimierung-I'
author: 'Jan Unger'
date: \today
subject: "Markdown"
keywords: [Markdown,Latex,HTML,PDF,Pandoc,Shell-Script]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!----------------------------------------------------+
Dozent: Marc Limburg
Thema:  Füllungsoptimierung-I
Fachbuch ([@brand:2020:fachkundeKfz] S. 243)
Fachbuch ([@respondeck:2019:servicetechniker] S. 142)
Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 281)
FS ([@bell:2020:formelsammlung] S. 32 - 37)
#
## 
ju 16-4-22
+----------------------------------------------------->

# Downsizing (Prüfung) 

Verkleinerung der Motoren (Hubraum und Zylinderzahl) bei gleicher Leistung.

# LSPI - Low Speed-Pre-Ignition

LSPI = vorzeitige Zündung, betrifft hoch aufgeladene Downsizing Motoren [^1]

[^1]: <https://www.autobild.de/artikel/lspi-vorzeitige-zuendung-16385077.html>

- **Turbo aufgeladene Motoren** 
  - geringes Verdichtungsverhältnis (7-8:1)
  - vor verdichtete Luft wird in den Zylinder eingeblasen und verdichtet 
  - Ladedruckregelung (Lastwunsch) 
  - vorgewärmte Luft (Ladeluftkühlung)
- vs. **hoch verdichtete Saugmotoren** 
  - hohes Verdichtungsverhältnis (10-11:1), endet bei Klopfgrenze

**Zwei Zündquellen, Ursache für die Selbstentzündung**

1. Niedergeschlagen Kraftstoff in Verbindung mit sehr niedrig Viskoses Öl
   - $\to$ ein brennbares Gemisch entsteht, mit einer nicht ganz bekannten Selbstentzündungstemperatur
2. Ölkohlerückstände (Kraftstoffreste) im Bereich der Einspritzdüsen

Durch eine überhohe Verdichtung $\to$ steigt Verdichtungsenddruck und damit Verdichtungstemperatur $\to$ dadurch hohe thermische Belastung. Die Folge ist ein kapitaler Motorschaden.

**Körnerschlag** [^2] Kolbenschäden $\to$ es entsteht eine Druckspritze bevor der Kolben OT erreicht, eine zweite Flammenfront entsteht, wenn jetzt zwei Flammfronten aufeinandertreffen, entstehen sehr hohe Druckspitzen, auch wenn der Kolben nach UT geht. 

[^2]: <https://cdn.germanscooterforum.de/monthly_05_2009/post-24449-1241606436.jpg>

**Kavitation** [^3] Dampfblasenbildung [^4]  z. B. Bootsschraube saugt Flüssigkeiten an, Druck fällt ab durch Unterdruck, wenn jetzt die Gasblasen implodieren, entstehen sog. Mikrojets $\to$ Druckspitzen.
 
[^3]: <https://prozesstechnik.industrie.de/wp-content/uploads/4/0/40278086.jpg>

[^4]: <https://www.youtube.com/watch?v=SEGTFbZ5RJ8>

# Vorteile von Downsizing Motoren

1. Geringere Pumpverluste (2 l vs. 1,2 l bei gleicher Leistung 150 PS) 
2. geringere Reibungsverluste aufgrund der geringeren Größe 
3. weniger Wärmeübertrag von Gasen zur Zylinderwandung


# Mehrventiltechnik

Fachbuch ([@respondeck:2019:servicetechniker] S. 141)

Um die Zylinderfüllung zu verbessern, werden drei oder mehr Ventile pro Zylinder in Verbrennungsmotoren eingesetzt. 

**Ziele von Mehrventiltechnik**

- Öffnungsquerschnitt der Ventile vergrößern, ohne die Drehzahlfestigkeit durch größere und damit trägere Ventile (mehr Masse) zu mindern.
   
**Vor- und Nachteile von Mehrventiltechnik**

- bessere Zylinderfüllung
- Drehzahlfest
- innere Reibung steigt
- Abgaswärmeentzug
  - Der Katalysator kommt schlechter auf Betriebstemperatur, da sich die Abgase an den Abgasrohren abkühlen können. 
  - Je mehr Auslassventile vorhanden sind, desto größer ist die Oberfläche der Abgasrohre und desto mehr kühlen die Abgase aus.

Honda NR 750 - Ovalkolben [^5]

[^5]: <https://de.wikipedia.org/wiki/Honda_NR_750>

**Dreiventiltechnik** (Vorteile)

- Verbrennungsdruck steigt (kürzere Flammwege)
- geringere Klopfneigung (weniger Zeit zur Gemischerwärmung vor Verbrennungsbeginn)
- Ausstoß unverbrannter Kohlenwasserstoffe verringert sich (Zündkerze ist in der Nähe der Zylinderwand, wo das Kondensat lagert)
- geringere NOx

Vgl. Kapitel "*Motorsteuerung / Dreiventiltechnik mit zwei Zündkerzen*"

# Nockenwellenverstellung - variable Steuerzeiten

Fachbuch ([@brand:2020:fachkundeKfz] S. 249)

Verdrehen der Einlassnockenwelle bzw. der Ein- und Auslassnockenwelle, abhängig von der Motordrehzahl, Motorlast und Temperatur. 
Hierdurch lässt sich die *Länge der Ventilüberschneidung* anpassen.

**Warum machen wir eine Nockenwellenverstellung?** (Vorteile)

1. Optimale Zylinderfüllung in den unterschiedlichen Last- und Drehzahlbereichen zu ermöglichen 
2. inneres AGR

**Ziele der Nockenwellenverstellung** 

- Wann das Ventil öffnet und schließt zu beeinflussen (variabel)
- bei gleichbleibenden Nocken, Dauer und Öffnungswinkel (Hub) ändern sich nicht
- Verdrehrichtung der Nockenwelle: Früh, Spät

**Verstellung der Einlassnockenwelle in Abhängigkeit vom Betriebszustand**

| **Betriebszustand**  | **Leerlauf** | **Teillast** | **Volllast** |
|----------------------|--------------|--------------|--------------|
| Verstellrichtung NW  | Spät         | Früh         | Spät         |
| Ventilüberschneidung | klein        | groß         | klein        |
| Abgas                | CO sinkt     | NOx sinkt    |              |
| EV schließt          | weit nach UT | kurz nach UT | weit nach UT |

Merkmale (Vgl. Tabelle Verstellung der Einlassnockenwelle in Abhängigkeit vom Betriebszustand)

- **Leerlauf** Kein Überströmen von Frischgasen und Abgasen, besserer Verbrennungsverlauf 
- **Teillast** Abgase strömen in den Einlasskanal und werden mit den Frischgasen angesaugt. Temperatur sinkt, NOx-Anteil sinkt 
- **Volllast** *Nachladeeffekt* Frischgase strömen trotz aufwärts gehenden Kolben in den Zylinder nach

**Ausgangspunkt** $\to$ 90er-Jahre, erste Form des AGR (inneres AGR), Drei-Wege-Katalysator, Ottomotor, Euro 2, Teillast (höchste AGR-Rate, 80 km/h auf der Landstraße, keine Lastabfrage, Spritspareffekt, NOx-Anteil senken)

## VarioCam - Verstellbarer Kettenspanner (Audi, VW)

$\to$ Verändern der Ventilöffnungszeit der Einlassnockenwelle

**Wie?** Vgl. Tabelle Verstellung der Einlassnockenwelle in Abhängigkeit vom Betriebszustand

- KW treibt Auslass-NW an und diese über einer Kette die Einlass-NW
- **Kettenspanner** spannt **Kette nach oben** (federbelastet)
- **NW** dreht sich **gegen UZS** (Uhrzeigersinn) in **Verstellposition** "spät" (Ausgangslage, Ventilüberschneidung klein)
- SG bestromt Magnetventil, Motoröl fließt in Kettenspanner. 
- **Kettenspanner** spannt **Kette nach unten** (Hydraulikzylinder)
- **NW** dreht sich **im UZS** in **Verstellposition** "früh", (Ventilüberschneidung groß)

## Vanos - Variable Nockenwellensteuerung (BMW)

**Wie?** 

- **Nockenwellenrad und Nockenwelle** sind über ein **steiles Gewinde** miteinander verbunden. 
- *Grundposition* NW steht in **Verstellposition** "spät"
- SG bestromt ein Magnetventil (4/2-Wegeventil) $\to$ gibt den **Ölzufluss** zum Frühkanal frei
- NW verdreht sich gegen Uhrzeigersinn in **Verstellposition** "früh" 
- Durch wechselseitigen Druckaufbau lässt sich die Position der Verstelleinheit halten.
  
## Flügelzellenversteller (Mercedes)

$\to$ Verändern der Steuerzeiten

**Wie?** 

- **Innenrotor** (fest mit NW) **und Außenrotor** (fest mit Kettenrad)
- SG bestromt **Magnetventil** $\to$ die **Ölräume** zwischen den Rotorblättern können wechselseitig mit Öl befüllt werden 
- Die Kraftübertragung vom Nockenwellenrad auf die NW erfolgt immer über das Öl.
- wird Ölraum rechts vom Innenrotorblatt mit Öl befüllt, kommt es zu einer **Verdrehung der NW gegen UZS** (Uhrzeigersinn) in Richtung "spät"
- wird Ölraum links vom Innenrotorblatt mit Öl befüllt, kommt es zu einer **Verdrehung der NW im UZS** in Richtung "früh"
- Durch wechselseitigen Druckaufbau lässt sich die Position der Verstelleinheit halten.

# Variabler Ventiltrieb

## Stufenweise variabler Ventiltrieb

**Vorteile**

Bessere Zylinderfüllung durch zwei unterschiedliche Nockenprofile

- *obere Drehzahlbereich* $\to$ steiler Nocken 
  - schnelles Öffnen, lange Öffnungsdauer, schnelles Schließen

- *untere Drehzahlbereich* $\to$ spitzer Nocken 
  - Verhinderung von ungewollter Abgasrückführung durch zu lange Ventilüberschneidung

### VTEC - Variable Valve Timing and Lift Electronic Control (Honda)

$\to$ Verändern von Ventilhub und Ventilöffnungszeit

**Wie?** 

- Verstelleinheit liegt in den Schlepphebeln
- **Umschaltung** zwischen dem Nockenprofilen erfolgt durch **Verblocken der Schlepphebel**
- **Schlepphebel entriegelt** 
  - Die beiden äußeren Nocken öffnen mithilfe der äußeren Schlepphebel die Ventile.
  - **Spitzer Nocken**
    - kleiner Ventilhub
    - kurze Ventilöffnungszeit
    - *niedrige Drehzahlen*
- SG bestromt Elektromagnet, **Öldruck** verschiebt die **Sperrschieber** und verblockt die Schlepphebel untereinander.
- **Schlepphebel verriegelt**
  - wenn der steile Nocken auf den mittleren Schlepphebel aufläuft, nimmt dieser die beiden äußeren Schlepphebel mit und diese öffnen die Ventile.
  - **Steiler Nocken**
    - großer Ventilhub
    - lange Ventilöffnungszeit
    - *hohe Drehzahlen*

### VarioCam Plus (Porsche)

$\to$ Verändern von Ventilhub und Ventilöffnungswinkel

**Wie?** 

- Verstelleinheit liegt im Tassenstößel 
- SG bestromt **Elektromagnet**, damit wird der **Tassenstößel mit Öldruck** gesteuert
- Diese bestehen aus **zwei Stößeln**, die mithilfe eines **Bolzens** gegeneinander verriegelt werden können. 
- innere Stößel $\to$ kleinen Nocken
- äußere Stößel $\to$ großen Nocken 
- **Stößel verriegelt** $\to$ große Ventilhub 
  - Innere und äußere Stößel wird durch einen Bolzen verriegelt
- **Stößel entriegelt** $\to$ kleiner Ventilhub
  - sinkt der Öldruck, wird durch die Federkraft der Bolzen zurückgeschoben

### Valvelift (Audi, + Zylinderabschaltung)

**Wie?**

- Änderung des Nockenprofils durch Verschieben der Verstelleinheit (Nockenstück) auf der NW
- SG bestromt **Elektromagnet** $\to$ **Metallstift** fährt aus **in eine Spiralnut** und verschiebt das **Nockenstück**
- damit schalte ich zwischen **zwei Nockenprofilen** um
- Arretierung des Nockenstücks erfolgt durch eine federbelastete Kugel.
- **Zylinderabschaltung** (Teillast)
  - Nockenprofil $\to$ Nockengrundkreis
  - Die Ventile bleiben bei abgeschaltetem Zylinder geschlossen.

## Stufenlos variabler Ventiltrieb

**Vorteile**

$\to$ Verändern von Ventilhub in allen Drehzahlbereichen

**Ziel im unteren Drehzahlbereich**: Ein zündbares Gemisch zu realisieren. 

**Wie?** 

- Durch geringe Ventilöffnung und damit Erhöhung der Strömungsgeschwindigkeit der Frischgase 
  - "Venturi-Prinzip" eine Verengung in einem Strömungskanal 
    - $\to$ höhere Strömungsgeschwindigkeit 
    - $\to$ bessere Verwirbelung 
    - $\to$ bessere Verteilung des Kraftstoff-Luftgemisches
- Drosselklappe könnte wegfallen, wird aber weiterhin verbaut
- **Wozu ist die Drosselklappe dann noch notwendig?**
  - Schaltung des AGR (Abgasrückführung)
    - Aufbau eines Druckgefälles/Druckdifferenz, durch Schließen der Drosselklappe wird ein Unterdruck erzeugt, was dazu führt, dass die Abgase in den Ansaugtrakt einströmen können
- Notlauf

### Valvetronic

$\to$ Verändern von Ventilöffnungswinkel (Hub) und Ventilöffnungsdauer (Nockenwellenverstellung) 

**Wie?** 

- SG verdreht mithilfe eines **Stellmotors** eine **Exzenterwelle** (Halbmondförmig)
- Druck des Nockens wird zunächst auf einen **Zwischenhebel** übertragen
- Der **Leerweg**, den der Zwischenhebel von der Betätigung durch den Nocken bis zur Übertragung auf das Ventil durchläuft, ist mittels einer Exzenterwelle einstellbar.
- Je größer der Leerweg, desto kleiner der Ventilhub.
- **Ventilhub** 0,3 mm und 9,85 mm

### Elektrohydraulischer Ventiltrieb (MultiAir)

**Vorteil** Vollvariable Steuerzeiten

$\to$ stufenlose Veränderung von Ventilhub, Ventilöffnungsdauer und die Anzahl der Ventilhübe der EV

**Wie?** 

- auf der **Auslassnockenwelle** gibt es einen **Extranocken**, über Schlepphebel wird ein **Pumpenelement** betätigt 
  - $\to$ der erzeugt einen **Öldruck**, um die **Einlassseite** zu steuern, 
- **Magnetventil geschlossen** Druck wird auf den Kolben übertragen, Ventil öffnen
- **Magnetventil offen** Ventil schließen. Der Öldruck fließt in den Druckspeicher ab.
- *Vorteil **Druckspeicher**:* von der Nockenwelle unabhängiger Zeitpunkt, mit Öffnung eines Magnetventils (SG) ein Öldruck aus dem Druckspeicher nutzen, der das **Ventil öffnet/schließt**
- **elektrohydraulisch-pneumatisch** (Ventile unabhängig von NW betätigen, noch nicht in der Großserie)
- chinesische Hersteller Qoros und der schwedische Luxussportwagenhersteller Königsegg

### Elektromagnetischer Ventiltrieb (noch nicht zur Serienreife geschafft)

**Vorteile**

- Vollvariable Steuerzeiten
- Anzahl der geöffneten Ventile pro Zylinder frei wählbar
- Zylinderabschaltung (ohne Gaswechselverluste möglich)
- Wegfall von Nockenwellen (Gewichtseinsparung)

**Wie?**

- Unterstützung des Elektromagneten beim schnellen Öffnen und Schließen des Ventils. 
- Abbremsen des Ventils kurz vor den Endstellungen geöffnet und geschlossen 
- Ventile beim abgeschalteten oder defekten Systems in halbgeöffnete Stellung bringen, um Motorschäden durch Aufsetzen der Ventile zu verhindern.