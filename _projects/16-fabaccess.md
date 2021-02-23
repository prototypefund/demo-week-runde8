---
layout: project
title: "FabAccess"
image: /assets/images/project_images/fabaccess/header.jpg
authors:
  - author: Kai Kriegel
    link:
  - author: Joseph Langosch
    link:
  - author: Jannis Rieger
    link:
  - author: Gregor Reitzenstein
    link:
  - author: Tasso Mulzer
    link:
brief: "Wir vereinfachen die Nutzungsverwaltung für offene Werkstätten."
summary: ""
---

<div class="iframe-container">
    <iframe src="https://www.youtube-nocookie.com/embed/CjBEGqvV_ms" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

## Das Projekt

Wir entwickeln FabAccess, ein föderierbares Verwaltungssystem für FabLabs, Makerspaces und Hackerspaces. Mit FabAccess soll der Zugriff auf Maschinen verwaltet werden, um so Unfälle zu vermeiden.

## Das Team

- Tasso: Product-Owner
- Gregor: Mädchen für alles, Backend
- Jannis: Design, Frontend
- Joseph: Frontend, Design
- Kai: Infrastruktur, Libraries

## Das Problem

Viele Hacker und Maker haben sich schon mit der Herausforderung befasst, ein eigenes FabLab nach den [Vorstellungen von Neil Gershenfeld](https://www.youtube.com/watch?v=aPbJmYCSCgA) aufzubauen und dieses mit wenig Personal "sicher" zu betreiben.
Um das möglich zumachen, haben diese auch angefangen eine Verwaltungssoftware für ihre eigenen Spaces zu schreiben.
Auch wir standen vor dieser Herausforderung: Wie kann man "gefährliche" Maschinen, wie unsere alte Drehbank, sicher betreiben? Gleichzeitig sollte natürlich die Idee des eigenständigen Lernens im FabLab erhalten bleiben, ohne dass ständig 20 Angestellte allen Nutzer:innen beim Umgang mit solchen Maschinen über die Schulter schauen müssen. Somit war die Idee für unser Projekt FabAccess geboren.

Aber das ist noch nicht alles, was FabAccess ausmacht. Aufgrund des sehr begrenzten Platzes in unserem Labor ist es uns nicht möglich, unseren Nutzer:innen jede Maschine zur Verfügung zu stellen.
Wie können wir es unseren Nutzer:innen also ermöglichen, unkompliziert an andere Maschinen zu kommen, ohne unnötigen Mehraufwand bei kooperierenden Spaces zu erzeugen?
Mit diesem Problem ergibt sich der zweite wichtige Aspekt von FabAccess: Es ist auch ein föderierbares Verwaltungssystem. Somit können sich Spaces aller Art zusammenschließen und die Nutzer:innen je nach Makerproblem den passenden Space besuchen. So wird die Kommunikation und Zusammenarbeit zwischen allen gestärkt. Aus Kommunikation entsteht bekanntlich Innovation.

## Die Ausgangslage

Da wir Kommunikation fördern wollen, haben wir zu Beginn des Projektes auch genau dort angefangen. Um möglichst allen Bedürfnissen und Wünschen, die aus vielen Perspektiven an ein solches Verwaltungssystem gestellt werden, gerecht zu werden, haben wir uns auf FabLab- und Makerkonferenzen umgehört und sind aktiv auf die verschiedensten Creator (Nutzer:innen eines Spaces) und Manager (Betreiber:innen) solcher Spaces zugegangen. Mit diesen haben wir uns in kleinen und mittleren Runden zusammengesetzt, um alle Ideen zusammenzuschreiben.

Natürlich dachten wir uns schon, dass wir nicht die Ersten sind, die sich an ein solches Projekt wagen. Daher haben wir nach guter OpenSource-Arbeitsweise, nach eben solchen Projekten gesucht, gefragt und sind auch dort aktiv auf die Beteiligten zugegangen.
Die Projekte waren auf den verschiedenesten Ständen, von einfachen Frontend-Designs bis hin zu lokal verwendeten Systemen. Um nicht auf dem Stand von "works for me" zu bleiben, haben wir uns mit den Entwickler:innen solcher Systeme getroffen und uns über die Umsetzung und "Lessons Learned" unterhalten, gechattet und offen diskutiert.

Die vielen Anregungen aus diesen Runden haben wir in einem Lastenheft kondensiert und festgehalten. Dieses Lastenheft bildet die Grundlage für unser Projekt, auch wenn wir in unserer Arbeitsweise nicht im klassischen [Wasserfallmodell](https://de.wikipedia.org/wiki/Wasserfallmodell) geblieben sind. Selbstverständlich haben wir flexibel und teilweise mit agilen Konzepten gearbeitet.

Da all diese Projekte nur lokal im Einsatz waren und wir einen föderativen Ansatz verfolgten (der "Verband offener Werkstätten" war an diesem Wunsch nicht ganz unbeteiligt), mussten wir dort gezielt ansetzen. Daraufhin haben wir uns auf die Förderung des Prototype Fund beworben, um uns in der Förderphase voll auf die Planung und Entwicklung dieses Projekts konzentrieren zu können.

Hier haben wir eine Liste von bekannten Projekten ähnlicher Zielrichtung zusammengefasst:

- [Commons Booking](https://prototypefund.de/project/commons-booking/)
- [Fab Lab Siegen (David Amend)](https://github.com/FabLabSiegen/FabLabAccessControl)
- [Düsseldorf (Fabian Meyer)](https://github.com/faaaaabi/)
- Beuth Hochschule für Technik Berlin
  - [qrhello](https://github.com/dequbed/qrhello)
  - [card2go](https://github.com/HazeCore/Card2Go/)
- [ETH Zürich](https://sph.ethz.ch/acos_project/)
- [Übersicht beim Verband offener Werkstätten](<https://cowiki.offene-werkstaetten.org/uploads/2017-06-23_11-31-15_Zugangssysteme%20%C3%9Cberblick%20(WS).pdf>)
- [FabLab L'Aquila](https://github.com/FabLabAQ/LabAccessControl)
- [Google makerspace-auth](https://github.com/google/makerspace-auth)
- [Dresden (Roseguarden)](https://github.com/mdrobisch/roseguarden)
- [FabLab München](https://github.com/sschaeffner/)
- [MakerSpace Graz ("LEASIE")](https://leasie.makerspace.at/)
- [Hackerspace Liege](https://github.com/LgHS/sign-in)
- [Flipdot e.V. Kassel](https://github.com/flipdot/gsm-door)
- [CoreDump, Rapperswil-Jona / Schweiz](https://github.com/coredump-ch/interna)
- [open-taffeta](https://github.com/apiraino/)

## Die Umsetzung

Da wir zu unseren Features und Plänen schon ein paar kleine Vorträge gehalten haben sowie vieles auf unserer Webseite niedergeschrieben ist, verlinken wir an dieser Stelle dorthin. Schaut es euch gerne an.

---

**FabAccess Feature Beschreibung:** [fab-access.org](https://fab-access.org/de/projects/fabaccess/)

**FabAccess Feature- und Planungsvortrag vom rC3:** [media.ccc.de](https://media.ccc.de/v/rc3-326175-fabaccess)

**Folien vom rC3 Vortrag:** [docs.google.com](https://docs.google.com/presentation/d/1Lk1l-6z8GM2PyjsHXDBPsHLr4PJJ27CuA3QnHiB23cM/edit?usp=sharing)

---

**tl;dr:**
FabAccess besitzt drei Hauptfunktionalitäten:

- Maschinenverwaltung
- Berechtigungssystem
- Nutzer:innenverwaltung

Das Prinzip von FabAccess ist es, Maschinen über den Stromanschluss ein- und auszuschalten. So sind Maschinen im Normalfall stromlos und damit ungefährlich. Erst wenn Nutzer:innen an der Maschine sind, die für die sichere Bedienung befähigt und eingewiesen sind, wird die Maschine mit dem Stromnetz verbunden.

### Tooling

Jedes Team braucht ein sinnvolles Tooling, die Frage ist nur, was heißt "sinnvoll"?
Der Ansatz für unser Tooling basiert, wie bei den meisten Projekten, auf den vorhandenen Fähigkeiten der Entwickler:innen.
Um einen möglichst stabilen Core zu entwickeln, wird unser Server in Rust entwickelt, da wir einen sehr guten Rustentwickler an Bord haben. Die Sprache ist auch gut für die Entwicklung stabiler Backends geeignet, weil viele Programmierfehler schon durch den relativ intelligenten Compiler verhindert werden.

Für das Frontend war es die "Wahl der Qual": Welche Plattformen will man unterstützen und mit welchem Framework kann man unsere Ideen überhaupt umsetzen?
Unsere Wahl ist aufgrund der kurzen Förderphase auf C# mit Xamarin gefallen, da einer von uns schon etwas Erfahrung mit WPF-Entwicklung hatte und sich mit Hilfe von Xamarin ein Client gut auf fast alle Plattformen portieren lässt.

Für eine funktionierende und langfristige Föderation benötigten wir eine stabile API, über die die einzelnen Instanzen und Clients mit unserem Server(BFFH - Diflouroborane) kommunizieren können. Auch eine Abwärtskompatibilität ist sinnvoll, wenn BFFH von einzelnen Spaces auf deren Bedürfnisse angepasst werden können soll. Dabei sollte unser Referenzclient (Borepin) nicht funktionsunfähig werden. Um all dies möglich zu machen, ist unsere API in Cap'n Proto geschrieben.

![Struktur von FabAccess, mit Schnittstellenaufteilung](https://i.imgur.com/5ovELvG.png)

> Struktur von FabAccess, mit Schnittstellenaufteilung

### Erweiterungen

Dieses Thema war bei Gesprächen mit den anderen Spaces immer vorne mit dabei, da keiner der Spaces seine selbst gebaute Hardware neu bauen will oder teuer eingekaufte Systeme verlieren möchte. Um das möglich zu machen, haben wir eine API geplant, die generisch genug ist, um verschiedenste Systeme anzubinden.
Damit nicht jeder Space seine Hardware selbst basteln muss und damit zum Entwickeln eigener Software gezwungen wird, entwickeln wir von unserer Seite aus passende Referenzhardware, um den Einstieg zu erleichtern.
Um die kommerziellen Produkte nicht außer acht zu lassen, arbeiten wir an der Einbindung der gängigsten Geräte, wie Shelly Plugs oder Systemen mit Tasmota und anderen. Somit kann sich ein Space beim Verwenden unseres Systems entweder unserer Bastelaufgabe stellen oder einen schnellen Einstieg durch gekaufte Produkte hinlegen.

### Hardware

Hardware zur Anbindung an die Geräte wurde uns unter anderem von einem sehr engagierten Unterstützer zur Verfügung gestellt.
Vielen Dank an dieser Stelle an Joris, der für uns den ersten Prototypen eines SmartCard-Readers entwickelt hat, der sich schon wunderbar an unsere Schnittstellen anbindet.

![Drehbank mit ursprünglichem Schaltungsprototypen](https://i.imgur.com/DMiYB24.jpg)

> Drehbank mit ursprünglichem Schaltungsprototypen

### Föderation

Nachdem wir die ganze Zeit von Föderation reden und schreiben, wollen wir auch die Frage klären, was Föderation für uns ist.
Wir haben unseren Ansatz wie folgt definiert:

> Föderation ist eine Form von Zusammenarbeit von Organisationen. Die Organisationen behalten dabei ihre Eigenständigkeit und arbeiten gleichberechtigt und weitgehend autonom bei der Erreichung gemeinsamer Ziele zusammen.

Unser gemeinsames Ziel mit FabAccess ist das niederschwellige und unkomplizierte Teilen von Nutzer:innen und somit die Verbesserung der Zusammenarbeit von Creatoren über Spacegrenzen hinweg sowie die gleichberechtigte Zusammenarbeit von Managern.

Unser Ansatz kann in der Realität wie folgt aussehen:
Creator aus Space A geht zu Space B und kann dort mit der Einweisung für eine Maschine aus Space A die gleiche Maschine in Space B verwenden, ohne eine weitere Einweisung zu benötigen.

Wir haben gesammelt und wissen, was die meisten anderen Projekte machen und gemacht haben, zumindest innerhalb einer einzelnen Werkstatt. Allerdings gibt es verschiedene Dach-Organisationen, die diese Werkstätten als Verband gemeinsam vertreten.
Um föderieren zu können, brauchen wir einen Standard, den alle nutzen können.
Das können eine stabile API-Beschreibung und stabile Strukturen sein, die von den einzelnen Teilnehmenden abwärtskompatibel erweitert werden können, ohne dass die ursprünglich implementierte Föderation gestört wird.

Um nicht auf eine spezielle Hardware angewiesen zu sein, braucht es generische Schnittstellen, die komplexe und einfache Hardware unterstützen. Sicherheitsanforderungen sollen vorerst, so weit das geht, bei den Anwender:innen bleiben und nicht auf uns zurückfallen.

Was wir können (wollen): Ein sicheres und stabiles Berechtigungssystem bieten, das die notwendige Kommunikation realisiert und Events an generische Schnittstellen geben kann.
Das System soll dabei granuliert und anwendungsorientiert Entscheidungen weitergeben. Weiterhin soll es den Anwender:innen dienen und dabei nicht in deren Prozesse eingreifen oder ihnen ungewollte Komplexität oder Strukturen aufzwingen oder gar in deren Entscheidungen einwirken.

Außerdem wollen wir, dass unter den einzelnen Instanzen gemeinsame Entscheidungen mit Föderation getroffen werden können, ohne dass die einzelnen Parteien ihre Rechte verlieren.

### SmartCards

Um Maschinen sicher mit einer SmartCard aktivieren zu können und nicht nur über ein Handy oder einen PC, setzten wir auf NXP MIFARE DESFire Karten.
Die Anforderungen an ein föderierbar einsetzbares SmartCard-System sind hoch, da so die jeweils andere Partei keine einfache Validierung der Karte durchführen kann. Auch das Authentifizieren mit einem Schlüssel gestaltet sich über Föderationen hinweg schwierig, da der Reader dem einen Space gehört und die Karte dem anderen. Ein Reader hat daher nicht immer die Schlüssel für die gelesenen Karten.
Die DESFire-Karte besitzt ein Feature, mit dem eine Karte via OTA-Verfahren (Over-the-Air) direkt mit einem entfernten Server kommunizieren kann, ohne dass der Reader Schlüssel für die Karte benötigt. Der Reader übernimmt dabei nur die Rolle eines Proxys (Brücke/Vermittler). Mit diesem Ansatz stellen wir ein sicher föderierbares Kartensystem, was wir so bisher noch nicht im OpenSource-Bereich finden konnten.

## Die Herausforderungen

Auch wir standen während der Umsetzung vor einigen Herausforderungen, die Schwierigsten haben wir mal niedergeschrieben.

### Aller Anfang ist schwer

Da unser Projekt viele Aspekte und eine hohe Komplexität besitzt, war das Auswählen schwierig. Wir konnten nicht direkt einzelne Features separat bauen, da der Core erst implementiert werden musste, bevor wir mit solchen Funktionalitäten beginnen konnten.
Auf der Core-Seite begannen wir mit dem Aufbau eines Event-Netzwerks und der Anbindung von einem MQTT Server sowie dem Aufbau der Datenbankstrukturen.
Auf der Client-Seite war die Auswahl für unabhängige Aufgaben begrenzt, da die Funktionalität im Core und über die Cap'n Proto API abgebildet wird. Daher stürzten wir uns auf die Implementierung von dem SmartCard Proof-of-Concept und der Anbindung der Cap'n Proto API.

### UX und NFC

In unserem ersten Coaching mit Simply Secure stellten wir unseren ersten Designentwurf für Borepin vor. Bei diesem Gespräch wurde angesprochen, dass wir ein Wiedererkennungsmerkmal für eine NFC-Interaktion kreieren sollten, um so Nutzer:innen eine einfache Erkennung von NFC-Tags oder Karten bereitzustellen. Daraufhin ist unser Design für eine NFC-Markierung entstanden.

![SmartCard und Maschinensticker im FabAccess NFC Design](https://i.imgur.com/IcxxwjR.jpg)

> SmartCard und Maschinensticker im FabAccess NFC Design

### Föderation und Netzwerke

Bei der Föderationsplanung und -entwicklung hatten wir ein paar ungeklärte Fragen zu beantworten.
Da unser langfristiges Ziel ist, über eine Föderation auch eine Abrechnung zu ermöglichen, sollten die Föderationsabläufe sicher und nachvollziehbar für beide Parteien sein.
Da Föderation für beide Seiten einen erkennbaren Vorteil mit sich bringen muss, ist unsere Planung bisher nur eine direkte Föderation zu erlauben. Somit föderieren nur Spaces miteinander, deren Manager sich kennen und zusammenarbeiten wollen. Es ist keine Netzwerkbildung möglich, bei der ein Zusammenschluss von Spaces entsteht, bei dem ein neuer Space direkt Zugriff auf alle Spaces erhält, ohne diese selbstständig und gegenseitig zu akzeptieren.

### Community

Bei Thema Community und Unterstützer:innen netzwerken wir nun schon seit über zwei Jahren für diese Projektidee und haben uns auch in Laufe der Förderung um eine Veröffentlichung unserer Fortschritte bemüht.

Um unsere Kommunikation für die Entwicklung des Projekts nicht in privaten Chatgruppe zuführen, haben wir uns für die Open Source Software Zulip entschieden und sind dort für neue und alte Interessierte und Unterstützer:innen leicht erreichbar. Das Threading ist in Zulip für ein solches Projekt ideal.

Durch die Verbindung unserer Teammitglieder zum Chaosumfeld haben wir unseren ersten Vortrag beim Chaostreff Potsdam Anfang Dezember gehalten. In diesem konnten wir unser Projekt vorstellen und die ersten Erkenntnisse und Planungen vorstellen. Vielen Dank an dieser Stelle an den Chaostreff Potsdam für diese Gelegenheit.

Da es nun schon fast Tradition ist, auf dem Chaos Communication Congress eine kleine Gesprächsrunde rund um das Thema FabLab zuführen, haben wir uns für eine digitale Gesprächsrunde auf dem rC3 entschieden.
Durch diesen Talk konnten wir unserem Projekt zu mehr Öffentlichkeit verhelfen. Auch die Make hat uns darauf hin in einem ihrer [Online-Artikel](https://www.heise.de/news/FabAccess-Bessere-Maschinenverwaltung-fuer-Fablabs-5027184.html) erwähnt sowie ein Beitrag in der aktuellen Ausgabe veröffentlicht.
Dieses mediale Interesse sowie die Rückmeldungen haben uns gezeigt, dass wir auf einem guten Weg sind und unser Projekt etwas verändern könnte.

## Der Stand

Wie leider so oft in durchgeplanten Projekten haben wir **nicht alle** Ziele schon am Ende des Förderzeitraums erreicht.

Wir haben, wie ihr im Video sehen könnt, einen Prototypen, der die Maschinen einschalten kann.

Das SmartCard-System haben wir bisher nur als Code Libraries und Proof-of-Concept vorliegen, es muss noch in den Core eingearbeitet werden.

Wir haben eine erste Version der API am Anfang des Projektes definiert, welche grundlegende Funktionen beinhaltet, die wir zu diesem Zeitpunkt schon festlegen konnten. Wir arbeiten gerade an einer verbesserten Version, in die unsere jetzigen Kenntnisse und zukünftigen Wünsche einfließen, um bald einen stabilen Stand bieten zu können. Auch die einzelnen Subsysteme, die wir definiert haben, werden jetzt dort eingearbeitet.

Auf der Seite des Clients gibt es noch einige Bugs zu fixen, um unseren Cap'n Proto Code auf allen Plattformen ausführen zu können.
Auch müssen wir unsere Designs noch in den Client einbauen. Das ist der nächste Schritt nach der API-Verbesserung.

Auch muss unsere komplette Planung noch genauer aufgeschrieben werden und unsere Konzeptentscheidungen festgehalten werden.

Für die Föderierbarkeit müssen noch ein paar Umsetzungsentscheidungen getroffen werden, dass wir dann auch alles in die API einfließen lassen können.

Wie ihr seht, haben wir noch einiges zu tun.

## Die Zukunft

Die gute Nachricht ist: **Wir machen weiter**.

Wir arbeiten an einer Strategie zur weiteren Förderung unseres Föderationskonzepts, um es gemeinsam mit dem Verband offener Werkstätten und dem Fab:Universe-Netzwerk fertigstellen zu können und ab der zweiten Hälfte des Jahres ein größeres Roll-out angehen zu können.

Auch wollen wir in einem Machbarkeitstest unseren Core (BFFH) erweitern und so testen, ob wir auch andere Anwendungen wie z. B. ein Netzwerk aus Lastenfahrradverleihen mit unserem System unterstützen können.
Unser offener und generischer Ansatz scheint sich auszuzahlen.

![Föderationsablaufbeispiel von FabAccess/DEMOKrAtIS](https://i.imgur.com/2nX7EV1.png)

> Föderationsablaufbeispiel von FabAccess/DEMOKrAtIS
> _DEMOKrAtIS ist der Projektname des Machbarkeitsprojektes_

Mit unseren Verbündeten aus der Schweiz werden wir auch weiter zusammenarbeiten und bekommen mit etwas Glück aus der Richtung auch noch zwei Entwickler:innen als Unterstützung.

Auch an der Hardwarefront wird weiter getüftelt, mit unserem Unterstützer wollen wir eine neue Version des Readers erarbeiten, die wir als OpenHardware und als Bausatz bereitstellen wollen.

Für das Abrechnungssystem sind wir noch auf der Suche nach einem Partner, mit dem wir als Open-Source-Lösung den FabLabs, Makerspaces und Hackerspaces bei der Abrechnung von Leistungen helfen können.

Wie ihr sehen könnt, haben wir noch einige Ideen und Visionen, an denen wir arbeiten können. Und wir bleiben unserem Motto vom Kick-off der Förderphase treu: "3 Billion Devices run FabAccess".

Für alle, die noch schöne Ideen für unser Projekt haben oder uns bei der Umsetzung (auch bei unseren anderen Fab... Projekten) helfen wollen, können wir nur sagen, kommt auf unser [Zulip](https://fabaccess.zulipchat.com/), **wir machen was Schönes draus**.

## Ein kleines Fazit

### Zum Projekt

Wir setzten mit diesem Projekt unseren Wunsch nach einer zusammenarbeitenden Open-Source-Gesellschaft um.

Wir haben mehr Zeit in einige Aufgaben gesteckt, als wir erwartet und geplant hatten. Mit den Ergebnissen können wir aber zufrieden sein. Wir sind unserem Ziel und der ursprünglichen Idee ein großes Stück näher gekommen.

Wir müssen aber auch zugeben, dass wir an unserem Teammanagment arbeiten müssen: Die nicht vollsynchrone Arbeitsweise mit nur wenigen persönlichen Treffen in der Gruppe bringt einige Schwierigkeiten mit sich und kann schnell zu Spannungen führen.

### Zur Prototype-Fund-Förderung

Die Förderung durch den Prototype Fund hat unserem Projekt einen riesigen Sprung nach vorne ermöglicht.
Ohne die Möglichkeit, viel Zeit in Planung und Entwicklung stecken zu können und dabei trotzdem unseren diversen finanziellen Verpflichtungen nachkommen zu können, wären wir nie in dem halben Jahr auf das Level gekommen, auf dem wir jetzt sind.

Die Organisation vom Prototype Fund ist gut, wir würden uns aber noch mehr Unterstützung bei den steuerlichen und finanziellen Aspekten der Förderung wünschen. Die Coachings waren sehr hilfreich für die Design-Entscheidungen, für die wir auch schon viel Lob bekommen haben, vielen Dank an Eileen und Simply Secure an dieser Stelle.

Da wir für unser Projekt auch Hardware benötigten, hätten wir uns über die Möglichkeit einer Föderung der Arbeit an zum Beispiel der Hardware eines SmartCard-Readers gefreut.

Wir hoffen, dass das BMBF auch in Zukunft solche Civic Tech Projekte unterstützt und so einen Startboost gibt.

Vielen Dank auch an die Teams von Prototype Fund, DLR und des BMBF für die Planung und Unterstützung im Rahmen dieser Förderung.
