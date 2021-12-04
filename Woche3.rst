=======================
Zusammenfassung Woche 3
=======================

Funktionen
==========

Zerlegen Probleme in Teilprobleme
Vorteile von Funktionen:
    Keine Codedopplung
    Wiederverwendbarkeit in anderen Programmen
    Code wird verständlicher und übersichtlicher
    Leichtere Pflege und Wartung des Codes

Funktionen ohne Parametern
--------------------------

Funktionsdefinition
-------------------

.. code-block:: console
   def funktions_name():
       # Anweisungen

Der Inhalt der Funktion muss eingerückt sein
Reine Definition, es wird nichts ausgeführt

Funktionsaufruf
---------------

.. code-block:: console
   funktions_name()

Durch den Funktionsaufruf wird eine Funktion ausgeführt
Eine Funktion kann mehrfach aufgerufen werden

Rückgabewert
------------

Mit return wird der Rückgabewert festgelegt
Der Rückgabewert kann weiterverwendet werden
Gibt eine Funktion einen Wert zurück, so wird die Ausführung innerhalb der Funktion mit der Rückgabe 
von return rueckgabewert beendet.

Funktionen mit Parametern
-------------------------

.. code-block:: console
   def funktions_name(aufgelistete_parameter):
       # Anweisungen

Bei der Funktionsdefinition können in Klammern mit Kommata getrennt Parameter mitgegeben werden
Diese werden beim Funktionsaufruf durch tatsächliche Werte, die sogenannten Argumente, ersetzt
Der Funktionsaufruf muss die gleiche Anzahl an Argumenten und die gleiche Reihenfolge der Argumente verwenden, 
wie es in der Funktionsdefinition angegeben ist

Dictionaries
============

Sind wie Wörterbücher
Bestehen aus Schlüssel-Werte-Paaren
Werden durch geschweifte Klammern erzeugt, in denen verschiedene Schlüssel-Werte-Paare durch Kommata 
sowie Schlüssel und ihre Werte durch einen Doppelpunkt getrennt sind
Beispiel: `hauptstaedte = {"Deutschland":"Berlin", "Österreich": "Wien", "Tschechien":"Prag" }`
Werte ändern oder hinzufügen: `dictionary[schlüssel] = neuer_Wert`
Wertpaare werden in einer Schleife nach der Reihenfolge des Hinzufügens zum Dictionary durchlaufen

Funktionen auf Dictionaries
---------------------------

    `dictionary.keys()` gibt alle Schlüssel zurück
    `dictionary.values()` gibt alle Werte zurück
    `dictionary.items()` gibt alle Schlüssel und Werte zurück

Zufallszahlen
=============

Können durch die Bibliothek `random` erzeugt werden
`random()` gibt zufällige Zahl zwischen 0 (eingeschlossen) und 1 (ausgeschlossen) zurück
`randint(start, ende)` gibt zufällige ganze Zahl zwischen start und ende zurück (beide eingeschlossen)


