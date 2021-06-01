---
layout: post
title: "Error/Exception Handling und IO"
date: 2021-05-06 12:00:00 -0000
categories: java sose advanced
excerpt_separator: <!--more-->
external_link: https://github.com/Demirro/SoSe21_03_IO_ErrorHandling
---
Eine Wiederholung zu den Themen der Exceptions, dem Umgang mit diesen und Input/Output in Java.
<!--more-->

# SoSe21_03_IO_ErrorHandling (Wiederholung)

## Übungsaufgabe für das Programmierpraktikum im SoSe 2021 zum 06.05.2021

In der Übungsstunde am Donnerstag haben wir uns als Wiederholung Inputs und Outputs sowie Fehlerbehandlung angeschaut. Also Dateien ein- und auslesen und alles was mit Exceptions, Errors, Try-Catch und throws zu tun hat. Die Aufgabe diese Woche soll einfach nur mal wiederholen und einsetzen, außerdem ist noch ein kleiner Comparator enthalten.

Der beiliegende Code ist meine Umsetzung. Guckt euch diese bitte nur an, wenn ihr fertig seid oder überhaupt nicht weiterkommt und schon die Ressourcen als Hilfe benutzt habt.

### 📝 Aufgabe:

Erstellt eine Klasse Namens FileScanner. Diese soll nur eine statische Methode beinhalten *scanFileToList*. Diese Methode soll eine Datei einlesen und eine Liste der einzelnen Wörter in der Datei zurückgeben. Wie ihr das umsetzt könnt ihr selbst entscheiden; da gibt es diverse Wege und denkt immer schön an die Fehlerbehandlung bei Dateioperationen.
In eurer Main-Methode könnt ihr das testen indem ihr beispielsweise die Wörter der Liste zählt/ausgibt, die Liste anzeigt o.ä.
Zu guter Letzt sollt ihr nun noch einen Comparator erstellen und einmal einsetzen, mit welchem ihr eure tolle neue Liste sortieren könnt. Die natürliche Reihenfolge von Strings ist ja alphabetisch, also versucht eine andere halbwegs sinnvolle Sortierung zu nehmen. Länge des Wortes oder von mir auch was verrückt wie Anzahl and Vokalen oder sowas. 

Eine Beispiel-Textdatei findet ihr hier in der Musterlösung *scanThis_Kafka.txt*. Die beinhaltet genau 498 Wörter. Euch ist aber freigestellt eure eigene Datei zu erstellen. 

Tipp: Wenn jemand mit Regex arbeiten will findet unten eine kleine Einleitung und hier ist der Ausdruck, um alle Satzzeichen und leerzeichen zu entfernen "[^a-zA-Z 0-9]"
Erfindet das Rad auch nicht neu. Ihr habt bereits mit IO gearbeitet. Klaut euch den Code und passt es an eure jetzigen Bedürfnisse an.

Ihr könntet auch noch weitergehen und eine Liste aus einzigartigen Wörtern zu machen. Dafür gibt es auch diverse Wege. Ich lasse aber erstmal außen vor, aber wenn jemand Lust hat, nur zu.

Viel Spaß und Erfolg
    
### ℹ️ Resourcen:
Hier noch ein paar nützliche 📃Artikel, 🖊️Threads und 🎥Videos

- [🎥 Börges Seminar Video (Comparable & Comparator)](https://www.ilias.uni-koeln.de/ilias/ilias.php?ref_id=3957251&eid=1fd96088-461a-4bc0-af78-869164662b58&cmd=streamVideo&cmdClass=xoctplayergui&cmdNode=x2:p7:18a:18l&baseClass=ilrepositorygui)

- [📃 Input & Outpur (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/IO.html)
- [📃 Fehlerbehandlung (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/IO.html)
- [📃 Fehlerbehandlung (Extern)](https://java-tutorial.org/exception-handling.html)
- [📃 Vergleichen und Sortieren (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/Vergleichen-Sortieren.html)
- [📃 Regex (extern)](https://openbook.rheinwerk-verlag.de/javainsel9/javainsel_04_007.htm)

- [📃 Java Naming Conventions](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Naming-Conventions.md)
