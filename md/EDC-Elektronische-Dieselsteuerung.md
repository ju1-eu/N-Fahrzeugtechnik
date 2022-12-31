---
title: 'EDC'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!------------------------------------------------------------------------+
![ . (Bild: Kai Borgeest)](images/EDC/EDC-1.pdf){width=70%} 
(Bild: Kai Borgeest)
(Foto: Robert Bosch GmbH)
Quelle: S. 57 [@borgeest:2021:elektronik].
ju 18-12-22 Elektronische-Dieselsteuerung (EDC)
+-------------------------------------------------------------------------->



# Aufgaben der Motorsteuerung

1. Einspritzung des Kraftstoffes in die Zylinder
1. Regelung und Begrenzung von Drehzahl und Geschwindigkeit,
1. Regelung des Luftsystems (Abgasrückführung und Ladedruckregelung),
1. Abgasnachbehandlung,
1. Glühkerzensteuerung und Thermomanagement,
1. Zylinderabschaltung,
1. Diagnose,
1. Wegfahrsperre.

\newpage
# Einspritzung

Quelle: S. 57 [@borgeest:2021:elektronik].

![Einspritzfunktion eines Dieselsteuergerätes ($\varphi$: Kurbelwellenwinkel). (Bild: Kai Borgeest)](images/EDC/EDC-1.pdf){width=70%} 

- SG optimalen Zeitpunkt für den Beginn der Einspritzung berechnet und die "richtige" Menge für die Einspritzung kennt.
    - Einspritzmenge
    - Zeitpunkt / Spritzbeginn
- Ansteuern der Einspritzventile für jeden Zylinder
- Fahrpedal (Fahrerwunsch)
- Winkeluhr im SG
    - aktuelle Stellung der Kurbelwelle und Drehzahl
    - zeitlich veränderliche Vorgänge im Motor nicht direkt als Funktion der Zeit, sondern als Funktion des Kurbelwellenwinkels (winkelsynchron) anzugeben und zu berechnen
    - In der Zeit $\Delta t$ bewegt sich bei der Drehzahl $n$ die Kurbelwelle um den Winkel 
    - $\Delta \varphi = 6 \cdot n \cdot \Delta t$ $\quad [^\circ \text{KW} = \text{min}^{-1} \cdot \text{s}]$
- Einspritzung bei 
    - $0^\circ$ bedeutet das der Kolben bei einem als Bezug gewählten Zylinder gerade am oberen Totpunkt steht.
    - $-10^\circ$ bedeuten, dass sich die Kurbelwelle noch um $10^\circ$ drehen muss, bis der Kolben im Bezugszylinder den OT erreicht hat. 
    - $+10^\circ$ bedeuten, dass der Kolben schon wieder auf dem Weg vom OT nach unten ist.

\newpage
![Signale vom Kurbelwellen- und Nockenwellensensor. (Bild: Kai Borgeest)](images/EDC/EDC-3.pdf){width=50%}


**Kurbelwellensensor**

- Impulsgeber, dessen Impulsfrequenz steigt mit der Drehzahl. Durch abzählen der Impulse lässt sich der Winkel bestimmen.

**Nockenwellensensor**

- OT-Verbrennung (Bezugsmarke/Referenzmarke) in $^\circ \text{KW}$

![Elektromagnetischer Sensor für die Drehzahl der Kurbelwelle. Die nur im Luftspalt eingezeichneten Magnetfeldlinien schließen sich über das Zahnrad, dessen Lagerung und über das Gehäuse, welches das Zahnrad umfasst und den Sensor aufnimmt. Durch Änderung des Feldes wird in der Spule die Spannung $U_{\text{ind}}$ induziert. (Bild: Kai Borgeest)](images/EDC/EDC-4.pdf){width=30%}

\newpage
**4-Zylinder Motor:** 

- $0^\circ (\text{Kolben im OT, Einspritzung Verbrennung}), 180^\circ (\text{UT})$
- und $360^\circ (\text{Kolben im OT, Ausstoßen}), 540^\circ (\text{UT})$
- zweideutigkeit (Kolben 2x im OT pro Arbeitsspiel)
- alle 4x-Takte: Ansaugen, Verdichten, Arbeiten/Verbrennen, Ausstoßen
- zwei Kurbelwellenumdrehungen ($720^\circ$), eine Nockenwellenumdrehung

