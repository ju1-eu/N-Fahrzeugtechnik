---
title: 'Bremsen I'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!--
![Bremsen, Quelle: Europa-Verlag](images/Bremsen/Bremsen-1.pdf){width=70%} 
ju 17-12-22  Bremsen I-->

# Bremsanlagen

**Aufgabe einer Betriebsbremsanlage (BBA)**

1. Fahrzeug im Stillstand halten
1. Fahrzeuggeschwindigkeit verringern
1. Fahrzeug anhalten
1. Fahrzeuggeschwindigkeit im Gefälle halten

**Aufgabe einer Hilfsbremsanlage (HBA)**

1. Bei Ausfall der Betriebsbremsanlage deren Aufgabe ggf. mit verminderter Wirkung übernehmen.

**Aufgabe einer Feststellbremsanlage (FBA)**

1. Fahrzeug gegen wegrollen sichern

**Aufgabe einer Dauerbremsanlage (DBA, Retarter)**

1. Fahrzeuggeschwindigkeit im Gefälle halten und verringern

# Bremsvorgang

doppelte Geschwindigkeit $\to$ 4-facher Bremsweg

Bremsweg $\boxed{s = \frac{v \cdot t}{2}} \quad \boxed{1~m/s = 3,6~km/h}$

$s_{40~km/h} = \frac{11~m/s \cdot 2,73~s}{2} = 15~m$

$s_{80~km/h} = \frac{22~m/s \cdot 5,5~s}{2} = 60~m$



Doppelte Masse $\to$ doppelte Bremsarbeit

Bremsarbeit $\boxed{W_B = \frac{m \cdot v^2_\text{konst}}{2000}} \text{ in kJ}$

$W_{B_{1000~kg}} = \frac{1000~kg \cdot \sim 22^2~m/s^2}{2000} = 242~kJ$

$W_{B_{2000~kg}} = \frac{2000~kg \cdot \sim 22^2~m/s^2}{2000} = 484~kJ$

\newpage
**Nenne Einflussgrößen für den Bremsweg**

1. Fahrgeschwindigkeit (Faktor 2, doppelte Geschwindigkeit $\to$ 4-facher Bremsweg)
1. Fahrzeugmasse (Doppelte Masse $\to$ doppelte Bremsarbeit)
1. Fahrbahnzustand (trocken, nass, verreist)
1. Reifenzustand (Alter, Fülldruck, Profiltiefe)
1. Zustand der Bremse (schwergängig, Belag verglast)
1. Zustand der Stoßdämpfer
1. Bremskraftregelung (ABS)

**Beispiel Bremskraftleistung eines Lkw**

$\boxed{t = \frac{2 \cdot s}{v_\text{konst}}} \quad \boxed{1~m/s = 3,6~km/h}$

$t_\text{Beschleunigung} = \frac{2 \cdot 660~m}{\sim 22~m/s} = 60~s$

$t_\text{Bremsen} = \frac{2 \cdot 60~m}{\sim 22~m/s} = 5,5~s$

- Beschleunigung 660 m in **60 s** auf 80 km/h (ca. 22 m/s)
- Negative Beschleunigung (Bremsen) 60 m in **5,5 s** bis zum Stillstand

\newpage
# Hydraulische Bremse

**Pascalsche Gesetz** der auf eine eingeschlossene Flüssigkeit ausgeübte Druck überträgt sich in dieser nach allen Richtungen gleichmäßig.

Die hebelübersetze Pedalkraft wird im Bremskraftverstärker um den Faktor 4 -- 10 verstärkt und wirkt auf die Kolben im Hauptbremszylinder. Die Bestätigungskraft wird in einen hydraulischen Druck umgewandelt. Diese liegt bei Vollbremsung im Bereich zwischen 100 -- 160 bar.


**Zusammenhang Druck, Fläche, Kraft und Weg**

