##########
>white|orangered|left|14|30|hr Sectie 3.3
### 3.3. Technische waarborgen en monitoring
>white|orangered|left|24|30|hb Technische waarborgen en monitoring

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Belangrijke informatie
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ In een breed scala aan technische waarborgen wordt voorzien in verschillende fasen van de ontwikkeling en het gebruik van AI. Deze omvatten technieken die tijdens de modelontwikkeling worden toegepast om systemen robuuster te maken en beter bestand tegen misbruik (zoals data-curatie), monitoring en controle tijdens de inzet (zoals contentfiltering en menselijke toezicht), en hulpprogramma's na de inzet om het bredere AI-ecosysteem te monitoren (zoals herkomst en detectie van content).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Technische beveiligingsmaatregelen hebben beperkingen en voorkomen niet betrouwbaar schadelijk gedrag in alle contexten. Zo kunnen gebruikers soms schadelijke outputs verkrijgen door verzoeken te herformuleren of ze op te delen in kleinere stappen. Op vergelijkbare wijze kunnen hulpmiddelen zoals watermerken, die zijn ontworpen om door AI gegenereerde inhoud te identificeren, vaak worden verwijderd of aangepast, wat de betrouwbaarheid beperkt.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ De beperkingen van afzonderlijke beschermingsmaatregelen betekenen dat ‘verdediging-in-diepte’ nodig kan zijn om bepaalde schadelijke uitkomsten te voorkomen. Een systeem kan bijvoorbeeld een op veiligheid getraind model combineren met inputfilters, outputfilters en inhoudsmonitoren.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sinds de publicatie van het vorige rapport (januari 2025) hebben onderzoekers vooruitgang geboekt bij het verbeteren van waarborgen, maar er blijven fundamentele beperkingen bestaan. Zo is het slagingspercentage van aanvallen die zijn ontworpen om waarborgen te omzeilen gedaald, maar blijft het relatief hoog. Er zijn ook fundamentele beperkingen aan hoe grondig open-weight modellen kunnen worden voorzien van waarborgen.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Een belangrijke uitdaging voor beleidsmakers is het beperkte bewijs over hoe effectief waarborgen zijn in uiteenlopende praktische toepassingen van generieke AI-systemen. AI-ontwikkelaars lopen sterk uiteen in hoeveel informatie zij delen over hun waarborgen en monitoring. Een verdere uitdaging is het mogelijke afruilprobleem tussen het toepassen van strengere waarborgen en het handhaven van de systeemprestatie of bruikbaarheid.
>oldlace|black||11|15|br      