![Darstellung der vier Takte eines Viertaktmotors von links nach rechts: a Beginn des Ansaugtaktes ($360-540^\circ$): Bei geöffneten Einlassventil saugt der sich abwärts bewegende Kolben Luft an. b Ende des Verdichtungstaktes ($540-720^\circ$): Beide Ventile sind geschlossen, durch die Aufwärtsbewegung des Kolbens wird die Luft komprimiert und dadurch erhitzt. c Beginn des Arbeitstaktes ($0-180^\circ$): Der Kraftstoff wird eingespritzt und verbrennt durch die hohe Lufttemperatur. Dadurch wird der Kolben nach unten gedrückt. d Ende des Ausstoßtaktes ($180-360^\circ$): Durch das nun geöffnete Auslassventil drückt der wieder steigende Kolben die Verbrennungsgase aus dem Zylinder heraus. (Bild: Kai Borgeest)](images/EDC/EDC-2.pdf){width=70%}

\newpage
## Berechnung der Einspritzmenge

**Fahrzustände** 

- Start, Leerlauf, Fahren
- **Schubbetrieb** bei Bergabfahrt mit einem niedrigen Gang; in diesem Falle bremst der Motor das bergab rollende Fahrzeug. 
- **Teillast und Volllast**
- **Notlauf**  Steuergerät erkennt einen kritischen Zustand  oder
- **Grenzzustände** (z. B. das Abregeln bei Erreichen von Drehzahl- oder Geschwindigkeitsgrenzen). 

Die **Einspritzmenge** berechnet sich über einen weiten Bereich näherungsweise proportional aus dem angeforderten Drehmoment (Fahrerwunsch), bzw. im Leerlauf von der Anforderung des Leerlaufreglers. 

Fahrerwunsch wird vom Gaspedal über einen Pedalwertgeber (PWG, Sensor der einen Winkel in eine Spannung umsetzt) elektrisch an das Steuergerät übertragen.

**weitere Parameter für das Drehmoment bzw. die Einspritzmenge** 

- aktuelle Drehzahl
- aktuelle Fahrgeschwindigkeit 
- Motorlast
- Temperatur des Motors (gemessen über die Kühlwassertemperatur, Öltemperatur), 
- Batteriespannung
- Informationen über das Getriebe
- Betriebszustand (z. B. Kaltstart) 
- Begrenzungen (z. B. Rauchbegrenzung)

**Mengenberechnung** 

1. **Mengenpfad** oder 
    - berechnet grob die erforderliche Einspritzmenge, passt diese dann durch etliche Korrekturrechnungen, Kennfelder, Begrenzungen und eventuelle externe Mengeneingriffe auf die exakt benötigte Menge an.
1. **Momentenpfad**
    - wird zuerst das vom Motor benötigte Drehmoment grob berechnet, sämtliche Berechnungen im Steuergerät werden mit Momenten statt mit Mengen durchgeführt und erst zum Schluss des Berechnungspfades wird die genaue Momentenanforderung in die exakte Einspritzmenge umgerechnet. 

Bei externen Eingriffen (Signale von anderen Steuergeräten) kann die Momentenstruktur als "gemeinsame Sprache" mehrerer Steuergeräte vorteilhaft sein, da Getriebesteuergeräte und Fahrdynamiksteuergeräte intern mit mechanischen Größen und nicht mit Kraftstoffmengen rechnen.


1. **Voreinspritzung** zur Geräuschminderung
    - PKW in der Größenordnung von $1 - 2~mm^3$
1. **Haupteinspritzung** Drehmoment
    - PKW in der Größenordnung von einiger $10~mm^3$
1. **Nacheinspritzung** zur Nachverbrennung von Partikeln im Zylinder oder zur Unterstützung der Abgasnachbehandlung. 
    - PKW in der Größenordnung von $1 - 2~mm^3$

Vgl. Wassertropfen ein Volumen von ca. $30~mm^3$

\newpage
## Berechnung des Spritzbeginns

1. **frühe Einspritzung** führt zu einer zu frühen Verbrennung. Dadurch wird bereits
eine Kraft von oben auf den Kolben ausgeübt, bevor er den OT erreicht. Dies führt zu
einem Verlust an Leistung, im Extremfall sogar zum Stillstand oder zur Beschädigung
des Motors. Weiterhin erreicht die Verbrennungstemperatur zu hohe Spitzenwerte, die zu
einer vermehrten Bildung von Stickoxiden im Abgas führen.

