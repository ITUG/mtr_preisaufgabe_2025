# Michael Trauth Gedächnispreis 2026

## Aufgabe 

In einem digitalen Editionsvorhaben befinden sich die Positionsangaben `lb` (line begin), `pb` (page begin) oder `cb` (code begin) teilweise *ausserhalb* der übergeordneten Einheit (`ab`, `p`). 
Zudem sind Leerzeilen (`<vg:whiteline/>`) ausserhalb der dadurch freigestellten Textblöcke positioniert.


Im folgenden Beispiel befinden sich die Zeilen 4-9 *innerhalb* (`ab`), Zeile 1, 2, 3, 10, 15, 27 und 28 und drei Leerzeilen jedoch *ausserhalb* des Textblocks. 

1. Verschiebe die freistehende Positionsangaben (Zeilen 1,2 und 3) *in* die dazugehörigen nachstehenden Textblöcke zu verschieben.
2. Verschiebe die nachgestellten Leerzeilen *in* die dazugehörigen vorstehenden Textblöcke.
3. Überprüfe die vorgenommenen Änderungen (Dokumentation, Beleg vorher/nachher, etc.)

Textgrundlage sind die unter Creative Commons Attribution, NonCommercial,   ShareAlike 4.0 International (CC BY-NC-SA 4.0) Lizenz bereitgestellten van Gogh Letters. 

Gearbeitet werden kann mit dem untenstehenden Textbeispiel oder einem oder mehreren oder allen Texten, die im van Gogh Repositiorum bereitgestellt werden: https://github.com/eeditiones/vangogh/tree/master/data

Diese Aufgabe darf/soll/kann mit parametergesteuerten TUSTEP-Modulen, TUSCRIPT oder im Editor gelöst werden. 

```xml
<div type="original" xml:lang="nl">
<pb f="1r" n="1" xml:id="pb-orig-1r-1" facs="#zone-pb-1r-1"/>
<lb n="1" xml:id="l-1"/>
<ab>
<supplied>Den Haag, 29 september 187</supplied>2.</ab>
<vg:whiteline/>
<lb n="2" xml:id="l-2"/>
<ab>
<supplied>Waarde</supplied> Theo,</ab>
<lb n="3" xml:id="l-3"/>
<ab>Dank voor je brief, <lb n="4" xml:id="l-4"/>het deed mij genoegen dat je <lb n="5" xml:id="l-5"/>weer goed aangekomen zijt. <lb n="6" xml:id="l-6"/>Ik heb je de eerste dagen ge<c type="shy">-</c>
<lb n="7" xml:id="l-7"/>mist &amp; het was mij vreemd <lb n="8" xml:id="l-8"/>je niet te vinden als ik s’mid<c type="shy">-</c>
<lb n="9" xml:id="l-9"/>dags t’huis kwam.</ab>
<lb n="10" xml:id="l-10"/>
<ab rend="indent">Wij hebben prettige dagen sa<c type="shy">-</c>
<lb n="11" xml:id="l-11"/>men gehad, en tusschen de <lb n="12" xml:id="l-12"/>droppeltjes door<anchor n="a" xml:id="note-o-a"/> toch nog al <lb n="13" xml:id="l-13"/>eens gewandeld &amp; het een en <lb n="14" xml:id="l-14"/>ander gezien.</ab>
<lb n="15" xml:id="l-15"/>
<ab rend="indent">Wat vreesselijk weer, je zult <lb n="16" xml:id="l-16"/>het wel <hi rend="ital">benauwd</hi> hebben <lb n="17" xml:id="l-17"/>op je wandelingen naar <lb n="18" xml:id="l-18"/>Ois<supplied>ter</supplied>wijk.<anchor n="1" xml:id="note-o-1"/> Gisteren is het hard<c type="shy">-</c>
<lb n="19" xml:id="l-19"/>draverij geweest ter gelegenheid van <lb n="20" xml:id="l-20"/>de tentoonstelling,<anchor n="2" xml:id="note-o-2"/> maar de illumi<c type="shy">-</c>
<lb n="21" xml:id="l-21"/>natie &amp; het vuurwerk zijn uit <lb n="22" xml:id="l-22"/>gesteld, om het slechte weer,<anchor n="3" xml:id="note-o-3"/> het <lb n="23" xml:id="l-23"/>is dus maar goed dat je niet <lb n="24" xml:id="l-24"/>gebleven zijt om die te zien. Groeten <lb n="25" xml:id="l-25"/>van de familie Haanebeek<anchor n="4" xml:id="note-o-4"/> &amp; Roos.<anchor n="5" xml:id="note-o-5"/> <lb n="26" xml:id="l-26"/>Steeds</ab>
<vg:whiteline/>
<lb n="27" xml:id="l-27"/>
<ab>je liefh.</ab>
<lb n="28" xml:id="l-28"/>
<ab>Vincent</ab>
<vg:whiteline/>
</div>
```
Quelle: https://github.com/eeditiones/vangogh/blob/master/data/let001.xml, Zeile 76-101

