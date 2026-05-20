##########
>white|orangered|left|14|30|hr Abschnitt 3.4
### 3.4. Open-Source-Modelle
>white|orangered|left|24|30|hb Open-Source-Modelle

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Wichtige Informationen
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Das Maß an Zugriff, das KI-Unternehmen auf die „Gewichte“ ihrer Modelle gewähren, beeinflusst die Risiken, die diese Modelle darstellen. Gewichte sind die mathematischen Parameter, die es KI-Modellen ermöglichen, Eingaben zu verarbeiten und Ausgaben zu generieren. Für ein bestimmtes Modell können Unternehmen wählen, ob sie die Gewichte vollständig geheim halten, ausgewählten Nutzern einen begrenzten Zugriff gewähren oder es jedermann erlauben, sie in voller Höhe herunterzuladen. Modelle, deren Gewichte öffentlich verfügbar sind, werden als „Open-Weight-Modelle“ bezeichnet.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Open-Weight-Modelle erleichtern Forschung und Innovation, aber ihre Schutzmaßnahmen lassen sich leichter entfernen. Weltweit können verschiedene Akteure – insbesondere solche mit weniger Ressourcen – Open-Weight-Modelle für Forschungs- und kommerzielle Zwecke nutzen. Im Vergleich zu Closed-Weight-Modellen sind Open-Weight-Modelle jedoch leichter so zu verändern, dass sie möglicherweise schädliche Verhaltensweisen zeigen, und es ist schwieriger.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Open-Weight-Modellfreigaben sind unumkehrbar. Sobald sie veröffentlicht wurden, können Modellgewichte nicht zurückgerufen werden. Dies erschwert die Eindämmung potenzieller Schäden, die sich aus der Veröffentlichung eines Modells mit gefährlichen Fähigkeiten ergeben können.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Seit der Veröffentlichung des letzten Berichts (Januar 2025) haben große Open-Weight-Veröffentlichungen die Fähigkeitslücke zu führenden geschlossenen Modellen deutlich verringert. Chinesische Entwickler haben mit DeepSeek und Alibaba ihre R1- bzw. Qwen-Modelle veröffentlicht, die eine mit führenden geschlossenen Modellen vergleichbare Leistung erreichten, während OpenAI seine ersten Open-Weight-Modelle seit 2019 herausbrachte. Die Fähigkeiten führender geschlossener Modelle werden nun auf weniger als ein Jahr Vorsprung gegenüber führenden Open-Weight-Modellen in bedeutenden AI-Benchmarks geschätzt.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Eine zentrale politische Herausforderung besteht darin, den Nutzen von Open-Weight-Modellen zugänglich zu machen, während zugleich ihre spezifischen Risiken gesteuert werden. Ein Ansatz besteht darin, Open-Weight-Modelle im Hinblick auf ihr „marginales Risiko“ zu bewerten: also das Ausmaß, in dem ihre Veröffentlichung faktisch-gegenüberstellend (kontrafaktisch) das gesellschaftliche Risiko über das hinaus erhöht, das bereits durch bestehende Modelle oder andere Technologien gegeben ist. Dies ist jedoch in der Praxis komplex. Kleine Zunahmen des marginalen Risikos im Laufe der Zeit können sich ebenfalls zu erheblichen Steigerungen des Gesamtrisikos summieren.
>oldlace|black||11|15|br      


Open-Weight-Modelle, deren Parameter öffentlich zum Download bereitgestellt werden, haben eindeutige Auswirkungen auf viele der in den vorangehenden Abschnitten behandelten Herausforderungen. Die „Gewichte“ eines KI-Modells enthalten die entscheidenden Informationen, die es ihm ermöglichen, für Nutzer hilfreiche Antworten zu generieren. Sobald sie freigegeben sind, können diese Gewichte nicht zurückgerufen werden: Jeder kann sie herunterladen, studieren, modifizieren, teilen und auf den eigenen Computern oder Cloud-Konten verwenden. Wenn Gewichte offen verfügbar sind, können andere das Modell leichter aufbauen und anpassen, unterschiedliche Bedürfnisse bedienen und Innovation vorantreiben (‡1317). Allerdings können mit demselben Mechanismus auch Nutzer mit böswilligen Absichten leichter Schutzmaßnahmen entfernen und Open-Weight-Modelle für schädliche Anwendungsfälle modifizieren (‡1122, ‡1160). Dadurch stellt sich die Frage, ob bestimmte Open-Weight-Modelle besonderen Anforderungen unterliegen sollten (z. B. strengere Tests vor der Veröffentlichung) oder umgekehrt spezielle Ausnahmen erhalten sollten (z. B. von regulatorischen Meldepflichten) (‡1033).