$\boxed{A = \frac{\pi \cdot d^2}{4}} \quad \boxed{F = p_\text{konst} \cdot A} \quad \boxed{W = F \cdot s} \quad \boxed{i = \frac{s_2}{s_1}} \quad \boxed{1~bar = 10~N/cm^2}$

- **geg:** 
    - $d_1 = 50~mm = 5~cm, d_2 = 71,36~mm = 7,136~cm, p = 10~bar = 100~N/cm^2$
- kleine Fläche und kleine Kraft $A_1 = \frac{\pi \cdot 5^2}{4} = 20~cm^2 \quad F_1 = \sim 10~bar \cdot 20~cm^2 = 200~N$
- große Fläche und große Kraft $A_2 = \frac{\pi \cdot 7,136^2}{4} = 40~cm^2 \quad F_2 = \sim 10~bar \cdot 40~cm^2 = 400~N$

![hydraulischen Bremse, Quelle: Europa-Verlag](images/Bremsen/Bremsen-1.pdf){width=50%}


- **geg:** 
    - $p_\text{max} = 180~bar = 1800~N/cm^2, F_\text{Hauptbremszylinder} = 1000~N, F_\text{4x Radzylinder} = 4000~N$, $s_\text{Hauptbremszylinder} = 8~mm, s_\text{4x Radzylinder} = 2~mm$
- kleine Kolbenfläche $A_\text{Hauptbremszylinder} = \frac{1000~N}{1800~N/cm^2} = 0,55~cm^2$
- große Kolbenfläche $A_\text{4x Radzylinder} = \frac{4000~N}{1800~N/cm^2} = 2,22~cm^2$
- übersetzung: 4x Kolbenweg am Hauptbremszylinder $i = \frac{2~mm}{8~mm} = 0,25 = 1:4$
- gleiche Arbeit $W_\text{Hauptbremszylinder} = 1000~N \cdot 0,008~m = 8~Nm$
- gleiche Arbeit $W_\text{4x Radzylinder} = 4000~N \cdot 0,002~m = 8~Nm$

**Nenne Vorteile einer hydraulischen Bremsanlage**

1. Drücke bis 180 bar
1. Geringe Flüssigkeitsmengen durch kleine Abmessungen der hydraulischen Bremsanlage
1. Kleines Lüftspiel
1. wartungsarm

\newpage
# Bremskraftaufteilung

**Welche Aufteilung von Bremskreisen gibt es?**

![Bremskreisaufteilungen, Quelle: Europa-Verlag](images/Bremsen/Bremsen-2.pdf){width=50%} 

1. II / TT (Schwarz-weiß) Bremskreis 1 (VA) und Bremskreis 2 (HA)
    - Bremskraftverteilung VA : HA (70 \% : 30 \%)
1. X (Diagonal) Bremskreis 1 (VA links + HA rechts) und Bremskreis 2 (VA rechts + HA links)
    - Bremskraftverteilung Kreis 1 : Kreis 2 (50 \% : 50 \%)
1. LL (Dreieck) Bremskreis 1 (VA + HA rechts) und Bremskreis 2 (VA + HA links)
    - Bremskraftverteilung Kreis 1 : Kreis 2 (50 \% : 50 \%)

**Warum gibt es eine Bremskreisaufteilung?**

Sicheres Abbremsen des Fahrzeugs gewährleisten, bei Ausfall eines Bremskreises.

\newpage
# Hauptbremszylinder

![Tandem-Hauptbremszylinder, Quelle: Europa-Verlag](images/Bremsen/Bremsen-3.pdf){width=50%} 

**Welche Aufgabe hat der Tandem-Hauptbremszylinder**

1. Umwandeln der Bremskraft in Bremsdruck in der Bremsanlage
1. schneller Druckaufbau ermöglichen
1. schneller Druckabbau zum Lösen der Bremse
1. Absicherung der Bremskreise 1 und 2
1. schnelles überwinden der Lüftspiele (Anlegen der Beläge an die Scheibe)



