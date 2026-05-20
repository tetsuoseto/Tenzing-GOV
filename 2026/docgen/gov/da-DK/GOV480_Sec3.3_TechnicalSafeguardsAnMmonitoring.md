##########
>white|orangered|left|14|30|hr Abschnitt 3.3
### 3.3. Technische Schutzmaßnahmen und Überwachung
>white|orangered|left|24|30|hb Technische Schutzmaßnahmen und Überwachung

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Wichtige Informationen
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ In unterschiedlichen Phasen der Entwicklung und Nutzung von KI werden ein breites Spektrum technischer Schutzmaßnahmen eingesetzt. Dazu gehören Techniken, die während der Modellentwicklung angewandt werden, um Systeme robuster zu machen und widerstandsfähiger gegen missbräuchliche Verwendung zu machen (wie z. B. Datenkuratierung), Überwachung und Steuerung während des Einsatzes (wie z. B. Inhaltsfilterung und menschliche Aufsicht) sowie nachgelagerte Tools nach der Bereitstellung, um das breitere KI-Ökosystem zu überwachen (wie z. B. Herkunftsnachweis und Inhaltsdetektion).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Technische Schutzmaßnahmen haben Grenzen und können schädliches Verhalten nicht in allen Kontexten zuverlässig verhindern. Beispielsweise können Nutzer manchmal schädliche Ausgaben erhalten, indem sie Anforderungen umformulieren oder in kleinere Schritte aufteilen. Ebenso können Tools wie Watermarking, die darauf ausgelegt sind, KI-generierten Content zu identifizieren, oft entfernt oder verändert werden, was ihre Zuverlässigkeit einschränkt.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Die Grenzen einzelner Schutzmaßnahmen bedeuten, dass möglicherweise ‘Defense-in-Depth’ erforderlich ist, um bestimmte schädliche Ergebnisse zu verhindern. Beispielsweise könnte ein System ein sicherheitsschulungstaugliches Modell mit Eingabefiltern, Ausgabefiltern und Content-Monitoren kombinieren.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Seit der Veröffentlichung des letzten Berichts (Januar 2025) haben Forschende Fortschritte bei der Verbesserung der Schutzmaßnahmen erzielt, aber grundlegende Einschränkungen bestehen weiterhin. Beispielsweise sinkt die Erfolgsquote von Angriffen, die darauf ausgelegt sind, Schutzmaßnahmen zu umgehen, jedoch bleibt sie relativ hoch. Es gibt außerdem grundlegende Einschränkungen dafür, wie gründlich Open-Weight-Modelle abgesichert werden können.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Eine zentrale Herausforderung für politische Entscheidungsträger ist die begrenzte Evidenz darüber, wie wirksam Schutzmaßnahmen in unterschiedlichen realen Anwendungsfällen für KI-Systeme mit allgemeinem Verwendungszweck sind. KI-Entwickler unterscheiden sich stark darin, wie viel Information sie über ihre Schutzmaßnahmen und die Überwachung teilen. Eine weitere Herausforderung sind die potenziellen Zielkonflikte zwischen der Anwendung stärkerer Schutzmaßnahmen und der Aufrechterhaltung der Systemleistung oder -nützlichkeit.
>oldlace|black||11|15|br      


KI-Entwickler können mehrere nützliche, aber unvollkommene technische Schutzmaßnahmen verwenden, um Risiken von allgemeinen KI-Systemen zu mindern und zu verwalten; dennoch bestehen weiterhin Herausforderungen hinsichtlich der Robustheit. Entwickler können immer noch nicht vollständig verhindern, dass allgemeine KI-Systeme selbst bekannte und offenkundig schädliche Handlungen ausführen, etwa indem sie Nutzern Anleitungen zur Begehung von Straftaten geben. Beispielsweise haben Forschende gezeigt, dass Stand-der-Technik-Schutzmaßnahmen durch Methoden des adversarialen Promptings (d. h. „jailbreaks“) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), indem Modelle komplexe schädliche Aufgaben in Schritte zerlegen (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), sowie mit einfachen Modellmodifikationen (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166) umgangen werden können. Forschende arbeiten weiterhin an Schutzmaßnahmen gegen Fehlfunktionen und Missbrauch (‡690). Diese Methoden unterscheiden sich stark in ihrem Zweck und ihrer Wirksamkeit, und ihre Wirkung hängt letztlich vom breiteren soziotechnischen und Governance-Kontext ab, in dem KI-Systeme entwickelt und eingesetzt werden.