###@ Hintergrund zu Open-Weight-Modellen

>white|orangered||14|15.5|bb Open-Weight-Modelle können sein, müssen aber nicht unbedingt „Open-Source“-Modelle sein

Obwohl sie oft als „Open Source“ bezeichnet werden, lassen sich die meisten öffentlich freigegebenen Modelle genauer als „Open Weight“ beschreiben. Dies liegt daran, dass die Entwickler zwar die Modellgewichte bereitstellen, aber den zugehörigen Trainingscode oder Datensätze nicht veröffentlichen. Darüber hinaus zeichnet sich Open-Source-Software üblicherweise durch zulässige Lizenzen aus, die den nachgelagerten Akteuren, welche die Software verwenden oder modifizieren, nur minimale Anforderungen auferlegen (‡1318). Beispielsweise haben die Llama-Modelle von Meta restriktive Lizenzbedingungen und enthalten nur Inferenzcode, nicht jedoch Trainingscode, und werden daher typischerweise nicht als Open Source betrachtet (‡1319, ‡1320). Optionen für die Modellfreigabe existieren auf einem Spektrum von vollständig geschlossen bis vollständig Open Source, wobei an jedem Punkt unterschiedliche Risiko-Nutzen-Abwägungen gelten (‡1086*, ‡1320, ‡1321). Tabelle 3.9 beschreibt diese Optionen.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Vollständig geschlossen
  Benutzer können nicht direkt mit dem Modell interagieren
  Beispiele: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Gehosteter Zugriff
  Benutzer können nur über eine bestimmte Anwendung oder eine bestimmte Schnittstelle interagieren, z. B. über eine mobile Chatbot-Anwendung
  Beispiele: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb API-Zugriff auf das Modell
  Benutzer können Anfragen an das Modell über Code senden, wodurch die Nutzung in externen Anwendungen ermöglicht wird.
  Beispiele: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb API-Zugriff auf das Fine-Tuning
  Benutzer können das Modell für ihre spezifischen Anforderungen feinabstimmen
  Beispiele: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Open-Weight: Gewichte zum Download verfügbar
  Benutzer können das Modell herunterladen und auf ihren eigenen Computern ausführen
  Beispiele: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Gewichte, Daten und Code zum Download verfügbar, mit Nutzungseinschränkungen
  Nutzer können das Modell sowie den Inferenz- und Trainingscode herunterladen und ausführen, aber es gibt bestimmte Lizenzbeschränkungen für dessen Verwendung
  Beispiele: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vollständig offen: Gewichte, Daten und Code stehen zum Download bereit, ohne Nutzungsbeschränkungen
  Benutzer haben die volle Freiheit, das Modell, den vollständigen Code und die Daten herunterzuladen, zu verwenden und zu ändern
  Beispiele: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabelle 3.9: Optionen zur Modellfreigabe, die von vollständig geschlossen bis vollständig offen reichen
>white|black||9|11|br Eine illustrative Auswahl von Modellfreigabeoptionen, die von vollständig geschlossenen Modellen (Modelle sind privat und ausschließlich für proprietäre Nutzung vorgehalten) bis hin zu vollständig offenen und Open-Source-Modellen reichen (Modellgewichte, Daten und Code sind frei und öffentlich verfügbar, ohne Einschränkungen hinsichtlich Nutzung, Modifikation und Weitergabe). Modelle, die in den ersten vier Kategorien fallen, werden häufig als „geschlossen“ bezeichnet. Dieser Abschnitt konzentriert sich auf die drei unteren Zeilen. Quelle: adaptiert aus Bommasani, 2024 (‡1317).


###@ Vorteile und Risiken

>white|orangered|left|14|15.5|bb Open-Source-Modelle können einfacher angepasst und evaluiert werden

