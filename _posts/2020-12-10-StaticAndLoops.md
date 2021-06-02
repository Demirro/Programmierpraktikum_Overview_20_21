---
layout: post
title: "Static und Lopps"
date: 2020-12-10 12:00:00 -0000
categories: java wise advanced
excerpt_separator: <!--more-->
external_link: https://github.com/Demirro/10-12_Static_and_Loops
---
Was macht das Stichwort Static und wie kann man Sachen wiederholt durchführen? Programmiert hier eine Hilfsklasse mit diversen mathematischen Methoden.
<!--more-->

# 10-12 Static und Loops
Übungsaufgabe für das Programmierpraktikum im Wise 20/21 zum 10.12.2020

# Willkommen bei der fünften Übungsaufgabe.

Diese Woche halten wir die Aufgabe kurz. Wir wenden sowohl das keyword *static* als auch Schleifen an. Das hochgeladene Projekt ist wieder eine Vorlage. Dort sind nur Tests enthalten, um zu sehen, ob eure Methoden funktionieren.

### 📝 Aufgabe:

Ihr habt im Seminar bereits die Math Klasse aus der Standardbibliothek in Java kennengelernt. Jetzt gehen wir aber einen Schritt zurück und programmieren unsere eigene simple MathUtils Klasse. Diese soll zwei Methoden enthalten, die in unserem gesamten Projekt aufrufbar sind. Dabei sollte kein Objekt der Klasse *MathUtils* erstellt werden müssen, um auf die Methoden zugreifen zu können.
Die zwei Methoden sollen wie folgt aufgebaut werden:

*power*:
- Berechnet die Potenz einer angegebenen Exponation
- Nimmt zwei Integer als Parameter. Dabei stellen die zwei Parameter folgendes dar:
    - Basis
    - Exponent
- Gibt den Potenzwert als integer zurück

*factorial*:
- Berrechnet die Fakultät einer angegeben Zahl
- Nimmt als Parameter einen int, dessen Fakultät errechnet werden soll
- Gibt das Ergebnis als integer zurück

Für beide dieser Methoden kann man verschiedene Schleifen benutzen, um das Problem zu lösen. Versucht vielleicht mal verschiedene Ansätze, damit ihr sowohl while als auch For-Schleifen kennenlernt. Zusätzlich könnt ihr eure Methoden mit JavaDoc kommentieren und auch da ein wenig üben. Gerade bei Utility-Klassen und Methoden ergibt das besonders viel Sinn.

    
### ℹ️ Resourcen:
Hier noch ein paar nützliche 📃Artikel, 🖊️Threads und 🎥Videos

- [🎥 Börges Seminar Video](https://www.ilias.uni-koeln.de/ilias/ilias.php?ref_id=3638292&eid=8365d934-fb95-44f2-ac19-397d2e32f014&cmd=streamVideo&cmdClass=xoctplayergui&cmdNode=wn:os:17u:185&baseClass=ilrepositorygui)

- [📃 Static Members (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/Static-Members.html)
- [📃 Schleifen (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/Schleifen.html)

- [📃 Java Naming Conventions](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Naming-Conventions.md)
