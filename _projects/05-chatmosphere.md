---
layout: project
title: "Chatmosphere"
image: /assets/images/project_images/chatmosphere/packshot-header.png
authors:
  - author: Anke Riemer
    link:
  - author: Kai Berthold
    link:
  - author: David Grieshammer
    link:
brief: "Der Open Source Video-Chat für informelle Unterhaltungen"
summary: ""
---

# Chatmosphere

### Live-Demo

[https://demo.chatmosphere.cc/](https://demo.chatmosphere.cc/)

Ihr seid sichtbar und könnt euch im Raum frei bewegen - eigentlich alles so wie damals, als wir uns noch in Kneipen treffen konnten. Es gilt also nach wie vor: [Be excellent to each other](https://github.com/Chatmosphere/chatmosphere-app/blob/master/docs/CODE_OF_CONDUCT.md).

Wir bitten euch den Einladungslink an einem Laptop oder Computer in Chrome zu öffnen, da unser Prototyp noch nicht auf allen Browsern stabil läuft. Mobile Phones oder Touch Devices sind auch nicht geeignet (da würdet ihr eh auch kaum jemanden sehen).

**Disclaimer**: Je nach Menge an Besucher:innnen kann es zu Bandbreitenproblemen auf unserem Demoserver kommen. Bisher hatten wir den Punkt noch nicht erreicht, aber das kann ja noch kommen.

Wir freuen uns auf euch!

### Idee

Die Idee zu Chatmosphere hat ihren Ursprung in der Zeit des ersten Corona-Lockdowns im Frühjahr 2020. Durch das Distanzierungsgebot erlangten damals virtuelle Zusammenkünfte, insbesondere Videokonferenzen, einen neuen Stellenwert.

So haben wir etwa das regelmäßig stattfindende Plenum der genossenschaftlichen Bar, in welcher wir Mitglieder sind, durch Video-Calls ersetzt. Schnell wurde das Bedürfnis nach informellem Austausch immer größer, was um schließlich dazu bewogen hat, eine virtuelle Bar ins Leben zu rufen. Vom Feierabendbier bis zur Geburtstagsfeier sind immer mehr Events im virtuellen Raum getestet worden. Durch diese zunehmende Verlagerung privater Treffen in den digitalen Raum wurden dann aber auch die Unzulänglichkeiten der etablierten Software-Lösungen schmerzhaft offensichtlich:

- Aktuelle Video-Call-Tools sind für den Arbeitskontext konzipiert und optimiert
- Informelle Gesprächsdynamik ist nicht vorgesehen, erschwert oder unmöglich
- Die Nutzung der bestehenden Tools hat viele Hürden: Kosten, Datensicherheit, Einrichtungs- / Bedienungsprobleme (vor allem für Menschen ohne Technik-Affinität)

Chatmosphere tritt daher seit September 2020 dafür an, einen informellen und dynamischen Austausch in im digitalen Raum zu ermöglichen. Wir wollen Probleme und Potenziale von Video-Chats explorieren und haben ein Tool entwickelt, dass technische und interaktive Hürden abbaut und eine sowohl inklusive als auch organische virtuelle Kommunikation ermöglicht.

Wir bauen auf der Open-Source-Software Jitsi auf und bieten eine Interface, dass zusammen mit einer Jitsi-Instanz dezentral gehostet werden kann. 
Die Anleitung für das Set-up findet sich [unserem GitHub-Repository](https://github.com/Chatmosphere/chatmosphere-app) und wir freuen uns über Erfahrungsberichte.

## Freie Platzwahl

Wie können wir die informellen Dynamiken echter Treffen, beispielsweise in einer Bar, in einem Video Call abbilden? In unserem Ansatz entsteht das Raumgefühl durch Unterschiede in der Lautstärke verschiedener Teilnehmer:innen zueinander. Je näher die Nutzer:innen mit ihrem Videobild anderen Nutzer:innen kommen, desto lauter können sie sich gegenseitig hören. Zur Verdeutlichung dieses Prinzips ist die kreisförmige Video-Repräsentation der Nutzer:innen mit einem Umkreis versehen, der die maximale Hörweite anzeigt. Das Interaktionsparadigma ist die freien Positionierung der eigenen Video-Repräsentation im Raum durch Drag and Drop.

<video src="/assets/images/project_images/chatmosphere/Chatmosphere_PrivateConversations_cut.mp4" autoplay controls muted loop></video>
*Nutzer:innen können sich also frei im Raum bewegen, sich zu kleineren Konversationen zusammenfinden oder diese unkompliziert wechseln.*

Es ist kein Herunterladen einer App oder eine Registrierung nötig. Eingeladene Nutzer:innen landen über einen Einladungslink direkt im Video-Call-Raum. Wir haben in unseren Tests gelernt, dass sich, in weniger digital affinen Gruppen, gerade diese direkte Teilnahmemöglichkeit bewährt hat. Solange die Person, die zum Call eingeladen hat schon im Raum anwesend ist, wird auch das Onboarding dynamisch: Die Bedienung kann gegenseitig erklärt werden, wenn beispielsweise Drag and Drop von ältere Teilnehmer:innen nicht durch ausprobieren exploriert werden konnte.

## You are not the user

Der Ansatz „Fail fast, fail often“ hat sich von Anfang an ausgezahlt. Bereits vier Tage nach Projektstart begannen wir eine kleine Nutzer:innenstudie. Für die Teilnehmenden präsentierte sich eine recht ansehnliche, vermeintlich fertige Software bei der in Wahrheit alle Funktionen von uns im Hintergrund gesteuert wurden.


![Mischpult beim user-test](/assets/images/project_images/chatmosphere/Chatmosphere_UserTest_Mischpult.png)
![Setup des User-Tests](/assets/images/project_images/chatmosphere/Chatmosphere_UserTest_Setup.png)
*Oben: Das Schatten-Setup / Unten: Ein Teilnehmer bedient eine augenscheinlich funktionierende Software*

Bereits in diesem Setting erwiesen sich einige Teile der angedachten Interaktionsparadigmen besonders für unbedarfte User als problematisch.

Neben [kleiner Korrekturen initialer Annahmen](https://chatmosphere.cc/user-test-1) hat uns der User-Test auch eine ganz große konzeptuelle Vereinfachung gebracht. So zeigte unsere Idee Räumlichkeit durch Stereo-Sound zu verdeutlichen keine Vorteile gegenüber einer simplen Lautstärkeregelung in Abhängigkeit der Entfernung der Avatare zueinander. Diese Erkenntnis entstand, da wir für den schnellen Test auf die schnelle keine Stereobox verwenden konnten. Die verfügbare kleine Bluetooth Box (oben im Bild des Test-Setups zu sehen) dazu geführt, dass wir die Stereo-Idee erstmal depriorisiert haben und das Projekt dadurch auf eine andere technologische Basis gestellt haben als zuerst angenommen (weniger Unity, mehr WebRTC).

Ein weiterer Test im Herbst 2020 hat uns auch vor Augen geführt, dass manche Annahmen eben nur Annahmen sind, die getestet werden müssen. Zum Beispiel wie “intuitiv” ein Interaktionspattern wie Drag and Drop wirklich ist, und welche Vorstellungen Nutzer:innen wohl haben, wenn sie andere Gesprächsteilnehmer:innen zwar sehen, aber nicht hören können. Zusammen mit den technischen Problemen, die viele der Test-User bei Video-Calls schon erlebt hatten, wurde manchmal lieber der Rechner neu gestartet, als der Versuch gewagt, sein eigenes Video per Drag and Drop auf dem Canvas zu bewegen.



![Lost User](/assets/images/project_images/chatmosphere/Chatmosphere_LostUser.png)
*Ein sich verloren fühlender Teilnehmer in der linken, oberen Ecke. Er kann niemanden hören und ihn hört auch niemand. Da er die Drag-and-Drop-Interaktion nicht von sich aus vermutet hat, findet er keinen Zugang zum Gespräch.*

Großartig war es dagegen zu sehen, dass andere Grundannahmen von den Nutzern:innen nach dem Erlernen des Interaktionsparadigmas weiter bestätigt wurden. So erwähnten Teilnehmer:innen etwa das “angenehme Setting”, in dem man ungezwungen seine Fokus verlagern und interessengesteuert an Gesprächen partizipieren kann. Hier wurde besonders die “sich natürlich anfühlende Möglichkeit” herausgestellt, schnell in temporäre private Gespräche aus größeren Runden auszubrechen zu können. Das positive Feedback auf unsere generelle Projektidee und all die neuen Feature Ideen und Anwendungsszenarien die in den Tests entstanden sind haben zu einem großen Motivationsschub geführt.

![Split Conversations](/assets/images/project_images/chatmosphere/Chatmosphere_SplitConversations.png)
*Verschiedene, gleichzeitig laufende Gespräche zu verschiedenen Themen im selben Raum.*

## Die Ernüchterung des Nicht-Tuns

Doch wie lange mit neuen Ideen experimentieren und wann fängt man an eine der Ideen stabil in einen finalen Prototypen zu überführen? Im Verlauf dieses Projekts sind viele Ideen entstanden, die wir gerne getestet hätten. Allerdings kostet es recht viel Zeit eine Idee so weit zu entwickeln, dass sie für eine diverse Gruppe von Menschen mit diversen Systemen einigermaßen nutzbar ist. User Research und frühes Prototypen hilft zwar beim aussortieren, jedoch kommt irgendwann der Punkt an dem Sack zugemacht werden muss, wenn etwas entstehen soll das Spaß macht, einigermaßen fehlerfrei programmiert und ausreichend dokumentiert ist. Dieser Punkt kam bei Chatmosphere früher als wir dachten und es ist, auch wenn wir unseren Prototypen lieben, bisweilen ernüchternd von all den tollen Ideen zu wissen, die wir (noch) nicht umgesetzt haben.

## Einfach Coden 

> “Coden wir lieber etwas oldschool, um den Einstieg einfacher zu machen und nachvollziehbar für potenzielle Contributors zu bleiben oder nutzen wir die neuesten heißen Libraries?”

Wie können andere (bei uns vor allem Designer:innen) im Sinne von Open Source möglichst einfach und selbstständig partizipieren? Contributions für und von nicht-Coder:innen sind super wertvoll, scheitern aber leider noch immer recht oft an hohen technische Hürden. Gezeigt hat sich das bei uns vor allem entlang der Logik von Styled-Components und Typescript.

![Chatmosphere Code](/assets/images/project_images/chatmosphere/Chatmosphere_Code.png)
*CSS mit Themes in Styled Components*

Beides ist prinzipiell enorm hilfreich, erzeugt aber eine weitere Abstraktion und damit Hürde für Partizipierende. So sollten die Styled Components vor allem die gemeinsame Arbeit am CSS reaktiver UI-Elementen mit Designer:innen erleichtern. Diese Hoffnung wurde in unserem Kontext leider nicht eingelöst, da die Implementierung der Styles (vor allem, wenn Theming verwendet wird) doch mehr Verständnis von Modulen, Build-Prozessen und Variablen voraussetzt, als initial erwartet. Da wir Zugänglichkeit und Partizipation für Hilfswillige aller Couleur ermöglichen wollen, würden wir in Zukunft, trotz der Vorteile durch Modularität zugunsten von Zugänglichkeit durch einfache Styles entscheiden.

## Vom Luxus dem Druck von Marktmechanismen ausweichen zu dürfen

An dieser Stelle wollen wir betonen, wie hilfreich diese explorative Arbeit im Rahmen des Protoype Funds für uns war: Hätten wir den Druck, ein konkurrenzfähiges Produkt zu entwickeln, hätten wir wahrscheinlich schon im Spätsommer einen Richtungswechsel in Richtung eines Workshop-Tools vorgenommen. Viele Tester:innen wollten die Ecken als Break-Out-Room-Ersatz verwenden und konnten sich Chatmosphere als Workshop-Tool vorstellen, vorausgesetzt die klassischen Zoom-Features würden abgebildet. Hierzu gab es auch eine konkrete Anfragen aus dem Unternehmenskontext. Allerdings hätten wir dafür den Fokus verändern müssen. Von informeller Gesprächsdynamik und Dokumentation auf Skalierung der Teilnehmer:innenanzahl, Whiteboardfunktionen, und Screensharing. Also einen Fokus hin zu wieder einem Meeting-Tool.

Wenn Zeit und Ressourcen vorhanden sind, spricht sicher nichts dagegen, weitere Features einzubauen. Auch solche, die wir aus bekannten Video-Call-Tools kennen. Doch im Fokus soll die zwischenmenschliche Interaktion bleiben, das fluide, das unmoderierte. Und die Förderung als Open-Source-Projekt hat hier möglich gemacht, dass wir mehr an [Dokumentation und Anschlussfähigkeit](https://github.com/Chatmosphere/chatmosphere-app) durch andere gearbeitet haben, als an Pitches und Features um uns zu differenzieren. Danke an der Stelle auch an unseren Mentor [Cade](https://newdesigncongress.org/en/), sowie Marie und Tasmo vom Prototype Fund Team, die zu diesem Thema sehr hilfreiche Gesprächpartner:innen waren.

## Lessons learned 

- Frühe User Tests sind aufschlussreich und sparen Zeit und Energie
- Auch in kleinen Teams lohnt es sich (frühzeitig) ein Task-Board anzulegen.
- Regelmäßige (bei uns wöchentliche) Stand-ups helfen bei der Koordination.
- Regelmäßiges Planen im Team (inkl. "Nicht-Tasks" und Time-Boxing bei unklaren Aufgaben) hilft dabei Missverständnisse, unnötige Arbeit oder Arbeitsdruck zu verringern. Wir hatten uns für einen 2-Wochen-Rhythmus entschieden.
- Es hilft Co-Working-Sessions auch im Remote-Setting einzuplanen, um voneinander zu lernen, sich auszutauschen und für’s allgemeine Wohlbefinden als Team.
- Über Visual Design-Ideen oder Feature-Ideen zu sprechen kann sehr viel Zeit kosten. Wireframes und Skizzen, die eine Designidee durchspielen erleichtern Entscheidungsprozesse.
- Wenn Diskussionen zu lange dauern, einfach erstmal über konkrete Vorschläge abstimmen (z.B. Dot-Votes).
- Informeller Austausch ist wichtig und muss in Zeiten von Corona aktiv (ein-)geplant werden. Wir haben uns zu gemeinsamen (virtuellen) Mittagessen verabredet, zum virtuellen Kaffee oder Feierabendbier oder einzeln zum spazierengehen.
- Keine Angst vor frühem Publizieren. Man weiß nie welche Menschen sich für das Projekt begeistern können und dabei helfen es weiterzuentwickeln.

# Ausblick 

Wie beschrieben, ist unsere Motivation informelle Gesprächsdynamiken zu explorieren. Vor allem für Bereiche außerhalb von Arbeit, sei es im Freizeitbereich oder für Initiativen die eine Community auch remote weiterentwickeln möchten. Wir konnten jetzt in dieser Runde des Prototype-Funds eine solide Basis schaffen, auf der wir selbst, aber auch andere weiter experimentieren können. 
Einsatzzwecke, die von Nutzer:innen angefragt wurden und sich in Gesprächen und Tests herausgebildet haben:

**Vereinfachte Installation**, um kleine Initiativen und private Gruppen dabei zu unterstützen Chatmosphere dezentral für sich zu nutzen.

**Einbettung einer Streaming-Oberfläche** um gemeinsam Filme oder Kulturveranstaltungen zu erleben. Denn Kunst und Kultur fehlt immer noch das gemeinsamen Erleben und die Reaktion von Publikum.

**Skalierung** der Teilnehmer:innenmenge. Denn zum informellen virtuelle Austausch in großen Gruppen, wie beispielsweise bei Meet-ups, als auch für große Workshops oder virtuelle Offices gibt es kaum sinnvolle Open-Source-Angebote. Und Chatmosphere wurde schon zu Workshops in fluiden Break-Out-Ecken verwendet.

**Einbetten unterschiedlicher Hintergrundbilder**. Sei es zur räumlichen Orientierung oder - vor allem - um gemeinsam Brettspiele zu spielen.

Wir haben für uns eine [kleine Roadmap](https://www.notion.so/Interactive-visual-Representation-of-Volume-Indicator-758363a7f3ce41ea934a672dbbac2a59) angelegt, um die Features zu sammeln, die wir im Rahmen der User Tests während der Projektlaufzeit identifiziert und (teils) ausgearbeitet haben. Features wie Screensharing oder Text-Chat können zukünftig auf Grundlage der Jitsi-API relativ einfach als Komponenten eingeführt werden.

## Dankeschön 

Großer Dank an das BMBF, das diese Förderung ermöglicht, und dem DLR, sowie Prototype-Fund-Team für die hilfreiche Unterstützung. Vielen Dank Yusuf und Emanuel, der andere Teil unseres Teams, und Dank an Christoph und Tillmann für die Ratschläge, Inspirationen und die ersten Contributions auf Github. Danke allen Mitgliedern von [Trink—Genosse](https://trink-genosse.de/), die an der Ideenfindung, dem Testen und der Nutzung dieses Projekts beteiligt waren sowie allen Test-Teilnehmer:innen <3