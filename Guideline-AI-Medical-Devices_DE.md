# Leitfaden zur KI bei Medizinprodukten

> Hinweis: Dieser Leitfaden befindet sich noch in der Entwicklung!

## A) Metainformationen

### 1. Ziele des Leitfadens

Dieser Leitfaden hat das Ziel, Medizinprodukte-Herstellern und Benannten Stellen eine Handlungsanleitung und eine konkrete Checkliste an die Hand zu geben, um

- zu verstehen, was die Erwartungen der Benannten Stellen sind,
- die schrittweise Umsetzung der Sicherheit von Medizinprodukten zu befördern, die Verfahren der künstlichen Intelligenz, insbesondere des maschinellen Lernens einsetzen,
- das Fehlen einer harmonisierten Norm (zwischenzeitlich) bestmöglich zu kompensieren.

Der Leitfaden hat **nicht** die Zielsetzung, als Lehrbuch oder Leitfaden für das Erreichen der Sicherheit von KI-basierten Medizinprodukten zu dienen. Vielmehr möchte er ein Leitfaden für deren Überprüfung sein.

Der Anhang nennt die Erwägungsgründe, die zur Entwicklung dieses Leitfadens führten.

### 2. Anwendungsbereich und Zielgruppe

Dieser Leitfaden ist nur für Medizinprodukte anwendbar, die Verfahren der KI, insbesondere des maschinellen Lernens verwenden. Der Leitfaden wendet sich insbesondere an 

- Hersteller dieser Produkte
- deren Dienstleister (z.B. Entwicklungsdienstleister)
- Personen und Organisation, die die Sicherheit dieser Produkte bewerten müssen, wie beispielsweise Auditoren, Behörden und Benannte Stellen.

### 3. Hinweise zur Verwendung

#### a) Aufbau des Leitfadens

Dieser Leitfaden folgt dem Gedanken, dass die Sicherheit KI-basierter Medizinprodukte nur durch einen prozessorientierten Ansatz erreicht werden kann, wobei alle relevanten Prozesse und Phasen des Lebenszyklus betrachtet werden müssen wie:

1. Forschung und Entwicklung
2. Datenmanagement
3. Überwachung nach der Inverkehrbringung

Entsprechend stellt der Leitfaden keine spezifischen Anforderungen an die Produkte, sondern an die Prozesse. Er enthält die folgenden Kapitel:

1. Allgemeine Anforderungen
2. Anforderungen an die Produktentwicklung
   1. Zweckbestimmung
   2. Software-Anforderungsspezifikation
   3. Datenmanagement
   4. Modellentwicklung
   5. Produktentwicklung
   6. Produktfreigabe
3. Anforderungen an die der Entwicklung nachgelagerten Phasen

#### b) Verbindlichkeit des Leitfadens

Dieser Leitfaden ist weder eine gesetzliche Anforderung noch eine harmonisierte Norm. Entsprechend unterscheidet er auch nicht zwischen normativen und informativen Elementen.

Dieser Leitfaden trägt Best Practices zusammen, um den gesetzlich geforderten "State-of-the-Art" bestmöglich zu beschreiben. Dabei ist zu berücksichtigen, dass eine Fokussierung allein auf diesen "State-of-the-Art" auch zur Entwicklung von Produkten mit geringem Nutzen und sogar Schaden für den Patienten führen und insofern für sich genommen kein hinreichendes Kriterium sein kann.

Einige dieser Best Practices sind daher nicht in allen Situationen, bei allen Produkten oder bei allen Verfahren des maschinellen Lernens anwendbar. Hersteller sollten nicht offensichtliche Ausschlüsse begründen.

#### c) Verwendung des Leitfadens

##### Vorgabedokumente erstellen und prüfen

Die Hersteller sollten den Leitfaden zuerst nutzen, um die Vollständigkeit der Vorgabedokumente (Verfahrens- und Arbeitsanweisungen, Checklisten usw.) zu prüfen. Diese Aufgaben obliegen üblicherweise den folgenden Rollen:

- Prozesseigner insbesondere Entwicklungsleiter
- Qualitätsmanager und Qualitätsmangementbeauftragte
- Regulatory Affairs Manager

##### Produkte und QM-Systeme bewerten

Anschließend sollten die Personen den Leitfaden nutzen, die für die folgende Aufgaben zuständig sind:

- Die Konformität der Produkte mit grundlegenden Sicherheit- und Leistungsanforderungen überprüfen
- Die Konformität der technischen Dokumentation mit den regulatorischen Anforderungen bewerten
- Die Wirksamkeit des eigenen Qualitätsmanagementsystems bewerten (z.B. bei Design-Reviews oder bei Audits)

Für diese Aufgaben sind üblicherweise die folgenden Rollen zuständig:

-  Qualitätsmanagementbeauftragte
- Externe und interne Auditoren (einschließlich Benannte Stellen)
- Interne und externe Prüfer von technischen Dokumentationen (einschließlich Benannte Stellen und Behörden)
- Tester
- Data Scientists
- Clinical Affairs Spezialisten
- Regulatory Affairs Manager
- Risikomanager

#### d) Struktur des Leitfadens

Der Leitfaden ist eine  nach den oben erwähnten Kapitel gruppierte Liste an Überprüfungskriterien. Jedes Listenelement enthält die folgenden Attribute:

- Eindeutige ID
- Überprüfungskriterium, des möglichst einfach und binär als erfüllt oder nicht-erfüllt bewertet werden kann
- Kommentare

Die Kommentare enthalten beispielsweise:

- Hinweis bzw. Referenz auf regulatorische Anforderung
- Empfehlung zur Umsetzung oder einen Verweis auf weitere Erläuterungen dazu
- Tipps für Auditor, wie die Erfüllung des Kriteriums geprüft werden kann
- Hinweise zur Verbindlichkeit und Anwendbarkeit und Einschränkungen

### 4. Autoren und Nutzungsrechte

Diesen Leitfaden haben die folgenden Autoren verfasst:

