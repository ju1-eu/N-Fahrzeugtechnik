---
title: 'Lösung - Gemischbildung Diesel'
author: 'Jan Unger'
date: \today
subject: "Markdown"
keywords: [Markdown,Latex,HTML,PDF,Pandoc,Shell-Script]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!--------------------------------------------------+
Dozent: Marc Limburg
Thema:  Loesung -- Betriebs- und Hilfsstoffe
Fachbuch S. 243 ([@brand:2020:fachkundeKfz])
Fachbuch S. 142 ([@respondeck:2019:servicetechniker])
Bosch S. 562 ([@reif:2022:boschkraftfahrtechnisches]).
Tabellenbuch S. 281 ([@bell:2021:tabellenbuchKfz])
FS S. 32 -- 37 ([@bell:2020:formelsammlung])
^\circ\text{C}
#
## 
ju 15-10-22
+----------------------------------------------------->

**1) Was versteht man unter innerer Gemischbildung beim Dieselmotor?**

Darunter versteht man, dass das Gemisch im Zylinderraum des Motors entsteht. Der Dieselkraftstoff also erst dort mit der Ansaugluft in Berührung kommt.


**2) Definieren Sie Quantitätsregelung und Qualitätsregelung.**


1. Unter einer **Quantitätsregelung** versteht man, dass der Motor durch eine Anpassung der Gemischmasse zum Beispiel durch eine Drosselklappe geregelt wird.
2. Bei einer **Qualitätsregelung** erfolgt die Luftzufuhr nahezu Last unabhängig. Lediglich die Kraftstoffmasse wird mit zunehmender Last erhöht.


**3) Bei welcher Temperatur wird Dieselkraftstoff zündfähig und wann entzündet er sich von selbst?**

1. zündfähig bei etwa $60^\circ\text{C}$

1. Selbstzündungstemperatur (untere Grenze) $220^\circ\text{C}$ (im Mittel) bei ca. $350^\circ\text{C}$ Quelle: Bosch S. 562 ([@reif:2022:boschkraftfahrtechnisches]).


**4) Erklären Sie ausführlich den Verbrennungsablauf im Brennraum eines direkt einspritzenden Dieselmotors.**

Gegen Ende des Verdichtungstaktes wird Dieselkraftstoff fein zerstäubt, in die $600 - 900^\circ\text{C}$ heiße Luft eingespritzt. Diese verdampft über die Oberfläche der entstandenen Kraftstofftropfen. Je feiner die Zerstäubung des Kraftstoffes, desto größer ist die Oberfläche im Verhältnis zum Volumen, was den Vergasungsprozess begünstigt. Die gasförmigen Kohlenwasserstoffe vermischen sich mit der Ansaugluft und erhitzen sich, bis sich bei ca. $220^\circ\text{C}$ zur Selbstentzündung des Kraftstoffes kommt. Je nach System wird dieser Vorgang Last- und Drehzahlabhängig in mehreren Vorgängen unterteilt, um den Druckanstieg im Zylinder und damit die Laufkultur des Motors zu begünstigen.


**5) Unter welchen motorischen Bedingungen entstehen beim Dieselmotor unverbrannte Kohlenwasserstoffe?**

1. Kaltstart- und Warmlaufphase (kalter Motor hat geringere Kompression, Kondensationsverluste an Zylinderwand, Wärmeabgabe an Brennraumwände)
1. Volllastbetrieb (Kraftstoffüberschuss)
1. Luftmangel (verstopfter Luftfilter, defekter Turbolader, undichter Ladeluftkühler)
1. Defekte Injektoren (schlechtes Strahlbild, tropfen nach $\to$ mehr Kraftstoff)
1. Kompressionsverluste (Verdichtungstemperatur wird später erreicht)


**6) Warum wird beim Dieselmotor bei Volllast über einen größeren Zeitraum eingespritzt?**

Da bei Volllast der maximale Einspritzdruck eingestellt wird, geht die Mengenregelung nur über die Zeit.

**7) Wie groß ist beim Dieselmotor der Luftüberschuss bei Leerlauf / Volllast?**

- Leerlauf $\lambda = 10 \dots 18$
- Volllast $\lambda = 1,15 \dots 2$

(Luftzahl / Lambda)


**8) Definieren Sie Zündverzug. Wie groß ist der Zündverzug?**

Die Zeitspanne von Einspritzbeginn an der Einspritzdüse und dem Zündbeginn des Kraftstoff-Luft-Gemisches im Brennraum.

Zündverzug bei betriebswarmer Motor: 1 ms


**9) Wodurch kann es bei betriebswarmem Motor zum Nageln kommen?**

Durch einen zu großen Zündverzug.

**Mögliche Ursachen:**

1. zu früher Einspritzbeginn
1. Mangelhafte Kompression
1. Luftmangel (verstopfter Luftfilter, defekter Turbolader, undichter Ladeluftkühler)
1. schlechte Kraftstoffqualität (Cetanzahl zu niedrig)
1. Nach tropfende Einspritzdüse


**10) Warum muss beim indirekt einspritzenden Dieselmotor das Verdichtungsverhältnis 18 - 24:1 betragen, während beim direkt einspritzenden Dieselmotor ein Verdichtungsverhältnis von 14 bis 18:1 ausreicht?**

Die Oberfläche des Zylinderraumes ist bedingt durch die Vor- oder Wirbelkammeroberfläche bei indirekt einspritzenden Dieselmotor größer, wodurch es zu stärkeren Wärmeverlusten kommt. Diese müssen durch eine stärkere Erwärmung der Luft, also durch ein höheres Verdichtungsverhältnis, kompensiert werden.

(Eine höhere Kompression kostet aber auch mehr Kompressionsarbeit.)