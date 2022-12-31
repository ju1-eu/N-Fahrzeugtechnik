---
title: 'Diesel II'
author: 'Jan Unger'
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!--update 15-10-22 Diesel II -->
**1) Beschreiben Sie ausführlich den Einspritzvorgang beim Pumpe–Düse–System mit Magnetventil.**

**Befüllen** bei ablaufenden Einspritznocken wird der Pumpenkolben nach oben gezogen
und der Hochdruckraum wird mit Kraftstoff befüllt. Solange Magnetventil offen ist, fließt
der Kraftstoff durch den Hochdruckraum in den Rücklauf ab. (kühlende Wirkung)
Bei auflaufenden Nocken wird der Pumpenkolben nach unten gedrückt. Magnetventil ist geschlossen und verschließt Kraftstoff, Vor- und Rücklaufleitung. Es baut sich ein
Hochdruck auf.

**Voreinspritzung** (Beginn) bei etwa 180 bar ist der Druck größer als die Düsen-Federkraft.
Durch das Einspritzen des Kraftstoffs haben wir einen kurzen Druckabfall und die Düsennadel
schließt (Ende).
Der Ausweichkolben hat seine schräge Druckschulter freigegeben (große Fläche, große
Kraft), wodurch er nach unten gedrückt wird und spannt die Düsenfeder vor.
Magnetventil öffnet und der überschüssige Kraftstoff entweicht in die Vor- und Rücklaufleitung.

**Haupteinspritzung** der Druck steigt weiter und drückt bei etwa 300 bar die Düsennadel
nach oben (Ende). Durch den Druckabfall schließt die Düsennadel.

**2) Wie lässt sich beim Pumpe–Leitung–Düse–System eine Voreinspritzung realisieren?** (NFZ)

Durch Zweifeder-Düsenhalter (kleine Feder - Voreinspritzung, große Feder - Haupteinspritzung). Bei geringem Kraftstoffdruck öffnet die Düse nur teilweise.

**3) Welche Hauptvorteile bietet das Common–Rail–System gegenüber allen anderen gängigen Einspritzsystemen?**

- Einspritzmenge lässt sich über Zeit und Einspritzdruck variieren (je nach Betriebszustand)
- Kein Druckanstieg im Einspritzvorgang: (der Öffnungsdruck entspricht dem jeweiligen Einspritzdruck)
- beliebige Anzahl von Einspritzvorgängen (ruhigen Motorleerlauf viele Einspritzungen, für maximales Drehmoment bei Volllast nur eine)
- Einspritzung unabhängig von Kurbelwellen- und Nockenwellenposition (Kraftstoffdruck steht immer an)
- Anpassung an unterschiedliche Motoren

**4) Welche Regelungsarten des Common–Rail–Systems kennen Sie?**

1. **Einsteller-Regelung**
    - **Druckregelung hochdruckseitig** über ein **Druckregelventil** (DRV)
        - Hochdruckpumpe fördert die maximale Fördermenge unabhängig von Bedarf an Kraftstoff
        - Raildruck wird über ein **Druckregelventil** geregelt, nicht benötigter Kraftstoff fließt zurück in den Tank
        - **Vorteil**
            - schneller Druckaufbau möglich
            - bei Lastwechsel agil
        - **Nachteil:** Hochdruckpumpe ist, konstant maximal belastet, dadurch 
            - geringere Nutzleistung
            - erhöhter Kraftstoffverbrauch, Schadstoffausstoß, Verschleiß 
            - unnötige Erwärmung des Kraftstoffs 
    - **Druckregelung niederdruckseitig** (Mengenregelung) über eine **Zumesseinheit** (ZME)
        - **Zumesseinheit** regelt die Zuflussmenge zur Hochdruckpumpe
        - **Bedarfsregelung**, d.h. es gelangt nur so viel Kraftstoff zu Hochdruckpumpe wie für die Einspritzung benötigt wird 
        - **Druckbegrenzungsventil** verhindert zu hohen Raildruck bei Ausfall der Zumesseinheit
        - **Vorteil**
            - bedarfsgerechte Förderung
            - Reduzierte Leistungsaufnahme der Pumpe
        - **Nachteil:** 
            - hohe Trägheit
            - Drucksteigerung erfordert zunächst eine Erhöhung des Niederdrucks, dadurch erhöhte Förderleistung der Hochdruckpumpe

