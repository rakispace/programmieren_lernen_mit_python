=======================
Zusammenfassung Woche 2
=======================

Verzweigungen
=============

Dadurch werden gewisse Programmzeilen nur unter bestimmten Bedingungen ausgeführt
Bedingungen können Vergleiche und Boolsche Aussagenlogik enthalten

.. code-block:: console
   if Bedingung:
      Aktion1
   else:
      Aktion2

Aktion1 wird ausgeführt, wenn die Bedingung wahr ist
Aktion2 wird ausgeführt, wenn die Bedingung falsch ist

.. code-block:: console
   if Bedingung1:
       Aktion1.1
       Aktion1.2
       ...
   elif Bedingung2: 
       Aktion2.1 
       ...
   elif Bedingung3:
       Aktion3.1 
        ...
   else: 
       ...

Bedingungen werden nacheinander geprüft
Erster Zweig, bei dem die Bedingung wahr ist, wird ausgeführt
Nachfolgende Bedingungen werden nicht mehr geprüft

Vergleiche
==========

Sind entweder True (wahr) oder False (falsch):
    a < b (a ist kleiner als b)
    a <= b (a ist kleiner oder gleich b)
    a > b (a ist größer als b)
    a >= b (a ist größer oder gleich b)
    a == b (a ist gleich b)
    a != b (a ist ungleich b)

Boolsche Aussagenlogik
----------------------

`and` ist wahr, wenn beide damit verknüpfte Aussagen wahr sind
`or` ist wahr, wenn mindestens eine der damit verknüpften Aussagen wahr ist

Daten importieren
=================

Mit `from <datei> import <name>` können nicht nur Funktionen, sondern auch Variablen aus einer Datei eingebunden werden
Wenn damit Variablen eingebunden werden, wurden ihnen in datei Werte zugewiesen, die man abfragen kann

Schleifen
=========

Zum mehrfachen Ausführen von Aktionen

For-Schleifen
-------------

Laufen für jedes Element variable der übergebenen Aufzählung die Schleife einmal durch

.. code-block:: console
    for variable in aufzaehlung:
      Aktion1
      Aktion2
      ...

`range(n)` gibt eine Aufzählung von 0 bis n-1 zurück

`range(start, ende, wert)` gibt Werte von start bis ende - 1 in Schritten der Größe wert zurück
    start ist optional und wird standardmäßig auf 0 gesetzt
    ende muss angegeben werden
    wert ist optional und wird standardmäßig auf 1 gesetzt

While-Schleifen
---------------

Wiederholen Aktionen so lange, wie die übergebene Bedingung erfüllt ist

.. code-block:: console
    while bedingung:
      Aktion1
      Aktion2
      ...

Listen
======

Fassen eine Menge an Daten zusammen
Elemente der Liste werden in eckigen Klammern und durch Kommata getrennt geschrieben
Können unterschiedliche Datentypen und weitere Listen enthalten
Beispiel: `haus = [[2, 4], "gelb", "Tür"]`
Können mit Plusoperator (+) kombiniert und mit Maloperator (*) vervielfacht werden
Iterieren über Listen z.B. mit einer For-Schleife möglich

Index
-----

Beschreibt eindeutige Position eines Elements in einer Liste
Beginnt bei 0 (Index des ersten Elements) und endet bei len(liste) - 1 (Index des letzten Elements)
Bei negativer Indexierung beschreibt die -1 das letzte Element, die -2 das vorletzte Element usw.
Mithilfe des Index' kann man auf Elemente zugreifen und sie verändern

Funktionen auf Listen
---------------------

`len(liste)` gibt die Anzahl an Elementen zurück
`liste.append(element)` fügt Element zur Liste hinzu
`liste.pop()` entfernt das letzte Element einer Liste und gibt es zurück
`liste.pop(index)` entfernt Element mit bestimmten Index aus einer Liste und gibt es zurück
`"trennzeichen".join(liste)` fügt die einzelnen Elemente einer Liste, getrennt durch das Trennzeichen, zu einem String zusammen
`string.split()` teilt einen String an den Leerzeichen in einzelne Elemente auf und gibt diese als Elemente einer neuen Liste zurück
Verschachtelte Indexierung: Zugriff auf Zeichen von Strings in einer Liste oder Elemente einer inneren Liste
Slicing: Zugriff auf bestimmte Elemente einer Liste mit Liste[<Startindex> : <Endindex>], wobei der Endindex nicht mit extrahiert wird


