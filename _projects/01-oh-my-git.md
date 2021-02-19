---
layout: project
title: "Oh My Git!"
image: /assets/images/project_images/oh-my-git/thumbnail.png
authors:
  - author: blinry
    link:
  - author: bleeptrack
    link:
brief: "Wir erschaffen einen spielerischen Zugang zum Lernen von Git."
summary: "Das Lernspiel bietet eine interaktive Einführung in das Versionskontrollsystem Git, und ermöglicht so souveräne und effiziente Zusammenzuarbeit beim Programmieren."
---

# Wir erschaffen einen spielerischen Zugang zum Lernen von Git.

Wenn man im Team Software entwickelt, steht man vor einem Problem: Wie tauscht man den Quelltext untereinander aus? Klar, eine Möglichkeit wäre, ihn auf USB-Sticks oder per E-Mail hin- und her zu schicken, aber es gibt eine bessere Möglichkeit: Sogenannte "Versionskontrollsysteme"! Das sind kleine Hilfprogramme, welche die Zusammenarbeit an beliebigen Textdateien über das Internet erleichtern.

Ein solches Programm, das über die letzten Jahre sehr populär geworden ist, heißt "Git". Es wurde 2005 von Linus Torvalds entwickelt, der auch den Linux Kernel initiierte, und wird heute von einer großen Community gepflegt und weiterentwickelt. Es ist momentan der absolute Standard für Softwareentwicklung im Team, und das Kernstück hinter der Plattform "GitHub".

Git hat allerdings den notorischen Ruf, eine steile Lernkurve zu haben. Es beinhaltet einige abstrakte Konzepte, an die man sich erstmal gewöhnen muss. Wir haben deshalb ein **Lernspiel entwickelt, das die Funktionsweise von Git interaktiv und intuititv begreifbar macht**. Wir möchten damit insbesondere Menschen in Ausbildung oder Quereinsteiger\*innen einen leichteren Zugang zur Softwareentwicklung ermöglichen.

## Download

Das Spiel ist im Wesentlichen fertig und benutzbar, und steht auf folgender Seite für Linux, macOS und Windows zum Download bereit:

