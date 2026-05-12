###@ Was sind Allzweck-KI-Systeme?

Allgemein verwendbare KI-Systeme sind Softwareprogramme, die Muster aus großen Datenmengen erlernen, sodass sie eine Vielzahl von Aufgaben ausführen können, statt auf eine einzelne bestimmte Funktion oder Domäne spezialisiert zu sein (siehe Tabelle 1.1). Um diese Systeme zu erstellen, führen KI-Entwickler einen mehrstufigen Prozess durch, der erhebliche rechnerische Ressourcen, große Datensätze und spezialisierte Expertise erfordert (siehe Tabelle 1.2). Rechnerische Ressourcen (oft auf „Compute“ verkürzt) werden sowohl benötigt, um KI-Systeme zu entwickeln als auch um sie bereitzustellen, und umfassen spezialisierte Computerchips sowie die Software und die Infrastruktur, die erforderlich sind, um sie auszuführen.† Da sie auf großen, vielfältigen Datensätzen trainiert werden, können allgemein verwendbare KI-Systeme viele unterschiedliche Aufgaben ausführen, etwa das Zusammenfassen von Texten, das Generieren von Bildern oder das Schreiben von Computercode. Dieser Abschnitt erklärt, wie allgemein verwendbare KI-Systeme hergestellt werden, was „Reasoning“-Modelle sind, und wie politische Entscheidungen die Entwicklung allgemein verwendbarer KI-Systeme beeinflussen.

    Hinweis † -- Der Begriff „Compute“ kann sich entweder auf eine Messgröße der Anzahl der Berechnungen beziehen, die ein Prozessor ausführen kann (typischerweise gemessen in Floating-Point-Operationen pro Sekunde), oder spezifisch auf die Hardware (wie z. B. Grafikprozessoren), die diese Berechnungen durchführt.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Sprachsysteme
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Befehl A (‡3*)
- EXAONE 4.0 (‡4*)
- Gemini 3 Pro (‡5*)
- GLM-4.5 (‡6*)
- GPT-5(‡7*)
- Hunyuan-Large (‡8*)
- Kimi K2 (‡9*)
- Mistral 3.1 (‡10*)
- Qwen3 (‡11*)
- DeepSeek-V3.2 (‡12*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Bildgeneratoren
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Bild (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Videogeneratoren
- Kosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Ich sehe 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotik- und Navigationssysteme
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Prädiktoren für verschiedene Klassen biomolekularer Strukturen
- AlphaFold 3 (‡27)
- Amplify (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ KI-Agenten
- AlphaEvolve (‡31*)
- ChatGPT-Agent (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magnetic-One (‡35*)
- OpenScholar (‡36*)
- Der KI-Wissenschaftler-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabelle 1.1: Allzweck- KI-Typen
>white|black||9|11|br Es gibt mehrere unterschiedliche Arten von allgemeiner KI. In diesem Bericht werden Modelle, die strukturelle Informationen für verschiedene Klassen von Molekülen vorhersagen können, als „allgemein verwendbare“ KI betrachtet, weil sie für eine Vielzahl von Aufgaben angepasst werden können. Beispielsweise sind Modelle, die darauf trainiert sind, die Proteinstruktur vorherzusagen, für eine Vielzahl weiterer Aufgaben geeignet, wie das Vorhersagen von Proteinwechselwirkungen, das Vorhersagen von Bindungsstellen für kleine Moleküle sowie das Vorhersagen und das Design zyklischer Peptide (‡40).


>white|orangered|left|13|15|bb Deep Learning ist grundlegend für KI mit allgemeinem Zweck

Forscher bauen allgemeine KI-Modelle mithilfe eines als „Deep Learning“ bezeichneten Prozesses auf, der Modelle darauf trainiert, aus Beispielen zu lernen (‡41). Im Gegensatz zum Software Engineering lernen Deep Learning-Modelle, Aufgaben mithilfe von Daten zu bewältigen, statt auf handgeschriebene Anweisungen zurückzugreifen. Indem diese Modelle große Mengen an Daten verarbeiten, wie z. B. Bilder, Text oder Audio, entdecken sie Möglichkeiten, diese Daten darzustellen, und erstellen interne Repräsentationen von Mustern (wie Formen, Wortassoziationen oder Klangstrukturen), die dem Modell dabei helfen, Zusammenhänge zu erkennen und Ausgaben zu erzeugen, die mit dem Trainingsziel übereinstimmen. Anschließend verwenden sie diese gelernten internen Repräsentationen als abstrakte Merkmale, um neue, ähnliche Daten zu analysieren und Ausgaben im selben Stil zu erzeugen. So kann beispielsweise ein allgemeines KI-Modell, das mit genügend Beispielen englischer romantischer Dichtung aus dem 19. Jahrhundert trainiert wurde, neue Gedichte in diesem Stil erkennen und neue Inhalte in einem ähnlichen Stil hervorbringen.

Auf einer granulareren Ebene funktioniert Deep Learning, indem es Daten über Schichten miteinander verbundener Informationsverarbeitungs-Knoten verarbeitet. Diese Knoten werden oft als ‚Neuronen‘ bezeichnet, weil sie lose von Neuronen in biologischen Gehirnen inspiriert sind (‚neuronale Netze‘) (Abbildung 1.1) (‡42). Während Informationen von einer Schicht von Neuronen zur nächsten fließen, wandelt das Modell die Daten schrittweise in abstraktere Repräsentationen um – als Gruppen gelernter Merkmale, also Muster, die das Modell automatisch in den Daten entdeckt hat, statt handkodierte. Beispielsweise könnte in einem bildverarbeitenden Modell die ersten Schichten darauf ausgelegt sein, einfache Merkmale wie Kanten oder grundlegende Formen zu erkennen, während tiefere Schichten diese Merkmale zusammenführen, um komplexere Muster wie Gesichter oder Objekte herauszufiltern.

Die Merkmale in allen Schichten werden durch den Optimierungsprozess entdeckt, der das Trainingsverfahren definiert. Während des Trainings, wenn das Modell Fehler macht, passen Deep-Learning-Algorithmen die Stärke verschiedener Verbindungen zwischen Neuronen an, um die Leistung des Modells zu verbessern. Die Stärke jeder Verbindung zwischen Knoten wird häufig als „Gewicht“ bezeichnet. Dieser geschichtete Ansatz gibt dem Deep Learning seinen Namen.

Deep Learning hat sich als sehr effektiv erwiesen, um KI-Systemen die Durchführung von Aufgaben zu ermöglichen, die zuvor als schwierig für traditionelle, handprogrammierte Computersysteme sowie für andere frühere symbolische oder regelbasierte KI-Methoden galten. Die meisten derzeit führenden, allgemeinzweckfähigen KI-Modelle basieren heute auf einer spezifischen neuronalen Netzwerkarchitektur, die als „Transformer“ bekannt ist (‡43, ‡44). Transformer verwenden einen „Attention“-Mechanismus (‡45), der dem Modell hilft, sich bei der Verarbeitung von Informationen auf die relevantesten Teile der Eingabedaten zu konzentrieren, wie zum Beispiel darauf, welche Wörter in einem Satz am wichtigsten für das Verständnis seiner Bedeutung sind. Diese besondere Art des Modellaufbaus hat zu bedeutenden Verbesserungen in der Übersetzung (‡43), der Verarbeitung natürlicher Sprache (‡46), der Bilderkennung (‡47) und der Spracherkennung (‡48, ‡49) geführt und letztlich zur Entwicklung der heute fortschrittlichsten Modelle.

![fig1.1](images/fig1.1_neural_network.png)

##### Abbildung 1.1: Eine anschauliche Darstellung eines „neuronalen Netzes“
>white|black||9|11|br Heutige Allzweck-Modelle für Künstliche Intelligenz basieren auf diesen Netzwerken, die nur lose von biologischen Gehirnen inspiriert sind. Unterschiedliche Netzwerke haben unterschiedliche Größen und Architekturen. Allerdings bestehen alle aus miteinander verbundenen Informationseinheiten zur Verarbeitung, die „Neuron“ genannt werden, wobei die Stärke der Verbindungen zwischen den Neuronen als „Gewichte“ bezeichnet wird. Gewichte werden durch das Training mit großen Mengen an Daten aktualisiert. Quelle: International AI Safety Report 2025 (‡50) (modifiziert).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Abbildung 1.2: Eine schematische Darstellung der Phasen der Entwicklung von Allzweck-KI
>white|black|left|9|11|br Internationaler KI-Sicherheitsbericht 2026.


>white|orangered|left|13|15|bb Allzweck-KI wird in Stufen entwickelt

Die Entwicklung eines universell einsetzbaren KI-Systems umfasst mehrere Phasen, von der anfänglichen Modelltrainierung bis hin zur Überwachung und Aktualisierung nach der Bereitstellung (Abbildung 1.2). In der Praxis überlappen sich diese Schritte häufig in einem iterativen Prozess. Jede Phase erfordert unterschiedliche Ressourceninputs (z. B. Daten, Arbeitskräfte, Rechenleistung) und unterschiedliche Techniken, und sie werden manchmal von verschiedenen Entwicklern durchgeführt (Abbildung 1.2 und Tabelle 1.2).

Beispielsweise erfordert das Vortraining von Modellen im Allgemeinen große Mengen an Rechenleistung und Daten, wodurch diese Phase besonders empfindlich gegenüber Richtlinien ist, die den Zugang zu rechnerischen Ressourcen oder Trainingsdaten beeinflussen (‡51, ‡52). Ebenso beinhalten die Datenaufbereitung und einige Methoden zur Feinabstimmung von Modellen derzeit große Mengen an menschlicher Arbeitskraft für die anfängliche Datennotation (‡53). Diese Phase ist daher empfindlich gegenüber Änderungen der Arbeitskosten, Plattformrichtlinien oder Vorschriften, die grenzüberschreitende Vertragsvereinbarungen betreffen.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Datensammlung und -aufbereitung
> 
  Bevor ein allgemeines KI-Modell trainiert wird, sammeln Entwickler und Datenverantwortliche Rohdaten, reinigen sie, kuratieren und standardisieren sie, sodass sie in ein Format gebracht werden, aus dem das Modell lernen kann. Dieser Prozess kann sehr arbeitsintensiv sein. Die Trainingsdatensätze hinter modernen Modellen bestehen aus einer immensen Anzahl von Beispielen aus dem gesamten Internet.
  Teams entwickeln häufig ausgeklügelte Filtermethoden, um schädliche Inhalte zu reduzieren, doppelte Daten zu eliminieren und die Repräsentation über verschiedene Themen und Quellen hinweg zu verbessern (‡54, ‡55). Data Curation kann zudem dazu beitragen, Urheberrechts- und Datenschutzverletzungen zu reduzieren, Beispiele zu entfernen, die gefährliches Wissen enthalten, mehrere Sprachen zu behandeln und die Dokumentation für die Nachverfolgbarkeit der Datenherkunft (data provenance) zu verbessern (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Vortraining (erste Trainingsphase)

  Während des Pre-Trainings füttern Entwickler Modelle mit riesigen Mengen vielfältiger Daten, um eine breite Wissensgrundlage und ein kontextuelles Verständnis zu verankern. Dieser Prozess erzeugt ein „Basismodell“. Dies ist ein äußerst daten- und rechenintensiver Prozess.

  Während des Vortrainings werden Modelle Milliarden oder Billionen von Beispielen für Inhalte wie Bilder, Texte oder Audio ausgesetzt. Durch diese Exposition entdeckt das Modell nach und nach abstrakte Merkmale, um Daten zu repräsentieren, und lernt, wie diese Merkmale miteinander zusammenhängen, sodass es neue Eingaben im jeweiligen Kontext sinnvoll verarbeiten kann. Dieser Vortrainingsprozess dauert Wochen oder Monate (‡59) und nutzt Dutzende oder Hunderte Tausend Grafikeinheiten (GPUs) oder Tensorverarbeitungseinheiten (TPUs) (‡60) – spezialisierte Computerchips, die dafür ausgelegt sind, viele solcher Berechnungen schnell zu verarbeiten. Einige Entwickler führen das Vortraining mit eigener Rechenleistung durch, während andere die von spezialisierten Compute-Providern bereitgestellten Ressourcen nutzen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Post-Training und Feinabstimmung (zweite Trainingsphase)

  „Post-Training“ verfeinert das Basismodell weiter, um es für eine spezifische Anwendung zu optimieren. Es handelt sich um einen moderat rechenintensiven und stark arbeitsintensiven Prozess. Eine Verlagerung hin zur Verwendung von „synthetischen Daten“ – künstlich generierten Informationen, die reale Daten nachahmen, aber mithilfe von Algorithmen oder Simulationen erzeugt werden – trägt dazu bei, diese Phase weniger arbeitsintensiv zu machen.
  Post-Training umfasst verschiedene Feinabstimmungsverfahren und weitere Modifikationen. „Supervised fine-tuning“ beinhaltet ein weiteres Training eines trainierten Modells auf spezifischen Datensätzen, um die Leistung des Modells in diesem Bereich zu verbessern (‡61, ‡62). Beispielsweise könnte ein Allzweckmodell zusätzlich auf einem großen Korpus radiologischer Bilder trainiert werden. „Reinforcement learning“ (RL) beinhaltet die Verbesserung der Modellleistung, indem ein Modell „belohnt“ wird (positive Rückmeldung) für erwünschte Ausgaben und ein Modell „bestraft“ wird (negative Rückmeldung) für unerwünschte Ausgaben. Es hat zwei bedeutende Unterkategorien. „Reinforcement learning from human feedback“ beinhaltet das Belohnen von Ausgaben, die mit den menschlichen Präferenzen übereinstimmen, und das Bestrafen von Ausgaben, die dies nicht tun, basierend auf menschlichem Feedback (‡63, ‡64*). „Reinforcement learning with verifiable rewards“ (RLVR) wird zur Verbesserung der Modellleistung bei Aufgaben verwendet, die eine sachliche Korrektheit erfordern, wie etwa Mathe- oder Code-Generierung. Entwickler wechseln typischerweise zwischen dem Anwenden von Post-Training-Techniken und dem Durchführen von Tests, bis die Ergebnisse zeigen, dass das Modell die gewünschten Spezifikationen erfüllt.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Systemintegration

  Entwickler kombinieren einen oder mehrere Allzweck-KI-Modelle mit anderen Komponenten, um ein einsatzbereites „KI-System“ zu erstellen. GPT-5 (zum Beispiel) ist ein Allzweck-KI-Modell, das Text, Bilder und Audio verarbeitet, während ChatGPT ein Allzweck-KI-System ist, das mehrere Modelle unterschiedlicher Größe und Fähigkeiten mit einer Chat-Schnittstelle, Inhaltsverarbeitung, Webzugriff und Anwendungsintegration kombiniert, um ein funktionsfähiges Produkt zu erstellen.
  Zusätzlich zur Inbetriebnahme von KI-Modellen zielen die weiteren Komponenten in einem KI-System auch darauf ab, die Leistungsfähigkeit, den Nutzen und die Sicherheit zu verbessern. Beispielsweise könnte ein System mit einem Filter ausgestattet sein, der Modell-Eingaben oder -Ausgaben erkennt und blockiert, die schädliche Inhalte enthalten (‡65*). Entwickler nutzen außerdem zunehmend „Scaffolding“ – zusätzliche Software, die um allgemeine KI-Modelle herum aufgebaut ist und es ihnen ermöglicht, vorauszuplanen, Ziele zu verfolgen und mit der Welt zu interagieren (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Bereitstellung und Veröffentlichung
  Bereitstellung ist der Prozess, bei dem das integrierte KI-System für den vorgesehenen Einsatz verfügbar gemacht wird. Entwickler und Bereitsteller implementieren KI-Systeme in reale Anwendungen, Produkte oder Services. Entwickler können KI-Systeme intern (für den eigenen Gebrauch) oder extern (für private Kunden oder für die öffentliche Nutzung) bereitstellen. Bei der externen Bereitstellung von KI-Systemen stellen Unternehmen den Nutzern häufig den Zugriff über Online-Benutzeroberflächen oder Anwendungsprogrammierschnittstellen (APIs) bereit, die es den Nutzern ermöglichen, auf das System zuzugreifen und es auszuführen. Beispielsweise könnte ein Unternehmen einen maßgeschneiderten Kundenservice-Chatbot entwerfen, der von einem allgemeinen KI-System eines anderen Unternehmens betrieben wird.
  „Bereitstellung eines KI-Systems“ bezeichnet das Bereitstellen eines Modells für den Einsatz in der realen Welt mit integrierten Tools und Schnittstellen, während „Modellfreigabe“ das Zugänglichmachen des Basis-Modells für andere umfasst – entweder als Open-Weight-Modell (herunterladbare Parameter) oder als Closed-Weight-Modell (nur API-Zugriff). Siehe §3.4. Open-Weight-Modelle.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Nachbereitendes Monitoring und Updates nach der Bereitstellung

  Entwickler sammeln häufig Nutzerfeedback, analysieren es, verfolgen Auswirkungen- und Leistungskennzahlen und nehmen iterative Verbesserungen vor, um Probleme zu adressieren, die bei der Nutzung in der realen Welt entdeckt wurden (‡67). Verbesserungen werden umgesetzt, indem Systemintegrationen aktualisiert werden, oft durch fortlaufendes Fine-Tuning und indem Modellen Zugriff auf externe Datenbanken mit (aktuellen) Fakten bereitgestellt wird. So bleiben große KI-Modelle auf dem neuesten Stand, ohne den vollständigen Vortrainingsprozess zu wiederholen (‡68*). Dies ermöglicht es, dass sich Fähigkeiten über aufeinanderfolgende Trainingsrunden hinweg ansammeln, während gleichzeitig Stabilität gewahrt und die Rechenkosten reduziert werden.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabelle 1.2: Allzweck-AI-Entwicklungsphasen
>white|black||9|11|br In jeder Phase der Entwicklung von allgemeinem KI entstehen, wird das KI-Modell für den nachgelagerten Einsatz verbessert und schließlich als vollständig integriertes KI-System bereitgestellt, überwacht und aktualisiert.


>white|orangered|left|13|15|bb Begründungssysteme generieren während der Inferenz „Ketten des Denkens“, um die Leistung zu verbessern

Inferenz tritt auf, wenn jemand das KI-Modell verwendet, nachdem es trainiert wurde. Beispielsweise liegt eine Inferenz vor, wenn eine Person ein KI-System bittet, eine Reise zu planen, und das Modell dahinter auf relevante Aspekte dessen zurückgreift, was es über Geografie, Transport und Küche gelernt hat, um eine Reiseroute zu generieren.

In the last decade, advances in AI capabilities have largely come from larger training runs; das heißt, durch Erhöhung der Rechenleistung, die zum Trainieren eines KI-Modells verwendet wird. In letzter Zeit jedoch erzielten Forschende mehr Fortschritte, indem sie den Modellen erlaubten, Informationen länger zu verarbeiten, und indem sie sie darauf trainierten, explizite Gedankenschritte zu produzieren, während sie eine Aufgabe bearbeiten (‡69*, ‡70). KI-Systeme, die so arbeiten, werden als „Reasoning-Systeme“ bezeichnet, und die Zwischenerklärungen, die sie durchlaufen, wenn sie ein Problem lösen oder eine Frage beantworten, heißen „chains of thought“. Reasoning-Systeme erfordern zum Zeitpunkt der Nutzung mehr Rechenressourcen, um diese anspruchsvollen chains of thought zu erzeugen (‡71, ‡72, ‡73, ‡74), sowie mehr Ressourcen während des Trainings, damit sie besser lernen, zu reasoning. In der Praxis ermöglichen diese Reasoning-Fähigkeiten es KI-Systemen, komplexere Probleme zu lösen, indem sie eine Aufgabe iterativ in kleinere Schritte zerlegen. Tabelle 1.3 zeigt ein Beispiel für ein Non-Reasoning-System und ein Reasoning-System, die dasselbe Problem lösen.

Begründungssysteme haben bei anspruchsvollen Aufgaben bedeutende Durchbrüche bei den Fähigkeiten erzielt. Zum Beispiel haben Begründungssysteme, die auf das Lösen mathematischer Probleme spezialisiert sind, wie Googles Gemini Deep Think und ein nicht veröffentlichtes, experimentelles Modell von OpenAI, im Jahr 2025 Internationale Mathematik-Olympiade-Aufgaben (in einer strukturierten Testumgebung) auf einem Niveau gelöst, das einer menschlichen Goldmedaillen-Leistung entspricht (‡75, ‡76). Begründungssysteme haben in formalen Domänen wie Mathematik, Logikrätseln und strukturierten wissenschaftlichen Fragestellungen erhebliche Fortschritte gezeigt, in denen eine Schritt-für-Schritt-Begründung explizit verifiziert werden kann (‡77). Allerdings können Begründungssysteme auch scheitern, indem sie irrelevante, unproduktive oder repetitive Ketten von Gedankenschritten erzeugen (‡78, ‡79).

###@ Updates zu Trainingsmethoden

Seit der Veröffentlichung des letzten Berichts (Januar 2025) hat eine Trainingsmethode namens „Distillation“ die Effizienz, mit der einige Modelle feinabgestimmt werden können, deutlich erhöht. Bei der Distillation wird ein „Student“-Modell anhand der Ausgaben eines leistungsfähigeren (und üblicherweise größeren) „Teacher“-Modells trainiert, sodass das Student-Modell die Ausgaben des Teacher-Modells direkt nachahmen kann (‡80). Beispielsweise entwickelte DeepSeek ein großes Modell namens DeepSeek-R1, das besonders gut bei „chain-of-thought“-Schlussfolgerungen ist. R1 erzeugte Schlussfolgerungs-Ausgaben, die anschließend verwendet wurden, um kleinere Student-Modelle feinabzustimmen, darunter DeepSeek-V3. DeepSeek-V3 behält einen Großteil der mathematischen-, Programmier- und Dokumentanalyse-Fähigkeiten von R1 bei und wurde Berichten zufolge für ungefähr $10,000 USD feinabgestimmt (wobei die Kosten der Vortrainierung nicht angegeben wurden) (‡81). Dies dürfte um Größenordnungen niedriger sein als die Kosten der Feinabstimmung ähnlich leistungsfähiger, größerer Modelle.

![table1.3](images/table1.3_example_reasoning.png)

##### Tabelle 1.3: Ein Beispiel für ein nicht-vernunftbasiertes System (links) versus ein vernunftbasiertes System (rechts)
>white|black||9|11|br Das Lösen des gleichen Rätsels: Diese Beispiele sind an echten KI-Antworten angepasst. Das Begründungssystem verwendet mehr Zeit und Rechenleistung für das „Denken“, indem es vor der Ausgabe seiner endgültigen Antwort eine „Kette des Denkens“ (chain of thought) aufbaut.

![figure.3](images/fig1.3_AI_agent.png)

##### Abbildung 1.3: Eine illustrative Darstellung eines KI-Agenten
>white|black||9|11|br Ein KI-Modell (Mitte), das so konfiguriert wurde, dass es iterativ plant, urteilt und Tools nutzt, um reale Aufgaben zu bewältigen. Quelle: International AI Safety Report 2026.


Distillation kann somit eine kostengünstige und effiziente Methode sein, damit Modelle leistungsfähigere Fähigkeiten erlangen (‡82). Einige Forschende haben Distillation genutzt, um hochleistungsfähige Modelle mit nur 1,000 Beispielen zu verfeinern, die von state-of-the-art-Modellen generiert wurden (‡83). Da Distillation ein vorab vorhandenes Teacher-Modell erfordert, kann sie nicht direkt dazu verwendet werden, Fähigkeiten von state-of-the-art-Modellen weiterzuentwickeln. Allerdings kann sie die Verbreitung fortgeschrittener KI-Fähigkeiten beschleunigen, auch von Closed-Source-Modellen aus (‡84*).

Zusammen mit technologischen Fortschritten bei „distributed compute“ und dezentralisiertem Training (Ansätze, bei denen Entwickler mehrere Prozessoren, Server oder Rechenzentren nutzen, die zusammenarbeiten, um KI-Training oder -Inference durchzuführen (‡85, ‡86, ‡87)) wurde der Grad reduziert, in dem viele KI-Entwicklungsprojekte auf große, zentralisierte Recheninfrastruktur angewiesen sind. Dies ermöglicht es zunehmend auch weniger gut ausgestatteten Akteuren, leistungsfähige Systeme zu entwickeln und bereitzustellen.

###@ Updates zu KI-Agenten

Seit dem letzten Bericht (January 2025) haben Fortschritte darin, wie Entwickler KI-Modelle mit Tools kombinieren, die Entwicklung zunehmend leistungsfähiger KI-Agenten ermöglicht. KI-Agenten sind darauf ausgelegt, Ziele zu verfolgen, die häufig von Nutzern in natürlicher Sprache festgelegt werden. Um diese Ziele zu erreichen, erhalten sie Zugriff auf Tools, wie z. B. Speicher, eine Computer-Schnittstelle und Webbrowser. Diese Tools und der Code, der verwendet wird, um sie mit dem Modell zu kombinieren, werden als „Scaffolding“ bezeichnet; sie helfen KI-Agenten, autonom mit der Welt zu interagieren, Pläne zu schmieden, sich wichtige Details zu merken und Ziele zu verfolgen (‡88*, ‡89) – mit deutlich weniger Aufsicht oder Unterstützung durch Menschen. So ist beispielsweise Manus AI ein beliebter KI-Agent, der verschiedene Aufgaben automatisieren kann, darunter Websuche, Softwareentwicklung und Online-Käufe (‡90). Abbildung 1.3 zeigt ein einfaches Beispiel für einen KI-Agenten, der aus einem allgemeinen KI-Modell „brain“ besteht, das iterativ planen, Schlussfolgerungen ziehen und Tools für Speicher, Webbrowser-Nutzung und die Nutzung eines Computers einsetzen kann.

Die digitale Infrastruktur für KI-Agenten wächst (‡91), und sie sind zunehmend branchenübergreifend verbreitet (‡92, ‡93, ‡94). KI-Agenten wurden für Aufgaben wie Forschung (‡37), Softwareentwicklung (‡95), robotergestützte Steuerung (‡96) und Kundenservice (‡97) entwickelt. Laufende Forschung und Entwicklung haben zu kontinuierlich leistungsfähigeren und stärker autonomen KI-Agenten bzw. Multi-Agenten-Systemen geführt. Forschende haben geschätzt, dass die Komplexität von Software-Benchmark-Aufgaben, die KI-Agenten bewältigen können, sich ungefähr alle sieben Monate verdoppelt (siehe auch §1.2. Aktuelle Fähigkeiten) (‡98). Expertinnen und Experten argumentieren, dass zunehmend leistungsfähige KI-Agenten sowohl große Chancen als auch Risiken hervorrufen werden (‡99, ‡100*) (siehe §2.2.1. Zuverlässigkeitsherausforderungen).

###@ Beweislücken

Die wichtigsten Evidenzlücken im Zusammenhang mit dem allgemeinen Entwicklungsprozess von General- Purpose- AI- Systemen ergeben sich vor allem aus dem Mangel an öffentlich verfügbaren Informationen darüber, wie sie entwickelt werden. Einige Entwickler sind sehr transparent darüber, wie sie General- Purpose- AI- Systeme entwickeln (‡1, ‡101). Im Allgemeinen ist jedoch der Grad an öffentlichem und politikgestaltetem Wissen darüber begrenzt, wie die meisten fortgeschrittenen Modelle entwickelt, abgesichert, evaluiert und eingesetzt werden. Dies gilt insbesondere für intern eingesetzte AI- Systeme, die in AI- Unternehmen verwendet werden, aber nicht von externen Stakeholdern genutzt oder verstanden werden (‡102, ‡103). Diese eingeschränkte externe Sichtbarkeit schafft Herausforderungen für Transparenz und Aufsicht. Verschiedene Forschende haben auf eine begrenzte und uneinheitliche Transparenz in Bezug auf Trainingsdaten (‡104, ‡105, ‡106), General- Purpose- AI- Modelle (‡107, ‡108), AI- Agenten (‡92), Evaluierungen (‡109), Entwicklungspipelines (‡110) und Sicherheit (‡111) hingewiesen. Einschränkungen bei der externen Offenlegung sind manchmal erforderlich, um die Geschäftsgeheimnisse und das geistige Eigentum der Unternehmen zu schützen. Gleichzeitig erschwert geringe Transparenz es unabhängigen Forschenden und politischen Entscheidungsträgern, General- Purpose- AI- Modelle und -Systeme zu untersuchen.


