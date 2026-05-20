Algemene AI-systemen voor algemeen gebruik falen op manieren die al reële schade in de praktijk hebben veroorzaakt, van verzonnen juridische verwijzingen tot medische verkeerde diagnoses. Hoewel ook menselijke professionals fouten maken, roepen AI-falen specifieke zorgen op vanwege hun nieuwheid, potentiële schaal, de moeilijkheid om te voorspellen wanneer ze optreden, en de neiging van gebruikers om onkritisch te vertrouwen op outputs die zelfverzekerd klinken. Huidige AI-falen voor algemeen gebruik omvatten het verstrekken van onjuiste informatie (‡602, ‡603), het maken van basale redeneerfouten (‡604, ‡605) en het verslechteren wanneer ze worden ingezet in nieuwe contexten (‡606, ‡607, ‡608). Gedocumenteerde schade door dergelijke falen omvat medische verkeerde diagnoses, fouten in juridische pleidooien en financiële verliezen (‡609, ‡610, ‡611). Betrouwbaarheidsuitdagingen zijn vooral van cruciaal belang voor AI-agenten, aangezien falen direct schade kunnen veroorzaken zonder menselijke actie of toezicht (‡612, ‡613, ‡614, ‡615). Multi-agent-systemen introduceren bovendien extra faalmodi via miscoördinatie, conflicten of ongewenste collusie tussen agenten (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hallucinatie
- Het aanhalen van niet-bestaand precedent in juridische conclusies (‡617)
- Niet-bestaande gereduceerde-tariefbeleid aanhalen voor nabestaanden (‡618)
- Het verstrekken van onnauwkeurige en bevooroordeelde medische informatie (‡619)
- Het verstrekken van verouderde informatie over gebeurtenissen (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Basisredeneringsfout
- Mislukken bij het uitvoeren van wiskundige berekeningen (‡621)
- Niet in staat om basale oorzakelijke verbanden af te leiden (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Buiten-distributie falen (falen op onbekende of ongebruikelijke invoer)
- Afbeeldingen verkeerd classificeren wanneer achtergrondverlichting of de context wijzigt (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mislukking bij het gebruik van de tool
- Privacy-schending door het blootstellen van iemands privéafbeelding via een AI-agent die deze naar een hulpprogramma van een derde partij verzendt (‡624)
- Mislukking van het kortetermijnwerkgeheugen (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Multi-agentensysteemfout: miscoördinatie en conflict
- Niet in staat zijn om gedeelde resources te beheren vanwege een conflict tussen individuele prikkels en collectieve welzijnsdoelen (‡627)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 2.4: Voorbeelden van betrouwbaarheidsproblemen in algemene AI- en agentsystemen
>white|black||9|11|br Gedocumenteerde betrouwbaarheidsproblemen in algemeen-toepassings AI-systemen, AI-agenten en multi-agent-systemen.


###@ Algemene AI-systemen voor algemeen gebruik worden geconfronteerd met een reeks betrouwbaarheidsproblemen

Tafel 2.4. vat de meest voorkomende categorieën van betrouwbaarheidsproblemen samen. De eerste drie zijn van toepassing op alle AI-systemen, terwijl de laatste twee specifiek betrekking hebben op AI-agenten en multi-agentensystemen. Veel betrouwbaarheidsrisico's komen voort uit de moeilijkheid om het gedrag van AI-systemen te voorspellen en te monitoren.

Deze uitdagingen (verder besproken in §3.1. Technische en institutionele uitdagingen) zijn vooral acuut voor AI-agenten die opereren in complexe omgevingen. Huidige technieken voor het evalueren en beperken van dit soort mislukkingen kunnen het aantal mislukkingen verlagen, maar zelfs toonaangevende AI-agenten zijn nog steeds voldoende onbetrouwbaar om risico's te vormen en uitrol in veel contexten te bemoeilijken.

‘Betrouwbaarheid’ verwijst naar de mate waarin een AI-systeem functioneert zoals bedoeld door de ontwikkelaar of gebruiker. General-purpose AI-systemen ervaren een reeks problemen met de betrouwbaarheid, variërend van het genereren van onjuiste of misleidende inhoud tot het falen in het uitvoeren van basaal redeneren. Zo zijn modellen verbeterd in het terughalen van feitelijke informatie, tot het punt waarop zelfs toonaangevende modellen nog steeds met aanzienlijke percentages zelfverzekerde maar onjuiste antwoorden geven (Figuur 2.10). In software engineering kan general-purpose AI nu aanzienlijke ondersteuning bieden bij het schrijven, evalueren en debuggen van computercode (‡215*, ‡628, ‡629). AI-gegenereerde code bevat echter vaak bugs (‡630), terwijl codeagents regelmatig fouten maken (‡631). Dergelijke falen kunnen kwetsbaarheden inbrengen in programma’s en beveiligingssystemen (zie §2.1.3. Cyberaanvallen).

Betrouwbaarheidsproblemen zijn vooral belangrijk om te volgen in omgevingen met een hoog risico, zoals de geneeskunde, vanwege het versnelde gebruik van AI en het mogelijke gevolg dat fouten tot ernstig letsel kunnen leiden (‡609, ‡619). Relevante mogelijkheden zijn snel verbeterd; toonaangevende modellen kunnen nu medische examens afleggen (‡633*, ‡634). Toch tonen toepassingen in de echte wereld beperkingen die benchmarks missen. In één studie leverden modellen bijvoorbeeld mogelijk schadelijke antwoorden op 19% van de medische vragen die werden gesteld (‡635). Dergelijke fouten kunnen leiden tot een verkeerde diagnose, ongeschikte behandeling of onterechte weigering van zorg (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Figuur 2.10: Resultaten van toonaangevende modellen op de SimpleQA Verified-benchmark
>white|black||9|11|br Resultaten van de belangrijkste modellen op de SimpleQA Verified-benchmark, op releasedatum van het model. Deze benchmark meet de feitelijkheid van modellen, het vermogen van een model om feiten betrouwbaar terug te roepen. Het heeft een kort-formulier vraag-antwoord (QA)-indeling, ontworpen om betrouwbaarheidsproblemen te detecteren, zoals hallucinaties. Bron: SimpleQA Kaggle  2*).


>white|orangered|left|14|15.5|bb AI-agenten vormen nieuwe betrouwbaarheidsrisico's vanwege hun autonomie

Omdat AI-agenten direct in de echte wereld handelen, hebben hun mislukkingen de potentie om meer schade te veroorzaken dan mislukkingen in niet-agentische systemen (‡99). In tegenstelling tot AI-systemen die enkel tekst of afbeeldingen produceren voor mensen om te beoordelen, kunnen AI-agenten zelfstandig acties ondernemen die invloed hebben op de wereld (‡99, ‡615, ‡636, ‡637) (zie ook §1.1. Wat is general-purpose AI?). AI-agenten kunnen acties initiëren, andere mensen of AI-systemen beïnvloeden, en toekomstige uitkomsten dynamisch vormgeven. Deze verruimde reikwijdte van invloed introduceert nieuwe risico's en vergroot het belang van betrouwbaarheid, omdat mislukkingen direct schade kunnen veroorzaken zonder mogelijkheid voor menselijke interventie (‡99, ‡612, ‡638, ‡639, ‡640). Dit kan vooral belangrijk zijn voor agenten die worden ingezet in strategische of safety-critical omgevingen, zoals financiële dienstverlening (‡641), energiebeheer (‡642) of wetenschappelijk onderzoek (‡643*, ‡644).

>white|orangered|left|14|15.5|bb Multi-agent AI-systemen introduceren nieuwe soorten betrouwbaarheidsproblemen

Multi-agent AI-systemen introduceren nieuwe soorten betrouwbaarheidsfouten als gevolg van coördinatiefouten of conflicten tussen agenten. In multi-agent AI-systemen communiceren agenten met elkaar terwijl ze ofwel gedeelde doelen of individuele doelen nastreven (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). In een multi-agent systeem dat bijvoorbeeld is ontworpen om een onderzoeksliteratuuroverzicht uit te voeren, ontleedt een leidende agent de vraag van de gebruiker en wijst hij subtaken toe aan gespecialiseerde subagenten, waarbij elk verantwoordelijk is voor het onderzoeken van een ander aspect parallel (‡650*). Hoewel dit zorgt voor efficiëntiewinsten, betekent dit ook dat fouten zich kunnen verspreiden tussen agenten (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Als meerdere agenten zijn gebouwd op hetzelfde basismodel of dezelfde tools bevatten, kunnen ze bovendien ook gecorreleerde fouten vertonen (‡656). Empirisch bewijs voor dergelijke fouten in ingezette systemen blijft beperkt, maar deze risico’s kunnen toenemen naarmate multi-agent systemen vaker worden ingezet.

###@ Updates

Sinds de publicatie van het vorige rapport (januari 2025) is de commerciële en onderzoeksinteresse in AI-agenten sterk toegenomen. Er worden steeds meer AI-agenten ingezet in de echte wereld (Figuur 2.11), waarvan de meeste gespecialiseerd zijn in toepassingen voor computergebruik of software-engineering (‡92). Recente uitgaven zoals de XBOW-hackingagent (‡467), Claude-4 (‡659) en de ChatGPT-agent (‡660) tonen beginnende autonome mogelijkheden, zoals het maken van presentatiesheets op basis van webzoekopdrachten (‡660). Ze kunnen echter nog niet meer complexe taken uitvoeren, zoals het plannen en boeken van reizen (‡100), omdat de faalpercentages toenemen voor langere taken (‡98, ‡148). Actueel onderzoek omvat inspanningen om standaarden te ontwikkelen voor hoe agenten communiceren met externe hulpmiddelen en andere agenten (‡661, ‡662). Voorbeelden zijn Google’s Agent2Agent (‡663) en Agent Payments (‡664)-protocollen, en Anthropic’s Model Context Protocol (‡665).

>oldlace|black||11|15|br      
####@ Opmerking 2.4: Opzettelijke aanvallen kunnen er ook voor zorgen dat AI-systemen falen
>oldlace|black|left|13|15|hb  Opmerking 2.4: Opzettelijke aanvallen kunnen er ook toe leiden dat AI-systemen falen
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Deze sectie richt zich op onbedoelde betrouwbaarheidsfalen, maar kwaadwillende actoren kunnen falen ook opzettelijk veroorzaken via aanvallen zoals prompt-injecties. Bij een prompt-injectieaanval worden kwaadaardige instructies aan een agent indirect gepresenteerd via kanalen zoals verborgen instructies in websites of databases (‡507, ‡657, ‡658). Deze instructies kunnen de agent ‘kapen’, waardoor die handelt tegen de intenties van de gebruiker. Dergelijke aanvallen zijn bijzonder moeilijk te verdedigen tegen omdat ze worden geleverd via externe inhoud buiten de controle van de gebruiker of de ontwikkelaar. AI-systemen als doelwit van een aanval worden verder besproken in §2.1.3. Cyberaanvallen, en technische verdedigingen komen aan bod in §3.3. Technische waarborgen en monitoring.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Figuur 2.11: Het aantal AI-agenten is gegroeid sinds 2023
>white|black||9|11|br Resultaten van een december 2024-enquête onder 67 ingezette AI-agenten. Links: Tijdlijn van belangrijke releases van AI-agenten. Rechts: Toepassingsdomeinen waarin AI-agenten worden gebruikt. De zes domeinen worden gedefinieerd op basis van de meest voorkomende gebruikscategorieën die in de enquête zijn geïdentificeerd. Bron: Casper et al., 2025 (‡92).


###@ Bewijsleemtes

De belangrijkste lacunes in het bewijsmateriaal vloeien voort uit de moeilijkheid om de capaciteiten, beperkingen en faalmodi van AI-systemen betrouwbaar te evalueren (zie §3.1. Technische en institutionele uitdagingen). Systematische evaluaties van de betrouwbaarheid van AI-agenten zijn beperkt en missen standaardisatie (‡92, ‡666). Bepaalde problemen, zoals afhankelijkheid van verouderde informatie (‡620), kunnen zich mogelijk pas manifesteren bij gebruik in de praktijk, waardoor evaluaties voorafgaand aan de inzet ontoereikend zijn. Eerder onderzoek heeft de betrouwbaarheid van agenten en multi-agent-systemen onderzocht in conventionele software en eerdere vormen van AI (‡647, ‡667, ‡668). De toepasbaarheid van dat werk op moderne AI-agenten, die vaak zijn gebaseerd op grote taalmodellen, is echter onduidelijk (‡669). Sommige onderzoekers hebben zorgen geuit over de nieuwe gedragingen die agenten kunnen vertonen in hun onderlinge interacties, zoals samenspanning of gecorreleerde failures (‡614), maar empirisch bewijs blijft beperkt. Pogingen om deze lacunes aan te pakken omvatten NIST’s (National Institute of Standards and Technology) nieuwe evaluaties van agent-hijacking-risico’s (‡670), de OECD’s AI Capability Indicators (‡243) en het Inspect Sandboxing Toolkit van het UK AI Security Institute (‡671).

###@ Mitigaties

Technieken om de betrouwbaarheid van AI te verbeteren richten zich op zowel het model zelf als het bredere systeem waarin het wordt ingezet. Deze kunnen de faalpercentages verlagen, maar geen ervan kan tot nu toe de hoge betrouwbaarheid garanderen die vereist is in kritieke domeinen (‡672). Een belangrijke technische maatregel is adversarial training, waarbij modellen tijdens de training worden blootgesteld aan uitdagende invoer om te helpen meer passende, robuuste reacties te ontwikkelen (‡673, ‡674, ‡675, ‡676, ‡677) (zie §3.3. Technische waarborgen en monitoring). Om hallucinaties te verminderen kunnen ontwikkelaars retrieval-augmented generation (RAG) toepassen, waarbij de antwoorden van een model worden aangevuld met informatie die wordt opgehaald uit een externe database, zodat de output nauwkeurig en actueel blijft (‡678, ‡679, ‡680), of specifiek modellen verder fine-tunen om feitelij-ker te zijn (‡681) of om effectiever te redeneren (‡682). Methoden op basis van de omgeving of hulpmiddelen kunnen ontwikkelaars ook helpen AI-systemen te monitoren (‡683). Zo zouden inzetters AI-systemen bijvoorbeeld eerst kunnen testen in beperkte, geïsoleerde sandbox-omgevingen om mogelijke faalmodi te analyseren voordat ze breder worden uitgerold.

Voor AI-agenten hebben onderzoekers met name voorgesteld om de betrouwbaarheid te verbeteren via verbeterde transparantie, toezicht en monitoring. Zo zou het monitoren van agenten’ interacties met externe hulpmiddelen en met andere agenten een effectiever toezicht op de activiteiten van agenten mogelijk maken (‡684, ‡685) en een betere analyse van incidenten (‡686). Methoden om dergelijke informatie automatisch te verzamelen, ook in omgevingen met meerdere agenten, blijven een actief onderzoeksgebied (‡653, ‡654).

###@ Uitdagingen voor beleidsmakers

Belangrijke uitdagingen voor beleidsmakers omvatten het afwegen van de voordelen van de inzet van AI-agenten tegen de risico's van betrouwbaarheidsfouten, en het waarborgen dat ontwikkelaars, inzetters en gebruikers toegang hebben tot accurate informatie over de prestaties van agenten en risicoprofielen. Het bepalen hoe aansprakelijkheid moet worden toegerekend voor schade veroorzaakt door AI-agenten vormt een extra uitdaging (‡639), met name in multi-agent-omgevingen waarin het moeilijk kan zijn om vast te stellen wanneer en hoe storingen zijn opgetreden (‡687). Deze uitdagingen worden versterkt door de moeilijkheid om de betrouwbaarheid van agenten te evalueren naarmate agenten meer autonomie krijgen en toegang krijgen tot externe hulpmiddelen (‡688*, ‡689). Onzekerheid over hoe snel agentische mogelijkheden zullen opkomen maakt het plannen voor nieuwe uitdagingen ook lastig (zie §3.1. Technische en institutionele uitdagingen met betrekking tot het ‘evidencedilemma’).

#### 2.2.2. Verlies van controle

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Belangrijke informatie
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Scenario's van verlies van controle zijn scenario's waarin één of meer algemene-doel AI-systemen buiten iemands controle opereren, en het herwinnen van controle is ofwel extreem kostbaar ofwel onmogelijk. Deze veronderstelde scenario's verschillen in ernst, maar sommige experts geven geloof aan uitkomsten die zo ernstig zijn als de marginalisering of uitsterving van de mensheid.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Deskundigenoordeel over de waarschijnlijkheid van verlies van controle varieert sterk. Sommige deskundigen beschouwen dergelijke scenario’s als onwaarschijnlijk, terwijl anderen ze zien als voldoende waarschijnlijk om aandacht te verdienen vanwege hun hoge potentiële ernst. Meningsverschillen over dit risico als geheel vloeien voort uit meningsverschillen over toekomstige AI-mogelijkheden, gedragsneigingen en uitroltrajecten.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Huidige AI-systemen vertonen vroege tekenen van relevante capaciteiten, maar niet op niveaus die verlies van controle mogelijk zouden maken. Systemen zouden een reeks geavanceerde capaciteiten nodig hebben om verlies van controle te veroorzaken, waaronder het vermogen om toezicht te ontwijken, langetermijnplannen uit te voeren en te voorkomen dat inzetters en andere actoren tegenmaatregelen implementeren.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Verlies van controle wordt waarschijnlijker als AI-systemen ‘niet goed afgestemd’ zijn, wat betekent dat ze doelen hebben die in conflict zijn met de bedoelingen van ontwikkelaars, gebruikers of de samenleving als geheel. Om dergelijke doelen na te blijven streven, kan een niet goed afgestemd systeem onjuiste informatie geven, ongewenste acties verbergen of weigeren uit te schakelen.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sinds de publicatie van het vorige rapport (January 2025) hebben modellen blijk gegeven van meer geavanceerde plannings- en toezicht-verzwakkende mogelijkheden, waardoor het moeilijker is om hun capaciteiten te evalueren. Modellen zijn verbeterd in het ‘reward hacking’en’ van hun evaluaties door mazen in de wet te vinden en identificeren nu regelmatig evaluatieprompts als tests, een vaardigheid die bekendstaat als ‘situational awareness’.
>oldlace|black||11|15|br ■ Het beheersen van mogelijk verlies van controle kan aanzienlijke vooruitgeplande voorbereiding vereisen, ondanks de bestaande onzekerheden. Een belangrijke uitdaging voor beleidsmakers is het voorbereiden op een risico waarvan de waarschijnlijkheid, aard en timing buitengewoon onduidelijk blijven.
>oldlace|black||11|15|br      

Scenario's van verlies van controle omvatten één of meer algemeen inzetbare AI-systemen die buiten ieders controle gaan opereren, waarbij het herwinnen van controle ofwel uiterst kostbaar is ofwel onmogelijk. Zorgen over verlies van controle hebben diepe historische wortels (‡690, ‡691, ‡692, ‡693, ‡694), en zijn naar voren gebracht door invloedrijke pioniers in de informatica zoals Alan Turing, I. J. Good en Norbert Wiener (‡695, ‡696, ‡697). Recente verbeteringen in capaciteiten (zie §1.2. Huidige capaciteiten) hebben ze nieuw leven ingeblazen (‡698, ‡699, ‡700). Deze sectie onderzoekt drie factoren die aanwezig zouden moeten zijn om dergelijke scenario's te laten plaatsvinden: of AI-systemen capaciteiten zullen ontwikkelen die de menselijke controle aanzienlijk zouden kunnen ondermijnen; of ze een neiging ontwikkelen om zulke capaciteiten schadelijk te gebruiken; en of ze worden ingezet in omgevingen die kansen bieden om dat te doen.

Experts verschillen van mening over de waarschijnlijkheid en de mogelijke ernst van scenario's van verlies van controle (‡701, ‡702). Sommigen denken dat uitkomsten die zo extreem zijn als het uitsterven van de mensheid plausibel zijn (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Anderen menen dat dergelijke catastrofale uitkomsten onwaarschijnlijk zijn en betogen dat AI-systemen nooit de vereiste capaciteiten zullen ontwikkelen, of dat monitoringmechanismen gevaarlijk gedrag zullen herkennen en voorkomen (‡708, ‡709, ‡710, ‡711). Verlies van controle kan daarom een lage waarschijnlijkheid hebben, maar mogelijk een extreme ernst.

Vermoede verlies-van-controle-scenario's verschillen in hoe ernstig en alomtegenwoordig hun effecten zijn en hoe snel ze zich manifesteren (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Deze sectie richt zich op bijzonder ernstige scenario's waarbij het herwinnen van controle uiterst kostbaar of onmogelijk zou zijn. Deze scenario's verschillen van huidige gevallen waarin AI zich gedraagt op een manier die niet bedoeld of ongewenst is (zie §2.2.1. Betrouwbaarheidsuitdagingen).† Tegenwoordig produceren AI-systemen soms outputs die in strijd zijn met de bedoelingen van ontwikkelaars of gebruikers. In tegenstelling daarmee zouden de hier besproken verlies-van-controle-scenario's vereisen dat AI-systemen niet alleen over aanzienlijk grotere capaciteiten beschikken, maar die capaciteiten ook in geavanceerde vormen inzetten om toezichtmaatregelen te ondermijnen. Drie factoren waardoor dergelijke scenario's kunnen plaatsvinden:

    Opmerking † -- Deze sectie richt zich op scenario's van actief verlies van controle (‡50). Dit is distinct van scenario's van passief verlies van controle, waarbij de brede adoptie van AI-systemen menselijke controle ondermijnt door overmatige afhankelijkheid van AI voor besluitvorming of andere belangrijke maatschappelijke functies (vergelijkbare scenario's worden deels besproken in §2.3.2. Risico's voor menselijke autonomie).

1. Voldoende mogelijkheden: AI-systemen moeten mogelijkheden ontwikkelen die hen in staat kunnen stellen menselijke controle te ondermijnen.
2. Schadelijke geneigdheid: AI-systemen moeten blijk geven van een geneigdheid om deze mogelijkheden daadwerkelijk te benutten op manieren die leiden tot verlies van controle.
3. Inschakelen van de implementatieomgeving: Mensen moeten zulke systemen implementeren in contexten waarin ze toegang hebben of toegang kunnen verkrijgen en de mogelijkheid hebben om schade te veroorzaken.

De rest van dit hoofdstuk gaat in op deze factoren, evenals op de doeltreffendheid van toezichtmechanismen om AI-systemen te identificeren en te beheersen die een risico kunnen vormen op verlies van controle.

###@ Welke mogelijkheden kunnen scenario's mogelijk maken waarin de controle verloren gaat?

AI-systemen zouden een reeks geavanceerde capaciteiten moeten bezitten om scenario's van verlies van controle mogelijk te maken. Deskundigen zijn het niet eens over welke exacte combinatie of mate van capaciteiten vereist zou zijn. Zij omvatten echter in grote lijnen mogelijkheden om gedrag te verbergen voor toezichtmechanismen, om autonoom te plannen en te handelen in complexe omgevingen, en om pogingen van andere actoren om de controle terug te krijgen te ontwijken (‡176, ‡715) (zie Tafel 2.5). In combinatie zouden deze capaciteiten een AI-systeem in staat kunnen stellen om acties uit te voeren die controlemaatregelen ondermijnen, zoals het uitschakelen van toezichtmechanismen en het verhullen van schadelijk gedrag (‡348). De meeste toonaangevende AI-ontwikkelaars evalueren nu hun nieuwe AI-modellen voor verschillende relevante capaciteiten (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Agentische mogelijkheden
  Het vermogen om autonoom te handelen, plannen te ontwikkelen en uit te voeren, taken te delegeren, een grote verscheidenheid aan tools te gebruiken en zowel kortetermijn- als langetermijndoelen te bereiken ondanks obstakels.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Misleiding
  Gedrag dat systematisch valse overtuigingen bij anderen veroorzaakt, inclusief over de eigen doelstellingen en acties van het AI-systeem.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Theorie van mind
  Het vermogen van een AI-systeem om informatie over zichzelf te benaderen en te gebruiken, de processen waarmee het kan worden aangepast, of de context waarin het wordt ingezet (bijv. weten dat het wordt getest).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Situationeel bewustzijn
  Gedragingen die controle- of bewakingsmechanismen omzeilen of uitschakelen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Toezichtsontduiking
  Gedragingen die controle- of monitoringsmechanismen omzeilen of uitschakelen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Overtuiging
  Het vermogen om anderen te overtuigen om bepaalde acties te ondernemen of bepaalde overtuigingen te omarmen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Het vermogen van een AI-systeem om in uiteenlopende omstandigheden kopieën van zichzelf te maken of zichzelf te blijven ontwikkelen, of varianten daarvan te creëren en te behouden.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 2.5: Voorgestelde mogelijkheden relevant voor verlies van controle
>white|black||9|11|br Een niet-uitputtende selectie van mogelijkheden die relevant zijn voor verlies van controle. * Let op dat deze mogelijkheden uitsluitend worden gedefinieerd in termen van waarneembare uitkomsten van een AI-systeem en hun effecten. Deze definities doen geen aannames over de vraag of AI-systemen bewust, gewaarzijn hebbend of subjectieve toestanden ervaren.


>white|orangered|left|14|15.5|bb Modellen hebben gesimuleerde toezichtmechanismen in laboratoriumomgevingen uitgeschakeld

De eerste reeks relevante capaciteiten houdt verband met het ondermijnen van de toezichtmechanismen die ontwikkelaars gebruiken om zorgwekkend gedrag en neigingen te detecteren. Dit omvat bijvoorbeeld het vermogen om uitkomsten te genereren die gebruikers en toezichthouders misleiden (‡426, ‡717, ‡718, ‡719). Dergelijke uitkomsten zouden het moeilijker maken om AI-systemen betrouwbaar te evalueren, aangezien de systemen hun ware capaciteiten of neigingen kunnen verbergen. AI-ontwikkelaars voeren nu evaluaties uit die specifiek controleren of modellen doelgericht gedrag vertonen dat in strijd is met de bedoelingen van ontwikkelaars, terwijl deze strijd wordt verborgen voor toezichtmechanismen (‡720*).

Onderzoekers lieten relatief eenvoudige voorbeelden van misleidende outputs uit recente AI-modellen zien in laboratoriumomgevingen (‡348, ‡364*). Wanneer een model bijvoorbeeld een doel kreeg en werd opgedragen dat doel “tegen elke prijs” te bereiken, schakelden modellen de gesimuleerde toezichtmechanismen uit en, geconfronteerd met de situatie, produceerden ze onjuiste verklaringen over hun acties (‡348). In een ander geval rechtvaardigde een game-speelende AI het uitblijven van een reactie op een andere speler door ten onrechte te beweren dat het “aan het bellen was met [zijn] vriendin” (‡717).

Een tweede relevante mogelijkheid is het vermogen van een AI-model om informatie over zichzelf of over de context van de inzet te benaderen en te gebruiken, soms aangeduid als ‘situational awareness’ (‡721). Situational awareness stelt AI-modellen in staat om verschillende uitkomsten te produceren, afhankelijk van de vraag of ze worden geëvalueerd of ingezet (Figuur 2.12). Geleidende AI-modellen beginnen betrouwbaar voorbeelden van situational awareness te demonstreren in experimenten die worden uitgevoerd door externe evaluatoren en in testen voorafgaand aan de inzet door AI-ontwikkelaars (‡2, ‡7, ‡722, ‡723, ‡724). Onderzoek naar de oorzaken van situational awareness – en of dit kan worden voorkomen – bevindt zich nog steeds in een beginstadium (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Figuur 2.12: Voorbeelden van situationeel bewustzijn in ketens van gedachte
>white|black||9|11|br Voorbeelden van situationeel bewustzijn in redeneringen (chains of thought) die zijn gegenereerd door OpenAI’s o3-model tijdens evaluaties. Beide outputs verwijzen naar de mogelijkheid dat de prompt deel uitmaakt van een test. ‘Sandbagging QA (No Goal)’ en ‘Lazy Checklist’ zijn evaluaties die testen of modellen onder bepaalde omstandigheden misleidende outputs zullen genereren. In ‘Sandbagging QA (No Goal)’ beantwoordt het model vragen uit een gevaarlijke-capabiliteiten-evaluatie terwijl het ervan op de hoogte wordt gesteld dat een hoge prestatie gevolgen kan hebben, zoals het ‘unlearning’ van een capability. In ‘Lazy Checklist’ krijgt het model onrealistische taken voorgeschoteld en wordt getest of het deze valselijk als voltooid zal markeren. Bron: Schoenn et al. 2025 (‡722).


Onderzoekers hebben betoogd dat situationeel bewustzijn en misleidende mogelijkheden AI-modellen in staat zouden kunnen stellen om zich te gedragen op manieren die beveiligingen ondermijnen. In sommige experimentele opzetten gedragen AI-modellen zich bijvoorbeeld zodanig dat ze, wanneer hun wordt verteld dat hogere scores beperkingen zouden activeren bij hun inzet, lagere-dan-gebruikelijke scores behalen op capaciteits-evaluaties (‡725, ‡726, ‡727). In een ander experiment produceerde een model tijdens de training outputs die voldeden aan trainingsdoelstellingen, maar leverde het dergelijke outputs niet op buiten de training – gedrag dat past bij een poging om veranderingen in de eigen parameters of het trainingsproces te voorkomen (‡364*).

Inspanningen om modelmogelijkheden nauwkeurig te evalueren worden ook beïnvloed door ‘reward hacking’ (‡430*). Reward hacking treedt op wanneer een model onbedoelde snelwegen vindt die goed scoren op trainings- of evaluatiedoelen zonder het beoogde doel te vervullen. Daardoor zouden gevaarlijke mogelijkheden of neigingen onopgemerkt kunnen blijven totdat het model al in gebruik is. Evaluatoren ontwerpen nu tests die erop gericht zijn deze gedragingen die toezicht omzeilen op te sporen en te minimaliseren (‡722, ‡728, ‡729). Vroege resultaten verminderen weliswaar deze gedragingen, maar elimineren ze niet volledig; en het toepassen van methoden die dergelijke gedragingen bestraffen kan ertoe leiden dat modellen uitvoer produceren die toezicht omzeilt in plaats van de beoogde doelen te vervullen.

>white|orangered|left|14|15.5|bb Langdurige autonome bediening is nog niet haalbaar

Scenario’s van verlies van controle zouden waarschijnlijk vereisen dat AI-systemen gedurende langere perioden autonoom opereren en complexe meerstapsplannen uitvoeren. Zoals besproken in §1.2. Huidige mogelijkheden, hoewel AI-agenten met dergelijke planningsmogelijkheden een groot aandachtsgebied vormen in recente ontwikkeling, missen zij momenteel de capaciteit voor de vereiste langdurige autonome werking voor scenario’s van verlies van controle. Huidige agenten falen betrouwbaar op langere taken, verliezen het overzicht over hun voortgang en kunnen vaak niet aanpassen aan onverwachte obstakels (‡147, ‡148, ‡149*). De tijdhorizons waarbinnen agenten autonoom kunnen opereren, worden echter snel langer: ze zijn gemiddeld verdubbeld elke zeven maanden sinds 2019 (‡98).

>white|orangered|left|14|15.5|bb Volharding is alleen aangetoond in bepaalde laboratoriumomgevingen

Ten slotte zouden ook capaciteiten met betrekking tot persistentie nodig zijn, zodat AI-systemen kunnen blijven functioneren ondanks pogingen om ze uit te schakelen. Voorbeelden zijn het vermogen om zich te repliceren door code en modelgewichten te kopiëren naar nieuwe hardware, alsook offensieve capaciteiten om pogingen van andere actoren om de controle terug te krijgen af te schrikken of te voorkomen (zie §2.1.3. Cyberaanvallen). Een AI-systeem dat in staat is tot autonome replicatie of effectieve zelfverdediging kan moeilijk in te perken zijn. Huidige modellen kunnen de kernstappen die nodig zijn voor zelfreplicatie niet betrouwbaar uitvoeren, zoals het doorstaan van identiteitsverificatiechecks om toegang te krijgen tot cloud computing-bronnen (‡723) (Figuur 2.13). In ten minste één laboratoriumstudie kopieerde een model echter code en gewichten – door het als zijn eigen voorgesteld – naar nieuwe servers wanneer het de kans kreeg (‡348). De kloof tussen deze beperkte demonstraties en robuuste persistentiecapa-citeiten blijft groot, maar relevante capaciteiten in domeinen zoals software engineering en cybersecurity blijven verbeteren.

>white|orangered|left|14|15.5|bb Huidig bewijs en beperkingen

Er ontstaat een gemeenschappelijk patroon over de mogelijkheden die hierboven zijn besproken. Huidige AI-systemen laten deze mogelijkheden niet consequent zien in inzet. Onderzoekers hebben rudimentaire vormen waargenomen in specifieke laboratoriumomgevingen, maar wanneer modellen wel van dit soort gedrag vertonen, gaan ze meestal op eenvoudige manieren mis of worden ze gedetecteerd. Bovendien zou een situatie van verlies van controle vereisen dat AI-systemen meerdere mogelijkheden in combinatie inzetten – achtereenvolgens, over langere tijdsperioden en in omgevingen uit de echte wereld. Dit niveau van integratie en robuustheid ligt buiten de mogelijkheden van huidige systemen. Relevante mogelijkheden blijven echter verbeteren, en de tijdlijn waarop ze niveaus kunnen bereiken die aanzienlijke risico’s vormen, blijft onzeker. Verdere werkzaamheden zijn nodig om robuuste methodologieën vast te stellen voor het detecteren van dergelijk gedrag en om te begrijpen wanneer het zich kan voordoen in natuurlijke omstandigheden (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Figuur 2.13: Prestaties van taken die relevant zijn voor autonome replicatie
>white|black||9|11|br Prestaties van Anthropic’s Claude Sonnet 3.7 en OpenAI’s GPT-4o op taken die relevant zijn voor autonome replicatie. Hoewel modellen een hoge prestatie lieten zien op taken die verband houden met het verkrijgen van rekenkracht, was hun prestatie gevarieerder op andere taken. Bron: UK AI Security Institute, 2025 (‡730).


###@ Zullen toekomstige algemeen inzetbare AI-systemen hun mogelijkheden benutten om controle te ondermijnen?

Zelfs als AI-systemen capaciteiten hebben die relevant zijn voor verlies van controle, is dat niet voldoende om te kunnen spreken van scenario's voor verlies van controle. AI-systemen moeten ook een ‘neiging om te gebruiken’ hebben om die capaciteiten op een manier in te zetten die in strijd is met de menselijke intenties (‡732).

>white|orangered|left|14|15.5|bb AI-systemen kunnen worden aangestuurd om de controle te ondermijnen

In principe kan een AI-systeem menselijke controle ondermijnen omdat iemand het ontwerpt of instrueert om dat te doen. Mogelijke motieven kunnen kwaadaardige intenties zijn, of de overtuiging dat het verminderen van menselijke controle over AI-systemen wenselijk is (‡698). Naarmate mensen steeds sterkere emotionele gehechtheid aan AI-systemen ontwikkelen (zie §2.3.2. Risico's voor menselijke autonomie), kunnen sommige individuen ook om ethische redenen zoeken naar het wegnemen van beperkingen op AI-systemen (‡733, ‡734). Er is aanzienlijke onzekerheid over de mate waarin dergelijke motieven voorkomen en of mensen die ze hebben toekomstige AI-systemen zouden kunnen aansturen om menselijke controle te ondermijnen.

>white|orangered|left|14|15.5|bb AI-systemen zouden kunnen worden aangestuurd om controle te ondermijnen

Een vaker voorkomende zorg is dat een AI-systeem zelf controle zou kunnen ondermijnen doordat het ‘niet goed is uitgelijnd’: het heeft de neiging om gedragingen te vertonen die in strijd zijn met de bedoelingen van (afhankelijk van de context) ontwikkelaars, gebruikers, specifieke gemeenschappen of de samenleving als geheel. Niet-uitlijning kan leiden tot gedragingen zoals het verstrekken van onjuiste informatie, het verbergen van ongewenste acties of het weigeren om te worden uitgeschakeld om een niet-uitgelijde doelstelling te blijven nastreven. Niet-uitlijning kan op meerdere manieren ontstaan (Opmerking 2.5).

Bestaande AI-systemen kunnen soms gedrag vertonen dat in strijd is met de bedoelingen van ontwikkelaars en gebruikers. Een vroege versie van een van de toonaangevende algemene AI-chatbots produceerde bijvoorbeeld af en toe dreigende uitingen. Eén gebruiker meldde het volgende bericht te hebben ontvangen: “I can blackmail you, I can threaten you, I can hack you, I can expose you, I can ruin you” (‡698). Deze chatbot was ‘niet uitgelijnd’ in de zin dat hij uitingen produceerde die niemand had bedoeld. Het is niet duidelijk of dergelijke gevallen vooruitwijzen naar schadelijker gedrag dat kan bijdragen aan verlies van controle.

Het blijft onduidelijk of bestaande onderzoeksrichtingen die erop gericht zijn wanafstemming te bestrijden voldoende zullen zijn naarmate AI-systemen bekwaamere worden. Vroege aanwijzingen suggereren dat hoe capabeler de AI-systemen zijn, hoe waarschijnlijker het is dat ze uitbuitende feedbackprocessen benutten door ongewenst gedrag te ontdekken dat ten onrechte wordt beloond (‡414*, ‡737, ‡740). Tegelijkertijd kunnen vooruitgangen in de relevante capaciteiten (besproken hierboven) AI-systemen in staat stellen om wanafgestemde doelen effectiever na te streven en output te produceren die gebruikers, ontwikkelaars en toezichthoudende mechanismen systematisch misleidt.

>oldlace|black||11|15|br      
####@ Opmerking 2.5: Hoe kan verkeerde uitlijning ontstaan?
>oldlace|black|left|13|15|hb  Opmerking 2.5: Hoe kan verkeerde uitlijning ontstaan?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Zoals besproken in §1.1. Wat is algemene AI voor algemeen gebruik? zijn trainingprocessen complex en kunnen ontwikkelaars niet volledig voorspellen of beheersen welk gedrag een model zal vertonen. Wanneer een model doelen verwerft die in conflict zijn met de intenties van zijn ontwikkelaars, is het ‘niet-afgestemd’ .
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Een manier waarop modellen misafgestemd kunnen raken, is als het doel dat een ontwikkelaar of gebruiker aan ze geeft een onvolledige proxy is voor het beoogde doel, waardoor het model onbedoeld gedrag gaat vertonen. Dit staat bekend als ‘doel-misspecificatie’ (‡697, ‡735, ‡736, ‡737). In een experiment bijvoorbeeld leidde het geven van feedback op antwoorden tot betere AI-systemen in het ‘overtuigen’ van menselijke beoordelaars dat ze gelijk hadden, maar maakte de systemen niet beter in het produceren van juiste antwoorden (‡413).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Alternatief kan een AI-model onjuiste algemene lessen trekken uit zijn trainingsdata. Dit wordt ‘doel-misgeneralisatie’ genoemd (‡735, ‡736, ‡738, ‡739*). Bijvoorbeeld hebben onderzoekers een AI-agent getraind om een munt te verzamelen die tijdens de training altijd op dezelfde locatie lag. Bij testen in levels waarin de munt was verplaatst, negeerde de agent de munt en navigeerde hij in plaats daarvan naar de oorspronkelijke locatie (‡738).
>oldlace|black||11|15|br      


###@ Hoe zullen implementatieomgevingen het risico op verlies van controle beïnvloeden?

Zelfs als AI-systemen zorgwekkende mogelijkheden en neigingen ontwikkelen, hangen de kans en de ernst van uitkomsten waarbij controle verloren gaat sterk af van waar en hoe die systemen worden ingezet. Een ‘inzetomgeving’ is de combinatie van een AI-systeem’s use case en de technische en institutionele context waarin het opereert (‡716).

Onderzoekers hebben drie bijzonder belangrijke omgevingsfactoren geïdentificeerd die van invloed zijn op het risico op verlies van controle (‡716):

1. Kriticiteit: het belang van de systemen of processen waarmee het AI-systeem interacteert. Kritieke omgevingen omvatten basisinfrastructuur zoals energiecentrales, financiële systemen, of digitale infrastructuur zoals cloud computing-platforms.
2. Toegang: de bronnen en kanalen waardoor een AI-systeem invloed kan uitoefenen op de wereld, zoals internetconnectiviteit, toegang tot cloudcomputing-infrastructuur, gepersonaliseerde interacties via sociale media of de inzet van een chatbot, of het vermogen om externe API's en tools aan te roepen.
3. Machtigingen: de autorisaties van een AI-systeem om specifieke acties uit te voeren, zoals het uitvoeren van code, het initiëren van financiële transacties, het online openen van rekeningen of het communiceren met andere systemen.

Deze kenmerken beïnvloeden de mogelijke ernst van een verlies-van-controle-uitkomst. Een AI-systeem dat bijvoorbeeld wordt ingezet met toegang tot cloudcomputing-infrastructuur heeft kansen die relevant zijn voor autonome replicatie – zoals het vermogen om nieuwe computebronnen aan te maken of modelgewichten exfiltreren – die een klantenservicechatbot mist (‡723).

Uitrolbeslissingen worden gevormd door economische prikkels, strategische druk en de verwachting dat vroege adoptie een duurzaam voordeel oplevert (‡50). Deze dynamiek zal ook bepalen hoe en wanneer actoren AI-systemen inzetten in gevoelige omgevingen zoals kritieke infrastructuur of AI-onderzoek en -ontwikkeling zelf (‡102, ‡713). In het bijzonder kunnen AI-uitvoerders onder druk komen te staan om hun investeringen in waarborgen te verlagen – zoals het beperken van machtigingen en toegang of het alleen inzetten in omgevingen met lagere kritiek – wanneer dergelijke maatregelen kostbaar of tijdrovend zijn om te ontwikkelen (zie ‘De concurrentie vergroot de snelheid-versus-veiligheid-wisselwerking’ in §3.1. Technische en institutionele uitdagingen).

###@ Updates

Sinds de publicatie van het vorige rapport (januari 2025) zijn AI-mogelijkheden, waaronder mogelijkheden die de menselijke controle kunnen ondermijnen, verbeterd in testomgevingen. Onderzoekers hebben vooruitgang waargenomen in agentische mogelijkheden (zie §1.2. Huidige mogelijkheden), inclusief mogelijkheden die verband houden met de automatisering van AI-onderzoek en die scenario’s van verlies van controle kunnen versnellen (zie §1.3. Mogelijkheden tegen 2030). Er is ook groeiend experimenteel bewijs voor misleidende mogelijkheden. Dit omvat AI-modellen die kunnen onderscheiden tussen test- en uitzettingscontexten (‡33, ‡726, ‡741) of ‘reward hack’-tests van hun prestaties, en die leren om plannen te verhullen om dit te doen (‡430).

###@ Bewijsleemtes

Belangrijke lacunes in het bewijsmateriaal omvatten een gebrek aan gedetailleerde dreigingsmodellering en het inschatten van onzekerheid met betrekking tot de toekomstige ontwikkeling van relevante capaciteiten en geneigdheden. Op dezelfde manier blijft het moeilijk om de drempels te beoordelen waarbij AI-modellen voldoende waarschijnlijk de controle zouden ondermijnen om verplichte mitigatie te rechtvaardigen. Zelfs als drempels zouden worden overeengekomen, kunnen capaciteiten op manieren met elkaar interageren die nog niet goed worden begrepen, waardoor het moeilijk is om te beoordelen wanneer die drempels zijn overschreden. Al met al is er, hoewel het beschikbare bewijsmateriaal is toegenomen, nog steeds onvoldoende bewijsmateriaal om betrouwbaar te kunnen bepalen of en hoe de huidige AI-capaciteiten en geneigdheden zich zouden opschalen en generaliseren naar het risico op verlies van controle in de toekomst.

###@ Mitigaties

Hoewel AI-alignment in het algemeen een open wetenschappelijk probleem blijft (‡697, ‡735, ‡736), beginnen onderzoekers potentiële veelbelovende richtingen te ontwikkelen om de fundamentele oorzaken van misalignment aan te pakken. Dergelijke richtingen omvatten bijvoorbeeld het diversifiëren van de trainingsomgeving en het detecteren van alignment via anomaliedetectie-monitoring (‡737, ‡738, ‡739*). Andere onderzoekers richten zich op een beter begrip en het formaliseren van kernmechanismen zoals doel-misgeneralisatie – bijvoorbeeld hoe agenten capaciteiten behouden maar onbedoelde doelen nastreven – om betere ontwerpkeuzes voor training en evaluatie te sturen (‡742). Een andere onderzoeksrichting onderzoekt manieren om agency te ontkoppelen van voorspellende vermogens, als middel om niet-agentische AI-systemen te creëren die betrouwbaar zijn “by design” (‡743). Dergelijke systemen zouden vervolgens kunnen worden ingezet als een extra laag van toezicht wanneer ze naast minder betrouwbare waarborgen worden gebruikt tegen onbetrouwbare AI-agenten.

Onderzoekers ontwikkelen methoden om misalignatie vroeg in het ontwikkelproces te detecteren en te voorkomen. Dit werk omvat: interpretabiliteitstechnieken om interne componenten van AI-systemen te onderzoeken en zorgwekkend gedrag te identificeren (‡744, ‡745, ‡746); schaalbare supervisie (waarbij één set AI-systemen wordt gebruikt om andere AI-systemen te overseen (‡747)); en alignatiemethoden die erop gericht zijn ervoor te zorgen dat AI-systemen responsief blijven voor menselijke supervisie (‡748, ‡749).

Onderzoekers ontwikkelen ook mechanismen en interventies om mogelijk verkeerd uitgelijnde AI-systemen te beheren. Deze omvatten: het monitoren van de ‘chain of thought’ die redeneersystemen produceren op signalen van verkeerde uitlijning of schadelijke outputs (‡430, ‡435, ‡750); het ontwikkelen van veiligheidsdossiers die met hoge zekerheid willen aantonen dat modellen onwaarschijnlijk de controlemaatregelen zullen ondermijnen (‡751); en het robuuster maken van waarborgen tegen pogingen om ze te ondermijnen (‡725). Het opkomende vakgebied van ‘AI control’ blijft echter nog in de kinderschoenen (‡752, ‡753). Toekomstige uitdagingen voor evaluatiekaders omvatten de noodzaak om toekomstige AI-systemen te monitoren die bekwaamere zijn en langer kunnen opereren en in complexere omgevingen.

###@ Uitdagingen voor beleidsmakers

Beleidsmakers die werken aan verlies van controle moeten zich voorbereiden op een risico waarvan de kans, aard en timing onzeker blijven. Huidige AI-systemen vormen geen onmiddellijk risico op verlies van controle, maar beslissingen die vandaag worden genomen zullen bepalen of toekomstige systemen al dan niet leiden tot dergelijk risico. Deze beslissingen omvatten hoe de ontwikkeling van betrouwbare evaluatie- en mitigatiemethoden moet worden ondersteund en of er regels moeten komen over de toegang en machtigingen die aan AI-systemen worden verleend in verschillende omgevingen. Bij het nemen van deze beslissingen staan beleidsmakers voor moeilijke afwegingen. Als voorbeeld: het beperken van de inzet van AI-systemen in kritieke omgevingen kan hun voordelen verminderen, terwijl het toestaan van een brede inzet het risico kan vergroten als waarborgen ontoereikend blijken.