1. **späte Einspritzung** führt dazu, dass der eingespritzte Kraftstoff nicht mehr vollständig verbrennt. Dadurch geht ebenfalls Leistung verloren und es bildet sich schwarzer Rauch, der Partikel enthält. Bei noch späterer Einspritzung wird der Kraftstoff völlig unverbrannt ausgestoßen, das Abgas färbt sich bläulich und riecht nach Diesel. Im Extremfall, wenn unverbrannter Kraftstoff sich als Flüssigkeit in der Kolbenmulde ansammelt, kommt es zum Motorschaden.

Bereits bei einer Abweichung des Spritzbeginns um $1^\circ \text{KW}$ lassen sich die gültigen Abgasgrenzwerte nicht mehr einhalten.

Der **optimale Spritzbeginn** ist keine Konstante, sondern er hängt vom Motor und von
mehreren Betriebsparametern ab. (leistungsoptimierte, abgasoptimierte Spritzbeginn)

**Parameter** 

- Drehzahl und die Einspritzmenge
    - Sowohl mit steigender Drehzahl als auch mit zunehmender Menge wird der Spritzbeginn nach früh verschoben. 
- Temperatur des Motors
- Temperatur der Ansaugluft
- atmosphärische Druck.

Im Steuergerät wird der Zusammenhang zwischen den gemessenen Parametern und dem daraus ermittelten Spritzbeginn durch Formeln oder über Kennlinien und Kennfelder, also über
Wertetabellen dargestellt. Diese werden zunächst mit Erfahrungswerten gefüllt, dann erfolgt am Prüfstand eine experimentelle Optimierung.

\newpage
## Ansteuerung des Einspritzsystems

![Überblick über ein Common-Rail-Einspritzsystem. (Bild: Kai Borgeest)](images/EDC/EDC-5.pdf){width=50%}


**Common-Rail-System**

**Vorteil von Common Rail** ist, dass permanent Kraftstoff einspritzbereit unter einem hohen, über mehrere Einspritzungen konstant regelbaren Druck verfügbar ist.

**Nachteil von älteren Einspritzsystemen** (Reihenpumpen, Einzelpumpen, Verteilerpumpen, Pumpe-Düse, Pumpe-Leitung-Düse) Druck ist nur zu bestimmten Zeiten, in denen ein Nocken einen Pumpenkolben betätigt verfügbar. 


- **Rail** rohrförmiger Druckbehälter mit Kraftstoff

- Über kurze Leitungen ist je ein Injektor (Einspritzventil) pro Zylinder mit dem Rail verbunden. 

- Der Injektor kann vom Steuergerät (ECU) zu definierten Zeiten zur Einspritzung geöffnet werden. 
    - **Piezo-Injektoren** und **elektromagnetischen Injektoren**

- Die eingespritzte Menge hängt von der elektrischen Ansteuerdauer
(die ungefähr der Dauer entspricht, in der der Injektor geöffnet ist) und vom Druck im Rail ab. 

- Den Druck im Rail bis 2700 bar, bei LKW bis 3000 bar, erzeugt eine Kolbenpumpe.

- Aufgrund der Systemkosten, des Energieaufwandes und der Druckwellenproblematik in den Leitungen bei Drücken oberhalb 2000 bar arbeiten einige neue Systeme mit einem Raildruck unterhalb 1000 bar und erhöhen erst unmittelbar vor der Einspritzung, idealerweise erst im Injektor, den Druck über einen hydraulischen Übersetzerkolben auf den Einspritzdruck von z. B. 2500 bar.
    - APCRS (Amplifier Piston Common Rail System) oder druckverstärktes Common Rail. Ein Pilotsystem ist das seit 2011 in LKW-Motoren eingesetzte "X-Pulse" - System von Daimler.

\newpage
## Ansteuerung der Injektoren


![Ansteuerschaltung für Common-Rail-Injektoren mit Magnetventilen (Prinzip). (Bild: Kai Borgeest)](images/EDC/EDC-8.pdf){width=50%}

**Injektoren mit Magnetventil**

![Injektors mit Magnetventil (bei Bosch bis zur Generation 2.16), oben geöffnet, unten geschlossen. 1 Kraftstoff-Rücklauf, 2 elektrischer Anschluss, 3 Elektromagnet, 4 Kraftstoff-Zulauf, 5 Ventilkugel, 6 Ablaufdrossel, 7 Zulaufdrossel, 8 Steuerraum, 9 Druckkolben, 10 Kraftstoff, 11 Nadel. (Bild: Robert Bosch GmbH)](images/EDC/EDC-6.pdf){width=70%}