[blinry.itch.io/git-hydra](https://blinry.itch.io/git-hydra)

## Trailer

<div class="iframe-container">
    <iframe src="https://www.youtube-nocookie.com/embed/1iOnNcOU0X8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

## Features

### Visualisierung des Git-Projektes

Oh My Git! stellt die internen Strukturen eines Git-Projektes visuell und in Echtzeit dar. Die Auswirkungen von Interaktionen damit sind sofort grafisch sichtbar:

<video src="/assets/images/project_images/oh-my-git/repository.mp4" autoplay muted loop></video>

## Spielkarten-Interface

Um Menschen den Einstieg in Git zu erleichtern, stellt das Spiel ein eigens hierfür konzipiertes Interface bereit, um mit Git zu interagieren: Spielkarten! Diese zeigen neben dem Git-Befehl auch eine kurze Beschreibung, sowie ein passendes Icon, und sind so Aktion und Dokumentation in einem.

<video src="/assets/images/project_images/oh-my-git/cards.mp4" autoplay muted loop></video>

## Eingebautes Terminal

Für fortgeschrittenere oder neugierige Spieler\*innen steht aber auch ein richtiges Terminal zur Verfügung, in dem beliebige Befehle ausgeführt werden können. In das Spiel ist ein "echtes" Git eingebaut, wodurch sämtliche Features von Git ausprobiert und erlernt werden können.

<video src="/assets/images/project_images/oh-my-git/terminal-git.mp4" autoplay muted loop></video>

## Entwicklungsgeschichte

Wir haben das Spiel iterativ entwickelt, und über die Projektlaufzeit insgesamt sechs Prototypen entwickelt:

### Prototyp 0

![](/assets/images/project_images/oh-my-git/prototype-0.png)

Dies war eine allererste **technische Machbarkeitsstudie**, die wir vor der Bewerbung entwickelten. Der Fokus lag auf der Visualisierungs-Komponente, es gab schon ein erstes Terminal, aber keinerlei Inhalte.

### Prototyp 1

![](/assets/images/project_images/oh-my-git/prototype-1.png)

Wir entwickelten ein einfaches **Levelformat**, mit Beschreibungen und Zielen, wählten eine hübsche Schriftart aus, und gaben den UI-Elementen ein einheitliches Theme. Außerdem gab es hier schon einen ersten einfachen **Dateibrowser**. Eine erste Levelsequenz erklärte die Funktionsweise von Git, angefangen bei den Internals - was recht ungewöhnliche Befehle erforderte, die im Alltag kaum zur Anwendung kommen.

Wir luden zwei erfahrene Git-Benutzer zum ersten Playtest ein. Beide hatten in diesem Stadium das Problem, dass sie Befehle, die eingeführt und erklärt wurden, schnell wieder vergaßen, da es keine gute Möglichkeit gab, diese nachzuschlagen. Einer der beiden fragte nach dem Test: "Was ist eigentlich eure Zielgruppe?" - was uns ziemlich zum Nachdenken brachte, und schließlich entscheiden ließ, nicht mit den Internals anzufangen, sondern mit den Standardbefehlen, die man im alltäglichen Umgang mit Git die ganze Zeit benutzt.

### Prototyp 2

![](/assets/images/project_images/oh-my-git/prototype-2.png)

Wir schrieben eine Levelsequenz, die eine **High-Level-Einführung** in Git darstelle. Wir versuchten hier bereits, ganz am Anfang zu motivieren, weshalb Git überhaupt nützlich ist, mit einer kleinen Geschichte über Aufsätze, die man schreiben sollte. Ohne Git musste man dort unzählige Kopien des Essays anlegen, die dann teilweise wieder versehentlich gelöscht wurden - und dann wurde gezeigt, wie Git dabei helfen kenn.

Außerdem entwickelten wir das Levelformat weiter - während vorher die einzelnen Komponenten wie Beschreibung, Zielsetzung, und Initialisierungs-Skript in einzelenen Dateien vorlagen, konnten sie nun in **einer einzigen Datei** untergebracht werden.

In diesen Zeitraum fiel auch unserer erstes **Coaching**. Wir sprachen darin viel über "visuellere" User Interfaces, und waren danach recht überzeugt, dass diese Leuten, die noch wenig Erfahrung mit Git oder der Kommandozeile hatten, sehr helfen würden.

### Prototyp 3

![](/assets/images/project_images/oh-my-git/prototype-3.png)

Das Interface, das uns am reizvollsten erschien, waren **Spielkarten**! Die verschiedenen Befehle auf eigenen Karten zu haben, mit Icons und Beschreibungen, fühlte sich sehr gut an - so hatten die Befehle quasi eine eingebaute Dokumentation!

Desweiteren fügten wir einen **grafischen Datei-Browser** hinzu. zu diesem Zeitpunkt erklärte das Spiel nichts über den Index, sodass eine reine Darstellung der aktuellen Dateiinhalte ausreichte.

Außerdem spielten wir hier zum ersten Mal mit der Idee einer **"Zeitreise"-Thematik!** Das bot sich als Analogie sehr an: Commits sind "Snapshots" von Objekten zu einem Zeitpunkt, branches sind "Zeitleisten", und mit dem HEAD kann man dann durch die Zeit reisen.

Unsere playtests hierzu waren sehr motivierend, beides schien gut anzukommen! Teilweise waren die Zielstellungen der Levels nicht ganz klar

### Eine Sackgasse: "2D-Welt"

![](/assets/images/project_images/oh-my-git/prototype-2d.png)

Hier verfolgten wir für eine Weile die Idee, die Dateien als richtige **Objekte in einer 2D-Welt** zu haben. Reizvoll daran war, dass drei Stufen von Dateiinhalten - Datei im working directory, Datei im Index, und Datei im aktuellen commit - sehr gut grafisch darstellbar waren, nämlich als weiße Datei, als blaue "Aura", und als grauer Schatten. Für uns selbst war diese Form der Darstellung sehr augenöffnend, um beispielsweise zu verstehen, dass `git reset` sehr wörtlich das Gegenteil von `git add` ist.

Wir dachten lange darüber nach, wie man **2D-Schiebepuzzle mit Türen** und Schaltern konstruieren könnte, und zwar so, dass man über die Kommandozeile nicht zu sehr "cheaten" könnte - fanden letztendlich aber keine Konfiguration von Regeln, die rund klang, und generell schien diese Richtung den Fokus von dem eigentlichen Lernhinhalt - Git selbst - wegzunehmen.

Nach einigen Wochen verwarfen wir die Änderungen in diesem branch komplett.

### Prototyp 4

![](/assets/images/project_images/oh-my-git/prototype-4.png)

Hier begann dann eine Phase des Feinschliffs. Auf das Feedback einer sehbehinderten Person hin machten wir hier alle **Texte größer**. Wir veränderten das **Bildschirm-Layout**, fügten eine **Levelübersicht** hinzu, sowie eine klarere **Aufschlüsselung der Ziele** als rote und grüne Boxen unter der Levelbeschreibung.

Wir machten viele kleine Verbesserungen im User Interface und polierten viele der Levels. Und wir fanden einen Weg, die Vorteile der "drei Dateiversionen" aus unseren 2D-Experimenten auch hier unterzubringen: Als **Dateiicons in mehreren "Schichten"**. Wenn diese exakt aufeinanderliegen, sind die Inhalte identisch, wenn die Position voneinander abweicht, sind sie unterschiedlich.

Auch die Playtests für diese Version bestätigten uns, dass wir auf einem guten Weg waren. Wir testeten hier unter anderem mit einer Person völlig ohne Git-Vorkenntnisse, und die Analogien, Hilfestellungen, und Strukturen, die wir uns überlegt hatten, schienen größtenteils zu funktionieren! Eine andere Testperson war wild entschlossen, den Umgang mit der Kommandozeile zu lernen, und die Karten nur als Dokumentation zu benutzen.

### Prototyp 5

![](/assets/images/project_images/oh-my-git/prototype-5.png)

Um die Kommandozeilen-Benutzung mehr zu motivieren bauten wir golden glitzernde **"Terminal-Abzeichen"** ins Spiel ein, die man bekommt, wenn man ein Level ohne die Spielkarten löst.

Die Level inhaltlich wirklich rund und vollständig zu haben, war zeitaufwändiger, als wir dachten, hier floss viel Polierarbeit hinein. Denn mittlerweile gab es viele Level zu verschiedensten Themen, mit deutlich über einer Stunde Gesamtspielzeit - und hier selbst den Überblick zu behalten, fiel uns nicht immer leicht. Um den Einstieg zu erleichtern, fügten wir an bestimmte Interfaceelemente kleine, einmalig angezeigte **"Hints"** an.

Unser Freund [winniehell](https://winniehell.de) produzierte außerdem einen **Soundtrack** für dieses Spiel!

Diese Version des Spiels stellten wir in einem 15-minütigen Vortrag auf Europas größter Open Source-Konferenz vor, der FOSDEM:

<iframe width="863" height="485" src="https://www.youtube.com/embed/mTxpLX8wh0A" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Danke!

Dieses Projekt im Rahmen des Prototype Funds umzusetzen, hat uns enorm viel Spaß gemacht, und wir haben jede Menge über remote-Zusammenarbeit, Selbstorganisation und die Spieleengine Godot gelernt - und nicht zuletzt auch viel über Git selbst!

Wir bedanken uns herzlich beim _Bundesministerium für Bildung und Forschung_ für die Förderung, und beim ganzen Prototype Fund-Team für die tolle Unterstützung!

## Zukunft und Links

Wir sind am Ende dieses Projektes insbesondere an Kontakt zu Menschen interessiert, die ein solches Spiel aktiv in der Lehre benutzen möchten, oder anderweitig Multiplikatorfunktion haben könnten!

Und auch Feedback zum Spiel selbst ist stets sehr willkommen, und hilft uns, es besser zu machen! Vielen Dank für's Lesen! :)

- [Downloadseite auf itch.io](https://blinry.itch.io/oh-my-git)
- [Projekt auf GitHub](https://github.com/git-learning-game/oh-my-git)

- bleeptrack: [Homepage](http://bleeptrack.de), [Twitter](https://twitter.com/bleeptrack)
- blinry: [Homepage](https://morr.cc), [Twitter](https://twitter.com/blinry)
