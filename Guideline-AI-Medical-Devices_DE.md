# Leitfaden für KI-basierte Medizinprodukte und IVD

## A) Metainformationen

### 1. Ziel des Leitfadens

Das Ziel dieses Leitfadens ist es, Herstellern von Medizinprodukten und IVD, Behörden und benannten Stellen Anweisungen und eine konkrete Checkliste zur Verfügung zu stellen, um

- zu verstehen, welche Erwartungen die benannten Stellen und Behörden haben, die sich ergeben aus den Vorschriften 
  - für Medizinprodukte wie [MDR](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32017R0745) (Verordnung (EU) 20 17/745 über Medizinprodukte) und der
  - [IVDR](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32017R0746) (Verordnung (EU) 2017/746 über In-vitro-Diagnostika) sowie
  - der [KI-Verordnung](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689) (Verordnung (EU) 2024/1689 über künstliche Intelligenz),

- die schrittweise Sicherheit von Medizinprodukten und IVD zu fördern, die Methoden der künstlichen Intelligenz, insbesondere maschinelles Lernen, verwenden,
- um das Fehlen einer harmonisierten Norm (in der Zwischenzeit) so weit wie möglich auszugleichen.

Der Leitfaden soll **nicht** als Schulungshandbuch oder Leitfaden dienen, wie man sichere KI-basierte Medizinprodukte bzw. IVD entwickelt. Er soll ein Leitfaden für deren Überprüfung sein.

Im Anhang sind die Erwägungsgründe aufgeführt, die zur Entwicklung dieses Leitfadens geführt haben.

### 2. Anwendungsbereich und Zielgruppe

Dieser Leitfaden gilt nur für Medizinprodukte und IVD, die KI-Methoden, insbesondere maschinelles Lernen, verwenden. Die Anforderungen der KI-Verordnung betreffen jedoch meist nicht Medizinprodukte der Klasse I und IVD der Klasse A.


Der Leitfaden gilt insbesondere für
- Hersteller dieser Produkte
- Ihre Dienstleister (z. B. Entwicklungsdienstleister)
- Personen und Organisationen, die die Sicherheit dieser Produkte bewerten müssen, wie z. B. Auditoren, Behörden und benannte Stellen.

