---
title: 'L-BremseII'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!--ju 24-12-22  Bremse II-->


**1) Was versteht man unter Schlupf?**

Schlupf ist die Differenz zwischen der Fahrgeschwindigkeit und der Radumfangsgeschwindigkeit.

**2) Was geschieht während der ABS – Regelung?**

- Zunächst wird der Druckaufbau gestoppt
- Wenn der Schlupf weiter zunimmt, wird der Druck geringfügig gesenkt
- Wenn der Schlupf wieder abnimmt, wird der Druck erhöht, um im optimalen Bremsbereich zu bleiben

Bemerkung:

Das ABS-Steuergerät erhält zur Regelung des Bremsvorgangs die Radgeschwindigkeit von den Raddrehzahlsensoren. 

- sinusförmige Wechselspannung (Induktivgeber) 
- oder ein Rechtecksignal (Hallgeber) 

Daraus wird eine Fahrzeug-Referenzgeschwindigkeit gebildet. Das Steuergerät erkennt Drehzahländerungen an einem oder mehreren Rädern. 

Sinkt die Raddrehzahl innerhalb einer Zeitspanne oder in Bezug auf die Referenzgeschwindigkeit, wird das als Blockiergefahr erkannt.



**3) Wie viele ABS – Regelkreise können bei einem Fahrzeug mit hydraulischer Bremsanlage vorhanden sein? Wie sind diese ggf. zugeordnet?**

- 2 $\to$  je ein Regelkreis pro Vorderrad
- 3 $\to$  je ein Regelkreis für jedes Rad der Vorderachse und ein gemeinsamer Regelkreis für die Räder der Hinterachse.
- 4 $\to$ je ein Regelkreis für jedes Rad der Vorder- und Hinterachse


**4) Wie ist ein aktiver Drehzahlsensor aufgebaut?**

Der Hall-Sensor besteht im Wesentlichen aus einem stromdurchflossen, Halbleiterbauelement und einem magnetischen, in Nord- und Südpole unterteilten Impulsring. Ändert sich die Polarität des, auf das Hall-Element wirkenden Magnetfeldes, ändert sich die Hallspannung innerhalb des Halbleiters, woraus die integrierte Auswerteelektronik ein Rechtecksignal formt und dieses an das Steuergerät sendet. Die Frequenz des Rechteckssignals ist proportional zur Raddrehzahl.

**5) Warum lässt sich ein Fahrzeug bei Ausfall des ABS noch normal bremsen?**

In der Ruhelage sind die Magnetventile in der Hydraulikeinheit einlassseitig geöffnet und auslassseitig geschlossen.

**6) Wie ist die grundsätzliche Wirkungsweise der Antriebsschlupfregelung (ASR)?**

Wird an einem der Antriebsräder ein erhöhter Schlupf (> 8 -- 35 \%) erkannt, so wird systemabhängig das Motordrehmoment reduziert und/oder die durchdrehenden Rad/Räder mithilfe der Betriebsbremse abgebremst.

**7) Was wird durch die Motorschleppmomentregelung (MSR) verhindert?**

Verhindert durch automatische Erhöhung des Motormoments, dass die Antriebsräder aufgrund der Abbremsung durch den Motor bei plötzlicher Gaswegnahme oder beim Zurückschalten einen erhöhten Schlupf aufweisen.

**8) Was versteht man unter dem Begriff "Giermoment"?**

**Giermoment / Drehrate** Drehung des Fahrzeugs um die Fahrzeughochachse

**9) Welche Systeme bilden mit ihren Funktionen das eigentliche elektronische Stabilitätsprogramm (ESP)?**

1. (+) Antiblockiersystem (ABS)
1. (+) Elektronische Bremskraftverteilung (EBV)
1. (+) Antriebsschlupfregelung (ASR) 
1. (+) Motorschleppmomentregelung (MSR)
1. (+) Giermomentregelung (GMR)
1. (=) Fahrdynamikregelsystem (FDR) = Elektronisches Stabilitätsprogramm (ESP)

**10) Wie reagiert das ESP – Steuergerät beim Übersteuern eines Fahrzeugs mit Standardantrieb?** 


**ESP-Eingriff beim Übersteuern:** 

- *ohne ESP* würde beim Fahrzeug das Heck ausbrechen und der Fahrer muss gegenlenken. 

- *mit ESP* unterstützt den Fahrer durch einen Bremseingriff, vorwiegend am kurvenäußeren Vorderrad. Dadurch entsteht ein Giermoment/Drehrate um die Hochachse, das das Auto wieder auf den gewünschten Fahrkurs zieht.
- Das Antriebsmoment der Hinterräder gesenkt und deren Seitenführungskräfte zu erhöhen

Bemerkung:

**ESP-Eingriff beim Untersteuern:** 

- *ohne ESP* würde das Fahrzeug über die Vorderräder aus der Kurve schieben. 

- *mit ESP* unterstützt die Lenkkorrektur des Fahrers durch einen Bremseingriff, vorwiegend am kurveninneren Hinterrad. Dadurch entsteht ein Giermoment/Drehrate um die Hochachse, das das Auto in die Kurve hineindreht.