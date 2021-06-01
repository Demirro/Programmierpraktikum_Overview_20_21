---
layout: post
title: "Error/Exception Handling und IO"
date: 2021-05-13 12:00:00 -0000
categories: java sose advanced
excerpt_separator: <!--more-->
external_link: https://github.com/Demirro/SoSe21_04_Recursion
---
Nicht einschlafen. Es geht ums Schafe zählen. Nur mit dem Wunder der Rekursion.
<!--more-->

# SoSe21_04_Recursion

## Übungsaufgabe für das Programmierpraktikum im SoSe 2021 zum 13.05.2021

Dieses mal eine kleinere Aufgabe. Es geht einfach nur um das Vertiefen des Konzeptes der Rekursion. Wer eine größere Challenge möchte, kann sich auch mal an das Tower of Hanoi Problem wagen. Oder sich zumindest angucken, wie dieses rekursiv und iterativ gelöst wird. Für die Leute, die womöglich noch einen Auffrischer oder eine Starthilfe bei dem Thema Rekursion brauchen, empfehle ich die externe Ressource am Ende dieser ReadMe.

Anbei wie immer meine Lösung .

### 📝 Aufgabe:

Wir wollen Schafe zählen (hoffentlich schläft keiner ein). Genauer gesagt die Anzahl an Beinen in einer Schafsherde Allerdings haben einige Schafe ein Bein verloren; jedes zweite Schaf unserer Herde genauer gesagt. Unsere Schafe sind so nummeriert worden, dass jedes Schaf mit einer ungeraden "Kennnummer" 4 Beine hat, jedes Schaf mit einer geraden "Kennnummer" allerdings nur drei. Schreibt also einen rekursiven Algorithmus, der die Anzahl an Schafsbeinen anhand der Anzahl an Schafen berechnen kann.

Bei einer Anzahl an 0 Schafen sollte der Output logischerweise 0 (Beine) sein.
Bei einem einzigen Schaf sollte der Output 4 (Beine) sein.
Bei zwei Schafen entsprechend 7 (Beine).
usw.

Testet euren Code natürlich. Hier nochmal ein paar Beispielergebnisse, damit ihr seht ob euer Code richtig ist
schafsBeine(0) → 0	
schafsBeine(1) → 4
schafsBeine(2) → 7
schafsBeine(3) → 11
schafsBeine(4) → 14	
schafsBeine(5) → 18
schafsBeine(6) → 21
schafsBeine(10) → 35

Viel Spaß und Erfolg
    
### ℹ️ Resourcen:
Hier noch ein paar nützliche 📃Artikel, 🖊️Threads und 🎥Videos

- [🎥 Börges Seminar Video (Iterable)](https://www.ilias.uni-koeln.de/ilias/ilias.php?ref_id=3957251&eid=fd0c3ca3-0bbb-4fbe-8448-2df6357419f3&cmd=streamVideo&cmdClass=xoctplayergui&cmdNode=x2:p7:18a:18l&baseClass=ilrepositorygui)

- [📃 Rekursion (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/Rekursion.html)
- [📃 Rekursion (Extern)](http://ais.informatik.uni-freiburg.de/teaching/ss09/info_MST/material/mst_08_recursion.pdf)

- [📃 Java Naming Conventions](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Naming-Conventions.md)