- Prof. Dr. Christian Johner ([Johner Institut](https://www.johner-institut.de))
- [Christoph Molnar](https://christophm.github.io/) ([LMU München](https://www.uni-muenchen.de/index.html))
- TODO: Dr. Andreas Purde, Dr. Abtin Rad ([TÜV SÜD](https://www.tuev-sued.de/))
- Prof. Dr. Christian Dierks ([Dierks + Company](https://www.dierks.company/))
- TODO ([Merantix](https://www.merantix.com/healthcare/))

Der Leitfaden ist unter der [Creative Commons Lizenz](https://creativecommons.org/licenses/?lang=de) vom Typ [BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/) veröffentlicht. Diese erfordert die Namensnennung der Autoren ("Christian Johner, Christoph Molnar et al. ") und erlaubt es Dritten, auf diesem Werk aufzubauen z.B. es zu verbessern; letzteres allerdings nur zu nicht-kommerziellen Zwecken.

Die Lizenz gestattet es, das Produkt zu Beratungszwecken einschließlich Audits kommerziell einzusetzen. Sie untersagt es aber, dieses Werk selbst in unveränderter oder veränderter Version kommerziell zu nutzen z.B. in Form eines Verkaufs als Broschüre.

### 5. Dokumentenlenkung, Dokumentenidentifikation

Dieses Dokument wird über das Versionsverwaltungssystem git bzw. die Plattform GitHub verwaltet. Einzig die in diesem Repository genannten Dokumente sind gültig.

Die Versionshistorie einschließlich der jeweiligen Autoren kann der Dokumentenhistorie entnommen werden.

Die freigegebenen Versionen sind über einen Tag im Repository als solche gekennzeichnet. Versionen ohne Tag sind Dokumente im Entwurfsstadium.

## B) Allgemeine Anforderungen

### 1. Prozesse

Die Hersteller sollten alle unten genannten Aspekte entweder in den Verfahrensanweisungen oder in den entsprechenden Plänen abdecken, um zu gewährleisten, dass die Sicherheit der Produkte systematisch gewährleistet wird. Üblicherweise sind die folgenden Verfahrensanweisungen bzw. Pläne betroffen:

- Entwicklung
- Risikomanagement
- Datenmanagement
- Verifizierung und Validierung (falls nicht Teil der Entwicklung)
- Überwachung der Produkte nach der Inverkehrbringung (Post-Market Surveillance) und Vigilanz
- Service, Installation, Außerbetriebnahme
- Kundenkommunikation
- Managementbewertung (ISO 13485:2016 fordert "anwendbare neue oder überarbeitete regulatorische Anforderungen" zu berücksichtigen.)

Nutzt der Hersteller ausgelagerte Prozesse, so gelten die Anforderungen entsprechend. Beispielsweise müsste ein (Software-)Entwicklungsdienstleister oder eine externe Auftragsforschung verpflichtet werden, die  relevanten Kapitel dieser Leitlinie zu beachten.

### 2. Kompetenzen

Die Hersteller müssen sicherstellen und nachweisen, dass sie über ausreichend Kompetenzen verfügen, um eine dem Stand der Technik entsprechende Sicherheit und Leistungsfähigkeit der Produkte zu gewährleisten. Diese Nachweise gelingen oft am leichtesten durch interne oder externe Schulungen.

Hersteller können dabei auch auf die Kompetenz externer Ressourcen zugreifen.

|Anforderung|Kommentare|
|:--|:--|
|Der Hersteller hat eine Liste aller Rollen erstellt, die mit dem Thema KI direkt oder indirekt befasst sind [^B2-01]||
|Der Hersteller hat für jede Rollen die Kompetenzen mit Bezug zur KI bestimmt [^B2-02]|Beispiele für Kompetenzen: Machine Learning, Explainable AI, Medizin (für entsprechende Domäne), klinische und Usability-Validierung|
|Der Hersteller hat angemessene Aufzeichnungen über die Ausbildung, Weiterbildung und Kompetenzen, die den Schluss erlauben, dass die Personen tatsächlich über diese Kompetenzen verfügen||
|Die (Software-)Entwicklungspläne legen produktspezifisch die (darüber hinausgehenden oder abweichenden) Kompetenzen fest|Anforderung der ISO 13485:2016|

[^B2-01]: Beispiele sind: Data Scientists, Entwickler, Tester, Regulatory Affairs und Qualitätsmanager, Mitarbeiter in Service und Support, Produktmanager, Medizinprodukteberater, Ärztinnen und Ärzte

[^B2-02]: Es sollten Kompetenzen (verstehen, können) und nicht primär Themen genannt sein

### 3. Dokumentation

Die Hersteller sollten den Nachweis führen können, die relevanten Anforderungen dieser Leitlinie beachtet zu haben. Es gibt keine spezifischen Anforderungen an die Dokumentation und "Objective Evidence".

Es besteht zumindest in Europa keine Pflicht, ein spezifisches Dokument zu erstellen, das die Aktivitäten speziell zur KI zusammenfasst. Vielmehr können Hersteller diese Aspekte in bereits bestehenden Dokumenten wie den Vorgabedokumenten des QM-Systems und der technischen Dokumentation (z.B. Software-Akte, Risikomanagementakte, klinische Bewertung, summative Bewertung der Gebrauchstauglichkeit) integrieren.

## C) Anforderungen an die Produktentwicklung

### 1. Zweckbestimmung und Stakeholder-Anforderungen

#### a) Zweckbestimmung

|Anforderung|Kommentare|
|:--|:--|
|Der Hersteller hat festgelegt, für welches medizinische Ziel (Diagnose, Therapie, Überwachung Vorhersage) das Medizinprodukt eingesetzt werden soll.|Die Zweckbestimmung ist nicht mit der Beschreibung von Funktionalität (z.B. Berechnung von Scores)  zu verwechseln.|
|Der Hersteller hat die Patienten charakterisiert, die mit dem Medizinprodukt diagnostiziert, behandelt oder überwacht werden sollen. Diese Charakterisierung schließt Indikationen, Kontraindikationen und Begleiterkrankungen mit ein.|Diese Charakterisierung fordert auch die IEC 62366-1. Patienten können gleichzeitig auch Nutzer (Anwender) des Produkts sein.|
|Der Hersteller hat festgelegt, an welcher Körperstelle das Produkt angewendet wird bzw. von welcher Körperstelle diese Daten stammen.|Diese Festlegung fordert auch die IEC 62366-1.|
|Die Zweckbestimmung lässt auch erkennen, welches Ziel die Verfahren des maschinellen Lernens verfolgen.|Klassifikation und Regression, Clustering, Similarity Search und Recommender Systems sind typischen Ziele von Verfahren des maschinellen Lernens.|

#### b) Vorhergesehene Nutzer, vorhergesehener Nutzungskontext

| Anforderung                                                  | Kommentare                                                   |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| Der Hersteller hat die vorgesehenen Nutzer charakterisiert z.B. anhand demographischer Merkmale (Alter, Geschlecht), bezüglich der Ausbildung, der Erfahrung in der medizinischen Domäne, bezüglich der technischen Kenntnisse, körperlichen und geistigen Einschränkungen, sprachlichen Fähigkeiten und kulturellem Hintergrund. | Wenn der Hersteller keine Einschränkungen bezüglich dieser Attribute vorsieht, muss er das auch dokumentieren. |


#### c) Stakeholder-Anforderungen

| Anforderung                                                  | Kommentare                                                   |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| Der Hersteller hat die in der Zweckbestimmung genannten Ziele mit quantitativen Werten operationalisiert [^C.1.c.1]. | Es ist nicht unüblich, dass diese Werte im Lauf der Entwicklung ergänzt und angepasst werden. |
| Der Hersteller hat die Laufzeitumgebung des Produkts bezüglich Hardware (Bildschirmgröße, Bildschirmauflösung, Speicher, Netzwerkanbindung etc.) und Software (z.B. Betriebssystem, Browser, Run-time Environments wie Java Run-time Environment oder .NET) bestimmt. | Bei Apps kann es sein, dass diese Charakterisierung für die App und für den Server-Teil erfolgen muss. |
| Der Hersteller hat alle Märkte und alle dort relevanten regulatorischen Anforderungen festgelegt. | Diese Liste sich zeigen lassen.                              |
| Der Hersteller hat festgelegt, ob das System nach der Inverkehrbringung weiter dazulernen soll. Falls dies der Fall ist, hat der Hersteller dargelegt, ob dieses kontinuierliche Training global/zentral oder dezentral (z.B. pro Produkt oder pro Krankenhaus) sowie online oder offline erfolgt. |                                                              |

[^C.1.c.1]: **Beispiel**: Zweck: Die Software unterstützt Radiologen beim Diagnostizieren von Krebserkrankungen anhand CT-Bilder des Schädels. Quantitativer Wert: 95% der Radiologen, die mit der Software arbeiten, erkennen den Krebs. 


#### d) Input für Risikomanagement und die klinische Bewertung

| Anforderung                                                  | Kommentare                                                   |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| Der Hersteller hat alternative Verfahren aufgelistet und bezüglich Nutzen, Sicherheit und Leistungsfähigkeit bewertet. | Die Diskussion des State-of-the-Art ist eine Forderung der MEDDEV 2.7/1 und der MDR/IVDR. |
| Der Hersteller hat die o.g. quantitativen Werte mit den entsprechenden Größen der alternativen Verfahren verglichen. | Hersteller sollten eine tabellarische Übersicht erstellen.   |
| Der Hersteller hat begründet, weshalb Machine Learning den anderen Verfahren überlegen ist und die damit einhergehenden Risiken rechtfertigt. |                                                              |
| Der Hersteller hat eine Liste an Risiken erstellt, die sich spezifisch durch die Anwendung der Verfahren des maschinellen Lernens ergeben. | Ist Teil der Risikomanagementakte                            |
| Die Hersteller haben Risiken analysiert, die sich ergeben, wenn andere als die spezifizierten Nutzer das Produkt nutzen. |                                                              |
| Die Hersteller haben Risiken analysiert, die sich ergeben durch die Nutzung in einer anderen als der spezifizierten Nutzungsumgebung. |                                                              |
| Die Hersteller haben Risiken analysiert, die sich ergeben durch Inputs, die nicht den spezifizierten Formaten genügen. |                                                              |
| Die Hersteller haben Risiken analysiert, die sich ergeben durch Daten, die nicht entsprechend der spezifizierten Voraussetzungen generiert wurden. |                                                              |
| Der Hersteller hat die Risiken bewertet, wenn das System bei einer anderen Patientenpopulation als der spezifizierten eingesetzt wird. |                                                              |



### 2. Software-Anforderungen

#### a) Funktionalität und Leistungsfähigkeit

|Anforderung|Kommentare|
|:--|:--|
|Der Hersteller hat aus der Zweckbestimmung nachvollziehbar quantitative Gütekriterien bzw. Anforderungen an die Software oder/und den Algorithmus abgeleitet [^C.2.a.1].|Diese Nachvollziehbarkeit lässt sich mit einer Traceability-Matrix besonders gut  darstellen.|
|Der Hersteller hat die erwarteten Wertebereiche der Outputs spezifiziert.||
|Der Hersteller hat die Anforderungen bezüglich der Wiederholbarkeit und Reproduzierbarkeit von Anforderungen spezifiziert.|Dies ist besonders bei "Continuous Learning Systems" relevant.|
|Der Hersteller hat festgelegt wie sich das System verhält, wenn die Inputs nicht die spezifizierten Voraussetzungen erfüllen[^C.2.a.2].|Dies ist ein Aspekt der Robustheit, der gemäß ISO 25010 und IEC 62304 Kapitel 5.2 zu spezifizieren ist.|
|Der Hersteller hat festgelegt, welche Selbsttests das System durchführen muss, und wie es sich verhält, wenn diese nicht erfolgreich sind.|Dies ist besonders bei "Continuous Learning Systems" relevant.|
|Der Hersteller hat festgelegt, wie schnell das System die Outputs erzeugen muss.|Diese Festlegung kann ggf. abhängig von der Größe und Menge der Daten erfolgen.|
|Der Hersteller hat die Verfügbarkeit des Medizinprodukts spezifiziert.|Dies ist ein Aspekt der Robustheit, der gemäß ISO 25010 und IEC 62304 Kapitel 5.2 zu spezifizieren ist.|

[^C.2.a.1]: Beispiele:  **Beispiel 1**: Die Stakeholder-Anforderungen lautet, dass 95% der Radiologen einen Krebsfall mit dem Produkt erkennen können müssen. Die Anforderung an den Algorithmus lautet, dass er eine Sensitivität von 97% aufweisen muss. **Beispiel 2**: Die Stakeholder-Anforderungen lautet, dass Arterienverkalkungen mit einer Sensitivität von 92% erkannt werden müssen. Die Anforderungen an den Algorithmus lautet, dass er die Stärke der Plaques im Blutgemäß auf 0,2mm genau vorhersagen muss.

[^C.2.a.2]:  Beispiele: unvollständige Datensätze, fehlende Datensätze, falsche Datenformate, zu große Datenmengen, Daten außerhalb spezifizierter Wertebereiche, falsche zeitliche Abfolge von Daten.

#### b) User Interface

| Anforderung                                                  | Kommentare                                               |
| :----------------------------------------------------------- | :------------------------------------------------------- |
| Der Hersteller hat spezifiziert, was das User Interface anzeigen muss, wenn die Voraussetzungen nicht erfüllt sind[^C.2.a.2], um das System sicher zu betreiben (z.B. nicht valide oder nicht erwartete Inputs). |                                                          |
| Der Hersteller hat spezifiziert, was das User Interface anzeigen muss, wenn die Output nicht den spezifizierten Gütekriterien entsprechen. |                                                          |
| Der Hersteller hat festgelegt, ob es einer Gebrauchsanweisung und Trainingsmaterialien bedarf. | Die MDR / IVDR erlauben Ausnahmen von der Verpflichtung. |

#### c) Weitere Software-Anforderungen

| Anforderung                                                  | Kommentare                                          |
| :----------------------------------------------------------- | :-------------------------------------------------- |
| Der Hersteller hat festgelegt, welche Anforderungen das System erfüllen muss, um Fehlverhalten feststellen zu können. | Könnten ein Auditlog oder ein Monitoring-Port sein. |
| Der Hersteller hat geprüft, dass Patienten durch das spezifizierte System nicht Entscheidungen ausgesetzt sind, die ausschließlich auf automatischer Datenverarbeitung beruhen. | Anforderung des Art. 22 der DSGVO.                  |



#### d) Risikomanagement und klinische Bewertung

| Anforderung                                                  | Kommentare                                                   |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| Der Hersteller hat die Risiken bewertet, die sich ergeben, wenn die Inputs nicht die spezifizierten Voraussetzungen erfüllen[^C.2.a.2]. |                                                              |
| Der Hersteller hat die quantitativen Güterkriterien anhand des Stands der Technik abgeleitet. | Der Hersteller muss die Gütekriterien für alternative Technologien und Verfahren benennen und argumentieren können, wenn das Medizinprodukt den Alternativen bezüglich der Gütekriterien nicht überlegen ist[^C.2.d.1]. |
| Der Hersteller hat den Goldstandard festgelegt und dessen Wahl begründet, mit dem die Gütekriterien überprüft werden sollen. |                                                              |
| Der Hersteller hat Risiken analysiert, die sich ergeben, wenn die Outputs nicht den spezifiziert Gütekriterien entsprechen. |                                                              |
| Der Hersteller hat die Folgen bewertet, wenn das System sozial inakzeptable Outputs liefert (z.B. diskriminierend). | Diese "Folgen" sind nicht notwendigerweise Risiken im Sinne der ISO 14971. |
| Der Hersteller hat die Risiken bewertet, wenn das System nicht verfügbar ist. |                                                              |
| Falls der Hersteller Selbsttests verwendet, hat er dargelegt, welche der spezifizierten Gütekriterien damit überprüft werden und welche Risiken dadurch beherrscht sind. |                                                              |
| Bei Continuous Learning Systems hat der Hersteller die Option, das System auf einen bekannten Zustand zurückzusetzen, erwogen. | In der Risikotabelle zeigen lassen.                          |
| Bei Continuous Learning Systems hat der Hersteller quantitativ dargelegt, weshalb das Nutzen-Risiko-Verhältnis besser als bei nicht kontinuierliche lernenden Systemen ist. |                                                              |


[^C.2.d.1]: Der Stand der Technik (State-of-the-Art) entspricht nicht notwendigerweise dem Stand der Wissenschaft und damit dem Goldstandard ("Ground Truth"). D.h. dass die Anforderungen an das System geringer sind als bei einem Goldstandard. Das ist inbesondere wahrscheinlich, insofern der Goldstandard ein invasives oder sehr kostenintensives Verfahren bedingt.

### 3. Datenmanagement

In diesem Kapitel sind Trainings-, Validierungs- und Testdaten gemeint, wenn von Daten gesprochen wird.

#### a) Sammlung der Daten

| Anforderung                                                  | Kommentar                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Der Hersteller hat die Anzahl der Datensätze festgelegt und eine Begründung gegeben, weshalb diese ausreichend ist[^C.3.a.1]. |                                                              |
| Der Hersteller hat spezifiziert, welche Daten pro Datensatz er benötigt, um den Algorithmus zu trainieren. |                                                              |
| Der Hersteller hat die Ein- und Ausschlusskriterien von Patientendaten  anhand relevanter Attribute[^C.3.a.2] charakterisiert. |                                                              |
| Der Hersteller hat technische Ein- und Ausschlusskriterien für Daten spezifiziert[^C.3.a.3]. |                                                              |
| Der Hersteller hat das Verfahren beschrieben, mit dem er sicherstellt, dass Datensätze, die nicht den Einschlusskriterien genügen bzw. ausgeschlossen werden sollen, tatsächlich ausgeschlossen werden. | Verfahren schließt eine Software-gestützte Bewertung mit ein. Diese Software ist zu validieren. |
| Der Hersteller hat die gesammelten Daten mit Hilfe einer deskriptiven Statistik beschrieben[^C.3.a.4]. | Empfehlenswert ist das ["Dataset Nutrition Label"](https://ahmedhosny.github.io/datanutrition/). |
| Der Hersteller hat begründet, wo er die Daten sammelt und weshalb diese repräsentativ für die Zielpopulation sind. So sinnvoll, haben sie diese mit Daten des Bundesamts für Statistik oder von Registern verglichen. |                                                              |
| Der Hersteller hat Faktoren gelistet und diskutiert, die einen "Bias" der Daten verursachen könnten. |                                                              |
| Der Hersteller hat analysiert, welche Einflüsse die Art und der Ort der Datensammlung auf die Daten hat[^C.3.a.5]. |                                                              |
| Der Hersteller hat ein Verfahren etabliert, mit dem Daten vor dem Testen und Training anonymisierten bzw. pseudonymisiert werden. |                                                              |
| Der Hersteller hat Möglichkeiten eines "Label Leakages" untersucht und ausgeschlossen[^C.3.a.6]. |                                                              |
| Der Hersteller, der Fragebögen verwendet, hat die Wahl der Fragen, den Zeitpunkt der Befragung und ggf. die Methode zu deren Auswertung begründet, insbesondere wenn kein standardisierter Fragebogen vorliegt. |                                                              |

[^C.3.a.1]: Eine generelle Vorgabe für die Anzahl der Daten kann es nicht geben. Diese hängt u.a. vom "Signal-Noise-Ratio" ab. Beispielsweise würde bei einem Gendatensatz der Prozentsatz relevanter Gene und die Stärke und Häufigkeit des vorherzusagenden Effekts die Anzahl beeinflussen. Bei Daten, die klassifiziert werden sollen, ist die Anzahl der Datensätze mit der selteneren Klasse (z.B. die Prävalenz von Krankheiten) entscheidend.

[^C.3.a.2]: z.B. demographische Daten (Alter, Geschlecht), körperliche Parameter (Größe, Gewicht), Erkrankungen, Vitalparameter, Laborparameter, Vorhandensein weitere Untersuchungen, Anamnese.

[^C.3.a.3]: Beispiele: **Beispiel 1**: Patienten, die wegen eines Herzschrittmachers oder einer Lungen-OP ausgeschlossen werden müssen, weil die Bilder nicht ausgewertet werden können oder zu Fehlklassifikation führen könnten. **Beispiel 2**: Formate und technischen Parameter wie Bildgrößen, Auflösungen, Helligkeit und Kontraste, Farbkodierung, Kompression, Aufnahmerichtungen, Aufnahmeverfahren (z.B. CT versus MRT), mit ohne Kontrastmittel, Zoom. **Beispiel 3**: Vollständigkeit von Meta-Daten.

[^C.3.a.4]: Übliche sind die Berechnung von Verteilungen (Histogrammen), Mittelwerten, Quartilen, ggf. "Joint Distribution of Features". Auch die Korrelation von Daten untereinander sollte untersucht sein. Weitere Beispiele finden sich in der in der [Publikation von Sarah Holland et al.](https://arxiv.org/pdf/1805.03677.pdf) (z.B. in der Tabelle 1)

[^C.3.a.5]: Beispiele: Einfluss von verschiedenen Messgeräten, Befragungen, Policies (z.B. ein Klinik nimmt Laborparameter nur im Notfall, eine andere routinemäßig. Frequenz und Anlass, mit der Patienten untersucht werden), Art der Klinik (z.B. kleines Krankenhaus, aus dem alle schweren Fälle verlegt werden versus Maximalversorger > Survivor Bias), Self-Selection Bias (z.B. Patienten mit diversen Vorerkrankungen gehen eher in ein Krankenhaus statt in eine Arztpraxis), Art der Studie (prospektiv versus retrospektiv)

[^C.3.a.6]: Das sind Daten, bei denen nicht-kausale Informationen über das Label in den Daten stecken z.B. in der Sortierung (z.B. erst die Daten von Gesunden, dann die von Kranken), im Krankenhaus (von einem stammen die schweren Fälle), im Bild (z.B. bei Hautkrebs ist immer noch ein Lineal zu sehen). Ein weiteres Beispiel wären mehrere CT-Bilder eines Patienten, bei denen das Modell anhand des Patienten und nicht der Krankheit lernt. Das könnte z.B. passieren, wenn auf mehreren Bildern mit Krebs auch ein Rippenbruch zu erkennen ist. 

#### b) Labeling von Daten

| Anforderung                                                  | Kommentar                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Der Hersteller hat beim "Supervised Learning", die Labels aus der Zweckbestimmung abgeleitet, mit denen die Trainingsdaten verstehen werden und diese Wahl begründet. |                                                              |
| Der Hersteller hat beim "Supervised Learning" ein Verfahren fürs Labeling festgelegt, falls noch keine Labels in den Daten vorhanden waren. |                                                              |
| Dieses Verfahren spezifiziert quantitative Klassifizierungskriterien für das Labeling. Die Wahl dieser Kriterien hat der Hersteller begründet[^C.3.b.1]. | Falls nicht der "Ground Truth"[^C.3.b.2] gewählt wird, weil dieser z.B. zu teuer oder zu invasiv ist, muss dies ebenfalls begründet sein. |
| Dieses Verfahren spezifiziert die Anforderungen an die Anzahl, Ausbildung und Kompetenz der für das Labeling verantwortlichen Personen. |                                                              |
| Dieses Verfahren legt fest, wie die Kompetenz der für das Labeling verantwortlichen Personen geprüft wird. | Dies kann durch das Labeling von ausgewählten Datensätzen erfolgen.  |
| Dieses Verfahren legt fest, wie die für das Labeling verantwortlichen Personen geschult werden und wie der Erfolg dieser Schulung überprüft wird. |                                                              |
| Dieses Verfahren legt fest, wie die Korrektheit der Labels systematisch überprüft wird. Die Wahl dieser Begründung hat der Hersteller dokumentiert. | Der Hersteller kann identische Datensätzen mehreren Personen zum Labeling vorlegen und die Übereinstimmung der Ergebnisse bewerten. |
| Dieses Verfahren legt fest, wie überwacht wird, dass die das Labeling verantwortlichen Personen auch während des Labelings dauerhaft leistungsfähig und leistungswillig sind[^C.3.b.3]. | Dies kann durch Datensätze mit bereits bekanntem Label erfolgen, die beim Labeling für die Person unmerklich eingeschoben werden. |

[^C.3.b.1]: Wenn beispielsweise die Klassifizierung in gesunde und kranken Patienten erfolgen soll, muss der Hersteller die Kriterien für die spezifische Fragestellung bzw. Zweckbestimmung ableiten, wann ein Patient als gesund und als krank zu klassifizieren ist.

[^C.3.a.2]: Der "Ground Truth" ist das präziseste Referenzverfahren ("Stand der Wissenschaft"), mit dem ein Größe der Klasse bestimmt ist. Für die Bestimmung einer arteriellen Hypertonie kann es z.B. eine invasive Blutdruck-Messung die genausten Ergebnisse und damit den "Ground Truth" bilden. 

[^C.3.b.3]: Das Labeling Dutzender Datensätze ist anstrengend. Eine Bezahlung pro Datensatz kann falsche Motivationsanreize setzen.

#### c) Verfahren zur (Vor-)Verarbeitung von Daten 

| Anforderung                                                  | Kommentar                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Der Hersteller hat ein Verfahren festgelegt, das die (Vor-)Verarbeitung ("pre-processing") der Daten beschreibt. |                                                              |
| Dieses Verfahren beschreibt die einzelnen Verarbeitungsschritte wie Umrechnungen, Transformationen, Aggregationen, Normalisierung, Formatumwandlungen, Berechnung von Feature, Umwandlung numerischer Daten in Kategorien. | Eine graphische Darstellung verschafft einen schnellen Überblick. Die Umwandlung von numerischen in kategoriale Werte bedarf einer Begründung. |
| Das Verfahren beschreibt, wie die Korrektheit der Zwischenschritte und der Endergebnisse überprüft wird[^C.3.c.0]. Diese Überprüfungen erfolgen risikobasiert. | Dies entspricht den Anforderungen der ISO 13485:2016 Kapitel 4.1.6. Die Risikomanagementakte muss diese Analysen enthalten. |
| Dieses Verfahren spezifiziert, wie Werte mit verschiedenen Messskalen bzw. Einheiten erkannt und verarbeitet werden. |                                                              |
| Dieses Verfahren spezifiziert, wie Werte, die mit verschiedenen Messverfahren bestimmt wurden, erkannt und verarbeitet werden. |                                                              |
| Dieses Verfahren spezifiziert, wie Werte bzw. Metadaten mit gleichem Namen (z.B. in Spaltenköpfen) erkannt und verarbeitet werden. |                                                              |
| Dieses Verfahren spezifiziert, wie fehlende Werte innerhalb von Datensätzen erkannt und verarbeitet werden. Diese Festlegung hat der Hersteller begründet[^C.3.c.1]. | Es ist darauf achten, dass der Hersteller bei der Begründung zwischen "missing at random" und "missing not at random" unterscheidet[^C.3.c.2]. |
| Dieses Verfahren spezifiziert, wie Outliers erkannt und verarbeitet werden[^C.3.c.3]. Diese Festlegung hat der Hersteller begründet[^C.3.C.4]. | Exemplarisch für ein Datum / Feature zeigen lassen.          |
| Dieses Verfahren spezifiziert, wie nicht verwendbare Datensätze erkannt werden und damit umgegangen wird.[^C.3.c.5]. Diese Festlegung hat der Hersteller begründet. | Exemplarisch für ein Datum / Feature zeigen lassen.          |


[^C.3.c.0]: Zu den Möglichkeiten der Überprüfung zählen Software-Tests und redundante bzw. alternative Berechnungen z.B. mit Excel.

[^C.3.c.1]: Zu den Optionen der Verarbeitung zählen, den Datensatz zu löschen, Ersetzen durch den Mittelwert anderer Datensätze, neuer Wert "missing" (bei kategoriellen Werten)

[^C.3.c.2]: Ein Beispiel für "missing not at random" sind zu hohe Laborwerte, die abgeschnitten werden.

[^C.3.c.3]: Zu den Optionen der Verarbeitung zählen, den Datensatz zu löschen, den Wert zu korrigieren, den Wert auf einen festgelegten Wert (Min/Max) zu setzen.

[^C.3.c.4]: Diese Begründung ist bei Regressionsverfahren wichtiger als bei Baum-Verfahren.

[^C.3.c.5]: Beispiele sind Röntgenbilder mangelnder Qualität, Patienten, die nicht den Inklusionskriterien entsprechen.

#### d) Dokumentation und Versionskontrolle

| Anforderung                                                  | Kommentar                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Der Hersteller hat den "Funnel" beschrieben, der erkennen lässt, wie viele Daten aus welchen Datenquellen (z.B. Kliniken) stammen und bei welchem Verarbeitungsschritt wie viele Datensätze aus welchem Grund weggefallen sind. |                                                              |
| Der Hersteller hat die verarbeiteten Daten mit Hilfe einer deskriptiven Statistik beschrieben[^C.3.a.4]. | Empfehlenswert ist das ["Dataset Nutrition Label"](https://ahmedhosny.github.io/datanutrition/) |
| Der Hersteller hat alle Software zur Datenverarbeitung einschließlich der dabei verwendeten Bibliotheken dokumentiert und unter Versionskontrolle. |                                                              |
| Der Hersteller hat Daten (Rohdaten, ggf. Zwischenergebnisse, Trainings-, Validierungs- und Testdaten) unter Versionskontrolle. |                                                              |
### 4. Modellentwicklung

#### a) Vorbereitung

| Anforderung                                                  | Kommentar                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Der Hersteller hat die Auswahl der Feature begründet, die er beim Training berücksichtigt. |                                                              |
| Der Hersteller hat die Abhängigkeit der Feature untereinander beschrieben. | Ein Directed Acyclic Graph (DAG) hilft bei der Visualisierung. |
| Der Hersteller hat sichergestellt, dass er das Modell nur mit Daten trainiert, die im "Feld" zum Zeitpunkt der Modellanwendung tatsächlich vorliegen. | Prüfen, ob keine Daten "aus der Zukunft" beim Training verwendet werden. |
| Der Hersteller hat dokumentiert und begründet, in welchem Verhältnis er die Daten in Trainings-, Validierungs- und Testdaten aufteilt. |                                                              |
| Der Hersteller hat dokumentiert, nach welcher Stratifizierung er die Daten in Trainings-, Validierungs- und Testdaten aufteilt[^C.4.a.1]. |                                                              |
| Der Hersteller hat dokumentiert, wie er sicherstellt, dass mehrere Datensätze zu einem Objekt im gleichen "Bucket" (Trainings-, Validierungs- bzw. Testdaten) sind. |                                                              |
| Der Hersteller hat dokumentiert, wie er sicherstellt, dass das Entwicklungsteam keinen Zugriff zu den Testdaten bekommen. |                                                              |
| Der Hersteller hat beschrieben, wenn er die Daten spezifisch für das Modell oder spezifisch für die Bibliothek umkodiert[^C.4.a.2]. |                                                              |

[^C.4.a.1]: Bei Daten mit seltenen Feature oder Labels kann es notwendig sein, die Daten nicht ausschließlich nach dem Zufallsprinzip zu verteilen.

[^C.4.a.2]: Beispiele dafür sind Normalisierung, Wahl von Klassen-Labels (z.B. 0 oder 1), Wahl von Spaltennamen, Aufteilung von kategoriellen Werten auf mehrere Spalten.

#### b) Training

| Anforderung                                                  | Kommentar                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Der Hersteller führt Modelltraining, Optimierung der Hyperparameter und Modellselektion ausschließlich mit den Trainings- und Validierungsdaten (mittels Kreuzvalidierung) durch. |                                                              |
| Der Hersteller hat die Wahl der Hyperparameter dokumentiert und begründet[^C.4.b.1]. |                                                              |
| Der Hersteller hat ggf. die Wahl der Epochen dokumentiert und begründet[^C.4.b.2]. | Wo möglich, anhand von Learning Curves zeigen lassen.        |
| Der Hersteller hat die Gütemaße bestimmt, dokumentiert und anhand der Zweckbestimmung begründet, für die er das Modell optimieren will. | Die Wahl dieser Gütemaße ist spezifisch für die Zweckbestimmung. |
| Der Hersteller hat mehrere Modelle mit mehreren Hyperparametern trainiert (darunter auch einfachere und interpretierbare Modell). |                                                              |

[^C.4.b.1]: Beispiele: Loss-Funktion, Optimizer, Lernrate, Anzahl Epochen

[^C.4.b.2]: Die Learning Curves gibt es beispielsweise für neuronale Netzwerke und Boosting-Verfahren, nicht aber für Modelle mit numerischer Lösung (z.B. lineare Regression) oder bei einem einzigen Baum.

#### c) Bewertung

| Anforderung                                                  | Kommentar                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Der Hersteller hat für die verschiedenen Modelle die Gütemaße z.B. bei einer binären Klassifikation mit Hilfe einer Vierfeldertafel dokumentiert. | Diese Dokumentation sollte nicht nur die Werte umfassen, auf die der Hersteller das Modell optimiert hat. |
| Der Hersteller hat die Gütemaße für die verschiedenen Modelle  nicht nur global bewertet und dokumentiert, sondern ggf. auch getrennt für verschiedene Feature. |                                                              |
| Der Hersteller hat die Datensätze untersucht, die besonders gut  und die besonders schlecht vorhergesagt wurden. | Empfehlenswert ist eine Residuen-Analyse, bei der ggf. die Fehler über die Feature-Werte aufgetragen sind. |
| Der Hersteller hat die Datensätze untersucht, bei denen sich das Modell besonders sicher und besonders unsicher[^C.4.c.1] ist. |                                                              |
| Der Hersteller hat anhand der Gütekriterien und der Zweckbestimmung die letztlich Wahl des Modells begründet und insbesondere dargelegt, wenn einfachere und interpretierbarere Modelle nicht zur Anwendung kamen. |                                                              |
| Der Hersteller hat sich für einzelne Datensätze die Feature anzeigen lassen, die das Modell besonders zur Entscheidung bewogen haben[^C.4.c.2]. |                                                              |
| Der Hersteller hat evaluiert, wie und wie stark sich einzelne Feature ändern  müssten, damit das Modell zu einer anderen Vorhersage kommt. | Man spricht von ["Counterfactuals"](https://christophm.github.io/interpretable-ml-book/counterfactual.html) |
| Der Hersteller hat die Abhängigkeit (Stärke, Richtung) der Vorhersagen von den Feature-Werten analysiert / visualisiert[^C.4.c.3]. |                                                              |
| Der Hersteller hat Datensätze synthetisiert, die das Modell besonders aktivieren[^C.4.c.4]. | Dies lässt sich als Best Practice nicht generell einfordern. |
| Der Hersteller hat das Modell durch ein vereinfachtes Surrogat-Modell wie einen Entscheidungsbaum approximiert. | Dies lässt sich als Best Practice nicht generell einfordern. |
| Der Hersteller hat das Modell mit Zufallswerten geprüft.     |                                                              |

[^C.4.c.1]: Bei Klassifikationsaufgaben ist der aktuelle Stand der Forschung zu berücksichtigen.

[^C.4.c.2]: zu den Ansätzen zählen LIME (Local Interpretable Model-agnostic Explanations), Beta (Black Box Explanations through Transparent Approximations), LRP (Layer-wise Relevance Propagation) und Feature Summary Statistics (inkl. Feature Importlande und Feature Interaktion.

[^C.4.c.3]: Beispiele sind Sharpley-Values, ICE-Plots, Partial Dependency Plots (PDP)

[^C.4.c.4]: Beispiele siehe http://yosinski.com/deepvis

#### d) Dokumentation 

| Anforderung                                                  | Kommentar                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Der Hersteller hat das Modell[^C.4.d.1] und/oder den Trainingscode unter Versions- und Konfigurationskontrolle. |                                                              |
| Der Hersteller hat die Trainingsdaten, die Testergebnisse und deren Bewertung unter Versionskontrolle. |                                                              |
| Der Hersteller hat die SOUP (Bibliotheken und Frameworks) unter Versions- und Konfigurationskontrolle. |                                                              |
| Der Hersteller hat die Architektur des Modells und das Modell selbst inklusive dessen Hyperparameter dokumentiert. | 
  |
| Der Hersteller hat beschrieben, wenn er mit einem "Pretrained Model" gearbeitet hat, und dargelegt, weshalb dieses "Pre-Training" der Aufgabenstellung angemessen ist. |                                                              |
| Der Hersteller hat die Güte der Modelle basierend auf den Gütemaßen dokumentiert.                | Diese Gütemaße beziehen sich auf Prüfung mit den Testdaten. |
| Der Hersteller hat die Trainingsdaten einschließlich deren Feature beschrieben und statistisch ausgewertet. | z.B. mit ["Data Nutrition Labels"](https://ahmedhosny.github.io/datanutrition/) |
| Der Hersteller hat dokumentiert, innerhalb welcher Grenzen (z.B. Feature-Werte) das Modell die Anforderungen an die Gütemaße erreicht. |                                                              |

[^C.4.d.1]: Trainierte Modelle lassen sich serialisieren.

### 5. Produktentwicklung

#### a) Software-Entwicklung

| Anforderung                                                  | Kommentar                       |
| ------------------------------------------------------------ | ------------------------------- |
| Der Hersteller hat alle von der IEC 62304 geforderten Aktivitäten durchgeführt und dokumentiert. | Hinweis für Auditoren[^C.5.a.1] |
| Wenn der Hersteller das Modell in einer anderen Sprache oder für eine andere Laufzeitumgebung implementiert hat, hat er einen Plan erstellt, welche der Aktivitäten gemäß Kapitel 4. er wiederholt. |                                 |
| Der Hersteller prüft die Performance (Antwortzeiten, Ressourcenverbrauch) auf der Zielhardware (z.B. Browser, Mobilgerät). |                                 |
| Der Hersteller hat für alle SOUP- bzw. OTS-Komponenten beschrieben, wie diese zu verifizieren sind. |                                 |

[^C.5.a.1]: Die Hersteller sollten die üblichen Best-Practices einhalten wie das Einhalten von Coding-Guidelines, die Überprüfung des Codes durch Code-Reviews anhand definierte Kriterien, das Testen des Codes durch Unit-Tests mit einem definierten Abedeckungsgrad usw.

#### b) Begleitmaterialien

| Anforderung                                                  | Kommentar                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Die Gebrauchsanweisung identifiziert eindeutig die Version des Produkts. | Falls möglich, die UDI angeben                               |
| Die Gebrauchsanweisung beschreibt die Zweckbestimmung des Produkts einschließlich des erwarteten medizinischen Nutzens. |                                                              |
| Die Gebrauchsanweisung die vorgesehene Patientenpopulation anhand Indikationen, Kontraindikationen und so relevant anhand weiterer Parameter wie Alter, Geschlecht, Begleiterkrankungen oder Verfügbarkeit von Informationen. |                                                              |
| Die Gebrauchsanweisung nennt explizit die Patienten / Daten  / Anwendungsfälle, bei denen das Produkt nicht verwendet werden darf. |                                                              |
| Die Gebrauchsanweisung dokumentiert die Anforderungen an die Input-Daten (inklusive Formate, Auflösungen, Wertebereich etc.). |                                                              |
| Die Gebrauchsanweisung spezifiziert die vorgesehenen primären und sekundären Anwender gemäß Zweckbestimmung. |                                                              |
| Die Gebrauchsanweisung beschreibt, von welchen sonstigen Voraussetzungen das Produkt ausgeht (z.B. Laufzeitumgebung, Nutzungsumgebung). |                                                              |
| Die Gebrauchsanweisung benennt die Restrisiken.              |                                                              |
| Die Gebrauchsanweisung gibt an, mit welchen Daten das Modell trainiert wurde. | Dies bezieht sich sowohl auf das Patientenkollektiv als auch auf die verwendeten Feature. |
| Die Gebrauchsanweisung beschreibt das Modell bzw. die Algorithmen. |                                                              |
| Die Gebrauchsanweisung benennt die Gütekriterien.            |                                                              |
| Die Gebrauchsanweisung listet die Faktoren auf, die sich negativ auf die Gütekriterien auswirken können. |                                                              |
| Die Gebrauchsanweisung spezifiziert, ob das Produkt während der Anwendung weiter trainiert wird. |                                                              |
| Die Gebrauchsanweisung beschreibt, wie Updates erfolgen.     |                                                              |
| Die Gebrauchsanweisung enthält ggf. Verweise auf weiterführende Literatur. |                                                              |
| Die Gebrauchsanweisung enthält ggf. Hinweise zu Lizenzrechten. |                                                              |
| Die Gebrauchsanweisung identifiziert den Hersteller und nennt Kanäle, über die Rückfragen zu stellen sind. |                                                              |
| Die Gebrauchsanweisung nennt mögliche ethische Problematiken. |                                                              |
| Die Gebrauchsanweisung benennt die URL, unter der die aktuellsten Versionen der Gebrauchsanweisung zu finden sind. |                                                              |

#### c) Usability-Validierung

| Anforderung                                                  | Kommentar |
| ------------------------------------------------------------ | --------- |
| Der Hersteller bewertet im Rahmen der Usability Validierung, ob die Nutzer die Gebrauchsanweisung verstehen. |           |
| Der Hersteller bewertet im Rahmen der Usability Validierung, ob die Nutzer dem Produkt blind vertrauen oder die Ergebnisse nachprüfen. |           |
| Der Hersteller bewertet im Rahmen der Usability Validierung, ob die Anwender die Ergebnisse korrekt erkennen und verstehen. |           |

#### c) Klinische Bewertung 

| Anforderung                                                  | Kommentar |
| ------------------------------------------------------------ | --------- |
| Der Hersteller bewertet im Rahmen der klinischen Bewertung, ob der versprochene medizinische Nutzen bei den gegebenen Güteparametern erreicht wird. |           |
| Der Hersteller bewertet im Rahmen der klinischen Bewertung, ob der versprochene medizinische Nutzen dem Stand der Technik entspricht. |           |
| Der Hersteller bewertet im Rahmen der klinischen Bewertung, ob das Modell gegen den "Ground Truth" bewertet wurde. |           |

### 6. Produktfreigabe

| Anforderung                                                  | Kommentar                     |
| ------------------------------------------------------------ | ----------------------------- |
| Der Hersteller hat das Modell anhand der in Kapitel 5.b) genannten Kriterien dokumentiert. |                               |
| Der Hersteller hat im Risikomanagement die Risiken als akzeptabel bewertet und dokumentiert, dass alle im Risikomanagementplan spezifizierten Aktivitäten durchgeführt wurden. | Hinweis für Auditoren[^C.6.1] |
| Der Hersteller hat bei Systemen, die er in den USA in den Verkehr bringen will, in den "Software as a Medical Device Pre-Specifications“ (SPS) dargelegt, welche Arten der Änderungen er antizipiert[^C.6.2]. |                               |
| Der Hersteller hat bei Systemen, die er in den USA in den Verkehr bringen will, im Algorithm Change Protocol (ACP) dargelegt, wie er diese Änderungen durchführen will[^C.6.3]. |                               |
| Der Hersteller hat einen Post-Market Surveillance Plan erstellt (s.u.). |                               |

[^C.6.1]: Anhand von Beispielen prüfen, dass die Wirksamkeit von Risikokontrollmaßnahmen geprüft wurde, dass es eine Traceability von Risiken zu Risikokontrollmaßnahmen gibt.

[^C.6.2]: Änderungen können die Zweckbestimmung, Dateninput, die klinische und analytische Leistungsfähigkeit betreffen.

[^C.6.3]: Das Vorgehensmodell muss z.B. eingehen auf den Umgang mit Daten, auf das Re-Training, auf die Leistungsbewertung und auf die Updates.

## D) Anforderungen an die der Entwicklung nachgelagerten Phasen

#### 1. Produktion, Distribution, Installation

|Anforderung|Stufe|Kommentare|
|:--|:--:|:--|
|Der Hersteller hat beschrieben, wie sichergestellt ist, dass nur genau die vorgesehenen Artefakte (Dateien) in genau der vorgesehenen Version im Produkt oder als Produkt ausgeliefert werden|1|Hier geht es ums Konfigurationsmanagement. Auch bei Downloads oder AppStores relevant|
|Der Hersteller hat beschrieben, wie die für die Installation verantwortlichen Personen wissen, welches die aktuellste Version ist und wie Verwechslungen bei der Installation ausgeschlossen werden können|2|Dies ist nur bei stand-alone Software relevant. Hier wäre eine Verfahrens- oder Arbeitsanweisung zu erwarten|
|Der Hersteller hat beschrieben, wie bei der Installation sichergestellt wird, dass die Anforderungen, die in den Begleitmaterialien spezifiziert sind (s.o.) tatsächlich erfüllt sind|1|Hier wäre eine Verfahrens- oder Arbeitsanweisung zu erwarten|
|Der Hersteller hat Verfahren etabliert, die gewährleisten, dass er mit den Betreibern und Anwendern seiner Produkte zeitnah kommunizieren kann|1|Bei unkritischen Produkten ist die Stufe 2 vertretbar|

#### 2. Marktüberwachung

|Anforderung|Kommentare|
|:--|:--|
|Der Hersteller hat einen Post-Market Surveillance (PMS) Plan erstellt.||
|Der Hersteller hat in diesem PMS-Plan die Daten spezifiziert, welche er sammeln und auswerten will.||
|Der Hersteller hat im PMS-Plan spezifiziert, bei welchen Gütekriterien und Grenzwerten er eine Handlung insbesondere eine Neubewertung des Nutzen-Risiko-Verhältnisses für notwendig erachtet.||
|Der Hersteller hat beim Festlegen dieser Schwellenwerte analysiert, welche Feedback-Loops die Schwellenwerte selbst beeinflussen können[^D.2.1].||
|Der Hersteller hat beim Festlegen dieser Schwellenwerte analysiert, welche Self-Fullfilling-Prophecies die Schwellenwerte selbst beeinflussen können[^D.2.2].||
|De Hersteller hat im PMS-Plan beschrieben, wie er welche Informationen zu unerwünschten medizinischen Nebenwirkungen sammelt und bewertet.||
|Der Hersteller hat im PMS-Plan beschrieben, wie er welche Informationen zu (unerwünschten) Verhaltensänderungen bzw. (vorhersagbarem) Missbrauch sammelt und bewertet[^D.2.3]||
|Der Hersteller hat im PMS-Plan beschrieben, wie er welche Informationen zu weiteren "unerwünschten Nebenwirkungen" sammelt und bewertet[^D.2.4].||
|Der Hersteller hat im PMS-Plan beschrieben, wie er welche Informationen sammelt, um bewerten zu können, ob die Daten im Feld den erwarteten Daten bzw. den Trainingsdaten entsprechen[^D.2.5].|Hinweis für Auditoren[^D.2.6]|
|Der Hersteller hat im PMS-Plan beschrieben, wie und wie oft er Informationen darüber sammeln will, ob das Produkt noch dem State-of-the-Art genügt.|Hinweis für Auditoren[^D.2.7]|
|Der Hersteller hat im PMS-Plan beschrieben, wie und wie oft er Informationen darüber sammeln will, ob der "Ground Truth" bzw. der Goldstandard noch aktuell sind.||
|Der Hersteller hat im PMS-Plan beschrieben, wie und wie oft er überprüft, dass Änderungen konform dem Algorithm Change Protocol (ACP) und innerhalb der „SaMD Pre-Specifications“ (SPS) erfolgen.||

[^D.2.1]: Beispiel für Feedback-Loops: Eine Reise-Empfehlungs-App verschickt abhängig von Feature (letzte Reise) gezielte Werbung. Diese wiederum beeinflusst das Reiseverhalten. Ein Algorithmus stellt Prognosen. Daher behandelt der Arzt die Patienten besser oder früher.

[^D.2.2]: Beispiele 1 (Kriminalistik): Algorithmus schlägt Polizei Orte vor, an denen sie kontrollieren soll. Wo viel kontrolliert wird, wird viel gefunden. Beispiel 2 (Medizin): Viele Patienten, die man in die Diagnostik schickt, werden zu viel Diagnosen führen. Daher wäre es hilfreich, im Post-Market die Daten/Objekte testen, die nicht vorgeschlagen wurden.

[^D.2.3]: Beispiel: Radiologen verlassen sich auf die Software und schauen sich die Bilder nicht mehr an, weshalb sie Befunde übersehen.

[^D.2.4]: Beispiele wären ethische Herausforderungen wie beispielsweise, der YouTube-Algorithmus, der zwar das Ziel erreicht, die Klick-Zahl bzw. die Nutzungsdauer zu maximieren, dabei aber Gewalt- und Verschwörungsvideos promotet.

[^D.2.5]: Man spricht von einem Distribution Shift bzw. von einer Data Drift.

[^D.2.6:]: Der Hersteller sollte Schwellenwerte für Feature oder für die Varianz / Kovarianz über die Zeit festlegen. Dies lässt sich insbesondere bei nicht-normalverteilten Daten über den Vergleich von Histogrammen oder Kerndichteschätzern visualisieren bzw. quantifizieren.

[^D.2.7]: Sich vom Hersteller beispielsweise den Prozess erklären lassen, wie er sich systematisch über neue Entwicklungen im Machine Learning informiert, wie er diese Entwicklungen bewertet sowie darauf reagiert.

## E) Anhänge

### 2. Weiterführende Literatur

#### a) Gesetze

- MDR
- IVDR

#### b) Normen und Best-Practice Guides

- **IEC 62304/AMD1**, Medical device software – Software life cycle processes
- **IEC 82304-1**, Health software – Part 1: General requirements for product safety
- [FDA Guidance Documents zum Machine Learning](https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-and-machine-learning-software-medical-device)

#### b) Fachliteratur, Lehrbücher

- Christoph Molnar: [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/)
- Patrick Hall: [Machine Learning Interpretability
  with H2O Driverless AI](http://docs.h2o.ai/driverless-ai/latest-stable/docs/booklets/MLIBooklet.pdf)
- Patrick Hall: [On the Art and Science of Machine Learning Explanations](https://arxiv.org/pdf/1810.02909.pdf)
- Johner Institut: [Videotrainings zum Machine Learning bei Medizinprodukten](www.auditgarant.de)

### 3. Erwägungsgründe

1. Hersteller entwickeln immer mehr Medizinprodukte die Verfahren der künstlichen Intelligenz, insbesondere des Machine Learnings, nutzen. Viele dieser Verfahren sind noch sehr neu und Best Practices fehlen. Dadurch entstehen Risiken für Patienten, Anwender und Dritte.
2. Die EU-Verordnungen (MDR, IVDR) fordern zwar explizit die Sicherheit der Produkte in den jeweiligen Anhängen I. Konkrete Anforderungen für diese Klasse der Produkte fehlen jedoch völlig. Daher fehlen sowohl den Herstellern als auch den Benannten Stellen und Behörden konkrete Leitlinien, wie sie die Sicherheit der Produkte bewerten können.
3. Im Gegensatz zu den meisten anderen grundlegenden Anforderungen sind keine Normen zum Thema KI harmonisiert. Daher gibt es keinen kanonischen Katalog an Anforderungen, der anerkannt den geforderten Stand der Technik reflektiert.
4. Die FDA hat begonnen, Anforderungen an den Umgang mit Continuous Learning Systems CLS zu formulieren. Diese Vorgaben sind ungeeignet, um bereits bei der Produktentwicklung ausreichend konkrete Anforderungen an die Produkte und Prozesse zu stellen. 
5. Die Sicherheit der Medizinprodukte muss in allen Phasen des Produkt-Lebenszyklusprozessen berücksichtigt werden. Eine Beschränkung auf das Testen ist unzureichend. Dieser Tatsache müssen Best Practices und Leitfäden gerecht werden. 
9. Es ist zu hoffen, dass Normen zur Sicherheit von KI-basierten Medizinprodukten entwickelt und harmonisiert werden. Das wird jedoch noch Jahre in Anspruch nehmen. Daher bedarf es eines Leitfadens (nur) in dieser Zwischenphase. 
10. Dieser Leitfaden soll zeitnah (bis Juli 2019) zur Verfügung stehen, um rasch den Herstellern als Orientierung zu dienen und es ihnen zu ermöglichen, sofort zu handeln. Die hohe Geschwindigkeit seiner Entwicklung macht Kompromisse bezüglich der Abstimmung mit möglichst vielen Parteien unumgänglich.
11. Der technologische Fortschritt im Bereich der künstlichen Intelligenz ist immens. Neue Verfahren und Technologien werden kontinuierlich publiziert. Einerseits soll ein Leitfaden so spezifisch wie möglich sein. Andererseits darf er nicht zu spezifisch auf ein Verfahren oder eine Technologie ausgerichtet sein, um eine sinnvolle "Haltbarkeitsdauer" zu erreichen. Daher muss ein Leitfaden allgemeine Konzepte adressieren und kann nie einen Anspruch auf Vollständigkeit erheben.
12. Ein solcher Leitfaden muss die Spezifika von Medizinprodukten berücksichtigen, wozu die Prinzipen der Patientensicherheit (Safety) und eines risikobasierten Ansatzes zählen. Im konkreten Fall können ausgewählte Maßnahmen der Informationssicherheit ("Controls") den grundlegenden Anforderungen entgegenstehen. Aus diesem Grund kann es für Medizingeräte keine feste Liste von "Controls" geben. Maßgeblich ist jeweils die vom Hersteller festgelegte Zweckbestimmung des Produkts.
14. Die einfache Verständlichkeit und Umsetzbarkeit ist entscheidend für den erhofften positiven Einfluss eines Leitfadens auf die Sicherheit KI-basierter Medizinprodukte. Daher stellt er möglichst keine abstrakten oder "high level" Anforderungen, sondern nennt "binär entscheidbare" Prüfkriterien. 
15. Um die Umsetzbarkeit zu erhöhen, vermeiden die Autoren auch, möglichst viele Anforderungen zusammenzutragen. Vielmehr beschränken sie sich auf diejenigen, die sie für besonders relevant und umsetzbar halten.
16. Auch um die Verteilung und den Bekanntheitsgrad zu fördern, soll der Leitfaden kostenfrei verfügbar sein und bleiben. 
17. Der Leitfaden sollte auf Deutsch und Englisch verfügbar sein.