*Wirkungskette:* Injektor öffnen $\to$ Steuergerät $\to$ Bestromung des Elektromagneten $\to$ Anzug des Ankers $\to$ Anheben der Nadel $\to$ Einspritzung 

\newpage
![Zeitlicher Verlauf des Stromes durch einen Common-Rail-Injektor bei einer Voreinspritzung und einer Haupteinspritzung. 1 Skalenteilung entspricht vertikal einem Strom von 5 A, horizontal einer Dauer von 400 $\mu s$. (Bild: Kai Borgeest)](images/EDC/EDC-7.pdf){width=50%}

Das Problem liegt nun darin, möglichst schnell den vollen Strom zu erreichen, um den
Anker hochzureißen. Dies lässt sich wegen der Leitungsinduktivitäten nicht mit Hilfe der Fahrzeug-Batterie realisieren. Stattdessen wird ein hinreichend großer Kondensator, auch Booster-Kondensator genannt, im Steuergerät auf eine Spannung in der Größenordnung 70 -- 90 V aufgeladen, der die Energie für den Anzug liefert.

- Das erste Stromniveau von ca. 20 A ist der **Anzugsstrom**, der möglichst schnell den Anker heben soll. Eine sehr kurze Einspritzung wie die Voreinspritzung kann bereits während dieser Anzugsphase wieder enden. Nach einer Dauer von etwa einer halben Millisekunde kann davon ausgegangen werden, dass der Anker angezogen ist. 

- Von nun an genügt ein kleinerer Strom von z.B. 13 A, der **Haltestrom**, um den Anker in dieser Position zu halten.

- Der zackige Verlauf der Stromniveaus ist darauf zurückzuführen, dass der Strom durch Ein- und Ausschalten von Transistoren um den mittleren Wert geregelt wird.

**Piezo-Injektoren**

Deren Aktorelement besteht aus einer piezoelektrischen Keramik die sich bei Anlegen der Spannung um einige $10~\mu m$ dehnt. Über einen hydraulischen Übersetzter betätigt das Piezo-Element ein Servoventil, welches das Öffnen der Nadel ermöglicht. 

**Vorteil** gegenüber einem Magnetventil ist ein kürzerer Verzug zwischen der elektrischen Ansteuerung und dem Beginn der Einspritzung. 

Aus elektrischer Sicht verhält sich ein Piezo-Injektor nicht wie eine Spule, sondern wie ein Kondensator, der zum Einspritzen aufgeladen und zum Schließen wieder entladen wird. 


![Vergleich zwischen Magnetventil-Injektor (rechts) und Piezo-Injektor (Mitte). Links wird ein Detail einer Düsennadel gezeigt. (Foto: Robert Bosch GmbH)](images/EDC/EDC-9.pdf){width=50%}

\newpage
## Regelung des Raildrucks

**hoher Raildruck** ist wünschenswert, um eine feine Zerstäubung des Kraftstoffs im Brennraum zu erreichen.

**Leerlauf** würde man mit einem maximalen Einspritzdruck von fast 3000 bar arbeiten, wäre der Motor unzumutbar laut und es wäre auch schwierig, bei solchen hohen Drücken mit entsprechend kurzen Ansteuerdauern kleine Mengen noch präzise darzustellen.

Man wird also zuerst abhängig vom Fahrzustand einen geeigneten Druck auswählen und dann erst die Ansteuerdauer als Funktion der gewünschten Menge und des Raildrucks berechnen.

**Raildrucksensoren** piezoresistive Sensoren, bei denen Änderungen des Druckes in Änderungen des elektrischen Widerstandes umgesetzt werden. Sie enthalten eine Metallmembran, die durch den Druck durchgebogen wird. Auf dieser Membran sind vier Dehnungsmessstreifen so aufgedampft oder mit Leitpaste aufgedruckt, dass zwei Streifen mit zunehmender Biegung gestaucht, die anderen beiden gedehnt werden. Die vier Streifen sind zu einer Wheatstone-Brücke verschaltet, in deren Diagonalzweig eine zum Druck näherungsweise proportionale Spannung abgegriffen werden kann. Heutige Sensoren enthalten bereits eine Auswerteelektronik, welche die Brückenspannung auf die gewünschte Ausgangsspannung umrechnet und Temperatureinflüsse kompensiert.

\newpage
# Drehzahlregelung 

**Änderung der Drehzahl** ergibt sich aus der 

- Einspritzmenge, die wiederum vom Fahrerwunsch abhängt und 
- Last, die z. B. vom Fahrzeuggewicht und der Steigung abhängt. 

