=====================
Fehlerarten in Python
=====================

Beim Programmieren können verschiedene Fehler auftreten. Seien es Schreibfehler im Code,
fehlerhafte Eingabe durch den Nutzer oder Fälle, die nicht abgedeckt wurden.
Im Folgenden wollen wir Euch einen kurzen Überblick über typische Fehler in Python geben,
die beim Schreiben Eurer Programme auftreten könnten.

SyntaxError
Der vermutlich am häufigsten auftretende Fehler ist der Syntaxfehler.
Ein Syntaxfehler tritt auf, wenn ein Verstoß gegen den "Satzbau" von Python auftritt.
Das heißt, der Quellcode konnte nicht verarbeitet und in das fertige Programm umgewandelt werden.
Ein Syntaxfehler ist zum Beispiel eine vergessene schließende Klammer oder ein vergessener Doppelpunkt.

NameError
Ein Namensfehler tritt meistens auf, wenn eine Variable verwendet wurde,
der zuvor kein Wert zugewiesen wurde. Dieser Fehler kann aber auch dadurch auftreten,
dass eine Funktion verwendet wird, die nicht definiert oder dessen Funktionsname falsch geschrieben wurde.
In diesem Fall wird nach einer Funktion gesucht, die nicht gefunden werden kann.

IndentationError
Ein Einrückungsfehler sagt aus, dass eine Zeile falsch eingerückt wurde - also zu viele
oder zu wenige Tabs verwendet wurden. Diese treten vor allem bei Kontrollstrukturen wie Verzweigungen
oder Schleifen oder bei der Definition von Funktionen auf.
Hier ist wichtig darauf zu achten, dass manchmal mehrere Einrückungen nötig sind, da
verschiedene Konstrukte ineinander verschachtelt sein können.

ValueError
Ein ValueError tritt auf, wenn eine Operation oder Funktion ein Argument gegeben bekommt,
das einen korrekten Typ hat, aber einen inkorrekten Wert.
Dies kann zum Beispiel der Fall sein, wenn man int("ein_string") aufruft.
Die Funktion int() erwartet einen String oder eine Zahl. Übergibt man der Funktion int() einen String,
muss sie diesen in eine ganze Zahl verwandeln können, was mit ein_string nicht möglich ist.

TypeError
Bei einem TypeError wurde einer Operation oder einer Funktion ein Argument mit einem
falschen Datentypen übergeben. Dies tritt beispielsweise auf, wenn einer Funktion wie input(),
die einen String erwartet, ein Integer mitgegeben wird.

ImportError
Ein Fehler beim Importieren tritt auf, wenn die importierte Bibliothek falsch geschrieben wurde
oder nicht existiert. Auch wenn nach dem from <bibliotheksname> import explizit Funktionsnamen aufgeführt werden,
die nicht existieren oder falsch geschrieben wurden, wird ein ImportError ausgelöst.
(Mehr zu Imports erfahrt Ihr am Ende von Woche 1 und in Woche 2.)

Wenn Ihr Euer Programm ausführt und nicht die typische grüne Ausgabe erscheint,
sondern ein orangener Text, ist ein Fehler aufgetreten. In der untersten Zeile der Ausgabe könnt Ihr immer sehen,
welcher Fehler an welcher Stelle aufgetreten ist.

