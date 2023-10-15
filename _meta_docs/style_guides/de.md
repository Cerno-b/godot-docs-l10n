# Stilregeln für die Übersetzung von Godot ins Deutsche

## Einleitung

Dieses Dokument soll dabei helfen, die deutsche Übersetzung von Godot, sowie
der Godot-Dokumentation, stilistisch zu vereinheitlichen. Dabei sollen
Lesbarkeit, Klarheit und Benutzbarkeit besonders im Vordergrund stehen.

Für die Übersetzung selbst ist das Tool Weblate im Einsatz, das in der
[offiziellen Dokumentation](https://docs.godotengine.org/de/4.x/contributing/documentation/editor_and_docs_localization.html) näher
erläutert wird. Die Bedienung von Weblate ist nicht Bestandteil dieses
Dokuments.

Weblate verfügt über ein Glossar, in dem häufig verwendete Begriffe gelistet
werden, damit sie einheitlich übersetzt werden können. In diesem Dokument
wird daher darauf verzichtet, die Übersetzung einzelner Begriffe zu
klären. Sollte es bei der Übersetzung eines Begriffs Uneinigkeit geben,
so sollte dieser Begriff ins Glossar eingetragen und die
Weblate-Kommentarfunktion verwendet werden, um zu einer Einigung zu kommen.
Weiterführende Diskussionen können aber auch im [Chatraum für die deutsche
Godot-Übersetzung](https://chat.godotengine.org/channel/translation-de) geklärt werden.


## Stilregeln

### Du oder Sie

Die aktuelle Übersetzung von Godot verwendet "Sie" statt "Du" bei direkter
Ansprache. Zwar wäre die freundlichere "Du"-Form im Gaming-Bereich ebenfalls
eine gute Wahl, jedoch ist eine Umstellung mit viel Arbeit verbunden.
Die Diskussion einer Umstellung auf "Du" hängt daher in erster Linie an
der Frage, ob sich eine hinreichend große Menge an Freiwilligen finden,
um die *gesamte* Übersetzung umzustellen. Bis dahin sollte aus
praktischen Gründen die Übersetzung beim formelleren "Sie" bleiben.

Beispiel:
> **Original:** Press button a
>
> :x:: Drücke Taste a
>
> :heavy_check_mark:: Drücken Sie Taste a


### Übersetzen oder Original lassen?

Manche Begriffe lassen sich nur schwer ins Deutsche übersetzen. Das sind zum
Beispiel technische Begriffe, die bereits in ihrer englischen
Form in den Sprachgebrauch Einzug gefunden haben (Thread, Debuggen,
Spawn-Punkt).

Es ist im Einzelfall zu prüfen, ob ein Begriff eine gebräuchliche deutsche
Übersetzung hat oder ob er in seiner englischen Form in der Fachsprache
akzeptiert ist.

Beispiel 1:
> **Original:** Stereo Panning
>
> :x:: Stereoverschiebung
>
> :heavy_check_mark:: Stereo-Panning

Beispiel 2:
> **Original:** Drag to pan the view
>
> :x:: Ziehen um den View zu pannen.
>
> :heavy_check_mark:: Ziehen um den View zu verschieben


Das erste Beispiel stammt aus dem Audio-Bereich, wo Stereo-Panning ein gängiger
Begriff ist. Das zweite Beispiel verwendet das Wort "panning" als normale
Vokabel in einem allgemeinen Satz. Hier ist kein besonderer technischer Jargon
gemeint, somit kann das Wort auch normal auf Deutsch übersetzt werden.

Diese Unterscheidung kann im Glossar durch zwei Einträge desselben Wortes
abgebildet werden, jeweils mit einer Beschreibung, in welchen Fällen
welche Übersetzung verwendet werden sollte.

Am Ende dieses Dokuments findest Du Recherchetipps, die dabei helfen sollen,
eine passende Übersetzung zu finden. Beachte bitte, dass Ergebnisse solcher
Recherchen sehr wertvoll sind und daher in einem Glossareintrag dokumentiert
werden sollten.

### Kompositionswörter

Das im Deutschen übliche Aneinanderreihen von Wörtern (Komposition) wird
im Englischen üblicherweise durch das Hintereinandersetzen von Wörtern mit
Leerzeichen erreicht. Bei sehr langen Wortfolgen ergeben sich dabei
logische Untergruppen aus dem Zusammenhang, auch wenn das in Extremfällen
manchmal wenig intuitiv erscheint:

> Default Font Multichannel Signed Distance Field

Im Deutschen sollte dagegen vermieden werden, lange Kompositionen zu bilden,
da die Lesbarkeit extrem leidet, wenn die Wörter sehr lang werden. Eine
einfache Lösung ist hier, mithilfe von Bindestrichen Klarheit zu schaffen.
Allerdings ist es im Allgemeinen besser, die grammatikalische Struktur des
Begriffs
aufzubrechen und ihn klar zu beschreiben. Dabei ist es notwendig,
nachzulesen, was dieser Begriff im Kontext von Godot eigentlich genau bedeutet:

Beispiel:
> **Original:** Medium Quality Probe Ray Count
>
> :x:: Mittelqualitätssondenstrahlenanzahl
>
> :heavy_check_mark:: Strahlenzahl für Sonden bei mittlerer Qualität

Es sollte bei der Übersetzung generell vermieden werden, überlange Komposita zu
erzeugen. Als Richtschnur sollten mehr als zwei Wörter nur in Ausnahmefällen zu
Komposita verbunden werden, mehr als drei Wörter hingegen am besten gar nicht.
Sollte sich keine brauchbare Übersetzung eines Kompositums finden, dann
sollten zumindest Bindestriche eingesetzt werden, um die Teilbegriffe klarer
voneinander zu trennen.

Beispiel 1:
> **Original:** Interaction Profile Path
>
> :x:: Interaktionsprofilpfad
>
> :heavy_minus_sign:: Interaktionsprofil-Pfad
>
> :heavy_check_mark:: Pfad zum Interaktionsprofil

Beispiel 2:
> **Original:** Render Target Size Multiplier
>
> :x:: Renderzielgrößenfaktor
>
> :heavy_minus_sign:: Render-Zielgrößen-Faktor
>
> :heavy_check_mark:: Faktor für Render-Zielgröße

### Schachtelsätze und "die die"-Wiederholungen

Beim direkten Übersetzen eines englischen Satzes kommt man leicht in
Versuchung, Schachtelsätze oder allgemein sehr lange Sätze zu bilden. Im
Allgemeinen ist es so, dass deutsche Wörter und Sätze statistisch länger
als ihre englischen Pendants sind. Daher sollte darauf geachtet werden,
die deutsche Übersetzung nicht zu komplex oder zu lang werden zu lassen. Es
kann durchaus guter Stil sein, einen Satz in zwei Sätze aufzuteilen, auch wenn
dabei die grammatikalische Form des Originals nicht erhalten bleibt.

Ein weiterer verwandter Aspekt ist hier die Verwendung der Wortwiederholung
"die die", die ebenfalls vermieden werden sollte. Eine Ersetzung durch "welche
die" scheint oft naheliegend, klingt aber umständlich und ist keine gute Lösung.
Stattdessen ist eine Umformulierung des Satzes oft die bessere Wahl.

Beispiel 1:
> **Original:** Min SDK cannot be lower than %d, which is the version
> needed by the Godot library.
>
> :x:: Min SDK kann nicht niedriger als %d sein, der Version, die die
> Godot-Bibliothek benötigt.
>
> :heavy_check_mark:: Min SDK kann nicht niedriger als %d sein (die
> Version, die von der Godot-Bibliothek benötigt wird).

Beispiel 2:
> **Original:** In addition, one will need a primary GUI for their game that
> manages the various menus and widgets the project needs.
>
> :x:: Außerdem benötigt man für sein Spiel eine primäre GUI, die die
> verschiedenen Menüs und Widgets verwaltet, die das Projekt benötigt.
>
> :heavy_check_mark:: Außerdem benötigt man für sein Spiel eine primäre GUI,
> um die verschiedenen Menüs und Widgets des Projekts zu verwalten.
>
> :heavy_check_mark:: Außerdem benötigt man für sein Spiel eine primäre GUI.
> Diese GUI verwaltet die verschiedenen Menüs und Widgets des Projekts.

### Eigene Ergänzungen

Achte bei der Übersetzung der Anleitung darauf, nur den Originaltext zu
übersetzen, ohne eigene Ergänzungen oder Erläuterungen vorzunehmen. Sollte
der Originaltext unvollständig oder erklärungswürdig sein, so beantrage zuerst
eine Änderung am Original. Wir sollten uns an dieser Stelle in erster
Linie als Übersetzer und nicht als Autoren verstehen.

Beispiel:
> **Original**: Computes the arctan of x
>
> :x:: Berechnet den Arcustangens von x. Der Arcustangens ist die Umkehrfunktion
> des Tangens.
>
> :heavy_check_mark:: Berechnet den Arcustangens von x

## Recherchetipps

Insbesondere Fachbegriffe aus dem mathematischen und physikalischen Bereich
haben oft gängige deutsche Übersetzungen.

Grundsätzlich sollte man sich bei
der Übersetzung eines Fachbegriffs gut überlegen, ob man eine korrekte
Übersetzung aus der eigenen Spracherfahrung vornehmen kann, oder besser erst
einmal etwas näher recherchieren sollte.

Grundbegriffe aus der
Wissenschaft kann man auf der englischen [Wikipedia](www.wikipedia.org)
nachschlagen.
Von dort aus lässt sich über das Sprachmenü der deutsche
Schwesterartikel aufrufen, wo man oft eine korrekte deutsche Übersetzung des
Begriffs findet. Achte allerdings darauf, ob der deutsche Artikel auch
dieselbe Bedeutung des Wortes beschreibt wie der englische Artikel.

Bei weiteren allgemeinen technischen Begriffen kann
man auf Webseiten wie www.linguee.com zurückgreifen, um zu schauen, wie oft
ein Begriff von anderen Übersetzern in unterschiedlichen Kontexten bereits
übersetzt wurde.

Zuletzt gibt es Fachbegriffe, die direkt aus dem Gaming oder Game-Design
stammen, und es ist sicherlich nicht verkehrt, bei der Übersetzung einmal
nachzuschauen, wie andere Tools aus dem Bereich diese Begriffe übersetzen
(Unity, Unreal). Da diese Tools über das Budget für professionelle
Übersetzer verfügen, ist dies eine besonders hilfreiche Quelle für sehr
spezifische Fachbegriffe.

Zuletzt ist es für Texte der Dokumentation oft nicht verkehrt, sich das
Original zunächst von dem sehr guten Übersetzungsdienst www.deepl.com
vorübersetzen zu lassen. Achte darauf, dass diese Übersetzung nicht
immer perfekt ist, und betrachte sie mehr als eine Rohübersetzung,
die nochmal überarbeitet werden muss.