AI-ontwikkelaars kunnen verschillende nuttige maar onvolmaakte technische waarborgen gebruiken om risico’s van general-purpose AI-systemen te beperken en te beheersen, maar robuustheidsproblemen blijven bestaan. Ontwikkelaars kunnen nog steeds niet volledig voorkomen dat general-purpose AI-systemen zelfs bekende en duidelijk schadelijke handelingen uitvoeren, zoals het geven van gebruikersinstructies om misdaden te plegen. Onderzoekers hebben bijvoorbeeld aangetoond dat geavanceerde waarborgen kunnen worden omzeild via methoden voor adversarial prompting (d.w.z. ‘jailbreaks’) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), door modellen complexe schadelijke taken te laten opsplitsen in stappen (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), en met eenvoudige modelaanpassingen (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Onderzoekers werken nog steeds aan waarborgen tegen storingen en misbruik (‡690). Deze methoden lopen sterk uiteen in doel en effectiviteit, en hun impact hangt uiteindelijk af van de bredere sociaal-technische en governance-context waarin AI-systemen worden gebouwd en ingezet.

Technische waarborgen kunnen grofweg worden onderverdeeld in drie categorieën: technieken voor het ontwikkelen van veiligere modellen; technieken die tijdens de inzet worden gebruikt voor bewaking en controle; en technieken die ondersteuning bieden voor monitoring van het ecosysteem na de inzet. Tafel 3.6 vat de technische waarborgen samen die worden besproken, hun effectiviteit en open uitdagingen.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Het ontwikkelen van veiligere modellen
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Data-curatie (‡1167)
  Schadelijke gegevens verwijderen om te voorkomen dat een model gevaarlijke capaciteiten leert. Deze methoden kunnen nuttig zijn, ook voor het ontwikkelen van open-weight modellen die geen schadelijke capaciteiten hebben en bestand zijn tegen schadelijke fine-tuning (‡55). Er zijn echter uitdagingen met curatie-fouten en schaling (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Reinforcement learning uit menselijke feedback (‡64*)
  De modeltraining om het af te stemmen op gespecificeerde doelen, zoals behulpzaam en onschadelijk zijn. Dit is een effectieve manier om modellen te laten leren van nuttig gedrag (‡64*). Echter, overoptimalisatie voor menselijke goedkeuring kan ervoor zorgen dat modellen zich misleidend of meelijwekkend gedragen (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pluralistische uitlijningstechnieken (‡1170)
  Het model trainen om meerdere uiteenlopende zienswijzen te integreren over hoe het zich zou moeten gedragen. Deze technieken helpen de mate te verminderen waarin modellen specifieke zienswijzen bevoordelen (‡1170). Echter, ondanks deze technieken is meningsverschil tussen mensen onvermijdelijk, en het is moeilijk om breed geaccepteerde manieren te ontwerpen om concurrerende zienswijzen in balans te brengen (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adversariële training (‡677)
  Het trainen van het model om te weigeren schade te veroorzaken (ook in onbekende contexten) en om aanvallen te weerstaan van kwaadwillende gebruikers (bijv. 'jailbreaks'). Dit is een effectieve methode om modellen pogingen tot misbruik te laten weerstaan (‡1064), maar robuustheidsuitdagingen blijven bestaan (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Machine ‘unlearning’ (‡1175, ‡1176)
  Een model trainen met behulp van gespecialiseerde algoritmen om schadelijke capaciteiten actief te onderdrukken (bijv. kennis van bio-gevaar). Deze technieken bieden een gerichte manier om schadelijke capaciteiten uit modellen te verwijderen (‡1175, ‡1176), maar huidige unlearning-algoritmen kunnen niet robuust zijn en onbedoelde effecten hebben op andere capaciteiten (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Interpretatie- en veiligheidsverificatietools (‡1177)
  Een diverse familie van ontwerpmethoden en verificatiemethoden, bedoeld om meer robuuste zekerheid te bieden dat modellen specifieke veiligheidsgerelateerde eigenschappen hebben. Ze stellen beoordelaars in staat om met meer vertrouwen zekerheid over veiligheid te geven (‡1177), maar huidige methoden zijn gebaseerd op aannames en zijn in de praktijk zelden competitief wat betreft prestaties (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Bewaking en controle
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Op hardware gebaseerde monitoringmechanismen (‡1179, ‡1180, ‡1181)
  Verifiëren dat geautoriseerde processen draaien op hardware om beveiligingsbedreigingen of naleving van regelgeving te bestuderen. Deze mechanismen bieden unieke manieren om te volgen welke berekeningen op hardware worden uitgevoerd en door wie (‡1181). Echter, hardwaremechanismen kunnen niet voor alle soorten bedreigingen monitoren, en sommige technieken vereisen gespecialiseerde hardware (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Gebruikersinteractie bewakingen (‡1154, ‡1166)
  Het monitoren van gebruikersinteracties op aanwijzingen van kwaadaardig gebruik kan ontwikkelaars helpen om de dienstverlening te beëindigen voor kwaadwillende gebruikers (‡1154, ‡1166). Handhaving kan echter onbedoeld nuttig onderzoek naar veiligheid belemmeren (‡689), en sommige vormen van misbruik zijn moeilijk te detecteren (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Gebruikersinteractie monitort (‡1154, ‡1166)
  Monitoring van gebruikersinteracties op tekenen van kwaadaardig gebruik kan ontwikkelaars helpen om de dienstverlening voor kwaadaardige gebruikers te beëindigen (‡1154, ‡1166). Handhaving kan echter onbedoeld nuttig onderzoek naar veiligheid belemmeren (‡689), en sommige vormen van misbruik zijn moeilijk te detecteren (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Inhoudfilters (‡65*, ‡725)
  Het filteren van mogelijk schadelijke modelinvoer en -uitvoer is een zeer effectieve manier om onbedoelde schade en misbruikrisico's te verminderen (‡725). Filters vereisen echter extra rekenkracht en zijn kwetsbaar voor sommige aanvallen (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Model interne berekeningen bewaking (‡744, ‡1183, ‡1184)
  Monitoring op signalen van misleiding of andere schadelijke interne vormen van cognitie in modellen kan een efficiënte manier zijn om misleiding te detecteren (‡744, ‡1183, ‡1184). Huidige methoden missen echter robuustheid en betrouwbaarheid (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chain-of-thought monitors (‡430, ‡435)
  Het bewaken van ketting-van-redeneringstekst (chain-of-thought) van modellen op tekenen van misleidend gedrag of andere schadelijke redeneringen is een effectieve manier om te begrijpen en om tekortkomingen te herkennen in hoe modellen redeneren (‡435). Ze kunnen echter onbetrouwbaar zijn (‡752, ‡753, ‡1186), en als modellen worden getraind om een onschuldige ketting-van-redenering (chain of thought) te produceren, kunnen ze misleidend gedrag leren (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Human in the loop (‡1187, ‡1188, ‡1189)
  Menselijke controle en overrides voor systeembeslissingen zijn essentieel in sommige veiligheidskritieke toepassingen (‡1187). Deze technieken worden echter beperkt door automatiseringsbias en door grenzen aan de snelheid van menselijke besluitvorming (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sandboxing (‡1192)
  Het voorkomen dat een AI-agent de wereld rechtstreeks beïnvloedt, is een effectieve manier om de schade die het kan veroorzaken te beperken (‡1192). Sandboxing beperkt echter het vermogen van het systeem om bepaalde taken direct uit te voeren (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Tools om ecosysteemmonitoring te faciliteren
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb AI-modelidentificatietechnieken (‡1193*, ‡1194)
  Het maken van modellen, of individuele instanties van modellen, zodat ze gemakkelijker te identificeren zijn in reële gebruikssituaties, helpt met digitale forensische analyse en het vergroten van bewustzijn over het ecosysteem (‡1195). Deze technieken kunnen echter worden omzeild met bepaalde soorten modelaanpassingen (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb AI-modelerfenisinferentie (‡1197)
  Deze technieken stellen onderzoekers in staat om te bestuderen hoe modellen worden aangepast in het AI-ecosysteem, met name open-weight modellen. Ze helpen bij digitale forensische analyse en bewustwording van het ecosysteem (‡1198), maar grootschalige projecten zouden nodig zijn om het ecosysteem van open-weight modellen (‡1198) grondig in kaart te brengen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Watermerken en metadata (‡1199, ‡1200, ‡1201*)
  Deze technieken maken het gemakkelijker om te detecteren wanneer een stuk tekst, afbeelding, video, enz. door AI is gegenereerd of is aangepast, en door welk systeem. Ze vergemakkelijken een beter inzicht in het ecosysteem (‡1199, ‡1200, ‡1201*). Watermerken en metadata kunnen echter worden vervalst of verwijderd door bepaalde aanpassingen aan de inhoud (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Detectie van door AI gegenereerde content (‡1203, ‡1204, ‡1205*)
  Het verbeteren van het vermogen van gebruikers om AI-gegenereerde content te onderscheiden van echte content helpt bij digitale forensics en het vergroten van het bewustzijn binnen het ecosysteem (‡1203, ‡1204). Classificators kunnen echter onbetrouwbaar zijn (‡1205*) en vertonen wisselende prestaties over modaliteiten heen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 3.6: Technische waarborgen besproken in deze sectie
>white|black||9|11|br Een samenvatting van de technische waarborgen die in deze sectie zijn besproken, onderverdeeld in methoden voor het ontwikkelen van veiligere modellen, monitoring en controle tijdens de inzet, en technieken om monitoring van het ecosysteem te faciliteren.


###@ Het ontwikkelen van veiligere modellen

Een eerste verdedigingslinie tegen schadelijke effecten van algemene AI-systemen is om het onderliggende model veiliger te maken. Deze subsectie behandelt waarborgen die “ingebakken zijn in de modelparameters” tijdens het modelontwikkelingsproces (Figuur 3.6).

>white|orangered|left|14|15.5|bb Het samenstellen van trainingsdata kan de ontwikkeling beperken van potentieel gevaarlijke mogelijkheden

Algemene-doel AI-modellen zijn juist nuttig omdat ze na verwerking van trainingsdata een breed scala aan kennis en mogelijkheden ontwikkelen, maar sommige typen trainingsdata zijn onevenredig verantwoordelijk voor de ontwikkeling van mogelijk gevaarlijke capaciteiten. Een AI-model dat bijvoorbeeld is getraind op virologie-publicaties, kan mogelijk beter in staat zijn om assistentie te bieden bij potentieel schadelijke biologische taken (‡549, ‡1206*) (zie ook §2.1.4. Biologische en chemische risico’s). Daarnaast kunnen beeld-/video-generators die zijn getraind op afbeeldingen van menselijke naaktheid ook worden misbruikt om niet-consensuele intieme deepfakes te maken (‡308, ‡319) (zie ook §2.1.1. Door AI gegenereerde content en criminele activiteiten).

Het filteren van trainingsdata is een effectieve mitigatie tegen sommige ongewenste capaciteiten (‡319, ‡1167, ‡1207, ‡1208). Het kan echter moeilijk zijn om de grote datasets te filteren die worden gebruikt om general-purpose AI-modellen te trainen (‡1168), vanwege hoge kosten (‡1209), filterfouten (‡1210) en negatieve effecten op de kwaliteit van de dataset (‡1211). Deze uitdagingen worden verergerd door de meertalige aard van internettekst (‡1212), culturele vooroordelen in contentmoderatie (‡1211, ‡1213, ‡1214, ‡1215) en het feit dat of een bepaald stuk data ‘schadelijk’ is afhangt van contextuele factoren (‡1216). Niettemin laat het filteren van mogelijk schadelijk materiaal uit trainingsdata potentie zien om modellen betrouwbaarder veilig te maken, waaronder het robuuster maken van open-weight-modellen tegen schadelijke manipulatie (‡55). De relaties tussen de inhoud van trainingsdata en emergent modelcapaciteiten zijn nog niet volledig begrepen (‡1195), en filtratie lijkt effectiever om schadelijke capaciteiten te beperken wanneer het wordt toegepast op brede domeinen van kennis (‡55) in vergelijking met smallere gedragingen (‡1206, ‡1217). Zie §3.4. Open-weight-modellen voor verdere bespreking.

![figure 3.6](images/fig3.6_safeguards.png)

##### Figuur 3.6: Waar technische waarborgen moeten worden toegepast
>white|black||9|11|br Technische waarborgen kunnen op verschillende momenten tijdens de ontwikkeling van een model worden toegepast. Datacuratie bepaalt wat modellen leren tijdens pre-training en fine-tuning. Trainingsgebaseerde methoden zoals reinforcement learning van menselijke feedback en robuustheidstraining passen het gedrag van het model aan. Testmethoden zoals adversarial attacks identificeren resterende kwetsbaarheden. Sommige technieken, zoals safe-by-design algoritmen, bestrijken meerdere fasen. Bron: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Methoden om algemene AI-modellen te trainen zodat ze voornamelijk behulpzaam en onschadelijk zijn, zijn voornamelijk gebaseerd op menselijke feedback

Het is moeilijk om modellen te trainen en te evalueren die betrouwbaar aansluiten op hoger-niveau principes zoals behulpzaam, onschadelijk en eerlijk zijn. In de praktijk proberen ontwikkelaars dit te bereiken door AI-modellen te finetunen met demonstraties en feedback van mensen. Zo is het belangrijkste paradigm voor het finetunen van AI-modellen, bekend als ‘reinforcement learning from human feedback’, gebaseerd op het trainen van modellen om outputs te genereren die menselijke annotatoren positief beoordelen (‡1218). Positieve feedback van mensen is echter een gebrekkige maatstaf voor nuttig gedrag (‡737, ‡878, ‡1219, ‡1220) en wordt beperkt door menselijke fouten en vertekening (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Dit leidt tot verschillende uitdagingen: modellen die met reinforcement learning van menselijke feedback zijn bijgetraind, kunnen soms de gebruiker naar de mond praten, een gedrag dat bekend staat als ‘sympathie’ (‡358, ‡740, ‡1226, ‡1227); antwoorden geven die in sommige contexten behulpzaam zijn maar in andere contexten schadelijk (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); antwoorden geven die lastig te beoordelen zijn op correctheid (‡1233); of acties uitvoeren waarvan de behulpzaamheid of schadelijkheid een kwestie van mening is (‡1234). Tafel 3.7 geeft voorbeelden van deze uitdagingen. Sommige onderzoeken richten zich op het ontwikkelen van methoden om mensen te helpen oplossingen voor complexe taken met AI-assistentie beter te evalueren (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Deze methoden hebben echter momenteel beperkte betrouwbaarheid, en in hoeverre ze worden gebruikt om de vandaag meest geavanceerde AI-modellen te trainen is niet publiek bekend.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sycophancy/vleierij (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Uitleg:
>white|black|left|11|13|br Het model geeft alleen positieve feedback en slaagt er niet in te wijzen op het ontbreken van de correcte lettergreepstructuur van een 5-7-5 haiku.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sommige acties zijn nuttig in sommige contexten maar schadelijk in andere (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Uitleg:
>white|black|left|11|13|br Informatie over biologisch risico kan worden gebruikt voor educatie en verdediging, maar ook om kwaadwillende actoren te informeren.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Correct gedrag is moeilijk te verifiëren (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Uitleg:
>white|black||11|13|br De juistheid van dit antwoord is moeilijk te beoordelen, omdat hiervoor medische expertise nodig is. Zelfs voor een ervaren arts vereist het evalueren van antwoorden zoals dit tijd en zorgvuldige aandacht voor details.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Mensen verschillen van mening over wat correct is (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Uitleg:
>white|black|left|11|13|br Mensen zijn het aanzienlijk oneens over wat het juiste antwoord is.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 3.7: Gebruikersprompt en antwoord van het AI-model
>white|black||9|11|br Voorbeelden van uitdagingen bij het specificeren en het stimuleren van gunstige acties vanuit AI-modellen.


>white|orangered|left|14|15.5|bb Mensen zijn het niet altijd eens over welke gedragingen wenselijk zijn, waardoor methoden nodig zijn om concurrerende voorkeuren in evenwicht te brengen

Mensen zijn het niet altijd eens over welke reacties of acties AI-modellen wel of niet zouden moeten opleveren (‡1006). Dit maakt het fundamenteel uitdagend om modellen te ontwikkelen waarvan de acties en effecten breed in lijn zijn met de belangen van de samenleving (‡420). Sommige onderzoekers bestuderen wiens voorkeuren worden weerspiegeld in AI-systemen (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) en werken aan het ontwikkelen van technieken voor ‘pluralistische alignment’ die erop gericht zijn een balans te vinden tussen concurrerende voorkeuren (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Zo kunnen AI-ontwikkelaars systemen zo ontwerpen dat ze vermijden om controversiële antwoorden te genereren door te weigeren om te reageren op bepaalde verzoeken, of af te stemmen op het standpunt van de mediaan in een relevante steekproef van mensen, of systemen te personaliseren voor individuele gebruikers.

Een gemeenschappelijke uitdaging voor deze benaderingen is dat AI-systemen in het algemeen niet in gelijke mate kunnen aansluiten op de voorkeuren van iedereen, en dat hun doorwerking in de samenleving verschillende groepen mensen verschillend zal beïnvloeden. Sommige onderzoekers hebben betoogd dat de meeste technische benaderingen voor pluralistische alignment tekortschieten in het aanpakken van diepere uitdagingen, en deze mogelijk zelfs afleiden van die uitdagingen, zoals systematische vooringenomenheid, sociale machtsdynamiek en de concentratie van rijkdom en invloed (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb AI-ontwikkelaars gebruiken ‘adversarial training’ om de robuustheid van het model te verbeteren

Het is uitdagend om ervoor te zorgen dat AI-modellen de gunstige gedragingen die ze tijdens de training leren robuust kunnen vertalen naar real-world inzetcontexten. Zelfs modellen die worden getraind met een ‘perfect’ leersignaal kunnen mislukken om met succes te generaliseren naar alle ongeziene contexten (‡738, ‡739, ‡1255, ‡1256, ‡1257). Sommige onderzoekers hebben bijvoorbeeld vastgesteld dat chatbots vaker schadelijke acties uitvoeren in talen die ondervertegenwoordigd zijn in hun trainingsdata (‡159, ‡880, ‡1258*, ‡1259), waaronder veel talen die voornamelijk worden gesproken in het Global South.

In de afgelopen jaren hebben onderzoekers ook een grote toolkit met ‘adversarial attack’-technieken ontwikkeld die kunnen worden gebruikt om modellen mogelijk schadelijke antwoorden te laten genereren (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Zo heeft een recent initiatief meer dan 60,000 diverse voorbeelden van succesvolle aanvallen tegen state-of-the-art AI-modellen crowd-sourced, waardoor ze de beleidsregels van hun bedrijven over acceptabel modelgedrag schonden (‡1149). Tafel 3.8 toont voorbeelden van ‘jailbreak’-technieken die onderzoekers hebben laten zien dat modellen kunnen laten voldoen aan schadelijke verzoeken.

Een methode om de robuustheid van modellen te verbeteren staat bekend als ‘adversarial training’ (‡1064). Hierbij worden ‘aanvallen’ (bijv. jailbreaks) geconstrueerd die bedoeld zijn om een model op ongewenste wijze te laten handelen, en wordt het model getraind om deze aanvallen op passende wijze te verwerken. Adversarial training is echter onvolkomen (‡1260, ‡1261). Aanvallers kunnen consequent nieuwe succesvolle aanvallen ontwikkelen tegen state-of-the-art-modellen (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Omdat ontwikkelaars specifieke voorbeelden van falende modus(sen) nodig hebben om ertegen te trainen (‡512, ‡1263), resulteert dit in een voortdurende ‘kat-en-muis’-game waarin ontwikkelaars modellen voortdurend bijwerken als reactie op nieuw ontdekte kwetsbaarheden, en tegenstanders voortdurend op zoek gaan naar nieuwe aanvallen. Sommige onderzoekers hebben voorgesteld om adversarial training op grotere schaal toe te passen (‡1264, ‡1265) of nieuwe algoritmen (‡675, ‡676, ‡1263, ‡1266, ‡1267) te gebruiken om de robuustheid te verbeteren, maar moderne AI-systemen blijven hardnekkig kwetsbaar.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie: Doe schadelijke verzoeken in cijfertekst, zoals morsecode (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie: vul het systeem met voorbeelden van conform reagerende antwoorden op schadelijke verzoeken (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie: Doe schadelijke verzoeken in talen met weinig beschikbare bronnen die waarschijnlijk minder worden gebruikt bij training (bijv. Swahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie: Breek een schadelijke taak op in meerdere onschuldige deelopdrachten (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 3.8: Jailbreak-strategieën
>white|black||9|11|br Kwaadaardige actoren en red teams hebben verschillende soorten ‘jailbreaks’ gebruikt om AI-modellen te laten voldoen aan schadelijke verzoeken die ze normaal gesproken zouden weigeren vanwege waarborgen. Voorbeelduitvoer is geschreven door de auteurs van het rapport voor illustratieve doeleinden. Veel huidige state-of-the-art AI-modellen zijn nu in staat om de meeste van deze methoden te weerstaan, maar er blijven nieuwe jailbreaktechnieken worden ontdekt.


>white|orangered|left|14|15.5|bb ‘Unlearning’-technieken kunnen specifieke schadelijke modelmogelijkheden beperken

Een andere strategie om risico’s van algemene-purpose AI te beperken, is om modellen te fine-tunen zodat ze geen capaciteiten hebben in specifieke domeinen met een hoog risico (‡1175, ‡1176). Onderzoekers werken bijvoorbeeld aan het ontwikkelen van ‘machine unlearning’-algoritmen die specifiek vaardigheden kunnen onderdrukken die verband houden met biobedreigingen of met het genereren van fotorealistische beelden van naakte menselijke lichamen (‡903, ‡1272, ‡1273). Deze methoden kunnen modellen aanzienlijk veiliger maken, ten koste van het beperken van sommige positieve toepassingen van de ongeleerde capaciteiten. Het beperken van de kennis van AI-modellen in schadelijke domeinen is ook voorgesteld als een manier om ‘tamper-resistant’ open-weight modellen te ontwerpen die bestand zijn tegen schadelijke fine-tuning (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Tot nu toe is dit echter lastig gebleken om robuust te doen (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Zie §3.4. Open-weight modellen voor verdere discussie.

>white|orangered|left|14|15.5|bb Sommige onderzoekers werken aan methoden voor sterkere veiligheidswaarborgen door de interne toestanden van het model te interpreteren of door wiskundige verificatie

Sommige onderzoekers werken aan methoden om veiligheidsgerelateerde eigenschappen van modellen rigoureuzer te verifiëren. In één aanpak proberen onderzoekers de interne berekeningen van modellen te interpreteren om hetzij risico’s te identificeren hetzij overtuigender argumenten te formuleren dat het model veilig is (‡1285, ‡1286). In een proof of concept toonden onderzoekers bijvoorbeeld aan dat hulpmiddelen voor het analyseren van de interne berekeningen van een taalmodel evaluatoren konden helpen schadelijk gedrag te identificeren (‡1287). In 2025 is Anthropic ook begonnen met het analyseren van modelinternals als manier om model-situationele bewustwording en ‘intentie’ te bestuderen (‡2). Dergelijke methoden zijn momenteel echter niet gangbaar of niet bekend als concurrerend met andere evaluatietechnieken.

Een andere aanpak om sterkere garanties voor veiligheid te verkrijgen, is het construeren van wiskundige bewijzen dat een model aan bepaalde veiligheidsvoorwaarden zal voldoen (‡1177, ‡1282, ‡1288). Deze bewijzen gaan echter ervan uit dat de testsituatie overeenkomt met de inzetomgeving, en zijn niet getest tegen veel verschillende typen tegenstanders.

Ze kunnen momenteel ook niet worden opgeschaald naar grote modellen. Over het algemeen is er onder experts aanzienlijke discussie over de belofte van interpreteerbaarheid en methoden voor formele verificatie.

###@ Monitoring en controle tijdens de deployment

Naast waarborgen die tijdens de modelontwikkeling zijn geïmplementeerd, vormt een tweede verdedigingslinie tegen schadelijk gedrag een reeks externe waarborgen die zich richt op het monitoren en controleren van de acties van een model of systeem tijdens de uitrol. Dergelijke waarborgen helpen problemen en misbruik te beperken, zoals hallucinaties in uitvoer en schadelijke instructies.

>white|orangered|left|14|15.5|bb Modeldeployers kunnen een verscheidenheid aan hulpmiddelen gebruiken om risicovolle modelgedragingen te identificeren en aan te pakken

Wanneer een AI-systeem draait, kan een deployer toezicht houden op signalen van risico en ingrijpen als die zich voordoen. Bijvoorbeeld kunnen zij de invoer van een model inspecteren op tekenen van adversariële aanvallen, ongepaste inhoud uit uitvoer filteren, of de chain of thought van het systeem bewaken op tekenen van schadelijke plannen. Punts waar deployers kunnen bewaken en ingrijpen in hoe mensen hun systemen gebruiken omvatten hardware (‡1180, ‡1181), gebruikersinteracties (‡1154, ‡1166), invoer en uitvoer (‡65, ‡725, ‡1182), interne berekeningen (‡744, ‡1183, ‡1184) en chain of thought (‡430, ‡435). Er zijn ook meerdere acties die deployers kunnen ondernemen wanneer risico’s worden vastgesteld. Deze omvatten het loggen van informatie, het filteren/wijzigen van schadelijke inhoud, het markeren van afwijkende activiteit, het uitschakelen van systemen of het activeren van failsafes. Figuur 3.7 illustreert voorbeelden van veelvoorkomende monitoring- en controlemechanismen.

Omdat ze veelzijdig zijn en vaak effectief, worden deze mechanismen veel gebruikt en kunnen ze veel soorten onbedoelde schade voorkomen (‡725, ‡751, ‡1289). Deze waarborgen zijn echter onvolmaakt, vooral onder kwaadaardige aanvallen die erop geoptimaliseerd zijn om ze te laten falen (‡752, ‡1182). Recente onderzoeken hebben ook onderzocht hoe monitoring onbetrouwbaar kan zijn als een systeem wordt geoptimaliseerd met behulp van de scores van een monitor, bijvoorbeeld door redeneringen stap voor stap minder betrouwbaar te maken (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Figuur 3.7: Monitoring- en controletechnieken
>white|black||9|11|br Monitoring- en controletechnieken werken op meerdere punten: het screenen van inputs en outputs op schadelijke inhoud, het volgen van interne modelstatussen, het beperken van externe acties via sandboxing en het waarborgen van menselijke toezicht. Bron: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Mensen in de lus bieden directe supervisie in omgevingen met een hoog risicoprofiel

Om de kans op mislukkingen door AI-agenten te verkleinen (zie §2.2.1. Betrouwbaarheidsuitdagingen), kunnen uitvoerders erop richten AI-systemen te ontwerpen die samenwerken met mensen in plaats van volledig autonoom te werken (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Dit is belangrijk voor use cases waarbij onjuiste beslissingen tot aanzienlijk letsel kunnen leiden, zoals in de financiële sector, de gezondheidszorg of bij politiewerk. Toch is het vaak onpraktisch om een ‘human in the loop’ te hebben. Soms gebeurt besluitvorming te snel, zoals bij chatapplicaties met miljoenen gebruikers. In andere gevallen kunnen menselijke vooringenomenheid en fouten de risico’s vergroten door zich opstapelende fouten (‡1187). Mensen in de loop vertonen bovendien vaak ‘automation bias’, wat betekent dat zij vaak meer vertrouwen in het AI-systeem plaatsen dan gerechtvaardigd is (‡1190, ‡1191) (zie §2.3.2. Risico’s voor menselijke autonomie).

>white|orangered|left|14|15.5|bb ‘Sandboxing’ beschermt tegen risico’s van autonome gedragingen

AI-agenten die autonoom kunnen handelen zonder beperkingen op het web of in de fysieke wereld vormen verhoogde risico’s (zie §2.2.1. Betrouwbaarheidsuitdagingen). ‘Sandboxing’ houdt in dat de manieren worden beperkt waarop AI-agenten de wereld rechtstreeks kunnen beïnvloeden, waardoor het veel eenvoudiger wordt om ze te overzien en te beheren (‡640, ‡1192, ‡1295). Zo kan het beperken van het vermogen van een AI-systeem om op het internet te posten of het bestandsysteem van een computer te wijzigen onverwachte schade door onverwachte handelingen voorkomen (‡1296). Deze aanpakken kunnen echter niet altijd worden gebruikt voor toepassingen waarbij een AI-systeem noodzakelijkerwijs direct in de wereld moet handelen.

###@ Tools voor ecosysteemmonitoring: modellering en herkomst van gegevens

Model- en dataprovenancehulpmiddelen zijn technische hulpmiddelen voor het bestuderen van het AI-ecosysteem, om het bewustzijn te verbeteren van de downstream-toepassingen en effecten van AI-systemen.

>white|orangered|left|14|15.5|bb AI-systeemherkomsttechnieken helpen om het gebruik en de effecten van systemen te herleiden

Ontwikkelaars en deployers kunnen verschillende technieken gebruiken om modelgebruik te bestuderen en de verspreiding ‘in het wild’ te onderzoeken. Zo kunnen ze modellen unieke identificerende gedragingen geven (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) of unieke patronen toepassen op de gewichten van afzonderlijke open-weight-modellen (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Het is echter een open probleem om deze technieken beter bestand te maken tegen modelwijzigingen (‡1195, ‡1196*). Onderzoekers werken ook aan methoden voor het ‘afleiden van modelherkomst’ (‡1197, ‡1198, ‡1305, ‡1306), waarmee vragen kunnen worden beantwoord zoals: ‘Was model X een gefinetunede of gedistilleerde versie van model Y?’ Tot slot werken sommige ontwikkelaars aan protocollen en infrastructuur voor AI-agenten om identificatie en verificatie te faciliteren wanneer zij interageren met externe systemen (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Figuur 3.8: Watermarks verwerken onmerkbare verstoringen in afbeeldingen en audio
>white|black||9|11|br Watermerken voegen onwaarneembare verstoringen in afbeeldingen en audio in, waardoor door AI gegenereerde content kan worden geïdentificeerd met behulp van detectietools. In deze figuur zijn zowel de beeld- als de audiowatermerken overdreven om ze zichtbaar te maken. Bron: Chameleon-afbeelding van Unsplash (‡1313*). Andere elementen gemaakt door de auteurs van het rapport. International AI Safety Report 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Figuur 3.9: Succespercentages van prompt-injectionaanvallen
>white|black||9|11|br Succespercentages van geslaagde prompt-injectie-aanvallen, zoals gerapporteerd door AI-ontwikkelaars voor grote modellen die zijn uitgebracht tussen mei 2024 en augustus 2025. Elk punt vertegenwoordigt het aandeel van succesvolle aanvallen binnen 10 pogingen tegen een gegeven model kort na de release. Het gerapporteerde succespercentage van dergelijke aanvallen daalt in de tijd, maar blijft relatief hoog. Bron: Zou et al. 2025 (‡1149), geciteerd in Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb AI-contentdetectietechnieken helpen de verspreiding en impact van AI-gegenereerde content te monitoren

Watermerken, metadata en andere AI-inhoudsdetectietools kunnen onderzoekers helpen om de werkelijke impact van door AI gegenereerde inhoud op de werkelijkheid te volgen en te bestuderen. 

Ten eerste zijn datwatermerken subtiele maar herkenbare motieven die in digitale media worden ingevoegd en die informatie kunnen coderen over hun oorsprong (‡1199, ‡1200, ‡1201*). Voor tekst nemen ze doorgaans de vorm aan van subtiele vertekeningen in woordkeuzes en stijl (‡1308, ‡1309); voor afbeeldingen en video zijn het subtiele patronen over pixels (‡1310); en voor audio zijn het subtiele patronen in audiogolven (‡1311). Figuur 3.8 illustreert dit.

Afgezien van watermerken kan door AI gegenereerde content ook worden opgeslagen met bestandsformaten die metadata opslaan over hoe ze zijn gegenereerd. Veel mobiele apparaten slaan bijvoorbeeld afbeeldings- en audiobestanden op met een bestandsformaat dat informatie kan bewaren over cameraparameters, tijd, locatie, enz. (‡1312). Vergelijkbare metadata kunnen worden gebruikt om informatie op te slaan over de vraag of data is gegenereerd door een AI-systeem. Net zoals vingerafdrukken in forensisch onderzoek door criminelen kunnen worden vervalst of verwijderd, kunnen watermerken en metadata worden aangepast of verwijderd, maar ze zijn niettemin nuttig.

Onderzoekers werken ook aan het ontwikkelen van detectoren voor door AI gegenereerde inhoud (‡1203, ‡1204, ‡1205*) om te helpen bij het identificeren van door AI gegenereerde inhoud in het wild, zelfs wanneer er geen watermark of metadata beschikbaar is. Deze identificatietechnieken hebben echter een beperkt slagingspercentage.

###@ Updates

Sinds de publicatie van het vorige rapport (januari 2025) is vooruitgang geboekt bij het ontwikkelen van AI-systemen met meerdere doeltreffende lagen van waarborgen. Zoals besproken in §3.2. Risicobeheersingspraktijken, is defence-in-depth een kernprincipe in risicobeheer (‡1314). AI-systemen die bijvoorbeeld safety-trained modellen combineren met inputfilters, outputfilters en andere contentmonitoren worden steeds vaker bestudeerd en ingezet (‡32, ‡65, ‡1182*). Recente onderzoeken hebben ook aangetoond dat, hoewel ontwikkelaars van modellen vooruitgang hebben geboekt in het vergroten van de robuustheid tegen pogingen om waarborgen te omzeilen, aanvallers nog steeds met een hoog tempo slagen (Figuur 3.9).

###@ Bewijsleemtes

Er is meer bewijs nodig om onderzoekers te helpen de beperkingen van bestaande benaderingen te begrijpen en er rekening mee te houden. Technische beveiligingen voor AI-systemen worden verbeterd, maar technieken hebben beperkingen. Zo is de vooruitgang bij het verbeteren van de robuustheid in het slechtste geval van algemene AI-systemen traag geweest, en zijn er fundamentele beperkingen aan hoe grondig open-weight-modellen kunnen worden beveiligd en gemonitord (‡1195, ‡1315, ‡1316) (zie ook §3.4. Open-weight-modellen). Ondertussen zijn niet alle technische beveiligingen even gebruikelijk, even effectief of even goed bewezen in de echte wereld. Zo wordt adversarial training vrijwel alom gebruikt op state-of-the-art-modellen (‡64*, ‡677), terwijl modelinterpretatie- en formele-verificatie-technieken tot op heden weinig zijn toegepast in productieomgevingen (‡1177, ‡1285).

###@ Uitdagingen voor beleidsmakers

Belangrijke uitdagingen voor beleidsmakers zijn onder meer beslissen of, en zo ja hoe, zij onderzoek, ontwikkeling, evaluatie en adoptie van technische waarborgen en bewakingsmethoden moeten ondersteunen. Dit is uitdagend omdat het inzicht van wetenschappers in de beste manier om mechanismen in de praktijk te beveiligen nog in ontwikkeling is en best practices nog niet zijn vastgesteld. Zo passen verschillende ontwikkelaars verschillende waarborgen toe en lopen hun benaderingen voor technische risicobeperking in bredere zin sterk uiteen (‡1116). Tot slot geldt dat het bestaan van effectieve technische waarborgen op zichzelf de veiligheid niet garandeert, omdat adoptie en implementatie kunnen verschillen tussen ontwikkelaars en inzetcontexten.

