=======================
Zusammenfassung Woche 1
=======================

Zeitaufwand: etwa 3 Minuten

Erstes Programmierbeispiel
==========================

Textausgabe
-----------

Textausgabe wird über die Funktion `print()` erzeugt,
in deren runde Klammern man den auszugebenen Text in Anführungsstrichen schreibt
`print("Hallo")` gibt den Text "Hallo" aus
Jeder Aufruf von `print()` erzeugt eine neue Zeile in der Konsolenausgabe
Mehrere Wörter - mit einem Leerzeichen getrennt - können ausgegeben werden,
indem man sie durch Kommata getrennt in der Funktion print() aufzählt
`print(“Hallo”, “du”, "da")` gibt "Hallo du da" auf einer Zeile aus

Kommentare
----------

Texte im Code, die nicht ausgeführt werden
Dienen dazu, komplizierte Textstellen zu erklären, sodass diese verständlicher sind

Einzeilige Kommentare beginnen mit einem Hashtag (#) und gehen bis zum Ende der Zeile

.. code-block:: python
    # Das ist ein einzeiliger Kommentar 

Mehrzeilige Kommentare beginnen und enden mit drei Anführungszeichen derselben Art (""" oder ''')

.. code-block:: python
    """ Das ein 
        mehrzeiliger Kommentar """

Abarbeitung von Anweisungen
---------------------------

Codezeilen werden in Python der Reihe nach von oben beginnend ausgeführt
Jede Anweisung sollte in eine eigene Zeile geschrieben werden
Kommentare werden bei der Ausführung übersprungen

Variablen
=========

Name für einen Wert, den man später noch einmal benötigt

Verwendung von Variablen
------------------------

Variable wird mit dem Gleichheitszeichen (=) ein Wert zugewiesen, der sich später noch ändern kann

.. code-block:: python
    kleidung = "T-Shirt"

Wert einer Variable kann verwenden werden, indem man an die Stelle, 
an die man eigentlich den gewünschten Wert schreiben würde, den Namen der Variable schreibt
Achtung: Wert der Variable muss zuvor gesetzt sein

Benennung von Variablen
-----------------------

In Python: kleingeschrieben und mit Unterstrichen, wenn sie aus mehreren Wörtern bestehen
- Sollten keine Umlaute enthalten
- Dürfen keine Sonderzeichen enthalten
- Sollten möglichst aussagekräftig sein
- Groß- und Kleinschreibung beachten

String
======

Zeichenkette, also eine Folge von Buchstaben und/oder anderen Zeichen
In Python mit einfachen (') oder doppelten (") Anführungszeichen geschrieben

Operationen auf Strings
-----------------------

Verkettung von Strings mit Plusoperator (+)
- Ergibt neuen String
Z- wischen den Strings wird nicht automatisch ein Leerzeichen eingefügt
Wiederholung von Strings mit Maloperator (*)
- Ergibt neuen String
- Zahl, mit der der String multipliziert wird, gibt an, wie häufig der String wiederholt wird
- len() gibt die Anzahl an Zeichen eines Strings (inklusive der Leer- und Sonderzeichen) zurück

Platzhalter
-----------

Lücke in einem String, die durch eine Variable ersetzt wird
Nur im Zusammenhang mit einem F-String möglich, der durch ein f oder F vor dem String gekennzeichnet wird
Durch geschweifte Klammern im F-String dargestellt, in der Variablenname steht

Beispiel, das "Stella singt gerne." ausgibt:

.. code-block:: python
   person = "Stella"	
   satz = f"{person} singt gerne."	
   print(satz)	

Datentypen
==========

Geben an, von welcher Art die Daten sind und welche Operationen damit durchgeführt werden können

String
------

Stellt Text dar und wird in Anführungszeichen geschrieben
Siehe weiter oben

Integer
-------

Stellt ganze Zahlen dar, mit denen gerechnet werden kann
Bei Division von Integern kann Float herauskommen
z.B. 42

Float
-----

Abkürzung für "floating point number"
Stellt (Gleit-)Kommazahlen dar, mit denen gerechnet werden kann
Wird mit einem Punkt dargestellt, z.B. 4.2

Boolean
-------

Stellt den Wahrheitswert True oder False dar
Wird vor allem für Verzweigungen genutzt


