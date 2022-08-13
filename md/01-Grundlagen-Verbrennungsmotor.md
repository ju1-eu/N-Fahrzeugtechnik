---
title: 'Grundlagen-Verbrennungsmotor'
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
Thema:  Grundlagen-Verbrennungsmotor
Fachbuch ([@brand:2020:fachkundeKfz] S. 243)
Fachbuch ([@respondeck:2019:servicetechniker] S. 142)
Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 281)
FS ([@bell:2020:formelsammlung] S. 32 - 37)
#
## 
ju 25-5-22
+----------------------------------------------------->

# Motorbauformen

- Reihenmotor, V-Motor, VR-Motor, Boxermotor
- Hubkolbenmotor, Kreiskolbenmotor

# Hubraum - Brennraum - Verdichtungsraum

$\text{Hubraum} \, V_h = \frac{\pi \cdot d^2}{4} \cdot s \,[cm^3]$

$\text{Gesamthubraum} \, V_H = V_h \cdot z$

$\text{Brennraum} = V_h + V_c$

$\text{Verdichtungsraum} \, V_c = \frac{V_h}{\epsilon - 1}$

$\text{Verdichtungsverhältnis} \, \epsilon = \frac{V_h + V_c}{V_c}$

# Arbeitsweise

(1) Vier-Takt-Arbeitsverfahren (1 Arbeitsspiel = 2 Kurbelwellenumdrehungen = 4 Kolbenhübe)
(2) Zwei-Takt-Arbeitsverfahren (1 Arbeitsspiel = 1 Kurbelwellenumdrehung = 2 Kolbenhübe)

# Ansaugen

- Abwärtsgehen des Kolbens
- Volumenvergrößerung, Druckdifferenz (Zylinderdruck versus höhere Außendruck)
- Einströmen der Luft (Ansaugen der Luft)
- zündfähiges Kraftstoff-Luft-Gemisch innen/außen bilden (Zylinder, Ansaugrohr)
- Kraftstoff (Kohlenstoff – Wasserstoff - Verbindung)

## Luftdruck

Luftdruck in Abhängigkeit der geodätischen Höhe

Luftdruck bezogen auf Meereshöhe $(1013~hPa = 1013~mbar, ca.\,1~bar)$ 

Erdanziehung ist von der Masse abhängig

Das Gewicht der Umgebungsluft drückt auf die Erdoberfläche und erzeugt einen Druck, Atmosphärendruck.


## Absolutdruck

Druck gegenüber Null (Vakuum, luftleeren Raum)

## Relativer Druck

Druck messen gegenüber Absolutdruck

## Zusammensetzung der Luft (Prüfung)

- $78~\%$ Stickstoff
- $21~\%$ Sauerstoff
- $0,9~\%$ Edelgase
- $0,1~\%$ Partikel, Feinstaub (Zell Gängigkeit, Blutkreislauf, Erbgutveränderung > Mutation)
- $0,040~\% ~ CO_2$ 



# Verdichten

- Aufwärtsgehen des Kolbens
- Kraftstoff-Luft-Gemisch wird verdichtet

## Hoch verdichtete Motoren

$10:1$

## Verdichtungsverhältnis

- **Mazda Motor:** $14:1$
- **Turbo Motor:** $7 - 8:1$
- **Direkt:** $17 - 18:1$ 
- **Indirekt** (Wirbel, Vorkammer): $21 - 36:1$
    - Vorkammer > Kugel > Wärmeabgabe > höher Verdichten

## Wärme

entsteht durch Reibung, Form von Energie, Bewegungsenergie kleiner Teilchen

## Wärmeabführung

an der Oberfläche, Luft (Isolator)

## Verdichten z. B. 10:1

$10~l$ großes Volumen wird auf den zehnten Teil verkleinert, also $1~l$

maximales Volumen zu minimales Volumen

Vgl. "*Kapitel Rechenbeispiele / Motor - Hubraum - Verdichtung*"

## Verdichtungsendtemperatur

$600 - 900^\circ\text{C}$ (Diesel: Zündung wird eingeleitet)

## Entzündungstemperatur Diesel

$230 - 250^\circ\text{C}$

## Zündverzug

$Entflammungsphase: \frac{1}{1000} s$

Ziel: Vollständige Verbrennung (feine Zerstäubung und hohe Temperaturen, das muss schnell gehen)

(1) **Benzin** Beginn Zündfunken bis zur Verbrennung 
(2) **Diesel** Beginn des Einspritzens bis zur Verbrennung

## Thermodynamischer Kreisprozess (keine Prüfung)

Wärmekraftmaschine: Verhältnis von Druck, Volumen und Temperatur beim Verdichten

Verhindert man die Ausdehnung, z. B. beim Verdichten, so verdoppelt sich der Druck.

Pro Grad der Erwärmung steigt der Druck um 273sten Teil seines Volumens im geschlossenen System

Erwärmt man das Gas um $273~K$, so dehnt es sich auf das doppelte Volumen aus.
Die Temperatur steigt und damit der Druck.

Grundlage: **1. Satz der Thermodynamik** "Die Energie bleibt in einem geschlossenen System konstant."

**Faktor 2** $\Rightarrow \frac{546}{273}$

Ziel: von $20^\circ\text{C} \Rightarrow 600^\circ\text{C}$ Verdichtungsendtemperatur

