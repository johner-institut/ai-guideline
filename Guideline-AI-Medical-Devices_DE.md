# Leitfaden zur KI bei Medizinprodukten

## A) Metainformationen

### 1. Ziele des Leitfadens

Dieser Leitfaden hat das Ziel, Medizinprodukte-Herstellern, Behörden und Benannten Stellen eine Handlungsanleitung und eine konkrete Checkliste an die Hand zu geben, um

- zu verstehen, was die Erwartungen der Benannten Stellen und Behörden sind,
- die schrittweise Umsetzung der Sicherheit von Medizinprodukten zu befördern, die Verfahren der künstlichen Intelligenz, insbesondere des maschinellen Lernens einsetzen,
- das Fehlen einer harmonisierten Norm (zwischenzeitlich) bestmöglich zu kompensieren.

Der Leitfaden hat **nicht** die Zielsetzung, als Lehrbuch oder Leitfaden für das Erreichen der Sicherheit von KI-basierten Medizinprodukten zu dienen. Vielmehr möchte er ein Leitfaden für deren Überprüfung sein.

Der Anhang nennt die Erwägungsgründe, die zur Entwicklung dieses Leitfadens führten.

### 2. Anwendungsbereich und Zielgruppe

Dieser Leitfaden ist nur für Medizinprodukte anwendbar, die Verfahren der KI, insbesondere des maschinellen Lernens verwenden. Der Leitfaden wendet sich insbesondere an 

- **Hersteller** dieser Produkte
- deren Dienstleister (z.B. **Entwicklungsdienstleister**)
- Personen und Organisationen, die die Sicherheit dieser Produkte bewerten müssen, wie beispielsweise Auditoren, **Behörden** und **Benannte Stellen**.


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
3. Anforderungen an die, der Entwicklung nachgelagerten Phasen

#### b) Verbindlichkeit des Leitfadens

Dieser Leitfaden ist weder eine gesetzliche Anforderung noch eine harmonisierte Norm. Entsprechend unterscheidet er auch nicht zwischen normativen und informativen Elementen.

Dieser Leitfaden trägt Best Practices zusammen, um den gesetzlich geforderten "State-of-the-Art" bestmöglich zu beschreiben. Dabei ist zu berücksichtigen, dass eine Fokussierung allein auf diesen "State-of-the-Art" auch zur Entwicklung von Produkten mit geringem Nutzen und sogar Schaden für den Patienten führen und insofern für sich genommen, kein hinreichendes Kriterium sein kann.

Einige dieser Best Practices sind nicht in allen Situationen, bei allen Produkten oder bei allen Verfahren des maschinellen Lernens anwendbar. Hersteller sollten nicht offensichtliche Ausschlüsse begründen.

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

Der Leitfaden ist eine nach dem oben erwähnten Kapitel gruppierte Liste an Überprüfungskriterien. Jedes Listenelement enthält die folgenden Attribute:

