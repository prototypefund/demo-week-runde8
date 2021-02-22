---
layout: project
title: "DiCaMa"
image: /assets/images/project_images/dicama/header.jpg
authors:
  - author: Christian Schulz
    link:
  - author: Christoph Speier
    link:
  - author: Sebastian Schroth
    link:
  - author: Jonas Jung
    link:
  - author: Sebastian Schneider
    link:
  - author: Dennise Cepeda
    link:
brief: "Wir entlasten Krebspatient:innen mit einem intuitiven und modularen Krebsmanagement."
summary: ""
---

<div class="iframe-container">
    <iframe src="https://www.youtube-nocookie.com/embed/i-tPAVnNrJg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

Die Diagnose Krebs bedeutet nicht nur Ängste und viele Sorgen, sondern oft auch einen zweiten Vollzeitjob: Krebsmanager:in. Die Arbeit und der Organisationsaufwand rund um die Erkrankung rauben Zeit und Energie. Beides Dinge von denen gerade Menschen mit einer Krebserkrankungen nicht viel haben.

Digitale Lösungen können hier Lebensqualität stiften und Arbeit abnehmen oder zumindest unterstützen, aber leider haben sich im komplexen Umfeld „Krebs“ mit kommerziellen Apps viele Insellösungen für einzelne Krebserkrankungen und spezifische Probleme entwickelt. In der Folge müssen Patientinnen mehrere verschiedene Apps nutzen, um ihre Krankheit digital zu managen. Das bedeutet für die Patient:innen oft die gleichen Fragen mehrfach zu beantworten, auf den Datenschutz verschiedenster Anbieter zu vertrauen und alles in allem Potential für smarte Lösungen zu verschenken.

DiCaMa will Patient:innen in ihrer schwierigen Situation mit einer digitalen, modularen sowie intuitiven Applikation unterstützen und dabei volle Datenhoheit gewährleisten. Dabei soll langfristig jede Form und Phase der Erkrankung von der Diagnose, über die Therapie bis hin zur Remission oder palliativen Betreuung angesprochen werden.

Der technische Kern auf Open Source Basis soll in der App die Möglichkeit schaffen, Module zielgenau für individuelle Bedürfnisse anzupassen. Wir setzen bei Open Source nicht nur darauf, dass jede:r am Entwicklungsprozess teilhaben kann, sondern wir wollen eine Dynamik erzeugen, dass Menschen mit einer Krebserkrankung und die Entwickler:innen sich verbünden, um sich gemeinsam Herausforderungen zu suchen und konkrete Probleme zu lösen. Wir glauben daran, dass Menschen sich gerne helfen und wir wollen helfen einfach machen. Dazu schaffen wir die technischen Voraussetzungen und bauen eine Community auf.

Im Rahmen des Prototype Funds wurde das Konzept mit dem Fokus auf Darmkrebs umgesetzt und das Ergebnis ist:

![](/assets/images/project_images/dicama/Folie1.PNG)
MONK – Dein Krebsmanager einfach und sicher

## Das Konzept

Der ursprüngliche Name DiCaMa als Abkürzung für „Digital Cancer Management“ beschreibt zwar treffsicher, was die App an sich tut, ist dabei aber sehr technokratisch. Deswegen haben wir uns früh entschlossen das Projekt umzubenennen, um dem Grundgedanken des Projekts besser gerecht zu werden: Eine Krebserkrankung ist ein sehr persönliches Thema mit vielen individuellen Herausforderungen und Problemen. Genau das beschreibt für uns der neue Name MONK, der für „Meine ONKologie“ steht. In diesem Namen steckt genau das, was wir und Patient:innen sich von einem digitalen Assistenten erwarten: Individualität und Einfühlungsvermögen.

Wir haben drei Grundsäulen definiert, die für eine digitale Unterstützung im Krebsalltag wichtig sind:

- Individualität,
- Leichtigkeit,
- Vertrauen.

Individualität bedeutet für uns, dass es letztlich egal sein sollte, um welchen Form des Krebs, welches Stadium und welche Bedürfnisse es geht. Die App passt sich dem Menschen an und diese Fähigkeit beruht auf dem modularen Aufbau. Wenn ein Bedarf noch nicht erfüllt ist, sollte es für die Patient:innen leicht sein diesen mitzuteilen und für die Entwickler:innen unkompliziert eine Lösung bereit zu stellen.