**Sonderfall Leerlauf** wenn der Motor durch das Auskuppeln oder weil kein Gang eingelegt ist, keinen Kraftschluss mit den Rädern hat und der Fahrer kein Gas gibt, erwarten wir vom Motor einen ruhigen gleichmäßigen Lauf ohne hörbare Drehzahlschwankungen.

**Leerlaufregler** benötigt zunächst eine Solldrehzahl. 

- **zu hohe Leerlaufdrehzahl** würde den Kraftstoffverbrauch, die Lautstärke und die Emissionen von Schadstoffen erhöhen. 

- **zu niedrige Deerlaufdrehzahl** würde zu einem trägen Anfahrverhalten führen und der Generator könnte nicht mehr die benötigte Bordnetzspannung erzeugen. 

- Ein typischer Wert liegt bei $750~min^{-1}$. 

\newpage
# Regelung des Luftsystems

**motorische Verbrennung** ist auf eine ausreichende Luftzufuhr angewiesen. Reicht die Luft nicht aus, verbrennt der Kraftstoff unvollständig. In Folge entstehen Schadstoffe und der Motor kann die geforderte Leistung nicht bringen. 

**Luftmangel erwünscht** der Verbrennungsprozess des Dieselmotors ist mit höheren Spitzentemperaturen (zwischen $1000^\circ \text{C}$ und $2000^\circ \text{C}$) als bei Ottomotoren verbunden. Bei solch hohen Temperaturen reagiert auch der in der Luft enthaltene Stickstoff mit dem Sauerstoff. Es entstehen Stickoxide, vor allem Stickstoffmonoxid (NO) und Stickstoffdioxid (NO2). 

**Abgasrückführung (AGR) oder Exhaust Gas Recirculation (EGR)** indem ein Teil des Abgases wieder zum Einlass des Zylinders rückgeführt wird. 

**Aufladen** um die Luftversorgung zu verbessern, saugt der Motor nicht nur selbst Umgebungsluft an, sondern ein Turbolader pumpt zusätzlich Luft in den Motor. 

\newpage
## Abgasrückführung

- einen Teil der frischen Verbrennungsluft durch sauerstoffarmes Abgas zu ersetzen und damit die NOx-bildende Temperaturspitze bei der Verbrennung zu senken. 

- das hauptsächlich aus Wasser und Kohlendioxid bestehende Abgas eine höhere Wärmekapazität als Frischluft hat und so ebenfalls zur Senkung der Spitzentemperatur beiträgt.

- Stickstoff, Sauerstoff, Kohlendioxid
    - Stickstoff (N2) ist sowohl im Frischgas als auch im Restgas enthalten. 
    - Sauerstoff-Anteil (O2) ist im Abgas gegenüber dem Frischgas zumindest stark reduziert. 
    - Erhöht ist im Abgas der Anteil an Kohlendioxid (CO2) und Wasser (H2O) im gasförmigen Zustand.  

- verschlechtert die Verbrennung künstlich und senkt so nicht nur den Stickoxid-Ausstoß, sondern auch die Motorleistung. Gleichzeitig entstehen mehr Rußpartikel durch die kältere Verbrennung. 

- Hochdruckrückführung und Niederdruckrückführung


**Abgasrückführrate** dient als Regelgröße. 
    - Die maximal bei PKW-Dieselmotoren eingesetzten Rückführraten liegen in der Größenordnung um 50 \%, d. h. die Hälfte der Zylinderfüllung stammt aus dem Abgas, der Rest ist Frischluft. 
    - Sobald die Rückführrate vom Sollwert abweicht,
        - steigt entweder die **NOx-Emission** wieder drastisch an oder 
        - verbunden mit einem Leistungsverlust und einer Verkokung des Turboladers die **Ruß-Emission**.


![Regelung der Abgasrückführrate. (Bild: Kai Borgeest)](images/EDC/EDC-10.pdf){width=50%}

\newpage
## Sensorik

Luftmassenmesser (LMM), auch MAF (Mass Airflow Meter) misst die angesaugte Frischluftmasse. 

- Die **ältesten Luftmassenmesser** bestanden aus einer Klappe, die durch den Luftstrom angehoben wurde. Über ein Potenziometer konnte dann der Winkel dieser Klappe gemessen werden. 

- **Hitzdrahtsensoren**