**Primärmanschette**
Die Primärmanschette dichtet den Druckraum beim Bremsvorgang ab, wird beim
Schnelllösevorgang als Ventil wirksam und ermöglicht so das "Nachsaugen".

**Füllscheibe/Ringscheibe** (Stahl oder Messing)
Die Füllscheibe schützt die Primärmanschette vor Beschädigungen durch die Füllbohrungen des Kolbens beim Bremsvorgang und wird beim Lösevorgang als Ventil wirksam.

**Sekundärmanschette/Ringmanschette**
Diese Manschette dichtet den Ringraum ab. Sie verhindert den Austritt von Flüssigkeit
und im Normalfall auch den Eintritt von Luft

**Ausgleichsbohrung** ($\varnothing 0,7~mm$)
Das Flüssigkeitsvolumen im Druckraum bei Temperaturschwankungen
und beim Lösevorgang auszugleichen.

**Nachfüllbohrung** ($\varnothing 3 - 5~mm$)
Den Ringraum beim Lösevorgang auffüllen und einen Lufteintritt in das Bremssystem verhindern.

**Zentralventil** 
verhindert eine Beschädigung der Primärmanschette des Zwischenkolbenkreises,
sobald der dort angeschlossene Hinterachskreis Blockierneigung aufweist
und das ABS dort den hydraulischen Druck pulsierend regelt.

**Hochdruckprüfung** 50 -- 100 bar, Prüfdauer 10 Min. (darf max. 10 \% abfallen)

- Undichtigkeit im Bremssystem prüfen

**Niederdruckprüfung** 2 -- 5 bar, Prüfdauer 5 Min. (darf nicht abfallen)

- Hauptbremszylinder überprüfen
    - Undichtigkeit am Zentralventil oder an der Primär- oder Trennmanschette eines Kolbens


\newpage
# Trommelbremse

**Nenne Eigenschaften einer Trommelbremse**

1. Selbstverstärkung (Nachteil: keine Dosierbarkeit der Bremskraft)
1. Schmutz geschützter Aufbau
1. Geringer Bremsbelagverschleiß
1. schlechte Wärmeabfuhr
1. Neigung zum Fading
1. FBA ist einfacher zu integrieren

**Selbstverstärkung**, die auflaufende Bremsbacke zieht in die Trommel hinein und verstärkt die Bremswirkung.

**Bremsfading** Nachlassen der Bremswirkung durch Temperatureinfluss / Überhitzung. (Bemerkung: Gaspolster entstehen.  Reibzahl des Belags nimmt bei hoher Temperatur ab.)

**Bremsenkennwert C - Selbstverstärkung** ist abhängig von der Bauart der Bremse

**Bauarten einer Trommelbremse**

![Bauarten von Trommelbremsen, Quelle: Europa-Verlag](images/Bremsen/Bremsen-4.pdf){width=50%} 

1. **Duo-Servo-Bremse**
    - Die untere Abstützung der Bremsbacken nach beiden Seiten beweglich.
    - Es laufen beide Backen bei Vorwärts und Rückwärtsfahrt selbstverstärkend auf.
1. **Simplex-Bremse**
    - Ein Radzylinder mit seinen zwei Kolben betätigt die Bremsbacken. 
    - Die Abstützung der Backen erfolgt unten am festen Stützlager. 
    - Es gibt bei einer Bremsung in beiden Fahrtrichtungen immer eine auflaufende und eine ablaufende Bremsbacke.
1. **Duplex-Bremsen**
    - Es gibt zwei einseitig wirkende Radzylinder, je Bremsbacke einer.
    - Bei Vorwärtsfahrt wirken beide Bremsbacken auflaufend, also beide selbstverstärkend.
    - Bei Rückwärtsfahrt wirken beide Bremsbacken ablaufend, somit ergibt sich dann nur eine relativ geringe Bremswirkung.

**Radbremszylinder** hydraulische Druck wirkt auf einen Kolben und erzeugt die Spannkraft. Abdichtung durch Nutringmanschette.

\newpage
# Scheibenbremse

