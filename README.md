# Michael Trauth Gedächnispreis 2026

## Aufgabe 

In einem digitalen Editionsvorhaben befinden sich die Positionsangaben `lb` (line begin), `pb` (page begin) oder `cb` (code begin) teilweise *ausserhalb* der übergeordneten Einheit (`ab`, `p`). 

Im folgenden Beispiel befinden sich die Zeilen 4-9 *innerhalb* des Textblocks (`ab`), Zeile 2 und 3 jedoch *ausserhalb*. 

1. Die erste Aufgabe besteht darin freistehende Positionsangaben *in* die dazugehörigen Textblöcke zu verschieben.

```xml
<lb n="2" xml:id="l-2"/>
<ab>
<supplied>Waarde</supplied> Theo,</ab>
<lb n="3" xml:id="l-3"/>
<ab>Dank voor je brief, <lb n="4" xml:id="l-4"/>het deed mij genoegen dat je <lb n="5" xml:id="l-5"/>weer goed aangekomen zijt. <lb n="6" xml:id="l-6"/>Ik heb je de eerste dagen ge<c type="shy">-</c>
<lb n="7" xml:id="l-7"/>mist &amp; het was mij vreemd <lb n="8" xml:id="l-8"/>je niet te vinden als ik s’mid<c type="shy">-</c>
<lb n="9" xml:id="l-9"/>dags t’huis kwam.</ab>
```
Quelle: https://github.com/eeditiones/vangogh/blob/master/data/let001.xml 




## Lösungen
