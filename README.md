# Michael Trauth Gedächnispreis 2025

In einem digitalen Editionsvorhaben sind Positionsangaben `lb` (line begin) und `pb` (page begin) teilweise *ausserhalb* der übergeordneten Blockeinheit (`ab`) gesetzt. 
Zudem sind Leerzeilen (`<vg:whiteline/>`) *ausserhalb* der dadurch nach unten abgesetzten Textblöcke positioniert.

Im folgenden Beispiel befinden sich die meisten Zeilen- und Seitenanfänge *innerhalb* des Textblocks (`ab`), ausserhalb - *vorangestellt* – befinden sich jedoch die Zeilen 1, 2, 3, 10, 15, 27 und 28 sowie - *nachgestellt* – drei Leerzeilen. 

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

Download als XML-Datei: https://raw.githubusercontent.com/eeditiones/vangogh/refs/heads/master/data/let001.xml 

Download als TUSTEP-Datei [let001.tf](https://github.com/ITUG/mtr_preisaufgabe_2025/blob/main/let001.tf)

## Aufgabe 
1. Verschiebe die freistehende Positionsangaben (Zeilen 1,2,3,10,15,27,28) *in* die dazugehörigen <ins>nachstehenden</ins> Textblöcke.
2. Verschiebe die nachgestellten Leerzeilen *in* die dazugehörigen <ins>vorstehenden</ins> Textblöcke.
3. Dokumentiere/überprüfe die vorgenommenen Änderungen (vorher/nachher).

Gearbeitet werden kann mit dem untenstehenden Textbeispiel oder einem oder mehreren oder allen Texten, die im van Gogh Repositiorum bereitgestellt werden: https://github.com/eeditiones/vangogh/tree/master/data

Diese Aufgabe darf/soll/kann mit parametergesteuerten TUSTEP-Modulen, TUSCRIPT oder im Editor gelöst werden. 

Auch Teillösungen zu 1, 2 oder 3 sind willkommen !

## Quelle
Textgrundlage sind die unter Creative Commons Attribution, NonCommercial, ShareAlike 4.0 International (CC BY-NC-SA 4.0) Lizenz bereitgestellten van Gogh Letters. 

* [teiPublisher Demo](https://teipublisher.com/exist/apps/vangogh/index.html)

* https://vangoghletters.org 


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
### Elke Zinsmeister
```bash
#-        Routine für Preisfrage, Tustep-Workshop 2025, Elke Zinsmeister

#-        Anlegen der Ziel- und einer Hilfsdatei
#DATEI,
 name = ziel,
 typ = seq-ap

#DATEI,
 name = vg1,
 fragen = -

#KOPIERE,
 quelle = let001.tf,
 ziel = vg1,
 loeschen = +,
 parameter = *
par       {}

          - Zeichengruppe mit den Zeichen, die in <lb> vorkommen können
>tg       ~ ~{\a}~{&0}~:~=~"~-~/~

          - neue Einteilung des Texts: Sätze beginnen bei <div und </ab
aa        ~<div~</ab~

          - <ab> wird vor <lb> gezogen
xx    1   ~<lb{00}{Z:tg}>{|} <ab>~{=2=}{=1=}~

          - <ab rend="indent"> wird vor <lb> gezogen
xx    2   ~<lb{00}{Z:tg}>{|} <ab rend="indent">~{=2=}{=1=}~

          - <ab> wird vor <pb> gezogen
xx    3   ~<pb */> {|} <ab>~{=2=}{=1=}~

          - <vg:whiteline/> wird vor </ab> gezogen
xx    4   ~</ab> {|}<vg:whiteline/>~{=2=}{=1=}~
*eof


#KOPIERE,
 quelle = vg1,
 ziel = ziel,
 modus = +,
 loeschen = +,
 parameter = *
par       {}
          - neue Einteilung des Texts: Sätze beginnen bei <div und </ab und </div
aa        ~<div>~<ab~</div~
za        ~<div>~<ab~</div~

          - Autauschen der Codierung für Apostroph
xx    1   ~#\[2019\]~#\[92\]~
*eof


#-        Kontrolle durch Vergleich mit vg_ziel, der Zieldatei von TK, mit Ergebnis im Ablaufprotokoll

#ANMELDE,
 lesen = vg_ziel

#VERGLEICHE,
 versiona = vg_ziel,
 versionb = ziel,
 protokoll = +

#-        - Kontrolle durch Dateienvergleich in oxygen:
#-        - Dateien vg_ziel und ziel über ez,(+1,-1) in gleichnamige in oxygen neu erstellte
#-        - XML-Dateien kopiert. Versuch, Dateien mit "Dateien vergleichen" zu vergleichen scheitert,
#-        - Fehlermeldung: "Fehler gefunden in ...\vg_ziel.xml: Cannot parse document.
#-        - Vergleiche mit Syntax-bewusst"

```

### Christian Sonder

Die Lösung von Christian Sonder liegt im Unterverzeichnis [mt_preis_cs](https://github.com/ITUG/mtr_preisaufgabe_2025/tree/main/mt_preis_cs)
Auszuführen sind die dort abgelegten `*.pr` Dateien, z.B. mit `#tue,preisaufgabe.pr`
### Thomas Kollatz (ausser Konkurrenz)