Leichtigkeit bedeutet, dass in der App und den jeweiligen Modulen der Fokus auf Usability gelegt wird, um der Patient:in eine einfache und intuitive Benutzung zu ermöglichen. Aber auch für Entwicklerinnen sollen Umsetzungen auf dem zugrundeliegenden Framework leicht von der Hand gehen.

Vertrauen bedeutet für uns, dass Daten nicht nur sicher sind, sondern auch der Umgang damit transparenter wird. Die sensiblen Daten gehören den Patient:innen und werden daher lokal verschlüsselt gespeichert. Um bei diesem komplexen Thema den Spagat zwischen Usability und Schutz zu meistern, setzen wir nicht nur technisch sondern auch in der Kommunikation klare Impulse.

## Die App

Beim ersten Start der App wird die Patient:in durch ein Onboarding geführt, das mit so wenig wie möglich Informationen versucht eine bestmögliche Auswahl an Modulen vorzuschlagen. Wir erfragen im Sinne der Datensparsamkeit keine Informationen, die wir nicht aus technischen oder medizinischen Aspekten benötigen. Gleichzeitig wird die/der Patient:in auch informiert über die Besonderheiten der App, sowie den Kerngedanken: sensible Daten verschlüsselt auf dem eigenen Telefon abzulegen.

![](/assets/images/project_images/dicama/Folie2.PNG)

Nach dem Onboarding steht de/de Patient:in die ausgewählte Funktionalität zur Verfügung und man erhält im Rahmen eines individuellen Dashboards eine - zunächst leere - übersichtliche Ansicht der Module. Neben dem Dashboard als Grid-Symbol und einer zentralen Übersicht für Benachrichtigungen als Glocken-Symbol gibt es in dem oberen Menü auch stets die Möglichkeit, sich mittels dem Schild-Symbols direkt über den Datenschutz zu informieren. Ein:e Patient:in muss sich also nicht zu einem versteckten Untermenü klicken, um den Datenschutz nachzuvollziehen, sondern kann sich über einen fixen und stets präsenten Menüpunkt über den Umgang mit den persönlichen Daten informieren. Welche Daten werden erfasst? Welchem Zweck dient dies? Welches Modul greift auf welche Daten zurück? Mit dieser klaren Verankerung des Datenschutzes wollen Transparenz und Verständnis für den Umgang mit Daten schaffen. Dies wird vor allem wichtig, wenn in Zukunft immer weitere Module entwickelt und eingebunden werden.

![](/assets/images/project_images/dicama/Folie3.PNG)

Im Dashboard hat man schnell und unmittelbar die Möglichkeit über die jeweiligen „+“ Symbole in den einzelnen Modulen jeweilige Kerninteraktion auszuführen. So kann beispielsweise ein neues Dokument hochgeladen oder ein Symptom erfasst werden. Das Ziel ist es, so leicht wie möglich und mit so wenigen Klicks wie nötig eine Aufgabe im Alltag zu erledigen. Befindet man sich in einem Modul selbst, verlagert sich diese Möglichkeit der Kerninteraktion in den sogenannten »Floating Action Button« unten rechts.

![](/assets/images/project_images/dicama/Folie4.PNG)

In den Modulen selbst gibt es ein zusätzliches und spezifisches unteres Menü. Dort gibt es drei wiederkehrende Elemente und ein flexibles Element. Das flexible Element stellt für die Entwickler:innen eines Moduls die Möglichkeit dar, eine weitere wichtige Interaktion prominent zu positionieren, z. B. eine Übersicht der favorisierten Dokumente im Dokumentenmanager oder die Erstellung eines Reports über Symptome. Die wiederkehrenden Elemente sind zum einen der Home-Button für das jeweilige Modul, um jederzeit von untergeordneten Ebenen auf die oberste Eben des Moduls zurückgelangen. Des Weiteren ist das ein Info-Button, der dazu dient, den Patient:innen Informationen über den aktuellen Screen zu geben. Diese Funktion soll die Patient:innen nicht nur unterstützen sich in neuen Modulen schneller und besser zurechtzufinden, sondern auch in schlechten kognitiven Zustand sich stets über die aktuellen Handlungen rückversichern zu können. Abschließend und falls erforderlich bzw. gewünscht können Entwickler:innen unter dem Menüpunkt „…“-Mehr weitere Interaktionsmöglichkeiten und Informationsfelder unterbringen.

