---
layout: project
title: "Direkte Demokratie Digital"
image: /assets/images/project_images/direkte-demokratie-digital/header.png
authors:
  - author: Laura Brämswig
    link:
  - author: Joy Ponader
    link:
  - author: Timur Celikel
    link:
  - author: Valentin Schagerl
    link:
  - author: Julia Baumhauer
    link:
brief: "Wir helfen dabei, Volksbegehren durchzuführen."
summary: "Das Direkte-Demokratie-Digital-Tool ermöglicht es Kampagnen eine Volksinitiativen-Plattform zu erstellen und hilft ihnen den analogen Prozess des Unterschriftensammelns digital zu unterstützen."
---

# Was steckt hinter dem Projekt?

Der deutsche Staat stellt seinen Bürger:innen gewisse Möglichkeiten zur direkten gesetzlichen Mitbestimmung zur Verfügung. Wir glauben, dass diese ein wichtiger Bestandteil einer gesunden Gesellschaft sind und eine Stärkung der direkten Demokratie sich positiv auf das gesellschaftliche Klima und die Qualität politischer Entscheidungen auswirken würde. Deshalb haben wir ein Projekt entwickelt, welches den Zugang zu direktdemokratischen Mitteln erleichtern soll.

In Deutschland gibt es kaum direktdemokratische Mittel auf Bundesebene. Deshalb finden die wichtigsten direktdemokratischen Verfahren entweder auf kommunaler Ebene oder auf Bundesländer-Ebene statt. Sie sind meist mehrstufig und unterscheiden sich in ihrem genauen Ablauf je nach Bundesland oder Kommune.
Eines ist jedoch allen Verfahren gemeinsam: Die notwendigen Unterschriften müssen analog auf Papier eingesammelt werden. Für potentielle Unterstützer:innen einer Initiative kann dies eine gewisse Hürde bedeuten. Zudem ist es durch die Corona-Krise schwieriger geworden, analoge Sammelaktionen zu organisieren und durchzuführen.
Eine Digitalisierung dieses Sammelprozesses wäre hier von großer Hilfe. Sie würde den Zugang zu den Mitteln der direkten Demokratie erleichtern und somit eine breite Mitbestimmung in größeren Teilen der Bevölkerung erlauben.
Es muss möglich sein, dass Bürger:innen unter Berücksichtigung der Corona-Auflagen weiter an direktdemokratischen Prozessen teilnehmen können. Eine Digitalisierung der Unterschriften-Sammlung ist ein wichtiger Schritt in diese Richtung.

Dieses Problem hat auch die gemeinnützige Organisation "Expedition Grundeinkommen" erkannt, die mit den Mitteln der direkten Demokratie einen staatlichen Modellversuch zum bedingungslosen Grundeinkommen herbeiführen möchte.
2019 entwickelte die Expedition Grundeinkommen ein Tool, welches das Sammeln analoger Unterschriften vereinfacht.

Im Jahr 2020 wünschten sich einige Mitglieder der Expedition, dieses Tool weiter zu entwickeln, so dass es auch andere Volksinitiativen nutzen können. Aus diesen Mitgliedern entstand unser Team “Direkte Demokratie Digital”.

Unser Team ist seit Jahren politisch interessiert und engagiert, wir vermissen aber häufig die Gestaltungsmöglichkeit einzelner Bürger:innen und Gruppierungen in der heutigen Gesellschaft. Da wir alle aus persönlicher Motivation heraus den Wunsch haben, die direkte Demokratie in Deutschland zu stärken, sahen wir im Tool der Expedition ein großes Potential. Unser Ziel ist es, allen Volksinitiativen in Deutschland einen niedrigschwelligen Zugang zur analogen Unterschriftensammlung zu ermöglichen und es damit mehr Menschen zu erleichtern, sich an direktdemokratischen Prozessen zu beteiligen.

## Der Plan: Ein digitales Tool für alle Volksinitiativen