z. B. Verdichtung: $(10:1)$ 
$1~bar \Rightarrow 20~bar$ Verdichtungsenddruck $(10~bar \cdot 2 = 20~bar)$ 

Vgl. "*Kapitel Rechenbeispiele / Druck - Volumen - Temperatur*"

**Diesel** Gleichdruckverbrennung
**Benzin** Gleichraumverbrennung
**Anwendung** Zylinderabschaltung, Studium

## Grad Celsius

als Fixpunkte werden die Temperaturen vom Gefrier- $(0^\circ\text{C})$ und Siedepunkt $(100^\circ\text{C})$ des Wassers verwendet

## Aggregatzustand

physikalischer Zustand eines Stoffs. Beispiel:  fest, flüssig, gasförmig, plasma

## Kelvin

absoluten Nullpunkt der Teilchen $(0K = -273^\circ\text{C})$

$0~K = -273,15^\circ\text{C}$

$273,15~K = 0^\circ\text{C}$

$373,15~K = 100^\circ\text{C}$

**Umrechnung** 

$Kelvin = T_{Grad~Celsius} + 273,15$

$Grad~Celsius = T_{Kelvin} - 273,15$

# Arbeiten

- Verbrennung wird durch den Zündfunken eingeleitet
- Die Expansion der Gase treibt den Kolben nach UT
- Wärmeenergie wird in mechanische Energie umgewandelt

## Verbrennungstemperatur

$2000 - 2500^\circ\text{C}$

## Kolbenmaterial

Aluminium-Silizium-Legierung

## Thermische Belastung Kolben

**Problem** Kolbenbodentemperaturen

(1) $390^\circ\text{C}$ Diesel 
(2) $290^\circ\text{C}$ Benziner 
(3) $421^\circ\text{C}$ Stahlkolben

**Kerbe** = Sollbruchstelle

## Kolbenfläche berechnen

$A = \frac{\pi \cdot d^2}{4} = [mm^2]$

Vgl. "*Kapitel Rechenbeispiele / Druckberechnung am Pleuellager*"

## Kolbenwärme abführen

- Kolbenboden
- $80~\%$ über 1. Kolbenring, Kompressionsring, Minutenring, (trapezförmig)
- Zylinderwand

## Kolbenkippen Ursache

- Druckverlagerung 
- Desachsierung des Kolbens
- Wann liegt der Kolbendruck an?
- Wann Übergehen der Kolbengleitbahnen (deshalb die Desachsierung des Kolbens)
- Welche Kolbenbauform?
- ausreichend langes Kolbenhemd $\to$ Problem mehr Masse
- Masse einmal beschleunigt, wenn Kolben nach unten (möchte durch die Ölwanne in den Boden) oder Kolben nach oben (durch die Motorhaube in den Himmel) davon hält das Pleuel ab


# Ausstoßen

- Abgase verlassen mit Überschallgeschwindigkeit den Zylinder

## Abgastemperatur

$600 - 900^\circ\text{C}$

## Wirkungsgrad (Effizienz)

1. Dieselmotoren ca. $46~\%$ und 
1. Ottomotoren ca. $35~\% \to$ werden in **Bewegungsenergie** als Antriebsenergie für Motor verwendet

Rest in **Reibung und Wärme**

## Wie bewegt sich die Kurbelwelle?

**Ungleichförmige Drehbewegung**

Hubkolbenbewegung Reihenmotor (abhängig Zylinderanzahl, Zündreihenfolge)

Kompensieren: Kurbelwellenrad exzentrisch ausgeführt (unterschiedliche Hebellängen)

Beschleunigt (Zündungstakt)

- alle zwei NW Umdrehungen
- alle vier KW Umdrehungen

## Hydrodynamischer Schmierkeil

- durch ungleichförmige Drehbewegung 
- wird eine Volumenvergrößerung zwischen Kurbelwelle und Lagerung erreicht
- dadurch ein Einströmen des Lageröls in die Lagerstelle begünstigt
- Und wenn jetzt der Verbrennungsdruck durch die Verbrennung erzeugt auf die Kurbelwellenlagerstelle schneller erfolgt, als die Verdrängung des Öls aus der Lagerstelle heraus
- Aufschwimmen auf unserem Lager 
- Wir bewegen uns auf dem hydrodynamischen Schmierkeil
- Ist in der Lage hohe Drücke  auszuhalten

Wie kann es sein, dass ich mit einem Versorgungsdruck von $5~bar$ einen Öldruck in den Lagern der Kurbelwelle einen Spitzendruck bis $1000~bar$ kompensieren kann > Hydrodynamischer Schmierkeil

Vgl. "*Kapitel Rechenbeispiele / Druckberechnung am Pleuellager*"


# Kurbelgehäusearten

1. Closed-Deck-Ausführung 
    - Dichtfläche bis auf Kühl- oder Ölkanäle geschlossen gegenüber Zylinderkopf
    - Niederdruckguss-Verfahren (AlSi-Legierung)
1. Open-Deck-Ausführung
    - Wassermantel um die Zylinderbohrungen offen gegenüber Zylinderkopf (geringe Steifigkeit, erfordert Metall-Zylinderkopfdichtung)
    - Druckgussverfahren


# Zylinderkopfdichtung

Gasabdichtung bei allen Betriebszuständen

1. Metall-Weichstoff-Zylinderkopfdichtung 
1. Metall-Zylinderkopfdichtung 