Über mehrere Wege gelangen die Patient:innen zu dem Modulstore. Hier kann man sich wie einem gängigen Play- oder Appstore über weitere Module informieren und diese aktivieren bzw. wieder deinstallieren.

## Die Module

Zu Beginn der Recherche haben wir mit einer Umfrage in einer aktiven Patient:innen-Community ermittelt, welche Module relevant für ein gutes Krebsmanagement sind. Das Ergebnis diente als Orientierung welche Basismodule priorisiert werden sollten. Es zeigte sich, dass egal an welcher Form von Krebs ein:e Patient:in erkrankt ist, alle zum einen Medikamente und zum anderen Dokumente verwalten müssen. Als spezifisches Modul für den Fokus Darmkrebs ergab sich ein Stuhlgangstagebuch. Alle drei Module werden im folgenden kurz vorgestellt:

![](/assets/images/project_images/dicama/Folie5.PNG)

Das Tracking von Symptomen bedeutet bei Darmkrebs vor allem, den Stuhlgang entsprechend zu protokollieren. Dabei ermöglicht das Modul den Patient:innen neben der Erfassung von typischen Stuhlgangscharakteristika auch Assoziationen in Form von Tags mit einzelnen Eingaben zu verknüpfen. Sei es eine bestimmte unverträgliche Mahlzeit oder der Wechsel auf ein neues Schmerzmittel - der/die Patient:in kann so modulübergreifend Informationen miteinander verknüpfen und eventuell Rückschlüsse erhalten oder Impulse in das nächste Gespräch mit dem/der Ärzt:in einbringen. Für diesen Zweck gibt es die Möglichkeit, sich über die Reportfunktion eine Übersicht als PDF erstellen zu lassen, die man entsprechend ausdrucken oder mit dem/der Ärzt:in teilen kann.

![](/assets/images/project_images/dicama/Folie6.PNG)

Eine Krebserkrankung hat die Einnahme von etlichen und unterschiedlichsten Medikamenten zur Folge. Hierbei den Überblick zu behalten - sowohl in der Einnahme selbst als auch beispielsweise in der Bevorratung - ist eine elementare Aufgabe im Alltag von Krebspatient:innen. Für eine:n Patient:in kann es beispielsweise dramatische Konsequenzen haben, wenn Schmerzmittel plötzlich am Wochenende oder im Urlaub leer gehen. Auch hier lässt sich über die Reportfunktion eine Übersicht erstellen, die beispielsweise die vorgeschriebene Einnahme dokumentiert. Des Weiteren ist die Information über die aktuelle Einstellung der Medikation auch für Ärzt:innen und Pfleger:innen von großer Bedeutung, so dass auch hier mit wenigen Klicks der verordnete Plan als Foto-Scan erfassen, sich anzeigen und teilen lässt. An dieser Stelle kann beim Anzeigen, Bearbeiten oder Hinzufügen eines Medikamentenplan exemplarisch der fließende Übergang in die Dokumenten-Verwaltung als ein weiteres Basismodul veranschaulicht werden.

![](/assets/images/project_images/dicama/Folie7.PNG)

Ein:e Krebspatient:in hat nicht nur viele Medikamente zu nehmen, sondern auch Berge von Papier zu bewältigen. Von Arztbriefen, Medikamentenplänen, Blutwerten, Gutachten bis hin zu Rechnungen sammeln sich schnell mehrere Ordner an Papier. Diese zu digitalisieren ist aufgrund von guten Smartphone-Kameras und Scannern zwar keine große Herausforderung mehr, aber wenige Scan-Apps ermöglichen eine getrennte und sichere Ablage sowie eine dedizierte Suche. Mit dem Modul der Dokumentenverwaltung ist es leicht möglich mit wenigen Klicks ein Dokument zu digitalisieren und dabei nach einer vorgegebenen oder selbstgewählten Systematik abzulegen. Neben der Möglichkeit Dokumente spezifisch zu benennen und abzulegen, gibt es auch hier die Möglichkeit spezifische Assoziationen und Schlüsselbegriffe als Tag mit Dokumenten zu verknüpfen. Dadurch erhält der/die Patient:in die Möglichkeit einer schnellen Suche nach den jeweiligen Dokumenten.