- **Heißfilm-Sensoren** 
    - in der Mitte des Sensorelements befindet sich eine beheizte Zone (4), auf beiden Seiten der Heizung befinden sich Temperatursensoren (M1 und M2). 
    - *Wenn keine Luft* durch den Sensor strömt, stellt sich eine symmetrische Temperaturverteilung um die Heizung ein und beide Sensoren messen die gleiche Temperatur. 
    - *Wenn nun Luft* (7) über die Oberfläche strömt, dann wird der in Strömungsrichtung vordere Sensor durch die Luft abgekühlt. Da die Luft über der Heizfläche Wärme aufnimmt, wird der hintere Sensor schwächer gekühlt. 
    - *Temperaturdifferenz* vor und hinter der Heizfläche wird als Maß für die vorbeiströmende Luftmasse und auch für die Strömungsrichtung benutzt. 
    - Die vorbeiströmende Luft enthält Staub und Öldämpfe aus dem Kurbelgehäuse des Motors. Der Sensor muss trotzdem über die gesamte Fahrzeuglebensdauer präzise messen. Grobe Abweichungen können die Motorsteuergeräte über Plausibilitätsprüfungen selbst erkennen und als Defekt melden.


![Aufbau und Prinzip des Heißfilm-Luftmassenmessers. (Bild: Robert Bosch GmbH)](images/EDC/EDC-11.pdf){width=50%}

**Lambda-Sonde** misst Restsauerstoff im Abgas

\newpage
## Aufladung

Die **Luftmenge**, die ein Motor aufnehmen kann, wenn der Kolben im Einlasstakt als saugende Pumpe wirkt, ist bei **Atmosphärendruck** durch das Volumen des Zylinders begrenzt.

Erhöhen lässt sich die **Luftmenge**, wenn die Luft mit einem **Überdruck** in den Zylinder gepresst wird. Dadurch verbrennt der Kraftstoff in den Phasen, in denen eine große Menge eingespritzt wird, besser und so entsteht weniger Rauch. Darüber hinaus lässt mit einer größeren Luftfüllung auch mehr Kraftstoff verbrennen und mehr Leistung erzeugen. 

Tatsächlich lässt sich mit einer Verdopplung des Ladedrucks der gleiche Effekt wie mit einer Verdopplung des Hubraums erzielen. Üblich sind Ladedrücke bis zum 2,5-fachen Atmosphärendruck.

Ein **Turbolader** besteht aus einem Pumpenrad im Ansaugtrakt, das über eine Welle von einer Turbine angetrieben wird. Die Turbine wird durch die Energie im Abgasstrom angetrieben. 

- **Vorteil** das die Abgasenergie sinnvoll genutzt wird und den

- **Nachteil** das insbesondere bei kleinen Drehzahlen die Energie im Abgas nicht ausreicht, um einen nennenswert erhöhten Ladedruck aufzubauen. Dieser Drehzahlbereich wird umgangssprachlich auch als Turboloch bezeichnet und ist für den Fahrer spürbar. 

- **Aufgabe Motorsteuergerät** Ladedruck zu regeln und eine schädliche Drucküberhöhung zu vermeiden. 
    - Da der Ladedruck einen erheblichen Einfluss auf das Fahrverhalten und den Kraftstoffverbrauch hat, können Steuergeräte eventuell die Führungsgrößen passend zum messbaren Fahrstil auswählen. Selten wird die Abgastemperatur vor der Turbine gemessen, um den Turbolader vor Überhitzung schützen zu können.

\newpage
# Abgasnachbehandlung (Ergänzen)

**Maßnahmen zur Absenkung der Stickoxidemissionen** Abgasrückführung oder späte Einspritzung erhöhen beim Dieselmotor die Partikelemissionen. 

**Maßnahmen zur Reduktion der Partikelemissionen** zu erhöhten Emissionen von Stickoxiden. 

**Möglichkeiten um schädliche Abgase zu minimieren**

1. ein Kompromiss zwischen Stickoxiden und Partikeln wird gesucht,
2. der Motor wird auf minimale NOx-Emissionen optimiert, die dabei zusätzlich entstehenden Partikel werden gefiltert,
3. der Motor wird auf minimale Partikelemissionen optimiert, die dabei zusätzlich entstehenden Stickoxide werden gefiltert oder
4. eine Abgasnachbehandlung reduziert zusätzlich NOx-Emissionen und Partikelemissionen.