- Eindeutige ID
- Überprüfungskriterium, das möglichst einfach und binär als erfüllt oder nicht-erfüllt bewertet werden kann
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
- Dr. Andreas Purde, Dr. Abtin Rad ([TÜV SÜD](https://www.tuev-sued.de/))
- Prof. Dr. Christian Dierks ([Dierks + Company](https://www.dierks.company/))
- Stefan Bunk (CTO) und Sven Piechottka (Government & Regulatory Affairs) ([Merantix](https://www.merantix.com/healthcare/))

Der Leitfaden ist unter der [Creative Commons Lizenz](https://creativecommons.org/licenses/?lang=de) vom Typ [BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/) veröffentlicht. Diese erfordert die Namensnennung der Autoren ("Christian Johner, Christoph Molnar et al. ") und erlaubt es Dritten, auf diesem Werk aufzubauen, z.B. es zu verbessern; letzteres allerdings nur zu nicht-kommerziellen Zwecken.

Die Lizenz gestattet es, das Produkt zu Beratungszwecken einschließlich Audits und Reviews kommerziell einzusetzen. Sie untersagt es aber, dieses Werk selbst in unveränderter oder veränderter Version kommerziell zu nutzen, z.B. in Form eines Verkaufs als Broschüre.


### 5. Dokumentenlenkung, Dokumentenidentifikation

Dieses Dokument wird über das Versionsverwaltungssystem git bzw. die Plattform GitHub verwaltet. Einzig, die in diesem Repository genannten Dokumente sind gültig.

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


### 2. Pläne

Die Hersteller müssen alle regulatorisch geforderten produktspezifischen Pläne erstellt haben:

* Entwicklungsplan (inkl. Verifizierung und Validierungsplanung)
* Post-Market-Surveillance Plan
* Risikomanagementplan
* Plan für die klinische Bewertung


### 3. Kompetenzen

Die Hersteller müssen sicherstellen und nachweisen, dass sie über ausreichend Kompetenzen verfügen, um eine, dem Stand der Technik entsprechende Sicherheit und Leistungsfähigkeit der Produkte zu gewährleisten. Diese Nachweise gelingen oft am leichtesten durch interne oder externe Schulungen.

Hersteller können dabei auch auf die Kompetenz externer Ressourcen zugreifen.

|Anforderung|Kommentare|Regulatorische Referenzen|
|:--|:--|:--|
|Der Hersteller hat eine Liste aller Rollen erstellt, die mit dem Thema KI direkt oder indirekt befasst sind [^B2-01]||ISO 13485, 5.5.1, 6.2., ISO 14971, 3.3., IEC 62304, 2017/745/ EU Artikel 10.9, 21 CFR part 820.30 (b)|
|Der Hersteller hat für jede Rollen die Kompetenzen mit Bezug zur KI bestimmt [^B2-02]|Beispiele für Kompetenzen: Machine Learning, Explainable AI, Medizin (für entsprechende Domäne), klinische und Usability-Validierung|ISO 13485, 6.2., ISO 14971:2019, 4.3, ISO 13485:2016, 7.3.2, IEC 82304, 6.1.|
|Der Hersteller hat angemessene Aufzeichnungen über die Ausbildung, Weiterbildung und Kompetenzen, die den Schluss erlauben, dass die Personen tatsächlich über diese Kompetenzen verfügen||ISO 13485, 6.2.|
|Die (Software-)Entwicklungspläne haben produktspezifisch die (darüberhinausgehenden oder abweichenden) Kompetenzen festgelegt|Anforderung der ISO 13485:2016| ISO 13485, 7.3.2., IEC 82304, 6.1.|


[^B2-01]: Beispiele sind: Data Scientists, Entwickler, Tester, Regulatory Affairs und Qualitätsmanager, Mitarbeiter in Service und Support, Produktmanager, Medizinprodukteberater, Ärztinnen und Ärzte

[^B2-02]: Es sollten Kompetenzen (verstehen, können) und nicht primär Themen genannt sein


### 4. Dokumentation

Die Hersteller sollten den Nachweis führen können, die relevanten Anforderungen dieser Leitlinie beachtet zu haben. Es gibt keine spezifischen Anforderungen an die Dokumentation und "Objective Evidence".

Es besteht zumindest in Europa keine Pflicht, ein spezifisches Dokument zu erstellen, das die Aktivitäten speziell zur KI zusammenfasst. Vielmehr können Hersteller diese Aspekte in bereits bestehenden Dokumenten, wie den Vorgabedokumenten des QM-Systems und der technischen Dokumentation (z.B. Software-Akte, Risikomanagementakte, klinische Bewertung, summative Bewertung der Gebrauchstauglichkeit) integrieren.

## C) Anforderungen an die Produktentwicklung

### 1. Zweckbestimmung und Stakeholder-Anforderungen

#### a) Zweckbestimmung

|Anforderung|Kommentare|Regulatorische Referenzen|
|:--|:--|:--|
|Der Hersteller hat festgelegt, für welches medizinische Ziel (Diagnose, Therapie, Überwachung, Vorhersage) das Medizinprodukt eingesetzt werden soll.|Die Zweckbestimmung ist nicht mit der Beschreibung von Funktionalität (z.B. Berechnung von Scores)  zu verwechseln.| ISO 13485, 4.2.3. und 7.3.2. c., 2017/745/EU Anhang II (1.1), ISO 14971:2019, 5.2, 21 CFR 814.20 (b)(3)(i), 21 CFR part 820.30(c)|
|Der Hersteller hat die Patienten charakterisiert, die mit dem Medizinprodukt diagnostiziert, behandelt oder überwacht werden sollen. Diese Charakterisierung schließt Indikationen, Kontraindikationen und Begleiterkrankungen mit ein.|Diese Charakterisierung fordert auch die IEC 62366-1. Patienten können gleichzeitig auch Nutzer (Anwender) des Produkts sein.| 2017/745/EU, Anhang I, 23.4 und Anhang II, 1.1. c, 2017/746/EU, Anhang 2, 1.1. c, IEC 62366-1, 5.1. und 5.3., ISO 13485, 7.3.3 a., 21 CFR 814.20 (b)(3)(i)|
|Der Hersteller hat festgelegt, an welcher Körperstelle das Produkt angewendet wird bzw. von welcher Körperstelle diese Daten stammen.|Diese Festlegung fordert auch die IEC 62366-1.| 2017/745/EU, Anhang II, 1.1., 2017/746/EU, Anhang II, 1.1., IEC 62366-1, 5.1.3.|
|Die Zweckbestimmung lässt auch erkennen, welches Ziel die Verfahren des maschinellen Lernens verfolgen.|Klassifikation und Regression, Clustering, Similarity Search und Recommender Systems sind typischen Ziele von Verfahren des maschinellen Lernens. Die Beschreibung der Rolle des maschinellen Lernens ist notwendig, um die Anforderung nach der Beschreibung des "physikalischen Prinzips" zu erfüllen.|IEC 62366-1, 5.1, 2017/745/EU Anhang II, 1.1, 21 CFR part 814.20, XAVIER University "Building Explainability and Trust for AI in Healthcare" |
|Der Hersteller hat die vorgesehene Lebensdauer des Medizinprodukts festgelegt.|Diese Lebensdauer bestimmen beispielsweise der Stand der Technik (z.B. medizinischer Fortschritt, neue ML-Methoden, Wettbewerbsprodukte) und die Geschwindigkeit, mit der die technische Umgebung und Bibliotheken weiterentwickelt werden.|

#### b) Vorhergesehene Nutzer, vorhergesehener Nutzungskontext

|Anforderung|Kommentare|Regulatorische Referenzen|
| :--| :--|:--|
| Der Hersteller hat die vorgesehenen Nutzer charakterisiert, z.B. anhand demographischer Merkmale (Alter, Geschlecht), bezüglich der Ausbildung, der Erfahrung in der medizinischen Domäne, bezüglich der technischen Kenntnisse, körperlichen und geistigen Einschränkungen, sprachlichen Fähigkeiten und kulturellem Hintergrund. | Wenn der Hersteller keine Einschränkungen bezüglich dieser Attribute vorsieht, muss er das auch dokumentieren. |2017/745/EU, Anhang I, 5 und Anhang II, 1.1, IEC 62366-1, 5.1., XAVIER University "Building Explainability and Trust for AI in Healthcare"|
| Der Hersteller hat die vorgesehene Nutzungsumgebung charakterisiert (auch soziale Umgebung wie Stress, Schichtbetrieb, häufig wechselnde Kollegen). | Diese Charakterisierung fordert auch die IEC 62366-1. Sie ist auch im Kontext der Erklärbarkeit von KI relevant. |2017/745/EU, Anhang I, 5, IEC 62366-1, 5, XAVIER University "Building Explainability and Trust for AI in Healthcare"|
| Der Hersteller hat die Kernaufgaben beschrieben, die das Medizinprodukt unterstützen soll. | Aus diesen Kernaufgaben können auch die Use Scenarios abgeleitet werden, welche die Hersteller laut IEC 62366-1 spezifizieren müssen. | IEC 62366-1 |


#### c) Stakeholder-Anforderungen

| Anforderung                                       | Kommentare                                                   |Regulatorische Referenzen|
| :-------------------------------------------------| :----------------------------------------------------------- |:---|
| Der Hersteller hat die, in der Zweckbestimmung genannten Ziele mit quantitativen Werten operationalisiert [^C.1.c.1]. | Es ist nicht unüblich, dass diese Werte im Laufe der Entwicklung ergänzt und angepasst werden. | 2017/745/EU, Anhang I, 23.4 und Anhang III, 1.1, FDA SW validation guidance 5.2.2, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. "Software Requirements Specification")|
| Der Hersteller hat die Laufzeitumgebung des Produkts bezüglich Hardware (Bildschirmgröße, Bildschirmauflösung, Speicher, Netzwerkanbindung etc.) und Software (z.B. Betriebssystem, Browser, Run-time Environments wie Java Run-time Environment oder .NET) bestimmt. | Bei Apps kann es sein, dass diese Charakterisierung für die App und für den Server-Teil erfolgen muss. |ISO 13485, 7.3.3, 2017/745/EU, Anhang I, 17.3 und 17.4, IEC 62304, 5.2, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA SW validation guidance 5.2.2, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. "Software Requirements Specification")|
| Der Hersteller hat die Datenschnittstellen anhand der Ebenen des  [Interoperabilitätsmodells](https://www.johner-institut.de/blog/tag/interoperabilitat/) spezifiziert und dabei auch die Formate und bei Bildern deren spezifischen Eigenschaften (Größe, Auflösung, Farbkodierung) festgelegt. | Diese wird auch gemäß IEC 62304 Kapitel 5.2.2 benötigt. | IEC 62304, 5.2.2, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. "Software Requirements Specification")|
| Der Hersteller hat die Anforderungen an die Input-Daten spezifiziert | Die Input-Daten können auch von der Generierung der Daten abhängen z.B. vom Aufnahmeverfahren, von technischen Parametern (Magnetfeldstärken, Anzahl der Ableit-Elektroden, Richtung), von Umgebungsbedingungen bei den Aufnahmen, vom Hersteller, vom Medizinprodukt usw..| IEC 62304, 5.2, ISO 14971:2019, 5.3, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. "Software Requirements Specification") |
| Der Hersteller hat alle Märkte und alle dort relevanten regulatorischen Anforderungen festgelegt. | Diese Liste sich zeigen lassen. | 2017/745/EU, Anhang IX, 2.2, ISO 13485, 5.2 and 7.2.1 | 
| Der Hersteller hat festgelegt, ob das System nach der Inverkehrbringung weiter dazulernen soll. Falls dies der Fall ist, hat der Hersteller dargelegt, ob dieses kontinuierliche Training global/zentral oder dezentral (z.B. pro Produkt oder pro Krankenhaus) sowie online oder offline erfolgt. |                                                              |

[^C.1.c.1]: **Beispiel**: Zweck: Die Software unterstützt Radiologen beim Diagnostizieren von Krebserkrankungen anhand CT-Bilder des Schädels. Quantitativer Wert: 95% der Radiologen, die mit der Software arbeiten, erkennen den Krebs. 


#### d) Input für Risikomanagement und die klinische Bewertung

| Anforderung                                       | Kommentare                                              | Regulatorische Referenzen|
| :-------------------------------------------------| :-------------------------------------------------------|:---|
| Der Hersteller hat alternative Verfahren aufgelistet und bezüglich Nutzen, Sicherheit und Leistungsfähigkeit bewertet. | Die Diskussion des State-of-the-Art ist eine Forderung der MEDDEV 2.7/1 und der MDR/IVDR. | 2017/745/EU, Anhang I, 1., 2017/746/EU, Anhang I, 1., MEDDEV 2.7/1, ISO 14971:2019, 4.2 und 10.9, FDA guidance on "Factors to Consider When Making Benefit-Risk Determinations in Medical Device Premarket Approval" (e.g. Part C) |
| Der Hersteller hat die o.g. quantitativen Werte mit den entsprechenden Größen der alternativen Verfahren verglichen. | Hersteller sollten eine tabellarische Übersicht erstellen.   |
| Der Hersteller hat begründet, weshalb Machine Learning den anderen Verfahren überlegen ist und die damit einhergehenden Risiken rechtfertigt. | |2017/745/EU, Anhnag I, 1., 2017/746/EU, Anhang I, 1., MEDDEV 2.7/1 | 
| Der Hersteller hat eine Liste an Risiken erstellt, die sich spezifisch durch die Anwendung der Verfahren des maschinellen Lernens ergeben. | Ist Teil der Risikomanagementakte|ISO 14971, 5.4. und 5.5., 2017/745/EU, Anhang I, 3., DIN SPECT 2, ISO/TR 31004:2013 - Risk management - Guidance for the implementation of ISO 31000|
| Der Hersteller hat die Risiken analysiert, die sich ergeben, wenn andere als die spezifizierten Patienten mit dem Produkt diagnostiziert, therapiert oder überwacht werden. | | |
| Der Hersteller hat die Risiken analysiert, die sich ergeben, wenn andere als die spezifizierten Nutzer das Produkt nutzen. |   | ISO 14971, 5. |
| Der Hersteller hat die Risiken analysiert, die sich ergeben durch die Nutzung in einer anderen als der spezifizierten Nutzungsumgebung. | | 2017/745/EU, Anhang I, 14.2.(d), 2017/746/EU, Anhang I, 13.2.(d), ISO 14971, 5., IEC 82304, 4.1. (b)|
| Der Hersteller hat die Risiken analysiert, die sich ergeben durch Inputs, die nicht den spezifizierten Formaten genügen. || ISO 14971, 5., IEC 82304, 4.1. (c)|
| Die Hersteller haben Risiken analysiert, die sich ergeben durch Daten, die nicht entsprechend der spezifizierten Voraussetzungen generiert wurden. |                                                              |
| Der Hersteller hat die Risiken bewertet, wenn das System bei einer anderen Patientenpopulation als der spezifizierten eingesetzt wird. |    | ISO 14971, 4.2., 4.3., 5., IEC 82304, 4.1.|


### 2. Software-Anforderungen

#### a) Funktionalität und Leistungsfähigkeit

|Anforderung|Kommentare|Regulatorische Referenzen|
|:--|:--|:--|
|Der Hersteller hat aus der Zweckbestimmung nachvollziehbar quantitative Gütekriterien bzw. Anforderungen an die Software oder/und den Algorithmus abgeleitet [^C.2.a.1].|Diese Nachvollziehbarkeit lässt sich mit einer Traceability-Matrix besonders gut  darstellen.| ISO 13485, 7.3.3., IEC 62304, 5.2, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA guidance on "Software Validation", Kapitel 5.2.2 |
|Der Hersteller hat beispielsweise die folgenden quantitativen Gütekriterien bzw. Anforderungen in Betracht gezogen: für Klassifikationsprobleme Genauigkeit (Mean oder Balanced Accuracy), positiver prädikativer Wert (Precision), Spezifität und Sensitivität; für Regressionsprobleme Mean Absoute Error und Mean Square Error.| Bei unbalancierten Daten, d.h. wenn Labels sehr unterschiedlich häufig vorkommen, sollte Balanced statt Mean Accuracy verwendet werden. Die Wahl der Gütekriterien hängt jedoch stark von der Zweckbestimmung ab. | ISO 13485, 7.3.3., 7.3.4., IEC 62304, 5.2. |
|Der Hersteller hat die erwarteten Wertebereiche der Outputs spezifiziert.|| ISO 13485, 7.3.3., 7.3.4., IEC 62304, 5.2. |
|Der Hersteller hat die Anforderungen bezüglich der Wiederholbarkeit und Reproduzierbarkeit von Anforderungen spezifiziert.|Dies ist besonders bei "Continuous Learning Systems" relevant.| 2017/745/EU, Anhang I, 17.1., 2017/746/EU, Anhang I, 16.1., ISO 13485, 7.3.3., 7.3.4 |
|Der Hersteller hat festgelegt, wie sich das System verhält, wenn die Inputs nicht die spezifizierten Voraussetzungen erfüllen[^C.2.a.2].|Dies ist ein Aspekt der Robustheit, der gemäß ISO 25010 und IEC 62304 Kapitel 5.2 zu spezifizieren ist.| ISO 25010,, IEC 62304, 5.2., ISO 14971:2019, 5.4, FDA guidance on "Software Validation" Kapitel 5.2.2, FDA digital health criteria| |
|Der Hersteller hat festgelegt, welche Selbsttests das System durchführen muss, und wie es sich verhält, wenn diese nicht erfolgreich sind.|Dies ist besonders bei "Continuous Learning Systems" relevant.|
|Der Hersteller hat festgelegt, wie schnell das System die Outputs erzeugen muss.|Diese Festlegung kann ggf. abhängig von der Größe und Menge der Daten erfolgen.| 2017/745/EU, Anhang I, 17.1., 2017/746/EU, Anhang I, 16.1., ISO 13485, 7.3.3.|
|Der Hersteller hat die Verfügbarkeit des Medizinprodukts spezifiziert.|Dies ist ein Aspekt der Robustheit, der gemäß ISO 25010 und IEC 62304 Kapitel 5.2 zu spezifizieren ist.| ISO 25010, IEC 62304, 5.2., ISO 14971, 4.3., ISO 13485, 7.3.3.|

[^C.2.a.1]: Beispiele:  **Beispiel 1**: Die Stakeholder-Anforderungen lautet, dass 95% der Radiologen einen Krebsfall mit dem Produkt erkennen können müssen. Die Anforderung an den Algorithmus lautet, dass er eine Sensitivität von 97% aufweisen muss. **Beispiel 2**: Die Stakeholder-Anforderungen lautet, dass Arterienverkalkungen mit einer Sensitivität von 92% erkannt werden müssen. Die Anforderungen an den Algorithmus lautet, dass er die Stärke der Plaques im Blutgemäß auf 0,2mm genau vorhersagen muss.

[^C.2.a.2]:  Beispiele: unvollständige Datensätze, fehlende Datensätze, falsche Datenformate, zu große Datenmengen, Daten außerhalb spezifizierter Wertebereiche, falsche zeitliche Abfolge von Daten.

#### b) User Interface

| Anforderung| Kommentare| Regulatorische Referenzen|
| :--| :--|:--|
| Der Hersteller hat spezifiziert, was das User Interface anzeigen muss, wenn die Voraussetzungen nicht erfüllt sind[^C.2.a.2], um das System sicher zu betreiben (z.B. nicht valide oder nicht erwartete Inputs). | | 2017/745/EU, Anhang I, 5., 2017/746/EU, Anhang 1, 5., IEC 62366-1, 5.2., FDA HFE guidance, FDA guidance on software validation, Kapitel 5.2.3 | 
| Der Hersteller hat spezifiziert, was das User Interface anzeigen muss, wenn die Outputs nicht den spezifizierten Gütekriterien entsprechen. |                                                          |
| Der Hersteller hat festgelegt, ob es einer Gebrauchsanweisung und Trainingsmaterialien bedarf. | Die MDR / IVDR erlauben Ausnahmen von der Verpflichtung. | 2017/745/EU, Anhang I, 23., 2017/746/EU, Anhang I, 20., ISO 13485, 4.2.3., FD&C, 21 CFR parts 801 and 820.120|

#### c) Weitere Software-Anforderungen

| Anforderung| Kommentare| Regulatorische Referenzen|
| :--| :--|:--|
| Der Hersteller hat festgelegt, welche Anforderungen das System erfüllen muss, um ein Fehlverhalten des Systems feststellen zu können. | Könnten ein Auditlog oder ein Monitoring-Port sein. | 2017/745/EU, Anhang I, 17, 18, 23.4, IEC 62304, 5.2, 5.3 und 7.1, ISO 149781:2019, 5.4, FDA guidance on software validation e.g. Kapitel 5.2.2, 5.2.3 und 5.2.4, GMLP Guiding Principles (by FDA et al) #2 (data integrity) |
| Gemäß DSGVO dürfen Patienten durch das spezifizierte System nicht Entscheidungen ausgesetzt sein, welche ausschließlich auf automatischer Datenverarbeitung beruhen. Hersteller sollten sich mit der entsprechenden Vorgabe auseinandersetzen und die gewählte rechtliche Grundlage begründen können. | Anforderung des Art. 22 der DSGVO. | Artikel 22, DSGVO |
| Der Hersteller hat die Anforderungen bestimmt, die die Software erfüllen muss, um die IT-Sicherheit des Produkts zu gewährleisten. | Die IT-Sicherheit ist nicht Gegenstand dieser Leitlinie, sondern der [IT-Sicherheits-Leitlinie](https://github.com/johner-institut/it-security-guideline/). |

#### d) Besondere Anforderungen an kontinuierliche lernende Systeme

| Anforderung| Kommentare| Regulatorische Referenzen|
| :--| :---|:--|
| Der Hersteller hat festgelegt, wann und wie häufig das Modell aktualisiert wird. | Hierzu sollte der Hersteller die "Trigger" dieser Updates festlegen. Er muss auch beschreiben, ob diese Updates pro einzelnem Medizinprodukt oder für alle Medizinprodukte des Typs erfolgen. |
| Der Hersteller hat festgelegt, wie die zusätzlichen Daten qualitätsgesichert werden und wie mit falschen, fehlenden oder umplausiblen Daten umgegangen wird. |                                                              |
| Der Hersteller hat festgelegt, in welchem Bereich sich die Output-Daten ändern dürfen. | Das setzt eine Beschreibung voraus, wie sich die Algorithmen ändern. |
| Der Hersteller hat beschrieben, wie er die Korrektheit und Genauigkeit der Output-Daten weiterhin sicherstellt und was passiert, wenn dies nicht mehr gewährleistet werden kann. | Selbstchecks, die Möglichkeit zu Roll-backs, die Begrenzung der Outputs sind mögliche Ansätze. |
| Der Hersteller hat beschrieben, ob und wie die Anwender über Änderungen des Algorithmus informiert werden und ob diese darüber entscheiden können. |                                                              |
| Der Hersteller hat die spezifischen Risiken identifiziert und beherrscht, die sich durch das kontinuierliche Lernen ergeben. | Dazu muss der Hersteller begründen, dass er durch das kontinuierliche Lernen ein besseres Nutzen-Risiko-Verhältnis erreicht. |


### 3. Datenmanagement

Daten sind grundsätzlich zu unterscheiden in Trainings-, Validierungs- und Testdaten, an welche unterschiedliche Anforderungen gestellt werden können. 

Insofern in diesem Kapitel nicht näher spezifiziert, schließt der Begriff "Daten" alle drei Arten mit ein.

#### a) Sammlung der Daten

| Anforderung| Kommentar| Regulatorische Referenzen|
| :--| :--| :--|
| Der Hersteller hat die Anzahl der Datensätze festgelegt und eine Begründung gegeben, weshalb diese ausreichend ist[^C.3.a.1]. | Das betrifft die Datensätze für Training, Validierung und Test. | ISO 13485, 7.3.7 |
| Der Hersteller hat die Ein- und Ausschlusskriterien von Daten  anhand relevanter Attribute[^C.3.a.2] charakterisiert. | Das schließt eine Dokumentation der Datentypen, Einheiten und Wertebereich mit ein. | ISO 24028, XAVIER University "Building Explainability and Trust for AI in Healthcare" |
| Der Hersteller hat technische Ein- und Ausschlusskriterien für Daten spezifiziert[^C.3.a.3]. |                                                              |
| Der Hersteller hat das Verfahren beschrieben, mit dem er sicherstellt, dass Datensätze, die nicht den Einschlusskriterien genügen bzw. ausgeschlossen werden sollen, tatsächlich ausgeschlossen werden. | Das Verfahren schließt eine softwaregestützte Bewertung mit ein. Diese Software ist zu validieren. |
| Der Hersteller hat die gesammelten Daten mit Hilfe einer deskriptiven Statistik beschrieben[^C.3.a.4]. | Empfehlenswert ist das ["Dataset Nutrition Label"](https://ahmedhosny.github.io/datanutrition/). |
| Der Hersteller hat begründet, wo er Testdaten sammelt und weshalb diese repräsentativ für die Zielpopulation sind. So sinnvoll, haben sie diese mit Daten des Bundesamts für Statistik, aus wissenschaftlichen Publikationen und von Registern verglichen. |                                                              |
| Der Hersteller hat Faktoren gelistet und diskutiert, die einen "Bias" der Trainings-, Validierungs- und Testdaten verursachen könnten. |  | ISO 24028, 10.5, DAISAM |      |
| Der Hersteller hat analysiert, welche Einflüsse die Art und der Ort der Datensammlung auf die Daten hat[^C.3.a.5]. |                                                              |
| Der Hersteller hat ein Verfahren etabliert, mit dem er gewährleistet, dass die Anforderungen an den Datenschutz erfüllt sind. | Beispielsweise werden die Daten vor dem Testen und Training anonymisiert bzw. pseudonymisiert. Hierzu sollte der Datenschutzbeauftragte einbezogen werden. |
| Der Hersteller hat Möglichkeiten eines "Label Leakages" untersucht und ausgeschlossen[^C.3.a.6]. | Dies ist abhängig von dem angewandten ML-Modell und lässt sich nicht generell als Best Practice einfordern. |
| Der Hersteller, der Fragebögen verwendet, hat die Wahl der Fragen, den Zeitpunkt der Befragung und ggf. die Methode zu deren Auswertung begründet, insbesondere wenn kein standardisierter Fragebogen vorliegt. |                                                              |

[^C.3.a.1]: Eine generelle Vorgabe für die Anzahl von Daten kann es nicht geben. Diese hängt u.a. vom "Signal-Noise-Ratio" ab. Beispielsweise würde bei einem Gendatensatz der Prozentsatz relevanter Gene und die Stärke und Häufigkeit des vorherzusagenden Effekts die Anzahl beeinflussen. Bei Daten, die klassifiziert werden sollen, ist die Anzahl der Datensätze mit der selteneren Klasse (z.B. die Prävalenz von Krankheiten) entscheidend.

[^C.3.a.2]: z.B. demographische Daten (Alter, Geschlecht), körperliche Parameter (Größe, Gewicht), Erkrankungen, Vitalparameter, Laborparameter, Vorhandensein weitere Untersuchungen, Anamnese.

[^C.3.a.3]: Beispiele: **Beispiel 1**: Patienten, die wegen eines Herzschrittmachers oder einer Lungen-OP ausgeschlossen werden müssen, weil die Bilder nicht ausgewertet werden können oder zu Fehlklassifikation führen könnten. **Beispiel 2**: Formate und technischen Parameter wie Bildgrößen, Auflösungen, Helligkeit und Kontraste, Farbkodierung, Kompression, Aufnahmerichtungen, Aufnahmeverfahren (z.B. CT versus MRT), mit ohne Kontrastmittel, Zoom. **Beispiel 3**: Vollständigkeit von Meta-Daten.

[^C.3.a.4]: Übliche sind die Berechnung von Verteilungen (Histogrammen), Mittelwerten, Quartilen, ggf. "Joint Distribution of Features". Auch die Korrelation von Daten untereinander sollte untersucht sein. Weitere Beispiele finden sich in der in der [Publikation von Sarah Holland et al.](https://arxiv.org/pdf/1805.03677.pdf) (z.B. in der Tabelle 1)

[^C.3.a.5]: Beispiele: Einfluss von verschiedenen Messgeräten, Befragungen, Policies (z.B. ein Klinik nimmt Laborparameter nur im Notfall, eine andere routinemäßig. Frequenz und Anlass, mit der Patienten untersucht werden), Art der Klinik (z.B. kleines Krankenhaus, aus dem alle schweren Fälle verlegt werden versus Maximalversorger > Survivor Bias), Self-Selection Bias (z.B. Patienten mit diversen Vorerkrankungen gehen eher in ein Krankenhaus statt in eine Arztpraxis), Art der Studie (prospektiv versus retrospektiv)

[^C.3.a.6]: Das sind Daten, bei denen nicht-kausale Informationen über das Label in den Daten stecken z.B. in der Sortierung (z.B. erst die Daten von Gesunden, dann die von Kranken), im Krankenhaus (von einem stammen die schweren Fälle), im Bild (z.B. bei Hautkrebs ist immer noch ein Lineal zu sehen). Ein weiteres Beispiel wären mehrere CT-Bilder eines Patienten, bei denen das Modell anhand des Patienten und nicht der Krankheit lernt. Das könnte z.B. passieren, wenn auf mehreren Bildern mit Krebs auch ein Rippenbruch zu erkennen ist. 

#### b) Labeling von Daten

| Anforderung| Kommentar| Regulatorische Referenzen|
| :--| :-- | :-- |
| Der Hersteller hat beim "Supervised Learning", die Labels aus der Zweckbestimmung abgeleitet, mit denen die Trainingsdaten versehen werden und diese Wahl begründet. |                                                              |
| Der Hersteller hat beim "Supervised Learning" ein Verfahren fürs Labeling festgelegt, falls noch keine Labels in den Daten vorhanden waren. |    | ISO 13485, 4.1 |                                                   
| Dieses Verfahren spezifiziert quantitative Klassifizierungskriterien für das Labeling. Die Wahl dieser Kriterien hat der Hersteller begründet[^C.3.b.1]. | Falls nicht der "Ground Truth"[^C.3.b.2] gewählt wird, weil dieser z.B. zu teuer oder zu invasiv ist, muss dies ebenfalls begründet sein. |
| Dieses Verfahren spezifiziert die Anforderungen an die Anzahl, Ausbildung und Kompetenz der für das Labeling verantwortlichen Personen. | |  ISO 13485, 6.2 and 7.3.2, FDA 21 CFR part 820.25  |
| Dieses Verfahren legt fest, wie die Kompetenz der für das Labeling verantwortlichen Personen geprüft wird. | Dies kann durch das Labeling von ausgewählten Datensätzen erfolgen. |
| Dieses Verfahren legt fest, wie die, für das Labeling verantwortlichen Personen geschult werden und wie der Erfolg dieser Schulung überprüft wird. |                                                              |
| Dieses Verfahren legt fest, wie die Korrektheit der Labels systematisch überprüft wird. Die Wahl dieser Begründung hat der Hersteller dokumentiert. | Der Hersteller kann identische Datensätzen mehreren Personen zum Labeling vorlegen und die Übereinstimmung der Ergebnisse bewerten. |
| Dieses Verfahren legt fest, wie überwacht wird, dass die für das Labeling verantwortlichen Personen auch während des Labelings dauerhaft leistungsfähig und leistungswillig sind[^C.3.b.3]. | Dies kann durch Datensätze mit bereits bekanntem Label erfolgen, die beim Labeling für die Person unmerklich eingeschoben werden. |

[^C.3.b.1]: Wenn beispielsweise die Klassifizierung in gesunde und kranken Patienten erfolgen soll, muss der Hersteller die Kriterien für die spezifische Fragestellung bzw. Zweckbestimmung ableiten, wann ein Patient als gesund und als krank zu klassifizieren ist.

[^C.3.b.2]: Der "Ground Truth" ist das präziseste Referenzverfahren ("Stand der Wissenschaft"). Für die Bestimmung einer arteriellen Hypertonie kann es z.B. eine invasive Blutdruck-Messung die genausten Ergebnisse und damit den "Ground Truth" bilden. 

[^C.3.b.3]: Das Labeling Dutzender Datensätze ist anstrengend. Eine Bezahlung pro Datensatz kann falsche Motivationsanreize setzen.

#### c) Verfahren zur (Vor-)Verarbeitung von Daten 

| Anforderung| Kommentar| Regulatorische Referenzen|
| :--| :-- | :-- |
| Der Hersteller hat ein Verfahren festgelegt, das die (Vor-)Verarbeitung ("pre-processing") der Daten beschreibt. |    | ISO 13485:2016, 4.1.6, 7.3.6, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA 21 CFR part 820.70(i)  |
| Dieses Verfahren beschreibt die einzelnen Verarbeitungsschritte wie Umrechnungen, Transformationen, Aggregationen, Normalisierung, Formatumwandlungen, Berechnung von Feature, Umwandlung numerischer Daten in Kategorien. | Eine graphische Darstellung verschafft einen schnellen Überblick. Die Umwandlung von numerischen in kategoriale Werte bedarf einer Begründung. | ISO 13485:2016, 4.1.6, 7.3.6, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA 21 CFR part 820.70(i)  |
| Das Verfahren beschreibt, wie die Korrektheit der Zwischenschritte und der Endergebnisse überprüft wird[^C.3.c.0]. Diese Überprüfungen erfolgen risikobasiert. | Dies entspricht den Anforderungen der ISO 13485:2016 Kapitel 4.1.6. Die Risikomanagementakte muss diese Analysen enthalten. | ISO 13485, 4.1.6., 7.3.2., 7.5.6. |
| Dieses Verfahren spezifiziert, wie Werte mit verschiedenen Messskalen bzw. Einheiten erkannt und verarbeitet werden. | Dies ist abhängig von dem angewandten ML-Verfahren (z.B. tabellarischen Daten / Bilddaten) und lässt sich nicht generell als Best Practice einfordern. |
| Dieses Verfahren spezifiziert, wie Werte, die mit verschiedenen Messverfahren bestimmt wurden, erkannt und verarbeitet werden. | Dies ist abhängig von dem angewandten ML-Verfahren (z.B. tabellarischen Daten / Bilddaten) und lässt sich nicht generell als Best Practice einfordern. |
| Dieses Verfahren spezifiziert, wie Werte bzw. Metadaten mit gleichem Namen (z.B. in Spaltenköpfen) erkannt und verarbeitet werden. | Dies ist abhängig von dem angewandten ML-Verfahren (z.B. tabellarischen Daten / Bilddaten) und lässt sich nicht generell als Best Practice einfordern. |
| Dieses Verfahren spezifiziert, wie fehlende Werte innerhalb von Datensätzen erkannt und verarbeitet werden. Diese Festlegung hat der Hersteller begründet[^C.3.c.1]. | Es ist darauf zu achten, dass der Hersteller bei der Begründung zwischen "missing at random" und "missing not at random" unterscheidet[^C.3.c.2]. |
| Dieses Verfahren spezifiziert, wie Outliers insb. bei tabellarischen Daten erkannt und verarbeitet werden[^C.3.c.3]. Diese Festlegung hat der Hersteller begründet[^C.3.C.4]. | Exemplarisch für ein Datum / Feature zeigen lassen. Dies ist abhängig von dem angewandten ML-Verfahren und lässt sich nicht generell als Best Practice einfordern. |
| Dieses Verfahren spezifiziert, wie nicht verwendbare Datensätze erkannt werden und damit umgegangen wird.[^C.3.c.5]. Diese Festlegung hat der Hersteller begründet. | Exemplarisch für ein Datum / Feature zeigen lassen.          |
| Der Hersteller hat die Risiken identifiziert, bewertet und beherrscht, die sich durch die Datenverarbeitung ergeben. | Risiken können beispielsweise verursacht werden durch Software-Fehler, Rundungsfehler, Re-Sampling und Komprimierung von Daten sowie das Aussortieren ungültiger Daten. |  AI4H-DAISAM | 


[^C.3.c.0]: Zu den Möglichkeiten der Überprüfung zählen Software-Tests und redundante bzw. alternative Berechnungen z.B. mit Excel.

[^C.3.c.1]: Zu den Optionen der Verarbeitung zählen, den Datensatz zu löschen, Ersetzen durch den Mittelwert anderer Datensätze, neuer Wert "missing" (bei kategoriellen Werten)

[^C.3.c.2]: Ein Beispiel für "missing not at random" sind zu hohe Laborwerte, die abgeschnitten werden.

[^C.3.c.3]: Zu den Optionen der Verarbeitung zählen, den Datensatz zu löschen, den Wert zu korrigieren, den Wert auf einen festgelegten Wert (Min/Max) zu setzen.

[^C.3.c.4]: Diese Begründung ist bei Regressionsverfahren wichtiger als bei Baum-Verfahren.

[^C.3.c.5]: Beispiele sind Röntgenbilder mangelnder Qualität, Patienten, die nicht den Inklusionskriterien entsprechen.

#### d) Dokumentation und Versionskontrolle

| Anforderung| Kommentar| Regulatorische Referenzen|
| :-- | :-- | :-- |
| Der Hersteller hat den "Funnel" beschrieben, der erkennen lässt, wie viele Daten aus welchen Datenquellen (z.B. Kliniken) stammen und bei welchem Verarbeitungsschritt, wie viele Datensätze aus welchem Grund weggefallen sind. |                                                              |
| Der Hersteller hat beschrieben, welche Teile der Software für welchen Verarbeitungsschritt verantwortlich sind. | Das sollte Teil der Architektur dieser Software sein.        |
| Der Hersteller hat die verarbeiteten Daten mit Hilfe einer deskriptiven Statistik beschrieben[^C.3.a.4]. | Empfehlenswert ist das ["Dataset Nutrition Label"](https://ahmedhosny.github.io/datanutrition/) |
| Der Hersteller hat alle Software zur Datenverarbeitung einschließlich, der dabei verwendeten Bibliotheken dokumentiert und unter Versionskontrolle. | | ISO 13485, 4.1.6., 4.2.4., 7.5.6. |


### 4. Modellentwicklung

#### a) Vorbereitung

| Anforderung| Kommentar|Regulatorische Referenzen|
| :--| :-- |:-- |
| Der Hersteller hat die Auswahl der Feature begründet, die er beim Training berücksichtigt. | Das setzt eine Liste aller Features voraus.                   | ISO 13485, 7.3.2., 7.3.3. |
| Der Hersteller hat insb. bei tabellarischen Daten, die Abhängigkeit der Features untereinander beschrieben. | Ein Directed Acyclic Graph (DAG) hilft bei der Visualisierung. Dies ist abhängig von dem angewandten ML-Verfahren und lässt sich nicht generell als Best Practice einfordern. | ISO 13485, 7.3.2., 7.3.3. |
| Der Hersteller hat dokumentiert und begründet, in welchem Verhältnis er die Daten in Trainings-, Validierungs- und Testdaten aufteilt. |                                                              |
| Der Hersteller hat dokumentiert, nach welcher Stratifizierung er die Daten in Trainings-, Validierungs- und Testdaten aufteilt[^C.4.a.1]. |    |  ISO 24028 9.8.2.1, DAISAM|
| Der Hersteller hat dokumentiert, wie er sicherstellt, dass mehrere Datensätze zu einem Objekt im gleichen "Bucket" (Trainings-, Validierungs- bzw. Testdaten) sind. |                                                              |
| Der Hersteller hat dokumentiert, wie er sicherstellt, dass die Testdaten nicht beim Training und Validieren des Modells verwendet wurden. |                                                              |
| Der Hersteller hat beschrieben, wenn er die Daten spezifisch für das Modell oder spezifisch für die Bibliothek umkodiert[^C.4.a.2]. |                                                              |

[^C.4.a.1]: Bei Daten mit seltenen Feature oder Labels kann es notwendig sein, die Daten nicht ausschließlich nach dem Zufallsprinzip zu verteilen.

[^C.4.a.2]: Beispiele dafür sind Normalisierung, Wahl von Klassen-Labels (z.B. 0 oder 1), Wahl von Spaltennamen, Aufteilung von kategoriellen Werten auf mehrere Spalten.

#### b) Training

| Anforderung| Kommentar| Regulatorische Referenzen|
| :-- | :--|:--|
| Der Hersteller führt Modelltraining, Optimierung der Hyperparameter und Modellselektion ausschließlich mit den Trainings- und Validierungsdaten (mittels Kreuzvalidierung) durch. | Dabei sollte der Hersteller auch aufzeigen, dass das Training die Güte des Modells tatsächlich verbessert. |
| Der Hersteller hat verschiedene Sätze an Hyperparametern ausprobiert und seine abschließende Wahl dokumentiert. [^C.4.b.1]. |                                                              |
| Der Hersteller hat ggf. die Wahl der Epochen dokumentiert. [^C.4.b.2] |                                                              |
| Der Hersteller hat die Gütemaße bestimmt, dokumentiert und anhand der Zweckbestimmung begründet, für die er das Modell optimieren will. | D.h. die Wahl dieser Gütemaße ist spezifisch für die Zweckbestimmung. |
| Der Hersteller hat - soweit sinnvoll - mehrere Modelltypen trainiert und verglichen (darunter auch einfachere und interpretierbare Modelle). |                                                              |
[^C.4.b.1]: Beispiele: Loss-Funktion, Optimizer, Lernrate, Anzahl Epochen

[^C.4.b.2]: Es kann sinnvoll sein, die Abhängigkeit der Güte des Modells von der Anzahl der Epochen anhand von Learning Curves aufzuzeigen. Diese Learning Curves gibt es beispielsweise für neuronale Netzwerke und Boosting-Verfahren, nicht aber für Modelle mit numerischer Lösung (z.B. lineare Regression) oder bei einem einzigen Baum.	

#### c) Bewertung

| Anforderung| Kommentar| Regulatorische Referenzen|
|:--|:--|:--|
| Der Hersteller hat die Bewertung des Modells geplant. | Dieser Plan kann Teil eines Entwicklungs- oder V&V-Plans sein. | ISO 13485, 7.3.2, 7.3.6 und  7.3.7, ISO 14971:2019, 10. |
| Der Hersteller hat für die verschiedenen Modelle die Gütemaße z.B. bei einer binären Klassifikation mit Hilfe einer Vierfeldertafel dokumentiert. | Diese Dokumentation sollte nicht nur die Werte umfassen, auf die der Hersteller das Modell optimiert hat. |
| Der Hersteller hat die Gütemaße für die verschiedenen Modelle  nicht nur global bewertet und dokumentiert, sondern ggf. auch getrennt für verschiedene Feature. |                                                              |
| Der Hersteller hat aufgezeigt, wie er ein Overfitting erkennen und so vermeiden kann. | | ISO 24028 9.8.2.23 |
| Der Hersteller hat die Datensätze untersucht, die besonders gut  und die besonders schlecht vorhergesagt wurden. | Empfehlenswert ist eine Residuen-Analyse, bei der ggf. die Fehler über die Feature-Werte aufgetragen sind. |
| Der Hersteller hat die Datensätze untersucht, bei denen sich das Modell besonders sicher und besonders unsicher[^C.4.c.1] ist. |                                                              |
| Der Hersteller hat anhand der Gütekriterien und der Zweckbestimmung die letztliche Wahl des Modells begründet und insbesondere dargelegt, wenn einfachere und interpretierbarere Modelle nicht zur Anwendung kamen. |   | ISO 14971:2019, XAVIER University "Building Explainability and Trust for AI in Healthcare", DIN SPECT 2 |
| Der Hersteller hat erwogen, sich insbesondere bei tabellarischen Daten für einzelne Datensätze die Feature anzeigen zu lassen, die das Modell besonders zur Entscheidung bewogen haben[^C.4.c.2]. | Dies lässt sich nicht generell als Best Practice einfordern. |
| Der Hersteller hat erwogen insbesondere bei tabellarischen Daten zu evaluieren, wie und wie stark sich einzelne Feature ändern müssten, damit das Modell zu einer anderen Vorhersage kommt. | Man spricht von ["Counterfactuals"](https://christophm.github.io/interpretable-ml-book/counterfactual.html). Dies lässt sich nicht generell als Best Practice einfordern. |
| Der Hersteller hat insbesondere bei tabellarischen Daten erwogen, die Abhängigkeit (Stärke, Richtung) der Vorhersagen von den Feature-Werten zu analysieren/ zu visualisieren [^C.4.c.3]. | Dies lässt sich nicht generell als Best Practice einfordern. |
| Der Hersteller hat erwogen, Datensätze zu synthetisieren, die das Modell besonders aktivieren[^C.4.c.4]. | Dies lässt sich nicht generell als Best Practice einfordern. |
| Der Hersteller hat erwogen, das Modell durch ein vereinfachtes Surrogat-Modell, wie einen Entscheidungsbaum zu approximieren. | Dies lässt sich nicht generell als Best Practice einfordern. |

[^C.4.c.1]: Bei Klassifikationsaufgaben ist der aktuelle Stand der Forschung zu berücksichtigen.

[^C.4.c.2]: zu den Ansätzen zählen LIME (Local Interpretable Model-agnostic Explanations), Beta (Black Box Explanations through Transparent Approximations), LRP (Layer-wise Relevance Propagation) und Feature Summary Statistics (inkl. Feature Importlande und Feature Interaktion.	

[^C.4.c.3]: Beispiele sind Sharpley-Values, ICE-Plots, Partial Dependency Plots (PDP)	

[^C.4.c.4]: Beispiele siehe http://yosinski.com/deepvis


#### d) Dokumentation 

| Anforderung| Kommentar| Regulatorische Referenzen|
| :-- | :-- |:-- |
| Der Hersteller hat das Modell[^C.4.d.1] und/oder den Trainingscode unter Versions- und Konfigurationskontrolle. | Das schließt Scripts und Build-Files mit ein. | ISO 13485, 4.1.6., 4.2.4., 7.5.6. |
| Der Hersteller hat seinen Code gemäß einer Policy dokumentiert. | Üblicherweise sind zumindest öffentliche Klasse, Methoden mit Übergabe- und Rückgabewerten sowie Attribute zu dokumentieren |
| Der Hersteller hat beschrieben, welche Datensätze er für das Training, für die Validierung und das Testen des Modells verwendet hat. |     | ISO 24028 9.8.2.1, DAISAM|
| Der Hersteller kann die Test- und Validierungsergebnisse reproduzieren. | Dazu ist der Einsatz eines Versionsverwaltungssystems nicht nur für den  Code, sondern auch für Daten, Testergebnisse und deren Bewertung sinnvoll. Es empfiehlt sich, auch die bei der Datenverarbeitung und dem Training verwendete Infrastruktur (Hardware, Betriebssystem, Virtualisierungsschichten wie Docker) zu dokumentieren. Abweichende Ergebnisse sind zu begründen (z.B. Hardware, Zufallsgeneratoren,  Rundungsfehler). Absolute Pfade und betriebssystemspezifische Befehle sind zu vermeiden. Eine README-Datei im .txt oder Markdown-Format hilft, sich in der Dokumentation schneller zurecht zu finden. | ISO 13485, 7.3.6., 7.3.3. |
| Der Hersteller hat die SOUP (Bibliotheken und Frameworks) unter Versions- und Konfigurationskontrolle. || IEC 62304, 8.1.2. |
| Der Hersteller hat die Architektur des Modells und das Modell selbst inklusive dessen Algorithmen und Hyperparameter dokumentiert. | Beispielsweise sollte bei einem CNN u.a. die Anzahl und Art der Schichten, die Verknüpfung der Neuronen bzw. Schichten, die Aktivierungsfunktion, der Optimizer und anderer Parameter inklusive deren Wertebereiche dokumentiert werden. Zur Dokumentation des Modells zählt auch die Spezifikation der Outputs, wie die Anzahl der Outputs, die jeweiligen Datentypen, Wertebereiche, Einheiten usw.. | ISO 13485, 4.2.3., 4.2.5. |
| Der Hersteller hat beschrieben, wie er die Architekturen ausgewählt, die Modelle trainiert und die Hyperparameter optimiert, und dieses Vorgehen begründet. | Prüfer möchten nachvollziehen können, wie die Hersteller vorgegangen sind und weshalb die gewählte Lösung die beste ist. Die IEC 62304 und die FDA wünschen keine "ad hoc design decisions". |
| Der Hersteller hat beschrieben, wenn er mit einem "Pretrained Model" gearbeitet hat, und dargelegt, weshalb dieses "Pre-Training" der Aufgabenstellung angemessen ist. ||
| Der Hersteller hat die Güte der Modelle basierend auf den Gütemaßen dokumentiert. | Diese Gütemaße beziehen sich auf Prüfung mit den Testdaten.  | ISO 13485, 4.2.3., 4.2.5. |
| Der Hersteller hat die Konfidenzintervalle für die Güteparameter abhängig für die Inputdaten angegeben. | Gerade an den Rändern der erlaubten Input-Daten sinkt häufig die Konfidenz stark ab. Diese Information sollte auch den Anwendern in den Begleitmaterialen zur Verfügung gestellt werden. |
| Der Hersteller hat insbesondere bei tabellarischen Daten dokumentiert, innerhalb welcher Grenzen (z.B. Feature-Werte) das Modell, die Anforderungen an die Gütemaße erreicht. | Dies ist abhängig von dem angewandten ML-Modell und lässt sich nicht generell als Best Practice einfordern. | ISO 13485, 4.2.3., 4.2.5. |
| Der Hersteller hat mehrere Modelle und deren Hyperparameter ausprobiert und dafür, die in diesem Abschnitt genannten Aspekte dokumentiert. | Diese Dokumentation dient dem Hersteller dazu, verschiedene Modelle zu vergleichen und seine Wahl eines Modells zu begründen. Dies ist notwendig, um die Anforderung der ISO 14971 zu erfüllen, das Nutzen-Risiko-Verhältnis zu maximieren. |

[^C.4.d.1]: Trainierte Modelle lassen sich serialisieren.


### 5. Produktentwicklung

#### a) Software-Entwicklung

| Anforderung| Kommentar| Regulatorische Referenzen|
| :--| :-- |:-- |
| Der Hersteller hat alle von der IEC 62304 geforderten Aktivitäten durchgeführt und dokumentiert. | Hinweis für Auditoren[^C.5.a.1]  | IEC 62304, IEC 82304, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA guidance on software validation, FDA OTS guidance  |
| Wenn der Hersteller das Modell in einer anderen Programmiersprache oder für eine andere Laufzeitumgebung implementiert hat, hat er einen Plan erstellt, welche der Aktivitäten gemäß Kapitel 4. wiederholt. || IEC 62304, IEC 82304 | 
| Der Hersteller prüft die Performance (Antwortzeiten, Ressourcenverbrauch) auf der Zielhardware (z.B. Browser, Mobilgerät). | | 2017/745/EU, Anhang I, 17.1., 17.3., 2017/746/EU, Anhang I, 16.1., 16.3. | 
| Der Hersteller hat für alle SOUP- bzw. OTS-Komponenten beschrieben, wie diese zu verifizieren sind und diese Verifizierung auch durchgeführt und dokumentiert. |  | IEC 62304, 5.3, 8.1.2, FDA OTS guidance | |
| Der Hersteller hat der Software die vorgeschriebenen Lizenzbedingungen beigefügt und die Rechtmäßigkeit der Verwendung von Software Dritter (z.B. Open Source Software) sichergestellt. | Hersteller nutzen häufig Open Source Software, welche nur im Rahmen von Lizenzen und Copy Right Angaben verwendet werden darf. |

[^C.5.a.1]: Die Hersteller sollten die üblichen Best-Practices einhalten wie das Einhalten von Coding-Guidelines, die Überprüfung des Codes durch Code-Reviews anhand definierte Kriterien, das Testen des Codes durch Unit-, Integrations- und Software-System-Tests mit einem definierten Abdeckungsgrad usw. Eine Beschreibung des Codes (Architektur) sollte einfach nachvollziehbar machen, welcher Code, welche Aufgabe übernimmt.

#### b) Begleitmaterialien

| Anforderung| Kommentar| Regulatorische Referenzen|
| :-- | :-- |:-- |
| Die Gebrauchsanweisung identifiziert eindeutig die Version des Produkts. | Falls möglich, die UDI angeben  | 2017/745/EU, Anhang I, Kapitel. III, 23.1, 23.4., FD&C, FDA 21 CFR parts801 and 820.120, ISO 24028 e.g. 10.11.3 |
| Die Gebrauchsanweisung beschreibt die Zweckbestimmung des Produkts einschließlich des erwarteten medizinischen Nutzens. |   | 2017/745/EU, Anhang I, Kapitel III, 23.1, 23.4., 21 CFR part 801, 21 CFR part 814.20, XAVIER: "Perspectives and Good Practices for AI and Continuously Learning Systems in Healthcare", ISO 24028, XAVIER University "Building Explainability and Trust for AI in Healthcare", ISO 24028 e.g. 10.11.3|
| Die Gebrauchsanweisung legt die vorgesehene Patientenpopulation anhand Indikationen, Kontraindikationen und so relevant anhand weiterer Parameter, wie Alter, Geschlecht, Begleiterkrankungen oder Verfügbarkeit von Informationen fest. | | 2017/745/EU, Anhang I, Kapitel. III, 23.1, 23.4. |
| Die Gebrauchsanweisung nennt explizit die Patienten / Daten  / Anwendungsfälle, bei denen das Produkt nicht verwendet werden darf. |   | 2017/745/EU, Anhang I, Kapitel. III, 23.1, 23.4. |
| Die Gebrauchsanweisung dokumentiert die Anforderungen an die Input-Daten (inklusive Formate, Auflösungen, Wertebereich etc.). |                                                              |
| Die Gebrauchsanweisung spezifiziert die vorgesehenen primären und sekundären Anwender gemäß Zweckbestimmung. |                                                              |
| Die Gebrauchsanweisung beschreibt, von welchen sonstigen Voraussetzungen das Produkt ausgeht (z.B. Laufzeitumgebung, Nutzungsumgebung). |                                                              |
| Die Gebrauchsanweisung beschreibt, wie das Produkt genutzt werden soll. | Das schließt auch das Verhalten im Fehlerfall und die sekundäre Nutzung, wie die Installation, das Upgrade und die Konfiguration mit ein. |
| Die Gebrauchsanweisung beschreibt die möglichen Outputs.     | Das schließt auch die Erklärungen des Produkts ("Explainability") mit ein. |
| Die Gebrauchsanweisung beschreibt die Restrisiken.           |   | 2017/745/EU, Anhang I, 23.4, ISO 14971:2019, 8, ISO 24028 e.g. 10.11.3 |
| Die Gebrauchsanweisung gibt an, mit welchen Daten das Modell trainiert wurde. | Dies bezieht sich sowohl auf das Patientenkollektiv als auch auf die verwendeten Features. |
| Die Gebrauchsanweisung beschreibt das Modell bzw. die Algorithmen. |                                                              |
| Die Gebrauchsanweisung benennt die Gütekriterien.            | Hier auch Konfidenz-Bereiche angeben.                        |
| Die Gebrauchsanweisung listet die Faktoren auf, die sich negativ auf die Gütekriterien auswirken können. |                                                              |
| Die Gebrauchsanweisung spezifiziert, ob das Produkt während der Anwendung weiter trainiert wird. | Bitte Hinweise im Kapitel zu den kontinuierliche lernenden Systemen beachten. |
| Die Gebrauchsanweisung beschreibt, wie Updates erfolgen.     |  |
| Die Gebrauchsanweisung enthält ggf. Verweise auf weiterführende Literatur. |  |
| Die Gebrauchsanweisung enthält ggf. Hinweise zu Lizenzrechten. |   | 2017/745/EU, Anhang I, 23.4, EU-Regulation 207/2012|
| Die Gebrauchsanweisung identifiziert den Hersteller und nennt Kanäle, über die Rückfragen zu stellen sind. | | 2017/745/EU, Anhang I, 23.4, EU-Regulation 207/2012|
| Die Gebrauchsanweisung nennt mögliche ethische Problematiken. |                                                              |
| Die Gebrauchsanweisung benennt die URL, unter der die aktuellsten Versionen der Gebrauchsanweisung zu finden sind. |     | 2017/745/EU, Anhang I, 23.4, EU-Regulation 207/2012|

#### c) Usability-Validierung

| Anforderung| Kommentar| Regulatorische Referenzen|
| :-- | :-- |:-- |
| Der Hersteller bewertet im Rahmen der Usability Validierung, ob die Nutzer die Gebrauchsanweisung verstehen. | Das schließt andere Begleitmaterialien mit ein. | IEC 62366-1, FDA HFE guidance |
| Der Hersteller bewertet im Rahmen der Usability Validierung, ob die Nutzer dem Produkt blind vertrauen oder die Ergebnisse nachprüfen. |  | IEC 62366-1 |
| Der Hersteller bewertet im Rahmen der Usability Validierung, ob die Anwender die Ergebnisse korrekt erkennen und verstehen. | Das schließt auch die Anzeige von Fehlern und die Erklärungen ("Explainability") mit ein. Hersteller sollten alle sicherheitsbezogenen Use Scenarios bei der Validierung und alle risikominimierenden Maßnahmen am Interface einbeziehen. | IEC 62366-1, 5.7. – 5.9. |

#### d) Risikomanagement

| Anforderung| Kommentare| Regulatorische Referenzen|
| :-- | :--| :--|
| Der Hersteller hat die Risiken bewertet, die sich ergeben, wenn die Inputs nicht die spezifizierten Voraussetzungen erfüllen[^C.2.a.2]. |   | ISO 14971:2019, 5.4, IEC 62304, 7.1, DIN SPEC 2, IEC 82304, 4.1.c)|
| Der Hersteller hat die quantitativen Güterkriterien anhand des Stands der Technik abgeleitet. | Der Hersteller muss die Gütekriterien für alternative Technologien und Verfahren benennen und argumentieren können, wenn das Medizinprodukt den Alternativen bezüglich der Gütekriterien nicht überlegen ist[^C.5.d.1]. |
| Der Hersteller hat den Goldstandard festgelegt und dessen Wahl begründet, mit dem die Gütekriterien überprüft werden sollen. |  | XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA proposed regulatory framework for modifications to AI/ML based SaMD: "reference standard" |
| Der Hersteller hat Risiken identifiziert, bewertet und beherrscht, die sich ergeben, wenn die Outputs nicht den spezifizierten Gütekriterien entsprechen. | Bei dieser Analyse betrachtet der Hersteller auch die spezifischen Eigenschaften des gewählten Modells sowie die beim Testen bestimmten Konfidenz-Intervalle der Output-Werte. | ISO 14971:2019, 5.3, IEC 62304, 7.1, IEC 82304, 4.1.c), XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA guidance on software validation, 5.2.2 |
| Der Hersteller hat die Folgen bewertet, wenn das System sozial inakzeptable Outputs liefert (z.B. diskriminierend). | Diese "Folgen" sind nicht notwendigerweise Risiken im Sinne der ISO 14971. | Ethische Leitlinien für vertrauenswürdige KI |
| Der Hersteller hat die Risiken identifiziert, bewertet und beherrscht, wenn das System nicht verfügbar ist. |                                                              |
| Der Hersteller hat die Risiken identifiziert, bewertet und beherrscht, die durch Software-Fehler entstehen. | Das beinhaltet auch Fehler in SOUP sowie in der Software, die für das "Pre-Processing" der Daten und für das Training des Modells verwendet wird. |
| Der Hersteller hat die Risiken identifiziert, bewertet und beherrscht, die durch die spezifische Wahl der Modell-Architektur entstehen. | Dabei sollten die Hersteller auch analysieren, ob die Modelle auf die richtigen Vorgaben hin optimiert wurden. | ISO 14971:2019 |
| Der Hersteller hat die Risiken identifiziert, bewertet und beherrscht, die durch die spezifische Wahl der Zielplattform entstehen. | Beispielsweise könnte die Zielplattform nicht die benötigte Rechenleistung bereitstellen oder zum Absturz der Software führen. |
| Der Hersteller hat die Risiken identifiziert, bewertet und beherrscht, die durch die Auswahl der Trainings-, Validierungs- und Testdaten ergeben. | Das betrifft sowohl die Quellen dieser Daten (wie Patienten, Institutionen) als auch die Aufteilung dieser Daten in Trainings-, Validierungs- und Testdaten. So sollten die Hersteller prüfen, dass kein Overfitting und kein Bias der Daten vorliegen. |
| Der Hersteller hat die Risiken identifiziert, bewertet und beherrscht, die sich dadurch ergeben, dass die Outputs (Vorhersagen, Klassifikationen etc.) nur zufällig richtig sind. | Mit Hilfe der "Interpretability" können Hersteller darlegen, weshalb ein ML-Modell eine konkrete Entscheidung getroffen hat. |
| Der Hersteller hat die Risiken identifiziert, die sich dadurch ergeben, dass die Vorhersagen selbst die vorhergesagten Ergebnisse ändern. | Bei diesem Phänomen wird das Model vom Beobachter zum Akteur[^C.5.d.2]. Es nennt sich "Performative Prediction". Die Hersteller sollten die möglichen Auswirkungen auf Menschen oder Systeme untersuchen und z.B. mit einem DAC ("directed acyclic graph") beschreiben, einen möglichen "Distribution Shift" und ggf. eine nicht beeinflusste Kontrollgruppe beobachten und bei Bedarf Maßnahmen ergreifen, wie z.B. ein anderes Model wählen oder das bestehende Modell neu trainieren. |
| Falls der Hersteller Selbsttests verwendet, hat er dargelegt, welche der spezifizierten Gütekriterien damit überprüft werden und welche Risiken dadurch beherrscht sind. |                                                              |
| Der Hersteller hat die Risiken durch Nutzungsfehler identifiziert, bewertet und beherrscht. | Diese Risiken sollten auch berücksichtigen, dass Anwender die Erklärung der Outputs ("Explainability") nicht oder falsch erkennen bzw. verstehen. | IEC 62366-1, 5.3f, FDA HFE guidance, FDA guidance on software validation, 5.2.3 | 
| Der Hersteller hat die sonstigen Risiken identifiziert, bewertet und beherrscht, die das Kapitel C.1.d) nennt. |                                                              |

[^C.5.d.1]: Der Stand der Technik (State-of-the-Art) entspricht nicht notwendigerweise dem Goldstandard, der wiederum nicht notwendigerweise dem "Ground Truth". D.h. die Anforderungen an das System können geringer sein als bei einem Goldstandard oder dem "Ground Truth", inbesondere wenn letztere ein invasives oder sehr kostenintensives Verfahren bedingen.
[^C.5.2.d]: Beispiele für dieses Phänomen finden sich [hier](https://mindfulmodeler.substack.com/p/correction-you-can-break-a-predictive). 

#### e) Klinische Bewertung 

| Anforderung| Kommentar | Regulatorische Referenzen|
| :-- | :-- |:-- |
| Der Hersteller hat im Rahmen der klinischen Bewertung bewertet, ob der versprochene medizinische Nutzen bei den gegebenen Güteparametern erreicht wird. |    | 2017/745/EU, Artikel 61, Anhang XIV und Anhang XV, 2017/746/EU, Anhang XIII und Anhang XIV, MEDDEV 2.7/1 rev.4, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA 21 CFR part 820.30(g)|
| Der Hersteller hat im Rahmen der klinischen Bewertung bewertet, ob der versprochene medizinische Nutzen und die Risiken, dem Stand der Technik entsprechen. |           |2017/745/EU, Artikel 61, Anhang XIV und Anhang XV, 2017/746/EU, Anhang XIII and Anhang XIV, MEDDEV 2.7/1 rev 4, ISO 14971:2019, 4.2  |


### 6. Produktfreigabe

| Anforderung| Kommentar| Regulatorische Referenzen|
| :-- |:-- |:-- |
| Der Hersteller hat sichergestellt, dass alle o.g. Dokumentation vorliegt. | Das betrifft u.a. die  in den Kapitel 3.d), 4.d und 5.b) geforderte Dokumentation. | 2017/745/EU, Anhänge I und II, ISO 13485, 7.3.5., FDA 21 CFR part 820.30(e) |
| Der Hersteller hat im Risikomanagement die Risiken als akzeptabel bewertet und dokumentiert, dass alle im Risikomanagementplan spezifizierten Aktivitäten durchgeführt wurden. | Hinweis für Auditoren[^C.6.1]                                |
| Der Hersteller hat bei Systemen, die er in den USA in den Verkehr bringen will, in den "Software as a Medical Device Pre-Specifications“ (SPS) dargelegt, welche Arten der Änderungen er antizipiert[^C.6.2]. |                                                              |
| Der Hersteller hat bei Systemen, die er in den USA in den Verkehr bringen will, im Algorithm Change Protocol (ACP) dargelegt, wie er diese Änderungen durchführen will[^C.6.3]. |                                                              |
| Der Hersteller hat einen Post-Market Surveillance Plan erstellt (s.u.). |                                                              |

[^C.6.1]: Anhand von Beispielen prüfen, dass die Wirksamkeit von Risikokontrollmaßnahmen geprüft wurde, dass es eine Traceability von Risiken zu Risikokontrollmaßnahmen gibt.

[^C.6.2]: Änderungen können die Zweckbestimmung, Dateninput, die klinische und analytische Leistungsfähigkeit betreffen.

[^C.6.3]: Das Vorgehensmodell muss z.B. eingehen auf den Umgang mit Daten, auf das Re-Training, auf die Leistungsbewertung und auf die Updates.


## D) Anforderungen an die der Entwicklung nachgelagerten Phasen

#### 1. Produktion, Distribution, Installation

|Anforderung|Kommentare|Regulatorische Referenzen|
|:--|:--|:--|
|Der Hersteller hat beschrieben, wie sichergestellt ist, dass nur genau die vorgesehenen Artefakte (Dateien) in genau der vorgesehenen Version im Produkt oder als Produkt ausgeliefert werden|Hier geht es ums Konfigurationsmanagement. Auch bei Downloads oder AppStores relevant|IEC 62304, 5.8.8.|
|Der Hersteller hat beschrieben, wie die für die Installation verantwortlichen Personen wissen, welches die aktuellste Version ist und wie Verwechselungen bei der Installation ausgeschlossen werden können|Dies ist nur bei stand-alone Software relevant. Hier wäre eine Verfahrens- oder Arbeitsanweisung zu erwarten| ISO 13485, 7.8.3., 8.3., IEC 62304, 5.8.4. |
|Der Hersteller hat beschrieben, wie bei der Installation sichergestellt wird, dass die Anforderungen, die in den Begleitmaterialien spezifiziert sind (s.o.), tatsächlich erfüllt sind|Hier wäre eine Verfahrens- oder Arbeitsanweisung zu erwarten| ISO 13485, 7.5.3. |
|Der Hersteller hat Verfahren etabliert, die gewährleisten, dass er mit den Betreibern und Anwendern seiner Produkte zeitnah kommunizieren kann|| ISO 13485, 7.2.3., 8.3.3., IEC 82304, 8.4. |


#### 2. Überwachung nach der Inverkehrbringung

|Anforderung|Kommentare|Regulatorische Referenzen|
|:--|:--|:--|
|Der Hersteller hat einen Post-Market Surveillance (PMS) Plan erstellt.|| 2017/745/EU, Artikel 10, i, Artikel 83, Anhang III, 1.1, FD&C act 522, 21 CFR part 822, IEC 62304 7.1.3, XAVIER: "Perspectives and Good Practices for AI and Continuously Learning Systems in Healthcare", ISO 24028, DIN SPECT 2, FDA proposed regulatory framework for modifications to AI/ML based SaMD chapter IV, Anhang C- IT security Guidelines |
|Der Hersteller hat in diesem PMS-Plan die Daten spezifiziert, welche er sammeln und auswerten will.|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII |
|Der Hersteller hat im PMS-Plan spezifiziert, bei welchen Gütekriterien und Grenzwerten er eine Handlung, insbesondere eine Neubewertung des Nutzen-Risiko-Verhältnisses für notwendig erachtet.|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII |
|Der Hersteller hat beim Festlegen dieser Schwellenwerte analysiert, welche Feedback-Loops die Schwellenwerte selbst beeinflussen können[^D.2.1].|Diese Analyse dient auch als Maßnahme gegen das o.g. Risiko durch "Performance Prediction".| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII |
|Der Hersteller hat beim Festlegen dieser Schwellenwerte analysiert, welche Self-Fullfilling-Prophecies die Schwellenwerte selbst beeinflussen können[^D.2.2].|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII |
|De Hersteller hat im PMS-Plan beschrieben, wie er welche Informationen zu unerwünschten medizinischen Nebenwirkungen sammelt und bewertet.|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII |
|Der Hersteller hat im PMS-Plan beschrieben, wie er welche Informationen zu (unerwünschten) Verhaltensänderungen bzw. (vorhersagbarem) Missbrauch sammelt und bewertet[^D.2.3]|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII |
|Der Hersteller hat im PMS-Plan beschrieben, wie er welche Informationen zu weiteren "unerwünschten Nebenwirkungen" sammelt und bewertet[^D.2.4].|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII |
|Der Hersteller hat im PMS-Plan beschrieben, wie er welche Informationen sammelt, um bewerten zu können, ob die Daten im Feld den erwarteten Daten bzw. den Trainingsdaten entsprechen[^D.2.5].|Hinweis für Auditoren[^D.2.6]| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII |
|Der Hersteller hat im PMS-Plan beschrieben, wie und wie oft er Informationen darüber sammeln will, ob das Produkt noch dem State-of-the-Art genügt.|Hinweis für Auditoren[^D.2.7]| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII |
|Der Hersteller hat im PMS-Plan beschrieben, wie und wie oft er Informationen darüber sammeln will, ob der "Ground Truth" bzw. der Goldstandard noch aktuell ist.|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII |
|Der Hersteller hat im PMS-Plan beschrieben, wie und wie oft er überprüft, dass Änderungen konform dem Algorithm Change Protocol (ACP) und innerhalb der „SaMD Pre-Specifications“ (SPS) erfolgen.|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII |
|Die in den Plänen geforderten Berichte liegen zu den darin bestimmten Zeitpunkten vor.|z.B. PSUR|

[^D.2.1]: Beispiel für Feedback-Loops: **Beispiel 1**: Eine Reise-Empfehlungs-App verschickt abhängig von Feature (letzte Reise) gezielte Werbung. Diese wiederum beeinflusst das Reiseverhalten. **Beispiel 2**: Ein Algorithmus stellt Prognosen. Daher behandelt der Arzt die Patienten besser oder früher.

[^D.2.2]: Beispiele 1 (Kriminalistik)

[^D.2.3]: Beispiel: Radiologen verlassen sich auf die Software und schauen sich die Bilder nicht mehr an, weshalb sie Befunde übersehen.

[^D.2.4]: Beispiele wären ethische Herausforderungen wie beispielsweise, der YouTube-Algorithmus, der zwar das Ziel erreicht, die Klick-Zahl bzw. die Nutzungsdauer zu maximieren, dabei aber Gewalt- und Verschwörungsvideos promotet.

[^D.2.5]: Man spricht von einem Distribution Shift bzw. von einer Data Drift.

[^D.2.6:]: Der Hersteller sollte Schwellenwerte für Feature oder für die Varianz / Kovarianz über die Zeit festlegen. Dies lässt sich insbesondere bei nicht-normalverteilten Daten über den Vergleich von Histogrammen oder Kerndichteschätzern visualisieren bzw. quantifizieren.

[^D.2.7]: Sich vom Hersteller beispielsweise den Prozess erklären lassen, wie er sich systematisch über neue Entwicklungen im Machine Learning informiert, wie er diese Entwicklungen bewertet sowie darauf reagiert.


#### 3. Außerbetriebnahme

| Anforderung| Kommentare|Regulatorische Referenzen|
| :-- | :-- |:-- |
| Der Hersteller hat einen Plan für die Außerbetriebnahme erstellt, bevor er sein Produkt aus dem Markt nimmt. | Solch ein Plan legt z.B. fest, ob und wie die Software deinstalliert werden muss, ob Daten gesichert oder exportiert werden müssen, wie die Vertraulichkeit der Daten gewährleistet bleibt, wer für diese Aktivitäten verantwortlich ist, wie der Fortschritt der Außerbetriebnahme überwacht und sichergestellt wird und welche Organisationen wie zu informieren sind. | ISO 24028 |
| Der Hersteller identifiziert, bewertet und beherrscht die Risiken, die sich aus der Außerbetriebnahme ergeben. | Dies ist in der Risikomanagementakte zu bewerten. Risiken durch die Nichtverfügbarkeit des Produkts, durch Nutzungsfehler und durch einen Einfluss auf andere Produkte sollten dabei betrachtet werden. | 2017/746/EU Anhang I, 3., ISO 14971:2019 Kapitel 10 in Kombination mit 3.8 und 3.12, ISO 24028 |


## E) Anhänge

### 1. Weiterführende Literatur

#### a) Gesetze

- [MDR](https://www.johner-institut.de/blog/regulatory-affairs/medical-device-regulation-mdr-medizinprodukteverordnung/)
- [IVDR](https://www.johner-institut.de/blog/regulatory-affairs/ivdr-in-vitro-diagnostic-device-regulation/)

#### b) Normen und Best-Practice Guides

- **IEC 62304/AMD1**, Medical device software – Software life cycle processes
- **IEC 82304-1**, Health software – Part 1: General requirements for product safety
- [FDA Guidance Documents zum Machine Learning](https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-and-machine-learning-software-medical-device)

#### c) Fachliteratur, Lehrbücher

- Christoph Molnar: [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/)
- Patrick Hall: [Machine Learning Interpretability
  with H2O Driverless AI](http://docs.h2o.ai/driverless-ai/latest-stable/docs/booklets/MLIBooklet.pdf)
- Patrick Hall: [On the Art and Science of Machine Learning Explanations](https://arxiv.org/pdf/1810.02909.pdf)
- Johner Institut: [Videotrainings zum Machine Learning bei Medizinprodukten](www.auditgarant.de)
- Johner Institut: Diesen [Leitfaden in anderen Formaten](https://www.johner-institut.de/ai-guideline/) z.B. als Excel-Datei zum einfachen bearbeiten

#### d) Quellen und Checklisten zur Reproduzierbarkeit

- https://www.cs.mcgill.ca/~jpineau/ReproducibilityChecklist-v2.0.pdf
- https://epub.ub.uni-muenchen.de/92151/1/92151.pdf
- https://github.com/craig-willis/reproducibility-checklist/
- https://2020.emnlp.org/call-for-papers#new-reproducibility-criteria
- https://onlinelibrary.wiley.com/pb-assets/assets/15214036/RR_Guideline.pdf

### 2. Erwägungsgründe

1. Hersteller entwickeln immer mehr Medizinprodukte, die Verfahren der künstlichen Intelligenz, insbesondere des Machine Learnings, nutzen. Viele dieser Verfahren sind noch sehr neu und Best Practices fehlen. Dadurch entstehen Risiken für Patienten, Anwender und Dritte.
2. Die EU-Verordnungen (MDR, IVDR) fordern zwar explizit die Sicherheit der Produkte in den jeweiligen Anhängen I. Konkrete Anforderungen für diese Klasse der Produkte fehlen jedoch völlig. Daher fehlen sowohl den Herstellern als auch den Benannten Stellen und Behörden konkrete Leitlinien, wie sie die Sicherheit der Produkte bewerten können.
3. Im Gegensatz zu den meisten anderen grundlegenden Anforderungen sind keine Normen zum Thema KI harmonisiert. Daher gibt es keinen kanonischen Katalog an Anforderungen, der anerkannt den geforderten Stand der Technik reflektiert.
4. Die FDA hat begonnen, Anforderungen an den Umgang mit Continuous Learning Systems CLS zu formulieren. Diese Vorgaben sind ungeeignet, um bereits bei der Produktentwicklung ausreichend konkrete Anforderungen an die Produkte und Prozesse zu stellen. 
5. Die Sicherheit der Medizinprodukte muss in allen Phasen des Produkt-Lebenszyklusprozesses berücksichtigt werden. Eine Beschränkung auf das Testen ist unzureichend. Dieser Tatsache müssen Best Practices und Leitfäden gerecht werden. 
9. Es ist zu hoffen, dass Normen zur Sicherheit von KI-basierten Medizinprodukten entwickelt und harmonisiert werden. Das wird jedoch noch Jahre in Anspruch nehmen. Daher bedarf es eines Leitfadens (nur) in dieser Zwischenphase. 
10. Dieser Leitfaden soll zeitnah (bis Juli 2019) zur Verfügung stehen, um rasch den Herstellern als Orientierung zu dienen und es ihnen zu ermöglichen, sofort zu handeln. Die hohe Geschwindigkeit seiner Entwicklung macht Kompromisse bezüglich der Abstimmung mit möglichst vielen Parteien unumgänglich.
11. Der technologische Fortschritt im Bereich der künstlichen Intelligenz ist immens. Neue Verfahren und Technologien werden kontinuierlich publiziert. Einerseits soll ein Leitfaden so spezifisch wie möglich sein. Andererseits darf er nicht zu spezifisch auf ein Verfahren oder eine Technologie ausgerichtet sein, um eine sinnvolle "Haltbarkeitsdauer" zu erreichen. Daher muss ein Leitfaden allgemeine Konzepte adressieren und kann nie einen Anspruch auf Vollständigkeit erheben.
12. Ein solcher Leitfaden muss die Spezifika von Medizinprodukten berücksichtigen, wozu die Prinzipen der Patientensicherheit (Safety) und eines risikobasierten Ansatzes zählen. Im konkreten Fall können ausgewählte Maßnahmen der Informationssicherheit ("Controls") den grundlegenden Anforderungen entgegenstehen. Aus diesem Grund kann es für Medizingeräte keine feste Liste von "Controls" geben. Maßgeblich ist jeweils die vom Hersteller festgelegte Zweckbestimmung des Produkts.
14. Die einfache Verständlichkeit und Umsetzbarkeit ist entscheidend für den erhofften positiven Einfluss eines Leitfadens auf die Sicherheit KI-basierter Medizinprodukte. Daher stellt er möglichst keine abstrakten oder "high level" Anforderungen, sondern nennt "binär entscheidbare" Prüfkriterien. 
15. Um die Umsetzbarkeit zu erhöhen, vermeiden die Autoren auch, möglichst viele Anforderungen zusammenzutragen. Vielmehr beschränken sie sich auf diejenigen, die sie für besonders relevant und umsetzbar halten.
16. Auch um die Verteilung und den Bekanntheitsgrad zu fördern, soll der Leitfaden kostenfrei verfügbar sein und bleiben. 
17. Der Leitfaden sollte auf Deutsch und Englisch verfügbar sein.