[Link zur Demo](#)

## Technische Konzepte

![](/assets/images/project_images/dicama/Folie8.PNG)

Die Systemarchitektur hat das Ziel Modularität und Offenheit für Entwicklungen zu bieten, gleichzeitig aber auch Datenhoheit und Qualitätssicherung zu gewährleisten.

Eine erste grundlegende Entscheidung betrifft die Speicherung der Daten und die entsprechenden Zugriffsberechtigungen. Die Daten werden nur lokal auf dem Gerät gespeichert und entsprechend mit einem „Private Key“ verschlüsselt. Dieser wird in der Keychain des Gerät abgelegt und der/die Patient:in kann die App zusätzlich via Systemsperre (z. B. Pin oder Fingerabdruck) absichern. Für spätere Backup-Lösungen soll der/die Patient:in mit Hilfe des Private Key alle Daten und Einstellungen absichern oder auf ein anderes Gerät überspielen.

Um entsprechende Modularität und gleichzeitig Datenhoheit zu gewährleisten, gibt es einen zentralen Access Layer, in dem klar definiert wird, welche Module auf welche Daten zugreifen können. Im jetzigen Stand ist das zwar noch eher Theorie, aber im späteren Anwendungsfall, in dem Module von Dritten entwickelt worden sind, soll der/die Patient:in über Zugriffe auf Daten aufgeklärt werden, Zustimmung erteilen und die Möglichkeit haben, Zugriffsrechte entsprechend anzupassen. Dies erfolgt entweder bei einem ersten Start eines neuen Moduls oder über die Datenschutzansicht (über Schutzschild Symbol in Top-Menü). Damit hierbei eine fundierte Entscheidung sowohl vom vorgesehenen MONK Audit Team im Review-Prozess und später von dem/der Patient:in selbst getroffen werden können, müssen Entwickler:innen, die auf Daten anderer Module zurückgreifen, einen Grund hierfür angeben. Im Rahmen einer Qualitätskontrolle durch das Audit Team vor der Zulassung in den internen Modulstore sollen dabei sowohl technische als auch medizinische Aspekte überprüft und bewertet werden.

Entwickler:innen sollen es leicht haben neue Ideen umzusetzen oder konkrete Probleme zu lösen. Neben den Zugriffsmöglichkeiten auf erforderliche Daten (z. B. Vitalparameter anderer Module) wurde hierfür auch die Möglichkeit geschaffen auf Templates im Code zurückzugreifen. Eine eigens entwickelte Skriptsprache ermöglicht es, Module zu entwickeln ohne selbst coden zu müssen. Einfache Module, wie beispielsweise der Gewichttracker oder die inspirierenden Zitate, wurden als Proof of Concept so aufgesetzt.

## Technische Spezifikationen

![](/assets/images/project_images/dicama/archdiagram.PNG)

## Zielgruppe

Im aktuellen Rahmen des Prototype Funds liegt der Fokus zwar auf Darmkrebs, allerdings sind bereits zwei von drei Modulen im Zweck so universal gehalten, dass sie für jede Form der Krebserkrankung angewendet werden können. Langfristig ist der Anspruch, für jede Krebsform und jedes Stadium spezifische Module zu schaffen und die Basisfunktionalitäten wie z. B. Dokumentenverwaltung und Medikamentenplan stetig zu verbessern. Gerade Patient:innen mit einer Affinität für moderne digitale Lösungen und einem ausgeprägten Bewusstsein für Datenschutz sind die Hauptzielgruppe. Jedoch soll die intuitive Bedienungen auch andere Zielgruppen erschließen.

Da ein Open-Source-Projekt auch von der Attraktivität für Entwickler:innen lebt, wurden verschiedene Aspekte hierfür berücksichtigt. Zunächst wurde technisch auf Flutter als Programmiersprache gesetzt. Diese ist nicht nur im Trend und weist eine starke Community auf, sondern ermöglicht auch die Bereitstellung sowohl von Android- als auch iOS-Apps. Der grundlegende Gedanke mit technischen Fähigkeiten einfach und mittelbar Menschen mit einer schweren Krankheit zu helfen und dabei nicht das Rad komplett neu zu erfinden und es dann erst auf die Geräte der Patient:innen zu bringen, ist ein wichtiges Argument, um Entwickler:innen für das Projekt zu begeistern. Darüber hinaus hoffen wir mit dem Anspruch „etwas wie Linux für das Management von Krebs“ zu entwickeln, auf allgemeines Interesse und Neugier in der technischen Community zu stoßen.

Ein Hauptziel des Projekts ist es, in der Zukunft die beiden unterschiedlichen Zielgruppen auch miteinander zu verknüpfen und verbünden. Bedarfe kommunizieren, Patient:innen und Entwickler:innen in den Dialog bringen, gegenseitiges Verständnis für Probleme schaffen, um eine schreckliche Krankheit ein kleines bisschen erträglicher zu machen und dabei auch gemeinsam Spaß an dieser sinnstiftenden Tätigkeit zu haben.

## Nächste Schritte

Im Rahmen einer feierlichen „Übergabe“ soll das Projekt vorübergehend dem gemeinnützigen Technologieverein Health Hackers e. V. aus Erlangen anvertraut werden, in dem das Projekt auch seinen Ursprung hatte und der Teil des Digital Health Hub Erlangen-Nürnberg ist. In den nächsten Schritten sollen der Aufbau der Tech Community und die Beta-Tests mit Patient:innen vorangetrieben werden. Parallel dazu stehen Überlegungen, eine eigene Stiftung nach dem Vorbild der Linux oder Mozilla Foundation zu gründen. Hierfür suchen wir aktiv Fördermitglieder und mögliche Sponsoren, die an die Idee glauben und diese unterstützen möchten. Bei Interesse gerne per Mail Kontakt mit Susanna (Krebskriegerin@web.de) und Christian (christian@healthhackers.de) aufnehmen.

## Team

Dennise Cepeda (UI / UX), Jonas Jung (UI / UX), Christian Schulz (Konzept / PM), Christoph Speier (Entwicklung), Sebastian Schroth (Entwicklung), Sebastian Schneider (Entwicklung) und die wundervolle „Krebskriegerin“ Susanna Zsoter (Feedback / Marketing)\*

\*ehrenamtliche Beteiligung aufgrund ihrer außergewöhnlichen gesundheitlichen Situation

## Danksagung

Wir bedanken uns herzlich bei:

Den wundervollen Patient:innen insbesondere Jenny, der gesamten Health Hacker Community insbesondere AlexQ und Felix Gundlack.

Allen Sponsoren für die damalige finanzielle Unterstützung die Idee im Rahmen des Cancer Management Hackathon im Oktober 2019 zu validieren insbesondere Novartis, Roche, Janssen Oncology, Proact, EIT Health, Sparkasse Erlangen, Curry Solution und dem Bayerischen Staatsministerium für Wirtschaft, Landesentwicklung und Energie.

Dem Prototype Fund für diese großartige Möglichkeit unsere Idee voranzutreiben und insbesondere bei Marie und Thomas sowie den anderen Coaches von Simple Secure.

Dem Bundesministerium für Bildung und Forschung für die Förderung. Dem Projektträger DLR insbesondere Frau Luckmann und Herr Konle für Ihre geduldige Art uns bei den administrativen Aufgaben zu unterstützen.

Letztendlich vor allem auch unseren Familien, Partner:innen und Freund:innen, die uns wegen des Projekts und der Hack-Session an den Wochenenden zeitweise entbehren mussten.

Kein Dank geht an Covid-19, dass zwar viel Ablenkung von uns „ferngehalten“ hat, aber dafür gesorgt hat, dass die Zusammenarbeit nur remote ablief.

## Links

Github: [https://github.com/dicama](https://github.com/dicama)

Demo: [Link Appetize.io Demo](https://appetize.io/app/4pt777c1yb0f2vmayummg063e4?device=pixel4&scale=75&orientation=portrait&osVersion=10.0)

Website: [www.monk-app.de](http://www.monk-app.de/)

Kontakt: [e-mail](mailto:info@monk-app.de)
