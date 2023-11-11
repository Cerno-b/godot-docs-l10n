# Stilregeln für die Übersetzung von Godot ins Deutsche

Originalautor: Cerno_b (cerno.b@gmail.com)

## Einleitung

Dieses Dokument soll dabei helfen, die deutsche Übersetzung von Godot, sowie
der Godot-Dokumentation, stilistisch zu vereinheitlichen. Dabei sollen
Lesbarkeit, Klarheit und Benutzbarkeit besonders im Vordergrund stehen.

Für die Übersetzung selbst ist das Tool 
[Weblate](https://hosted.weblate.org/projects/godot-engine/) im Einsatz, das in der
[offiziellen Dokumentation](https://docs.godotengine.org/de/4.x/contributing/documentation/editor_and_docs_localization.html) näher
erläutert wird. Die Bedienung von Weblate ist nicht Bestandteil dieses
Dokuments.

Weblate verfügt über ein Glossar, in dem häufig verwendete Begriffe gelistet
werden, damit sie einheitlich übersetzt werden können. In diesem Dokument
wird daher darauf verzichtet, die Übersetzung einzelner Begriffe zu
klären. Sollte es bei der Übersetzung eines Begriffs Uneinigkeit geben,
so sollte dies zunächst im  [Chatraum für die deutsche
Godot-Übersetzung](https://chat.godotengine.org/channel/translation-de) diskutiert und dann ins Glossar eingetragen werden.

## Technische Hilfsmittel

### Automatische Übersetzungen und Workflow

Die Erfahrung zeigt, dass eine Übersetzung von längeren Texten, z.B. aus der
Anleitung oder der Klassenreferenz oft zu schnelleren und besseren Ergebnissen
führt, wenn man den Originaltext von einer KI vorübersetzen lässt.

Ein sehr zu empfehlender Übersetzungsdienst ist hier die Website 
https://www.deepl.com, die hervorragende Erstübersetzungen zur Verfügung stellt 
und selbst Formatierungszeichen, wie Fettdruck oder Links in vielen Fällen
korrekt in die Übersetzung übernimmt.

Ein weiterer Vorteil dieser Art zu übersetzen ist, dass ein und derselbe Text
mit hoher Wahrscheinlichkeit strukturell wiederholt gleich übersetzt wird, was 
sehr hilfreich sein kann, wenn sich die Originaltexte leicht ändern und dann
die vorgenerierte Übersetzung immer noch dicht an der vorigen Übersetzung war.

Hier ist ein empfohlener Workflow für die Übersetzung eines Textblocks:

* Originaltext kopieren
* In DeepL übersetzen lassen
* In Übersetzungsfeld einfügen
* Text auf Abweichungen zum Glossar prüfen und ggf. korrigieren
* Eigene Änderungen vornehmen, wo sinnvoll


## Stilregeln

### Du oder Sie

Die aktuelle Übersetzung von Godot verwendet &bdquo;Sie&rdquo; statt &bdquo;Du&rdquo; bei direkter
Ansprache. Zwar wäre die freundlichere &bdquo;Du&rdquo;-Form im Gaming-Bereich ebenfalls
eine gute Wahl, jedoch ist eine Umstellung mit sehr viel Arbeit verbunden.
Die Diskussion einer Umstellung auf &bdquo;Du&rdquo; hängt daher in erster Linie an
der Frage, ob sich eine hinreichend große Menge an Freiwilligen finden,
um die *gesamte* Anleitung umzustellen. Bis dahin sollte aus
praktischen Gründen die Übersetzung beim formelleren &bdquo;Sie&rdquo; bleiben.

Beispiel:
> **Original:** You can also use the search function in the top-left corner.
>
> :x: Du kannst auch die Suchfunktion in der oberen linken Ecke verwenden.
>
> :heavy_check_mark: Sie können auch die Suchfunktion in der oberen linken Ecke verwenden.

### Grammatikalische Prinzipien

Die Godot-Übersetzung lässt sich in vier grobe Blöcke einteilen: *Editor*, 
*Properties*, *Anleitung* und *Klassenreferenz*.

Jeder dieser Blöcke hat eigene Ansprüche
an eine Übersetzung. Während die Anleitung in erster Linie auf Verständlichkeit
ausgelegt ist und sich angenehm lesen soll, ist im Editor und den Properties
häufig eine etwas knappere Sprache erforderlich, weil oft nur begrenzt
Platz für die Texte zur Verfügung steht.

Es ist daher sinnvoll, grammatikalische Grundregeln für die Übersetzung 
aufzustellen. Beachte, dass diese Regeln nicht absolut sind und im Zweifel 
mit Augenmaß übersetzt werden sollte. Trotzdem helfen solche Regeln, 
einen einheitlichen Sprachstil über die gesamte Dokumentation hinweg zu fördern.

Folgende Grundregeln werden aktuell in der Übersetzung angewendet: 

#### Anleitung/Klassenreferenz

In der Anleitung sollte die grammatikalische Form des Originaltexts beibehalten
werden, es sei denn die Lesbarkeit leidet darunter. Es sollte darauf verzichtet
werden, auf Zwang bestimmte Sprachkonstrukte, wie Passiv zu verwenden, wenn 
der Originaltext dies nicht auch tut. Insbesondere die direkte Ansprache mit 
"Sie" ist in diesem Teil der Dokumentation weit verbreitet.

Beispiele:
> **Original:** The table of contents in the sidebar should let you easily 
> access the documentation for your topic of interest.
> 
> :heavy_check_mark: Mithilfe des Inhaltsverzeichnisses in der Seitenleiste 
> können Sie leicht auf die Dokumentation zu Ihrem gewünschten Thema zugreifen. 
 
> **Original:**  To move our icon, we need to update its position and rotation 
> every frame in the game loop.
> 
> :heavy_check_mark: Um unser Icon zu bewegen, müssen wir seine Position und 
> Drehung in jedem Frame der Spielschleife aktualisieren. 

> **Original:** This build can be manually triggered by clicking the "Build" 
> button at the top right of the editor.
> 
> > :heavy_check_mark: Dieser Build kann manuell ausgelöst werden, indem man auf den
> &bdquo;Build&rdquo;-Button oben rechts im Editor klickt.


Bei manchen Abschnitten der Anleitung, wie bestimmten Überschriften oder Aufzählungen,
bietet sich der [Infinitiv-Imperativ](https://de.wikipedia.org/wiki/Imperativ_(Modus)#Infinitiv) an. 

> **Original:** Setting up the project
> 
> :heavy_check_mark: Das Projekt einrichten

> **Original:** For the player, we need to do the following:
> * Check for input.
> * Move in the given direction.
> * Play the appropriate animation.
> 
> :heavy_check_mark: Für den Spieler müssen wir Folgendes tun:
> * Auf Eingaben prüfen.
> * Sich in die angegebene Richtung bewegen.
> * Die entsprechende Animation abspielen.

#### Properties

Die *Properties* sind sehr knapp beschriebene Eigenschaften von Godot-Features,
die im Editor oft wenig Platz einnehmen. Hier handelt es sich oft um einzelne Begriffe,
bei denen die Schwierigkeit eher im Finden der korrekten Vokabel besteht (dazu mehr unten).

Manchmal sind es jedoch kurze Sätze, die in den meisten Fällen am besten
im Infinitiv-Imperativ (siehe Beispiele oben) zu übersetzen sind, da diese Form 
hier sprachlich gut passt und wenig Platz einnimmt. Auch sollten hier wo möglich, 
Artikel weggelassen werden, was aber oft bereits im Original so gemacht wird.

> **Original** Keep Screen On
>
> :x: Der Bildschirm wird eingeschaltet gelassen
> 
> :heavy_check_mark: Bildschirm eingeschaltet lassen

#### Editor

Die Texte des Editors bestehen sowohl aus kleinen Textblöcken, wenn z.B. ein Tooltip 
eine Einstellung näher beschreibt, als auch aus kurzen Begriffen, die oft wenig
Platz zur Verfügung haben.

Bei der Übersetzung des Editors gelten somit sowohl die Regeln für die Anleitung, als auch 
die für die Properties, je nachdem, ob der zu übersetzende Text eher Langform
oder Kurzform darstellt.

### Keine Angst vor englischen Begriffen

Manche Begriffe lassen sich nur schwer ins Deutsche übersetzen. Das sind zum
Beispiel technische Begriffe, die bereits in ihrer englischen
Form in den Sprachgebrauch Einzug gefunden haben (Thread, Debuggen,
Spawn-Punkt).

Andere Begriffe haben gängige deutsche Übersetzungen, wie z.B. *Knoten* für *node*. 
Da es in der Godot-Welt Objekte gibt, die feststehende Namen haben, 
etwa `Node2D`, wollen wir davon abgeleitete Vokabeln ebenfalls englisch lassen.

> **Original:** This feature is only available when connecting nodes in the editor.
> 
> :x: Dieses Feature ist nur verfügbar, wenn Knoten im Editor verbunden werden.
> 
> :heavy_check_mark: Dieses Feature ist nur verfügbar, wenn Nodes im Editor verbunden werden.

Du wirst beim Lesen der Anleitung vieler dieser absichtlich unübersetzen
Begriffe finden. Dies mag an der einen oder anderen Stelle etwas ungewohnt wirken,
aber es gibt viele Stellen, an denen damit Übersetzungsprobleme vermieden werden können.

Sollte es vorkommen, dass eine Regel unsinnig erscheint, sollte das im 
[Chat](https://chat.godotengine.org/channel/translation-de) diskutiert werden. Um einen Überblick über die dokumentierten Begriffe 
zu bekommen, die englisch bleiben sollen, lohnt sich ein 
Blick ins [Glossar](https://hosted.weblate.org/browse/godot-engine/glossary/de/). 
Sollte ein Begriff dort nicht hinterlegt sein, kann man die Suchfunktion
von Weblate zu verwenden, um Beispiele in den vorhandenen Übersetzungen zu finden.

Manchmal ist es auch notwendig, nach eigenem Empfinden eine Entscheidung zu
treffen oder von einer der Glossar-Regeln abzuweichen. 
Sprache ist zu komplex, als dass es für jeden Fall eine vordefinierte
Lösung gibt.

Beispiel 1:
> **Original:** Stereo Panning
>
> :x: Stereoverschiebung
>
> :heavy_check_mark: Stereo-Panning

Beispiel 2:
> **Original:** Drag to pan the view
>
> :x: Ziehen, um den View zu pannen.
>
> :heavy_check_mark: Ziehen um den View zu verschieben


Das Erste Beispiel stammt aus dem Audio-Bereich, wo Stereo-Panning ein gängiger
Begriff ist. Das zweite Beispiel verwendet das Wort &bdquo;panning&rdquo; als 
allgemeine Vokabel. Hier ist kein besonderer technischer Jargon
gemeint, somit kann das Wort auch normal auf Deutsch übersetzt werden.

Diese Unterscheidung wird im Glossar oft mit zwei Einträge desselben Wortes
abgebildet. Dabei soll ein Beschreibungstext dabei helfen, zu erklären,
in welchem Kontext welche Übersetzung passend ist.

Weiter unten findest Du Recherchetipps, die dabei helfen können,
eine passende Übersetzung zu finden, sollte ein Begriff weder im Glossar
noch in der bestehenden Dokumentation hinterlegt sein.

### Kompositionswörter

Das im deutschen übliche Aneinanderreihen von Wörtern (Komposition) wird
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
aufzubrechen und ihn klar zu beschreiben. Dabei ist es notwenig,
nachzulesen, was dieser Begriff im Kontext von Godot eigentlich genau bedeutet:

Beispiel:
> **Original:** Medium Quality Probe Ray Count
>
> :x: Mittelqualitätsprobestrahlenanzahl
>
> :heavy_check_mark: Strahlenzahl für Probes bei mittlerer Qualität

Es sollte bei der Übersetzung generell vermieden werden, überlange Komposita zu
erzeugen. Als Richtschnur sollten mehr als zwei Wörter nur in Ausnahmefällen zu
Komposita verbunden werden, mehr als drei Wörter hingegen am besten gar nicht.
Sollte sich keine brauchbare Übersetzung eines Kompositums finden, dann
sollten zumindest Bindestriche eingesetzt werden, um die Teilbegriffe klarer
voneinander zu trennen.

Beispiel 1:
> **Original:** Interaction Profile Path
>
> :x: Interaktionsprofilpfad
>
> :heavy_minus_sign: Interaktionsprofil-Pfad
>
> :heavy_check_mark: Pfad zum Interaktionsprofil

Beispiel 2:
> **Original:** Render Target Size Multiplier
>
> :x: Renderzielgrößenfaktor
>
> :heavy_minus_sign: Render-Zielgrößen-Faktor
>
> :heavy_check_mark: Faktor für Render-Zielgröße

### Schachtelsätze und &bdquo;die die&rdquo;-Wiederholungen

Beim direkten Übersetzen eines englischen Satzes kommt man leicht in
Versuchung, Schachtelsätze oder allgemein sehr lange Sätze zu bilden. Im
Allgemeinen ist es so, dass deutsche Wörter und Sätze statistisch länger
als ihre englischen Pendants sind. Daher sollte darauf geachtet werden,
die deutsche Übersetzung nicht zu komplex oder zu lang werden zu lassen. Es
kann durchaus guter Stil sein, einen Satz in zwei Sätze aufzuteilen, auch wenn
dabei die grammatikalische Form des Originals nicht erhalten bleibt.

Ein weiterer verwandter Aspekt ist hier die Verwendung der Wortwiederholung
&bdquo;die die&rdquo;, die ebenfalls vermieden werden sollte. Eine Ersetzung durch &bdquo;welche
die&rdquo; scheint oft naheliegend, klingt aber umständlich und ist keine gute Lösung.
Stattdessen ist eine Umformulierung des Satzes oft die bessere Wahl.

Beispiel 1:
> **Original:** Min SDK cannot be lower than %d, which is the version
> needed by the Godot library.
>
> :x: Min SDK kann nicht niedriger als %d sein, der Version, die die
> Godot-Bibliothek benötigt.
>
> :heavy_check_mark: Min SDK kann nicht niedriger als %d sein (die
> Version, die von der Godot-Bibliothek benötigt wird).

Beispiel 2:
> **Original:** In addition, one will need a primary GUI for their game that
> manages the various menus and widgets the project needs.
>
> :x: Außerdem benötigt man für sein Spiel eine primäre GUI, die die
> verschiedenen Menüs und Widgets verwaltet, die das Projekt benötigt.
>
> :heavy_check_mark: Außerdem benötigt man für sein Spiel eine primäre GUI,
> um die verschiedenen Menüs und Widgets des Projekts zu verwalten.
>
> :heavy_check_mark: Außerdem benötigt man für sein Spiel eine primäre GUI.
> Diese GUI verwaltet die verschiedenen Menüs und Widgets des Projekts.

### Eigene Ergänzungen

Achte bei der Übersetzung der Anleitung darauf, nur den Originaltext zu
übersetzen, ohne eigene Ergänzungen oder Erläuterungen vorzunehmen. Sollte
der Originaltext unvollständig oder erklärungswürdig sein, so beantrage zuerst
eine Änderung am Original oder stelle selbst einen Pull-Request in 
[godot-docs](https://github.com/godotengine/godot-docs). 
Wir sollten uns auf Weblate in erster Linie als Übersetzer und nicht als 
Autoren verstehen.

Beispiel:
> **Original**: Computes the arctan of x
>
> :x: Berechnet den Arcustangens von x. Der Arcustangens ist die Umkehrfunktion
> des Tangens.
>
> :heavy_check_mark: Berechnet den Arcustangens von x

## Konsistenz zwischen Editor/Properties und Anleitung

Wenn Du einen Begriff aus dem Editor oder den Properties änderst, solltest Du
die Weblate-Seite der Anleitung nach diesen Begriffen durchsuchen und sie 
entsprechend anpassen, damit die Übersetzungen konsistent bleiben.

Beachte auch, dass ein Editor/Property-Begriff meist an mehreren Stellen im Editor
oder den Properties vorkommt, sodass nach Möglichkeit alle dieser Stellen
mit übersetzt werden sollten.

## Testen der Übersetzung

Für Übersetzungen des Editors und der Properties ist es ratsam, diese 
auch selbst zu testen, indem 
man [die aktuelle Übersetzung herunterlädt](https://docs.godotengine.org/de/4.x/contributing/documentation/editor_and_docs_localization.html#offline-translation-and-testing) 
und Godot mit den Änderungen [selbst kompiliert](https://docs.godotengine.org/de/4.x/contributing/development/compiling/compiling_for_windows.html).

Gerade bei der Anleitung kommt es oft auf den Kontext zwischen benachbarten
Textblöcken an, sodass das Lesen eines ganzen Artikels Fehler sichtbar 
macht, die in Weblate leicht überlesen werden können.

## Recherchetipps

Grundsätzlich sollte man sich bei
der Übersetzung eines Begriffs gut überlegen, ob man eine korrekte
Übersetzung aus der eigenen Spracherfahrung vornehmen kann, oder besser erst
einmal etwas näher recherchieren sollte.

Die erste Quelle bei der Übersetzung feststehender Begriffe
sollte das Glossar und die bestehenden Übersetzungen in Weblate sein. 
Die Suchfunktion von Weblate leistet hier gute Dienste.

Wenn ein Begriff in diesen Quellen nicht gefunden werden kann oder Zweifel an 
ihrer Korrektheit bestehen, gibt es einige weitere hilfreiche Quellen:

Grundbegriffe aus der
Wissenschaft kann man auf der englischen [Wikipedia](https://www.wikipedia.org)
nachschlagen.
Von dort aus lässt sich über das Sprachmenü der deutsche
Schwesterartikel aufrufen, wo man oft eine korrekte deutsche Übersetzung des
Begriffs findet. Achte allerdings darauf, ob der deutsche Artikel auch
dieselbe Bedeutung des Wortes beschreibt, wie der englische Artikel.

Bei weiteren allgemeinen technischen Begriffen kann
man auf Webseiten wie www.linguee.com zurückgreifen, um zu schauen, wie
ein Begriff von anderen, oft professionellen, Übersetzern in unterschiedlichen 
Kontexten bereits übersetzt wurde.

Zuletzt gibt es Fachbegriffe, die direkt aus dem Gaming oder Game-Design
stammen, und es ist sicherlich nicht verkehrt, bei der Übersetzung einmal
nachzuschauen, wie andere Tools aus dem Bereich diese Begriffe übersetzen
(Unity, Unreal). Da diese Tools über das Budget für professionelle
Übersetzer verfügen, ist dies eine besonders hilfreiche Quelle für sehr
spezifische Fachbegriffe.

Zuletzt kann es hilfreich sein, sich an erfahrene Entwickler zu wenden, um
die Übersetzung eines Begriffs zu klären, entweder im [Chat](https://chat.godotengine.org/channel/translation-de) oder im
[deutschen Godot-Discord](https://discord.com/channels/553242711109533729/)


## Glossar-Regeln

Dieser Abschnitt befasst sich mit dem Glossar. Wenn Du einfach nur übersetzen 
möchtest, kannst Du ihn überspringen. Falls Du aber Glossar-Einträge pflegen 
möchtest, ist es ratsam, diesen Abschnitt zu lesen. 

Das Weblate-Glossar folgt bestimmten eigenen Regeln, die beachtet werden 
sollten:

### Was kommt überhaupt ins Glossar?

Das Glossar hat seinen praktischen Nutzen dort, wo man ein Wort an 
verschiedenen Stellen gleich übersetzen möchte. Immer, wenn das 
gewährleistet werden soll, lohnt sich auch ein Glossar-Eintrag. Beachte 
allerdings auch, dass ein sehr großes Glossar Pflegeaufwand bedeutet. Nicht 
jedes Wort muss also unbedingt einen Eintrag bekommen.

Beispiel:
> :x: color -> Farbe

Das Wort &bdquo;color&rdquo; ist ziemlich eindeutig und bedarf vermutlich keiner 
expliziten Klärung in einem Glossar. 

> :heavy_check_mark: ctrl -> Strg
 
Hier haben wir einen Fachbegriff, der über ein eindeutiges 
deutsches Äquivalent verfügt. Hier kann man durch eine &bdquo;Forbidden 
Translation&rdquo; (s.u.) außerdem darauf hinweisen, dass eine Übersetzung als das 
vielleicht naheliegende &bdquo;Ctrl&rdquo; nicht zulässig ist.

> :heavy_check_mark: aligned -> bündig/ausgerichet

In diesem Fall kann das Glossar dabei helfen, die verschiedenen 
Übersetzungen des Wortes &bdquo;aligned&rdquo; zu definieren, das in der Form 
*left-aligned* als *linksbündig* und in der Form *axis-aligned* als *an den 
Achsen ausgerichtet* übersetzt werden sollte.

> :heavy_check_mark: blitting -> Blitting

Hier verweist das Glossar darauf, dass ein Begriff ein 
feststehender Fachbegriff ist, der im Deutschen keine gute deutsche Entsprechung 
hat und daher englisch bleibt.

### Ein Wort, ein Eintrag

Da Weblate seine Glossar-Einträge bei der Übersetzung automatisch anbitet,
sobald im Originaltext ein Glossar-Begriff vorkommt, sollte 
sichergestellt werden, dass Einträge auch gefunden werden. Das kann nur 
gelingen, wenn ein Eintrag in der englischen Form genau so auch in einem 
Text vorkommen kann.

Beispiel:
> :x: float, floats
>
> :heavy_check_mark: float

Im vorigen Beispiel könnte Weblate den Glossareintrag das Wort nicht 
finden, da der Begriff *float, floats* so im Originaltext nicht vorkommen wird,
wenn dort lediglich der Begriff *float* beschrieben wird.

### Ein Wort, mehrere Bedeutungen

Sollte ein englisches Wort auf mehrere Arten übersetzt werden können, dann 
sollte für jede Übersetzung ein eigener Glossar-Eintrag angelegt werden. 
Dies hilft bei der Lesbarkeit und macht es später leichter, weitere Bedeutungen 
hinzuzufügen.

Beispiel:
> :x: Volumen, Lautstärke
>
> :heavy_check_mark: Volumen (*Translation Explanation:* im Sinne von &bdquo;Rauminhalt&rdquo;)
> 
> :heavy_check_mark: Lautstärke (*Translation Explanation:* im Audio-Kontext)

Es bietet sich an, über das jeweilige Explanation-Feld zu beschreiben, wie sich 
die verschiedenen Übersetzungen unterscheiden und in welchen Fällen man sie 
verwenden sollte.

### Grundformen verwenden

Ein englisches Wort sollte grundsätzlich in seiner einfachsten Form ins 
Glossar eingetragen werden, damit es in möglichst vielen Fällen automatisch 
zugeordnet werden kann. Das bedeutet bei Verben die Grundform (**wichtig:** ohne *to*) 
und bei Substantiven der Singular.

Beispiel 1:
> :x: to hide -> verbergen
> 
> :heavy_check_mark: hide -> verbergen

Beispiel 2:
> :x: constants -> Konstanten
> 
> :heavy_check_mark: constant -> Konstante

Leider unterstützt die aktuelle Version von Weblate keine 
morphologischen Varianten. Wenn also ein Wort im Glossar als Singular angegeben wird, dann
wird es beim Übersetzen nur angeboten, wenn auch im Übersetzungstext der Singular 
verwendet wird. Es gibt bereits ein [Ticket](https://github.com/WeblateOrg/weblate/issues/3023)
dazu im Weblate-Github. Bis zur Lösung dieses Problems sollten wir vermeiden, 
als Workaround Singular *und* Plural-Einträge im Glossar zu erzeugen, da das
schlecht zu warten ist.

### Terminology

Ein als &bdquo;Terminology&rdquo; markierter Eintrag wird automatisch in allen 
anderen Sprachen in die Glossare eingetragen und führt dort zu offenen 
Arbeitspaketen. 

Das kann dazu führen, dass neue Glossareinträge in der deutschen
Übersetzung erscheinen, weil eine andere Sprache sie eingefügt hat. In diesem
Fall ist es legitim, das Terminology-Flag zu entfernen und den Eintrag zu löschen, 
wenn er aus unserer Sicht nicht sinnvoll ist. Dieser Vorgang lässt den Eintrag
in allen anderen Sprachen unverändert.

Wir sollten das Terminology-Flag grundsätzlich nicht setzen, da es potentiell
die Glossare anderer Sprachen zumüllt, insbesondere, wenn diese andere Definitionen 
davon haben, welche Art von Begriffen als &bdquo;Terminologie&rdquo; zu bewerten sind. 


### Untranslatable

Ein als &bdquo;Untranslatable&rdquo; markierter Eintrag ist ein Begriff, der bewusst nicht 
übersetzt werden soll, z.B. feststehende Begriffe wie `Android` oder `OpenGL`.
Allerdings haben viele dieser Begriffe eigentlich nichts im Glossar verloren,
sodass dieses Flag nicht allzu häufig vorkommen sollte. 
Man kann einen als *untranslatable* markierten Begriff daran 
erkennen, dass er bei der Glossar-Einblendung gelb hinterlegt ist.

### Forbidden Translation

Ein als &bdquo;Forbidden Translation&rdquo; markierter Eintrag kann dazu verwendet 
werden, um eine Übersetzung aufzuzeigen, die nicht verwendet werden soll, zum 
Beispiel weil sie einen fehleranfälligen 
[Falschen Freund](https://de.wikipedia.org/wiki/Falscher_Freund) darstellt 
oder um bestimmte deutsche Begriffe zu sperren. Zum Beispiel könnte man sich 
darauf einigen, den Begriff *enemy* durchgängig als *Gegner* und nicht als das 
extremere *Feind* zu übersetzen.

## Änderungen an diesem Dokument

Änderungen an diesem Dokument sollten im [Chat](https://chat.godotengine.org/channel/translation-de) diskutiert und nach 
Klärung per Pull-Request ins Github-Repo committet werden. 