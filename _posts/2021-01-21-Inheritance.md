---
layout: post
title: "Inheritance (Vererbung)"
date: 2021-01-21 12:00:00 -0000
categories: java wise advanced
excerpt_separator: <!--more-->
external_link: https://github.com/Demirro/21-01_Inheritance
---
Programmstruktur aufbauen, Klassen verbinden und Eigenschaften und Methoden von einer Klasse zur nächsten vererben. Eines der Wichtigsten Konzepte der Objektorientierten Programmierung. In dieser Aufgaben spielen wir Gott in der Schöpfungsgeschichte und bauen unsere Realität rudimentär nach. (Es soll kein religiöser Kommentar sein, weder positiv, noch negativ)
<!--more-->

# 21-01_Inheritance
Übungsaufgabe für das Programmierpraktikum im Wise 20/21 zum 21.01.2021

# Willkommen bei der siebten Übungsaufgabe.

Diese Woche sollt ihr einfach nur üben das neue Konzept der Vererbung zu nutzen. Ich lade eine Lösung direkt mit hoch, allerdings findet ihr dieses Mal auch den Code aus der letzten Übungsstunde im Repo. Mit diesem Code werden wir die nächsten Stunden/Wochen noch weiterarbeiten.
Wir nehmen uns da den Satz "God is an OOP programmer zu Herzen" und bauen die Struktur der Welt in Java nach. Angefangen haben wir, indem wir Menschen erstellt haben. Dadrunter sind zwei Subklassen, die vom Menschen "erben": Male und Female. Male und Female habe als Subklassen von Human teilweise gleiche Eigenschaften Fähigkeiten, unterscheiden sich aber in einigen Aspekten voneinander, was in Java ideal durch Vererbung dargestellt werden kann.
Der Code aus der letzten Stunde ist ein erster (kommentierter) Ansatz und kann als Beispiel dienen, um sich mit Vererbung bekannt zu machen.


### 📝 Aufgabe:

![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) __Der Code auf Github ist nur die Lösung und Code aus der letzten Stunde, keine Vorlage__

Stellt euch vor ihr seit in einem HR-Department. Ihr müsst die diversen Arbeitnehmer in eurem Unternehmen für die Unterlagen und euer System klassifizieren können.
Ihr schreibt eine simple Anwendung in Java, um ein Ordnungssystem zu erstellen.
Eure Mitarbeiter haben zwar diverse Fachrichtungen haben aber dennoch (im Rahmen des Unternehmens) Gemeinsamkeiten. Um euch Arbeit zu sparen und eine gute Struktur zu schaffen entscheidet ihr euch Vererbung zu nuten. 
Ihr erstellt erstmal drei Klassen für ein Proof-of-concept: Employee, Programmer und Artist

#### *Klassen*:
*Employee*:
Diese Klasse beinhaltet alle Eigenschaften und Fähigkeiten, die jeder Arbeitnehmer hat (bspw.):
- Name
- Alter
- Gehalt
- Methode raise(int percent) zum erhöhen des Gehalts
  - Nimmt einen Integer als Parameter, der für die prozentuale Erhöhung des Gehalts steht
- Methode printData() zum Anzeigen der Eigenschaften
  - Name, Alter, Gehalt

*Programmer*:
- erbt von Employee
- besitzt als Instanzvariable die genutzte Programmiersprache (Java, Python, C# oder sonst was)
- printData() wird ergänzt mit einer Ausgabe über die Programmiersprache


*Programmer*:
- erbt von Employee
- besitzt als Instanzvariable das genutzte Programm (Photoshop, Gimp, InDesign oder sonst was)
- printData() wird ergänzt mit einer Ausgabe über das Programm

Testet mit einer vierten Klassen (mit der Main-Methode) eure Klassen und Methoden.

### Kleines Extra:
Guckt euch Getter & Setter und Konstruktoren genauer an. Eines davon werdet ihr mindestens brauchen, um die Aufgabe zu schaffen. Getter & Setter sind einfacher zu verstehen, aber benötigen mehr Schreibarbeit. Konstruktoren sind effizienter und schöner im Code. Idealerweise solltet ihr mit beidem vertraut sein. Man nutzt meistens auch beides zusammen.

Ihr könnt wenn ihr Lust und Zeit habt sowohl das Employee-Beispiel als auch unser Gott-Beispiel aus der Übungsstunde selbsständig erweitern und Methoden und Attribute hinzufügen. Übung ist beim Programmieren das wichtigste.
    
### ℹ️ Resourcen:
Hier noch ein paar nützliche 📃Artikel, 🖊️Threads und 🎥Videos

- [🎥 Börges Seminar Video](https://www.ilias.uni-koeln.de/ilias/ilias.php?ref_id=3638292&eid=57e30ebc-8c9d-4978-9b36-7fa333c00d6d&cmd=streamVideo&cmdClass=xoctplayergui&cmdNode=wn:os:17v:186&baseClass=ilrepositorygui)

- [📃 Objektorientierte Programmierung (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/OOP-Klassen-und-Objekte.html)
- [📃 Objekte I (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/Objekte-I-Initialisierung-Members-Zugriff.html)
- [📃 Vererbung I (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/Vererbung-I-Grundlagen.html)
- [📃 Vererbung (Extern)](http://openbook.rheinwerk-verlag.de/javainsel9/javainsel_05_008.htm)

- [📃 Java Naming Conventions](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Naming-Conventions.md)
