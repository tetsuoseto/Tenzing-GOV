##########
>white|orangered|left|14|30|hr Abschnitt 3.2
### 3.2. Risikomanagementpraktiken
>white|orangered|left|24|30|hb Risikomanagementpraktiken

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Wichtige Informationen
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Das Risiko-Management für Allzweck-KI umfasst eine Reihe von Vorgehensweisen zur Identifizierung, Bewertung und Reduzierung von Risiken durch Allzweck-KI. Dazu gehören Modell-Tests und -Evaluierungen auf Modell-Ebene (wie „Red-Teaming“), organisatorische Prozesse, die Entwicklungs- und Freigabeentscheidungen steuern, bedingte Schutzmaßnahmen (wie „if-then“-Verpflichtungen) sowie Vorfallmeldungen.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Mehrere KI-Entwickler haben Frontier-KI-Sicherheitsrahmenwerke erstellt. Diese Rahmenwerke enthalten Informationen zu Risikoanalysen und legen bedingte Maßnahmen fest, wie z. B. Zugriffsrestriktionen, die Unternehmen für leistungsfähigere Modelle einführen wollen. Sie unterscheiden sich darin, welche Risiken abgedeckt werden, wie sie Fähigkeits-Schwellenwerte definieren und welche Maßnahmen ausgelöst werden, wenn diese Schwellenwerte erreicht sind.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Die Evidenz zur realen Wirksamkeit von KI-Risikomanagementpraktiken bleibt begrenzt. Das Fehlen von Vorfallmeldungen und Monitoring erschwert die Einschätzung, wie gut die aktuellen Praktiken Risiken reduzieren, und wie konsequent sie umgesetzt werden.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Seit der Veröffentlichung des letzten Berichts (Januar 2025) ist das Risikomanagement durch neue Branchen- und Governance-Initiativen strukturierter geworden. Neue Instrumente wie der EU-Verhaltenskodex für KI mit allgemeinem Zweck, der KI-Sicherheits-Governance-Rahmen 2.0 in China und der G7-Berichtsrahmen des Hiroshima-KI-Prozesses zeigen zusammen mit unternehmensgeleiteten Initiativen den Trend hin zu stärker standardisierten Ansätzen für Transparenz, Bewertung und die Meldung von Vorfällen.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Marktdynamiken und das Tempo der KI-Entwicklung stellen zusätzliche Herausforderungen dar. Aufgrund des Wettbewerbsdrucks könnten KI-Unternehmen Zielkonflikte zwischen schnelleren Produkteinführungen und Investitionen in Maßnahmen zur Risikominderung haben. Viele KI-bezogene Schäden werden zudem externalisiert, und die rechtliche Haftung dafür bleibt unklar, während Governance-Prozesse möglicherweise nur langsam auf Veränderungen in der KI-Landschaft reagieren können.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Zu den zentralen Herausforderungen für politische Entscheidungsträger gehört es, Prioritäten zwischen den vielfältigen Risiken zu setzen, die durch General-Purpose-AI entstehen, und zu klären, welche Akteure entlang der gesamten AI-Wertschöpfungskette am besten positioniert sind, um diese Risiken zu mindern. Diese Herausforderungen werden durch begrenzte Transparenz darüber verstärkt, wie Risiken in der Praxis identifiziert, bewertet und gesteuert werden, sowie durch die Aufspaltung des Informationsaustauschs zwischen Entwicklern, Betreibern und Anbietern von Infrastruktur.
>oldlace|black||11|15|br      


Das Risikomanagement für KI umfasst eine Reihe von Maßnahmen, die darauf abzielen, Risiken im Zusammenhang mit KI-Systemen zu identifizieren, zu bewerten und die Wahrscheinlichkeit und Schwere dieser Risiken zu reduzieren. Diese Maßnahmen können von KI-Entwicklern, Betreibern, Evaluatoren und Regulierungsbehörden umgesetzt werden. Beispiele sind Threat Modeling, Risk Tiering, Red-Teaming, Auditing und Incident Reporting. Dieser Abschnitt beschreibt aktuelle Risikomanagement-Praktiken, neue Entwicklungen und verbleibende Einschränkungen.

Seit Beginn 2025 haben sich mehrere neue internationale Initiativen für das Risikomanagement von General-Purpose-KI entwickelt, darunter organisatorische Transparenz- und Risikoberichts-Frameworks sowie regulatorische- und Governance-Frameworks.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Abbildung 3.4: Vier Komponenten des Risikomanagements
>white|black||9|11|br Die vier Kategorien von Methoden für das Risikomanagement bei Allzweck-KI: Risikenermittlung; Risikoanalyse und -bewertung; Risikominderung; und Risikogovernance. Diese bilden einen iterativen und zyklischen Prozess. Die Risikogovernance, dargestellt in der Mitte, erleichtert den Erfolg der anderen Komponenten. Quelle: International AI Safety Report 2026.


Zu den verbleibenden Herausforderungen gehören eine begrenzte Standardisierung, die die Einhaltung und Bewertung erschwert, sowie ein begrenzter Nachweis hinsichtlich der Wirksamkeit im realen Einsatz. Darüber hinaus unterscheiden sich die institutionellen, kulturellen und politischen Rahmenbedingungen weltweit, was bedeutet, dass sich die Vorgehensweisen zur Identifizierung und zum Management von Risiken, einschließlich akzeptabler Risikoschwellen, je nach Region unterscheiden können. Die Diskussion der Risikomanagementansätze in diesem Abschnitt ist beschreibend: Sie soll die Akteure im KI-Ökosystem über die derzeitigen globalen Ansätze zum Risikomanagement informieren. Sofern verfügbar, wird die Evidenz zur Wirksamkeit und zu den Grenzen dieser Ansätze erörtert, jedoch liegen politische Empfehlungen außerhalb des Geltungsbereichs dieser Arbeit.

###@ Komponenten des Risikomanagements

Risikomanagement ist ein iterativer Prozess mit Praktiken und Methoden, die den gesamten Lebenszyklus der Entwicklung und Bereitstellung von KI abdecken, jedoch kohärent zusammenwirken (‡969). Risikomanagement für allgemeine KI kann Rollen für eine Vielzahl von Akteuren umfassen, darunter Datenwissenschaftler, Modellingenieure, Auditoren, Domänenexperten, Führungskräfte, Endnutzer, betroffene Gemeinschaften, Drittanbieter, politische Entscheidungsträger, Regierungen, Organisationen für Standards sowie Organisationen der Zivilgesellschaft (‡970, ‡971, ‡972). Führende Risiko-Management-Standards sind häufig interoperabel, verwenden jedoch unterschiedliche Terminologie, um die Elemente des Risikomanagements zu beschreiben (‡973, ‡974). Sie haben typischerweise vier miteinander verbundene Komponenten (Abbildung 3.4): Risiken identifizieren; analysieren und bewerten; Risiken mindern; und das Risikomanagement steuern (‡970, ‡973, ‡975, ‡976). Die Tabellen unten geben beispielhafte Beispiele für relevante Methoden, Techniken und Tools. Die Praktiken entwickeln sich weiter, sodass die Tabellen nicht vollständig sind und die Anwendbarkeit je nach Kontext variieren wird.

###@ Risikidentifikation

