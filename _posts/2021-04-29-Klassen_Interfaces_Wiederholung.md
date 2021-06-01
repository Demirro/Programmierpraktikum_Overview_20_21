---
layout: post
title: "Klassen, Interfaces (Wiederholung"
date: 2021-04-29 12:00:00 -0000
categories: java sose basics
excerpt_separator: <!--more-->
external_link: https://github.com/Demirro/SoSe21_02_KlassenInterfaces_Wiederholung/
---
Der erste Teil der Wiederholung für das zweite Semester des Java-Seminars. Noch einmal die Grundlagen der Objektorientierten Programmierung durcharbeiten!
<!--more-->

# SoSe21_02_KlassenInterfaces_Wiederholung

## Übungsaufgabe für das Programmierpraktikum im SoSe 2021 zum 29.04.2021

In der Übungsstunde am Donnerstag haben wir uns als Wiederholung Klassen, Vererbung und Interfaces angeschaut. Da das zu großen Teilen ein Monolog meinerseits war hier jetzt nochmal eine entsprechende Aufgabe, damit ihr das auch anwenden könnt.

Der beiliegende Code ist meine Umsetzung. Guckt euch diese bitte nur an, wenn ihr fertig seid oder überhaupt nicht weiterkommt und schon die Ressourcen als Hilfe benutzt habt.

### 📝 Aufgabe:

Erstellt ein neues Projekt mit folgender Hierarchie:
- Interface: ITossable
- Klasse mit der Main-Methode
- Human:
  - Abstract: Human
    - Male
    - Female
- Nature:
  - Abstract: Fruit
    - Apple (ITossable)
    - Ananas
  - Rock (ITossable)
- Ball:
  - Abstract: Ball (ITossable)
    - Basketball

Erläuterung:
Erstellt selbst ein Interface eine "Main"-Klasse. Die darauffolgenden Ebenen sind packages also (Human, Nature, Ball). Dadrunter befinden sich abstrake Klassen und wiederum unter diesen die "Kinderklassen", welche von den abstrakten Klassen erben.

Das Interface ITossable soll Objekte "markieren" die (für unsere Menschen) werfbar sind. Beispielsweise einen Stein, Bälle jeglicher Art oder auch Früchte. Wobei eine Ananas zu schmeißen, vielleicht keine so gute Idee ist, mit den ganzen Spitzen und Blättern.
Heißt konkret, wir müssen den Menschen eine Methode toss(...) geben, die nur Objekte akzeptiert, die das Interface ITossable implementiert. Übersetzt Menschen sollen nur Objekte werfen, die sie auch wirklich werfen können (rein physisch).

Im Interface wird definiert, dass die Methode getTossed() implementiert werden muss. Die kann einfach einen String zurückgeben wie ("Der Apfel wurde geschmissen") oder ("Der Basketball fliegt und prallt mehrmals auf"). Sowas in die Richtung.

Ihr schreibt dann also eine Methode beim Menschen, die einfach die getTossed()-Methode des jeweiligen Objektes aufruft.

Zuletzt testet ihr das ganze am Besten. Also die Main-Klasse befüllen und ein zwei Menschen erstellen. Ein paar Früchte, Steine und Bälle erstellen und werfen was das Zeug hält.

Mit welchen Eigenschaften oder Methoden ihr eure Klassen füllt sei euch überlassen. Es geht mir bei dieser Aufgabe darum nicht, dass ihr super detaillierte Klassen mit vielen Methoden habt, sondern darum, dass ihr einmal diese Funktionsweise eines Interfaces umsetzt und auch eine Programmstruktur aufbaut, die sowas hergibt. Aber feel free euch da ein wenig auszutoben und euch ein bisschen was auszudenken.

Guckt auch in die Ressourcen, dort findet ihr ebenfalls die Aufgabe zu Interfaces des letzen Semesters, die eine ähnliche Struktur und ähnliche Klassen beinhaltet, wie wir sie hier haben.

Super als Übung ist es auch sinnvolle Konstruktoren zu erstellen, sowie Getter und Setter! Nutzt die Chance :)

Viel Spaß und Erfolg
    
### ℹ️ Resourcen:
Hier noch ein paar nützliche 📃Artikel, 🖊️Threads und 🎥Videos

- [🎥 Börges Seminar Video (Iterable)](https://www.ilias.uni-koeln.de/ilias/ilias.php?ref_id=3957251&eid=fb2c2032-8197-43cf-96a6-5f449ee76601&cmd=streamVideo&cmdClass=xoctplayergui&cmdNode=x2:p7:18a:18l&baseClass=ilrepositorygui)

- [📃 OOP, Klassen und Objekte (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/OOP-Klassen-und-Objekte.html)
- [📃 Objekte I: Initialisierung, Members, Zugriff (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/Objekte-I-Initialisierung-Members-Zugriff.html)
- [📃 Vererbung I: Grundlagen (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/Vererbung-I-Grundlagen.html)
- [📃 Vererbung II: Abstrakte Klassen und Methoden (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/Vererbung-II-Abstrakte-Klassen-und-Methoden.html)
- [📃 Vererbung III: Interfaces (Wegweiser)](https://dh-cologne.github.io/java-wegweiser/articles/Vererbung-III-Interfaces.html)
- [📃 Interfaces (extern)](https://www.programmierenlernenhq.de/interfaces-in-java/)

- [📝 Übungsaufgabe zu Interfaces und Vererbung WiSe20/21 - Beinhaltet einen ähnlichen Projektaufbau mit Menschen und co.](https://github.com/Demirro/04-02_Interfaces)

- [📃 Java Naming Conventions](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Naming-Conventions.md)