**Nenne Eigenschaften einer Schreibenbremse**

1. Verbesserung der Wärmeabfuhr durch innenbelüftete Bremsscheiben
1. geringe Neigung zum Fading 
1. gute Dosierbarkeit der Bremskraft
1. höherer Belagverschleiß
1. Keine Selbstverstärkung
1. gute Kühlung
1. Wartung und Belagwechsel einfach
1. Selbsttätige Nachstellung des Lüftspiels
1. stärkere Erwärmung der Bremsflüssigkeit
1. Gefahr der Dampfblasenbildung

**Bauarten von Scheibenbremsen**

1. **Festsattel-Scheibenbremse** (mehrere Kolben)
1. **Faustsattel-Scheibenbremse** (ein Kolben)
    - Geringes Gewicht
    - Kleine Baugröße
    - Gute Wärmeableitung
    - Große Belagflächen
    - Geringer Platzbedarf
    - Geringe Neigung zur Dampfblasenbildung (Bremszylinder ist nur auf der Halterseite)
    - Wartungsfreie Gehäuseführung (unempfindlich gegen Schmutz)
1. **Schwimmsattel-Scheibenbremse**

**Wie erfolgt die Nachstellung bei Scheibenbremsen? (Kolbenrückstellung)**

- Nach Beendigung des Bremsvorganges und Abbau des Bremsdruckes werden die Bremskolben durch das Entspannen des Rechteckringes in ihre Ausgangslage gebracht. 
- **Lüftspiel** 0,15 mm. 
- Dieser Vorgang kann durch Spreizfedern unterstützt werden.

**Was kann ein Lenkradflattern beim Bremsen verursachen?**

- Radlagerspiel zu groß
- Bremsscheibenschlag zu groß

**Wozu dient eine gelochte oder geschlitzte Bremsscheibe?**

- bei nassen Scheiben schnelle Abfuhr des Wassers
- bessere Kühlung
- bessere Schmutz-, Wasser- und Wärmeabfuhr

**Bremsscheibe**

Die Größe der Bremsscheibe ist ausschlaggebend für das am Rad zur Verfügung stehende Bremsmoment (ergibt sich aus dem Hebelarm) sowie die Wärmeabfuhr und Lebensdauer der Scheibe.

Zur besseren Wärmeabfuhr ist sie heutzutage in der Regel innenbelüftet. Zur besseren Wasser und Schmutzbeseitigung kann sie zudem gelocht oder geschlitzt sein. 

**Material Kohlefaserverstärkte- oder Keramik-Carbon Bremsscheibe**

- ca. 70 \% leichter
- Hitzebeständigkeit bis zu $1600^\circ\text{C}$ (Vgl. Stahlscheibe $800^\circ\text{C}$ Kirschrot)
- nahezu konstanter Reibwert bei Erreichen der Betriebstemperatur
- geringer Verschleiß
- kostenintensiv

**Was bringt es, wenn eine Bremse leichter ist?**

- Weniger **ungefederte Massen** (alles unterhalb des Stoßdämpfer -befestigungspunktes)
- geringere Massenträgheit

**Nenne fünf Anforderungen von Bremsbelägen**

1. Hitzebeständigkeit
1. hohe Standzeit
1. Wasser und Schmutz unempfindlich
1. gleichbleibende hohe Reibungszahl ($\mu$)
1. hohe mechanische Festigkeit
1. Kein **Verglasen** (schlechtere Reibungszahl, Scheibe bekommt Riefen)

**Bremsbelag**

- Asbest wurde in Deutschland 1993 verboten und bis 42 \% in Bremsbelag enthalten
- mit Prüfzeichen ($E_1$, ECE Genehmigungsnummer) diese belegen, dass der Bremsbelag geprüft wurde
    - gleicher Reibwert wie Original-Beläge des Herstellers
    - Abweichung bis $\pm15 \%$ sind erlaubt
    - Druck- und Scherfestigkeit
    - Asbestfreiheit

