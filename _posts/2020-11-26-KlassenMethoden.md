---
layout: post
title: "Klassen und Methoden"
date: 2020-11-26 12:00:00 -0000
categories: java wise basics
excerpt_separator: <!--more-->
---
Ohne und Klassen und Methoden kommen wir bei Java nicht weit.
<!--more-->

[Link zum Repository](https://github.com/Demirro/26-11_Klassen_Methoden)

# 26-11_Klassen_Methoden
Übungsaufgabe für das Programmierpraktikum im Wise 20/21 für den 26.11.2020

# Willkommen bei der dritten Übungsaufgabe.

Ihr findet im Download wieder eine Vorlage. Es geht diesmal um Klassen und Methoden. Es liegen zwei Klassen vor. Einmal *Application* und einmal *Konto*. In *Application* befindet sich die Main-Methode und ein paar Sachen die ich da eingebaut habe. Ihr sollt in *Konto* jetzt Konstruktoren und Methoden einbauen, damit die *Application*-Klasse funktioniert.

### 📝 Aufgabe:

Stellt euch vor ihr programmiert ein rudimentäres Banksystem. Ihr fangt an die Struktur für Bankkonten zu bauen. Das ist eure Klasse *Konto*. Dort sind drei Instanzvariablen (*id, name, kontostand*) mit drei **Gettern**, zwei **Konstruktoren** und zwei zusätzlichen **Methoden/Fähigkeiten** einzubauen.

#### Eure spezifischen Aufgaben sind:
- Baut Getter für die drei Instanzvariablen *id, name, kontostand*
- Erstellt zwei Konstruktoren
  - Ein Konstruktor soll als Argumente eine ID und einen Namen annehmen
  - Der andere Konstruktor soll als Argumente eine ID, einen Namen und den Kontostand annehmen
  - **Wichtig:** Es sollten dennoch alle Instanzvariablen gesetzt werden. Heißt beim ersten Konstruktor sollte automatisch ein Wert für den Kontostand gesetzt werden.
- Programmiert zwei Methoden (*einzahlen, auszahlen*)
- Einzahlen (braucht keinen Rückgabewert/return):
  - nimmt als Argument einen int an
  - fügt den gegebenen Betrag dem Kontostand hinzu
  - Gibt auf der Konsole einen Text aus, der auf den Erfolg der Transaktion und auf den neuen Kontostand hinweist
- Auszahlen (braucht keinen Rückgabewert/return):
  - nimmt als Argument einen int an
  - zieht den gegebenen Betrag dem Konto ab
  - es sollte geprüft werden, ob genug Geld auf dem Konto ist
    - Wenn ja: Betrag abziehen, Erfolgsnachricht und Kontostand ausgeben
    - Wenn nein: Fehlermeldung
  

## Tipps
- In diesem Projekt werden keine Setter benutzt. Die Setter sind deswegen aber quasi Teil der Konstruktoren
- Ihr könnt von einem Konstruktor einen anderen Konstruktor aufrufen

- Im Projekt befindet sich eine Zip, welche meine Musterlösung beinhaltet
    
### ℹ️ Resourcen:
Hier noch ein paar nützliche 📃Artikel, 🖊️Threads und 🎥Videos

- [🎥 Aufzeichnung des Seminars](https://www.ilias.uni-koeln.de/ilias/ilias.php?ref_id=3638292&eid=458d2edf-ddf9-48bd-be52-331242cf4681&cmd=streamVideo&cmdClass=xoctplayergui&cmdNode=wn:os:17u:185&baseClass=ilrepositorygui)
- [📃 Methoden (Wegweiser)](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Methoden.md)
- [📃 Klassen und Objekte (Wegweiser)](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/OOP-Klassen-und-Objekte.md)
- [📃 Objekte (Wegweiser)](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Objekte-I-Initialisierung-Members-Zugriff.md)

- [📃 Java Naming Conventions](https://github.com/DH-Cologne/java-wegweiser/blob/master/articles/Naming-Conventions.md)


### P.S. Global Variablen in Java
**an diejenigen aus dem letzten Zoom-Meeting und an die, die es interessiert**

Es gibt keine direkte globale Variable in Java. Beziehungsweise nicht explizit. In der letzten Übungsstunde hatten wir uns ja lokale Variablen, Instanz- und Klassenvariablen angeguckt. Klassenvariablen (private static int variable;) sind ja Variablen, die für alle Instanzen/Objekte einer Klasse gleich sind. Da diese aber private sind, können sie nur über Getter/Setter aufgerufen werden und auch nur, wenn man ein Objekt der Klasse erstellt hat.

Um eine globale Variable zu "simulieren" kann man eine Klasse erstellen, beispielsweise die Klasse *Globals*. In dieser Klasse erstellt man eine Klassenvariable, nur macht man diese public. Also:
```java
public class Globals {
public static int globalSize = 20;
}
```
Die Variable *globalSize* ist jetzt überall im Code abrufbar, auch ohne eine Instanz zu erstellen. Beispiel:
```java
System.out.println(Globals.globalSize);
```
Es gibt noch eine zweite Methode, aber dafür braucht man Sachen aus Java, die ihr noch nicht kennt.
Mehr dazu hier:
- [📃 Variablen - Gültigskeitsbereiche](http://java-latte.blogspot.com/2014/01/global-variable-vs-class-variable-vs.html)