Risikenermittlung ist der Prozess, Risiken zu finden, zu erkennen und zu beschreiben. Umfassende Risikenermittlung umfasst typischerweise fähigkeitsgesteuerte Bewertungen, die testen, ob Modelle über bestimmte gefährliche Fähigkeiten (‡977) verfügen, sowie Risikomodellierung (‡978) und Prognostizierung (‡715*), die verwendet werden, um bestehende und sich abzeichnende Risiken zu untersuchen. Tabelle 3.1 stellt verschiedene Beispiele für Risikenermittlungspraktiken bereit. Die Risikenermittlung greift außerdem auf die Einbindung relevanter Expertinnen und Experten sowie Communities zurück, um den größeren Kontext zu verstehen, wie Risiken entstehen (‡979, ‡980). Mechanismen wie Bug-Bounty-Programme können diesen Prozess unterstützen, indem sie die Identifizierung zuvor unbekannter Schwachstellen (‡981) incentivieren (Tabelle 3.1). Ein zentrales Ziel der Risikenermittlung ist es, sowohl bekannte, gut verstandene Risiken als auch potenzielle zukünftige Risiken zu berücksichtigen, die weiterhin unsicher oder nur unzureichend charakterisiert sind (‡982). Dies ist besonders wichtig für General-Purpose-AI, bei der viele Risiken möglicherweise noch nicht vollständig verstanden oder beobachtbar sind (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bug-Bounty-Programme
  Bug Bounties oder Programme zur Meldung von Sicherheitslücken schaffen Anreize für Personen, Schwachstellen in KI-Systemen zu finden und zu melden. Mehrere Entwickler haben Bug-Bounty-Programme implementiert (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Expertenberatung
  Fachleute aus dem jeweiligen Bereich, Nutzer und betroffene Gemeinschaften liefern Einblicke in wahrscheinliche Risiken. Es gibt neue Leitlinien für partizipative und inklusive KI (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Fischgräten-(Ishikawa)-Diagramm
  Fischgräten-Diagramme sind etablierte Werkzeuge zur Ursachenanalyse, und Forschende haben vorgeschlagen, sie für eine strukturierte Analyse von Vorfällen mit KI-Risiken zu verwenden (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Prognose
  Prognose ist der Prozess des Vorhersagens zukünftiger Ereignisse oder Trends auf der Grundlage der Analyse von vergangenen und aktuellen Daten. Sie wurde verwendet, um die relative Wahrscheinlichkeit von beispielsweise unterschiedlichen wirtschaftlichen Ergebnissen aufgrund fortschrittlicher KI zu vergleichen (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risikotaxonomie
  Risikotaxonomien sind eine Möglichkeit, Risiken über mehrere Dimensionen hinweg zu kategorisieren und zu organisieren. Es gibt mehrere, die Risiken aus General-Purpose-KI (‡906, ‡988) darstellen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Szenarioplanung
  Szenarioplanung beinhaltet die Entwicklung plausibler zukünftiger Szenarien und die Analyse, wie sich Risiken manifestieren. Dies wurde verwendet, um die Risiken und Auswirkungen von KI-Modellen zu untersuchen (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bedrohungsmodellierung
  Threat-Modeling ist ein Prozess zur Identifizierung von Bedrohungen und Schwachstellen für ein System. Zahlreiche KI-Entwickler heben den Einsatz von Threat-Modeling hervor, um potenzielle Missbrauchsszenarien von KI-Systemen vorherzusehen (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabelle 3.1: Beispiele zur Risikoidentifikation im Allgemeinen AI-Risikomanagement für Allzweck-AI
>white|black||9|11|br Beispielmethoden zur Identifizierung von KI-Risiken, alphabetisch aufgelistet. Die Methoden umfassen
sind so konzipiert, die Risikoidentifikation für viele verschiedene Risikotypen zu unterstützen, einschließlich Risiken aus böswilliger Verwendung, Risiken aus Fehlfunktionen und systemischen Risiken. Angesichts der noch frühen Entwicklung des Risikomanagements für allgemeine KI sind nicht alle Methoden für jeden KI-Entwickler oder -Betreiber geeignet.


>white|orangered|left|14|15.5|bb Bedrohungsmodellierung und Risikoklassifikationen sind bedeutende Methoden der Risikenermittlung.

Zwei bedeutende Methoden zur Identifizierung der Risiken von allgemeiner Zweck-KI sind Threat Modeling (International AI Safety Report 2026) (ein strukturierter Prozess, der abbildet, wie sich KI-bezogene Risiken möglicherweise materialisieren) und Risikoklassifikationen. Meta verwendet beispielsweise Threat-Modeling-Übungen, um potenzielle Missbrauchsszenarien ihrer KI-Modelle zu antizipieren (‡990), und Anthropic führt Threat Modeling als Teil seines ASL-3 Deployment Standard (‡991) aus. KI-Risiko- und Gefahrentaxonomien, die Risikokategorien und Beispiele auflisten, können ebenso als Ausgangspunkt dienen, um die wesentlichen Risiken, die mit allgemeiner Zweck-KI in spezifischen Anwendungsdomänen verbunden sind, zu konzeptualisieren, zu identifizieren und zu spezifizieren (‡906, ‡988, ‡992, ‡993).

###@ Risikobewertung und -analyse

Risikobewertung und -evaluation ist der Prozess der Bestimmung des Risikoniveaus eines KI-Modells oder -Systems und des Vergleichs mit festgelegten Kriterien, um die Zulässigkeit zu bewerten oder die Notwendigkeit von Gegenmaßnahmen festzustellen (‡994, ‡995, ‡996, ‡997). Dazu gehören Praktiken wie das Messen der Modellleistung anhand von Benchmarks (‡998) und Evaluierungen (‡176, ‡715), die Durchführung von Red-Teaming-Übungen (‡999*), Folgenabschätzungen (‡1000) und Audits (‡1001, ‡1002). Siehe Tabelle 3.2 für Beispiele einer allgemeinen Risikoanalyse und -evaluation für KI mit allgemeinem Verwendungszweck. Die Methoden sind darauf ausgelegt, Analysen und Evaluierungen für viele unterschiedliche Risikotypen gleichzeitig zu unterstützen.

Die zentralen Ziele der Risikoanalyse und -bewertung sind, Bewertungen der Modellfähigkeiten und -verwundbarkeiten durchzuführen (‡1003), robuste Risikomodellierung zu nutzen, um Entscheidungen über Risikoschwellen zu informieren (‡1004, ‡1005), und zu verstehen, wie KI-Systeme in der Praxis eingesetzt werden, um nachgelagerte gesellschaftliche Auswirkungen zu bewerten (‡869, ‡904, ‡905, ‡1006). Risikoanalyse- und Bewertungsprozesse gelten häufig als eher geeignet, Risiken zu identifizieren, wenn sie eine unabhängige Überprüfung einbeziehen (‡1001, ‡1007), auf Fachwissen aus verschiedenen Branchen zurückgreifen (‡1008) und unterschiedliche Perspektiven aus mehreren Domänen und Disziplinen sowie aus betroffenen Gemeinschaften einbeziehen (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Audits
  Audits sind formale Überprüfungen der Leistung und Auswirkungen von KI-Modellen und/ oder der Compliance einer Organisation mit Standards, Richtlinien und Verfahren, die intern oder durch eine externe Partei durchgeführt werden. KI-Auditing ist ein wachsendes Fachgebiet, und es gibt zahlreiche Tools und Verfahren zum Auditing von KI-Modellen sowie der Praktiken von KI-Modellentwicklern (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Benchmarks
  Benchmarks sind standardisierte, oft quantitative Tests oder Kennzahlen, die verwendet werden, um die Leistung von KI-Systemen auf einer festen Menge von Aufgaben zu bewerten und zu vergleichen, die dafür ausgelegt ist, reale Nutzung abzubilden (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bowtie-Methode
  Die Schleifchenmethode ist eine bekannte Methode zur Visualisierung, an welchen Stellen Kontrollen hinzugefügt werden können, um Risikoevents abzumildern. Sie ermöglicht eine klare Unterscheidung zwischen proaktivem und reaktivem Risikomanagement (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Delphi-Methode
  Die Delphi-Methode ist eine Gruppenentscheidungs-Technik, die eine Reihe von Fragebögen verwendet, um einen Konsens von einem Gremium von Experten zu erheben (‡1020, ‡1021). Sie wurde eingesetzt, um dabei zu helfen, mögliche Zukunftsszenarien mit fortgeschrittener KI zu erkunden (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Feldtest
  Feldtests bewerten die Leistung und die Auswirkungen eines KI-Systems in einer realen, operativen Umgebung. Einige Forschungen betonen Feldtests als Ergänzung zur Modellbewertung, um reale Ergebnisse und Konsequenzen zu bewerten (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Auswirkungsanalyse
  Wirkungsabschätzungen bewerten die potenziellen Auswirkungen einer Technologie oder eines Projekts. Dazu kann gehören, Auswirkungen zu quantifizieren, zu aggregieren und zu priorisieren. Das EU AI Act verlangt beispielsweise von Entwicklern von KI-Systemen mit hohem Risiko, Fundamental Rights Impact Assessments (‡1024) durchzuführen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modelbewertung
  Modelbewertungen umfassen Prozesse und Tests, um die Leistung eines KI-Modells für eine bestimmte Aufgabe zu bewerten und zu messen. Es gibt zahlreiche KI-Evaluierungen, um unterschiedliche Fähigkeiten und Risiken zu beurteilen, einschließlich für Sicherheit, Sicherheitsschutz und sozialen Einfluss (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Probabilistische Risikoanalyse
  Probabilistische Risikoanalyse ist eine Methodik zur Bewertung von Risiken im Zusammenhang mit komplexen Systemen oder Prozessen, die Unsicherheit berücksichtigt. Sie wurde für fortgeschrittene KI-Systeme angepasst (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Red-Teaming
  Red-Teaming ist eine Übung, bei der eine Gruppe von Personen oder automatisierten Systemen vorgibt, ein Gegner zu sein, und die technologischen Systeme einer Organisation angreift, um Schwachstellen zu identifizieren. Zahlreiche KI-Unternehmen haben interne Praktiken zum Red-Teaming von KI-Systemen (‡458, ‡1028). Red-Teaming kann auch von Akteuren außerhalb von Unternehmen durchgeführt werden. Diese Teams stehen vor Herausforderungen wie einem eingeschränkten Zugang, können aber auch eigenständige Erkenntnisse zutage fördern (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risikomatrizen
  Risikomatrizen sind ein visuelles Hilfsmittel, um Risiken anhand ihrer Eintrittswahrscheinlichkeit und ihres potenziellen Einflusses zu priorisieren (‡1027). Einige KI-Entwickler fügen ihren Frontier-AI-Safety-Frameworks grundlegende Risikomatrizen hinzu (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risikogrenzen / Risikostufen
  Risikogrenzen oder -stufen sind quantitative oder qualitative Schwellenwerte, die akzeptierbare von nicht akzeptierbaren Risiken unterscheiden und bei Überschreitung spezifische Maßnahmen des Risikomanagements auslösen. Bei allgemeinem Zweck-KI werden sie durch eine Kombination aus Fähigkeiten, Auswirkung, Rechenleistung, Reichweite und weiteren Faktoren bestimmt (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risikotoleranz
  Risikotoleranz bezeichnet das Ausmaß an Risiko, das eine Organisation bereit ist zu akzeptieren. In der KI werden Risikotoleranzen häufig implizit durch Unternehmensrichtlinien und -praktiken festgelegt, während einige regulatorische Rahmenwerke ausdrücklich nicht akzeptierbare Risiken definieren und rechtliche Konsequenzen daran knüpfen (‡1032). Einige Unternehmen beschreiben ihre Risikotoleranz in Bezug auf das marginale Risiko eines neuen Modells; das heißt, in welchem Ausmaß ein Modell das Risiko kontrafaktisch über das hinaus erhöht, das bereits durch bestehende Modelle oder andere Technologien verursacht wird (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sicherheitsfälle
  Ein Safety Case ist ein strukturierter Argumentationsnachweis, der durch Nachweise gestützt wird und darlegt, dass ein System in einem bestimmten Kontext akzeptabel sicher betrieben werden kann. Aktuelle Literatur (‡1037, ‡1038, ‡1039) hat Safety Cases für Frontier AI-Systeme und bestimmte Frontier AI Safety Frameworks untersucht, die sie anführen (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb System- Sicherheitsanalyse
  System-Sicherheitsanalyse hebt Abhängigkeiten zwischen Komponenten und dem System, zu dem sie gehören, hervor, um vorherzusehen, wie systemweite Gefährdungen aus Ausfällen von Komponenten oder Prozessen oder aus Interaktionen zwischen Subsystemen, menschlichen Faktoren und Umweltbedingungen entstehen können. In der Literatur angewandte Ansätze für KI-Systeme umfassen die systemtheoretische Prozessanalyse (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabelle 3.2: Risikoanalyse/-bewertung im Allgemeinen Rahmen für das Risikomanagement bei General-Purpose-KI
>white|black||9|11|br Beispielmethoden für die KI-Risikoanalyse/-bewertung, alphabetisch aufgelistet. Aufgrund der noch jungen Natur des Risikomanagements für KI mit allgemeinem Zweck werden nicht alle Methoden für jeden KI-Entwickler oder -Betreiber geeignet sein.


>white|orangered|left|14|15.5|bb Zu den gängigen Werkzeugen der Risikoanalyse gehören Benchmarks und Modellevaluierungen

Benchmarks und Modellbewertungen sind standardisierte Tests, um die Leistungsfähigkeit von Allzweck-KI-Systemen bei bestimmten Aufgaben zu beurteilen. Forschende haben eine breite Palette von Benchmarks und Bewertungen entwickelt, darunter Sammlungen anspruchsvoller Multiple-Choice-Fragen, Software-Engineering-Probleme und arbeitsbezogene Aufgaben in simulierten Büro-Umgebungen (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Bewertungsverfahren für schädliche Fähigkeiten (‡715) werden eingesetzt, um zu prüfen, ob ein Allzweck-KI-Modell oder -System besonders gefährliches Wissen oder besondere Fertigkeiten besitzt, wie z. B. die Fähigkeit, bei Cyberangriffen zu helfen (siehe §2.1.3. Cyberangriffe).

Hochfolgende Entscheidungen von Unternehmen und Regierungen über Modellfreigaben stützen sich teilweise auf diese Bewertungen (‡1050, ‡1051, ‡1052). Allerdings variieren Benchmarks erheblich in Qualität und Umfang (‡998, ‡1003), und es kann schwierig sein, ihre Gültigkeit einzuschätzen, da zahlreiche Mängel in den Benchmarking-Praktiken vorliegen (‡902, ‡909, ‡1003, ‡1053*). Beispielsweise können Benchmarks „gesättigt“ werden – wenn die Punktzahlen vieler Modelle sich dem Top-Wert annähern – was bedeutet, dass sie die Modelle nicht mehr deutlich voneinander unterscheiden. Modelle sind außerdem zunehmend wahrscheinlicher, bestimmte Aufgaben als Bewertungen zu erkennen und in Auswertungskontexten andere Verhaltensweisen zu zeigen als bei ähnlichen Aufgaben in Einsatzkontexten, aufgrund von „situational awareness“ (siehe §2.2.2. Verlust der Kontrolle). Schließlich haben Benchmarks und Bewertungen gut dokumentierte Grenzen: Insbesondere erfassen sie nicht die Risiken, die mit dem Einsatz von Allzweck-KI in neuen Domänen und für neuartige Aufgaben verbunden sind, da sich die Testbedingungen in unterschiedlichem Maß vom realen Einsatz unterscheiden (‡913) (siehe §1.2. Aktuelle Fähigkeiten und §3.1. Technische und institutionelle Herausforderungen).

>white|orangered|left|14|15.5|bb Red-Teaming ermöglicht genauere, domänenspezifische Bewertungen des Risikos

Eine weitere gängige Methode zur Bewertung von Risiken ist Red-Teaming. Ein „Red Team“ ist eine Gruppe von Gutachtern, die damit beauftragt ist, nach Schwachstellen, Einschränkungen oder dem Missbrauchspotenzial zu suchen. Red-Teaming kann domänenspezifisch sein und von Domänenexperten durchgeführt werden, oder offen angelegt werden, um neue Risikofaktoren zu untersuchen. Beispielsweise könnte ein Red Team „Jailbreaking“-Angriffe untersuchen, die die Sicherheitsbeschränkungen des Modells unterlaufen (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). Im Gegensatz zu Benchmarks ist ein wesentlicher Vorteil von Red-Teaming, dass Red Teams ihre Bewertungen an das jeweilige zu testende System anpassen können. Beispielsweise können Red Teams benutzerdefinierte Eingaben entwerfen, um Worst-Case-Verhalten, Möglichkeiten für bösartige Nutzung und unerwartete Ausfälle zu identifizieren. Allerdings kann dafür ein spezieller Zugriff auf Modelle erforderlich sein, und es kann sein, dass wichtige Risikokategorien nicht sichtbar werden (‡999, ‡1028).

Wichtig ist, dass das Fehlen identifizierter Risiken nicht bedeutet, dass diese Risiken niedrig sind: Frühere Arbeiten zeigen, dass Fehler häufig der Erkennung entgehen, insbesondere wenn Red Teams nur begrenzten Zugriff oder begrenzte Ressourcen haben (‡1060). Die Forschung hat außerdem in Frage gestellt, ob Red-Teaming verlässliche und reproduzierbare Ergebnisse hervorbringen kann (‡1061). Die Zusammensetzung des Red Teams und die den Red Teamern bereitgestellten Anweisungen (‡1062), die Anzahl der Angriffsrunden (‡1063) sowie der Zugriff des Modells auf Werkzeuge (‡1064, ‡1065) können die Ergebnisse erheblich beeinflussen, einschließlich der abgedeckten Angriffsfläche. Um einige dieser Herausforderungen zu adressieren, zielen umfassende Leitlinien zum Red-Teaming darauf ab, (‡1066).

###@ Risikominderung

Risikominderung ist der Prozess der Priorisierung, Bewertung und Implementierung von Kontrollen und Gegenmaßnahmen, um identifizierte Risiken zu reduzieren. Beispiele sind Zugriffskontrollen (‡991), kontinuierliches Monitoring (‡986) und Wenn-dann-Verpflichtungen (‡700). Die Risikominderung wirft eine zentrale Frage auf: welches akzeptable Risikoniveau ist zulässig? Jüngste Frameworks und Unternehmensrichtlinien haben begonnen, Kriterien für die formale „Risikobewilligung“ (‡965, ‡1040) festzulegen. Allerdings bleibt die Festlegung geeigneter Schwellenwerte herausfordernd, insbesondere für Risiken mit weitreichenden gesellschaftlichen Auswirkungen (‡986, ‡1067). Gegenwärtig existiert kein etabliertes Mechanismus zur Validierung von Risikobewilligungsentscheidungen, die von Entwicklerinnen und Entwicklern vor der Veröffentlichung getroffen wurden (‡1005).

Die in Tabelle 3.3 unten beschriebenen Methoden zur Risikominderung sind anpassbar und können eine Reihe von Risiken mindern, einschließlich einiger unerwarteter Risiken. Die Tabelle enthält keine technischen Methoden zur Risikominderung wie adversarial training, Inhaltsfilter und chain-of-thought monitoring. Diese werden in §3.3 behandelt, Technische Schutzmaßnahmen und Überwachung, sowie im gesamten Bericht in den Abschnitten „Mitigations“ für jedes Risiko in §2. Risks.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Richtlinien zur zulässigen Nutzung
  Eine Nutzungsrichtlinie für einen akzeptablen Gebrauch ist eine Sammlung von Regeln und Leitlinien für die verantwortungsvolle, ethische und rechtmäßige Nutzung von KI-Modellen. Es ist üblich, dass KI-Entwickler bei neuen Modellveröffentlichungen (‡1068, ‡1069) Nutzungsrichtlinien für einen akzeptablen Gebrauch sowie Richtlinien für verbotene Nutzungen veröffentlichen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Zugriffskontrolle/Benutzerrisikoprüfung
  Zugriffssteuerungen beinhalten die Verwendung von Richtlinien und Regeln, um den Zugriff auf KI-Modelle, Daten und Systeme anhand von Benutzerrollen, Attributen und anderen Bedingungen einzuschränken, um nicht autorisierte Nutzung, Manipulation oder Datenverletzungen zu verhindern. KI-Unternehmen deaktivieren häufig Konten, die als an kriminellen Aktivitäten beteiligt gefunden werden (‡486), und führen eine Benutzerrüfung sowie Know-Your-Customer-Überprüfungen durch, um sicherzustellen, dass die Modelle nur von vertrauenswürdigen Akteuren verwendet werden (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Verhaltens-/Modellspezifikation
  Eine Verhaltensspezifikation für KI ist ein Dokument, das festlegt, wie sich ein KI-Modell in verschiedenen Situationen verhalten soll. Sie dient als Blaupause für KI-Alignment und -Sicherheit und steuert die Modellentwicklung, das Training, die Evaluierung und die Ausgaben. Mehrere KI-Unternehmen verwenden Modell-Spezifikationsdokumente und machen zumindest Teile davon öffentlich (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kontinuierliches Monitoring
  Kontinuierliches Monitoring ist der fortlaufende, automatisierte Prozess des Beobachtens, Analysierens und Kontrollierens von eingesetzten KI-Systemen, bei dem ihre Leistung überwacht und ihr Verhalten so begrenzt wird, dass Zuverlässigkeit, Wirksamkeit und Sicherheit gewährleistet sind. Es gibt zahlreiche Werkzeuge für kontinuierliches Monitoring (‡1073*) sowie Techniken zur Unterstützung
KI-Beobachtbarkeit (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Verteidigung in der Tiefe
  Verteidigung in der Tiefe ist die Idee, dass mehrere unabhängige und sich überlappende Verteidigungsschichten implementiert werden können, sodass, wenn eine ausfällt, die anderen weiterhin wirksam sind (‡1075, ‡1076). Mehrere Frontier-AI-Sicherheitsframeworks beziehen sich darauf (z. B. (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ökosystemüberwachung
  Dies ist der Prozess der Überwachung des breiteren KI-Ökosystems, einschließlich der Nachverfolgung von Compute und Hardware, der Modellherkunft, der Datenherkunft und der Nutzungsmuster. Die Forschungsliteratur behandelt eine solche Überwachung im Zusammenhang mit Risiken durch KI für allgemeine Zwecke (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb If-then-Verpflichtungen
  Wenn-dann-Zusagen sind eine Reihe technischer und organisatorischer Protokolle sowie Zusagen zur Steuerung von Risiken, während KI-Modelle leistungsfähiger werden. Mehrere KI-Entwickler verwenden diese Arten von Zusagen als Teil ihrer Frontier- KI-Sicherheits-Frameworks (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rote Linien oder Verbote
  Rote Linien sind spezifische Grenzen, die als Fähigkeiten, Auswirkungen oder Nutzungsarten ausgedrückt werden. Der Begriff taucht in öffentlichen Stellungnahmen und Initiativen auf, ebenso wie in regulatorischen Verboten (‡1079, ‡1080, ‡1081). Die Literatur weist außerdem auf Einschränkungen von Ansätzen mit roten Linien hin, einschließlich Herausforderungen in Bezug auf Konsens und Durchsetzbarkeit.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Freigabe- und Bereitstellungsstrategien
  Release- und Bereitstellungsstrategien für Allzweck-KI können die Verwendung gestufter Releases oder den Zugriff über eine API einschließen, sodass im Falle von Missbrauch oder unerwarteten Schäden mehr Eindämmungsoptionen zur Verfügung stehen (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabelle 3.3: Risikominimierung im Risikomanagement von Allzweck-KI
>white|black||9|11|br Beispielmethoden zur Minderung von KI-Risiken sind alphabetisch aufgelistet. Die enthaltenen Methoden sind so ausgelegt, dass sie die Risikominderung für viele unterschiedliche Risikotypen gleichzeitig unterstützen, einschließlich Risiken aus böswilliger Nutzung, Risiken aus Fehlfunktionen und systemischen Risiken. Aufgrund der noch frühen Entwicklung des Risikomanagements für KI mit allgemeinem Zweck sind nicht alle Methoden für jeden KI-Entwickler oder KI-Betreiber geeignet.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Abbildung 3.5: Ein „Swiss-cheese-Diagramm“, das den Defence-in-Depth-Ansatz veranschaulicht
>white|black||9|11|br Mehrere Schichten von Abwehrmaßnahmen können Mängel in einzelnen Schichten ausgleichen. Aktuelle Risikomanagement-Techniken für KI haben Schwächen, aber ihre Kombination in Schichten kann einen deutlich stärkeren Schutz gegen Risiken bieten. Quelle: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Defense-in-Depth und Release-Strategien sind wichtige Minderungsmaßnahmen

Ein „defence-in-depth“-Modell kann ein allgemeines Risikomanagement für KI unterstützen. In diesem Zusammenhang bezieht sich „defence-in-depth“ auf eine Kombination aus technischen, organisatorischen und gesellschaftlichen Maßnahmen, die über verschiedene Phasen der Entwicklung und Bereitstellung hinweg angewendet werden (Abbildung 3.5). Das bedeutet, dass mehrere Schichten unabhängiger Schutzvorkehrungen geschaffen werden: Wenn eine Schicht versagt, können andere Schichten die Schadensvermeidung dennoch gewährleisten. Ein häufig genanntes Beispiel für ein defence-in-depth-Modell ist die Palette vorbeugender Maßnahmen, die eingesetzt werden, um Infektionskrankheiten zu verhindern. Impfungen, Masken und Händewaschen sowie andere Maßnahmen können das Risiko einer Infektion in Kombination erheblich senken, obwohl keine dieser Methoden für sich allein zu 100% wirksam ist (‡1083*). Für allgemeine KI umfasst defence-in-depth Kontrollen, die nicht auf dem KI-Modell selbst liegen, sondern auf dem breiteren Ökosystem. Dazu gehören beispielsweise Kontrollen der Materialien, die für die Durchführung eines biologischen Angriffs erforderlich sind, wie Reagenzien (‡1084, ‡1085). Allerdings adressieren defence-in-depth-Maßnahmen primär Risiken im Zusammenhang mit Unfällen, Fehlfunktionen und böswilliger Nutzung und können bei der Steuerung systemischer Risiken eine geringere Rolle spielen (siehe §3.5. Aufbau gesellschaftlicher Resilienz).

Die Veröffentlichungs- und Einsatzstrategie eines Unternehmens ist ein wichtiger Bestandteil der Risikominderung. Entscheidungen darüber, wie Modelle den Nutzern bereitgestellt werden, können das Risikoprofil erheblich beeinflussen (‡1082). Zu den unterschiedlichen Optionen für Veröffentlichung und Bereitstellung gehören gestaffelte Freigaben an begrenzte Nutzergruppen, der Zugang über kontrollierte Online-Dienste (wie APIs) sowie der Einsatz von Lizenzvereinbarungen und Richtlinien zur zulässigen Nutzung, die bestimmte schädliche Anwendungen rechtlich verbieten (‡176, ‡1086, ‡1087). §3.4. Open-Weight-Modelle erörtert ausführlicher, wie sich die Veröffentlichung von Modellgewichten auf Risiken auswirkt.

###@ Risikogovernance

Risikogovernance ist der Prozess, durch den Risikomanagement-Bewertungen, Entscheidungen und Maßnahmen mit der Strategie und den Zielen einer Organisation oder einer anderen Einheit verknüpft werden (‡1088, ‡1089). Tabelle 3.4 gibt einen Überblick über gängige Techniken der Risikogovernance. Wie in Abbildung 3.4 dargestellt, kann Risikogovernance als das Kernstück des Risikomanagements verstanden werden, da sie den effektiven Betrieb der übrigen Komponenten des Risikomanagements ermöglicht. Sie schafft Verantwortlichkeit, Transparenz und Klarheit, die fundierte Entscheidungen im Risikomanagement unterstützen. Risikogovernance kann Verfahren wie das Melden von Vorfällen (‡1090), die Zuweisung von Risikoverantwortlichkeiten (‡965) und den Schutz von Hinweisgebern (‡1091) umfassen. Umfassender kann Risikogovernance auch Leitlinien, Rahmenwerke, Gesetzgebung, Regulierung, nationale und internationale Standards sowie Trainings- und Bildungsinitiativen einschließen. Ein zentrales Ziel der Risikogovernance ist es, Organisationsrichtlinien und -mechanismen festzulegen, die verdeutlichen, wie Risikomanagement-Verantwortlichkeiten über eine Organisation oder eine andere Einheit hinweg zugewiesen werden, um eine angemessene Aufsicht und Verantwortlichkeit zu unterstützen (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dokumentation
  Dokumentationspraktiken helfen dabei, wichtige Informationen über KI-Systeme nachzuverfolgen, wie etwa Trainingsdaten, Designentscheidungen, beabsichtigte Verwendungen, Einschränkungen und Risiken. „Model Cards“ und „System Cards“, die Informationen darüber bereitstellen, wie ein KI-Modell oder -System trainiert und evaluiert wurde, sind Beispiele für bedeutende bewährte Verfahren der KI-Dokumentation (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vorfallmeldung
  Incident Reporting ist der Prozess, bei dem Fälle, in denen die Entwicklung oder Bereitstellung von KI direkt oder indirekt zu Schaden geführt hat, systematisch dokumentiert und geteilt werden. Es gibt mehrere Plattformen, die Incident Reporting für KI erleichtern (‡1096, ‡1097), sowie Frameworks, die ein effektiveres Incident Reporting für KI unterstützen (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risikomanagement-Frameworks
  Risikomanagement-Frameworks sind organisatorische Pläne, um Lücken in der Risikodeckung zu reduzieren, verschiedene Risikomanagement-Aktivitäten zu koordinieren und Kontrollen und Gegenmaßnahmen umzusetzen. Frameworks, die speziell für allgemeinzweckliche KI (‡986, ‡1098) entwickelt wurden, verweisen häufig auf die anderen in diesem Abschnitt genannten Maßnahmen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risikoregister
  Ein Risikoregister ist ein Verzeichnis verschiedener Risiken, ihre Priorisierung, Zuständigkeiten und Minderungspläne. Diese sind relativ in vielen Branchen üblich, einschließlich Cybersicherheit (‡1099), und werden manchmal verwendet, um regulatorische Compliance-Anforderungen zu erfüllen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risikoverantwortungszuweisung
  Die Zuweisung von Rollen und Verantwortlichkeiten für das Risikomanagement innerhalb einer Organisation kann die interne Überwachung der Entscheidungsfindung strukturieren (‡1002, ‡1093). Solche Vorkehrungen spiegeln sich in einigen Governance-Frameworks wider, einschließlich des EU-weiten Verhaltenskodex für KI mit allgemeinem Zweck (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Transparenzberichte
  Transparenzberichte beschreiben die Risikomanagement-Praktiken eines KI-Unternehmens, indem sie bestimmte Informationen öffentlich offenlegen oder indem sie Dokumentationen mit Branchenverbänden oder staatlichen Stellen teilen. Beispielsweise reichen zahlreiche KI-Unternehmen Transparenzberichte zum Hiroshima AI Process (HAIP) ein (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Whistleblower-Schutz
  Da ein Großteil der KI-Entwicklung hinter verschlossenen Türen stattfindet, enthalten einige Governance-Frameworks Schutzmaßnahmen für Hinweisgeber, um die Offenlegung potenzieller Risiken gegenüber den zuständigen Behörden zu ermöglichen (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabelle 3.4: Risikogovernance im Risikomanagement für General-Purpose-KI
>white|black||9|11|br Beispielmethoden für das KI-Risikomanagement, aufgeführt alphabetisch. Die enthaltenen Methoden sind so ausgelegt, dass sie das Risikomanagement für viele verschiedene Risikotypen gleichzeitig unterstützen, einschließlich Risiken durch böswillige Nutzung, Risiken durch Fehlfunktionen und systemische Risiken. Angesichts der noch frühen Entwicklung des Risikomanagements für Allzweck-KI sind nicht alle Methoden für jeden KI-Entwickler oder -Betreiber geeignet.


>white|orangered|left|14|15.5|bb Dokumentation und Transparenz sind Bestandteile des Risikogovernance-Systems

Dokumentations- und institutionelle Transparenzmechanismen sowie Informationsaustauschpraktiken erleichtern die externe Prüfung und unterstützen dabei, Risiken im Zusammenhang mit allgemein einsetzbarer KI (‡1101, ‡1102) zu steuern. Es ist gängige Praxis geworden, die Ergebnisse von Pre-Deployment-Tests in einer „Model Card“ oder „System Card“ zu veröffentlichen, zusammen mit grundlegenden Angaben zum Modell oder System, einschließlich dazu, wie es trainiert wurde, und welche potenziellen Einschränkungen es hat (‡1094, ‡1095). Einige Entwickler veröffentlichen zudem Transparenzberichte, die Einzelheiten zu ihren Risiko-Managementpraktiken im weiteren Sinne enthalten (‡1103). Weitere Elemente von Dokumentation und Transparenz umfassen Monitoring und Incident Reporting (‡176, ‡1083*, ‡1103) sowie Informationsaustausch, der durch Dritte wie das Frontier Model Forum ermöglicht werden kann. Einige regulatorische Rahmenwerke, wie der EU AI Act oder „California’s Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53)“ (‡1081, ‡1104), schreiben in bestimmten Fällen den Informationsaustausch über Risiken allgemein einsetzbarer KI vor.

>white|orangered|left|14|15.5|bb Führungsengagement und Anreize prägen die Risikomanagementpraktiken

Die Unternehmenskultur, die Führungsstruktur und Anreizmechanismen beeinflussen die Bemühungen zum Risikomanagement auf unterschiedliche Weise (‡1105). Die Führungszusage und Anreizstrukturen sind häufig relevant dafür, wie Risikomanagementrichtlinien in der Praxis funktionieren. Einige Entwickler verfügen über interne Entscheidungsgremien, die darüber beraten, wie neue KI-Systeme sicher und verantwortungsvoll entworfen, entwickelt und überprüft werden. Aufsicht- und Beratungsausschüsse, Trusts oder KI-Ethikgremien können ebenfalls als Mechanismen für risikomanagementbezogene Leitlinien und organisatorische Aufsicht dienen (‡1092*, ‡1106, ‡1107, ‡1108). Forschende haben argumentiert, dass Herausforderungen bei der freiwilligen Selbstregulierung bedeuten, dass eine Prüfung durch Dritte, Verifizierung und Standardisierung dazu beitragen könnten, das allgemeine Risikomanagement für General-Purpose-KI zu stärken (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Organisatorisches Risikomanagement, Transparenz und Risikoberichterstattungs-Frameworks

Mehrere neue Initiativen konzentrieren sich auf Risikomanagement-Prozesse, Dokumentation und Transparenz. In seiner derzeitigen Form fungiert der EU-Verhaltenskodex für Allgemeinzweck-KI als freiwilliger Rahmen, der Transparenz-, Urheberrechts- sowie Sicherheits- und Sicherheitspraktiken anleitet, um die Einhaltung der Bestimmungen des EU AI Act für Allgemeinzweck-KI zu unterstützen (‡965). Stand Dezember 2025 haben sich mehr als zwei Dutzend Unternehmen† angeschlossen. Der G7 Hiroshima AI Process (HAIP) Reporting Framework (‡1100) ist der erste internationale Rahmen für freiwillige öffentliche Berichterstattung über organisatorische Risikomanagementpraktiken für fortgeschrittene KI-Systeme. Mindestens 20 Entwickler haben öffentliche Transparenzberichte veröffentlicht, die Risikountererkennung, Evaluationsmetriken, Minderungsstrategien und Prozesse zur Datensicherheit abdecken.

KI-Entwickler haben freiwillige Transparenzverpflichtungen übernommen. In China wurden Zusagen von 17 chinesischen KI-Unternehmen veröffentlicht, die vom AI Industry Alliance of China koordiniert wurden; dies geschah im Dezember 2024 (‡1113) und wurde 2025 aktualisiert (‡1114). Auf dem AI Seoul Summit im Mai 2024 in Südkorea unterzeichneten 16 KI-Entwickler aus mehreren Ländern freiwillige Verpflichtungen, für ihre leistungsfähigsten Modelle und Systeme Frontier- KI-Sicherheitsrahmenwerke zu veröffentlichen, und außerdem Risikomanagementpraktiken über die Phasen der Modellentwicklung und -bereitstellung hinweg anzuwenden (‡1052).

    Hinweis † -- Unterzeichner (Stand: Dezember 2025) umfassen: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing und WRITER.

>white|orangered|left|14|15.5|bb Frontier-AI-Sicherheits-Frameworks sind zu einem bedeutenden organisationsweiten Ansatz für das AI-Risikomanagement geworden

Seit 2023 haben mehrere führende KI-Entwickler freiwillig Dokumente veröffentlicht, in denen sie beschreiben, wie sie planen, ernste Risiken aus ihren fortschrittlichsten Systemen zu identifizieren und darauf zu reagieren. Diese Frontier- KI-Sicherheitsrahmenwerke beschreiben, wie ein KI-Entwickler plant, seine fortschrittlichsten KI-Modelle und -Systeme vor und während der Bereitstellung zu bewerten, zu überwachen und zu kontrollieren. Diese Rahmenwerke weisen viele Ähnlichkeiten auf, unterscheiden sich jedoch in wichtigen Punkten (‡1115, ‡1116). Die meisten konzentrieren sich auf Risiken im Zusammenhang mit chemischen, biologischen, radiologischen und nuklearen (CBRN) Bedrohungen, erweiterten Cyberfähigkeiten und erweitertem autonomem Verhalten (‡1115, ‡1117). Eine Minderheit der Rahmenwerke behandelt zusätzliche Risikodomänen wie rechtswidrige Diskriminierung im großen Maßstab und die Ausbeutung von Kindern in sexualisierter Form.

Mehrere Entwickler aktualisierten ihre Frameworks im Jahr 2025 und fügten neue Abschnitte zu schädlicher Manipulation, Fehlanpassungsrisiko und autonomer Replikation und Anpassung hinzu (‡1078, ‡1118). Während viele Frameworks ähnliche Ansätze zum Risikomanagement beschreiben – einschließlich Threat Modelling, Red-Teaming und Bewertungen gefährlicher Fähigkeiten – unterscheiden sie sich in ihren Definitionen von Risikostufen und Schwellenwerten, der Häufigkeit von Bewertungen, Puffern zwischen Bewertungen und Schwellenwerten sowie in der Ausführlichkeit ihrer Zusagen zur Minderung von Risiken (zum Beispiel, ob sie das Löschen von Modellgewichten einschließen oder nur die Entwicklung pausieren) (‡1115, ‡1119). Weitere Informationen finden Sie in Tabelle 3.5.

>white|orangered|left|14|15.5|bb Viele Aktionen in Frontier-AI-Sicherheitsrahmenwerken basieren auf Wenn-dann-Zusagen

Ein zentraler Bestandteil der Frontier- AI-Sicherheits-Frameworks sind „If-Then“-Verpflichtungen. Dabei handelt es sich um bedingte Protokolle, die spezifische Reaktionen auslösen, wenn KI-Modelle und -Systeme vordefinierte Fähigkeits-Schwellenwerte erreichen (‡1120). Beispielsweise könnte eine If-Then-Verpflichtung vorsehen, dass, wenn ein Modell als in der Lage befunden wird, Anfängern sinnvoll dabei zu helfen, CBRN-Waffen zu erstellen und einzusetzen, dann der Entwickler erweiterte Sicherheitsmaßnahmen, Bereitstellungskontrollen und eine Echtzeit-Überwachung implementiert (‡991*).

Im Jahr 2025 gaben mehrere KI-Entwickler bekannt, dass neue Modelle Frühwarnalarme auslösten oder dass sie die Möglichkeit nicht ausschließen konnten, dass eine weitere Bewertung zeigen würde, dass die Modelle Fähigkeitsgrenzen überschritten haben. Dies veranlasste sie, als vorsorgliche Maßnahme erhöhte Schutzmaßnahmen anzuwenden (‡7, ‡33, ‡1121*). Frontier AI Safety Frameworks verlangen üblicherweise vor der Risikominderung eine erste Fähigkeitsbewertung sowie eine verbleibende Risikoanalyse oder einen Sicherheitsnachweis, die oft nach der Minderung durch Red-Teaming informiert werden. Siehe Tabelle 3.5 für detaillierte Informationen.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Preparedness Framework 2 (‡1078*)
  Abgedeckte Risiken:
1. Biologische und chemische Fähigkeiten
2. Cybersicherheitsfähigkeiten
3. KI-Fähigkeiten zur Selbstverbesserung
  Risikostufen oder entsprechende Kennzeichnungen und zugehörige Schutzmaßnahmen:
- Hoch: Könnte bestehende Wege verstärken und zu schwerwiegenden Schäden führen (Erfordert Sicherheitskontrollen und Schutzmaßnahmen)
- Kritisch: Könnte beispiellose neue Wege zu schwerem Schaden ermöglichen (Entwicklung weiter einstellen, bis die angegebenen Schutzmaßnahmen und Sicherheitskontrollstandards einen Kritisch-Standard erfüllen)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Richtlinie zum verantwortungsvollen Skalieren 2.2 (‡991*)
  Abgedeckte Risiken:
1. CBRN-Waffen
2. Autonome KI-Forschung und -Entwicklung (KI-F&E)
3. Cyber-Operationen (unter Bewertung)
  Risikostufen oder entsprechende Maßnahmen und zugehörige Schutzmaßnahmen:
  KI-Sicherheitsstufen (KIS)
- ASL-1: Kein bedeutendes katastrophales Risiko
- ASL-2: Frühe Anzeichen gefährlicher Fähigkeiten (Modelle müssen die ASL-2-Bereitstellungs- und Sicherheitsstandards erfüllen)
- ASL-3: Erheblich erhöhtes Risiko für katastrophalen Missbrauch (Modelle müssen die ASL-3- Bereitstellungs- und/ oder Sicherheitsstandards erfüllen)
- ASL-4+: Zukünftige Klassifizierungen (noch nicht definiert)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Frontier Safety Framework 3.0 (‡1040*)
  Abgedeckte Risiken:
1. Missbrauch
    a. CBRN
    b. Cyber
    c. Schädliche Manipulation
2. Maschinelles Lernen-Forschung und -Entwicklung
3. Fehlanpassung/ instrumentelles Schlussfolgern
  Risikostufen oder gleichwertige Kategorien und zugehörige Schutzmaßnahmen:
  Kritische Fähigkeitsstufen
    Fähigkeitsstufen, bei denen ohne Abhilfemaßnahmen (Sicherheitsnachweise für Bereitstellungen und Sicherheitsmitigations, die mit RAND-Sicherheitsstufen 2, 3 oder 4 ausgerichtet sind (‡1122)) KI-Modelle oder -Systeme ein erhöhtes Risiko für schwere Schäden darstellen können. Die Fähigkeitsstufen umfassen „Früherkennungsbewertungen“ mit spezifischen „Alarm-Schwellenwerten“
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Frontier-AI-Framework 1.1 (‡990*)
  Abgedeckte Risiken:
1. Cybersicherheit
2. Chemische und biologische Risiken
  Risikostufen oder gleichwertige Kategorien und zugehörige Schutzmaßnahmen:
  Risikotoleranzstufen
- Mäßig (Freigabe mit geeigneten Sicherheitsmaßnahmen und Gegenmaßnahmen)
- igh (nicht freigeben)
- Kritisch (Entwicklung stoppen)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Framework für Frontier-Modellsicherheit (‡1123*)
  Abgedeckte Risiken:
1. CBRN-Waffenverbreitung
2. Offensive Cyber-Operationen
3. Automatisierte KI-F&E
  Risikostufen oder Äquivalent und zugehörige Schutzmaßnahmen:
  Wesentliche Fähigkeits-Schwellenwerte
    Modellfähigkeiten, die bei missbräuchlicher Nutzung potenziell erhebliche Schäden für die Öffentlichkeit verursachen können. (Wenn die Schwellenwerte erreicht oder überschritten werden, wird das Modell ohne angemessene Risikominderungsmaßnahmen nicht öffentlich bereitgestellt.)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Frontier-Governance-Framework (‡1124*)
  Abgedeckte Risiken:
1. CBRN-Waffen
2. Offensive Cyber-Operationen
3. Fortgeschrittene Autonomie (einschließlich KI-Forschung und -Entwicklung)
  Risikostufen oder Äquivalent sowie zugehörige Schutzmaßnahmen:
  Risikostufen
- Niedrig oder Mittel (bereitgestellt zulässig gemäß den Anforderungen des Responsible-AI-Programms)
- Hoch oder Kritisch (Weitere Überprüfung und Gegenmaßnahmen
erforderlich)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Frontier-KI-Risikoanalyse (‡1029*)
  Abgedeckte Risiken:
1. Cyberangriff
2. CBRN
3. Überredung und Manipulation
4. Unzulässige Diskriminierung im großen Maßstab
  Risikostufen oder entsprechende Äquivalente und zugeordnete Schutzmaßnahmen:
  Risikogrenzen – Modellrisiko (MR)-Scores
- MR1 oder MR2 (Bewertungsergebnisse werden von Engineering-Teams dokumentiert)
- MR3 (Risikominderungsmaßnahmen und Bewertungsergebnisse werden von den Engineering-Teams dokumentiert und regelmäßig überprüft)
- MR4 (Eine detaillierte Risikoanalyse sollte abgeschlossen werden und eine Genehmigung durch den Leiter der Geschäftseinheit ist erforderlich)
- MR5 (Eine detaillierte Risikoanalyse sollte durchgeführt und von einem unabhängigen Ausschuss genehmigt werden, z. B. von NVIDIAs AI-Ethikkomitee)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Secure AI Frontier Model Framework (‡1125*)
  Abgedeckte Risiken:
1. Bösartige Nutzung (z. B. Malware, sexuelle Ausbeutung von Kindern)
2. Schaden bei gewöhnlicher, nicht-missbräuchlicher Nutzung, z.B. Ausgaben, die zu einem illegalen diskriminierenden Ergebnis führen oder zur Generierung unsicheren Codes
  Risikostufen oder entsprechende Einstufungen und zugeordnete Schutzmaßnahmen:
  Wahrscheinlichkeit und Schwere des Schadens im Kontext
- Niedrig
- Mittel
- Hoch
- Sehr hoch
    (Risikominderungsmaßnahmen und Sicherheitskontrollen sind für alle Systeme und Prozesse vorhanden; zusätzliche Maßnahmen müssen an das KI-System und den Anwendungsfall angepasst werden, in dem ein Modell bereitgestellt wird)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: AGI-Bereitschaftsrichtlinie (‡1127*)
  Abgedeckte Risiken:
1. Cyberangriff
2. Automatisierte KI-F&E
3. Autonome Replikation und Anpassung
4. Biologische Waffenunterstützung
  Risikostufen oder entsprechende Kategorien und zugehörige Schutzmaßnahmen:
  Wesentliche Fähigkeits-Schwellenwerte
    Quantitative Schwellenwerte für Fähigkeits-Benchmarks (falls überschritten, führen Sie gefährliche Fähigkeitsbewertungen, Informationssicherheitsmaßnahmen und Bereitstellungs-Minderungsmaßnahmen durch, oder stoppen Sie die Entwicklung)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: AGI-Bereitschaftsrichtlinie (‡1127*)
  Abgedeckte Risiken:
1. Cyberangriff
2. Automatisierte KI-F&E
3. Autonome Replikation und Anpassung
4. Biologische Waffenunterstützung
  Risikostufen oder gleichwertige Kategorien und zugehörige Schutzmaßnahmen:
  Wesentliche Fähigkeits-Schwellenwerte
    Quantitative Schwellenwerte für Fähigkeits-Benchmarks (Wenn überschritten, Durchführung gefährlicher Fähigkeitsbewertungen, Maßnahmen zur Informationssicherheit und Bereitstellungs-Mitigations oder Abbruch der Entwicklung)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: KI-Sicherheitsframework (‡1128*)
  Abgedeckte Risiken:
1. Kontrollverlust
2. Missbrauch (z.B. biochemische Waffenherstellung
  Risikostufen oder gleichwertige Einstufungen sowie zugehörige Schutzmaßnahmen:
  Risikostufen
- Geringes Risiko (KI-Systeme bereitstellen, aber anschließend überwachen, um Risiken zu steuern)
- Risiko identifiziert (Entweder OpenAI-Systeme nur für autorisierte Nutzer freigeben, um Risiken zu mindern, oder die Bereitstellung zurückhalten, bis zusätzliche Sicherheitsmaßnahmen ergriffen wurden, je nach Anwendungsfall)
- Hohes Risiko (Keine KI-Systeme bereitstellen)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Rahmenwerk für die Frontiersicherheit von KI (‡1129*)
  Abgedeckte Risiken:
1. Biologische Bedrohungen
2. Offensive Cybersecurity
3. Autonome Bedienung und fortgeschrittene Manipulation
  Risikostufen oder entsprechende Einstufungen sowie zugehörige Schutzmaßnahmen:
  Risikostufen
- Level 1 (Grundlegende Schutzmaßnahmen für minimale Risiken und die Möglichkeit einer Open-Source-Veröffentlichung)
- Stufe 2 (Echtzeitüberwachung, Prompt-Filtering, Erkennung verhaltensbezogener Anomalien, Zugriffskontrollen, Red-Teaming und Adversarial-Simulationen)
- Stufe 3 (Erweiterte Schutzmaßnahmen einschließlich Red-Teaming, gestaffelten Rollouts, adversarialem Testing, Verschlüsselung, Multi-Party-Zugriffskontrollen und Zero-Trust-Architektur)
- Ebene 4 (maximale Sicherheitsprotokolle für risikohohe Modelle und maximale Sicherheitsmaßnahmen)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabelle 3.5: Frontier-KI-Sicherheits-Frameworks
>white|black||9|11|br Die erste Reihe der Frontier AI Safety Frameworks, die von einer Teilmenge der KI-Entwickler veröffentlicht wurden, die die Frontier AI Safety Commitments unterzeichnet haben. Die Frameworks decken ähnliche Risiken (mit leichten Abweichungen) ab und verwenden unterschiedliche Risikostufen sowie Ansätze zur Risikoverwaltung.


>white|orangered|left|14|15.5|bb Die Wirksamkeit von Frontier-AI-Sicherheits-Frameworks ist ungewiss

Frontier AI Safety Frameworks können unter bestimmten Bedingungen und für bestimmte Risikokategorien als Risikomanagement-Tools dienen, die einen glaubwürdigen Weg zu Schaden haben (‡1117). Gleichzeitig befassen sich mehrere Analysen mit Fragen nach ihrer Klarheit und ihrem Umfang (‡111, ‡986) sowie mit der Robustheit von KI-Fähigkeiten und Risikoschwellen (‡1031, ‡1130). Bestehende Frameworks konzentrieren sich häufig auf eine Teilmenge von Risikodomänen. Infolgedessen erhalten einige bedeutende Risiken, wie rechtswidrige Überwachung (‡1131, ‡1132) und nicht-einvernehmliche intime Bildinhalte (‡287), weniger Aufmerksamkeit. Im Unterschied zu Risikomanagement-Ansätzen aus anderen Sektoren, wie Luftfahrt oder Nuklearenergie (‡1133*), verwenden Frontier AI Safety Frameworks typischerweise keine expliziten quantitativen Risikoschwellen (‡1134).

Externe Bewertungen der Einhaltung der Frontier- AI-Sicherheitsrahmenwerke durch Entwickler sind bisher begrenzt, unter anderem weil die meisten Rahmenwerke neu sind, öffentlich verfügbare Informationen rar sind und es keine standardisierten externen Audits gibt. Ihre Wirksamkeit wird außerdem davon geprägt, wie gut – und in welchem Umfang – die Zusagen in der Praxis umgesetzt werden. Für sich allein können diese Rahmenwerke kein wirksames Risikomanagement gewährleisten, da ihre praktische Wirkung davon abhängt, wie gut – und in welchem Umfang – sie umgesetzt werden. Bislang sind sie nicht vollständig mit internationalen Standards für das Risikomanagement in Einklang (‡1135). Eine Studie zu früheren freiwilligen Zusagen fand eine uneinheitliche Erfüllung über die Maßnahmen hinweg, was darauf hindeutet, dass die Einhaltung freiwilliger Zusagen wahrscheinlich zwischen Unternehmen und Domänen variieren wird (‡1109).

Zusammengenommen stellen Frontier AI Safety Frameworks die detaillierteste Form des derzeit eingesetzten freiwilligen organisatorischen Risikomanagements dar, unterscheiden sich jedoch erheblich in Umfang, Schwellenwerten und Durchsetzbarkeit.

###@ Regulatorische und Governance-Initiativen

>white|orangered|left|14|15.5|bb Mehrere Rechtsordnungen haben Gesetze mit Transparenzanforderungen eingeführt

Mehrere frühe regulatorische Ansätze führen rechtliche Anforderungen ein, die darauf abzielen, die Standardisierung und Transparenz im Risikomanagement zu erhöhen. Das EU AI Act, das 2024 in Kraft getreten ist, legt Anforderungen in Bezug auf Transparenz, Urheberrecht und Sicherheit für Allzweck-KI-Modelle fest. 2025 wurde der EU-Verhaltenskodex für Allzweck-KI veröffentlicht, um die Einhaltung dieser Verpflichtungen zu unterstützen, indem er Leitlinien zur Modell-Dokumentation und zum Urheberrecht bereitstellt sowie – für die fortschrittlichsten Modelle – bewährte Verfahren im Risikomanagement, wie z. B. Evaluierungen, Risikoabschätzung und -minderung, Informationssicherheit und Meldung schwerwiegender Vorfälle (‡965).

Weitere Beispiele neuer regulatorischer Anforderungen sind das Rahmenrecht in Südkorea zum Ausbau der Entwicklung Künstlicher Intelligenz und zur Schaffung von Vertrauen, das Anforderungen für „hochwirksame“ KI-Systeme in kritischen Bereichen einführt (‡1136), sowie Californias SB 53, das Transparenzanforderungen an Sicherheitsrahmenwerke und die Meldung von Vorfällen festlegt (‡1104). Da diese Anforderungen erst kürzlich eingeführt wurden, ist es noch zu früh, um im Detail beurteilen zu können, wie sie sich auf Risikomanagementpraktiken oder tatsächliche Risikoergebnisse auswirken werden.

>white|orangered|left|14|15.5|bb Breitere Governance-Initiativen bieten freiwillige Orientierungshilfen

Mehrere regionale und grenzübergreifende Governance-Rahmenwerke formulieren mittlerweile gemeinsame Erwartungen für das Risikomanagement durch General-Purpose-AI, indem sie unverbindliche Leitlinien für politische Entscheidungsträger und Organisationen bereitstellen. Chinas „AI Safety Governance Framework 2.0“, veröffentlicht im Jahr 2025, bietet strukturierte Leitlinien zur Risikokategorisierung und zu Gegenmaßnahmen über den gesamten Prozess der Entwicklung und Bereitstellung von KI hinweg (‡1137). Die ASEAN-Mitgliedstaaten veröffentlichten die „ASEAN Expanded Guide on AI Governance and Ethics (Generative AI)“, die Leitlinien zur Governance und Ethik für General-Purpose-AI bereitstellt und darauf abzielt, eine stärkere politische Ausrichtung zwischen den ASEAN-Mitgliedstaaten zu unterstützen (‡1138). Darüber hinaus skizzieren expertengestützte Initiativen wie der „Singapore Consensus“, der von KI-Wissenschaftlerinnen und -Wissenschaftlern aus mehreren Ländern entwickelt wurde, Forschungsprioritäten für die Sicherheit von General-Purpose-AI über die Phasen der Risikoerfassung, Entwicklung und Kontrolle hinweg (‡690).

###@ Aktualisierungen

Seit der Veröffentlichung des letzten Berichts (Januar 2025) hat sich die Risikomanagement-Landschaft für allgemeine KI weiterentwickelt; insbesondere durch die Veröffentlichung neuer Ressourcen wie des EU-Verhaltenskodex für allgemeine KI (Code of Practice), des G7 HAIP-Reporting-Frameworks, Chinas nationalen Rahmens für KI-Sicherheits-Governance 2.0 sowie verschiedener Frontier AI Safety Frameworks verschiedener KI-Entwickler. Diese Initiativen beschreiben Ansätze und Praktiken, die von KI-Entwicklern verwendet werden, um die Risiken im Zusammenhang mit allgemeinen KI-Systemen zu steuern (‡1115). Zwischen den verschiedenen Frontier AI Safety Frameworks und über HAIP-Transparenzberichte hinweg bestehen erhebliche Unterschiede (‡1103); dies spiegelt Unterschiede in den organisatorischen Praktiken, der Risikopriorisierung und dem frühen Entwicklungsstand des Ökosystems für das Risikomanagement bei allgemeiner KI wider. Ein vertrauenswürdiges Ökosystem, in dem unterschiedliche KI-Akteure komplementäre Risikomanagement-Praktiken über den gesamten Lebenszyklus hinweg einbringen, kann zu einem wirksamen Risikomanagement beitragen (‡690).

###@ Beweislücken

Es mangelt an Belegen dafür, wie die Schwere, die Verbreitung und der zeitliche Rahmen neu aufkommender Risiken gemessen werden können; in welchem Umfang diese Risiken in realen Kontexten gemindert werden können; und wie eine Minderung wirksam gefördert oder durchgesetzt werden kann, über vielfältige Akteure hinweg. Es sind weitere Forschungen erforderlich, um besser zu verstehen, wie verbreitet unterschiedliche Risiken sind und wie stark sie sich zwischen verschiedenen Regionen der Welt unterscheiden, insbesondere für Regionen wie Asien, Afrika und Lateinamerika, die sich rasch digitalisieren. Da KI-Modelle zunehmend Handlungsfähigkeit und Autorität erhalten und der Stand der Wissenschaft zu Risiken der General-Purpose-KI voranschreitet, müssen sich auch Risikomanagementansätze weiterentwickeln (‡639, ‡1139).

Bestimmte Risikominderungsmaßnahmen werden zunehmend beliebter (‡690, ‡956), jedoch ist weitere Forschung erforderlich, um zu verstehen, wie robust Risikominderungsmaßnahmen und Schutzvorkehrungen in der Praxis für unterschiedliche Gemeinschaften und KI-Akteure sind (einschließlich für kleine und mittelgroße Unternehmen). Ein größerer Zugang zu Daten über reale Bereitstellungen und die Nutzung von Modellen ist für solche Bewertungen relevant. Darüber hinaus unterscheiden sich die Bemühungen zum Risikomanagement derzeit stark zwischen führenden KI-Unternehmen. Es wurde argumentiert, dass die Anreize von Entwicklern nicht hinreichend mit einer gründlichen Risikoanalyse und dem Risikomanagement in Einklang stehen (‡934). Es besteht weiterhin eine Evidenzlücke hinsichtlich des Umfangs, in dem unterschiedliche freiwillige Verpflichtungen erfüllt werden, welche Hindernisse Unternehmen bei einer vollständigen Einhaltung der Verpflichtungen haben, und wie sie Frontier AI Safety Frameworks in umfassendere Praktiken des KI-Risikomanagements integrieren.

###@ Herausforderungen für politische Entscheidungsträger

Zu den wichtigsten Herausforderungen gehört die Frage, wie die vielfältigen Risiken von Allzweck-KI priorisiert werden sollen, welche Akteure am besten in der Lage sind, diese zu mindern, und wie die Anreize und Zwänge zu verstehen sind, die ihr Handeln prägen. Evidenz deutet darauf hin, dass politische Entscheidungsträger derzeit nur begrenzten Zugang zu Informationen darüber haben, wie KI-Entwickler und -Nutzer (Deployers) die entstehenden Risiken testen, bewerten und überwachen, sowie darüber, wie wirksam unterschiedliche Minderungspraktiken sind (‡1140). Forschende und politische Entscheidungsträger haben Transparenzbemühungen und systematischere Meldungen von Zwischenfällen als mögliche Wege erörtert, um die Risikopriorisierung zu informieren, Vertrauen zu fördern und verantwortliche Entwicklung zu incentivieren (‡957). In der Praxis umfasst das Risikomanagement mehrere Akteure entlang der KI-Wertschöpfungskette – etwa Daten- und Cloud-Anbieter, Modellentwickler und Plattformen für das Hosting von Modellen – wobei jeder Akteur unterschiedliche Möglichkeiten hat, verschiedene Risiken zu bewerten und zu steuern (‡1141). Ein begrenzter Informationsaustausch zwischen diesen Akteuren erschwert es, festzustellen, welche Risiken am wahrscheinlichsten oder am stärksten wirken, insbesondere wenn nachgelagerte gesellschaftliche Auswirkungen berücksichtigt werden.