1. **Zweisteller-Regelung** (**Druckregelung nieder- und hochdruckseitig**)
    - Zusammenspiel von Zumesseinheit (ZME) und Druckregelventil (DRV) 
    - **Vorteile**
        - geringe Leistungsaufnahme der Hochdruckpumpe bei konstant hohen Drücken
        - hohe Agilität bei geringen Drücken
    - **Kaltstart / Motorstart und Warmlaufphase** (angesteuert: **DRV**) "Druckregelung hochdruckseitig geregelt"
        - Schneller Druckaufbau möglich. Bessere Kraftstoffvorwärmung. Verzicht auf Kraftstoffheizung möglich.
        - Kraftstoff soll sich erwärmen, um ihn damit fließ- und zündfähiger zu machen
    - **betriebswarmer Motor: Leerlauf / Teilllast / Schub** (angesteuert: **DRV und ZME**) "Zweisteller-Betrieb"
        - große Sprünge des Raildrucks sind wahrscheinlich (zwischen Motor im Leerlauf / Teillast und $\to$ Lastwunsch des Fahrers bei Volllast)
        - Raildruckregelung bei reduzierter Leistungsaufnahme der Pumpe
    - **hohen Motorlast** (angesteuert: **ZME**) "Druckregelung niederdruckseitig geregelt"
        - große Steigerungen des Raildrucks nicht möglich und deshalb ist die Trägheit vernachlässigbar
        - Reduzierter Leistungsaufnahme der Pumpe. Gesamte Kraftstoffmenge der Pumpe wird eingespritzt.

**5) Was passiert, wenn das Druckregelventil eines Common–Rail–Systems ausfällt?**

Da das Druckregelventil im spannungsfreien Zustand nur ca. 100 bar halten kann, der CR-Motor aber, um anzuspringen, 250 bar benötigt, läuft der Motor bei Ausfall des Druckregelventils nicht.

**6) Warum wird der Druck in der Rail bei kaltem Motor ausschließlich über das Druckregelventil geregelt?**

Um den Kraftstoff schneller zu erwärmen, um ihn damit fließ- und zündfähiger zu machen.


**7) Welche Spannung ist zum Öffnen eines Magnetspuleninjektors notwendig? Wie wird diese erzeugt?**

Um den Magnetventilspuleninjektor zu öffnen, wird eine Spannung von ca. 100 V bei einer Stromstärke von 20 A benötigt. Diese entsteht als Selbstinduktionsspannung im Abschaltmoment des Injektors und wird im Steuergerät in sogenannten Boosterkondensatoren gespeichert. Sind die Boosterkondensatoren entladen, kann das Steuergerät die Entstehung einer Selbstinduktionsspannung provozieren, in dem es die Injektoren mehrfach mit Bordnetzspannung an taktet, wodurch diese zwar nicht öffnen, jedoch die erforderliche Selbstinduktionsspannung entstehen kann.

**8) Welche Vorteile bietet der Piezoinjektor gegenüber dem Magnetspuleninjektor? Erläutern Sie den technischen Hintergrund.**

Während die Anzahl der Einspritzvorgänge pro Arbeitstakt beim Magnetspuleninjektor auf maximal fünf begrenzt ist, da es bei jeden Magnetfeldaufbau in ihm zu einer Gegeninduktion kommt, die den Magnetfeldaufbau hemmt und den einzelnen Einspritzvorgang damit verlangsamt, kann der Piezoinjektor problemlos sieben und mehr Einspritzvorgänge pro Arbeitstakt realisieren.

**9) Beschreiben Sie den Aufbau einer elektronisch geregelten Glühstiftkerze. Wie schafft man es, dass diese Glühkerze deutlich schneller auf Glühtemperatur ist, als die herkömmliche Glühkerze?**

Die elektronisch geregelte Glühstiftkerze besteht wie auch die herkömmlich Selbstregelnde Glühkerze aus einer Heiz- und einer verkürzten Regelwendel. Sie besitzt allerdings nur eine Nennspannung von 5 -- 8 V, um die Glühkerze besonders schnell auf Glühtemperatur zu bekommen, wird sie durch ein PWM-Signal kurzzeitig mit ca. 11 V angesteuert, also eigentlich überlastet. Hierdurch erreicht sie binnen 1 -- 2 Sekunden eine Glühtemperatur von bis zu $1000^\circ\text{C}$ bevor das Tastverhältnis, das PWM-Signal so weit verändert, dass an der Glühkerze nur ihre Nennspannung anliegt. Die ausreichend ist, um sie auf Temperatur zu halten.

**10) Welche Möglichkeiten der Motor- und Innenraum-Zuheizung kennen Sie. Nennen Sie Vor- und Nachteile der einzelnen Systeme.**

| **System**                | **Innenraum** | **Innenraum + Motor** | **Energie** | **Kühlen** |
|---------------------------|:-------------:|:---------------------:|:-----------:|:----------:|
| Kraftstoff-Zuheizer       |               |      \checkmark       | \checkmark  |            |
| PTC-Heizung               |  \checkmark   |                       | \checkmark  |            |
| Elektrisches Zuheizsystem |               |      \checkmark       | \checkmark  |            |
| Abgas-Wärmetauscher       |  \checkmark   |                       |             |            |
| Wassergekühlter Generator |               |      \checkmark       |             | \checkmark |
| Kraftstoff-Wärmetauscher  |               |      \checkmark       |             | \checkmark |

**Motorzuheizung** nach Motorstart wird beheizt.

(**Standheizung** ca. 10 Minuten vorheizen, bei Motorstart schon warm.)