Open-Weight-Modelle bieten erhebliche Vorteile für Forschung, Innovation und Zugang. Wie in Abschnitt §1.1 erörtert: Was ist allgemeine KI?, ist das Training allgemeiner KI-Modelle äußerst kostspielig – führende Modelle kosten für die Entwicklung Hunderte von Millionen Dollar. Die offene Veröffentlichung von Modellgewichten ermöglicht es Akteuren mit geringerem Ressourcenbestand, bestehende Systeme zu replizieren, zu untersuchen und darauf aufzubauen. Ohne einen solchen Zugang riskieren Gemeinschaften in ressourcenschwachen Regionen, von den Vorteilen der KI ausgeschlossen zu werden, weshalb Open Weights entscheidend sind, um eine globale Mehrheitsbeteiligung an der KI-Entwicklung zu ermöglichen (‡1322). Nachgelagerte Entwickler können Modelle für vielfältige Anwendungen feinabstimmen, z. B. indem sie sie an unterversorgte Minderheitensprachen anpassen oder die Leistung für spezifische Aufgaben optimieren, etwa für rechtliche Ausarbeitungen oder das Verfassen medizinischer Notizen (‡1323, ‡1324*). Auf diese Weise können Open-Weight-Modelle es mehr Menschen und Gemeinschaften ermöglichen, KI zu nutzen und davon zu profitieren, als dies andernfalls möglich wäre (‡1325). Im Fall von Modellen, die nicht leistungsfähig genug sind, um gefährlich zu sein, können diese Vorteile das zusätzliche Risiko, Gewichte offen freizugeben, überwiegen, wobei dies von der Risikotoleranz der relevanten Entscheidungsträger abhängt.

Die Veröffentlichung von Open-Weights erweitert außerdem den Kreis von Entwicklern und Forschern, die das Modell untersuchen, seine Fähigkeiten bewerten, auf Schwachstellen testen und Iterationen zur Verbesserung vornehmen können (‡1326, ‡1327). Dadurch ist es wahrscheinlicher, dass sowohl nützliche Anwendungen als auch schädliche Schwächen identifiziert werden, was jedoch nicht garantiert ist (‡1328, ‡1329). Nutzer können Open-Weight-Modelle zudem auf ihren eigenen Geräten ausführen, sodass sie die Kontrolle über sensible Daten behalten und vermeiden können, dass diese an Server Dritter gesendet werden.

Es gibt zusätzliche Vorteile, wenn Entwicklende Informationen teilen, wie zum Beispiel Trainingsdaten, Code, Evaluationswerkzeuge und Dokumentation sowie Modellgewichte (‡1320, ‡1330, ‡1331, ‡1332*). Mit mehr Informationen können nachgelagerte Entwickelnde und andere Forschende Open-Weight-Modelle besser verstehen und sie an neue Anwendungen anpassen.

>white|orangered|left|14|15.5|bb Sicherheitsvorkehrungen von Open-Weight-Modellen lassen sich leichter entfernen, was einen potenziell missbräuchlichen Einsatz ermöglicht