Eine Prüfnummer mit (E) beginnend, muss am Ersatzteil dauerhaft identifizierbar vorhanden sein. Die Verpackung der Beläge muss verklebt oder versiegelt sein, um vorheriges Öffnen klar zu erkennen. Auf der Verpackung müssen die für den Belag zugelassenen Fahrzeuge gelistet sein.

**Arten von Bremskraftverstärkern** (Hilfskraft, Fußkraft des Fahrers unterstützen)

1. Unterdruck-Bremskraftverstärker
    - Die geringe **Druckdifferenz** zwischen Luftdruck 1 bar und Saugrohrdruck von etwa 0,2 Bar erfordert große Flächen des Arbeitskolbens, um die Druckstangenkraft um den Faktor 4 -- 10 zu verstärken.
    - **Unterdruckerzeugung**
        - *Dieselmotor:* vom Motor angetriebene Vakuumpumpe
        - *Saug-Ottomotor:* wird dem Ansaugrohr entnommen
        - *Hybridfahrzeug:* Elektrische Vakuumpumpe

1. Tandem-Bremskraftverstärker
1. Pneumatischer Bremskraftverstärker
1. Hydraulischer Bremskraftverstärker
1. Elektro-mechanischer Bremskraftverstärker (eBKV, Unterdruck ist nicht erforderlich)
    - Tandem-Hauptbremszylinder mit Vorratsbehälter
    - Elektromotor mit Getriebe und Verstärkungselement
    - Steuergerät
    - Differenzwegsensor

**Blended Braking** Überlagerung von elektrischem Bremsen (Rekuperation des Drehstrommotors) + hydraulischem Bremsen = gewünschte Verzögerung des Fahrers

**Bremsassistent (BAS)** ab einer bestimmten Pedalweggeschwindigkeit (Membranwegsensor dient zur Berechnung) wird von einer Notbremsung ausgegangen, und die Bremsassistentfunktion wird ausgelöst. Dafür wird im Bremskraftverstärker ein Magnetventil (BAS) geschaltet, das die Arbeitskammer belüftet und so die maximale Bremskraftunterstützung gewährleistet. Der Fahrer betätigt das Bremspedal in einer Gefahrensituation zwar schnell genug, jedoch nicht stark genug.

**Feststellbremse**

1. Mechanisch über Bremsseile
1. Elektro-mechanische Feststellbremse (Parkbremse, EPB)
1. Elektro-mechanischer Aktor

**Was ist aktive und passive Sicherheit? Nenne jeweils 5x Beispiele.**

**Aktive Sicherheit** Maßnahmen zur Vermeidung von Unfällen

1. ABS
1. ESP
1. Klima
1. Scheibenwischer
1. ACC (adaptive Geschwindigkeitsregelung)
1. Beleuchtungseinrichtung
1. Todwinkelassistent

*Klima*: die Raumtemperatur wird runtergekühlt, Aufmerksamkeit steigt und der Pollenfilter bewirkt eine geringere Last für Allergiker.

**Passive Sicherheit** Maßnahmen zur Minderung von Unfallfolgen

1. Fahrerairbag
1. Beifahrerairbag
1. Kopfairbag
1. Seitenairbag
1. Gurtstraffer 
1. Batterietrennschalter (Kurzschluss, Brandgefahr)
1. Motorhaubenaufsteller
1. Nackenstütze

**Nenne Vorteile und Nachteile einer Scheibenbremse gegenüber einer Trommelbremse**

**Vorteile**

1. automatische Nachstellung
1. keine Vergrößerung des Bremspedalweges bei erwärmter Bremse
1. gleiche Bremswirkung in beiden Fahrrichtungen
1. gleiche Bremsbelagbelastung auf einer Achse

**Nachteile**

1. keine Selbstverstärkung
1. starke Erwärmung der Bremsscheiben

**Welche Siedeanforderung hat DOT4?**

- $\geq 230^\circ\text{C}$ 
- durch die Wasseraufnahme sinkt der Siedepunkt