Deshalb implementierten wir im Rahmen dieses Projekts ein Werkzeug zur Erstellung von Plattformen für Volksinitiativen. So sollen Kampagnen, die keine Kapazitäten dafür besitzen, eine eigene Webanwendung zu konzipieren, designen und programmieren, von unserer vergangenen und auch zukünftigen Arbeit profitieren. Dabei war es uns von großer Bedeutung, dass die Flexibilität und die Möglichkeiten, die Plattform den eigenen Wünschen anzupassen, möglichst wenig eingeschränkt wird. Kampagnen sollten mittels unseres Baukastens ihre eigene Infrastruktur aus dem Nichts generieren können und so alleinig Zugriff auf ihre Daten besitzen.

Das Herzstück der Plattform ist ein Tool, dass es Nutzer:innen ermöglicht, Unterschriftenlisten als PDF herunterzuladen und auszudrucken. Auf jeder Liste ist ein Barcode aufgedruckt, welcher die Liste identifiziert. Wenn die Liste im Büro der Kampagne ankommt, kann sie mit einem Barcode-Scanner gescannt werden und die eingegangene Zahl der Unterschriften wird im System automatisch gespeichert. Die eingegangene Zahl der Unterschriften wird dann auf der Website in Echtzeit in Form eines Fortschrittsbalkens angezeigt. Die Absenderin bekommt außerdem automatisch eine E-Mail, dass ihr Brief im Büro angekommen ist und die Unterschriften erfolgreich im System gespeichert wurden. In ihrem Profil können User:innen die Anzahl ihrer gesammelten Unterschriften bestaunen, ein Profilbild hochladen oder weitere Einstellungen vornehmen.

Auf diese Weise wird das analoge Unterschreiben vereinfacht und durch das direkte Feedback auch motivierender. Der steigende Fortschrittsbalken animiert Unterstützer:innen dazu, im Bekanntenkreis mehr Unterschriften zu sammeln, um den Balken weiter wachsen zu sehen. Außerdem lassen sich auf diese Weise auch Menschen erreichen, welche unter anderen Umständen möglicherweise nicht mit der Unterschriftensammlung in Berührung gekommen wären.

Um das Tool der Expedition mittels Abstrahierung durch andere Initiativen einbinden zu lassen, haben wir die unterschiedlichen Komponenten als NPM-Packages restrukturiert. Bei den drei Modulen handelt es sich um das Frontend, das Backend und das Admin Panel. Siehe hierzu “Gatsby-Theme”, “Serverless Architektur” und “Admin Panel”. Um Kampagnen, die unser Tool verwenden wollen, die Einbindung und Anpassung dieser Komponenten möglichst einfach zu ermöglichen, haben wir zudem ein CLI-Tool geschrieben (siehe “CLI-Tool und Komponenten”). Dieses führt die Kampagnen durch den Prozess der Konfiguration, der Generierung der Infrastruktur, des Aufsetzens eines Content-Management-Systems (siehe “Contentful”) und des Deployments (siehe “Netlify”).

Dieser Prozess soll auch von Nicht-Expert:innen ohne weitere Probleme durchlaufen werden können. Bei noch mehr gewünschter Flexibilität und größerer technischer Expertise können weitere Anpassungen an Funktionalitäten vorgenommen werden. Unser Baukasten strebt jedoch bereits ein hohes Maß an Flexibilität an. So kann das Design und die Struktur des Frontends den eigenen Wünschen entsprechend festgelegt werden. Des Weiteren kann das Design und der Text automatisierter E-Mails angepasst oder es kann definiert werden, wie viele verschiedene Kampagnen es geben soll (falls eine Initiative z.B. in mehreren Bundesländern aktiv ist).

## Hinter den Kulissen

### CLI-Tool und Komponenten

Kampagnen, die unser Tool verwenden wollen, werden mittels einer CLI durch den Konfigurationsprozess geführt.