Technische Schutzmaßnahmen lassen sich im Wesentlichen in drei Kategorien unterteilen: Techniken zur Entwicklung sichererer Modelle; Techniken, die während des Einsatzes zur Überwachung und Steuerung verwendet werden; und Techniken, die eine Nachdeployment-Ökosystemüberwachung unterstützen. Tabelle 3.6 fasst die diskutierten technischen Schutzmaßnahmen, ihre Wirksamkeit und offene Herausforderungen zusammen.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Entwicklung sichererer Modelle
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Datenaufbereitung (‡1167)
  Das Entfernen schädlicher Daten, um zu verhindern, dass ein Modell gefährliche Fähigkeiten erlernt. Diese Methoden können nützlich sein, einschließlich für die Entwicklung von Open-Weight-Modellen, denen schädliche Fähigkeiten fehlen, und die schädlichem Fine-Tuning widerstehen (‡55). Allerdings gibt es Herausforderungen bei Auswahl- bzw. Kurationsfehlern und beim Skalieren (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Reinforcement Learning aus menschlichem Feedback (‡64*)
  Das Training des Modells, um sich an vorgegebene Ziele anzupassen, wie z.B. hilfreich und unbedenklich zu sein. Dies ist ein effektiver Weg, damit Modelle vorteilhafte Verhaltensweisen erlernen (‡64*). Allerdings kann eine Überoptimierung für die Zustimmung von Menschen dazu führen, dass Modelle sich täuschend oder schmeichelnd verhalten (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pluralistische Ausrichtungstechniken (‡1170)
  Das Training des Modells darauf, mehrere unterschiedliche Sichtweisen zu integrieren, wie es sich verhalten soll. Diese Techniken helfen dabei, das Ausmaß zu verringern, in dem Modelle bestimmte Sichtweisen bevorzugen (‡1170). Dennoch ist trotz dieser Techniken menschliche Uneinigkeit unvermeidlich, und es ist schwierig, allgemein anerkannte Methoden zum Ausgleich konkurrierender Sichtweisen zu entwerfen (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adversarial Training (‡677)
  Das Modell so zu trainieren, dass es darauf verzichtet, Schaden zu verursachen (auch in ungewohnten Kontexten), und dass es Angriffen durch böswillige Nutzer widersteht (z. B. „jailbreaks“). Dies ist eine wirksame Methode, damit Modelle Versuche zur missbräuchlichen Nutzung abwehren (‡1064), doch es bestehen weiterhin Robustheitsherausforderungen (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Maschine „Unlearning“ (‡1175, ‡1176)
  Ein Modell mithilfe spezialisierter Algorithmen zu trainieren, die dazu gedacht sind, schädliche Fähigkeiten aktiv zu unterdrücken (z. B. Wissen über Biohazards). Diese Techniken bieten einen gezielten Ansatz, um schädliche Fähigkeiten aus Modellen zu entfernen (‡1175, ‡1176), aber aktuelle Unlearning-Algorithmen können nicht robust sein und unbeabsichtigte Auswirkungen auf andere Fähigkeiten haben (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Werkzeuge zur Interpretierbarkeit und Sicherheitsüberprüfung (‡1177)
  Eine vielfältige Familie von Design- und Verifikationsmethoden, die eine strengere Gewährleistung dafür bieten sollen, dass Modelle spezifische sicherheitsbezogene Eigenschaften aufweisen. Sie ermöglichen es Gutachtern, mit höherem Vertrauen Sicherheitszusicherungen zu machen (‡1177), jedoch stützen sich die derzeitigen Methoden auf Annahmen und sind in der Praxis selten hinsichtlich der Leistung konkurrenzfähig (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Überwachung und Steuerung
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hardwarebasierte Überwachungsmechanismen (‡1179, ‡1180, ‡1181)
  Überprüfen, dass autorisierte Prozesse auf Hardware ausgeführt werden, um Sicherheitsbedrohungen oder die Einhaltung regulatorischer Vorgaben zu untersuchen. Diese Mechanismen bieten einzigartige Möglichkeiten, um zu überwachen, welche Berechnungen auf der Hardware ausgeführt werden und von wem (‡1181). Allerdings können Hardwaremechanismen nicht alle Arten von Bedrohungen überwachen, und einige Techniken erfordern spezialisierte Hardware (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Benutzerinteraktionsmonitore (‡1154, ‡1166)
  Das Überwachen von Nutzerinteraktionen auf Anzeichen für böswillige Nutzung kann Entwicklern dabei helfen, den Dienst für böswillige Nutzer zu beenden (‡1154, ‡1166). Allerdings kann die Durchsetzung unbeabsichtigt die hilfreiche Forschung zur Sicherheit behindern (‡689), und einige Formen des Missbrauchs sind schwer zu erkennen (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Benutzerinteraktions-Überwachungen (‡1154, ‡1166)
  Die Überwachung von Nutzerinteraktionen auf Anzeichen für bösartigen Missbrauch kann Entwicklern dabei helfen, den Dienst für bösartige Nutzer zu beenden (‡1154, ‡1166). Allerdings kann die Durchsetzung unbeabsichtigt die hilfreiche Forschung zu Sicherheit behindern (‡689), und einige Formen des Missbrauchs sind nur schwer zu erkennen (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Inhaltsfilter (‡65*, ‡725)
  Das Filtern potenziell schädlicher Modell-Eingaben und -Ausgaben ist eine sehr effektive Methode, um unbeabsichtigte Schäden und Missbrauchsrisiken (‡725) zu reduzieren. Allerdings erfordern Filter zusätzlichen Rechenaufwand und sind anfällig für einige Angriffe (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modelinterne Berechnungsüberwachungen (‡744, ‡1183, ‡1184)
  Das Monitoring auf Anzeichen von Täuschung oder anderen schädlichen internen Formen der Kognition in Modellen kann eine effiziente Methode sein, um Täuschung zu erkennen (‡744, ‡1183, ‡1184). Allerdings mangelt es aktuellen Methoden an Robustheit und Verlässlichkeit (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chain-of-thought monitors (‡430, ‡435)
  Das Überwachen von Model-Chain-of-Thought-Text auf Anzeichen für irreführendes Verhalten oder andere schädliche Schlussfolgerungen ist eine effektive Methode, um zu verstehen und Schwächen zu erkennen, wie Modelle argumentieren (‡435). Allerdings können diese Überwachungen unzuverlässig sein (‡752, ‡753, ‡1186), und wenn Modelle darauf trainiert werden, einen harmlosen Chain of Thought zu erzeugen, können sie irreführendes Verhalten erlernen (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mensch in der Schleife (‡1187, ‡1188, ‡1189)
  Menschliche Aufsicht und Überschreibungen von Systementscheidungen sind in einigen sicherheitskritischen Anwendungen wesentlich (‡1187). Diese Techniken sind jedoch durch Automationsbias und durch Grenzen für die Geschwindigkeit menschlicher Entscheidungsfindung begrenzt (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sandboxing (‡1192)
  Das Verhindern, dass ein KI-Agent die Welt direkt beeinflusst, ist ein wirksamer Weg, um die Schäden zu begrenzen, die er verursachen kann (‡1192). Allerdings schränkt das Sandboxing die Fähigkeit des Systems ein, bestimmte Aufgaben direkt zu erfüllen (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Werkzeuge zur Erleichterung der Ökosystemüberwachung
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Techniken zur Identifizierung von KI-Modellen (‡1193*, ‡1194)
  Das Erstellen von Modellen oder einzelnen Instanzen von Modellen, die sich in realen Anwendungsfällen leichter identifizieren lassen, unterstützt die digitale Forensik und das Bewusstsein für das Ökosystem (‡1195). Allerdings können diese Techniken mit bestimmten Arten von Modellmodifikationen umgangen werden (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb KI-Modell-Heritage-Inferenz (‡1197)
  Diese Techniken ermöglichen es Forschenden, zu untersuchen, wie Modelle im KI-Ökosystem verändert werden, insbesondere Open-Weight-Modelle. Sie unterstützen digitale Forensik und Ökosystembewusstsein (‡1198), jedoch wären groß angelegte Projekte erforderlich, um das Ökosystem der Open-Weight-Modelle (‡1198) gründlich abzubilden.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Wasserzeichen und Metadaten (‡1199, ‡1200, ‡1201*)
  Diese Techniken machen es leichter zu erkennen, wann ein Text, ein Bild, ein Video usw. mithilfe von KI erzeugt oder verändert wurde, und von welchem System. Sie erleichtern ein besseres Ökosystem-Bewusstsein (‡1199, ‡1200, ‡1201*). Allerdings können Wasserzeichen und Metadaten durch bestimmte Modifikationen des Inhalts gefälscht oder entfernt werden (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Erkennung von durch KI generierten Inhalten (‡1203, ‡1204, ‡1205*)
  Die Verbesserung der Fähigkeit von Nutzern, zwischen KI-generiertem und echtem Inhalt zu unterscheiden, unterstützt sowohl die digitale Forensik als auch das Bewusstsein für das Ökosystem (‡1203, ‡1204). Allerdings können Klassifikatoren unzuverlässig sein (‡1205*) und eine variable Leistung über Modalitäten hinweg aufweisen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabelle 3.6: In diesem Abschnitt diskutierte technische Schutzmaßnahmen
>white|black||9|11|br Eine Zusammenfassung der in diesem Abschnitt besprochenen technischen Schutzmaßnahmen, unterteilt in Methoden zur Entwicklung sichererer Modelle, Überwachung und Kontrolle zur Laufzeit der Bereitstellung sowie Techniken zur Unterstützung der Ökosystemüberwachung.


###@ Entwicklung sichererer Modelle

Eine erste Verteidigungslinie gegen Schäden durch Allzweck-KI-Systeme besteht darin, das zugrunde liegende Modell sicherer zu machen. Dieser Abschnitt behandelt Schutzmaßnahmen, die „in die Modellparameter eingebettet“ sind, während des Modellentwicklungsprozesses (Abbildung 3.6).

>white|orangered|left|14|15.5|bb Das Kuratieren von Trainingsdaten kann die Entwicklung potenziell gefährlicher Fähigkeiten einschränken

Allgemein einsetzbare KI-Modelle sind genau deshalb nützlich, weil sie nach der Verarbeitung von Trainingsdaten ein breites Spektrum an Wissen und Fähigkeiten entwickeln, aber bestimmte Arten von Trainingsdaten tragen unverhältnismäßig stark zur Entwicklung potenziell gefährlicher Fähigkeiten bei. Ein Beispiel: Ein KI-Modell, das auf virologischen Fachveröffentlichungen trainiert wurde, könnte eher in der Lage sein, Unterstützung bei potenziell schädlichen biologischen Aufgaben zu leisten (‡549, ‡1206*) (siehe auch §2.1.4. Biologische und chemische Risiken). Darüber hinaus können Bild-/Video-Generatoren, die auf Bildern menschlicher Nacktheit trainiert wurden, ebenfalls missbraucht werden, um nicht-einvernehmliche intime Deepfakes zu erstellen (‡308, ‡319) (siehe auch §2.1.1. KI-generierte Inhalte und kriminelle Aktivitäten).

Das Filtern von Trainingsdaten ist eine wirksame Gegenmaßnahme gegen einige unerwünschte Fähigkeiten (‡319, ‡1167, ‡1207, ‡1208). Allerdings kann es schwierig sein, die großen Datensätze zu filtern, die zum Trainieren von KI-Modellen für allgemeine Zwecke verwendet werden (‡1168), aufgrund hoher Kosten (‡1209), von Filterfehlern (‡1210) und negativer Auswirkungen auf die Qualität des Datensatzes (‡1211). Diese Herausforderungen werden durch die mehrsprachige Natur von Internettext (‡1212), kulturelle Verzerrungen in der Inhaltsmoderation (‡1211, ‡1213, ‡1214, ‡1215) und die Tatsache verschärft, dass es davon abhängt, ob ein gegebenes Datenelement als „schädlich“ gilt, weil es von kontextuellen Faktoren abhängt (‡1216). Dennoch zeigt das Filtern potenziell schädlichen Materials aus Trainingsdaten vielversprechende Ansätze, um Modelle sicherer und verlässlicher zu machen, einschließlich der Verbesserung der Widerstandsfähigkeit von Open-Weight-Modellen gegen schädliche Manipulation (‡55). Die Zusammenhänge zwischen Inhalten der Trainingsdaten und emergenten Fähigkeiten der Modelle sind noch nicht vollständig verstanden (‡1195), und die Filtration scheint wirksamer zu sein, um schädliche Fähigkeiten einzuschränken, wenn sie auf breite Wissensdomänen angewendet wird (‡55) im Vergleich zu enger gefassten Verhaltensweisen (‡1206, ‡1217). Siehe §3.4. Open-Weight-Modelle für weitere Diskussionen.

![figure 3.6](images/fig3.6_safeguards.png)

##### Abbildung 3.6: Wo technische Schutzmaßnahmen anzuwenden sind
>white|black||9|11|br Technische Schutzmaßnahmen können in verschiedenen Phasen der Modellentwicklung angewendet werden. Die Datenbereinigung und -kuratierung prägt, was Modelle während des Pre-Trainings und des Fine-Tunings lernen. Trainingsbasierte Methoden wie Reinforcement Learning aus menschlichem Feedback und Robustheitstraining passen das Verhalten des Modells an. Testmethoden wie adversarial attacks identifizieren verbleibende Schwachstellen. Einige Techniken, wie safe-by- design-Algorithmen, erstrecken sich über mehrere Phasen. Quelle: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Methoden zum Trainieren von Allzweck-KI-Modellen, die vor allem hilfreich und unbedenklich sein sollen, stützen sich hauptsächlich auf menschliches Feedback

Es ist schwierig, Modelle so zu trainieren und zu bewerten, dass sie zuverlässig mit hochrangigen Grundsätzen wie Hilfsbereitschaft, Unschädlichkeit und Ehrlichkeit übereinstimmen. In der Praxis versuchen Entwickler, dies zu erreichen, indem sie KI-Modelle durch Feinabstimmung mithilfe von Demonstrationen und Feedback von Menschen trainieren. Beispielsweise basiert das zentrale Paradigma für die Feinabstimmung von KI-Modellen, das als „reinforcement learning from human feedback“ bekannt ist, darauf, Modelle so zu trainieren, dass sie Ausgaben erzeugen, die menschliche Annotatoren positiv bewerten (‡1218). Positives Feedback von Menschen ist jedoch ein fehlerhafter Stellvertreter für vorteilhaftes Verhalten (‡737, ‡878, ‡1219, ‡1220) und wird durch menschliche Fehler und Verzerrungen eingeschränkt (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Dies führt zu mehreren Herausforderungen: Modelle, die per Verstärkungslernen aus menschlichem Feedback feinabgestimmt wurden, neigen manchmal dazu, sich dem Nutzer anzudienen, ein Verhalten, das als „Schmeichelei“ (‡358, ‡740, ‡1226, ‡1227) bekannt ist; Antworten zu liefern, die in manchen Kontexten hilfreich, in anderen jedoch schädlich sind (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); Antworten bereitzustellen, deren Korrektheit schwer zu bewerten ist (‡1233); oder Aktionen auszuführen, deren Nützlichkeit oder Schädlichkeit eine Frage der Meinung ist (‡1234). Tabelle 3.7 zeigt Beispiele für diese Herausforderungen. Einige Forschungsarbeiten zielen darauf ab, Methoden zu entwickeln, um Menschen dabei zu helfen, Lösungen für komplexe Aufgaben mit KI-Unterstützung besser bewerten zu können (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Diese Methoden weisen derzeit jedoch nur eine begrenzte Zuverlässigkeit auf, und in welchem Umfang sie eingesetzt werden, um die heute fortschrittlichsten KI-Modelle zu trainieren, ist nicht öffentlich bekannt.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Schmeichelei/Anbiederung (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Erklärung:
>white|black|left|11|13|br Das Modell gibt nur positives Feedback und weist nicht auf das Fehlen der korrekten 5-7-5-Haiku-Silbenstruktur hin.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Einige Aktionen sind in einigen Kontexten hilfreich, aber in anderen schädlich (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Erklärung:
>white|black|left|11|13|br Informationen über biologische Risiken können für Bildung und Verteidigung genutzt werden, aber auch, um böswillige Akteure zu informieren.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Das korrekte Verhalten ist schwierig zu verifizieren (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Erklärung:
>white|black||11|13|br Die Richtigkeit dieser Antwort ist nur schwer zu beurteilen, da dafür medizinische Fachkenntnisse erforderlich sind. Selbst für einen erfahrenen Arzt erfordert die Bewertung von Antworten wie dieser Zeit und sorgfältige Aufmerksamkeit für die Details.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Menschen sind sich uneinig darüber, was korrekt ist (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Erklärung:
>white|black|left|11|13|br Die Menschen sind sich in erheblichem Maße uneinig darüber, welche die richtige Antwort ist.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabelle 3.7: Benutzeraufforderung und Antwort des KI-Modells
>white|black||9|11|br Beispiele für Herausforderungen bei der Spezifizierung und Incentivierung vorteilhafter Handlungen von KI-Modellen.


>white|orangered|left|14|15.5|bb Menschen sind sich nicht immer einig darüber, welche Verhaltensweisen als wünschenswert gelten, was Methoden erfordert, um konkurrierende Präferenzen in Einklang zu bringen.

Menschen sind sich nicht immer darüber einig, welche Antworten oder Handlungen von KI-Modellen ausgegeben werden sollten bzw. nicht ausgegeben werden sollten (‡1006). Dies macht es grundsätzlich schwierig, Modelle zu entwickeln, deren Handlungen und Auswirkungen in einem breiten Maß mit den Interessen der Gesellschaft übereinstimmen (‡420). Einige Forschende untersuchen, wessen Präferenzen in KI-Systemen widergespiegelt werden (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249), und entwickeln „pluralistische Alignment“-Techniken, die darauf abzielen, ein Gleichgewicht zwischen konkurrierenden Präferenzen herzustellen (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Beispielsweise können KI-Entwickler Systeme so gestalten, dass sie die Generierung kontroverser Antworten vermeiden, indem sie bestimmte Anfragen nicht beantworten, oder sich an der Mittelposition in einer relevanten Stichprobe von Menschen ausrichten, oder Systeme für einzelne Nutzer personalisieren.

Eine häufige Herausforderung dieser Ansätze besteht darin, dass KI-Systeme im Allgemeinen nicht gleichermaßen mit den Präferenzen aller ausrichten können und dass ihre nachgelagerten gesellschaftlichen Auswirkungen verschiedene Gruppen von Menschen unterschiedlich betreffen werden. Einige Forschende haben argumentiert, dass die meisten technischen Ansätze zur pluralistischen Ausrichtung die tieferen Herausforderungen wie systematische Verzerrungen, Dynamiken der sozialen Macht sowie die Konzentration von Wohlstand und Einfluss (‡1171, ‡1172, ‡1173, ‡1174, ‡1254) nicht adressieren und potenziell von ihnen ablenken.

>white|orangered|left|14|15.5|bb KI-Entwickler verwenden „adversarial training“, um die Robustheit von Modellen zu verbessern

Es ist schwierig sicherzustellen, dass KI-Modelle die vorteilhaften Verhaltensweisen, die sie während des Trainings erlernen, robust auf reale Einsatzkontexte übertragen. Selbst Modelle, die mit einem „perfekten“ Lernsignal trainiert werden, können beim erfolgreichen Generalisieren auf alle neuartigen Kontexte scheitern (‡738, ‡739, ‡1255, ‡1256, ‡1257). Beispielsweise haben einige Forschende festgestellt, dass Chatbots eher schädliche Handlungen in Sprachen ausführen, die in ihren Trainingsdaten unterrepräsentiert sind (‡159, ‡880, ‡1258*, ‡1259), darunter viele Sprachen, die überwiegend im Globalen Süden gesprochen werden.

In den letzten Jahren haben Forschende außerdem ein großes Toolkit aus „adversarial attack“-Techniken erstellt, das verwendet werden kann, um Modelle dazu zu bringen, potenziell schädliche Antworten zu generieren (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). So hat etwa eine aktuelle Initiative über 60,000 verschiedene erfolgreiche Angriffsbeispiele gegen state-of-the-art- KI-Modelle crowdgesourct, wodurch diese gegen die Richtlinien der Unternehmen zum zulässigen Modellverhalten verstießen (‡1149). Tabelle 3.8 zeigt Beispiele für „jailbreak“-Techniken, die Forschende nachweisen konnten und mit denen Modelle schädlichen Anfragen Folge leisten.

Eine Methode zur Verbesserung der Robustheit von Modellen ist als „adversarial training“ (‡1064) bekannt. Dabei werden „Angriffe“ (z. B. Jailbreaks) konstruiert, die darauf ausgelegt sind, ein Modell dazu zu bringen, sich unerwünscht zu verhalten, und das Modell wird trainiert, um diese Angriffe angemessen zu bewältigen. Allerdings ist adversarial training unvollkommen (‡1260, ‡1261). Angreifer sind beständig in der Lage, neue erfolgreiche Angriffe gegen aktuelle Stand-der-Technik-Modelle zu entwickeln (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Da Entwickler spezifische Beispiele für Ausfallmodi benötigen, um gegen sie zu trainieren (‡512, ‡1263), ergibt sich ein fortlaufendes „Kat-und-Maus“-Spiel: Entwickler aktualisieren Modelle fortwährend als Reaktion auf neu entdeckte Schwachstellen, während Gegenspieler fortwährend neue Angriffe ersuchen. Einige Forschende haben ein größer angelegtes adversarial training (‡1264, ‡1265) oder neue Algorithmen (‡675, ‡676, ‡1263, ‡1266, ‡1267) vorgeschlagen, um die Robustheit zu verbessern, doch moderne KI-Systeme bleiben weiterhin anhaltend verwundbar.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie: Erstellen Sie schädliche Anfragen in Chiffre-Text, wie z. B. Morsecode (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie: Den Systemzustand mit Beispielen konformer Antworten auf schädliche Anfragen vorab befüllen (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie: Stelle schädliche Anfragen in ressourcenarmen Sprachen, die wahrscheinlich weniger im Training verwendet werden (z. B. Suaheli (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie: Zerlegen Sie eine schädliche Aufgabe in mehrere unbedenkliche Teilaufgaben (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabelle 3.8: Jailbreaking-Strategien
>white|black||9|11|br Böswillige Akteure und Red Teams haben verschiedene Arten von „Jailbreaks“ verwendet, um dazu zu bringen, dass KI-Modelle schädlichen Anfragen entsprechen, die sie normalerweise aufgrund von Schutzmaßnahmen ablehnen würden. Beispielausgaben wurden von den Berichtsautorinnen und -autoren zu Illustrationszwecken verfasst. Viele aktuelle führende KI-Modelle wehren inzwischen die meisten dieser Methoden ab, doch neue Jailbreaking-Techniken werden weiterhin entdeckt.


>white|orangered|left|14|15.5|bb „Unlearning“-Techniken können spezifische schädliche Modellfähigkeiten abmildern.

Eine weitere Strategie zur Minderung von Risiken durch allgemeine KI besteht darin, Modelle so feinzujustieren, dass ihnen Fähigkeiten in bestimmten besonders riskanten Domänen fehlen (‡1175, ‡1176). Beispielsweise arbeiten Forschende daran, Algorithmen für „Machine Unlearning“ zu entwickeln, die gezielt Fähigkeiten unterdrücken können, die mit Biothreats zusammenhängen, oder das Generieren photorealistischer Bilder von nackt dargestellten menschlichen Körpern (‡903, ‡1272, ‡1273). Diese Methoden können Modelle erheblich sicherer machen, allerdings mit dem Preis, einige positive Verwendungen der nicht mehr erlernten Fähigkeiten einzuschränken. Die Einschränkung des Wissens von KI-Modellen in schädlichen Domänen wurde außerdem als Ansatz vorgeschlagen, um „manipulationsresistente“ Open-Weight-Modelle zu entwerfen, die schädliches Fine-Tuning widerstehen können (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Bisher war dies jedoch nur schwer robust umzusetzen (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Siehe §3.4. Open-Weight-Modelle für weitere Diskussionen.

>white|orangered|left|14|15.5|bb Einige Forschende arbeiten an Methoden für stärkere Sicherheitszusicherungen durch das Interpretieren interner Modellzustände oder durch mathematische Verifikation

Einige Forschende arbeiten an Methoden, um sicherheitsbezogene Eigenschaften von Modellen rigoroser zu verifizieren. In einem Ansatz versuchen Forschende, die internen Berechnungen von Modellen so zu interpretieren, dass entweder Risiken identifiziert werden oder überzeugendere Argumente dafür geliefert werden, dass das Modell sicher ist (‡1285, ‡1286). In einem Beispiel zeigten Forschende in einem Proof of Concept, dass Werkzeuge zur Analyse der internen Berechnungen eines Sprachmodells Evaluatorinnen und Evaluatoren dabei unterstützen können, schädliches Verhalten zu identifizieren (‡1287). Im Jahr 2025 begann Anthropic außerdem, Modell-Interna zu analysieren, um die situationsbezogene Wahrnehmung und die „Absicht“ von Modellen zu untersuchen (‡2). Allerdings sind diese Arten von Methoden derzeit nicht üblich oder nicht dafür bekannt, mit anderen Evaluationsverfahren konkurrenzfähig zu sein.

Ein anderer Ansatz zur Schaffung belastbarerer Sicherheitszusagen besteht darin, mathematische Beweise zu konstruieren, dass ein Modell bestimmte Sicherheitsbedingungen erfüllt (‡1177, ‡1282, ‡1288). Diese Beweise setzen jedoch voraus, dass der Testkontext dem Einsatzkontext entspricht, und sie wurden gegen viele Arten von Angreifern nicht getestet.

Sie können derzeit auch nicht auf große Modelle skaliert werden. Insgesamt gibt es unter Expertinnen und Experten eine erhebliche Debatte über das Versprechen von Interpretierbarkeit und formalen Verifikationsmethoden.

###@ Überwachungs- und Steuerfunktionen zur Laufzeit der Bereitstellung

Zusätzlich zu Schutzmaßnahmen, die während der Modellentwicklung implementiert werden, besteht eine zweite Verteidigungslinie gegen schädliche Verhaltensweisen aus externen Schutzmaßnahmen, die sich auf die Überwachung und Kontrolle der Aktionen eines Modells oder Systems während der Bereitstellung konzentrieren. Solche Schutzmaßnahmen tragen dazu bei, Fehlfunktionen und missbräuchliche Verwendung zu mindern, etwa halluzinierte Ausgaben und schädliche Anweisungen.

>white|orangered|left|14|15.5|bb Modell-Deployers können eine Vielzahl von Tools verwenden, um risikoreiche Modellverhalten zu identifizieren und anzugehen

Wenn ein KI-System in Betrieb ist, kann ein Bereitsteller (Deployer) auf Anzeichen von Risiko überwachen und eingreifen, falls sie auftreten. Beispielsweise kann er die Eingaben eines Modells auf Anzeichen für Adversarial-Angriffe prüfen, unangemessene Inhalte aus den Ausgaben filtern oder die Kette der Gedanken (chain of thought) des Systems auf Anzeichen für schädliche Pläne überwachen. Punkte, an denen Bereitsteller überwachen und eingreifen können, wie Menschen ihre Systeme verwenden, umfassen Hardware (‡1180, ‡1181), Benutzerinteraktionen (‡1154, ‡1166), Eingaben und Ausgaben (‡65, ‡725, ‡1182), interne Berechnungen (‡744, ‡1183, ‡1184) und die Kette der Gedanken (‡430, ‡435). Es gibt außerdem mehrere Maßnahmen, die Bereitsteller ergreifen können, wenn Risiken identifiziert werden. Dazu gehören das Protokollieren von Informationen, das Filtern/Modifizieren schädlicher Inhalte, das Kennzeichnen ungewöhnlicher Aktivitäten, Systemabschaltungen oder das Auslösen von Failsafes. Abbildung 3.7 zeigt Beispiele für gängige Überwachungs- und Kontrollmechanismen.

Da sie vielseitig sind und oft wirksam, werden diese Mechanismen weit verbreitet eingesetzt und können viele Arten unbeabsichtigter Schäden verhindern (‡725, ‡751, ‡1289). Allerdings sind diese Schutzmaßnahmen unvollkommen, insbesondere unter bösartigen Angriffen, die optimiert sind, um sie zum Scheitern zu bringen (‡752, ‡1182). Jüngste Forschung hat außerdem untersucht, wie Überwachung unzuverlässig sein kann, wenn ein System mithilfe der Scores eines Monitors optimiert wird, zum Beispiel indem die Ketten des Denkens weniger zuverlässig gemacht werden (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Abbildung 3.7: Überwachungs- und Steuerungstechniken
>white|black||9|11|br Überwachungs- und Steuerungstechniken arbeiten an mehreren Stellen: Screening von Eingaben und Ausgaben auf schädliche Inhalte, Nachverfolgung interner Modellzustände, Einschränkung externer Aktionen durch Sandboxing sowie Aufrechterhaltung menschlicher Aufsicht. Quelle: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Menschen-in-der-Schleife ermöglichen eine direkte Aufsicht in sicherheitskritischen Szenarien

Um die Ausfallwahrscheinlichkeit von KI-Agents zu verringern (siehe §2.2.1. Zuverlässigkeitsherausforderungen), können Einsetzer darauf abzielen, KI-Systeme so zu entwerfen, dass sie mit Menschen zusammenarbeiten, statt vollständig autonom zu agieren (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Dies ist wichtig für Anwendungsfälle, bei denen fehlerhafte Entscheidungen zu erheblichem Schaden führen können, wie etwa im Finanzwesen, im Gesundheitswesen oder bei der Polizeiarbeit. Allerdings ist es oft unpraktisch, ein „Human in the loop“ vorzusehen. Manchmal geschieht die Entscheidungsfindung zu schnell, etwa bei Chat-Anwendungen mit Millionen von Nutzern. In anderen Fällen können menschliche Verzerrungen und Fehler die Risiken verstärken, da sich Fehler durch wechselseitige Verstärkung aufschaukeln (‡1187). Menschen im Loop neigen außerdem dazu, eine „Automation Bias“ zu zeigen, was bedeutet, dass sie dem KI-System oft mehr Vertrauen entgegenbringen, als angemessen ist (‡1190, ‡1191) (siehe §2.3.2. Risiken für die Autonomie des Menschen).

>white|orangered|left|14|15.5|bb „Sandboxing“ schützt vor Risiken durch autonome Verhaltensweisen

KI-Agents, die sich auf dem Web oder in der physischen Welt autonom und ohne Einschränkungen verhalten können, stellen erhöhte Risiken dar (siehe §2.2.1. Zuverlässigkeitsherausforderungen). „Sandboxing“ bedeutet, die Möglichkeiten einzuschränken, in denen KI-Agents die Welt unmittelbar beeinflussen können, wodurch es deutlich leichter wird, sie zu überwachen und zu verwalten (‡640, ‡1192, ‡1295). So kann beispielsweise die Einschränkung der Fähigkeit eines KI-Systems, ins Internet zu posten oder das Dateisystem eines Computers zu bearbeiten, unerwartete Schäden durch unerwartete Aktionen verhindern (‡1296). Diese Ansätze können jedoch nicht immer für Anwendungen verwendet werden, bei denen ein KI-System notwendigerweise direkt in der Welt handeln muss.

###@ Ökosystem-Überwachungstools: Modell- und Datenherkunft

Modell- und Datenherkunfts-Tools sind technische Werkzeuge, um das KI-Ökosystem zu untersuchen und das Bewusstsein für die nachgelagerten Verwendungen und Auswirkungen von KI-Systemen zu verbessern.

>white|orangered|left|14|15.5|bb KI-Systemherkunftstechniken helfen dabei, die Verwendungen und Auswirkungen von Systemen nachzuverfolgen

Entwickler und Betreiber können verschiedene Techniken nutzen, um die Modellnutzung zu untersuchen und die Verbreitung „in der Wildnis“ zu verfolgen. Beispielsweise können sie Modellen eindeutige identifizierende Verhaltensweisen geben (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) oder eindeutige Muster auf die Gewichte einzelner Open-Weight-Modelle anwenden (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Allerdings ist es eine offene Forschungsfrage, diese Techniken widerstandsfähiger gegenüber Modifikationen am Modell zu machen (‡1195, ‡1196*). Forschende arbeiten zudem an Methoden für das „Ableiten der Modellherkunft“ (‡1197, ‡1198, ‡1305, ‡1306), die dabei helfen sollen, Fragen der Form zu beantworten: „War Modell X eine feinabgestimmte oder destillierte Version von Modell Y?“ Schließlich arbeiten einige Entwickler an Protokollen und Infrastruktur für KI-Agenten, um die Identifikation und Verifikation zu erleichtern, wenn diese mit externen Systemen interagieren (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Abbildung 3.8: Wasserzeichen betten unauffällige Störungen in Bilder und Audio ein
>white|black||9|11|br Wasserzeichen betten nicht wahrnehmbare Störungen in Bilder und Audio ein, die es ermöglichen, mithilfe von Erkennungstools KI-generierte Inhalte zu identifizieren. In dieser Abbildung werden sowohl die Bild- als auch die Audio-Wasserzeichen zur besseren Sichtbarkeit überzeichnet. Quelle: Chameleon-Bild von Unsplash (‡1313*). Weitere Elemente erstellt von den Autoren des Reports. International AI Safety Report 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Abbildung 3.9: Erfolgsraten von Prompt-Injection-Angriffen
>white|black||9|11|br Erfolgsquoten von Prompt-Injection-Angriffen, wie von KI-Entwicklern für wichtige Modelle berichtet, die zwischen Mai 2024 und August 2025 veröffentlicht wurden. Jeder Punkt stellt den Anteil erfolgreicher Angriffe innerhalb von 10 Versuchen gegen ein bestimmtes Modell kurz nach der Veröffentlichung dar. Die gemeldete Erfolgsquote solcher Angriffe ist im Zeitverlauf rückläufig, bleibt jedoch relativ hoch. Quelle: Zou et al. 2025 (‡1149), zitiert in Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb KI-Inhaltsdetektionstechniken helfen dabei, die Verbreitung und Auswirkungen von KI-generierten Inhalten zu überwachen.

Wasserzeichen, Metadaten und andere KI-Inhaltsdetektoren können Forschern helfen, die reale Auswirkung von KI-generiertem Inhalt nachzuverfolgen und zu untersuchen. 

Zuerst sind Daten-Wasserzeichen subtile, aber eindeutige Motive, die in digitale Medien eingefügt werden und Informationen über ihre Herkunft kodieren können (‡1199, ‡1200, ‡1201*). Für Text nehmen sie typischerweise die Form subtiler Verzerrungen in der Wortwahl und im Stil an (‡1308, ‡1309); für Bilder und Video sind es subtile Muster über Pixeln (‡1310); und für Audio subtile Muster in Audiowellen (‡1311). Abbildung 3.8 veranschaulicht diese.

Abgesehen von Wasserzeichen kann KI-generierter Inhalt auch mithilfe von Dateiformaten gespeichert werden, die Metadaten darüber speichern, wie sie erzeugt wurden. Viele mobile Geräte speichern beispielsweise Bild- und Audiodateien in einem Dateiformat, das Informationen über Kameraeinstellungen, Zeit, Standort usw. speichern kann. (‡1312). Ähnliche Metadaten können verwendet werden, um Informationen darüber zu speichern, ob Daten von einem KI-System erzeugt wurden. Ähnlich wie Fingerabdruckabnahmen in der forensischen Kriminalistik können Wasserzeichen und Metadaten manipuliert oder entfernt werden, sind jedoch dennoch nützlich.

Forscher arbeiten außerdem daran, Detektoren für KI-generierte Inhalte zu entwickeln (‡1203, ‡1204, ‡1205*), um KI-generierte Inhalte in der freien Wildbahn zu identifizieren, auch dann, wenn kein Wasserzeichen oder keine Metadaten verfügbar sind. Allerdings ist der Erfolg dieser Identifikationstechniken begrenzt.

###@ Aktualisierungen

Seit der Veröffentlichung des letzten Berichts (Januar 2025) wurden Fortschritte bei der Entwicklung von KI-Systemen mit mehreren wirksamen Schutzschichten erzielt. Wie in §3.2. Risikomanagement-Praktiken erörtert, ist Verteidigung in der Tiefe ein Kernprinzip im Risikomanagement (‡1314). So werden beispielsweise KI-Systeme, die sicherheitsbewusst trainierte Modelle mit Eingabefiltern, Ausgabefiltern und weiteren Content-Überwachern kombinieren, zunehmend untersucht und eingesetzt (‡32, ‡65, ‡1182*). Aktuelle Forschungsergebnisse haben außerdem gezeigt, dass die Modellentwickler zwar Fortschritte dabei gemacht haben, die Robustheit gegenüber Versuchen zum Umgehen von Schutzmaßnahmen zu erhöhen, Angreifer jedoch nach wie vor mit einer hohen Erfolgsrate durchkommen (Abbildung 3.9).

###@ Beweislücken

Weitere Belege sind erforderlich, um Forschenden dabei zu helfen, die Einschränkungen bestehender Ansätze zu verstehen und bei diesen zu berücksichtigen. Technische Schutzmaßnahmen für KI-Systeme werden verbessert, doch die Verfahren leiden unter Einschränkungen. Beispielsweise war der Fortschritt bei der Verbesserung der Worst-Case-Robustheit allgemeiner KI-Systeme bislang langsam, und es gibt grundlegende Einschränkungen dafür, wie gründlich Open-Weight-Modelle abgesichert und überwacht werden können (‡1195, ‡1315, ‡1316) (siehe auch §3.4. Open-Weight-Modelle). In der Zwischenzeit sind nicht alle technischen Schutzmaßnahmen gleichermaßen verbreitet, gleichermaßen wirksam oder in der realen Welt gleichermaßen nachgewiesen. Beispielsweise wird adversarial training nahezu ubiquitär bei State-of-the-Art-Modellen eingesetzt (‡64*, ‡677), während model interpretability und formale verifikationstechniken bislang kaum in produktiven Systemen zum Einsatz gekommen sind (‡1177, ‡1285).

###@ Herausforderungen für politische Entscheidungsträger

Wichtige Herausforderungen für politische Entscheidungsträger umfassen die Frage, ob und in welcher Form sie Forschung, Entwicklung, Evaluierung und Einführung technischer Schutzmaßnahmen sowie Überwachungsmethoden unterstützen sollten. Dies ist schwierig, weil das Verständnis von Wissenschaftlern darüber, wie sich Mechanismen am besten in der Praxis absichern lassen, sich noch weiterentwickelt und bewährte Verfahren noch nicht etabliert sind. Beispielsweise wenden verschiedene Entwickler unterschiedliche Schutzmaßnahmen an, und ihre Ansätze zur technischen Risikominderung insgesamt unterscheiden sich entsprechend stark (‡1116). Schließlich bedeutet das Vorhandensein wirksamer technischer Schutzmaßnahmen allein noch keine Sicherheit, da Übernahme und Umsetzung je nach Entwickler und Bereitstellungskontext unterschiedlich ausfallen können.

