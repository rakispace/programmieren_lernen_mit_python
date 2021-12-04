=================
Turtle-Bibliothek
=================

Begriff der Bibliothek
======================

Mit from <bibliothek> import <funktionen> können eine oder mehrere Funktionen einer Bibliothek eingebunden und somit im eigenen Code genutzt werden
Mehrere Funktionen können eingebunden werden, indem anstelle von <funktionen> explizit mehrere Funktionen durch Kommata getrennt aufgelistet werden
Steht anstelle von <funktionen> ein Sternchen (*), werden alle Funktionen der Bibliothek eingebunden
Mit from turtle import * kann die Turtle-Bibliothek eingebunden werden, um grafische Ausgaben in Python zu erzeugen

Turtle-Funktionen
=================

Im Folgenden findet Ihr eine Zusammenstellung aller Funktionen aus der Turtle-Bibliothek vor, die wir im Laufe des Kurses vorstellen werden. Eine allgemeine Funktionsübersicht gibt es beispielsweise hier auf Deutsch oder hier auf Englisch.
Bewegung

`forward(schritte)` bzw. `backward(schritte)` bewegt die Turtle um eine gewisse Schrittanzahl nach vorne bzw. nach hinten
Ist `penup()` zuvor nicht aufgerufen worden, wird dadurch eine Linie mit der Länge schritte gezeichnet
`goto(x, y)` bewegt die Turtle an den Bildpunkt (x, y)
Ist `penup()` zuvor nicht aufgerufen worden, wird dadurch eine Linie von dem aktuellen Punkt der Turtle zu dem Punkt (x, y) gezeichnet
Auf CodeOcean dürfen x und y höchstens 200 und kleinstens -200 sein
`speed(zahl)` beschleunigt oder verlangsamt die Bewegung der Turtle
zahl kann Wert von 0 bis 10 annehmen
0 bedeutet keine Animation, Turtle "springt" zum Zielpunkt
1 ist die langsamste und 10 ist die schnellste animierte Bewegung
wird eine Zahl größer als 10 angegeben, wird der Wert auf 0 gesetzt

Position
--------

`position()` gibt die aktuellen x- und y-Koordinaten zurück
`xcor()` bzw. `ycor()` geben x- bzw. y-Koordinate zurück
`setx(neuer_wert)` bzw. `sety(neuer_wert)` setzen die x- bzw. y-Koordinate der Turtle neu
Ist `penup()` zuvor nicht aufgerufen worden, wird dadurch eine Linie von dem aktuellen Punkt der Turtle zu dem neuen Punkt gezeichnet

Ausrichtung
-----------

`right(winkel)` rotiert die Turtle um einen bestimmten Winkel nach rechts
    winkel ist typischerweise eine ganze Zahl zwischen 0 und 360
`left(winkel)` rotiert die Turtle um einen bestimmten Winkel nach links
`setheading(winkel)` legt die Ausrichtung der Turtle fest
    `setheading(0)` steht für eine Ausrichtung nach rechts, `setheading(90)` Ausrichtung nach oben, `setheading(180)` Ausrichtung nach links, `setheading(270)` Ausrichtung nach unten
`direction (Woche 4)` gibt bei der Snake-Implementierung die Richtung des Schlangenkopfs an

Sichtbarkeit
------------

`penup()` hebt den Stift an, wodurch keine Linie mehr gezeichnet wird
`pendown()` setzt den Stift wieder ab, sodass eine Linie gezeichnet wird
`hideturtle()` versteckt die Form der Turtle

Form
----

`shape(string)` legt die Form der Turtle fest
Mögliche Formstrings sind: "turtle", "arrow", "circle", "square" , "triangle", "classic"
`register_shape(name_der_form, aufzaehlung_von_eckpunkten)` ermöglicht es, eine eigene Form zu definieren, die durch `shape(name_der_form)` angewendet werden kann

Farbe
-----

`pencolor(string)` setzt die Stiftfarbe der Turtle fest
Mögliche Farbstrings sind: "yellow", "blue", "red", "green", "orange"
`bgcolor(string)` setzt die Hintergrundfarbe des Bildschirmes fest
Mit `begin_fill()` und `end_fill()` werden Codezeilen "umrahmt", die eine Form zeichen, die anschließend farblich ausgefüllt werden soll
Füllfarbe ist schwarz, wenn man nicht zuvor mit fillcolor(string) eine andere Farbe festlegt

Weitere spannende Funktionen aus dem Forum
Position
--------

`home()` bewegt die Turtle zur Ausgangsposition (0, 0) und richtet sie in die Ausgangsorientierung aus
Ist `penup()` zuvor nicht aufgerufen worden, wird dadurch eine Linie von dem aktuellen Punkt der Turtle zu dem Punkt (0, 0) gezeichnet

Stiftdicke
----------

`pensize(zahl)` und `width(zahl)` setzen die Stiftdicke fest - also wie breit die Linie ist, die gemalt wird
zahl ist eine beliebige positive Zahl
desto größer zahl ist, desto breiter ist die Linie

Form
----

`circle(radius, winkel, schritte)` zeichnet einen Kreis, bei dem die aktuelle Position der Turtle den Startpunkt des Kreises bestimmt
radius muss angegeben werden und beschreibt den Radius des Kreises in Form einer Linksdrehung
winkel ist optional und bestimmt, welcher Teil des Kreises dargestellt wird (z.B. würde `circle(100, 180)` einen Halbkreis mit einem Radius von 100 zeichnen)
wenn winkel nicht gesetzt wird, wird der gesamte Kreis gezeichnet
schritte ist optional und gibt an, aus vielen Punkten die gezeichnete Kreislinie besteht

Farbe
-----

`colormode( 255 )` setzt die Einstellung, dass Farben nun nicht mehr nur als Farbstring, sondern auch als RGB Werte im Bereich von 0 bis 255 angegeben werden können
`fillcolor(252, 148, 3)` ermöglicht z.B. das die Füllfarbe nun orange ist
RGB steht für rot, grün, blau
RGB-Werte bestehen aus drei Zahlen, die durch Kommata getrennt sind

Alternativ zu einem Farbstring, kann man auch den Hexwert (Hexadezimale Farbdefinition) einer Farbe angeben
z.B. `fillcolor("#ff0000")` erzeugt eine rote Füllfarbe

Auf dieser englischen Wikipediaseite findet ihr die RGB Werte für viele Farben als Hexwert und als Dezimalzahl

Auf dieser Internetseite findet ihr einen Color picker (Farbwähler), bei dem ihr eine beliebige Farbe auswählen könnt und die RGB Werte als Hexwert und als Dezimalzahl erhaltet