![Umfangreich ausgestattetes Partikelfiltersystem mit zwei Oxidationskatalysatoren (OK), Partikelfilter (DPF), Temperatur-, Differenzdruck- und Rußsensor und zusätzlicher Kraftstoffeinspritzung in den Abgastrakt. (Bild: Kai Borgeest)](images/EDC/EDC-13.pdf){width=50%} 

![System zur selektiven katalytischen Reduktion (SCR) mit Harnstoff-Einspritzung, Oxidations-Katalysatoren (OK) und einem Ammoniak-Sperrfilter (SF). Da beide Steuergeräte über den CAN-Bus kommunizieren, kann die Zuordnung der Sensoren zu den Steuergeräten auch anders als im Bild erfolgen. (Bild: Kai Borgeest)](images/EDC/EDC-14.pdf){width=50%}

\newpage
# Abgasskandal


2015 wurde die Öffentlichkeit über die Medien informiert, dass Automobilhersteller bei der Feststellung von Abgaswerten manipulierten, um Fahrzeuge in den Markt zu bringen, die ohne Manipulationen nicht die gesetzlichen Grenzwerte einhalten.

In der Vergangenheit wurde auf einem Rollenprüfstand ein genormter Testzyklus
(**NEFZ**, Neuer Europäischer Fahrzyklus) gefahren, die Abgase während dieses Zyklus
wurden gemessen und mit den gesetzlichen Grenzwerten verglichen. Dieser Zyklus
vermied emissionskritische Situationen wie realistische Beschleunigungen und hohe
Geschwindigkeiten, außerdem enthielt er hohe Stillstandsanteile.

Der **Kern des Abgasskandals** lag nicht in der Verwendung eines unrealistischen Zyklus, sondern darin, dass viele Fahrzeughersteller Funktionen in der Software des Motorsteuergeräts oder des Getriebesteuergeräts implementiert haben, die einen derartigen Testzyklus von einer realen Straßenfahrt unterscheiden können. 

Die bloße Erkennung ist **legal**, so muss z. B. das ABS deaktiviert werden, wenn auf dem Rollenprüfstand nur die Antriebsräder drehen, nicht hingegen die anderen Räder.

**Illegal** ist hingegen, das Verhalten des Motorsteuergerätes so zu verändern, dass auf dem Prüfstand der Motor mit anderen Parametern betrieben wird und damit faktisch im Straßenverkehr ein anderer Motor als bei der Typprüfung eingesetzt wird ("Cycle Beating"). Auf dem Prüfstand werden Abgasrückführung und Abgasnachbehandlung so geregelt, dass die gesetzlichen Grenzwerte eingehalten werden, im Verkehr werden diese Einrichtungen abgeschaltet oder vermindert eingesetzt.

Die **Unterscheidung zwischen Prüfstand und Straße** erfolgt über die Auswertung von Fahrprofilen, der Umgebungsbedingungen (einige Fahrzeuge reduzieren abgasreinigende Maßnahmen unterhalb $17^\circ \text{C}$, weil für den NEFZ eine Mindesttemperatur von $20^\circ \text{C}$ vorgeschrieben war) oder im einfachsten Fall über einen Timer, der den Prüfstandsmodus nach Ablauf der Prüfzyklusdauer abschaltet. Häufige illegale Eingriffe („Abschaltfunktionen“) ins Motormanagement sind z. B. unterschiedliche Abgasrückführraten oder unterschiedliche SCR-Betriebsstrategien am Prüfstand und im Straßenverkehr.

Für Neuzulassungen wurde 2017 in Europa ein realistischerer Testzyklus im Rahmen
der **WLTP** (Worldwide Harmonized Light Vehicles Test Procedure) eingeführt, dieser
wurde bereits vor etlichen Jahren definiert, seine Einführung aber immer wieder verzögert.

Neu eingeführt wurde in der EU eine zusätzliche Straßenfahrt mit Abgasmessung (Real Driving Emissions, **RDE**), eine Erkennung der Abgasmessung wurde so erheblich erschwert.

\newpage
# Thermomanagement

**Ziel** nach dem Start schnell die optimale Betriebstemperatur des Motors von ca. $90^\circ \text{C}$ zu erreichen und dann zu halten. 

**mechanisch angetriebene Wasserpumpe** und über eine Zweipunktregelung mit Hilfe eines **Thermostaten**. 

- Der Thermostat bewirkt, dass bei noch kaltem Motor das Kühlwasser zunächst nicht über den Luftwärmetauscher (Kühler) fließt, sondern nur in einem kleinen Kreislauf.


**elektrisch angetriebene Wasserpumpe** 

