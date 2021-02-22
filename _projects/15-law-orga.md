---
layout: project
title: "Law & Orga"
image: /assets/images/project_images/law-orga/header.jpg
authors:
  - author: Dominik Walser
    link:
brief: "Wir unterstützen Refugee Law Clinics, damit diese noch bessere Beratungen anbieten können."
summary: "Mit Law&Orga entwickeln wir ein System zur Akten- und Organisationsverwaltung für ehrenamtliche, studentische Vereine, welche Geflüchteten Rechtsberatung bieten."
---

Geflüchtete stehen vor vielen Schwierigkeiten. Unter anderem haben sie oft nur schwer Zugang zum Recht - obwohl es sich bei ihren rechtlichen Problemen meist um existenzielle handelt.
Um dieser Ungerechtigkeit zu begegnen, haben sich Refugee Law Clinics, kurz RLCs, gebildet. RLCs sind zum Großteil studentisch organisierte Vereine, welche Geflüchteten ehrenamtlich und kostenlos Rechtsberatung bieten - um ihnen so die Informationen und Unterstützung zu bieten, die ihnen faire und menschenwürdige Behandlung und Rechtsschutz ermöglichen.

Um diese Arbeit zu ermöglichen, ist ein den höchsten Datenschutzansprüchen genügendes System zur Aktenverwaltung und (Vereins-)Organsiation nötig.
Der Dachverband der RLCs entwickelt dafür seit einiger Zeit Law&Orga, ein solches System, welches genau auf die Bedarfe der RLCs zugeschnitten ist.
Dabei haben alle RLCs individuelle Verfahren und Organisationsstrukturen - und genau das bildet Law&Orga über klar abgetrennte und einzeln verwaltbare Bereiche ab. So können bisher einzelne Akten angelegt und bearbeitet, Dokumente und Dateien abgelegt und Mitglieder verwaltet werden. All dies mit strikter Vergabe von Einzelberechtigungen, um bei den hochsensiblen Daten für Sicherheit zu sorgen.

## Komponenten

Im bisherigen System fehlte die Möglichkeit, gemeinsam an Projekten wie beispielsweise der strategischen Prozessführung oder der Öffentlichkeitsarbeit/Vereinsstruktur zu arbeiten. Auch die Möglichkeit, umfassende Erkenntnisse aus den Beratungen zu ziehen und so die Arbeit bedarfsorientierter gestalten zu können, war bisher nicht gegeben.
Im Rahmen des Prototype Funds hatten wir die Möglichkeit, unser System um diese zwei Komponenten zu erweitern:
Einerseits mit einer Kollaborations-Komponente, kurz Collab, andererseits eine Statistik-Komponente zur Aufschlüsselung unserer Arbeit.

### Collab

<div class="iframe-container">
    <iframe src="https://www.youtube-nocookie.com/embed/Qd80dr-3uwA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

Collab bietet die Möglichkeit für die Mitglieder der RLCs, gleichzeitig kollaborativ an Dokumenten zu arbeiten. Dies ist besonders wichtig, da gerade im ehrenamtlichen Bereich viele Personen zusammen an unterschiedlichen Orten arbeiten. Gerade bei zeitkritischen Schriftsätzen ist also eine simultane Bearbeitung von Dokumenten essentiell - die dezentrale Arbeit verstärkt diesen Bedarf zusätzlich.
Collab kann dabei über einen Reiter, wie die anderen Komponenten des Systems, ausgewählt werden.
Die Dokumente von Collab lassen sich wie in einer Ordnerstruktur organisieren. Ein Dokument kann also unabhängig im ‘obersten’ Level oder einem anderen Dokument untergeordnet sein.

Die Dokumente werden immer in ihrer letzten veröffentlichten Version angezeigt. Möchte man das Dokument bearbeiten, kann man hierfür in einen eigenen Modus wechseln.
Hier wird im Hintergrund mit yjs ein geteilter Zustand erstellt, in welchem der aktuelle Inhalt des Dokuments mit allen gleichzeitig bearbeitenden Personen des Dokuments geteilt wird.
Die ursprüngliche Verbindung erfolgt dabei über einen öffentlichen Signaling-Server von yjs, welche jedoch mit einem generierten Passwort geschützt wird. Anschließend verbindet sich jeder Client mit jedem anderen Clients. Diese Methode ist somit also weniger für sehr viele gleichzeitig Bearbeitende geeignet, minimiert jedoch die Serverlast, da so kein Websocket aufgebaut werden muss, welches die Clients miteinander synchronisiert.
So werden die Änderungen eines Nutzenden direkt an die anderen weitergegeben - und gemeinsames digitales und ortsunabhängiges Arbeiten möglich.

Im Texteditor, bei welchem wir das Open-Source-Projekt [Quill](https://quilljs.com/) einbinden, finden sich übliche Textbearbeitung-Features wieder, wie zum Beispiel geordnete und ungeordnete Listen, Überschriften sowie Text- und Hintergrundfarbe.
Außerdem können alte Versionen des Dokuments eingesehen werden.

In Zukunft können wir uns hier einige weitere Features gut vorstellen. Insbesondere Kommentare direkt im Text, der Export in PDF- und Textdokumente und Hervorhebungen in Versionen des Dokuments. Auch das Verlinken von Nutzer:innen wäre eine sinnvolle weitere Ergänzungsmöglichkeit.

### Statistik

Die Statistik-Komponente ermöglicht den einzelnen Vereinen statistische Informationen über die aktuellen Ereignisse innerhalb der Organisation zu erhalten. Für die Darstellung konnten wir [ngx-charts](https://swimlane.gitbook.io/ngx-charts/) nutzen, die Daten kommen direkt aus unserem [Django](https://www.djangoproject.com/)-Backend.

Hierbei konnten wir unter anderem Daten über die Verteilung der Themenschwerpunkte, eine übersichtliche Darstellung des Status aller Akten und einen zeitlichen Verlauf der Akten hinzufügen.

![](/assets/images/project_images/law-orga/screenshot1.png)

Außerdem haben wir dadurch den Grundstock für weitere Informationsangaben gelegt, welche nun mit sehr wenig zusätzlichem Aufwand hinzugefügt werden können.

Direkt zu Anfang konnten wir außerdem eine Cloud-Umgebung mit [Prometheus](https://prometheus.io/) und [Grafana](https://grafana.com/) erstellen. Hiermit erhalten wir genauere Informationen über das laufende System selbst und können auftretenden Probleme ggf. vorhersehen.

![](/assets/images/project_images/law-orga/screenshot2.png)

### Fazit

Law&Orga ist schon in einigen RLCs in aktiver Benutzung. Mit der Implementierung dieser weiteren Komponenten können wir die Attraktivität des Systems für weitere Vereine weiter steigern und für unsere Nutzer:innen einen großen Mehrwert bieten. Denn hierdurch können sie effektiver und qualitativ hochwertiger Menschen in Not helfen.
Wir hoffen dem System in Zukunft weitere große Komponenten und viele kleine Verbesserungen hinzufügen zu können, um mittelfristig ein System bieten zu können, welches alle Bedarfe der RLCs datenschutzkonform, individualisierbar und anpassbar deckt.

Wir bedanken uns herzlich beim Bundesministerium für Bildung und Forschung sowie beim Projektträger DLR und dem Prototype Fund.
