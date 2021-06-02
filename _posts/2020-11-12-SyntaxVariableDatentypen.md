---
layout: post
title: "Syntax, Variablen und Datentypen"
date: 2020-11-12 12:00:00 -0000
categories: java wise basics
excerpt_separator: <!--more-->
external_link: https://github.com/Demirro/12-11_Syntax_Variablen_Datentypen
---
Eine kleine Einführung in die Basics der Java-Syntax und Bausteine für das Basteln erster Programme. In dieser Aufgaben wird ein Personalausweis in Java nachgebaut.
<!--more-->

# Willkommen bei der ersten Übungsaufgabe.

Zu aller Erst: Guckt euch das Seminarvideo an bevor ihr diese Aufgabe bearbeitet.
Die Videos bzw. das Hauptseminar werden immer die Grundlage für diese Übungsaufgaben bilden.

Der hochgeladene Code ist eine Musterlösung. Es ist nicht die einzig wahre Lösung, aber so wie ich mir die Lösung der Aufgabe vorgestellt habe.

### 📝 Aufgabe:

Es handelt sich bei dieser Aufgabe um eine relativ kleine Aufgabe. Sie soll dazu dienen euch die primitiven Datentypen etwas näher zu bringen und diese richtig auszuwählen und einzusetzen.

![personalausweis](https://raw.githubusercontent.com/Demirro/12-11_Syntax_Variablen_Datentypen/main/PersonalAusweis_Java.jpg)

Hier seht ihr einen Personalausweis mit diversen Feldern. Diese Felder beschreiben die Person und bilden diverse Eigenschaften ab.
Dabei sollte in eurem Programm immer der zweite Teil des Feldes in eine Variable gespeichert werden. Beispiel für ein Feld:

Vorname: Max

Hier sollte "Max" in eine Variable gespeichert werden.

Es sollte auch direkt auffallen, dass die verschiedenen Eigenschaften auch verschiedene "Datentypen" benutzen.

Ihr sollt nun die gesamten Daten des Personalausweises in ein kleines Java-Programm übertragen. 
1. Erstellt ein neues Java Projekt und die benötigte Main-Methode
2. Erstellt eine Variable für jedes Datenfeld des Personalausweises.
    1. Überlegt euch immer welcher Datentyp am sinnvollsten ist. Es wird nicht unbedingt jeder einzelene Datentyp benutzt.
3. Gebt die gespeicherten Variablen in der Konsole aus (eine Zeile pro Variable)
4. Versucht euren Code sinnvoll zu kommentieren
5. Beachtet die Java Naming Conventions

Als kleine Hilfestellung findet ihr hier unten noch ein paar Ressourcen, die euch weiterhelfen können. Beziehungsweise die Überblicke über die verschiedenen Themen aus dem Java-Wegweiser.

## Datentyp String
Ein Datentyp der per se kein primitiver Datentyp ist, jedoch fast so genutzt wird, ist der *String*.
Ein String wird genutzt, um eine längere Zeichenkette, wie einen Satz, zu speichern, verarbeiten oder auszugeben. Beispiel wie man eine String-Variable in Java erstellt:

`String variable = "Hier ist eine längere Zeichenkette";`

Den Datentypen String werdet ihr in dieser Aufgabe nutzen müssen.

    
### ℹ️ Resourcen:
Hier noch ein paar nützliche 📃Artikel, 🖊️Threads und 🎥Videos

- [🎥 Börges Seminar Video](https://www.ilias.uni-koeln.de/ilias/ilias.php?ref_id=3638292&eid=ccc0c271-a980-47c7-8484-c1160a1e6933&cmd=streamVideo&cmdClass=xoctplayergui&cmdNode=wn:os:17u:185&baseClass=ilrepositorygui)

- [📃 Primitive Datentypen (Wegweiser)](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Datentypen.md)
- [📃 Primitive Datentypen (extern)](https://de.wikibooks.org/wiki/Java_Standard:_Primitive_Datentypen)
- [📃 Konsolenausgabe (grundlegend)](https://www.geeksforgeeks.org/system-out-println-in-java/)
- [📃 Java Naming Conventions](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Naming-Conventions.md)
- [📃 Java String Datentyp](https://www.inf.fh-flensburg.de/lang/prog/string.htm)
- [📃 ASCII-Tabelle (für char)](https://www.torsten-horn.de/techdocs/ascii.htm)