Open-Weight-Modelle bergen auch zusätzliche Risiken, weil ihre Schutzmechanismen leichter zu entfernen sind. Zwar können sowohl Open-Weight- als auch Closed-Modelle Schutzmechanismen haben, um schädliche Benutzeranfragen abzulehnen, diese Schutzmechanismen sind jedoch bei Open-Weight-Modellen wesentlich leichter zu entfernen. Böswillige Akteure können ein Modell so feinabstimmen, dass es seine Leistung für schädliche Anwendungen optimiert, Teile des Codes entfernen, die für verhindernde schädliche Verwendungen vorgesehen sind, oder eine frühere sicherheitsbezogene Feinabstimmung rückgängig machen (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Dadurch können offene Modellgewichte die in §2.1 erörterten Risiken missbräuchlicher Verwendung verstärken. Risiken durch böswillige Nutzung, indem mehr Akteure ohne Aufsicht bestehende Fähigkeiten für böswillige Zwecke nutzen und erweitern können (‡1122, ‡1315). Obwohl viele Nutzer nicht über die Fähigkeit oder Motivation verfügen werden, Schutzmechanismen bei Open-Weight-Modellen zu entfernen, sind hoch motivierte böswillige Akteure dennoch ein Problem. Darüber hinaus könnten böswillige Akteure Open-Weight-Modelle auch nutzen, um Schwachstellen in ähnlichen Closed-Modellen zu identifizieren (‡1055*). Solche Schwächen sind schwerer zu finden, wenn man nur Closed-Modelle ausführt, aufgrund der stärkeren Kontroll- und Überwachungsmaßnahmen, die Anbieter von Closed-Modellen umsetzen können.

>white|orangered|left|14|15.5|bb Das Teilen von Modellgewichten ist unumkehrbar

Sobald Modellgewichte für den öffentlichen Download verfügbar sind, gibt es keine Möglichkeit, einen umfassenden Rollback aller bestehenden Kopien umzusetzen. Internet-Hosting-Plattformen wie GitHub und Hugging Face können Modelle von ihren Plattformen entfernen, wodurch es für einige Akteure schwieriger wird, herunterladbare Kopien zu finden, und wodurch eine erhebliche Hürde für viele zufällige böswillige Nutzer entsteht (‡1339). Motivierte Akteure können jedoch weiterhin Kopien erhalten, wenn das Modell bereits heruntergeladen und andernorts neu gehostet wurde oder lokal gespeichert ist. Darüber hinaus übernehmen nachgelagerte Entwickler, die Open-Weight-Modelle in ihre Systeme integrieren, ebenfalls alle Schwächen, z. B. Verwundbarkeiten gegenüber Adversarial-Attacken (‡1055) oder Modelleigenschaften, um Überwachungssysteme zu umgehen (siehe §2.2.2. Verlust der Kontrolle) (‡1315). Im Gegensatz zu geschlossenen Modellen, bei denen Hosts universell Updates ausrollen können, können Entwickler von Open-Weight-Modellen nicht garantieren, dass Updates von den Nutzern übernommen werden.

###@ Aktualisierungen

Seit der Veröffentlichung des letzten Berichts (Januar 2025) hat sich die Fähigkeitslücke zwischen führenden Open-Weight- und Closed-Modellen verringert. Chinesische Entwickler sind dabei insbesondere zu wichtigen Anbietern von Open-Weight-Modellen geworden. Im Januar 2025 veröffentlichte DeepSeek sein R1-Modell, das auf mehreren Benchmarks eine Leistung erreichte, die mit OpenAI’s o1 vergleichbar war (‡1340). Alibabas Qwen-Modelle haben ebenfalls an Zugkraft gewonnen und belegten bis August 2025 den Spitzenplatz für ein Open-Weight-Modell auf Chatbot Arena, einem weithin genutzten Performance-Benchmark (‡1341, ‡1342*). Im August 2025 veröffentlichte OpenAI seine ersten Open-Weight-Modelle seit der Veröffentlichung von GPT-2 im Jahr 2019, gpt-oss-120b und gpt-oss-20b. Meta hat die Veröffentlichung von Llama-Modellen mit Open Weights fortgesetzt. Die Fähigkeiten der führenden Closed-Modelle werden mittlerweile auf prominentem AI-Benchmarking auf weniger als ein Jahr Vorsprung gegenüber den führenden Open-Modellen geschätzt (Abbildung 3.10).

###@ Beweislücken

Eine zentrale Evidenzlücke betrifft die reale Wirksamkeit technischer Lösungen zur Verhinderung des Missbrauchs von Open-Weight-Modellen. Forschende haben verschiedene Ansätze vorgeschlagen, um Modelle manipulationssicherer zu machen. Dazu gehören neue Trainingsverfahren, die darauf ausgelegt sind, Modelle gegenüber schädlichen Veränderungen widerstandsfähig zu machen (‡1276), das Filtern schädlicher Inhalte aus Trainingsdaten (‡55) sowie Abwehrmaßnahmen gegen Jailbreaks (‡675, ‡676). Diese Verfahren werden inzwischen in praxisnahen Veröffentlichungen großer Entwickler übernommen. So hat OpenAI einige dieser Techniken in seinen gpt-oss-Modellen eingesetzt und berichtet, dass adversarial feinjustierte Versionen keine hohen Fähigkeits-Schwellen erreichten (‡1344*). Allerdings hat die Forschung gezeigt, dass böswillige Akteure Schutzmechanismen außer Kraft setzen können, indem sie Modelle anhand schädlicher Beispiele neu trainieren (‡1345, ‡1346). Darüber hinaus ist es weiterhin schwierig, die Robustheit von Schutzmaßnahmen zuverlässig zu bewerten, wodurch ihre Wirksamkeit gegenüber realen Angriffen ungewiss bleibt (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Abbildung 3.10: Fähigkeitslücke zwischen den führenden Open-Weight- und Closed-AI-Modellen
>white|black||9|11|br Epoch-Fähigkeitsindex (ECI)-Scores der bestplatzierten Open-Weight-(Dunkelblau) und Closed-(Hellblau) Modelle im Zeitverlauf. Der ECI kombiniert Scores von 39 Benchmarks zu einer einzigen allgemeinen Fähigkeits-Skala. Die besten Open-Weight-Modelle liegen ungefähr ein Jahr hinter den Closed-Modellen zurück. Quelle: Epoch AI, 2025 (‡1343).


###@ Minderungen

Technische Gegenmaßnahmen für Risiken von Open-Weight-Modellen greifen während des gesamten Prozesses der KI-Entwicklung und -Bereitstellung (‡1141, ‡1195, ‡1347). Wenn Modelle beispielsweise entwickelt werden, können Entwickler und nachgelagerte Adapter sensible Inhalte aus den Trainingsdaten herausfiltern, um schädliche Fähigkeiten zu minimieren. Das Entfernen schädlicher Beispiele aus den Trainingsdaten eines Modells kann schädliche adversariale Feinanpassungen 10-mal wirksamer verhindern als Verteidigungen, die erst nach dem Training hinzugefügt werden, obwohl dies auch positive Fähigkeiten beeinträchtigen kann (‡55). KI-Anwendungsanbieter können außerdem Mechanismen zur Vorfallsberichterstattung und -reaktion implementieren (‡1348).

Zusätzlich können Hosting-Plattformen wie HuggingFace und GitHub Plattformbedingungen festlegen, um Modelle zu entfernen, die für schädliche Zwecke modifiziert wurden (‡1141, ‡1324). Modellentwickler können Auditoren vollständigen Zugang vor der Veröffentlichung gewähren oder eine Strategie für eine „gestaffelte“ Veröffentlichung wählen – indem Modelle an schrittweise größere Gruppen freigegeben werden (‡1086). Dies kann dabei helfen, potenzielle Fehlfunktionen oder Verwundbarkeiten zu identifizieren, bevor ein Modell weithin verfügbar gemacht wird (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Anmerkung 3.1: Modellsicherheitsgewicht
>oldlace|black|left|13|15|hb  Anmerkung 3.1: Modellsicherheitsgewicht
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Die in diesem Abschnitt besprochenen Risiken setzen voraus, dass die Modellgewichte absichtlich freigegeben werden. Allerdings können geschlossene Modellgewichte auch durch Diebstahl oder Lecks zugänglich werden. Geschlossene Modelle kosten Hunderte von Millionen Dollar, um sie zu entwickeln (§1.1. What is general-purpose AI?), und sind im Durchschnitt leistungsfähiger als Open-Weight-Modelle (‡1343). Dadurch werden sie für Akteure von Amateur-Hackern bis hin zu Nationalstaaten attraktiv, die darauf abzielen, führende KI-Modelle zu erlangen.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Gestohlene geschlossene Modellgewichte würden Risiken verursachen, die denen für Open-Weight-Modelle ähnlich sind, aber möglicherweise ohne irgendeine der Gegenmaßnahmen. Schadakteure könnten Schutzvorrichtungen von den leistungsfähigsten Modellen entfernen. Anders als legitime Entwickler würden solche Akteure nicht den Reputations-, Rechts- oder kommerziellen Einschränkungen unterliegen, die derzeit dazu beitragen, dass führende KI-Unternehmen ihre Modelle sicher bereitstellen.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Die aktuellen Sicherheitsniveaus variieren in der Branche und können gegenüber anspruchsvollen Angreifern möglicherweise unzureichend sein. Einige Entwickler verpflichten sich dazu, Modellgewichte gegen Cybercrime-Syndikate und Insiderbedrohungen abzusichern (‡582), während andere keine öffentlichen Sicherheitszusagen gemacht haben (‡1109, ‡1349). Forschungsergebnisse deuten darauf hin, dass KI-Datenzentren möglicherweise nicht in der Lage sind, Angriffen der anspruchsvollsten und bestausgestatteten Akteure standzuhalten (‡582, ‡1350, ‡1351). Stand Dezember 2025 gibt es keine bestätigten, öffentlich dokumentierten Fälle von Diebstahl von Modellgewichten. Allerdings wurden andere Sicherheitsverletzungen bei führenden KI-Unternehmen gemeldet, darunter das Eindringen in die E-Mail-Systeme von Microsoft (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Das Schließen dieser Sicherheitslücken würde erhebliche Investitionen in Hardware, Software, Personal und die Sicherung der Einrichtungen erfordern. Einige Sicherheitsverbesserungen könnten mit koordiniertem Vorgehen relativ schnell umgesetzt werden (‡1122). Andere, jedoch ebenso wichtige Maßnahmen, wie die Sicherung von Hardware-Lieferketten und Einrichtungen, würden vermutlich Jahre in Anspruch nehmen (‡1122). Private Unternehmen verfügen möglicherweise auch nicht über die Ressourcen oder Informationen, um allein einen ausreichenden Schutz zu entwickeln. Beispielsweise haben KI-Entwickler keinen Zugriff auf die klassifizierte Bedrohungsaufklärung, die Regierungen haben (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Herausforderungen für politische Entscheidungsträger

Eine zentrale Herausforderung für politische Entscheidungsträger besteht darin, die Vorteile der Veröffentlichung und gemeinsamen Nutzung von Open-Weight-Modellen zu sichern, ohne das Risiko erheblich zu erhöhen. Um katastrophalen Schaden zu vermeiden, sollten Entwickler von Open-Weight-Modellen keine Modelle veröffentlichen, ohne die Risiken bewertet zu haben—sowohl mithilfe etablierter Bewertungsmethoden, die für geschlossene Modelle verwendet werden, als auch durch zusätzliche Tests, da böswillige Akteure Modelle feinabstimmen und Sicherheitsvorkehrungen entfernen können. In der Praxis kann dies schwierig sein, weil Fähigkeitsentwicklungen unvorhersehbar sein können, Open-Weight-Veröffentlichungen nicht rückgängig gemacht werden können und Bewertungsvorhaben erforderlich sind, um vorherzusagen, wann eine Veröffentlichung erhebliche potenzielle Schäden verursachen würde. Ein Ansatz besteht darin, das „marginale Risiko“ offener Veröffentlichungen zu bewerten: das Ausmaß, in dem die Veröffentlichung kontrafaktisch das gesellschaftliche Risiko über das bereits durch bestehende Modelle oder andere Technologien verursachte Risiko hinaus erhöht (‡556, ‡1033, ‡1354, ‡1355) (siehe §3.2. Risiko-Management-Praktiken). Die Abschätzung jedoch, wie ein System das Risiko nachgelagerter Anwendungen erhöhen oder verringern wird, nachdem es eingesetzt wurde, ist komplex und situationsabhängig. In riskanten Situationen können sich schrittweise Risikozunahmen mit aufeinanderfolgenden Veröffentlichungen im Zeitverlauf zu erheblichen Anstiegen des Gesamtrisikos aufsummieren, selbst wenn das jeweils mit jeder Veröffentlichung verbundene marginale Risiko als akzeptabel erscheint (‡1356, ‡1357). Die Dual-Use-Natur von KI-Fähigkeiten erschwert die Governance zusätzlich: Funktionen, die das Ermöglichen nützlicher Anwendungen in Medizin oder Forschung erlauben, können für schädliche Zwecke umgewidmet werden, und sobald die Gewichte öffentlich sind, kann es schwierig sein, legitime von böswilligen Verwendungen zu unterscheiden. Unklar ist zudem, wer zur Verantwortung gezogen werden sollte, wenn Open-Weight-Modelle für schädliche Zwecke modifiziert werden.