So werden zum Einen essentielle Informationen wie Zugangsdaten für Contentful-, Netlify- und AWS-Account abgefragt. Diese müssen jeweils im Vorfeld durch die Initiativen erstellt werden. Für die Einbindung von Contentful als Content-Management-Systems und Netlify für das Hosting der Webseite fallen keine Kosten an. Die Preise für die Nutzung von AWS hängen, wie es für Cloud Computing typisch ist, von HTTP-Anfragen, Datentransfer, etc. ab.

<figure>
  <img src="/assets/images/project_images/direkte-demokratie-digital/cli.png" alt="CLI"/>
  <figcaption>Bild 1: Konfiguration in der CLI</figcaption>
</figure>

Die einzelnen Komponenten werden auf Basis der Einstellungen konfiguriert. Daraufhin hat die Kampagne die Möglichkeit, weitere Anpassungen durchzuführen: Das Farbschema anpassen, ein Logo hinzufügen, etc. Schließlich werden alle Komponenten deployt. Sobald dieser Prozess abgeschlossen ist, kann die eigene Webseite bewundert werden. Die Verknüpfung der Einzelteile (z.B. Frontend und Serverless Backend) wurde im Hintergrund durch unsere Skripte durchgeführt.

Im Folgenden werden die einzelnen Komponenten, deren Zweck und Anwendung detaillierter beschrieben.

### Wiederverwendbarkeit des Frontend-Codes: Gatsby-Theme

Unser Frontend-Code ist in React geschrieben. Als Framework für den Build der Website und als Static-Site-Generator verwenden wir Gatsby.

Ein äußerst praktisches Abstraktions-Feature von Gatsby sind Themes. Mit leichten Anpassungen kann so der Code für eine Webseite als Schema für viele ähnliche Webseiten zur Verfügung gestellt werden. Das Besondere an Gatsby-Themes ist die Möglichkeit jede Datei, die vom Theme bereitgestellt wird, mit einer eigenen zu überschreiben. Dieses sogenannte „Shadowing“ nutzen wir beispielsweise, damit in wenigen Konfigurations-Dateien Variablen zur Anpassung des Designs und Farbschemas überschrieben werden können. Auch das Logo der Kampagne kann so flexibel in verschiedenen Dateiformaten in einem dafür vorhergesehenen Ordner abgelegt werden. Ein weiterer Vorteil ist, dass die Details der Implementierung nur insoweit im Projektordner der Kampagne sichtbar sind, wie sie tatsächlich benötigt werden, das Theme an sich ist nur als NPM-Package eingebunden.

### Content-Managment-System: Contentful

Damit die Inhalte der Webseite getrennt vom Code editierbar sind und inhaltliche Änderungen nicht nur von Entwickler:innen ausgeführt werden können, verwenden wir das Content-Management-System (CMS) von Contentful. Grundlegende Entscheidungen zur Seitenstruktur, wie die Haupt- und Footer-Navigation, können hier definiert werden, aber auch der Aufbau einzelner Seiten kann individuell angepasst werden. Außerdem können die Inhalte der Seite, wie Texte, Bilder und Visualisierungen hier festgelegt werden.

Bei der ersten Konfiguration durch das CLI-Tool wird ein Starter-Template in den Contentful-Account der Kampagne kopiert, das alle verfügbaren Features veranschaulicht und von Texten begleitet wird, die einen kurzen Überblick geben, wie diese im CMS angepasst werden können.

<figure>
  <img src="/assets/images/project_images/direkte-demokratie-digital/screenshot.jpg" alt="Website screenshot"/>
  <figcaption>Bild 2: Startseite des Starter-Templates</figcaption>
</figure>

Unser Ziel ist es eine möglichst große Flexibilität im CMS herzustellen, sodass für einen einfachen Anwendungsfall nach der Einrichtung kein Expertenwissen nötig ist, die Seite anzupassen und zu erweitern.