Der Leitfaden deckt nur allgemeine Sicherheits- und Leistungsanforderungen in Bezug auf KI ab. Er befasst sich z. B. nicht mit Aspekten der IT-Sicherheit, es sei denn, sie sind KI-spezifisch. Die IT-Sicherheit ist Gegenstand einer [dedizierten Leitfaden zur IT-Sicherheits](https://github.com/johner-institut/it-security-guideline/).

### 3. Gebrauchsanweisung

#### a) Struktur des Leitfadens

Dieser Leitfaden folgt dem Gedanken, dass die Sicherheit von KI-basierten Medizinprodukten nur durch einen prozessorientierten Ansatz erreicht werden kann, bei dem alle relevanten Prozesse und Phasen des Lebenszyklus berücksichtigt werden, wie z. B.:

1. Forschung und Entwicklung
2. Datenmanagement
3. Überwachung nach dem Inverkehrbringen

Dementsprechend legt der Leitfaden keine spezifischen Anforderungen an die Produkte fest, sondern an die Prozesse. Er enthält die folgenden Kapitel:

1. Allgemeine Anforderungen
2. Anforderungen an die Produktentwicklung
   1. Zweckbestimmung
   2. Softwareanforderungsspezifikation
   3. Datenverwaltung
   4. Modellentwicklung
   5. Produktentwicklung
   6. Produktfreigabe

3. Anforderungen an die der Entwicklung nachgelagerte Phase

#### b) Verbindlichkeit des Leitfadens

Dieser Leitfaden ist weder eine gesetzliche Anforderung noch eine harmonisierte Norm. Dementsprechend unterscheidet er nicht zwischen normativen und informativen Anforderungen.

Vielmehr stellt der Leitfaden "Best Practices" zusammen, um den erforderlichen „Stand der Technik“ widerzuspiegeln.

Einige dieser bewährten "Best Practices" sind nicht in allen Situationen, für alle Produkte oder für alle Methoden des maschinellen Lernens anwendbar. Die Hersteller sollten zumindest nicht offensichtliche Ausschlüsse begründen.

#### c) Verwendung des Leitfadens

##### Erstellung und Überprüfung von Vorgabedokumenten

Die Hersteller sollten zunächst den Leitfaden verwenden, um die Vollständigkeit der Vorgabedokumente (Prozess- und Arbeitsanweisungen, Checklisten usw.) zu überprüfen. Diese Aufgaben werden normalerweise von den folgenden Rollen übernommen:

- Prozessbezogene Personen, insbesondere Leiter und Leiterinnen der Entwicklung, des Risikomanagements und des Produktmanagements
- Qualitätsmanager und Qualitätsmanagementbeauftragte
- Regulatory Affairs Manager

##### Bewertung von Produkten und QM-System

Dann sollten die Personen, die für die folgenden Aufgaben verantwortlich sind, den Leitfaden verwenden:

- Überprüfung der Konformität von Produkten mit den grundlegenden Sicherheits- und Leistungsanforderungen
- Bewertung der Konformität der technischen Dokumentation mit den regulatorischen Anforderungen
- Bewertung der Wirksamkeit des internen Qualitätsmanagementsystems (z. B. für Design Reviews oder Audits)

Die folgenden Rollen sind normalerweise für diese Aufgaben verantwortlich:

- Qualitätsmanager / Qualitätsmanagerinnen
- Externe und interne Auditoren / Auditorinnen (einschließlich benannter Stellen)
- Interne und externe Prüfer /Prüferinnen der technischen Dokumentation (einschließlich benannter Stellen und Behörden)
- Tester
- "Data Scientists"
- Spezialisten für klinische Angelegenheiten
- Regulatory Affairs Manager
- Risikomanager / Risikomanagerinnen

#### d) Struktur des Leitfadens

Der Leitfaden ist eine gruppierte Liste von Prüfkriterien gemäß dem oben genannten Kapitel. Jedes Listenelement enthält die folgenden Attribute:

- Eindeutige ID
- Anforderungen/Prüfkriterien, die einfach als erfüllt oder nicht erfüllt bewertet werden können
- Kommentare
- Regulatorischee Verweise
- Verweis auf die ID des [Fragebogens des Team-NB](https://www.team-nb.org/wp-content/uploads/2024/11/Team-NB-PositionPaper-AI-in-MD-Questionnaire-V1-20241125.pdf) (der auf diesem Leitfaden basiert)

Die Kommentare können Folgendes enthalten:

- Beispiele
- Empfehlungen zur Umsetzung von Verweisen auf zusätzliche Erläuterungen
- Hinweise für Auditoren, wie die Erfüllung der Kriterien bewertet werden kann

### 4. Autoren und Nutzungsrechte

Die folgenden Autoren haben diesen Leitfaden erstellt:

- Prof. Dr. Christian Johner ([Johner Institute](https://www.johner-institut.de)) (Version 2019 und folgende)
- [Christoph Molnar](https://christophm.github.io/) ([LMU München](https://www.uni-muenchen.de/index.html)) (Version 2019)
- Dr. Andreas Purde, Dr. Abtin Rad ([TÜV SÜD](https://www.tuev-sued.de/)) (Version 2019)
- Prof. Dr. Dr. Christian Dierks ([Dierks + Company](https://www.dierks.company/)) (Version 2019)
- Stefan Bunk (CTO) und Sven Piechottka (Government & Regulatory Affairs) ([Merantix](https://www.merantix.com/healthcare/)) (Version 2019)

Der Leitfaden wird unter der ([Creative Commons License](https://creativecommons.org/licenses/?lang=de)) vom Typ [BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/) veröffentlicht. Dies erfordert eine Namensnennung der Autoren („Christian Johner, Christoph Molnar et al.“) und erlaubt es Dritten, auf dieser Arbeit aufzubauen, z. B. um sie zu korrigieren; allerdings nur für nicht-kommerzielle Zwecke.

Die Lizenz erlaubt die Nutzung des Produkts für kommerzielle Beratungszwecke einschließlich Audits und Reviews. Es ist jedoch verboten, dieses Werk selbst in unveränderter oder veränderter Form für kommerzielle Zwecke zu nutzen, z. B. in Form eines Verkaufs als Broschüre.

### 5. Dokumentenverwaltung, Dokumentenidentifikation

Dieses Dokument wird über das Versionsverwaltungssystem git oder die GitHub-Plattform verwaltet. Nur die in diesem Repository aufgeführten Dokumente sind gültig.

Die Versionshistorie inklusive eventueller Autoren ist in der Dokumenthistorie zu finden.

Die freigegebenen Versionen befinden sich auf dem Hauptzweig. Entwurfsversionen befinden sich in anderen Zweigen.

## B) Allgemeine Anforderungen

### 1. Prozessanforderungen

Die Hersteller sollten alle unten aufgeführten Aspekte entweder in den Standardarbeitsanweisungen oder in den entsprechenden Plänen abdecken, um sicherzustellen, dass die Sicherheit des Produkts systematisch gewährleistet ist. In der Regel sind die folgenden Standardarbeitsanweisungen oder Pläne betroffen:

- Entwicklung
- Risikomanagement
- Datenverwaltung
- Verifizierung und Validierung einschließlich Testen von KI-Modellen (falls nicht Teil der Entwicklung)
- Kennzeichnung / Labeling
- Sammlung und Analyse von „automatisch erzeugten Protokollen“ gemäß Artikel 19 der Verordnung (EU) 2024/1689
- Überwachung und Beobachtung nach dem Inverkehrbringen
- Service, Installation, Außerbetriebnahme
- Kundenkommunikation
- Managementbewertung (ISO 13485:2021 verlangt die Berücksichtigung „anwendbarer neuer oder überarbeiteter regulatorischer Anforderungen“.)
- Datenschutz
- Identifizierung anwendbarer regulatorischer Anforderungen (Verordnungen, Richtlinien, Gesetze, gemeinsame Spezifikationen, harmonisierte Normen)

Wenn der Hersteller Prozesse auslagert, gelten die Anforderungen entsprechend. Beispiele wären ein (Software-)Entwicklungsdienstleister oder eine Auftragsforschungsorganisation verpflichtet, die relevanten Kapitel dieses Leitfadens zu berücksichtigen.

### 2. Pläne

Der Hersteller sollte alle produktspezifischen Pläne gemäß den jeweiligen Vorschriften zusammenstellen.

- Entwicklungsplan (einschließlich Verifizierungs- und Validierungsplanung)
- Plan zur Überwachung nach dem Inverkehrbringen (s. 2017/745/EU Anhang 1II, 2017/745/EU Anhang IIII, 2024/1689 Artikel 72 Abschnitt 3.)
- Risikomanagementplan
- Plan für die klinische Bewertung

### 3. Kompetenzanforderungen

Die Hersteller müssen sicherstellen und nachweisen, dass sie über ausreichende Kompetenzen verfügen, um die relevante Sicherheit und Leistung der Produkte gemäß dem Stand der Technik zu gewährleisten. Dieser Nachweis wird oft am einfachsten durch interne oder externe Schulungen erbracht.

Hersteller können die Kompetenz externer Ressourcen nutzen.

|ID|Anforderungen|Kommentare|Regulatorische Referenzen|Team-NB-ID|
|:--|:--|:--|---|:--|
|3.1|Der Hersteller hat eine Liste aller Rollen innerhalb des Geltungsbereichs seines QM-Systems erstellt, die direkt oder indirekt mit KI zu tun haben.|Beispiele [^B2-01]|ISO 13485 5.5.1 und 6.2., ISO 14971 3.3., IEC 62304 5.1, 2017/745/EU Artikel 10.9, 21 CFR Teil 820.30 (b) | 5.1.1. |
|3.2|Der Hersteller hat die Kompetenzanforderungen für jede Rolle innerhalb des Geltungsbereichs seines QM-Systems, die direkt oder indirekt mit KI zu tun hat, ermittelt und dokumentiert. [^B2-02]|Kompetenzen beziehen sich auf Bildung, Wissen oder Fähigkeiten. Beispiele für Kompetenzen: Maschinelles Lernen, erklärbare KI, Medizin (für relevante Bereiche), klinische und Usability-Validierung.| ISO 13485 6.2., ISO 14971:2019 4.3, ISO 13 485:2016 7.3.2, IEC 82304-1 6.1, 2024/1689/EU Artikel 4 und 9 Abschnitt 5. | 5.1.2. |
|3.3|Der Hersteller verfügt über geeignete Aufzeichnungen über die Schulung, Weiterbildung und Kompetenzen, die den Schluss zulassen, dass die Personen tatsächlich über diese Kompetenzen verfügen.|| ISO 13485 6.2., ISO 14971 4.3 | 5.1.3 |
|3.4|Die (Software-)Entwicklungspläne haben die produktspezifischen Kompetenzen (darüber hinausgehend oder abweichend) definiert.|| ISO 13485 7.3.2., IEC 82304-1 6.1. | 5.1.4 |
|3.5 |Diese Kompetenzanforderungen werden auch für externe Ressourcen (Auftragnehmer, ausgelagerte Prozesse) erfüllt |||5.1.5|

[^B2-01]: Beispiele sind: Datenwissenschaftler, Entwickler, Tester, Manager für regulatorische Angelegenheiten und Qualität, Service- und Supportmitarbeiter, Produktmanager, Berater für Medizinprodukte, Ärzte

[^B2-02]: Kompetenzstufen wie das Verständnis der Fähigkeit, Aufgaben auszuführen, sollten aufgeführt werden, nicht nur Themen

### 4. Dokumentation

Die Hersteller sollten Nachweise darüber aufbewahren, dass sie die relevanten Anforderungen dieses Leitfadens befolgt haben. Es gibt keine KI-spezifischen Anforderungen für die Dokumentation und den „objektiven Nachweis“.

Zumindest in Europa besteht keine Verpflichtung, ein spezifisches Dokument zu erstellen, das die Aktivitäten speziell für KI zusammenfasst. Hersteller können diese Aspekte in bestehende Dokumente wie QM-Dokumente (z. B. SOPs, Arbeitsanweisungen) und die technische Dokumentation (z. B. Software-Akte, Risikomanagementakte, klinische Bewertung, summative Bewertung der Gebrauchstauglichkeit) integrieren.

Die Verordnung 2024/1689/EU empfiehlt, die KI-spezifische Dokumentation in eine bestehende technische Dokumentation zu integrieren. Sie schreibt vor, dass die Dokumentation zehn Jahre lang aufbewahrt werden muss, nachdem das KI-System auf den Markt gebracht wurde (Artikel 18.1).

## C) Anforderungen an die Produktentwicklung

### 1. Verwendungszweck und Stakeholder-Anforderungen

#### a) Beabsichtigter medizinischer Verwendungszweck

|ID|Anforderungen|Kommentare|Regulatorische Referenzen|Team-NB-ID |
|:--|:--|:--|---|:--|
|C1a1|Der Hersteller hat festgelegt, für welchen medizinischen Zweck (Diagnose, Therapie, Überwachung, Vorhersagen) das Medizinprodukt eingesetzt werden soll.|Der Verwendungszweck/Zweck sollte nicht mit der Beschreibung der Funktionalität (z. B. Berechnung von Scores) verwechselt werden.| ISO 13485, 4.2.3. und 7.3.2. c., 2017/745/ EU Anhang II (1.1), 2924/1689/EG Anhang IV Abschnitt 1.(a), ISO 14971:2019, 5.2, 21 CFR 814.20 (b)(3)(i), 21 CFR Teil 820.30(c) | 6.1.1.1. |
|C1a2|Der Hersteller hat die Patienten charakterisiert, die mit dem Medizinprodukt diagnostiziert, behandelt oder überwacht werden sollen. Diese Charakterisierung umfasst die demografischen Daten der Patienten, Indikationen, Kontraindikationen und assoziierte Krankheiten.|Diese Charakterisierung ist auch in IEC 62366-1 enthalten. Patienten können gleichzeitig auch Anwender des Produkts sein. | 2017/745/EU, Anhang I, 23.4 und Anhang II, 1.1. c, 2017/746/EU, Anhang II, 1.1. c, IEC 62366-1, 5.1. und 5.3., ISO 13485, 7.3.3 a., 21 CFR 814.20 (b)(3)(i) |6.1.1.2|
|C1a3|Der Hersteller hat angegeben, ob es Patienten unter 18 Jahren oder andere vulnerable Gruppen gibt,||2024/1689/EG Artikel 9 Abschnitt 10.||
|C1a4|Der Hersteller hat angegeben, an welchen Körperstellen das Produkt verwendet wird oder von welchen Körperstellen die Daten stammen.|Auch gefordert in IEC 62366-1, Abschnitt 5.1.| 201 7/745/EU, Anhang II, 1.1., 2017/746/EU, Anhang II, 1.1., IEC 62366-1, 5.1.3. | 6.1.1.3 |
|C1a5|Der beabsichtigte Verwendungszweck lässt erkennen, was das Ziel der/des Verfahrens  des maschinellen Lernens ist.|Klassifizierung und Regression, Clustering, Ähnlichkeitssuche und Empfehlungssysteme sind typische Ziele von maschinellen Lernmethoden. Die Beschreibung der Rolle des maschinellen Lernens ist notwendig, um die Anforderung der Beschreibung des „physikalischen Prinzips“ zu erfüllen. | IEC 62366-1, 5.1, 2017/745/EU Anhang II, 1.1, 21 CFR Teil 814.20, XAVIER University „Building Explainability and Trust for AI in Healthcare“ | 6.1.1.5 |
|C1a6|Falls zutreffend, hat der Hersteller beschrieben, ob das Produkt Messfunktionen enthält.|Diese Eingabe wird z. B. benötigt, um die Risikoklasse des Produkts korrekt zu bestimmen.||6.1.1.4|
|C1a7|Der Hersteller hat die vorgesehene Lebensdauer des Medizinprodukts bzw. IVD festgelegt.|Diese Lebensdauer wird beispielsweise durch den Stand der Technik (z. B. medizinische Fortschritte, neue ML-Methoden, Wettbewerbsprodukte) und die Geschwindigkeit, mit der sich die technische Umgebung und die Bibliotheken weiterentwickeln, bestimmt.|||


#### b) Vorgesehene Anwender und Nutzungskontext

| ID | Anforderungen | Kommentare |Regulatorische Referenzen|Team-NB-ID|
| :----------------------------------------------------------- | :----------------------------------------------------------- |:--|---|:--|
| C1b1 | Der Hersteller hat die vorgesehenen Anwender / Nutzer charakterisiert, z. B. anhand demografischer Merkmale (Alter, Geschlecht), in Bezug auf die Ausbildung, Erfahrung in medizinischen Bereichen, in Bezug auf technisches Wissen, körperliche und geistige Einschränkungen, Sprachkenntnisse und kulturellen Hintergrund. | Wenn der Hersteller keine Einschränkungen in Bezug auf diese Attribute vorsieht, muss er dies dokumentieren. | 2017/745/EU, Anhang I, 5 und Anhang II, 1.1, IEC 62366-1, 5.1., XAVIER University „Building Explainability and Trust for AI in Healthcare“| 6.1.2.1 |
|C1b2|Der Hersteller hat angegeben, ob das Produkt für die Nutzung durch Laien vorgesehen ist.|Diese Entscheidung hat regulatorische Auswirkungen, wie z. B. die Anwendbarkeit der Anforderungen der Verordnungen 2017/745/EU und 2017/746/EU in Anhang I und 2024/1689/EU.|2017/745/EU Anhang I Abschnitt 22 und 2017/746/EU Anhang I Abschnitt 19|6.1.2.3|
| C1b3 | Der Hersteller hat die vorgesehene Nutzungsumgebung (auch das soziale Umfeld wie Stress, Schichtarbeit, häufig wechselnde Kollegen) charakterisiert. | Diese Charakterisierung ist auch in IEC 62366-1 vorgeschrieben. Sie ist auch im Zusammenhang mit der Erklärbarkeit von KI relevant, da KI die Nutzungsumgebung, z. B. Aufgaben und Arbeitsbelastung, verändern kann. | 2017/745/EU, Anhang I, 5, IEC 62366-1, 5, XAVIER University „Building Explainability and Trust for AI in Healthcare“, UK 811.4 Positionspapier | 6.1.2.2 |
|C1b4| Der Hersteller hat die Kernaufgaben beschrieben, die das Medizinprodukt unterstützen soll. | Aus diesen Kernaufgaben lassen sich auch die Anwendungsszenarien ableiten, die Hersteller gemäß IEC 62366-1 spezifizieren müssen.| IEC 62366-1 | |

#### c) Stakeholder-Anforderungen

| ID | Anforderungen | Kommentare |Regulatorische Referenzen|Team-NB-ID|
| :----------------------------------------------------------- | :----------------------------------------------------------- |:--|---|:--|
| C1c1 | Der Hersteller hat die in der Zweckbestimmung aufgeführten Ziele mit quantitativen Werten operationalisiert [^C.1.c.1]. | Es ist nicht ungewöhnlich, dass diese Werte im Laufe der Entwicklung ergänzt und überarbeitet werden. | 2017/745/EU, Anhang I, 23.4 und Anhang III, 1.1, FDA SW validation guidance 5.2.2, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. „Software Requirements Specification“)| |
| C1c2 | Der Hersteller hat die Laufzeitumgebung des Produkts in Bezug auf Hardware (Bildschirmgröße, Bildschirmauflösung, Speicher, Netzwerkverbindung usw.) und Software (z. B. Betriebssystem, Browser, Laufzeitumgebungen wie Java-Laufzeitumgebung oder .NET) festgelegt. | Bei einigen mobilen Apps muss diese Charakterisierung für die App und für den Serverteil erfolgen. | 2024/1689/EU Anhang IV Abschnitt 1.(b), ISO 13485, 7.3.3, 2017/745/EU, Anhang I, 17.3 und 17.4, IEC 6 2304, 5.2, XAVIER University „Building Explainability and Trust for AI in Healthcare“, FDA SW validation guidance 5.2.2, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. „Software Requirements Specification“)| |
| C1c3 | Der Hersteller hat die Datenschnittstellen anhand der Ebenen des [Interoperabilitätsmodells](https://www.johner-institut.de/blog/tag/interoperabilitat/) spezifiziert und die Formate sowie für Bilder deren spezifische Eigenschaften (Größe, Auflösung, Farbcodierung) festgelegt. | Dies ist gemäß IEC 62304 Kapitel 5.2.2 erforderlich. | 2024/1689/EU Anhang IV Abschnitt 1.(b), IEC 62304, 5.2.2, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. „Software Requirements Specification“) | 6.2.3.1. |
|C1c4 |Der Hersteller hat die Anforderungen an die Eingabedaten festgelegt. | Die Eingabedaten können auch von der Datenerzeugung abhängen, z. B. von der Aufzeichnungsmethode, von technischen Parametern (magnetische Feldstärken, Anzahl der leitfähigen Elektroden, Richtung), von den Umgebungsbedingungen während der Aufzeichnungen, vom Hersteller, vom Medizinprodukt usw. | IEC 62304, 5.2, ISO 14971:2019, 5.3, FDA-Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. „Software Requirements Specification“) | 6.2.3.2. |
| C1c5 | Der Hersteller hat alle Märkte festgelegt und die Liste der dort geltenden regulatorischen Anforderungen sowie das Verfahren zur Ermittlung dieser Anforderungen dokumentiert. | Zu den regulatorischen Anforderungen gehören Verordnungen, Richtlinien, Gesetze, gemeinsame Spezifikationen und harmonisierte Normen. Auditoren sollten sich diese Liste zeigen lassen. | 2017/745/EU, Anhang IX, 2.2, ISO 13485, 5.2 und 7.2.1, EN ISO 13485 4.1.1, 2024/1689/EU Artikel 17 Abschnitt 1.(e), 41 Abschnitt 5. und Anhang IV 7. | 6.1.3.2 |
| C1c6 | Der Hersteller hat angegeben, ob das System nach dem Inverkehrbringen weiter lernen soll. |Wenn dies der Fall ist, hat der Hersteller angegeben, ob dieses kontinuierliche Training global/zentralisiert oder dezentralisiert (z. B. pro Produkt oder pro Krankenhaus) und online oder offline erfolgen soll.|||

[^C.1.c.1]: **Beispiel**: Zweck: Die Software unterstützt Radiologen bei der Diagnose von Krebserkrankungen anhand von CT-Bildern des Kopfes. Quantitativer Wert: 95 % der Radiologen, die mit der Software arbeiten, erkennen den Krebs.


#### d) Input für Risikomanagement und klinische Bewertung

| ID | Anforderungen | Kommentare | Regulatorische Referenzen| Team-NB-ID |
| :------------------------------------------------------------ | :------------------------------------------------------------ |:--|---|:--|
| C1d1 | Der Hersteller hat alternative Verfahren aufgelistet und sie im Hinblick auf Nutzen, Sicherheit und Leistung bewertet. | Die Erörterung des Stands der Technik ist eine Anforderung von MEDDEV 2.7/1 und der MDR/IVDR. | 2017/745/EU, Anhang I, 1., 2017/746/EU, Anhang I, 1., MEDDEV 2.7/1, ISO 14971:2 019, 4.2 und 10.9, FDA Guidance „Factors to Consider When Making Benefit-Risk Determinations in Medical Device Premarket Approval“ (z. B. Teil C) | 6.1.5.1 |
| C1d2 | Der Hersteller hat die oben genannten quantitativen Werte mit den relevanten Werten alternativer Methoden verglichen. | Die Hersteller sollten eine tabellarische Übersicht erstellen. ||(6.4.4.9.)|
| C1d3 | Der Hersteller hat begründet, warum maschinelles Lernen den anderen Methoden überlegen ist und damit die damit verbundenen Risiken gerechtfertigt. | | 2017/745/EU, Anhang I, 1., 2017/746/EU, Anhang I, 1., MEDDEV 2.7/1 | (6.1.4.2) |
| C1d4 | Der Hersteller hat eine Liste der Risiken erstellt, die sich speziell aus der Anwendung von Methoden des maschinellen Lernens ergeben. | Z. B. können selbstlernende Systeme und LLMs trotz unveränderter Eingabedaten eine unterschiedliche Ausgabe liefern. | ISO 14971, 5.4. und 5.5., 2017/745/EU, Anhang I, 3., DIN SPECT 2, ISO/TR 31004:2013 - Risikomanagement - Anleitung zur Umsetzung von ISO 31000, UK 811.4 Positionspapier | (6.1.2.5), 6.1.4.3 |
| C1d5 | Der Hersteller hat die Risiken analysiert, die entstehen, wenn andere Personen als die vorgesehenen Benutzer das Produkt verwenden. | | ISO 14971, 5. | 6.1.4.5 |
| C1d6 | Der Hersteller hat die Risiken analysiert, die durch eine Änderung der Nutzungsumgebung beim Einsatz eines KI-basierten Systems entstehen. |Z. B. können diese Systeme Aufgaben ändern, hinzufügen oder eliminieren oder die Arbeitsbelastung erhöhen. Ein weiteres Beispiel ist die Arbeit aus der Ferne statt in einem Krankenhaus. |UK 811.4 Positionspapier||
| C1d7 | Der Hersteller hat die Risiken analysiert, die sich aus der Nutzung in einer anderen als der angegebenen Umgebung ergeben. | z.B. wird das Produkt unerwartet im Home-Office verwendet. | 2017/745/EU, Anhang I, 14.2.(d), 2017/746/EU, Anhang I, 13.2.(d), ISO 14971, 5., IEC 82304-1, 4.1. (b) | 6.1.4.9 |
| C1d8 | Der Hersteller hat die Risiken analysiert, die sich aus Eingaben ergeben, die nicht den festgelegten Voraussetzungen (z. B. Qualität, Wertebereich, Format und Einheit) entsprechen. | | ISO 14971, 5., IEC 82304-1, 4.1. (c) | 6.1.4.6 |
| C1d9 | Hersteller haben Risiken analysiert, die sich aus Daten ergeben, die nicht gemäß den festgelegten Voraussetzungen generiert wurden. | Beispiele: neuer CT-Scannertyp, MRT mit neuen Sequenzen ||(6.1.4.11)|
| C1d10 | Der Hersteller hat die Risiken bewertet, die entstehen, wenn das System für andere als die spezifizierten Patienten oder Patientengruppen verwendet wird. | Dies könnte Teil eines vorhersehbaren Missbrauchs sein. | ISO 14971, 4.2., 4.3., 5., IEC 82304-1, 4.1., 2024/1689/EU Artikel 9 Abschnitt 2.(b) | 6.1.2.6, 6.1.4.8 |
| C1d11 | Der Hersteller hat das Risiko für die Grundrechte analysiert. |Beispiele sind das Recht auf informationelle Selbstbestimmung (Datenschutz) und das Recht auf Zugang zu angemessener Gesundheitsversorgung.|2024/1689/EU Artikel 9 Abschnitt 2.(a)||


### 2. Softwareanforderungen

#### a) Funktionalität und Leistung

|ID|Anforderungen|Kommentare|Verweis auf Vorschriften|Team-NB-ID|
|:--|:--|:--|---|:--|
|C2a1|Der Hersteller hat quantitative Qualitätskriterien oder Anforderungen für die Software oder/und den Algorithmus aus der Zweckbestimmung und den Stakeholder-Anforderungen nachvollziehbar abgeleitet [^C.2.a.1].|Diese Nachvollziehbarkeit lässt sich besonders gut mit einer "Traceabiliy-Matrix" darstellen.| 2024/1689/EU Anhang IV, ISO 13485, 7.3.3., IEC 62304, 5.2, XAVIER University „Building Explainability and Trust for AI in Healthcare“, FDA Guidance zur „Software-Validierung“, Kapitel 5.2.2 | (6.1.3.1.), 6.2.1.1. |
|C2a2|Der Hersteller berücksichtigte beispielsweise die folgenden quantitativen Qualitätskriterien oder -anforderungen: bei Klassifizierungsproblemen Genauigkeit (mittlere oder ausgewogene Genauigkeit), positiver Vorhersagewert (Präzision), Spezifität und Sensitivität; bei Regressionsproblemen mittlerer absoluter Fehler und mittlerer quadratischer Fehler.| Bei unausgewogenen Daten, d. h. wenn Labels mit sehr unterschiedlichen Häufigkeiten auftreten, sollte anstelle der mittleren Genauigkeit eine ausgewogene Genauigkeit verwendet werden. Die Wahl der Qualitätskriterien hängt jedoch stark von der Zweckbestimmung ab. | ISO 13485, 7.3.3., 7.3.4., IEC 62304, 5.2. | 6.2.1.2. |
| C2a3 | Der Hersteller hat die erwarteten Wertebereiche der Ausgaben (Outputs) angegeben. | | ISO 13485, 7.3.3., 7.3.4., IEC 62304, 5.2. | 6.2.1.4. |
|C2a4|Der Hersteller hat die Anforderungen bezüglich der Wiederholbarkeit und Reproduzierbarkeit der Anforderungen festgelegt.|Dies ist besonders relevant bei „Continuous Learning Systems“ (kontinuierlichen Lernsystemen).| 2017/745/EU, Anhang I, 17.1. , 2017/746/EU, Anhang I, 16.1., ISO 13485, 7.3.3., 7.3.4 | 6.2.1.5. |
|C2a5|Der Hersteller hat angegeben, wie sich das System verhält, wenn die Eingaben nicht den festgelegten Anforderungen entsprechen [^C.2.a.2].|Dies ist ein Aspekt der Robustheit, der gemäß ISO 25010 und IEC 62304 Kapitel 5.2 festgelegt werden muss. | ISO 25010,, IEC 62304, 5.2., ISO 14971:2019, 5.4, FDA Guidance zur „Software-Validierung“, Kapitel 5.2.2, FDA-Kriterien für "digital health" | 6.2.1.6. |
|C2a6|Der Hersteller hat festgelegt, welche Selbsttests das System durchführen muss und wie es sich verhält, wenn diese nicht erfolgreich sind.|Dies ist besonders relevant für „Continuous Learning Systems“ (kontinuierlich lernende Systeme).| ISO 13485, 7.3.3. | (6.2.1.7.) |
|C2a7|Der Hersteller hat festgelegt, wie schnell das System die Ausgaben erstellen muss.|Diese Festlegung kann in Abhängigkeit von der Größe und der Datenmenge erfolgen.| 2017/745/EU, Anhang I, 17.1., 2017/746/EU, Anhang I, 16.1., ISO 13485, 7.3.3. | 6.2.1.8. |
|C2a8|Der Hersteller hat die Verfügbarkeit des Medizinprodukts angegeben.|Dies ist ein Aspekt der Robustheit und muss gemäß ISO 25010 und IEC 62304 Kapitel 5.2 angegeben werden. | ISO 25010, IEC 62304, 5.2., ISO 14971, 4.3., ISO 13485, 7.3.3. | 6.2.1.9. |
|C2a9 |Der Hersteller hat die Anforderungen in Bezug auf "Audit Logs" festgelegt. |AI Act spricht von „Protokollen“.|2024/1689/EU Artikel 12||

[^C.2.a.1]: Beispiele: **Beispiel 1**: Die Stakeholder-Anforderung (Nutzungsanforderng) besagt, dass 95 % der Radiologen in der Lage sein müssen, mit dem Produkt Krebs zu erkennen. Die Anforderung an den Algorithmus besagt, dass er eine Sensitivität von 97 % aufweisen muss. **Beispiel 2**: Die Anforderungen der Stakeholder besagen, dass eine Arterienverkalkung mit einer Sensitivität von 92 % erkannt werden können muss. Die Anforderungen an den Algorithmus besagen, dass er die Stärke der Plaques im Blut auf 0,2 mm genau vorhersagen können muss.

[^C.2.a.2]: Beispiele: unvollständige Datensätze, fehlende Datensätze, falsches Datenformat, übermäßige Datenmengen, Daten außerhalb der spezifizierten Wertebereiche, falsche zeitliche Abfolge der Daten.

#### b) Benutzerschnittstelle

| ID | Anforderungen | Kommentare | Regulatorische Referenzen| Team-NB-ID |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :--| ---| :--|
|C2b1 |Der Hersteller hat die Benutzerschnittstelle (Anforderungen) spezifiziert. |IEC TR 62366-2 enthält Beispiele.| 2024/1689/EU Anhang IV Abschnitt 1.(g), IEC 62304 5.2.2 f), IEC 62366-1 5.6 | |
| C2b2 | Der Hersteller hat festgelegt, was die Benutzerschnittstelle anzeigen muss, wenn die Voraussetzungen nicht erfüllt sind [^C.2.a.2] oder wenn interne Fehler vorliegen, um das System sicher zu betreiben (z. B. ungültige oder nicht erwartete Eingaben). | AI Act erfordert eine „menschliche Aufsicht“, die selbst zu Produkt-/UI-Anforderungen wie der Überwachung von Informationen, der Warnung vor Anomalien und Fehlfunktionen sowie einem Notausschalter führen kann. | 2017/745/EU, Anhang I, 5., 2017/746/EU, Anhang 1, 5., 2024/1689/EU Artikel 14 Abschnitt 4., IEC 62366-1, 5.2., FDA HFE-Leitfaden, FDA Guidance zur Softwarevalidierung, z. B. Kapitel 5.2.3 | 6.2.2.1. |
| C2b3 | Der Hersteller hat festgelegt, was auf der Benutzeroberfläche angezeigt werden muss, wenn die Ausgabe nicht den festgelegten Qualitätskriterien entspricht. | | | 6.2.2.2. |
|C2b4|Der Hersteller hat die Informationen angegeben, die die Benutzeroberfläche bereitstellen muss, um die Systemausgabe (Ergebnisse) zu erklären. | Alternativ muss eine Begründung dafür gegeben werden, dass keine „Erklärbarkeit“ erforderlich ist. Ziel dieser Informationen ist es, Risiken zu reduzieren und die „menschliche Aufsicht“ zu ermöglichen. | 2024/1689/EU Artikel 14 Abschnitt 4.(c) ||
| C2b5 | Der Hersteller hat festgelegt, ob Gebrauchsanweisungen und Schulungsmaterialien erforderlich sind. | Die MDR/IVDR lassen Ausnahmen von dieser Verpflichtung zu. | 2017/745/EU, Anhang I, 23., 2017/746/EU, Anhang I, 20., ISO 13485, 4.2.3., FD&C, 21 CFR Teile 801 und 820.120| 6.2.2.3. |


#### c) Zusätzliche Softwareanforderungen

| ID | Anforderungen | Kommentare | Verweise auf Vorschriften| Team-NB-ID |
| :----------------------------------------------------------- | :------------------------------------------ |:--|---|:--|
| C2c1 | Der Hersteller hat festgelegt, welche Anforderungen das System erfüllen muss, um interne Systemfehler zu erkennen. | Dies kann ein "Audit Log2" oder ein Überwachungsschnittstelle (Port) sein. | 2017/745/EU, Anhang I, 17, 18, 23.4, IEC 62304, 5.2, 5.3 und 7.1, ISO 149781:2019 , 5.4, FDA Guidance zur Softwarevalidierung, z. B. Kapitel 5.2.2, 5.2.3 und 5.2.4, GMLP-Leitprinzipien (von der FDA et al.) #2 (Datenintegrität) | 6.2.3.3. |
| C2c2 | Gemäß der DSGVO darf das spezifizierte System Patienten keinen Entscheidungen aussetzen, die ausschließlich auf automatischer Datenverarbeitung basieren. Hersteller sollten die entsprechende Anforderung erfüllen und in der Lage sein, die gewählte Rechtsgrundlage zu begründen. |  | Art. 22 der DSGVO. | |
| C2c3 | Der Hersteller hat die Anforderungen festgelegt, die die Software erfüllen muss, um die IT-Sicherheit des Produkts zu gewährleisten. | IT-Sicherheit ist nicht Gegenstand dieser Richtlinie, sondern der [Leitfaden zur IT-Sicherheit](https://github.com/johner-institut/it-security-guideline/). | 2024/1689/EU Artikel 15 Absatz 5. | 6.2.4.x |



#### d) Besondere Anforderungen an "Continuous Learning Systems"

| ID | Anforderungen | Kommentare | Verweise auf Vorschriften | Team-NB-ID |
| :----------------------------------------------------------- | :----------------------------------------------------------- |:--|:--|---|
| C2d1 | Der Hersteller hat definiert, wann und wie oft das Modell aktualisiert wird. | Zu diesem Zweck sollte der Hersteller die „Auslöser“ dieser Aktualisierungen definieren. Er muss auch beschreiben, ob diese Aktualisierungen für jedes einzelne Medizinprodukt oder für alle Medizinprodukte des Typs erfolgen. | | |
| C2d2 | Der Hersteller hat angegeben, wie die Qualität der zusätzlichen Daten sichergestellt wird und wie mit falschen, fehlenden oder unplausiblen Daten umgegangen wird. ||||
| C2d3 | Der Hersteller hat definiert, in welchem Bereich sich die Ausgabedaten ändern dürfen. | Dies erfordert eine Beschreibung, wie sich die Algorithmen ändern. |||
| C2d4 | Der Hersteller hat beschrieben, wie er weiterhin die Korrektheit und Genauigkeit der Ausgabedaten sicherstellt und was passiert, wenn dies nicht mehr gewährleistet werden kann. | Selbstkontrollen, die Möglichkeit von Rollbacks, die Begrenzung von Ausgaben sind mögliche Ansätze. |||
|C2d5 |Der Hersteller hat beschrieben, ob und wie Nutzer über Änderungen am Algorithmus informiert werden und ob sie darüber entscheiden können. | |||
|C2d6 |Der Hersteller hat die spezifischen Risiken, die sich aus dem kontinuierlichen Lernen ergeben, identifiziert und gemanagt. | Zu diesem Zweck muss der Hersteller begründen, dass er durch kontinuierliches Lernen ein besseres Risiko-Nutzen-Verhältnis erreicht. |||

[^C.2.d.1]: Der Stand der Technik entspricht nicht unbedingt dem Stand der Wissenschaft und damit dem Goldstandard oder der „Ground Truth“. Dies bedeutet, dass die Systemanforderungen niedriger sind als bei einem Goldstandard bzw. der „Ground Truth“. Dies wäre insbesondere dann der Fall, wenn letztere ein invasives oder sehr kostenintensives Verfahren erfordern.

### 3. Datenmanagement

Daten sind generell als Trainings-, Validierungs- und Testdaten sowie Label zu verstehen. Jeder Typ muss spezifische Anforderungen erfüllen. Wenn nicht anders angegeben, bezieht sich die Verwendung des Begriffs „Daten“ im Folgenden jedoch auf alle Typen.

#### a) Datenerhebung

| ID | Anforderungen | Kommentare | Regulatorische Referenzen| Team-NB-ID [^6.3.a.7]|
| :------------------------------------------------------------| :------------------------------------------------------------|:--|---|:--|
|C3a1|Der Hersteller hat ein Verfahren definiert, das das Datenmanagement einschließlich Datenerhebung, Datenverarbeitung und Datenanalyse definiert||2024/1689/EU Artikel 10 Abschnitt 2 und 17 Abschnitt 1.(f), ISO 13485 4.1||
| C3a2 | Der Hersteller hat die Anzahl der Datensätze angegeben und begründet, warum diese ausreichend ist [^C.3.a.1]. | Dies betrifft die Datensätze für Training, Validierung und Test. | ISO 13485, 7.3.7, 2024/1689/EU Artikel 10 Abschnitt 2.(b) und (e) | 6.3.1.9. |
|C3a3 |Der Hersteller hat die Ein- und Ausschlusskriterien von Daten durch relevante Attribute charakterisiert [^C.3.a.2]. | Dies umfasst die Dokumentation von Datentypen, Einheiten und Wertebereichen. | ISO 24028, XAVIER University „Building Explainability and Trust for AI in Healthcare“ | 6.3.1.10. |
|C3a4 |Der Hersteller hat Ein- und Ausschlusskriterien für Daten festgelegt [^C.3.a.3]. ||2024/1689/EU Artikel 10 Abschnitt 2.(f)|6.3.1.11.|
| C3a5 | Der Hersteller hat das Verfahren beschrieben, mit dem er sicherstellt, dass Datensätze, die die Einschlusskriterien nicht erfüllen oder ausgeschlossen werden sollten, tatsächlich ausgeschlossen werden. | Das Verfahren umfasst eine softwaregestützte Bewertung. Diese Software muss validiert werden. |2024/1689/EU Artikel 10 Abschnitt 2.(f)|6.3.1.12.|
| C3a6 | Der Hersteller hat die gesammelten Daten mithilfe deskriptiver Statistiken beschrieben [^C.3.a.4]. | [Der „Dataset Nutrition Label“](https://ahmedhosny.github.io/datanutrition/) ist eine empfohlene Option. | 2024/1689/EU Artikel 10 Abschnitt 2.(f) und Anhang IV Abschnitt 2.(d)| 6.3.1.13., 6.3.4.13. |
| C3a7 | Der Hersteller hat die Herkunft der Daten (z. B. Kliniken, Geräte) beschrieben. | | | 6.3.4.12. |
| C3a8 | Der Hersteller hat begründet, wo die Daten erhoben wurden und warum diese für die Zielpopulation repräsentativ sind. Soweit sinnvoll, wurden diese mit wissenschaftlichen Veröffentlichungen und Registern verglichen. | | 2024/1689/EU Artikel 10 Abschnitt 4 und 5.| 6.3.1.14. |
| C3a9 | Der Hersteller hat Faktoren aufgelistet und erörtert, die zu einer Verzerrung der Daten führen könnten. | | ISO 24028 z. B. 10.5, 2024/1689/EU Artikel 9 Abschnitte 2.(d) und 5.(a), Artikel 10 Abschnitte 2.(f), 2.(g), 4.| 6.3.1.16. |
| C3a10 | Der Hersteller hat analysiert, welche Auswirkungen die Art und der Ort der Datenerhebung auf die Daten haben [^C.3.a.5]. |||6.3.1.17.|
|C3a11 | Der Hersteller hat ein Verfahren festgelegt, um sicherzustellen, dass die Datenschutzanforderungen erfüllt werden. | Beispielsweise werden die Daten vor dem Testen und Training anonymisiert oder pseudonymisiert. Der Datenschutzbeauftragte sollte daran beteiligt werden. |2024/1689/EU Artikel 10 Absatz 5, 2016/679/EU|6.3.1.18.|
| C3a12 | Der Hersteller hat die Möglichkeit eines „Label Leakage“ untersucht und ausgeschlossen. [^C.3.a.6] | Dies hängt vom angewandten ML-Modell ab und ist keine allgemeine "Best Practice". | 6.3.1.19., 6.3.1.20.||
| C3a13 | Der Hersteller, der Umfragen verwendet, hat die Auswahl der Umfragen, den Zeitpunkt der Umfrage und möglicherweise die Methode für ihre Bewertung begründet, insbesondere wenn keine standardisierte Umfrage existiert. | |||

[^C.3.a.1]: Eine Angabe zur Anzahl der Daten ist kaum möglich. Dies hängt unter anderem vom „Signal-Rausch-Verhältnis“ ab. Bei einem Datensatz beispielsweise beeinflussen der Prozentsatz relevanter Gene sowie die Stärke und Häufigkeit der vorhergesagten Effekte die Anzahl. Für die Klassifizierung von Daten ist die Anzahl der Datensätze mit der seltenen Klasse (z. B. die Prävalenz von Krankheiten) entscheidend.

[^C.3.a.2]: z. B. demographische Daten (Alter, Geschlecht), physikalische Parameter (Größe, Gewicht), Krankheiten, Vitalparameter, Laborparameter, Vorhandensein zusätzlicher Tests, Krankengeschichte.

[^C.3.a.3]: Beispiele: **Beispiel 1**: Patienten, bei denen aufgrund eines Herzschrittmachers oder einer Lungenoperation ausgeschlossen werden muss, weil die Bilder nicht analysiert werden können oder zu einer fehlerhaften Klassifizierung führen könnten. **Beispiel 2**: Formate und technische Parameter wie Bildgröße, Auflösung, Helligkeit und Kontrast, Farbcodierung, Kompression, Aufnahmegerät, Aufnahmemethode (z. B. CT versus MRT), mit oder ohne Kontrastmittel, Zoom. **Beispiel 3**: Vollständigkeit der Metadaten.

[^C.3.a.4]: In der Regel die Berechnung von Verteilungen (Histogramme), Mittel-/Durchschnittswerten, Quartilen, möglicherweise „joint distribution of features“. Die Korrelation von Daten innerhalb dieser Daten sollte untersucht werden. Weitere Beispiele finden sich in der [Publikation von Sarah Holland et al.](https://arxiv.org/pdf/1805.03677.pdf) (z. B. in Tabelle 1)

[^C.3.a.5]: Beispiele: Einfluss verschiedener Messgeräte, Erhebungen, interne Richtlinien (z. B. nimmt eine Klinik nur in Notfällen Laborparameter, eine andere routinemäßig. Häufigkeit und Grund werden mit dem Patienten untersucht), Art der Klinik (z. B. kleines Krankenhaus, an das alle schweren Fälle überwiesen werden müssen, im Gegensatz zu einer Universitätsklinik > survivor bias, self-selection bias (z. B. Patienten mit verschiedenen Vorerkrankungen gehen in der Regel eher in ein Krankenhaus als in eine Arztpraxis), Art der Studie (prospektiv vs. retrospektiv)

[^C.3.a.6]: Dies sind Daten, in denen nicht-kausale Informationen in den Daten über die Bezeichnung gefunden werden, z. B. in der Sortierung (z. B. zuerst die Daten von gesunden Personen, dann von kranken Personen), im Krankenhaus (von einem stammen die schweren Fälle), in Bildern (z. B. bei Hautkrebs muss immer ein Lineal zu sehen sein). Ein weiteres Beispiel wären mehrere CT-Bilder eines Patienten, bei denen das Modell anhand des Patienten und nicht anhand der Krankheit lernt. Dies könnte der Fall sein, wenn auf mehreren Bildern zusätzlich zum Krebs ein Rippenbruch zu sehen ist.

[^C.3.a.7]: Das Team-NB-Dokument beginnt die Nummerierung dieses Abschnitts mit 9 statt mit 1. D. h. es gibt keine Punkte 6.3.1.1. bis 6.3.1.8.

#### b) Data Labeling

| ID | Anforderungen | Kommentare | Verweise auf Vorschriften| Team-NB-ID |
| :------------------------------------------------------------| :------------------------------------------------------------|:--|---|:--|
| C3b1 | Im Fall von „Supervised Learning“ hat der Hersteller die Labels aus derZweckbestimmung abgeleitet, in der die Trainingsdaten bereitgestellt werden, und diese Wahl begründet. | |2024/1689/EU Artikel 10 Abschnitt 3|6.3.2.1.|
| C3b2 | Der Hersteller hat ein Verfahren zum Labeling bei „überwachten Lernen“ definiert, falls die Daten noch keine Labels enthalten. | | ISO 13485, 4.1, 2024/1689/EU Artikel 10 Abschnitt 2.(c) | 6.3.2.2. |
| C3b3 | Dieses Verfahren legt quantitative Klassifizierungskriterien für das Labeling fest. Die Auswahl dieser Kriterien wurde vom Hersteller begründet [^C.3.b.1]. | Wenn die „Ground Truth“ nicht gewählt wird [^C.3.b.2], weil sie zu teuer oder invasiv ist, muss dies ebenfalls begründet werden. | | 6.3.2.3. |
| C3b4 | Dieses Verfahren legt die Anforderungen an die Anzahl, Schulung und Kompetenz der für das Labeling verantwortlichen Personen fest. | | ISO 13485, 6.2 und 7.3.2, FDA 21 CFR Teil 820.25 | 6.3.2.4. |
| C3b5 | Dieses Verfahren legt fest, wie die Kompetenzen der für das Labeling verantwortlichen Personen überprüft werden. | Dies kann durch das Labeling ausgewählter Datensätze erfolgen. |  |6.3.2.5.|
| C3b6 | Dieses Verfahren legt fest, wie die für das Labeling verantwortlichen Personen geschult werden und wie der Erfolg dieser Schulung bewertet wird. |  ||6.3.2.6.|
| C3b7 | Dieses Verfahren legt fest, wie die Richtigkeit des Labelings systematisch überprüft wird. Die Auswahl dieser Begründung wurde vom Hersteller dokumentiert. | Der Hersteller kann identische Datensätze mehrerer Personen bereitstellen und die Konsistenz der Ergebnisse bewerten. | 6.3.2.7||
| C3b8 | Dieses Verfahren legt fest, wie die Überwachung erfolgt, dass die für das Labeling verantwortlichen Personen kontinuierlich in der Lage und bereit sind, das Labeling durchzuführen [^C.3.b.3]. | Dies kann mit Datensätzen mit bereits bekannten Labels erfolgen, die unbemerkt eingefügt werden während die Person das Labeling macht. ||6.3.2.8.|

[^C.3.b.1]: Wenn beispielsweise Patienten als gesund und krank klassifiziert werden müssen, muss der Hersteller die Kriterien speziell für die Zweckbestimmung ableiten, wann ein Patient als gesund und wann als krank zu klassifizieren ist.

[^C.3.b.2]: Die „Ground Truth“ ist die präziseste Referenzmethode (Stand der Technik). Für die Bestimmung der arteriellen Hypertonie kann eine invasive Blutdruckmessung die genauesten Ergebnisse liefern.

[^C.3.b.3]: Die Kennzeichnung von Dutzenden von Datensätzen ist mühsam. Eine Bezahlung pro Datensatz kann zu einer unangemessenen Motivation führen.

#### c) Verfahren zur (Vor-)Verarbeitung von Daten

| ID | Anforderungen | Kommentare | Regulatorische Referenzen| Team-NB-ID |
| :------------------------------------------------------------| :------------------------------------------------------------|:--|---|:--|
| C3c1 | Der Hersteller hat ein Verfahren festgelegt, das die Vorverarbeitung der Daten beschreibt. | | ISO 13485:2016, 4.1.6, 7.3.6, XAVIER University „Building Explainability and Trust for AI in Healthcare“, FDA 21 CFR part 820.70(i) | 6.3.3.1. |
| C3c2 | Dieses Verfahren beschreibt die einzelnen Verarbeitungsschritte wie Konvertierung, Transformation, Aggregation, Normalisierung, Formatkonvertierung, Berechnung von Merkmalen, Konvertierung numerischer Daten in Kategorien. | Eine grafische Darstellung schafft einen schnellen Überblick. Die Umwandlung von numerischen in diskrete Werte erfordert eine Begründung. | | 6.3.3.2. |
| C3c3 | Das Verfahren beschreibt, wie die Korrektheit der Zwischenschritte und der Endergebnisse durch risikobasierte Bewertungen bewertet werden. [^C.3.c.0] | Dies steht im Einklang mit den Anforderungen von ISO 13485:2016 Kapitel 4.1.6. Die Risikomanagementakte muss diese Analysen enthalten. | ISO 13485, 4.1.6., 7.3.2., 7.5.6. | 6.3.3.3. |
| C3c4 | Dieses Verfahren legt fest, wie Werte mit verschiedenen Messskalen oder Einheiten erfasst und verarbeitet werden. | Dies hängt von der verwendeten ML-Methode ab (z. B. tabellarische Daten/Bilddaten) und kann nicht als allgemeines bewährtes Verfahren gefordert werden. | | 6.3.3.4. |
| C3c5 | Dieses Verfahren legt fest, wie Werte erkannt und verarbeitet werden, die mit verschiedenen Messmethoden erfasst wurden. | Dies hängt von der verwendeten ML-Methode ab (z. B. tabellarische Daten/Bilddaten) und kann nicht als allgemeine bewährte Methode gefordert werden. | | 6.3.3.5. |
| C3c6 | Dieses Verfahren legt fest, wie gleichnamige Werte oder Metadaten (z. B. in Spaltenüberschriften) erkannt und verarbeitet werden. | Dies hängt jedoch von der verwendeten ML-Methode ab (z. B. tabellarische Daten/Bilddaten) und kann nicht als allgemeine bewährte Methode gefordert werden. ||6.3.3.6.|
| C3c7 | Dieses Verfahren legt fest, wie fehlende Werte in Datensätzen erkannt und verarbeitet werden. Der Hersteller begründet seine Entscheidung [^C.3.c.1]. | Stellen Sie sicher, dass in der Begründung zwischen „zufällig fehlend“ und „nicht zufällig fehlend“ unterschieden wird [^C.3.c.2]. | | (6.3.3.7.) |
| C3c8 | Dieses Verfahren legt fest, wie Ausreißer erkannt und verarbeitet werden [^C.3.c.3]. Der Hersteller begründet seine Entscheidung [^C.3.c.4]. | Beispiel für ein Datum/Merkmal anzeigen. Dies hängt jedoch von der verwendeten ML-Methode ab (z. B. Tabellendaten/Bilddaten) und kann nicht als allgemeine bewährte Methode gefordert werden. ||(6.3.3.7.)|
| C3c9 | Dieses Verfahren legt fest, wie unbrauchbare Datensätze erkannt und behandelt werden [^C.3.c.5]. Die Festlegung wurde vom Hersteller begründet. | Beispiel für ein Datum/Merkmal anfordern. ||(6.3.3.7.)|
| C3c10 | Der Hersteller hat die Risiken, die sich aus der Datenverarbeitung ergeben, identifiziert, bewertet und gemanagt. | Risiken können beispielsweise durch Softwarefehler, Rundungsfehler, Re-Sampling und Komprimierung von Daten sowie das Aussortieren ungültiger Daten verursacht werden. | AI4H-DAISAM | |

[^C.3.c.0]: Zu den Optionen gehören Softwaretests und redundante oder alternative Berechnungen wie mit Excel.

[^C.3.c.1]: Zu den Optionen für die Verarbeitung gehören das Löschen des Datensatzes, das Ersetzen durch den Durchschnittswert anderer Datensätze, der neue Wert „fehlt“ (für kategoriale Werte).

[^C.3.c.2]: Ein Beispiel für „fehlt nicht zufällig“ sind Laborwerte, die zu hoch sind und abgeschnitten werden.

[^C.3.c.3]: Zu den Optionen für die Verarbeitung gehören das Löschen des Datensatzes, die Korrektur des Wertes und das Setzen des Wertes auf einen festgelegten Wert (min/max).

[^C.3.c.4]: Diese Begründung ist bei der Regressionsmethode wichtiger als bei "baumartigen Methoden" wie Forest Trees.

[^C.3.c.5]: Beispiele sind Röntgenbilder von schlechter Qualität oder Patienten, die die Einschlusskriterien nicht erfüllen.

#### d) Dokumentation und Versionskontrolle

| ID | Anforderungen | Kommentare | Verweise auf Vorschriften| Team-NB-ID [^C.3.d.1.] |
| :------------------------------------------------------------| :------------------------------------------------------------|:--|---|:--|
| C3c1 | Der Hersteller hat den „Trichter“ beschrieben, der zeigt, wie viele Daten aus welchen Datenquellen (z. B. Kliniken) stammen und bei welchem Verarbeitungsschritt wie viele Datensätze aus welchem Grund verworfen wurden. | |||
| C3c2 | Der Hersteller hat beschrieben, welche Teile der Software für welchen Verarbeitungsschritt verantwortlich sind. | Dies sollte Teil der Architektur dieser Software sein. |||
| C3c3 | Der Hersteller hat die verarbeiteten Daten mit Hilfe deskriptiver Statistiken beschrieben [^C.3.a.4]. | [„Dataset Nutrition Label“](https://ahmedhosny.github.io/datanutrition/) wird empfohlen.|||
| C3c4 | Der Hersteller hat die gesamte Software für die Datenverarbeitung, einschließlich der im Prozess verwendeten Bibliotheken, dokumentiert und unter Versionskontrolle. || ISO 13485, 4.1.6., 4.2.4., 7.5.6. | 6.3.4.10. |
| C3c5 | Der Hersteller hat alle Schulungs-, Validierungs- und Testdaten unter Versionskontrolle. || | 6.3.4.11. |
| C3c6 | Der Hersteller verfügt über ein Verfahren zur Datenspeicherung und -aufbewahrung gemäß den geltenden behördlichen Anforderungen. |Diese Anforderungen legen zum einen eine Mindestaufbewahrungsfrist fest, wie z. B. 2017/745/EG, 2024/1689/EG, ISO 13485. Zum anderen gibt es Datenschutzanforderungen zur Minimierung der (Zeit) der Datenspeicherung.| | 6.3.4.14. |


[^C.3.d.1.]: Die Nummerierung des entsprechenden Abschnitts 6.3.4 im Team-NB-Dokument beginnt mit 9. D. h., die Nummern 6.3.4.1. bis 6.3.4.8. fehlen.

### 4. Modellentwicklung 

#### a) Vorbereitung

| ID | Anforderungen | Kommentare | Verweise auf Vorschriften| Team-NB-ID |
| :------------------------------------------------------------| :------------------------------------------------------------|:--|---|:--|
| C4a1 | Der Hersteller hat die Auswahl der Merkmale begründet, die er beim Training berücksichtigt. | Dies erfordert eine Liste aller Feature. | ISO 13485, 7.3.2., 7.3.3. | (6.4.1.1) |
| C4a2 | Der Hersteller hat die Abhängigkeit der Merkmale untereinander beschrieben, insbesondere für tabellarische Daten. | Ein gerichteter azyklischer Graph (DAG) hilft bei der Visualisierung. Dies hängt von der angewandten ML-Methode ab und kann nicht als "Best Practice" gefordert werden. | ISO 13485, 7.3.2., 7.3.3. | 6.4.1.3. |
| C4a3 | Der Hersteller hat das Verhältnis, in dem er die Daten in Trainings-, Validierungs- und Testdaten aufteilt, dokumentiert und begründet. | ||6.4.1.4.|
| C4a4 | Der Hersteller hat die von ihm verwendete Strategie dokumentiert, um die Daten in Trainings-, Validierungs- und Testdaten aufzuteilen [^C.4.a.1]. | | ISO 24028 9.8.2.1, DAISAM | 6.4.1.5. |
| C4a5 | Der Hersteller hat dokumentiert, wie er sicherstellt, dass mehrere Datensätze für ein Objekt in demselben „Bucket“ (Trainings-, Validierungs- und Testdaten) liegen. | | | |
| C4a6 | Der Hersteller hat dokumentiert, wie er sicherstellt, dass Testdaten nicht für das Modelltraining und die Validierung verwendet werden. | | | 6.4.1.7. |
| C4a7 | Der Hersteller hat beschrieben, ob/wie er die Daten speziell für das Modell oder speziell für die Bibliothek neu codiert [^C.4.a.2]. | ||6.4.1.8.|

[^C.4.a.1]: Bei Daten mit seltenen Merkmalen oder Labels kann es erforderlich sein, die Daten nicht nur zufällig zu verteilen.

[^C.4.a.2]: Beispiele hierfür sind Normalisierung, Auswahl von Klassenbezeichnungen (z. B. 0 oder 1), Auswahl von Spaltennamen, Verteilung von kategorialen Werten über mehrere Spalten.

#### b) Training

| ID | Anforderungen | Kommentare | Regulatorische Referenzen| Team-NB-ID |
| ------------------------------------------------------------ | ------------------------------------------------------------ | -- | -- | -- |
| C4b1 | Der Hersteller führt das Modelltraining, das Tuning der Hyperparameter und die Modellauswahl ausschließlich mit den Trainings- und Validierungsdaten durch (z. B. durch Kreuzvalidierung). | Der Hersteller sollte auch zeigen, dass das Training die Qualität des Modells tatsächlich verbessert. | | |
| C4b2 | Der Hersteller hat verschiedene Sätze von Hyperparametern ausprobiert und seine endgültige Wahl dokumentiert.[^C.4.b.1]. | ISO 14971 verlangt, dass Risiken minimiert werden. | | |
| C4b3 | Der Hersteller hat die Wahl der Epochen dokumentiert [^C.4.b.2]. | |||
| C4b4 | Der Hersteller hat die Qualitätsparameter auf der Grundlage der Zweckbestimmung, für den er das Modell optimieren möchte, festgelegt, dokumentiert und begründet. | Dies bedeutet, dass die Wahl dieser Qualitätsparameter spezifisch für den beabsichtigten Verwendungszweck ist. ||(6.4.2.1.)|
| C4b5 | Der Hersteller hat – soweit sinnvoll – mehrere Modelltypen (einschließlich einfacherer und interpretierbarer Modelle) trainiert und verglichen. | ||6.4.2.2.|

[^C.4.b.1]: Beispiele: Loss-Function, Optimizer, Lernrate, Anzahl der Epochen

[^C.4.b.2]: Es kann nützlich sein, die Abhängigkeit der Qualität des Modells von der Anzahl der Epochen anhand von Lernkurven darzustellen. Diese Lernkurven existieren beispielsweise für neuronale Netze und Boosting-Methoden, nicht jedoch für Modelle mit numerischer Lösung (z. B. lineare Regression) oder mit einem einzelnen Baum. 

#### c) Bewertung / Evaluierung

| ID | Anforderungen | Bemerkungen | Regulatorische Referenzen| Team-NB-ID |
| ------------------------------------------------------------ | ------------------------------------------------------------ |--|--|--|
|C4c1|Der Hersteller hat die Evaluierung des Modells geplant.| Dieser Plan kann Teil eines Entwicklungs- oder V&V-Plans sein. | ISO 13485, 7.3.2, 7.3.6 und 7.3.7, ISO 14971:2019, 10., IEC 62304 5.1 | |
|C4c2 |Der Hersteller hat die Qualitätsmaßnahmen für die verschiedenen Modelle dokumentiert, z. B. im Falle einer binären Klassifizierung unter Verwendung einer Vierfeldertafel. | Diese Dokumentation sollte nicht nur die Werte enthalten, auf die der Hersteller das Modell optimiert hat. | 2024/1689/EU Artikel 9 Abschnitt 8. und Anhang IV Abschnitt 2.(g)| 6.4.3.1. |
|C4c3 |Der Hersteller hat die Qualitätsmetriken nicht nur für die verschiedenen Modelle global bewertet und dokumentiert, sondern gegebenenfalls auch separat für verschiedene Funktionen. | ||6.4.3.2., 6.4.3.3., 6.4.4.9|
|C4c4 |Der Hersteller hat gezeigt, wie man Overfitting erkennt und somit vermeidet. | | ISO 24028 9.8.2.23 | 6.4.3.4. |
|C4c5 |Der Hersteller hat die Datensätze untersucht, die besonders gut und die besonders schlecht vorhergesagt wurden. | Es wird eine Residuenanalyse empfohlen, bei der die Fehler gegebenenfalls gegen die Feature-Werte aufgetragen werden. ||6.4.3.5|
|C4c6|Der Hersteller hat die Datensätze untersucht, für die das Modell besonders sicher und besonders unsicher ist [^C.4.c.1]. | Dies hilft bei der Identifizierung von Einschränkungen, z. B. für bestimmte Patientengruppen | 2024/1689/EU Anhang IV Abschnitt 3| 6.4.3.6|
|C4c7 |Der Hersteller hat die endgültige Wahl des Modells auf der Grundlage der Qualitätskriterien und der Zweckbestimmung begründet und insbesondere erläutert, warum keine einfacheren und besser interpretierbaren Modelle verwendet wurden. | | ISO 14971:2019, XAVIER University „Building Explainability and Trust for AI in Healthcare“, DIN SPECT 2 | 6.4.3.7. |
|C4c8 |Der Hersteller hat insbesondere bei tabellarischen Daten für einzelne Datensätze berücksichtigt, dass das Modell die Feature anzeigt, die die Entscheidung besonders beeinflusst haben [^C.4.c.2]. | Dies kann nicht generell als "Best Practice" gefordert werden. | 6.4.3.8||
|C4c9 |Der Hersteller hat erwogen, insbesondere für tabellarische Daten zu bewerten, wie und wie stark sich einzelne Merkmale ändern müssten, damit das Modell zu einer anderen Vorhersage kommt. | Dies wird als [„counterfactuals“](https://christophm.github.io/interpretable-ml-book/counterfactual.html) bezeichnet. Dies kann nicht generell als "Best Practice" gefordert werden. ||6.4.3.9.|
|C4c10 |Der Hersteller hat in Betracht gezogen, die Abhängigkeit (Stärke, Richtung) der Vorhersagen von den Feature-Werten zu analysieren/visualisieren, insbesondere für tabellarische Daten [^C.4.c.3]. | Dies kann nicht generell als "Best Practice" gefordert werden. ||6.4.3.10.|
|C4c11 |Der Hersteller hat die Synthetisierung von Datensätzen in Betracht gezogen, die das Modell besonders aktivieren [^C.4.c.4]. | Dies kann nicht generell als "Best Practice" gefordert werden. |||
|C4c12 |Der Hersteller hat in Betracht gezogen, das Modell durch ein vereinfachtes "Surogat-Modell" wie einen Entscheidungsbaum anzunähern. | Dies kann nicht generell als "Best Practice" gefordert werden. |||

[^C.4.c.1]: Klassifizierungsaufgaben müssen den aktuellen Stand der Forschung berücksichtigen.

[^C.4.c.2]: Zu den Ansätzen gehören LIME (Local Interpretable Model-agnostic Explanations), Beta (Black Box Explanations through Transparent Approximations), LRP (Layer-wise Relevance Propagation) und Feature Summary Statistics (inkl. Feature Importance und Feature Interaction).

[^C.4.c.3]: Beispiele für Shapley-Werte, ICE-Diagramme, Partial Dependency Plots (PDP)

[^C.4.c.4]: Beispiele finden Sie unter http://yosinski.com/deepvis

#### d) Dokumentation

| ID | Anforderungen | Kommentare |Regulatorische Referenzen|Team-NB-ID|
| ------------------------------------------------------------ | ------------------------------------------------------------ |--|--|--|
| C4d1 | Der Hersteller hat das Modell [^C.4.d.1] und/oder den Trainingscode unter Versions- und Konfigurationskontrolle. | Dies umfasst Skripte und Build-Dateien. | ISO 13485, 4.1.6., 4.2.4., 7.5.6. | 6.4.4.1. |
| C4d2 | Der Hersteller hat seinen Code gemäß seiner Vorgaben dokumentiert. | In der Regel sind mindestens die öffentliche Klasse, Methoden mit Übergabe- und Rückgabewerten sowie Attribute zu dokumentieren |||
| C4d3 | Der Hersteller hat beschrieben, welche Datensätze er für das Training, die Validierung und das Testen des Modells verwendet hat. | |ISO 24028 9.8.2.1, DAISAM||
| C4d4 | Der Hersteller kann die Test- und Validierungsergebnisse reproduzieren. | Zu diesem Zweck ist es sinnvoll, ein Versionsverwaltungssystem nicht nur für den Code, sondern auch für Daten, Testergebnisse und deren Auswertung zu verwenden. Es wird empfohlen, auch die bei der Datenverarbeitung und beim Training verwendete Infrastruktur (Hardware, Betriebssystem, Virtualisierungsebenen wie Docker) zu dokumentieren. Abweichende Ergebnisse sollten begründet werden (z. B. Hardware, Zufallsgeneratoren, Rundungsfehler). Absolute Pfade und betriebssystemspezifische Befehle sind zu vermeiden. | ISO 13485, 7.3.6., 7.3.3. | 6.4.4.2. |
| C4d5 | Der Hersteller hat die SOUP (Bibliotheken und Frameworks) unter Versions- und Konfigurationskontrolle. | | IEC 62304, 8.1.2. | 6.4.4.3. |
| C4d6 | Der Hersteller hat die Architektur des Modells und das Modell selbst einschließlich seiner Algorithmen und Hyperparameter dokumentiert. | Beispielsweise sollten im Fall eines CNN unter anderem die Anzahl und der Typ der Schichten, die Verknüpfung der Neuronen oder Schichten, die Aktivierungsfunktion, der Optimierer und andere Parameter einschließlich ihrer Wertebereiche dokumentiert werden. Die Dokumentation des Modells umfasst auch die Spezifikation der Ausgaben wie die Anzahl der Ausgaben, die jeweiligen Datentypen, Wertebereiche, Einheiten usw. | 2024/1689/EU Anhang IV Abschnitt 2. (b) und (c), IEC 62304 5.3, ISO 13485, 4.2.3., 4.2.5. | 6.4.4.4. |
| C4d7 | Der Hersteller hat beschrieben, wie er die Architekturen ausgewählt, die Modelle trainiert und die Hyperparameter optimiert hat, und dieses Verfahren begründet. | Auditoren möchten nachvollziehen können, wie der Hersteller vorgegangen ist und warum die gewählte Lösung die beste ist. IEC 62304 und die FDA wollen keine „Ad-hoc-Designentscheidungen“. ||(6.4.4.9)|
| C4d8 | Der Hersteller hat beschrieben, wann er mit einem „vortrainierten Modell“ gearbeitet hat, und gezeigt, warum dieses „Vortraining“ für die Aufgabe geeignet ist. | ||6.4.4.5.|
| C4d9 | Der Hersteller hat die Qualität der Modelle auf der Grundlage der Qualitätsmetriken dokumentiert. | Diese Qualitätsmetriken beziehen sich auf das Testen mit den Testdaten. | ISO 13485, 4.2.3., 4.2.5. | 6.4.4.6. |
| C4d10 | Der Hersteller hat die Vertrauensintervalle für die Qualitätsmetriken in Abhängigkeit von den Eingabedaten angegeben. | Insbesondere an den Rändern der zulässigen Eingabedaten nimmt das Vertrauen oft stark ab. Diese Information sollte auch den Anwendern in den Begleitmaterialien zur Verfügung gestellt werden. ||6.4.4.8.|
| C4d11 | Der Hersteller hat insbesondere für tabellarische Daten dokumentiert, innerhalb welcher Grenzen (z. B. Feature-Werte) das Modell die Anforderungen an die Qualitätsmetriken erfüllt. | Dies hängt vom angewandten ML-Modell ab und kann nicht generell als "Best Practise" gefordert werden. | ISO 13485, 4.2.3., 4.2.5. | 6.4.4.7. |
| C4d12 | Der Hersteller hat mehrere Modelle und ihre Hyperparameter ausprobiert und die in diesem Abschnitt genannten Aspekte für sie dokumentiert. | Diese Dokumentation dient dem Hersteller dazu, verschiedene Modelle zu vergleichen und seine Wahl eines Modells zu begründen. Dies ist notwendig, um die Anforderung der ISO 14971 zu erfüllen, das Risiko-Nutzen-Verhältnis zu maximieren. |||

[^C.4.d.1]: Trainierte Modelle können serialisiert werden.

### 5. Produktentwicklung

#### a) Softwareentwicklung

| ID | Anforderungen | Kommentare | Regulatorische Referenzen| Team-NB-ID |
| ------------------------------------------------------------ | ------------------------------- |--| ------------------------------------------------------------ | ------------------------------------------------------------ |
| C5a1 | Der Hersteller hat die erforderlichen Aktivitäten gemäß IEC 62304 durchgeführt und dokumentiert. | Hinweise für Auditoren[^C.5.a.1] | IEC 62304, IEC 82304-1, XAVIER University „Building Explainability and Trust for AI in Healthcare“, FDA-Guideline zur Softwarevalidierung, FDA OTS-Leitfaden | (6.5.1.1.) |
| C5a2 | Wenn der Hersteller das Modell in einer anderen Programmiersprache oder für eine andere Laufzeitumgebung implementiert hat, hat er einen Plan erstellt, der die Aktivitäten gemäß Kapitel 4 wiederholt. | | IEC 62304, IEC 82304-1 | 6.5.1.2. |
| C5a3 | Der Hersteller hat die Leistung (Reaktionszeiten, Ressourcenverbrauch) auf der Zielhardware (z. B. Browser, Mobilgerät) überprüft. | | 2017/745/EU, Anhang I, 17.1., 17.3., 2017/746/EU, Anhang I, 16.1., 16.3. | 6.5.1.3. |
| C5a4 | Der Hersteller hat die SOUP- und OTS-Anforderungen spezifiziert. | ISO 25010 enthält eine Liste von Qualitätsaspekten wie Leistung, IT-Sicherheit, Portabilität und Interoperabilität. | IEC 62304, 5.3, | 6.5.1.5. |
| C5a5 | Der Hersteller hat beschrieben, wie alle SOUP- und OTS-Komponenten zu verifizieren sind und hat diese Verifizierung auch durchgeführt und dokumentiert. | | IEC 62304, 5.3, 8.1.2, FDA OTS Guidance | 6.5.1.4. |
| C5a6 | Der Hersteller hat die vorgeschriebenen Lizenzbedingungen der Software beigefügt und die Rechtmäßigkeit der Verwendung von Software von Drittanbietern (z. B. Open-Source-Software) sichergestellt. | Hersteller verwenden häufig Open-Source-Software, die nur im Rahmen von Lizenzen und Erklärungen zu den Nutzungsbedingungen verwendet werden darf. |||

[^C.5.a.1]: Die Hersteller sollten sich an die üblichen bewährten Verfahren halten, wie die Einhaltung von Programmierrichtlinien, die Überprüfung des Codes durch Code-Reviews anhand definierter Kriterien, das Testen des Codes mit Unit-Tests mit einer definierten Abdeckung usw. Eine Beschreibung des Codes (Architektur) sollte leicht verständlich machen, welcher Code welche Aufgabe erfüllt.


#### b) Begleitmaterialien

| ID | Anforderungen | Kommentare | Verweise auf Vorschriften| Team-NB-ID |
| ------------------------------------------------------------ | ------------------------------------------------------------ |--|--|--|
| C5b1 | Die Gebrauchsanweisung muss die Produktversion eindeutig identifizieren. | Wenn möglich, geben Sie die UDI an. | 2017/745/EU, Anhang I, Kap. III, 23.1, 23.4., 2024/1689/EU Artikel 13 Abschnitt 3.(b)(i), FD&C, FDA 21 CFR Teile 801 und 820.120, ISO 24028 z. B. 10.11.3 | 6.5.2.1 |
| C5b2 | Die Gebrauchsanweisung beschreibt den bestimmungsgemäßen Gebrauch des Produkts einschließlich des erwarteten medizinischen Nutzens. | | 2017/745/EU, Anhang I, Kap. III, 23.1, 23.4., 21 CFR Teil 801, 21 CFR Teil 814.20, XAVIER: „Perspectives and Good Practices for AI and Continuously Learning Systems in Healthcare“, ISO 24028, XAVIER University Building Explainability and Trust for AI in Healthcare‘, ISO 24028 z. B. 10.11.3 | 6.5.2.3. |
| C5b3 | Die Gebrauchsanweisung spezifiziert die vorgesehene Patientengruppe anhand von Indikationen, Kontraindikationen und gegebenenfalls anhand anderer zusätzlicher Parameter wie Alter, Geschlecht, Begleiterkrankungen. | | 2017/745/EU, Anhang I, Kap. III, 23.1, 23.4. | 6.5.2.4. |
| C5b4 | Die Gebrauchsanweisung führt ausdrücklich die Patienten / Daten / Anwendungsfälle auf, für die das Produkt **nicht** verwendet werden darf. | | 2017/745/EU, Anhang I, Kap. III, 23.1, 23.4. | 6.5.2.6. |
| C5b5 | Die Gebrauchsanweisung dokumentiert die Anforderungen an die Eingabedaten (einschließlich Formate, Auflösungen, Wertebereiche usw.). | |2024/1689/EU Artikel 13 Abschnitt 3.(b)(vi)|6.5.2.7.|
| C5b6 | In der Gebrauchsanweisung sind die vorgesehenen primären und sekundären Nutzer gemäß der vorgesehenen Verwendung anzugeben. | Primäre Nutzer verwenden das System, um die vorgesehene medizinische Zweckbestimmung zu erreichen, z. B. zur Diagnose von Patienten. Die sekundäre Verwendung umfasst die anderen Zwecke wie Installation, Update, Konfiguration und Verwaltung des Produkts. | 2024/1689/EU Artikel 13 Abschnitt 3.(b)(v)| 6.5.2.8. |
| C5b7 | Die Gebrauchsanweisung beschreibt die sonstigen für das Produkt geltenden Voraussetzungen (z. B. Laufzeitumgebung, Nutzungsumgebung). | Die Laufzeitumgebung umfasst Hardware- und Softwarevoraussetzungen. | 2024/1689/EU Artikel 13 Abschnitt 3 Buchstabe e und Anhang IV Abschnitte 1 Buchstaben b und e|6.5.2.10.|
| C5b8 | Die Gebrauchsanweisung beschreibt, wie das Produkt zu verwenden ist. | Dies umfasst das Verhalten im Falle eines Problems (z. B. „menschliches Versagen“) sowie die sekundäre Nutzung wie Installation, Aktualisierung, Upgrade und Konfiguration sowie Verwaltung der Audit-Protokolle). |2024/1689/EU Artikel 13 Abschnitt 3.(d), (e) und (f)|6.5.2.2.|
| C5b9 | Die Gebrauchsanweisung beschreibt die möglichen Ergebnisse. | Dies umfasst auch die vom Produkt angezeigten Erläuterungen („Erklärbarkeit“). | 2024/1689/EU Artikel 13 Abschnitt 3. Buchstabe b Ziffer vii ||
| C5b10 | Die Gebrauchsanweisung beschreibt die Restrisiken. | Auch das Risiko einer vorhersehbaren Fehlanwendung | 2017/745/EU, Anhang I, 23.4, ISO 14971:2019, 8, 2024/16 89/EU Artikel 13 Abschnitt 3.b.iii, ISO 24028 z. B. 10.11.3 | 6.5.2.11., 6.6.3. |
| C5b11 | Die Gebrauchsanweisung gibt die Daten an, mit denen das Modell trainiert wurde. | Dies bezieht sich sowohl auf die Patientenpopulation als auch auf die verwendeten Funktionen. | 6.5.2.12 ||
| C5b12 | Die Gebrauchsanweisung beschreibt das Modell und die Algorithmen. |  ||6.5.2.13|
| C5b13 | Die Gebrauchsanweisung nennt die Qualitätsmetriken. | Geben Sie hier auch die Konfidenzbereiche an. | 2024/1689/EU Artikel 13 Abschnitt 3.b.ii | 6.5.2.14. |
| C5b14 | Die Gebrauchsanweisung listet die Faktoren auf, die sich negativ auf die Leistung des Produkts auswirken könnten. | |2024/1689/EU Artikel 13 Abschnitt 3.(b)(iii) |6.5.2.15. |
| C5b15 | Die Gebrauchsanweisung gibt an, ob das Produkt während der Nutzung weiter trainiert wird. | Bitte beachten Sie die Hinweise im Kapitel über kontinuierlich lernende Systeme. | | |
| C5b16 | Die Gebrauchsanweisung enthält Verweise auf weiterführende Literatur. | |||
| C5b17 | Die Gebrauchsanweisung enthält Verweise auf Lizenzrechte. | | 2017/745/EU, Anhang I, 23.4, EU-Verordnung 207/2012| |
| C5b18 | Die Gebrauchsanweisung nennt den Hersteller und listet Kommunikationskanäle für Fragen auf. | | 2017/745/EU, Anhang I, 23.4, EU-Verordnung 207/2012| 6.5.2.17. |
| C5b19 | Die Gebrauchsanweisung listet mögliche ethische Probleme auf. | |||
| C5b20 | Die Gebrauchsanweisung enthält die URL, unter der die aktuellsten Versionen der Gebrauchsanweisung zu finden sind. | Unterschiedliche Vorschriften erlauben, verbieten oder erzwingen elektronische Gebrauchsanweisungen. | 2017/745/EU, Anhang I, 23.4, EU-Verordnung 207/2012| 6.5.2.18. |


#### c) Validierung der Gebrauchstauglichkeit

|ID |Anforderungen |Kommentare| Verweise auf Vorschriften| Team-NB-ID |
| ------------------------------------------------------------ | --------- |--|--|--|
| C5c1 | Im Rahmen der Validierung der Gebrauchstauglichkeit bewertet der Hersteller, ob die Benutzer die Gebrauchsanweisung verstehen. | Dies umfasst auch andere Begleitmaterialien. | IEC 62366-1, FDA HFE-Leitfaden | 6.5.3.1. |
| C5c2 | Im Rahmen der Validierung der Gebrauchstauglichkeit bewertet der Hersteller, ob die Benutzer dem Produkt blind vertrauen oder die Ergebnisse überprüfen. | | IEC 62366-1 | 6.5.3.2. |
| C5c3 | Im Rahmen der  Validierung der Gebrauchstauglichkeit bewertet der Hersteller, ob die Benutzer die Ergebnisse richtig erkennen und verstehen. | Dies umfasst auch die Anzeige von Fehlern und die Erklärungen („Erklärbarkeit“). Hersteller sollten alle sicherheitsrelevanten Nutzungsszenarien in die Validierung und alle risikominimierenden Maßnahmen an der Schnittstelle einbeziehen. | IEC 62366-1, 5.7-5.9 | 6.5.3.3. |


#### d) Risikomanagement

| ID | Anforderungen | Kommentare | Verweise auf Vorschriften| Team-NB-ID |
| ------------------------------------------------------------ | -------- |--| ------------------------------------------------------------ | ------------------------------------------------------------ |
| C5d1 | Der Hersteller hat die Risiken bewertet, die entstehen, wenn die Eingaben nicht den festgelegten Anforderungen entsprechen [^C.2.a.2]. | | ISO 14971:2019, 5.4, IEC 62304, 7.1, DIN SPEC 2, IEC 82304-1 4.1.c) | |
| C5d2 | Der Hersteller hat Risiken, die durch "adversarial attacks" entstehen, identifiziert und gemindert. | Diese Angriffe (in der Regel durch subtile Manipulationen der Eingabedaten) sollen dazu führen, dass das KI-System falsche Vorhersagen machen wie Fehlklassifizierungen. | | 6.2.4.6. |
| C5d3 | Der Hersteller hat die quantitativen Qualitätskriterien auf der Grundlage des Stands der Technik abgeleitet. | Der Hersteller muss in der Lage sein, die Qualitätskriterien für alternative Technologien und Verfahren zu benennen und zu argumentieren, wenn das Medizinprodukt den Alternativen in Bezug auf die Qualitätskriterien nicht überlegen ist [^C.5.d.1]. | 2017/745/EU Anhang 1 1., 2017/745/EU Anhang 1 1., 2024/1689 Artikel 8 Abschnitt 1.| 6.1.4.10. |
| C5d4 | Der Hersteller hat den Goldstandard definiert und seine Wahl begründet, der zur Überprüfung der Qualitätskriterien verwendet wird. | | XAVIER University „Building Explainability and Trust for AI in Healthcare“, FDA proposed regulatory framework for modifications to AI/ML based SaMD: "reference standard" | |
| C5d5 | Der Hersteller hat Risiken identifiziert, bewertet und gemanagt, die entstehen, wenn die Ergebnisse nicht den festgelegten Qualitätskriterien entsprechen. | In dieser Analyse berücksichtigt der Hersteller auch die spezifischen Eigenschaften des ausgewählten Modells sowie die Konfidenzintervalle der während des Tests ermittelten Ausgabewerte. | ISO 14971:2019, 5.3, IEC 62304, 7.1, IEC 82304-1, 4.1.c), XAVIER University „Building Explainability und Vertrauen für KI im Gesundheitswesen“, FDA Guidance zur Softwarevalidierung, 5.2.2, 2024/1689/EU Artikel 9 Abschnitte 2.(d) und 5.(a) | 6.1.4.7 |
| C5d6 | Der Hersteller hat die Folgen bewertet, wenn das System sozial inakzeptable Ergebnisse liefert (z. B. diskriminierend). | Diese „Folgen“ sind nicht unbedingt Risiken im Sinne von ISO 14971. | Ethik-Leitlinien für vertrauenswürdige KI, 2024/1689/EU Artikel 9 2. Abschnitte 2.(d) und 5.(a) | |
| C5d7 | Der Hersteller hat die Risiken ermittelt, bewertet und gemanagt, wenn das System nicht verfügbar ist. | | 2024/1689/EU Artikel 9 Abschnitt 2.| 6.1.4.12 |
| C5d8 | Der Hersteller hat die Risiken, die sich aus Softwarefehlern ergeben, ermittelt, bewertet und gemanagt. | Dies umfasst Fehler in SOUP sowie in der Software, die für die „Vorverarbeitung“ der Daten und für das Training des Modells verwendet wird. | | |
| C5d9 | Der Hersteller hat die Risiken, die sich aus der spezifischen Wahl der Modellarchitektur ergeben, identifiziert, bewertet und gemanagt. | Dabei sollten die Hersteller auch analysieren, ob die Modelle auf die richtigen Spezifikationen hin optimiert wurden. | ISO 14971:2019 | |
| C5d10 | Der Hersteller hat die Risiken, die sich aus der spezifischen Wahl der Zielplattform ergeben, identifiziert, bewertet und gemanagt. | Beispielsweise könnte die Zielplattform nicht die erforderliche Rechenleistung bieten oder einen Absturz der Software verursachen. | | 6.1.4.13 |
| C5d11 | Der Hersteller hat die Risiken, die sich aus der Auswahl der Trainings-, Validierungs- und Testdaten ergeben, ermittelt, bewertet und beherrscht. | Dies betrifft sowohl die Quellen dieser Daten (z. B. Patienten, Einrichtungen) als auch die Aufteilung dieser Daten in Trainings-, Validierungs- und Testdaten. Beispielsweise sollten Hersteller überprüfen, ob die Ergebnisse nicht "overfitted" sind oder oder einen Bias haben. | 2024/1689/EU Artikel 9 Abschnitte 2.(d) und 5.(a), Artikel 10 Abschnitte 2.(f), 2.(g), 4. | (6.1.2.5), (6.1.4.11), (6.1.4.14) |
| C5d12 | Der Hersteller hat die Risiken, dass die Ergebnisse (Vorhersagen, Klassifizierungen usw.) nur zufällig korrekt sind, identifiziert, bewertet und gemanagt. | Die Interpretierbarkeit ermöglicht es Herstellern zu zeigen, warum ein ML-Modell eine bestimmte Entscheidung getroffen hat. |||
| C5d13 | Der Hersteller hat die Risiken identifiziert, die sich daraus ergeben, dass die Vorhersagen selbst die vorhergesagten Ergebnisse verändern. | Bei diesem Phänomen wechselt das Modell vom Beobachter zum Akteur [^C.5.d.2]. Man spricht von „performative prediction“. Hersteller sollten die möglichen Auswirkungen auf Menschen oder Systeme untersuchen und sie z. B. mit einem DAC („directed acyclic graph“) beschreiben, eine mögliche „distribution shift“ und ggf. eine unbeeinflusste Kontrollgruppe beobachten und ggf. Maßnahmen ergreifen, wie die Wahl eines anderen Modells oder das erneute Training des bestehenden Modells. | 2024/1689/EU Artikel 15 Abschnitt 4| 6.1.4.17 |
| C5d14 | Wenn der Hersteller Selbsttests verwendet, hat er erklärt, welche der festgelegten Qualitätskriterien damit überprüft werden und welche Risiken dadurch kontrolliert werden. | Diese Selbsttests entsprechen einem Mittel zur Risikominderung. |||
| C5d15 | Der Hersteller hat die Risiken von Nutzungsfehlern, die durch Wahrnehmungsprobleme verursacht werden, identifiziert, bewertet und gemanagt. | Diese Probleme können durch komplexe Benutzerschnittstellen, neue Eingabemodalitäten, neue oder zusätzliche Informationen (die zu einer kognitiven Überlastung führen) verursacht werden. | IEC 62366-1, 5.3f, FDA HFE-Leitfaden, FDA Guidance zur Softwarevalidierung, 5.2.3, UK 811.4 Positionspapier | (6.1.4.17) |
| C5d16 | Der Hersteller hat die Risiken von Nutzungsfehlern, die durch kognitive Probleme verursacht werden, identifiziert, bewertet und gemanagt. | Beispiele sind kognitive Überlastung, mangelndes Situationsbewusstsein (situational awareness), mangelndes Bewusstsein für die Grenzen des Systems, "confirmation bias", ein fehlerhaftes mentales Modell, übermäßiges Vertrauen und Misstrauen. | IEC 62366-1, 5.3f, FDA HFE-Leitfaden, FDA Guidance zur Softwarevalidierung, 5.2.3, UK 811.4 Positionspapier | (6.1.4.17) |
| C5d17 | Der Hersteller hat die Risiken von Nutzungsfehlern, die durch die Erläuterungen auf der Benutzeroberfläche oder in der Gebrauchsanweisung verursacht werden, identifiziert, bewertet und gemanagt. | „Erklärbarkeit“ kann ein Mittel für die Risikominderung sein, aber selbst neue Nutzungsfehlern verursachen. | IEC 62366-1, 5.3f, FDA HFE-Leitfaden, FDA Guidance zur Softwarevalidierung, 5.2.3 | (6.1.4.17) |
| C5d18 | Der Hersteller hat die Risiken durch falsche, verspätete oder fehlende Handlungen der Nutzer ermittelt, bewertet und gemanagt. | Z. B. können KI-Systeme Angst/Zögern verursachen und dadurch Handlungen verzögern oder aufgrund von Überforderung im System zu keiner Handlung führen. | UK 811.4 Positionspapier||
| C5d19 | Der Hersteller hat die anderen in Kapitel C.1.d) genannten Risiken ermittelt, bewertet und kontrolliert. | |||
|C5d20 |Der Hersteller hat „menschliche Aufsicht“ als eine Maßnahme zur Risikominderung bewertet und die Entscheidung dokumentiert. |Benutzer können eingreifen, z. B. einen Not-Aus-Schalter drücken.| 2024/1689/EU Artikel 14 und Anhang IV Abschnitt 2.(e)| |
|C5d21|Der Hersteller hat die "Protokolle" gemäß 2024/1689/EU auf Risiken analysiert.| Dies ist auch eine Pflicht zur Überwachung nach dem Inverkehrbringen. |2024/1689/EU Artikel 9 Abschnitt 2.||

[^C.5.d.1]: Der Stand der Technik entspricht nicht unbedingt dem Goldstandard, der wiederum nicht unbedingt der "ground truth" entspricht. Das heißt, die Systemanforderungen können niedriger sein als bei einem Goldstandard oder einer Grundwahrheit, insbesondere wenn letztere ein invasives oder sehr kostspieliges Verfahren erfordern. 
[^C.5.2.d]: Beispiele für dieses Phänomen finden Sie [hier](https://mindfulmodeler.substack.com/p/correction-you-can-break-a-predictive). 

#### e) Klinische Bewertung, Leistungsbewertung

|ID |Anforderungen |Kommentare| Verweise auf Vorschriften| Team-NB-ID |
| ------------------------------------------------------------ | --------- |--| ------------------------------------------------------------ | ------------------------------------------------------------ |
| C5e1 | Im Rahmen der klinischen Bewertung/Leistungsbewertung hat der Hersteller bewertet, ob der versprochene medizinische Nutzen für die gegebenen Qualitätsparameter erreicht wird. |  | 2017/745/EU, Artikel 61, Anhang XIV und Anhang XV, 2017/746/EU, Anhang XIII und Anhang XIV, MEDDEV 2.7/1 rev.4, XAVIER University „Building Explainability and Trust for AI in Healthcare“, FDA 21 CFR Teil 820.30(g) |6.5.4.1.|
| C5e2 | Im Rahmen der klinischen/Leistungsbewertung hat der Hersteller beurteilt, ob die versprochenen medizinischen Vorteile und Risiken dem Stand der Technik entsprechen. | | 2017/745/EU, Artikel 61, Anhang XIV und Anhang XV, 2017/746/EU, Anhang XIII und Anhang XIV, MEDDEV 2.7/1 rev 4, ISO 14971:2019, 4.2 | 6.5.4.2. |
| C5e3 | Der Hersteller hat die PMCF-/PMPF-Anforderungen festgelegt. | | 2017/745/EU, Artikel 61 (11), 2017/746/EU, Artikel 56 (6, | 6.5.4.4. |


### 6. Produktfreigabe

|ID |Anforderungen |Kommentare| Verweise auf Vorschriften| Team-NB-ID |
| ------------------------------------------------------------ | --------- |--|--|--|
| C6.1 | Der Hersteller hat sichergestellt, dass alle oben genannten Unterlagen verfügbar sind. | Dies betrifft unter anderem die in den Kapiteln 3.d), 4.d und 5.b) geforderte Dokumentation. | 2017/745/EU, Anhänge I und II, ISO 13485 z. B. 7.3.5, FDA 21 CFR Teil 820.30(e) | (6.6.1) |
|C6.2|Der Hersteller hat die Softwareversion in der Dokumentation angegeben.|| 2024/1689/EU Anhang IV Abschnitt 1.c| |
| C6.3 | Der Hersteller hat die Risiken im Rahmen des Risikomanagements als akzeptabel bewertet und dokumentiert, dass alle im Risikomanagementplan festgelegten Maßnahmen durchgeführt wurden. | Hinweis für Auditoren [^C.6.1] ||6.6.2.|
|C6.4| Der Hersteller hat in den Software as a Medical Device Pre-Specifications (SPS) dargelegt, welche Arten von Änderungen er für Systeme erwartet, die er in den USA vermarkten möchte [^C.6.2]. | | 2024/1689/EU Anhang IV Abschnitt 2.(f), FDA | |
| C6.5 | Der Hersteller hat im Algorithmus-Änderungsprotokoll (ACP) dargelegt, wie er diese Änderungen für Systeme, die er vermarkten möchte, durchführen wird [^C.6.3]. | |2024/1689/EU Anhang IV Abschnitt 2.(f), FDA||
| C6.6 | Der Hersteller hat einen Plan zur Überwachung nach dem Inverkehrbringen erstellt, siehe unten. | |||

[^C.6.1]: Anhand von Beispielen ist zu überprüfen, ob die Wirksamkeit der Maßnahmen zur Risikokontrolle getestet wurde, damit die Risiken zu den Maßnahmen rückverfolgbar sind.

[^C.6.2]: Änderungen können sich auf die Zweckbestimmung, die Eingabedaten und die klinische und analytische Leistung auswirken.

[^C.6.3]: Der Ansatz muss beispielsweise den Umgang mit Daten, die erneute Schulung, die Leistung und die Aktualisierungen berücksichtigen.

## D) Anforderungen für die Phasen nach der Entwicklung

### 1. Produktion, Vertrieb, Installation

|ID|Anforderung|Kommentar|Regulatorische Referenzen|Team-NB-ID |
|:--|:--|:--|---|:--|
|D1.1|Der Hersteller hat beschrieben, wie er sicherstellt, dass nur genau die vorgesehenen Artefakte (Dateien) in genau der vorgesehenen Version des Produkts oder als Produkt ausgeliefert werden.|Dies ist das Konfigurationsmanagement. Auch relevant für Downloads oder AppStores.| IEC 62304, 5.8.8. | 7.1.1. |
|D1.2 |Der Hersteller hat beschrieben, wie die für die Installation verantwortlichen Personen wissen, welche die neueste Version ist und wie Verwechslungen während der Installation ausgeschlossen werden können. |Dies ist nur für eigenständige Software relevant. Hier wäre eine SOP oder Arbeitsanweisung zu erwarten.| ISO 13485, 7.8.3., 8.3., IEC 62304, 5.8.4. | 7.1.2. |
|D1.3|Der Hersteller hat beschrieben, wie während der Installation sichergestellt wird, dass die in den Begleitmaterialien (siehe oben) angegebenen Anforderungen tatsächlich erfüllt werden.|Hier wäre eine SOP oder Arbeitsanweisung zu erwarten.| ISO 13485, 7.5.3. | 7.1.3. |
|D1.4|Der Hersteller hat Verfahren festgelegt, die sicherstellen, dass er zeitnah mit den Betreibern und Anwendern seines Produkts kommunizieren kann.|| ISO 13485, 7.2.3., 8.3.3., IEC 82304-1, 8.4. | 7.1.4. |


### 2. Überwachung nach dem Inverkehrbringen (Post-Market Surveillance)

|ID|Anforderungen|Kommentare| Verweise auf Vorschriften| Team-NB-ID |
|:--|:--|:--|---|:--|
|D2.1|Der Hersteller hat einen Plan zur Überwachung nach dem Inverkehrbringen (PMS) erstellt.|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII, 2024/1689/EG Artikel 17 Abschnitt 1.(h), Artikel 72 | 6.6.4., 7.2.1. |
|D2.2|Der Hersteller hat die Daten angegeben, die er in diesem PMS-Plan erfassen und analysieren möchte.|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII | 7.2.2. |
|D2.3 |Im PMS-Plan hat der Hersteller festgelegt, dass die Informationen aus dne "Protokollen" gesammelt und analysiert werden. |Diese Informationen sind die „automatisch erstellten Protokolle“ gemäß 2024/1689/EG, Artikel 12 Absatz 2 Buchstabe b.|2024/1689/EC article 12 section 2.(b)||
|D2.4|Im PMS-Plan hat der Hersteller die Qualitätskriterien und Schwellenwerte angegeben, die er für notwendig erachtet, um insbesondere eine Neubewertung der Risiko-Nutzen-Analyse vorzunehmen.|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII | 7.2.3. |
|D2.5|Der Hersteller hat bei der Festlegung dieser Schwellenwerte analysiert, welche Rückkopplungsschleifen ("feedback loops") die Schwellenwerte beeinflussen können[^D.2.1].|Diese Analyse dient auch als Maßnahme gegen das oben genannte Risiko durch „Performance Prediction“.| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII | |
|D2.6|Der Hersteller hat bei der Festlegung dieser Schwellenwerte analysiert, welche "self-fulfilling prophecies" die Schwellenwerte beeinflussen können[^D.2.2].|  | 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII ||
|D2.7|Im PMS-Plan hat der Hersteller beschrieben, wie er Informationen über unerwünschte Nebenwirkungen sammelt und analysiert.|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII | 7.2.4. |
|D2.8|Im PMS-Plan hat der Hersteller beschrieben, welche Informationen über (nachteilige) Verhaltensänderungen oder (vorhersehbaren) Missbrauch gesammelt und analysiert werden[^D.2.3].|| 2017/74 5/EU, Kapitel VII, 2017/746/EU, Kapitel VII, 2024/1689/EG Artikel 9 Abschnitt 2.(b) | 7.2.5. |
|D2.9|Im PMS-Plan hat der Hersteller beschrieben, wie er Informationen über zusätzliche „unerwünschte Wirkungen“ sammelt und analysiert [^D.2.4].|  | 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII |7.2.6.|
|D2.10|Der Hersteller hat im PMS-Plan beschrieben, wie er Informationen sammelt, um analysieren zu können, ob die Daten im Feld mit den erwarteten Daten oder Trainingsdaten übereinstimmen[^D.2.5].|Hinweis für Auditoren[^D.2.6]| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII | 7.2.7. |
|D2.11|Im PMS-Plan hat der Hersteller beschrieben, wie und wie oft er Informationen darüber sammeln möchte, ob das Produkt noch dem Stand der Technik entspricht.|Hinweis für Auditoren[^D.2.7]| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII | 7.2.8. |
|D2.12|Im PMS-Plan hat der Hersteller beschrieben, wie und wie oft er Informationen darüber sammeln möchte, ob die „Ground Truth“ oder der Goldstandard noch aktuell sind.|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII | 7.2.9. |
|D2.13|Im PMS-Plan hat der Hersteller beschrieben, wie und wie oft Änderungen gemäß dem Algorithmus-Änderungsprotokoll (ACP) und innerhalb der „SaMD-Vorab-Spezifikationen“ (SPS) vorgenommen werden.|| 2017/745/EU, Kapitel VII, 2017/746/EU, Kapitel VII | |
|D2.14|Die in den Plänen geforderten Berichte sind zu den darin angegebenen Zeiten verfügbar.|z. B. PSUR, SSCP|2017/745/EU Artikel 85 f., 2017/747EU Artikel 80 f.|7.2.10.|

[^D.2.1]: Beispiele für diese Rückkopplungsschleifen: **Beispiel 1**: Eine Reiseempfehlungs-App sendet je nach Funktion (letzte Reise) gezielte Werbung. Dies beeinflusst das Reiseverhalten. **Beispiel 2**: Ein Algorithmus liefert Prognosen. Daher wird der Arzt die Patienten besser oder früher behandeln...

[^D.2.2]: Beispiel 1 (Kriminalistik)

[^D.2.3]: Beispiel: Radiologen verlassen sich auf die Software und schauen sich die Bilder nicht mehr an, sodass sie Befunde übersehen.

[^D.2.4]: Beispiele wären ethische Herausforderungen wie der YouTube-Algorithmus, der zwar das Ziel erreicht, die Klickzahl oder Nutzungsdauer zu maximieren, aber Gewalt- und Verschwörungsvideos fördert.

[^D.2.5]: Man spricht hier von einer "distribution drift" oder "data drift".

[^D.2.6:]: Der Hersteller sollte Schwellenwerte für Merkmale oder für die Varianz/Kovarianz über die Zeit festlegen. Dies ermöglicht eine Visualisierung oder Quantifizierung insbesondere für nicht normalverteilte Daten über den Vergleich von Histogrammen oder "Density Estimations".

[^D.2.7]: Lassen Sie sich beispielsweise vom Hersteller erklären, wie er systematisch über neue Entwicklungen im Bereich des maschinellen Lernens informiert wird, wie er diese Entwicklungen bewertet und darauf reagiert.



### 3. Außerbetriebnahme


|ID|Anforderungen|Kommentare| Verweise auf Vorschriften| Team-NB-ID |
|:--|:--|:--|---|:--|
|D3.1 |Der Hersteller hat einen Außerbetriebnahmeplan erstellt, bevor er sein Produkt vom Markt nimmt. | Ein solcher Plan legt beispielsweise fest, ob und wie die Software deinstalliert werden muss, ob Daten gesichert oder exportiert werden müssen, wie die Vertraulichkeit der Daten gewährleistet bleibt, wer für diese Aktivitäten verantwortlich ist, wie der Fortschritt der Außerbetriebnahme überwacht und sichergestellt wird und welche Organisationen informiert werden müssen und wie.| ISO 24028 | 7.3.1 |
|D3.2 |Der Hersteller hat identifiziert, bewertet und kontrolliert die Risiken, die sich aus der Außerbetriebnahme ergeben. | Dies ist in der Risikomanagementakte zu bewerten. Risiken durch Nichtverfügbarkeit des Produkts, durch Anwendungsfehler und durch Beeinflussung anderer Produkte sind zu berücksichtigen. | 2017/746/EU Anhang I, 3., ISO 14971:2019 Kapitel 10 in Verbindung mit 3.8 und 3.12, ISO 24028 | 7.3.2. |


## E) Anhänge

### 1. Weiterführende Literatur

#### a) Gesetze

- [Verordnung über Medizinprodukte](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=uriserv:OJ.L_.2017.117.01.0001.01.DEU&toc=OJ:L:2017:117:FULL) MDR
- [Verordnung über In-vitro-Diagnostika](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=uriserv:OJ.L_.2017.117.01.0176.01.DEU&toc=OJ:L:2017:117:FULL) IVDR
- [Verordnung über künstliche Intelligenz](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202401689) (KI-Verordnung, AI Act)

#### b) Normen und Leitfäden für bewährte Verfahren

* **IEC 62304/AMD1**, Software für Medizinprodukte – Software-Lebenszyklusprozesse
* **IEC 82304-1**, Gesundheitssoftware – Teil 1: Allgemeine Anforderungen an die Produktsicherheit
* [FDA-Leitfäden zum maschinellen Lernen](https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-and-machine-learning-software-medical-device)
* [Position Paper of DKE UK 811.4 'Usability Engineering for Medical Devices using Artificial Intelligence and Machine Learning Technology'](https://doi.org/10.5281/zenodo.14203190)

#### c) Branchenliteratur, Lehrbücher

- Christoph Molnar: [Interpretierbares maschinelles Lernen](https://christophm.github.io/interpretable-ml-book/)
- Patrick Hall: [Interpretierbarkeit des maschinellen Lernens
mit H2O Driverless AI](http://docs.h2o.ai/driverless-ai/latest-stable/docs/booklets/MLIBooklet.pdf)
- Patrick Hall: [On the Art and Science of Machine Learning Explanations](https://arxiv.org/pdf/1810.02909.pdf)
- Johner Institute: [Video-Schulung zum maschinellen Lernen für Medizinprodukte](www.auditgarant.de)

#### d) Quellen und Checklisten für die Reproduzierbarkeit

- https://www.cs.mcgill.ca/~jpineau/ReproducibilityChecklist-v2.0.pdf
- https://epub.ub.uni-muenchen.de/92151/1/92151.pdf
- https://github.com/craig-willis/reproducibility-checklist/
- https://2020.emnlp.org/call-for-papers#new-reproducibility-criteria
- https://onlinelibrary.wiley.com/pb-assets/assets/15214036/RR_Guideline.pdf

### 2. Erwägungsgründe

1. Hersteller entwickeln zunehmend Medizinprodukte, die Verfahren der künstlichen Intelligenz, insbesondere des maschinellen Lernens, nutzen. Viele dieser Verfahren sind noch sehr neu und es fehlen bewährte Verfahren. Dies birgt neue Risiken für Patienten, Anwender und Dritte.
2. Die EU-Richtlinien (MDR, IVDR) fordern in den entsprechenden Anhängen I ausdrücklich die Sicherheit der Produkte. Konkrete Anforderungen für diese Produktklassen fehlen jedoch vollständig. Daher fehlen sowohl den Herstellern als auch den benannten Stellen und Behörden konkrete Richtlinien, wie die Sicherheit der Produkte bewertet werden kann.
3. Im Gegensatz zu den meisten anderen grundlegenden Anforderungen sind keine Normen zum Thema KI harmonisiert. Daher gibt es keinen kanonischen Anforderungskatalog, der den anerkannten Stand der Technik widerspiegelt.
4. Die FDA hat begonnen, Anforderungen an den Einsatz von Continuous Learning Systems, CLS, zu formulieren. Diese Vorgaben sind ungeeignet, um bereits in der Produktentwicklung hinreichend Anforderungen an die Produkte und Prozesse zu stellen.
5. Die Sicherheit von Medizinprodukten muss in allen Phasen der Produktlebenszyklusprozesse berücksichtigt werden. Eine Beschränkung auf die Prüfung ist unzureichend. Diese Tatsache muss mit bewährten Verfahren und Richtlinien in Einklang stehen.
6. Man hofft, dass Normen für die Sicherheit von KI-basierten Medizinprodukten entwickelt und harmonisiert werden. Dies wird noch Jahre dauern. Daher brauchen wir (erst) in dieser Zwischenphase einen Leitfaden.
7. Dieser Leitfaden sollte sehr bald (bis Juli 2019) verfügbar sein, um den Herstellern schnell als Orientierung zu dienen und ihnen ein sofortiges Handeln zu ermöglichen. Die hohe Entwicklungsgeschwindigkeit macht Kompromisse bei der Harmonisierung mit den meisten Parteien unvermeidlich.
8. Der technologische Fortschritt im Bereich der künstlichen Intelligenz ist immens. Es werden fortlaufend neue Verfahren und Technologien veröffentlicht. Ein Leitfaden sollte einerseits so spezifisch wie möglich sein. Andererseits kann er nicht so spezifisch auf ein Verfahren oder eine Technologie ausgerichtet sein, um eine sinnvolle „Lebensdauer“ zu erreichen. Daher muss ein Leitfaden allgemeine Konzepte behandeln. Er kann jedoch nicht den Anspruch auf Vollständigkeit erheben.
9. Ein solcher Leitfaden muss die Besonderheiten von Medizinprodukten berücksichtigen, wozu die Grundsätze der Patientensicherheit (Safety) und ein risikobasierter Ansatz gehören. Im konkreten Fall werden ausgewählte Maßnahmen zur Informationssicherheit („Controls“) im Widerspruch zu den grundlegenden Anforderungen stehen. Aus diesem Grund kann es keine festgelegte Liste von „Controls“ für Medizinprodukte geben. Die vom Hersteller festgelegte Zweckbestimmung des Produkts ist entscheidend.
10. Für den gewünschten positiven Einfluss eines Leitfadens auf die Sicherheit KI-basierter Medizinprodukte ist die einfache Verständlichkeit und Praktikabilität wesentlich. Daher muss es möglichst wenig abstrakte oder „hochrangige“ Anforderungen, sondern „binär entscheidende“ Prüfkriterien geben.
11. Um die Praktikabilität zu erhöhen, haben die Autoren es weitestgehend vermieden, viele Anforderungen zusammenzufassen. Sie haben sich vielmehr auf diejenigen beschränkt, die sie für besonders relevant und umsetzbar halten.
12. Um die Verbreitung und den Bekanntheitsgrad zu fördern, muss die Richtlinie außerdem kostenlos verfügbar sein und bleiben.
13. Die Richtlinie sollte auf Deutsch und Englisch verfügbar sein.