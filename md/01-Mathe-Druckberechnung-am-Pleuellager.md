---
title: 'M-Druckberechnung am Pleuellager'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown, Example]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!---------------------------------------------------+
Dozent: Marc Limburg
Thema:  Mathe - Druckberechnung am Pleuellager
Fachbuch ([@brand:2020:fachkundeKfz] S. 243)
Fachbuch ([@respondeck:2019:servicetechniker] S. 142)
Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 281)
FS ([@bell:2020:formelsammlung] S. 32 - 37)
#
## 
ju 15-4-22
+----------------------------------------------------->

# Druckberechnung am Pleuellager

**Kolbenflächenberechnung:** $\boxed{A = \frac{d^2}{4} \cdot \pi}$

Kolbendurchmesser $d = 80~mm = 8~cm$

$A_{Kolben} = \frac{(80~mm)^2}{4} \cdot \pi 
= 5026,55~mm^2 
= 50,27~cm^2$

**Kolbenkraftberechnung:** $\boxed{\text{Druck} = \frac{\text{Kraft}}{\text{Fläche}}}$

$\boxed{p = \frac{F}{A}} \quad 
\boxed{p\,[N/cm^2] \quad 
F\,[N] \quad 
A\,[cm^2]} \quad
\boxed{10~N/cm^2 = 1~bar}$

**Verbrennungsdrücke:**

$\text{Benzin} \to 65~bar = 650~N/cm^2 \quad
\text{Diesel} \to 180~bar = 1800~N/cm^2$

$F = p \cdot A \\ 
F_{Kolben_B}  = 50,27~cm^2 \cdot 650~N/cm^2 
             = 32675,5~N \\
F_{Kolben_D}  = 50,27~cm^2 \cdot 1800~N/cm^2 
             = 90486~N$

**Kreisbogenberechnung:** $\boxed{A = \frac{d \cdot \pi}{2} \cdot b}$

$d_{Kurbelwelle} = 60~mm = 6~cm \\
d_{Lager}        = 25~mm = 2,5~cm$

$A_{Krb} = \frac{6~cm \cdot \pi}{2} \cdot 2,5~cm
         = 23,56~cm^2$

**Druckberechnung Pleuelfuß:**

$p_{Pleuel_{Benzin}} = \frac{F}{A} 
                  = \frac{32675,5~N}{23,56~cm^2}
                  = 1386,91~N/cm^2
                  = 138,69~bar  \\
p_{Pleuel_{Diesel}}  = \frac{F}{A} 
                  = \frac{90486~N}{23,56~cm^2}
                  = 3840,66~N/cm^2
                  = 384,07~bar$

**Versorgungsdruck (Öldruck) max.** $5~bar$

$\to p_{Pleuel_{Benzin}}:\,138,69~bar$

$\to p_{Pleuel_{Diesel}}:\,384,07~bar$

Vgl. Kapitel "*Motormechanik / Hydrodynamischer Schmierkeil*"