- deren Verbreitung allerdings die hohe Leistung des Elektromotors entgegensteht. - 
- bei stehendem Motor z. B. um einen überhitzten Motor kontrolliert abzukühlen, ohne einen Temperaturschock des Motors zu riskieren.
- Die erwähnte Kühlwassertemperatur von $90^\circ \text{C}$ beinhaltet einen großen **Sicherheitsspielraum**, weil die Flüssigkeit je nach Überdruck im Kühlsystem und chemischer Zusammensetzung erst bei etwa $110$ bis $120^\circ \text{C}$ zu sieden beginnt. Eine geregelte Wasserpumpe ermöglicht eine Verkleinerung des Sicherheitsspielraumes zugunsten des Motorwirkungsgrades.


**Thermosiphon-Kühlung** Motoren ohne Wasserpumpe, bei denen die Konvektion (warmes Kühlmittel steigt aufgrund geringerer Dichte auf) genügte, das Kühlwasser umzuwälzen. **Energieeinsparung** bei schwacher Belastung des Motors die Wasserpumpe stillzulegen und zu überbrücken, wenn der Kühlkreis so ausgelegt ist, dass durch Konvektion eine ausreichende Kühlung sichergestellt ist.

**Gebläse mit einem Lüfterrad** hinter dem Kühler, das den Luftstrom unterstützt, wenn der Fahrtwind nicht ausreicht.

- Das Gebläse wird vom Motorsteuergerät abhängig von der Kühlwassertemperatur gesteuert. 
- Eventuell wird es auch nach Abstellen des Fahrzeugs und Ausschalten der Zündung noch angesteuert. In diesem Falle muss das Steuergerät während des Lüfternachlaufs auch noch seine eigene Spannungsversorgung aufrechterhalten. 
- Bei größeren Motoren ist die **Leistung elektrischer Lüfter** zu hoch für das Bordnetz, in diesem Fall wird der Lüfter mechanisch über eine Ölkupplung (Visco-Kupplung) oder zukünftig evtl. über eine Kupplung aus Formgedächtnislegierungen angetrieben. 


**elektrisch verstellbare Jalousie** vor dem Kühler, diese öffnet bei hohem Kühlbedarf, ansonsten schließt sie ganz oder teilweise und kann so auch die Aerodynamik des Fahrzeugs verbessern.

**elektrische Zuheizer** um schnell die Betriebstemperatur zu erreichen, werden bereits heute bei Dieselmotoren mit hohem Wirkungsgrad (und damit geringer Verlustleistung) im Kühlwasserkreislauf oder auch im Ansauglufttrakt verwendet. 

- *PTC-Heizer* bei Erreichen einer Solltemperatur steigt deren Widerstand sprunghaft an und der Heizstrom sinkt. 

**Ansteuerung der Glühkerzen** die Glühkerzen ragen bei "direkt einspritzenden Motoren" in den Brennraum, bei "Vorkammermotoren" heizen sie die Vorkammerwände auf.   

- sollen eine schnellere Verdampfung des Kraftstoffes beim Kaltstart bewirken. Sie erreichen innerhalb weniger Sekunden Oberflächentemperaturen von über $1000^\circ \text{C}$. 
- lange Vorglühen eines Dieselmotors vor dem Start, einst umgangssprachlich als Diesel-Gedenkminute bezeichnet, ist mit heutigen Glühkerzen nur noch bei tiefem Frost nötig. 
- können einen Strom von über 30 A (pro Kerze, 4-Zylinder ca. 120 A) verbrauchen, dies zu einem Zeitpunkt, zu dem auch der Anlasser Leistung von der evtl. kälteschwachen Batterie abfordert und der Fahrer womöglich Großverbraucher wie die Heckscheibenheizung eingeschaltet hat. 

**moderne Glühsysteme** bei denen die Kerzen nicht mehr über Relais geschaltet werden, kann das Steuergerät die Spannung nach Erreichen der Betriebstemperatur absenken und damit auch den Strom. 

- **Zwischenglühen** können Glühkerzen zugeschaltet werden, um insbesondere im Leerlauf die Verbrennung und damit die Abgaswerte zu verbessern. 
- **gelbe Kontrollleuchte** wird im Armaturenbrett angesteuert. Um den Fahrer nicht zu irritieren, leuchtet sie nicht bei jedem Glühvorgang, sondern nur wenn es sinnvoll ist, mit dem Starten zu warten.

**Brennraumdruck-Sensoren** können in Glühkerzen integriert werden.