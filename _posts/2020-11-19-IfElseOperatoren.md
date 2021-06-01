---
layout: post
title: "If & Else Operatoren"
date: 2020-11-19 12:00:00 -0000
categories: java wise basics
excerpt_separator: <!--more-->
external_link: https://github.com/Demirro/16-11_IfElse_Operatoren
---
Der Grundstein der Programmierung: If-Else in Java
<!--more-->

# 16-11_IfElse_Operatoren
Übungsaufgabe für das Programmierpraktikum im Wise 20/21 für den 16.11.2020

# Willkommen bei der zweiten Übungsaufgabe.

Diese Woche habe ich eine Vorlage hochgeladen. Ladet euch also bitte den Code herunter und bearbeitet die Aufgabe damit.
Ihr habt in der letzten Seminarstunde das Casting und Operatoren kennengelernt. Die folgende Aufgabe soll euch sowohl den Umgang damit beibringen, als euch auch die sogenannten If-Else Blöcke näherbringen.

### 📝 Aufgabe:

Ihr sollt diese Woche einen Notenrechner erstellen. In der Vorlage sind zwei Variablen gegeben (*erreichtePunktzahl* und *maximalePunktzahl*). Ihr sollt eine dritte Variable (*erreichteProzente*) aus den zwei ersten Variablen errechnen.

Anhand der nun errechneten Prozent sollte ihr jetzt eine Ausgabe generieren, die sagt ob die Punktzahl reicht um zu bestehen und welche Note man bekommt. Dazu folgender Notenspiegel:
| Note             | Prozent |
|------------------|---------|
| 1 (sehr gut)     | 100-90  |
| 2 (gut)          | 89-75   |
| 3 (befriedigend) | 74-60   |
| 4 (ausreichend)  | 59-50   |
| 5 (mangelhaft)   | 49-35   |
| 6 (ungenügend)   | 34-0    |

Um diese Ausgabe zu generieren müssen wir überprüfen, in welchem Bereich des Notenspiegels der Wert der Variable *erreichteProzente* fällt. Dazu brauchen wir:

## If-Else
Aus dem [Wegweiser](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Konditionale.md):

Ein `if/else`-Statement führt Code in Abhängigkeit vom Wahrheitsgehalt (`true`/`false`) einer Aussage bzw. eines boolschen Ausdrucks aus. Es besteht mindestens aus **einem** `if`-Block (_wenn, dann..._), einer **beliebigen Anzahl von** `else if`-Blöcken (_sonst wenn, dann..._) und **maximal einem** `else`-Block (_sonst..._). 

**:point_right: [Syntax](../Glossar.md#syntax)-Beispiel:**
```java
int i = 4;

if (i > 5){
  // größer!
} else if (i < 5) {
  // kleiner!
} else {
  // gleich!
}
```

Es wird hier generell immer **nur einer** der Blöcke ausgeführt! Wenn im `if`-Block die Bedingung erfüllt ist, dann werden die folgenden Blöcke ignoriert. Wenn nicht, dann werden nacheinander die (optionalen) `else if`-Blöcke überprüft und ggf. einer davon ausgeführt. Falls keine der angegebenen Bedingungen zutraf, wird der (ebenfalls optionale) `else`-Block ausgeführt.

## Tipps
- Falls die If-Else Geschichte noch nicht klar ist, guckt bitte in die Ressourcen. Da gibt es noch weitere Erklärungen der Thematik
- Denkt beim Berechnen der erreichten Prozente an die Datentypen
- Benutzt die Operatoren in den Bedingungen und vergesst nicht, dass es *&&* oder *||* gibt
- Kontrolliert euer Programm indem ihr auch mal die Ausgangsvariablen ändert und schaut ob alles so funktioniert wie es sollte

    
### ℹ️ Resourcen:
Hier noch ein paar nützliche 📃Artikel, 🖊️Threads und 🎥Videos

- [🎥 Aufzeichnung des Seminars](https://www.ilias.uni-koeln.de/ilias/ilias.php?ref_id=3638292&eid=3ebe7375-f969-4330-ad74-a1dbb784ec62&cmd=streamVideo&cmdClass=xoctplayergui&cmdNode=wn:os:17u:185&baseClass=ilrepositorygui)

- [📃 Primitive Datentypen (Wegweiser)](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Datentypen.md)
- [📃 If-Else (Conditionals) (Wegweiser)](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Konditionale.md)
- [📃 If-Else (extern)](https://www.java-programmieren.com/if-anweisung-java.php)
- [📃 Operatoren (Wegweiser)](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Operatoren.md)
- [📃 Casting (Wegweiser)](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Casting.md)

- [📃 Java Naming Conventions](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Naming-Conventions.md)

### P.S. Wieso double statt float?
**an diejenigen aus dem letzten Zoom-Meeting und an die, die es interessiert**

Java geht bei der Eingabe von Kommazahlen wie *0.5* standardmäßig davon aus, dass es sich um den Datentypen Double handelt.
Das ist im ersten Moment nicht ganz intuitiv, da der Datentyp Double 8 Bytes belegt, wohingegen der Datentyp float (auch für Kommazahlen genutz) nur 4 Bytes belegt. Nach aller bisher bekannten Logik sollte man also meinen, dass ein Datentyp der weniger Arbeitsspeicher belegt sinnvoller als Standard ist.

Jetzt die Krux:
Float und Double werden als binäre Gleitkommazahlen gespeichert. Ich will jetzt nicht zu viel ausschweifen aber erinnert euch an BIT und an die Geschichte mit den Mantissen und co. Nun in diesem System kommt das Problem auf, dass die Repräsentation einer Kommazahl aus dem Dezimalsystem in binärer Form sehr ungenau ist. 

Beispiel:

0.5 wäre in binär 0.1

0.6 wäre in binäre 0.10011001100110011001100110011001100110011001100110011001100110... und so weiter. Also es wiederholt sich periodisch.

Als float würde 0.6 also wie folgt aussehen: 0.100110

Als double würde 0.6 wie folgt aussehen:     0.10011001100110

Also ist double viel präziser und das ist oft sehr wichtig, wichtiger als Arbeitsspeicher. Zusätzlich braucht man scheinbar nicht mehr Rechenleistung wenn man mit double statt float arbeitet.
Heißt konkret, man setzt float nur ein, wenn man mit streng limitierten Arbeitsspeicher arbeiten muss und die Präzision vernachlässigt werden kann. Und deswegen haben die Java-Designer sich dazu entschieden double als Standard für Kommazahlen zu nutzen.