### Hosting: Netlify

Anstatt die durch Gatsby erstellten statischen Seiten auf einem eigenen Server zu hosten, bieten wir Kampagnen an, mit unserem CLI-Tool die Seiten beim Anbieter Netlify zu deployen. Unser Tool bindet im Hintergrund die Netlify-CLI ein, die den Login und den Upload der Webseiten-Daten regelt. Im einfachen Anwendungsfall können Aktualisierungen der Webseite dann immer wieder erneut über die CLI generiert und hochgeladen werden. Für erfahrenere Anwender bieten wir auch eine Anleitung an, wie dieser Prozess automatisiert werden kann, wenn ein Repository auf GitHub für den Code erstellt wird.

### Serverless Architektur

Das Backend basiert auf einer Serverless Architektur. Sie bezeichnet eine Form des Cloud Computing, bei der Infrastruktur und Code nicht selber gehostet werden müssten, sondern durch einen Cloud Anbieter (hier AWS) verwaltet werden. Zwar kommt das Backend nicht wortwörtlich ohne Server aus, aber die Aufgaben der Provisionierung, Skalierung und Verwaltung werden ausgelagert.

Für die Umsetzung wird hierzu das Serverless [Framework](https://www.serverless.com/) zur Hilfe genommen. Dies bietet im Kontext dieses Projektes den großen Vorteil, dass nicht nur Code des Backend mittels des NPM-Packages repliziert werden kann, sondern sogar die gesamte Infrastruktur im Vorhinein definiert werden kann. Sprich: Datenbank-Tabellen, Einstellungen der HTTPS-Schnittstellen, Autorisierungs-Schichten und Events wurden durch uns in einer YAML-Datei konfiguriert. Während des erstmaligen Deployments wird die komplette Infrastruktur in der Cloud aufgebaut. Diese Form der Konfiguration wird _Infrastructure as code_ (IaC) genannt.

### Admin Panel

Eine weitere essentielle Komponente unseres Projektes ist das Admin Panel. Ohne die Funktionalitäten, die das Programm bietet, wäre unser Tool für Kampagnen nicht in sinnvollem Maße nutzbar. Es handelt sich hierbei um eine vom Frontend unabhängige React App, die genau wie die Webseite ebenfalls zu Netlify deployt wird und auf Endpunkte des Backends zugreift. Das Admin Panel bietet dabei zum Beispiel folgende Möglichkeiten:

- Eintragen von Unterschriften: Angekommene Unterschriften einer Kampagne werden eingetragen. Daraufhin wird automatisiert eine Benachrichtigung per E-Mail an die Person, von der die Unterschriftenliste stammt, gesendet (siehe Bild 4).
- Statistiken und Graphen zur Analyse der Daten: Zum Beispiel kann eingesehen werden, wie viele Unterschriften bereits angekommen sind, sowie sogar die chronologische Entwicklung der Zahlen (siehe Bild 5).
- Außerdem: Spendenübersicht, User:innen-Suche, etc.

<figure>
  <img src="/assets/images/project_images/direkte-demokratie-digital/pic3.png" alt="Unterschriften eintragen"/>
  <figcaption>Bild 3: Unterschriften eintragen</figcaption>
</figure>

<figure>
  <img src="/assets/images/project_images/direkte-demokratie-digital/pic4.png" alt="Unterschriftenverlauf"/>
  <figcaption>Bild 4: Unterschriftenverlauf</figcaption>
</figure>

### Unsere Learnings

Abgesehen von inhaltlichen und technischen Lernprozessen haben wir uns vor allem darüber gefreut, dass wir aus dem Projekt wichtige Learnings im Bereich Abläufe, Abstimmungen und Koordination mitnehmen können. Zum Beispiel waren wir uns anfangs nicht sicher, als wir einen relativ detaillierten Zeitplan mit Etappen-Deadlines ausgearbeitet hatten, ob wir uns tatsächlich daran halten können würden. Im Verlauf des Projekts hatten wir zwar zwischendurch auch Rückstände zu unserem Zeitplan, wussten aber dann genau, wann wir diese wieder einholen können.
Eine Aufgabe, die wir zeitlich jedoch unterschätzt haben, ist die Dokumentation. Dafür haben wir zwar früh ein gemeinsames Dokument aufgesetzt, aber waren ein bisschen nachlässig mit der Pflege desselben. Hier könnten wir in Zukunft die Dokumentation in der Review mit einschließen, damit es eine höhere Verbindlichkeit gibt, diese als Teil eines Features oder einer Etappe zu sehen.
Für unseren Ablauf war es auch sehr hilfreich Peer-Programming Sitzungen zu machen, insbesondere am Anfang, wenn ein neues Feature geplant wurde. Dadurch hatten wir schnell ein gemeinsames Bild von den grundlegenden Entscheidungen und konnten schnell identifizieren, wer welche Detailausarbeitungen übernehmen kann.

Inhaltlich, beziehungsweise technisch, waren viele Learnings an unser konkretes Projekt gebunden und wahrscheinlich nur für ähnlich gelagerte Projekte relevant. Grundsätzlich kann man jedoch sagen, dass wir in Zukunft bei der Planung einer Abstraktion zu Anfang mehr Zeit in die Recherche investieren wollen, ob die Technologie, die wir verwenden möchten, schon eine Schnittstelle zur Abstraktion anbietet. Im Frontend hatten wir zum Beispiel schon einen aufwendigen Prozess entwickelt, wie der bereits bestehende Code von einer anderen Initiative flexibel angepasst und dann auch gebundelt werden kann. Wir sind erst später auf die Möglichkeit gestoßen ein Gatsby-Theme zu erstellen, das dafür schon eine sehr komfortable und flexible Schnittstelle bietet. Für unser CLI-Tool haben wir dann auf die CLI-Tools von Contentful und Netlify zurückgegriffen, was uns zum Beispiel die Autorisierung bei diesen Anbietern sehr erleichtert hat.

### Nächste Schritte und Perspektive

Wir sind stolz auf das, was wir zu Ende des Förderzeitraums erreicht haben. Dennoch sehen wir viel weiteres Potential für unser Projekt. Dies ist unsere Vision:

- Wir wollen, dass möglichst viele Initiativen das Tool nutzen
- Wir wollen, dass direkte Demokratie gestärkt wird
- Langfristig wollen wir, dass das Unterschriftensammeln digitaler und einfacher wird. Dafür streben wir auch eine Zusammenarbeit mit anderen Organisationen an, die dasselbe Ziel verfolgen

Es gibt noch viele Möglichkeiten, die Plattform weiter zu entwickeln. Da die Website der Expedition Grundeinkommen auf diesem Projekt aufbaut, werden zukünftige Änderungen und Weiterentwicklungen der Expeditions-Webseite auch ihren Weg zurück in die Plattform finden. Geplante Änderungen beinhalten das Ausbauen des Profilbereichs der Seite, das Schaffen von Vernetzungsmöglichkeiten bei Unterstützer:innen, sowie die Einbindung von zusätzlichen Möglichkeiten der Unterschriftensammlung und des Organizing.

Damit möglichst viele Organisationen von unserer Arbeit profitieren können, freuen wir uns über Unterstützung und Input aus der [Open Source Community](https://github.com/grundeinkommensbuero/direct-democracy-digital). Manche der möglichen geplanten Anpassungen sind vom Umfang her durchaus ambitioniert. Jegliche Mithilfe am Projekt ist daher herzlich willkommen!
Wir freuen uns, wenn das Projekt mithilfe der Gemeinschaft weiter wächst und der direkten Demokratie in Deutschland dadurch Aufschwung verleiht.

Wir danken dem BMBF für die Ermöglichung des Projektes.