## Ziel
```xml
<div type="original" xml:lang="nl">
<ab><pb f="1r" n="1" xml:id="pb-orig-1r-1" facs="#zone-pb-1r-1"/>
<lb n="1" xml:id="l-1"/>
<supplied>Den Haag, 29 september 187</supplied>2.<vg:whiteline/></ab>
<ab><lb n="2" xml:id="l-2"/>
<supplied>Waarde</supplied> Theo,</ab>
<ab><lb n="3" xml:id="l-3"/>Dank voor je brief, <lb n="4" xml:id="l-4"/>het deed mij genoegen dat je <lb n="5" xml:id="l-5"/>weer goed aangekomen zijt. <lb n="6" xml:id="l-6"/>Ik heb je de eerste dagen ge<c type="shy">-</c>
<lb n="7" xml:id="l-7"/>mist &amp; het was mij vreemd <lb n="8" xml:id="l-8"/>je niet te vinden als ik s’mid<c type="shy">-</c>
<lb n="9" xml:id="l-9"/>dags t’huis kwam.</ab>
<ab rend="indent"><lb n="10" xml:id="l-10"/>Wij hebben prettige dagen sa<c type="shy">-</c>
<lb n="11" xml:id="l-11"/>men gehad, en tusschen de <lb n="12" xml:id="l-12"/>droppeltjes door<anchor n="a" xml:id="note-o-a"/> toch nog al <lb n="13" xml:id="l-13"/>eens gewandeld &amp; het een en <lb n="14" xml:id="l-14"/>ander gezien.</ab>
<ab rend="indent"><lb n="15" xml:id="l-15"/>Wat vreesselijk weer, je zult <lb n="16" xml:id="l-16"/>het wel <hi rend="ital">benauwd</hi> hebben <lb n="17" xml:id="l-17"/>op je wandelingen naar <lb n="18" xml:id="l-18"/>Ois<supplied>ter</supplied>wijk.<anchor n="1" xml:id="note-o-1"/> Gisteren is het hard<c type="shy">-</c>
<lb n="19" xml:id="l-19"/>draverij geweest ter gelegenheid van <lb n="20" xml:id="l-20"/>de tentoonstelling,<anchor n="2" xml:id="note-o-2"/> maar de illumi<c type="shy">-</c>
<lb n="21" xml:id="l-21"/>natie &amp; het vuurwerk zijn uit <lb n="22" xml:id="l-22"/>gesteld, om het slechte weer,<anchor n="3" xml:id="note-o-3"/> het <lb n="23" xml:id="l-23"/>is dus maar goed dat je niet <lb n="24" xml:id="l-24"/>gebleven zijt om die te zien. Groeten <lb n="25" xml:id="l-25"/>van de familie Haanebeek<anchor n="4" xml:id="note-o-4"/> &amp; Roos.<anchor n="5" xml:id="note-o-5"/> <lb n="26" xml:id="l-26"/>Steeds<vg:whiteline/></ab>
<ab><lb n="27" xml:id="l-27"/>je liefh.</ab>
<ab><lb n="28" xml:id="l-28"/>Vincent<vg:whiteline/></ab>
</div>
```





## Lösungen
