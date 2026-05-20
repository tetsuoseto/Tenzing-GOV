##########
>white|orangered|left|14|30|hr Sectie 3.2
### 3.2. Risicobeheersingspraktijken
>white|orangered|left|24|30|hb Risicobeheerspraktijken

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Belangrijke informatie
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Risicobeheer voor algemeen inzetbare AI bestaat uit een reeks praktijken die worden gebruikt om risico's van algemeen inzetbare AI te identificeren, beoordelen en te verminderen. Dit omvat testen en evalueren op modelniveau (zoals ‘red-teaming’), organisatorische processen die ontwikkeling- en releasebeslissingen sturen, conditionele waarborgen (zoals ‘if-then’-toezeggingen) en incidentrapportage.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Verschillende AI-ontwikkelaars hebben Frontier AI Safety-frameworks opgesteld. Deze frameworks bevatten informatie over risicobeoordelingen en specificeren voorwaardelijke maatregelen, zoals toegangsbeperkingen die bedrijven van plan zijn in te voeren voor krachtigere modellen. Ze verschillen in de risico’s die ze behandelen, hoe ze drempels voor bekwaamheid definiëren, en welke acties worden geactiveerd wanneer drempels worden bereikt.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Het bewijs voor de effectiviteit in de echte wereld van AI-risicobeheerpraktijken blijft beperkt. Het ontbreken van incidentmeldingen en monitoring maakt het moeilijk om te beoordelen hoe goed de huidige praktijken risico's verminderen, of hoe consequent ze worden geïmplementeerd.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sinds de publicatie van het vorige Rapport (januari 2025) is risicomanagement gestructureerder geworden via nieuwe initiatieven op het gebied van industrie en governance. Nieuwe instrumenten zoals de Algemene Verordening AI Gedragscode voor algemeen gebruik van de EU, het Chinese kader voor AI-veiligheidsgovernance 2.0 en het G7-rapportagekader voor het Hiroshima AI-proces, samen met door bedrijven geleide initiatieven, illustreren de trend naar meer gestandaardiseerde benaderingen voor transparantie, evaluatie en incidentrapportage.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Marktmechanismen en het tempo van AI-ontwikkeling vormen extra uitdagingen. Door concurrentiedruk kunnen AI-bedrijven voor keuzes komen te staan tussen snellere productreleases en investeringen in risicoreductie-inspanningen. Veel AI-gerelateerde schade wordt bovendien afgewenteld, en de juridische aansprakelijkheid daarvoor blijft onduidelijk, terwijl governance-processen langzaam kunnen zijn in het aanpassen aan veranderingen in het AI-landschap.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Belangrijke uitdagingen voor beleidsmakers omvatten het prioriteren van de diverse risico's die door AI voor algemeen gebruik worden veroorzaakt, en het verduidelijken welke actoren binnen de hele AI-waardeketen het best gepositioneerd zijn om deze risico's te beperken. Deze uitdagingen worden verergerd door beperkte zichtbaarheid op hoe risico's in de praktijk worden geïdentificeerd, beoordeeld en beheerd, evenals door versnipperde informatie-uitwisseling tussen ontwikkelaars, inzetpartners en aanbieders van infrastructuur.
>oldlace|black||11|15|br      


AI-risicobeheer omvat een reeks praktijken die erop gericht zijn om risico's die samenhangen met AI-systemen te identificeren, te beoordelen en de waarschijnlijkheid en ernst ervan te verminderen. Deze praktijken kunnen worden toegepast door AI-ontwikkelaars, inzetters, evaluatoren en regelgevers. Voorbeelden zijn dreigingsmodellering, risicoclassificatie, red-teaming, auditing en incidentrapportage. Deze sectie beschrijft de huidige risicobeheerpraktijken, nieuwe ontwikkelingen en de resterende beperkingen.

Sinds het begin van 2025 zijn er verschillende nieuwe internationale initiatieven voor risicobeheer van general-purpose AI ontwikkeld, waaronder raamwerken voor organisatorische transparantie en risicorapportage, evenals regelgevende en governance-raamwerken.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Figuur 3.4: Vier componenten van risicobeheer
>white|black||9|11|br De vier categorieën methoden voor risicobeheer van algemene AI: risico-identificatie; risicoanalyse en -evaluatie; risicobeheersing; en risicogovernance. Deze vormen een iteratief en cyclisch proces. Risicogovernance, weergegeven in het midden, vergemakkelijkt het succes van de andere onderdelen. Bron: International AI Safety Report 2026.


Resterende uitdagingen omvatten beperkte standaardisatie, wat naleving en beoordeling bemoeilijkt, en beperkte bewijslast met betrekking tot doeltreffendheid in de praktijk. Bovendien verschillen institutionele, culturele en politieke contexten wereldwijd, wat betekent dat benaderingen voor het identificeren en beheren van risico’s, inclusief aanvaardbare risicodrempels, per regio kunnen verschillen. De bespreking in dit hoofdstuk van benaderingen voor risicobeheer is beschrijvend: het is bedoeld om actoren in het AI-ecosysteem te informeren over de huidige mondiale benaderingen voor risicobeheer. Waar beschikbaar wordt ingegaan op bewijs over de doeltreffendheid en beperkingen van deze benaderingen, maar beleidsaanbevelingen vallen buiten het bereik van dit werk.

###@ Onderdelen van risicobeheer

Risicomanagement is een iteratief proces met praktijken en methoden die de volledige cyclus van AI-ontwikkeling en -implementatie bestrijken, maar die samenhangend werken (‡969). Risicomanagement voor general-purpose AI kan rollen omvatten voor een brede variëteit aan actoren, waaronder data scientists, model engineers, auditors, domeinexperts, leidinggevenden, eindgebruikers, getroffen gemeenschappen, leveranciers van derden, beleidsmakers, overheden, organisaties voor standaarden en maatschappelijke organisaties (‡970, ‡971, ‡972). Toonaangevende risicomanagementstandaarden zijn vaak onderling uitwisselbaar, maar gebruiken verschillende terminologie om de elementen van risicomanagement te beschrijven (‡973, ‡974). Ze hebben doorgaans vier onderling verbonden componenten (Figuur 3.4): het identificeren; analyseren en evalueren; het beperken; en het besturen van risico’s (‡970, ‡973, ‡975, ‡976). De tabellen hieronder geven illustratieve voorbeelden van relevante methoden, technieken en tools. Praktijken blijven zich ontwikkelen, dus de tabellen zijn niet uitputtend en de toepasbaarheid zal per context verschillen.

###@ Risico-identificatie

Risico-identificatie is het proces van het vinden, herkennen en beschrijven van risico's. Alomvattende risico-identificatie omvat doorgaans capability-gedreven beoordelingen, die testen of modellen specifieke gevaarlijke capabilities hebben (‡977), evenals risicomodellering (‡978) en forecasting (‡715*), die worden gebruikt om bestaande en opkomende risico's te verkennen. Tafel 3.1 geeft verschillende voorbeelden van praktijken voor risico-identificatie. Risico-identificatie put ook uit afstemming met relevante experts en communities om de bredere context te begrijpen waarin risico's ontstaan (‡979, ‡980). Mechanismen zoals bug bounty-programma's kunnen dit proces ondersteunen door het identificeren van voorheen onbekende kwetsbaarheden te stimuleren (‡981) (Tafel 3.1). Een belangrijk doel van risico-identificatie is om zowel rekening te houden met goed bekende, goed begrepen risico's als met mogelijke toekomstige risico's die nog onzeker zijn of slecht gekarakteriseerd (‡982). Dit is met name belangrijk voor general-purpose AI, waarbij veel risico's nog niet volledig begrepen of observeerbaar zijn (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bug bounty-programma's
  Bug bounties of programma's voor responsible disclosure stimuleren mensen om kwetsbaarheden in AI-systemen te vinden en te melden. Verschillende ontwikkelaars hebben bug bounty-programma's geïmplementeerd (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Expertconsultatie
  Domeindeskundigen, gebruikers en getroffen gemeenschappen leveren inzichten in waarschijnlijke risico’s. Er ontstaan er richtlijnen voor participatieve en inclusieve AI (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Fishbone (Ishikawa) diagram
  Fishbone-diagrammen zijn al lang gevestigde hulpmiddelen voor analyse van hoofdoorzaken, en onderzoekers hebben voorgesteld ze te gebruiken voor gestructureerde analyse van incidenten met AI-risico’s (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Voorspellen
  Voorspellen is het proces van het voorspellen van toekomstige gebeurtenissen of trends op basis van analyse van gegevens uit het verleden en het heden. Het is gebruikt om de relatieve waarschijnlijkheid te vergelijken van bijvoorbeeld verschillende economische uitkomsten als gevolg van geavanceerde AI (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risico-taxonomie
  Risicotaxonomieën zijn een manier om risico's te categoriseren en te organiseren over meerdere dimensies. Er zijn er meerdere die risico's beschrijven vanuit algemeen inzetbare AI (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Scenario planning
  Scenario planning houdt in dat er plausibele toekomstige scenario's worden ontwikkeld en wordt geanalyseerd hoe risico's zich manifesteren. Dit is gebruikt om de risico's en gevolgen van AI-modellen te onderzoeken (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Threatmodellering
  Threat modeling is een proces voor het identificeren van bedreigingen en kwetsbaarheden voor een systeem. Talrijke AI-ontwikkelaars benadrukken het gebruik ervan om mogelijke scenario's van misbruik van AI-systemen te voorzien (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 3.1: Risico-identificatievoorbeelden in algemeen-toepasselijk AI-risicobeheer
>white|black||9|11|br Voorbeeldmethoden voor AI-risico-identificatie worden alfabetisch vermeld. De methoden die zijn inbegrepen
zijn ontworpen om risicodetectie te ondersteunen voor veel verschillende type risico's, waaronder risico's door kwaadaardig gebruik, risico's door storingen en systemische risico's. Gegeven de nog prille aard van risicobeheersing voor algemene AI, zullen niet alle methoden geschikt zijn voor elke AI-ontwikkelaar of -uitvoerder.


>white|orangered|left|14|15.5|bb Threatmodellering en risicoclassificatieschema's zijn prominente methoden voor risicodetectie

Twee prominente methoden voor het identificeren van de risico’s van general-purpose AI zijn threat modelling (International AI Safety Report 2026) en risicotaxonomieën. Meta gebruikt bijvoorbeeld threat modelling-oefeningen om mogelijke scenario’s voor misbruik van zijn AI-modellen te voorzien (‡990), en Anthropic omvat threat modelling als onderdeel van zijn ASL-3 Deployment Standard (‡991). AI-risico- en hazard-taxonomieën, die risicocategorieën en voorbeelden opsommen, kunnen evenzeer dienen als startpunt om de relevante risico’s die samenhangen met general-purpose AI in specifieke toepassingsdomeinen te conceptualiseren, te identificeren en te specificeren (‡906, ‡988, ‡992, ‡993).

###@ Risicoanalyse en evaluatie

Risicoanalyse en -evaluatie is het proces van het bepalen van het risiconiveau van een AI-model of -systeem en het vergelijken daarvan met vastgestelde criteria om de aanvaardbaarheid te beoordelen of de noodzaak voor mitigatie (‡994, ‡995, ‡996, ‡997). Het omvat praktijken zoals het meten van de modelprestaties op benchmarks (‡998) en evaluaties (‡176, ‡715), het uitvoeren van red-teaming-oefeningen (‡999*), impact assessments (‡1000) en audits (‡1001, ‡1002). Zie Tafel 3.2 voor voorbeelden van algemene AI-risicoanalyse en -evaluatie. De methoden zijn ontworpen om gelijktijdig ondersteuning te bieden bij analyse en evaluatie voor veel verschillende typen risico's.

De kernmarkten van risicoanalyse en -evaluatie zijn het uitvoeren van evaluaties van modelmogelijkheden en -kwetsbaarheden (‡1003), het benutten van robuuste risicomodellering om beslissingen over risicodrempels te onderbouwen (‡1004, ‡1005), en het begrijpen hoe AI-systemen in de praktijk worden gebruikt om downstream-maatschappelijke effecten te beoordelen (‡869, ‡904, ‡905, ‡1006). Risicoanalyse- en evaluatieprocessen worden vaak beschouwd als processen die waarschijnlijker risico’s identificeren wanneer ze onafhankelijke beoordeling bevatten (‡1001, ‡1007), putten uit expertise uit meerdere sectoren (‡1008) en diverse perspectieven omvatten vanuit meerdere domeinen en disciplines, evenals vanuit getroffen gemeenschappen (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Audits
  Audits zijn formele beoordelingen van de prestaties en effecten van AI-modellen en/ of van de naleving van normen, beleidsregels en procedures door een organisatie, uitgevoerd binnen de organisatie of door een externe partij. AI-auditing is een groeiend vakgebied en er bestaan tal van hulpmiddelen en werkwijzen voor het auditen van AI-modellen en de werkwijzen van ontwikkelaars van AI-modellen (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Benchmarks
  Benchmarks zijn gestandaardiseerde, vaak kwantitatieve tests of maatstaven die worden gebruikt om de prestaties van AI-systemen te evalueren en te vergelijken op een vaste set taken, ontworpen om reëel gebruik in de praktijk te representeren (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bowtie-methode
  De strikdas-methode is een bekende methode om te visualiseren waar besturingselementen kunnen worden toegevoegd om risicogebeurtenissen te mitigeren. De methode biedt een duidelijke differentiatie tussen proactief en reactief risicobeheer (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Delphi-methode
  De Delphi-methode is een techniek voor groepsbesluitvorming die een reeks vragenlijsten gebruikt om overeenstemming te verzamelen van een panel van experts (‡1020, ‡1021). Ze is gebruikt om mogelijke toekomstige scenario's te verkennen met geavanceerde AI (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Veldtesten
  Veldtesten evalueren de prestaties en impact van een AI-systeem in een echte, operationele omgeving. Sommige onderzoeken benadrukken dat veldtesten een aanvulling vormen op modelevaluatie voor het beoordelen van uitkomsten en gevolgen in de echte wereld (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Impactbeoordeling
  Impact assessments beoordelen de mogelijke effecten van een technologie of project. Dit kan het kwantificeren, aggregeren en prioriteren van effecten omvatten. De EU AI Act vereist bijvoorbeeld dat ontwikkelaars van AI-systemen met een hoog risico Fundamentele Rechten Impact Assessments uitvoeren (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modelevaluatie
  Modelevaluaties omvatten processen en tests om de prestaties van een AI-model op een specifieke taak te beoordelen en te meten. Er zijn talloze AI-evaluaties om verschillende mogelijkheden en risico’s te beoordelen, waaronder op het gebied van veiligheid, beveiliging en maatschappelijke impact (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Probabilistische risicobeoordeling
  Probabilistische risicoanalyse is een methodologie voor het evalueren van risico's die samenhangen met complexe systemen of processen en die onzekerheid meeneemt. Het is aangepast voor geavanceerde AI-systemen (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Red-teaming
  Red-teaming is een oefening waarbij een groep mensen of geautomatiseerde systemen zich voordoet als een tegenstander en de technologische systemen van een organisatie aanvalt om kwetsbaarheden te identificeren. Talrijke AI-bedrijven hebben interne praktijken voor red-teaming van AI-systemen (‡458, ‡1028). Red-teaming kan ook worden uitgevoerd door actoren buiten bedrijven. Deze teams krijgen te maken met uitdagingen zoals beperkte toegang, maar kunnen ook distincte inzichten naar voren brengen (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risicomatrices
  Risicomatrices zijn een visueel hulpmiddel om risico's te helpen prioriteren op basis van hun waarschijnlijkheid van optreden en mogelijke impact (‡1027). Sommige AI-ontwikkelaars nemen basisrisicomatrices op in hun Frontier AI Safety Frameworks (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risicodrempels/ risiconiveaus
  Risicodrempels of -niveaus zijn kwantitatieve of kwalitatieve grenzen die onderscheid maken tussen aanvaardbare en onaanvaardbare risico's en die specifieke risicobeheersmaatregelen activeren wanneer ze worden overschreden. Voor general-purpose AI worden ze bepaald door een combinatie van mogelijkheden, impact, compute, bereik en andere factoren (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risicotolerantie
  Risicotolerantie verwijst naar het risiconiveau dat een organisatie bereid is te accepteren. In AI worden risicotoleranties vaak impliciet ingesteld via bedrijfsbeleid en -praktijken, terwijl sommige regelgevingsregimes expliciet niet-acceptabele risico's definiëren en er juridische consequenties aan verbinden (‡1032). Sommige bedrijven beschrijven hun risicotolerantie in termen van het marginale risico van een nieuw model; dat wil zeggen, de mate waarin een model contrafactueel het risico verhoogt boven het risico dat al wordt veroorzaakt door bestaande modellen of andere technologieën (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Veiligheidsdossiers
  Een safety case is een gestructureerd betoog, ondersteund door bewijs, dat aantoont dat een systeem in een specifieke context acceptabel veilig is om te gebruiken. Recente literatuur (‡1037, ‡1038, ‡1039) heeft safety cases onderzocht voor frontier AI-systemen en sommige Frontier AI Safety Frameworks verwijzen ernaar (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Systeembestandsanalyse
  Systeemveiligheidsanalyse benadrukt afhankelijkheden tussen componenten en het systeem waarvan ze deel uitmaken, om te kunnen voorzien hoe systeemniveau-gevaren kunnen ontstaan uit falen van componenten of processen, of uit interacties tussen subsystemen, menselijke factoren en omgevingsomstandigheden. Benaderingen die voor AI-systemen in de literatuur worden toegepast omvatten systeembenaderingsmatige procesanalyse (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 3.2: Risicoanalyse/evaluatie in algemeen gebruik AI-risicobeheer
>white|black||9|11|br Voorbeeldmethoden voor AI-risicoanalyse/-evaluatie, alfabetisch gerangschikt. Gezien de prille aard van risicobeheer voor algemene AI, zullen niet alle methoden geschikt zijn voor elke AI-ontwikkelaar of -deployers.


>white|orangered|left|14|15.5|bb Veelgebruikte risicoanalysehulpmiddelen omvatten benchmarks en modelbeoordelingen

Benchmarks en modelevaluaties zijn gestandaardiseerde tests om de prestaties van general-purpose AI-systemen op specifieke taken te beoordelen. Onderzoekers hebben een breed scala aan benchmarks en evaluaties ontwikkeld, waaronder sets met uitdagende meerkeuzevragen, software engineering-problemen en op het werk gerichte taken in gesimuleerde kantooromgevingen (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Evaluaties van schadelijke capaciteiten (‡715) worden gebruikt om te beoordelen of een general-purpose AI-model of -systeem over met name gevaarlijke kennis of vaardigheden beschikt, zoals het vermogen om te helpen bij cyberaanvallen (zie §2.1.3. Cyberaanvallen).

Hoogst ingrijpende beslissingen door bedrijven en overheden over modelreleases steunen deels op deze evaluaties (‡1050, ‡1051, ‡1052). De kwaliteit en reikwijdte van benchmarks lopen echter sterk uiteen (‡998, ‡1003), en het kan lastig zijn om hun geldigheid te beoordelen vanwege talrijke tekortkomingen in de benchmarkingpraktijken (‡902, ‡909, ‡1003, ‡1053*). Zo kunnen benchmarks ‘verzadigd’ raken – wanneer de scores van veel modellen de hoogste score benaderen – waardoor ze niet langer in sterke mate onderscheid maken tussen modellen. Modellen identificeren ook steeds vaker bepaalde taken als evaluaties en vertonen dan ander gedrag dan ze zouden doen bij vergelijkbare taken in uitrolcontexten door ‘situationele bewustwording’ (zie §2.2.2. Verlies van controle). Tot slot hebben benchmarks en evaluaties goed gedocumenteerde beperkingen: met name nemen ze de risico’s die samenhangen met het gebruik van algemene AI in nieuwe domeinen en voor nieuwe taken niet goed mee, omdat de testomstandigheden in uiteenlopende mate afwijken van het daadwerkelijke gebruik (‡913) (zie §1.2. Huidige mogelijkheden en §3.1. Technische en institutionele uitdagingen).

>white|orangered|left|14|15.5|bb Red-teaming maakt meer domeinspecifieke beoordelingen van risico mogelijk

Een andere veelgebruikte methode om risico’s te beoordelen is red-teaming. Een ‘red team’ is een groep beoordelaars die is belast met het zoeken naar kwetsbaarheden, beperkingen of mogelijkheden voor misbruik. Red-teaming kan domeinspecifiek zijn en worden uitgevoerd door domeinexperts, of open-ended zijn om nieuwe risicofactoren te verkennen. Een red team zou bijvoorbeeld ‘jailbreaking’-aanvallen kunnen verkennen die de veiligheidsbeperkingen van het model omzeilen (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). In tegenstelling tot benchmarks is een belangrijk voordeel van red-teaming dat red teams hun evaluaties kunnen aanpassen aan het specifieke systeem dat wordt getest. Red teams kunnen bijvoorbeeld aangepaste invoerontwerpen maken om het slechtste gedrag, kansen voor kwaadwillig gebruik en onverwachte storingen te identificeren. Het kan echter speciale toegang tot modellen vereisen en kan ertoe leiden dat belangrijke klassen van risico’s niet worden blootgelegd (‡999, ‡1028).

Belangrijk is dat het ontbreken van geïdentificeerde risico’s niet betekent dat die risico’s laag zijn: eerder werk laat zien dat bugs vaak aan detectie ontsnappen, met name wanneer red teams beperkte toegang of middelen hebben (‡1060). Onderzoek heeft bovendien de vraag opgeworpen of red-teaming betrouwbare en reproduceerbare resultaten kan opleveren (‡1061). De samenstelling van het red team en de instructies die aan red-teamers worden gegeven (‡1062), het aantal aanvalsronden (‡1063) en de toegang van het model tot hulpmiddelen (‡1064, ‡1065) kunnen de uitkomsten aanzienlijk beïnvloeden, inclusief het risicogebied dat wordt afgedekt. Volledige richtlijnen voor red-teaming proberen enkele van deze uitdagingen aan te pakken (‡1066).

###@ Risicobeperking

Risicobeperking is het proces van het prioriteren, evalueren en implementeren van beheersmaatregelen en tegenmaatregelen om geïdentificeerde risico's te verkleinen. Voorbeelden zijn toegangscontrole (‡991), continue monitoring (‡986) en if-then-toezeggingen (‡700). Het beperken van risico brengt een belangrijke vraag met zich mee: wat is het aanvaardbare risiconiveau? Recente kaders en bedrijfsbeleid zijn begonnen om formele criteria voor ‘risicoacceptatie’ vast te leggen (‡965, ‡1040). Het instellen van passende drempels blijft echter uitdagend, met name voor risico's met brede maatschappelijke gevolgen (‡986, ‡1067). Er bestaat momenteel geen vastgesteld mechanisme om beslissingen over risicoacceptatie die door ontwikkelaars vóór de release zijn genomen, te valideren (‡1005).

De risicobeperkende methoden die hieronder in Tafel 3.3 worden beschreven, zijn aanpasbaar en kunnen een reeks risico's beperken, waaronder sommige onverwachte risico's. De tabel bevat geen technische risicobeperkende methoden zoals adversarial training, contentfilters en chain-of-thought monitoring. Deze worden behandeld in §3.3 Technische waarborgen en monitoring, evenals in de 'Mitigations'-paragrafen voor elk risico in §2. Risico's door het hele Rapport heen.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Aanvaardbaar-gebruiksbeleid
  Een acceptabel-gebruikbeleid is een set regels en richtlijnen voor het verantwoordelijke, ethische en juridische gebruik van AI-modellen. Het is gebruikelijk dat AI-ontwikkelaars acceptabel-gebruikbeleid, evenals verboden-gebruikbeleid, publiceren bij nieuwe modelreleases (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Toegangscontrole / gebruikersverificatie
  Toegangscontroles omvatten het gebruik van beleidsregels en regels om de toegang tot AI-modellen, gegevens en systemen te beperken op basis van gebruikersrollen, attributen en andere voorwaarden, om ongeautoriseerd gebruik, manipulatie of datalekken te voorkomen. AI-bedrijven schakelen accounts die worden aangetroffen terwijl ze zich bezighouden met criminele activiteiten (‡486) vaak uit en nemen user vetting en Know-Your-Customer-screenings op om te waarborgen dat modellen alleen worden gebruikt door vertrouwde actoren (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Gedrags-/model-specificatie
  Een AI-gedragspecificatie is een document dat definieert hoe een AI-model zich moet gedragen in verschillende situaties. Het dient als blauwdruk voor AI-alignment en veiligheid en stuurt modelontwikkeling, training, evaluatie en output. Verschillende AI-bedrijven gebruiken modelspecificatiedocumenten en maken ten minste delen ervan publiek (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Continue monitoring
  Continue monitoring is het voortdurende, geautomatiseerde proces van het observeren, analyseren en controleren van AI-systemen in gebruik, waarbij hun prestaties worden gevolgd en hun gedrag wordt begrensd om betrouwbaarheid, doeltreffendheid en veiligheid te waarborgen. Er zijn tal van hulpmiddelen beschikbaar voor continue monitoring (‡1073*) evenals technieken om te ondersteunen
AI-observeerbaarheid (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb verdediging-in-diepte
  Defence-in-depth is het idee dat meerdere onafhankelijke en overlappende verdedigingslagen kunnen worden geïmplementeerd, zodat als één ervan faalt, de andere nog steeds effectief zullen zijn (‡1075, ‡1076). Meerdere Frontier AI Safety Frameworks verwijzen ernaar (bijv. (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ecossysteemmonitoring
  Dit is het proces van het monitoren van het bredere AI-ecosysteem, inclusief het volgen van rekenkracht en hardware, modelherkomst, gegevensherkomst en gebruikspatronen. De onderzoeksliteratuur bespreekt dergelijke monitoring in relatie tot risico's van general-purpose AI (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb If-then-toezeggingen
  Als-dan-toezeggingen zijn een set technische en organisatorische protocollen en toezeggingen om risico's te beheren naarmate AI-modellen capabeler worden. Verscheidene AI-ontwikkelaars gebruiken dit soort toezeggingen als onderdeel van hun Frontier AI Safety Frameworks (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rode lijnen of verboden
  Rode lijnen zijn specifieke grenzen die worden uitgedrukt als capaciteiten, impact of typen gebruik. Het concept komt voor in openbare verklaringen en initiatieven, evenals in regelgevende verboden (‡1079, ‡1080, ‡1081). De literatuur signaleert ook beperkingen van benaderingen met rode lijnen, waaronder uitdagingen rond consensus en handhaafbaarheid.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Release- en implementatiestrategieën
  Vrijgave- en implementatiestrategieën voor algemene AI kunnen onder meer het gebruik van gefaseerde vrijgaven of API-toegang omvatten, zodat er meer mitigatieopties beschikbaar zijn in het geval van misbruik of onverwachte schade (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 3.3: Risicobeperking in risicomanagement voor algemene AI-toepassingen
>white|black||9|11|br Voorbeeldmethoden voor AI-risicobeperking vermeld in alfabetische volgorde. De opgenomen methoden zijn ontworpen om gelijktijdig ondersteuning te bieden voor risicobeperking voor veel verschillende typen risico's, waaronder risico's door kwaadwillend gebruik, risico's door storingen en systeemrisico's. Gezien het prille karakter van algemeen toepasbaar AI-risicobeheer zullen niet alle methoden geschikt zijn voor elke AI-ontwikkelaar of -deployer.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Figuur 3.5: Een ‘Zwitserse kaas-diagram’ dat de defence-in-depth benadering illustreert
>white|black||9|11|br Meerdere lagen van verdedigingsmechanismen kunnen tekortkomingen in afzonderlijke lagen compenseren. Huidige risicobeheertechnieken voor AI hebben tekortkomingen, maar het stapelen ervan kan veel sterkere bescherming bieden tegen risico's. Bron: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Defensie-in-diepte- en release-strategieën zijn belangrijke mitigatiehulpmiddelen

Een ‘defense-in-depth’-model kan algemeen- purpose AI-risicobeheer ondersteunen. In deze context verwijst ‘defense-in-depth’ naar een combinatie van technische, organisatorische en maatschappelijke maatregelen die worden toegepast in verschillende stadia van ontwikkeling en inzet (Figuur 3.5). Dit betekent het creëren van lagen van onafhankelijke waarborgen, zodat als één laag faalt, andere lagen nog steeds schade kunnen voorkomen. Een vaak aangehaald voorbeeld van een defense-in-depth-model is de reeks preventieve maatregelen die worden ingezet om infectieziekten te voorkomen. Vaccins, mondmaskers en handenwassen, onder andere maatregelen, kunnen het infectierisico aanzienlijk verlagen in combinatie, ook al is geen van deze methoden op zichzelf 100% effectief (‡1083*). Voor general-purpose AI omvat defense-in-depth controles die niet op het AI-model zelf staan, maar op het bredere ecosysteem. Dit omvat (bijvoorbeeld) controles op de materialen die nodig zijn om een biologische aanval uit te voeren, zoals reagentia (‡1084, ‡1085). Defense-in-depth-maatregelen richten zich echter vooral op risico’s die verband houden met ongevallen, storingen en kwaadaardig gebruik, en kunnen een minder grote rol spelen bij het beheersen van systeemrisico’s (zie §3.5. Maatschappelijke veerkracht opbouwen).

Een release- en plaatsingsstrategie van een bedrijf is een belangrijk onderdeel van risicobeperking. Beslissingen over hoe modellen beschikbaar worden gesteld aan gebruikers kunnen de risicoblootstelling aanzienlijk beïnvloeden (‡1082). Verschillende release- en plaatsingsopties omvatten gefaseerde release aan beperkte gebruikersgroepen, toegang via gecontroleerde online services (zoals API's), en het gebruik van licentieovereenkomsten en acceptabel-gebruikbeleid waarmee juridisch bepaalde schadelijke toepassingen worden verboden (‡176, ‡1086, ‡1087). §3.4. Open-weight-modellen bespreekt in meer detail hoe het vrijgeven van modelgewichten risico's beïnvloedt.

###@ Risicobeheer

Risicobestuur is het proces waarbij evaluaties, beslissingen en acties van risicomanagement worden gekoppeld aan de strategie en doelstellingen van een organisatie of andere entiteit (‡1088, ‡1089). Tafel 3.4 geeft een overzicht van gangbare risicobestuursmethoden. Zoals weergegeven in Figuur 3.4 kan risicobestuur worden begrepen als de kern van risicomanagement, omdat het de effectieve werking van andere componenten van risicomanagement mogelijk maakt. Het biedt verantwoording, transparantie en duidelijkheid die geïnformeerde beslissingen over risicomanagement ondersteunen. Risicobestuur kan praktijken omvatten zoals incidentrapportage (‡1090), het toewijzen van risicoverantwoordelijkheden (‡965) en bescherming van klokkenluiders (‡1091). In bredere zin kan risicobestuur begeleiding, kaders, wetgeving, regelgeving, nationale en internationale normen omvatten, evenals trainings- en educatieve initiatieven. Een belangrijk doel van risicobestuur is het vaststellen van organisatorische beleidsregels en mechanismen die verduidelijken hoe risicomanagementverantwoordelijkheden binnen een organisatie of andere entiteit worden verdeeld, om passend toezicht en verantwoording te ondersteunen (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Documentatie
  Documentatiepraktijken helpen bij het bijhouden van belangrijke informatie over AI-systemen, zoals trainingsdata, ontwerpkeuzes, beoogd gebruik, beperkingen en risico's. ‘Modelkaarten’ en ‘systeemaanslagen’, die informatie geven over hoe een AI-model of -systeem is getraind en geëvalueerd, zijn voorbeelden van prominente best practices voor AI-documentatie (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Incidentrapportage
  Incidentrapportage is het proces van systematisch vastleggen en delen van gevallen waarin het ontwikkelen of inzetten van AI directe of indirecte schade heeft veroorzaakt. Er zijn verschillende platforms die incidentrapportage voor AI faciliteren (‡1096, ‡1097) en kaders om meer effectieve incidentrapportage voor AI te faciliteren (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risicobeheersingskaders
  Risicobeheersingskaders zijn organisatorische plannen om lacunes in de risicobeheersing te verminderen, verschillende risicobeheersactiviteiten te coördineren en controles en tegenwichten in te voeren. Kaders die specifiek zijn voor algemeen inzetbare AI (‡986, ‡1098) verwijzen vaak naar de andere maatregelen die in deze sectie worden genoemd.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risicoregister
  Een risicoregister is een verzameling van verschillende risico's, hun prioritering, verantwoordelijken en mitigatieplannen. Deze komen relatief vaak voor in veel sectoren, waaronder cybersecurity (‡1099), en worden soms gebruikt om te voldoen aan vereisten voor regelgevende naleving.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risicoverantwoordelijkheidsverdeling
  De verdeling van rollen en verantwoordelijkheden voor risicomanagement binnen een organisatie kan de interne controle op besluitvorming structureren (‡1002, ‡1093). Dergelijke regelingen worden weerspiegeld in sommige governance-frameworks, waaronder de EU’s General-Purpose AI Code of Practice (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Transparantierapporten
  Transparantierapporten beschrijven de risicobeheerspraktijken van een AI-bedrijf door publiekelijk bepaalde informatie te openbaar te maken of door documentatie te delen met brancheorganisaties of overheidsinstanties. Zo dienen talrijke AI-bedrijven transparantierapporten over het Hiroshima AI Process (HAIP) in (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Klokkenluidersbescherming
  Omdat veel AI-ontwikkeling plaatsvindt achter gesloten deuren, bevatten sommige governance-frameworks bescherming voor klokkenluiders om openbaarmaking van mogelijke risico's aan autoriteiten mogelijk te maken (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 3.4: Risicogovernance in algemeen-doel AI-risicobeheer
>white|black||9|11|br Voorbeeldmethoden voor AI-risicobesturing zijn alfabetisch opgesomd. De opgenomen methoden zijn ontworpen om gelijktijdig ondersteuning te bieden voor risicobesturing voor veel verschillende risicotypen, waaronder risico's door kwaadwillend gebruik, risico's door storingen en systeemrisico's. Gezien de prille aard van risicobeheer voor general-purpose AI zullen niet alle methoden geschikt zijn voor elke AI-ontwikkelaar of -inzetter.


>white|orangered|left|14|15.5|bb Documentatie en transparantie zijn onderdelen van risicobeheer.

Documentatie- en institutionele transparantiemechanismen, samen met informatie-uitwisselingspraktijken, vergemakkelijken externe controle en ondersteunen inspanningen om risico’s te beheersen die samenhangen met general-purpose AI (‡1101, ‡1102). Het is gebruikelijk geworden om de resultaten van pre- deployment tests te publiceren in een ‘model card’ of ‘system card’, samen met basisdetails over het model of het systeem, waaronder hoe het is getraind en welke mogelijke beperkingen het heeft (‡1094, ‡1095). Sommige ontwikkelaars publiceren ook transparantierapporten met daarin details over hun risicobeheerspraktijken in bredere zin (‡1103). Andere elementen van documentatie en transparantie omvatten monitoring en incidentrapportage (‡176, ‡1083*, ‡1103) en informatie-uitwisseling, die kunnen worden gefaciliteerd door derde partijen zoals de Frontier Model Forum. Sommige regelgevingskaders, zoals de EU AI Act of California’s Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53) (‡1081, ‡1104), verplichten in sommige gevallen informatie-uitwisseling over risico’s van general-purpose AI.

>white|orangered|left|14|15.5|bb Leiderschapscommitment en incentives vormen risicobeheerspraktijken

Organisatiecultuur, leiderschapsstructuur en prikkels beïnvloeden risicobeheersingsinspanningen op verschillende manieren (‡1105). Leiderschapsbetrokkenheid en prikkelstructuren zijn vaak relevant voor de manier waarop risicobeheerbeleid in de praktijk functioneert. Sommige ontwikkelaars hebben interne besluitvormingspanels die beraadslagen over hoe nieuwe AI-systemen veilig en verantwoord kunnen worden ontworpen, ontwikkeld en beoordeeld. Toezichts- en adviescommissies, trusts of AI-ethische raden kunnen ook dienen als mechanismen voor richtlijnen voor risicobeheer en voor organisatorisch toezicht (‡1092*, ‡1106, ‡1107, ‡1108). Onderzoekers hebben betoogd dat uitdagingen met vrijwillige zelfregulering betekenen dat externe auditing, verificatie en standaardisatie kunnen helpen om algemeen inzetbaar AI-risicobeheer te versterken (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Organisatorisch risicomanagement, transparantie en risicorapporteringskaders

Verschillende nieuwe initiatieven richten zich op risicobeheersprocessen, documentatie en transparantie. In de huidige vorm functioneert de EU Code of Practice voor AI voor algemeen doel als een vrijwillig kader om transparantie-, auteursrecht- en veiligheids- en beveiligingspraktijken te sturen ter ondersteuning van de naleving van de bepalingen van de EU AI Act voor AI voor algemeen doel (‡965). Per december 2025 hebben meer dan twee dozijn bedrijven† zich aangesloten. Het G7 Hiroshima AI Process (HAIP) Reporting Framework (‡1100) is het eerste internationale kader voor vrijwillige openbare rapportage van organisatorische risicobeheerspraktijken voor geavanceerde AI-systemen. Ten minste 20 ontwikkelaars hebben openbare transparantieverslagen gepubliceerd met betrekking tot risicodetectie, evaluatiemetrieken, mitigatiestrategieën en databeveiligingsprocessen.

AI-ontwikkelaars hebben vrijwillige transparantieverbintenissen aangenomen. In China zijn in december 2024 (‡1113) toezeggingen van 17 Chinese AI-bedrijven, gecoördineerd door het AI Industry Alliance of China, vrijgegeven en in 2025 bijgewerkt (‡1114). Tijdens de AI Seoul Summit in mei 2024 in Zuid-Korea hebben 16 AI-ontwikkelaars uit meerdere landen vrijwillige toezeggingen ondertekend om Frontier AI Safety Frameworks te publiceren voor hun meest capabele modellen en systemen, en om risicobeheerspraktijken toe te passen in alle stadia van modelontwikkeling en -deployments (‡1052).

    Opmerking † -- Ondertekenaars per december 2025 omvatten: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing, en WRITER.

>white|orangered|left|14|15.5|bb Frontier AI Safety Frameworks zijn een prominente organisatorische aanpak geworden voor het beheer van AI-risico’s

Sinds 2023 hebben verschillende vooraanstaande AI-ontwikkelaars vrijwillig documenten gepubliceerd waarin wordt beschreven hoe zij van plan zijn om ernstige risico's voortkomend uit hun meest geavanceerde systemen te identificeren en erop te reageren. Deze Frontier AI Safety Frameworks beschrijven hoe een AI-ontwikkelaar van plan is om zijn meest geavanceerde AI-modellen en -systemen te evalueren, te monitoren en te beheersen vóór en tijdens de inzet. Deze frameworks vertonen veel overeenkomsten, maar verschillen op belangrijke punten (‡1115, ‡1116). De meeste richten zich op risico's die samenhangen met chemische, biologische, radiologische en nucleaire (CBRN) dreigingen, geavanceerde cybermogelijkheden en geavanceerd autonoom gedrag (‡1115, ‡1117). Een minderheid van de frameworks behandelt aanvullende risicodomeinen, zoals grootschalige onrechtmatige discriminatie en seksuele uitbuiting van kinderen.

Verschillende ontwikkelaars hebben hun frameworks in 2025 geüpdatet en nieuwe secties toegevoegd over schadelijke manipulatie, het misalignement-risico en autonome replicatie en adaptatie (‡1078, ‡1118). Hoewel veel frameworks vergelijkbare benaderingen voor risicobeheer beschrijven – waaronder threat modelling, red-teaming en evaluaties van gevaarlijke mogelijkheden – verschillen ze in hun definities van risiconiveaus en drempels, de frequentie van evaluaties, buffers tussen evaluaties en drempels, en de algehele volledigheid van hun mitigatie-inzet (bijvoorbeeld of ze het verwijderen van modelgewichten omvatten versus alleen het pauzeren van ontwikkeling) (‡1115, ‡1119). Zie Tafel 3.5 voor meer informatie.

>white|orangered|left|14|15.5|bb Veel acties in Frontier AI Safety Frameworks zijn gebaseerd op if-then-toezeggingen

Een belangrijk onderdeel van Frontier AI Safety Frameworks zijn “if-then”-toezeggingen. Dit zijn voorwaardelijke protocollen die specifieke reacties activeren wanneer AI-modellen en -systemen vooraf gedefinieerde capaciteitsdrempels bereiken (‡1120). Een voorbeeld van een if-then-toezegging is dat als wordt vastgesteld dat een model de mogelijkheid heeft om betekenisvol beginners te helpen bij het creëren en inzetten van CBRN-wapens, dan de ontwikkelaar uitgebreidere beveiligingsmaatregelen, inzetcontrolemaatregelen en real-time monitoring zal implementeren (‡991*).

In 2025 kondigden verschillende AI-ontwikkelaars aan dat nieuwe modellen vroegewaarschuwingsalarmen activeerden of dat ze niet konden uitsluiten dat verdere evaluatie zou aantonen dat modellen drempels voor capaciteiten hebben overschreden. Dit leidde ertoe dat ze als voorzorgsmaatregel verhoogde waarborgen toepasten (‡7, ‡33, ‡1121*). Frontier AI Safety Frameworks vereisen doorgaans een initiële evaluatie van capaciteiten vóór risicobeperking, alsmede een analyse van resterend risico of een safety case, vaak geïnformeerd door red-teaming, na de mitigatie. Zie Tafel 3.5 voor gedetailleerde informatie.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Voorbereidingskader 2 (‡1078*)
  Gedekte risico's:
1. Biologische en chemische capaciteiten
2. Cybersecurity-mogelijkheden
3. AI-zelfverbeteringsmogelijkheden
  Risiconiveaus of equivalent en bijbehorende waarborgen:
- Hoog: Kan bestaande paden versterken tot ernstige schade (vereist beveiligingscontroles en -maatregelen)
- Kritiek: Kan ongekende nieuwe routes naar ernstige schade introduceren (stop verdere ontwikkeling totdat gespecificeerde waarborgen en standaarden voor beveiligings- en controlemaatregelen een Kritiek niveau bereiken)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Verantwoord Schaalbeleid 2.2 (‡991*)
  Gedekte risico's:
1. CBRN-wapens
2. Autonome AI-onderzoek en -ontwikkeling (AI R&D)
3. Cyberoperaties (onder beoordeling)
  Risiconiveaus of equivalent en bijbehorende waarborgen:
  AI-veiligheidsniveaus (ASL)
- ASL-1: Geen significant catastrofaal risico
- ASL-2: Vroege tekenen van gevaarlijke mogelijkheden (Modellen moeten voldoen aan de ASL-2 implementatie- en veiligheidsstandaarden)
- ASL-3: Aanzienlijk verhoogd risico op catastrofaal misbruik (Modellen moeten voldoen aan de ASL-3-implementatie- en/of beveiligingsnormen)
- ASL-4+: Toekomstige classificaties (nog niet gedefinieerd)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Frontier Safety Framework 3.0 (‡1040*)
  Gedekte risico's:
1. Misbruik
    a. CBRN
    b. Cyber
    c. Schadelijke manipulatie
2. Machine learning R&D
3. Wanverlijning/ instrumentele redenering
  Risicogroepen of equivalent en bijbehorende waarborgen:
  Kritieke capaciteitsniveaus
    Vermogensniveaus waarbij, bij afwezigheid van mitigerende maatregelen (veiligheidsdossiers voor inzet en beveiligingsmitigaties afgestemd op RAND-beveiligingsniveaus 2, 3 of 4 (‡1122)), AI-modellen of -systemen een verhoogd risico op ernstige schade kunnen vormen. De vermogensniveaus omvatten ‘evaluaties voor vroege waarschuwing’, met specifieke ‘waarschuwingsdrempels’
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Frontier AI-framework 1.1 (‡990*)
  Gedekte risico's:
1. Cyberbeveiliging
2. Chemische en biologische risico's
  Risicotiercategorieën of gelijkwaardig en bijbehorende waarborgen:
  Riscodrempelniveaus
- Matig (release met passende beveiligingsmaatregelen en mitigaties)
- igh (niet vrijgeven)
- Kritiek (ontwikkeling stopzetten)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Frontier Model Safety Framework (‡1123*)
  Gedekte risico's:
1. Verspreiding van CBRN-wapens
2. Offensieve cyberoperaties
3. Geautomatiseerd AI-onderzoek en -ontwikkeling
  Risiconiveaus of equivalenten en bijbehorende waarborgen:
  Kritieke capaciteitsdrempels
    Modelmogelijkheden die, bij misbruik, aanzienlijke schade aan het publiek kunnen veroorzaken. (Als de drempels worden gehaald of overschreden, wordt het model niet publiek ingezet zonder passende risicobeperkende maatregelen)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Frontier Governance Framework (‡1124*)
  Gedekte risico's:
1. CBRN-wapens
2. Offensieve cyberoperaties
3. Geavanceerde autonomie (inclusief AI-onderzoek en -ontwikkeling)
  Risicotier-indelingen of equivalent en bijbehorende waarborgen:
  Risiconiveaus
- Laag of Middel (Toezetting toegestaan in overeenstemming met de vereisten van het Responsible AI Program)
- Hoog of Kritiek (verdere beoordeling en mitigerende maatregelen
vereist)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Beoordeling van het risico van Frontier AI (‡1029*)
  Gedekte risico's:
1. Cybermisdaad
2. CBRN
3. Overreding en manipulatie
4. Onrechtmatige discriminatie op schaal
  Risicocategorieën of equivalent en bijbehorende beveiligingsmaatregelen:
  Risicodrempels – modelrisico (MR)-scores
- MR1 of MR2 (Evaluatieresultaten worden gedocumenteerd door engineering teams)
- MR3 (Risicobeperkende maatregelen en evaluatieresultaten worden gedocumenteerd door engineeringteams en periodiek beoordeeld)
- MR4 (Er moet een gedetailleerde risicoanalyse worden uitgevoerd en goedkeuring van de leidinggevende van de business unit is vereist)
- MR5 (Er moet een gedetailleerde risicoanalyse worden uitgevoerd en goedgekeurd door een onafhankelijke commissie, bv. NVIDIA’s AI-ethiekcommissie)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Secure AI Frontier Model Framework (‡1125*)
  Gedekte risico's:
1. Kwaadwillend gebruik (bijv. malware, seksuele uitbuiting van kinderen)
2. Schade bij normaal, niet-malafide gebruik, bv. outputs die resulteren in een illegale discriminerende uitkomst of in het genereren van onveilige code
  Risicocategorieën of gelijkwaardig en bijbehorende waarborgen:
  Waarschijnlijkheid en Ernst van Schade in de Context
- Laag
- Gemiddeld
- Hoog
- Zeer hoog
    (Risicobeperkende maatregelen en beveiligingscontroles zijn aanwezig voor alle systemen en processen; aanvullende maatregelen moeten worden aangepast aan het AI-systeem en het use case waarin een model wordt ingezet)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: AGI-gereedheidsbeleid (‡1127*)
  Gedekte risico's:
1. Cybermisdaad
2. Geautomatiseerd AI-onderzoek en -ontwikkeling
3. Autonome replicatie en adaptatie
4. Biologische wapenassistentie
  Risicocategorieën of equivalenten en bijbehorende waarborgen:
  Kritieke capaciteitsdrempels
    Kwantitatieve drempels op capaciteitsbenchmarks (als ze worden overschreden, voer gevaarlijke capaciteits-evaluaties uit, informatiebeveiligingsmaatregelen en inzetbeperkingen, of stop de ontwikkeling)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: AGI-Gereedheidsbeleid (‡1127*)
  Gedekte risico's:
1. Cybermisdaad
2. Geautomatiseerd AI-onderzoek en -ontwikkeling
3. Autonome replicatie en adaptatie
4. Biologische wapenassistentie
  Risiconiveaus of equivalent en bijbehorende waarborgen:
  Kritieke capaciteitsdrempels
    Kwantitatieve drempels op bekwaamheidsbenchmarks (indien overschreden, voer gevaarlijke evaluaties van bekwaamheid uit, maatregelen voor informatiebeveiliging en inzet-mitigaties, of stop de ontwikkeling)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: AI Safety Framework (‡1128*)
  Gedekte risico's:
1. Verlies van controle
2. Misbruik (bijv. biochemische wapenproductie
  Risiconiveaus of equivalente niveaus en de bijbehorende waarborgen:
  Risiconiveaus
- Laag risico (AI-systemen implementeren, maar daarna monitoring uitvoeren om risico's te beheersen)
- Risico vastgesteld (Ofwel alleen open AI-systemen beschikbaar stellen voor geautoriseerde gebruikers om risico’s te beperken, ofwel de uitrol uitstellen totdat aanvullende veiligheidsmaatregelen zijn genomen, afhankelijk van het gebruiksscenario)
- Hoog risico (AI-systemen niet inzetten)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Frontier AI Safety Framework (‡1129*)
  Gedekte risico's:
1. Biologische bedreigingen
2. Offensieve cybersecurity
3. Autonome werking en geavanceerde manipulatie
  Risicotiers of equivalenten en bijbehorende waarborgen:
  Risiconiveaus
- Niveau 1 (Basiswaarborgen voor minimale risico's en de mogelijkheid van een open source-publicatie)
- Niveau 2 (Realtime monitoring, prompt filtering, gedragsafwijkingsdetectie, toegangscontroles, red-teaming en adversariële simulaties)
- Niveau 3 (Geavanceerde waarborgen, inclusief red-teaming, gefaseerde uitrol, adversarial testing, encryptie, besturing met multi-party-toegang en zero-trust-architectuur)
- Niveau 4 (Maximum veiligheidsprotocollen voor modellen met een hoog risico en maximale beveiligingsmaatregelen)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 3.5: Frontier AI Safety-frameworks
>white|black||9|11|br De eerste set Frontier AI Safety Frameworks die is uitgebracht door een subset van de AI-ontwikkelaars die de Frontier AI Safety Commitments hebben ondertekend. De frameworks behandelen vergelijkbare risico's (met geringe variaties) en hanteren verschillende risicocategorieën en benaderingen voor risicobeheer.


>white|orangered|left|14|15.5|bb De effectiviteit van Frontier AI Safety-frameworks is onzeker

Frontier AI Safety Frameworks kunnen dienen als risicobeheertools onder specifieke omstandigheden en voor bepaalde risicocategorieën die een geloofwaardige route naar schade hebben (‡1117). Tegelijk bespreken verschillende analyses vragen over hun helderheid en reikwijdte (‡111, ‡986) en over de robuustheid van AI-capabiliteiten en risicodrempels (‡1031, ‡1130). Bestaande frameworks richten zich doorgaans op een subset van risicodomeinen. Als gevolg krijgen sommige prominente risico's, zoals onrechtmatige surveillance (‡1131, ‡1132) en intieme beeldvorming zonder toestemming (‡287), minder nadruk. In tegenstelling tot benaderingen voor risicobeheer uit andere sectoren, zoals de luchtvaart of kernenergie (‡1133*), gebruiken Frontier AI Safety Frameworks doorgaans geen expliciete kwantitatieve risicodrempels (‡1134).

Externe beoordelingen van de naleving door ontwikkelaars van hun Frontier AI Safety Frameworks tot nu toe blijven beperkt, deels omdat de meeste frameworks recent zijn, openbare informatie schaars is en er geen gestandaardiseerde externe audits bestaan. Hun doeltreffendheid zal ook worden bepaald door hoe goed – en in welke mate – toezeggingen in de praktijk worden geïmplementeerd. Op zichzelf kunnen deze frameworks mogelijk geen effectief risicobeheer waarborgen, aangezien hun praktische impact afhangt van hoe goed – en in welke mate – ze worden geïmplementeerd. Tot op heden sluiten ze niet volledig aan op internationale risicobeheernormen (‡1135). Een studie naar eerdere vrijwillige toezeggingen vond een ongelijkmatige nakoming over maatregelen, wat erop wijst dat naleving van vrijwillige toezeggingen waarschijnlijk zal verschillen tussen bedrijven en domeinen (‡1109).

Samen genomen vertegenwoordigen Frontier AI Safety Frameworks de meest gedetailleerde vorm van vrijwillig organisatorisch risicobeheer die momenteel wordt gebruikt, maar ze verschillen aanzienlijk in reikwijdte, drempels en afdwingbaarheid.

###@ Regelgevende en governance-initiatieven

>white|orangered|left|14|15.5|bb Verschillende jurisdicties hebben wetten ingevoerd met vereisten op het gebied van transparantie

Verschillende vroege regelgevende benaderingen introduceren juridische vereisten die bedoeld zijn om standaardisatie en transparantie in risicobeheer te vergroten. De EU AI Act, die in 2024 in werking is getreden, stelt vereisten vast met betrekking tot transparantie, auteursrecht en veiligheid voor general-purpose AI-modellen. In 2025 werd de EU General-Purpose AI Code of Practice gepubliceerd om naleving van deze verplichtingen te ondersteunen door richtsnoeren te bieden over modeldocumentatie en auteursrecht, evenals – voor de meest geavanceerde modellen – risicobeheerspraktijken zoals evaluaties, risicobeoordeling en -mitigatie, informatiebeveiliging en het melden van ernstige incidenten (‡965).

Andere voorbeelden van nieuwe regelgevingseisen omvatten de Kaderwet van Zuid-Korea inzake de ontwikkeling van kunstmatige intelligentie en de totstandbrenging van vertrouwen, die eisen invoert voor ‘hoog-risico’ AI-systemen in kritieke sectoren (‡1136), en Californië’s SB 53, die transparantie-eisen vastlegt over veiligheidskaders en incidentrapportage (‡1104). Gezien hoe recent deze eisen zijn vastgesteld, is het te vroeg om in detail te beoordelen hoe ze van invloed zullen zijn op risicobeheerpraktijken of op daadwerkelijke risicobeoordelingsuitkomsten.

>white|orangered|left|14|15.5|bb Brede governance-initiatieven bieden vrijwillige richtlijnen

Verschillende regionale en interregionale bestuurskaders formuleren nu gedeelde verwachtingen voor het beheren van risico’s van algemeen inzetbare AI door niet-bindende richtsnoeren te bieden voor beleidsmakers en organisaties. Het Chinese AI Safety Governance Framework 2.0, gepubliceerd in 2025, geeft gestructureerde richtsnoeren voor risicoclassificatie en tegenmaatregelen gedurende het proces van AI-ontwikkeling en -inzet (‡1137). ASEAN-lidstaten publiceerden de ‘ASEAN Expanded Guide on AI Governance and Ethics (Generative AI)’, die richtsnoeren biedt voor governance en ethiek van algemeen inzetbare AI en bedoeld is om een grotere beleidsafstemming tussen ASEAN-lidstaten te ondersteunen (‡1138). Daarnaast schetsen door experts geleide initiatieven zoals het Singapore Consensus, ontwikkeld door AI-wetenschappers uit meerdere landen, onderzoeksprioriteiten voor AI-veiligheid voor algemeen inzetbare AI op het gebied van risicobeoordeling, ontwikkeling en beheersing (‡690).

###@ Updates

Sinds de publicatie van het vorige rapport (januari 2025) is het risicobeheerslandschap voor general-purpose AI geëvolueerd, met de publicatie van nieuwe middelen zoals de EU’s General-Purpose AI Code of Practice, het G7 HAIP Reporting Framework, China’s nationale AI Safety Governance Framework 2.0 en diverse Frontier AI Safety Frameworks van AI-ontwikkelaars. Deze initiatieven beschrijven aanpakken en praktijken die door AI-ontwikkelaars worden gebruikt om de risico’s te beheersen die samenhangen met general-purpose AI-systemen (‡1115). Er is aanzienlijke variatie tussen de Frontier AI Safety Frameworks en tussen de HAIP-transparantierapporten (‡1103), wat weerspiegelt dat organisatorische praktijken, risicoprioritering en het vroege stadium van het ecosysteem voor risicobeheer van general-purpose AI uiteenlopen. Een betrouwbaar ecosysteem waarin verschillende AI-acteurs gedurende de volledige levenscyclus complementaire praktijken voor risicobeheer bijdragen, kan bijdragen aan effectief risicobeheer (‡690).

###@ Bewijsleemtes

Er is onvoldoende bewijs voor: hoe de ernst, prevalentie en tijdshorizon van opkomende risico's kunnen worden gemeten; in welke mate deze risico's kunnen worden beperkt in praktijksituaties; en hoe beperking van de adoptie ervan effectief kan worden aangemoedigd of afgedwongen bij uiteenlopende actoren. Er is meer onderzoek nodig om te begrijpen hoe prevalent verschillende risico's zijn en in hoeverre zij verschillen tussen regio's wereldwijd, met name voor regio's zoals Azië, Afrika en Latijns-Amerika die zich snel digitaliseren. Aangezien AI-modellen steeds meer handelingsbevoegdheid en gezag krijgen en de stand van de wetenschap rond risico's van general-purpose AI vordert, zullen ook risicobeheersaanpakken moeten evolueren (‡639, ‡1139).

Bepaalde risicobeperkende maatregelen worden steeds populairder (‡690, ‡956), maar er is meer onderzoek nodig om te begrijpen hoe robuuste risicobeperkende maatregelen en waarborgen in de praktijk zijn voor verschillende gemeenschappen en AI-actoren (ook voor kleine en middelgrote ondernemingen). Meer toegang tot data over real-life inzet en gebruik van modellen is relevant voor dergelijke beoordelingen. Bovendien lopen de inspanningen op het gebied van risicobeheer momenteel sterk uiteen tussen toonaangevende AI-bedrijven. Er is aangevoerd dat de prikkels van ontwikkelaars niet goed aansluiten op een grondige risicobeoordeling en risicobeheersing (‡934). Er is nog steeds een kenniskloof over in welke mate verschillende vrijwillige toezeggingen worden nagekomen, welke obstakels bedrijven tegenkomen bij het volledig nakomen van toezeggingen, en hoe zij Frontier AI Safety Frameworks integreren in bredere praktijken voor AI-risicobeheer.

###@ Uitdagingen voor beleidsmakers

Belangrijkste uitdagingen zijn onder meer bepalen hoe de diverse risico’s die worden veroorzaakt door algemene-purpose AI moeten worden geprioriteerd, verduidelijken welke actoren het best gepositioneerd zijn om deze risico’s te beperken, en begrijpen welke prikkels en beperkingen hun handelen vormgeven. Bewijs wijst erop dat beleidsmakers momenteel beperkte toegang hebben tot informatie over hoe AI-ontwikkelaars en -deployers de opkomende risico’s testen, evalueren en monitoren, en over de effectiviteit van verschillende mitigatiepraktijken (‡1140). Onderzoekers en beleidsmakers hebben besproken dat transparantie-inspanningen en meer systematische incidentrapportage mogelijke manieren zijn om risicoprioritering te informeren, vertrouwen te bevorderen en verantwoordelijke ontwikkeling te stimuleren (‡957). In de praktijk omvat risicobeheer meerdere actoren in de AI-waardeketen – zoals dataproviders en cloudproviders, modelontwikkelaars en model-hostingplatforms – die elk andere mogelijkheden hebben om verschillende risico’s te beoordelen en te beheersen (‡1141). Beperkte informatie-uitwisseling tussen deze actoren maakt het moeilijk om te bepalen welke risico’s het waarschijnlijkst of het meest impactvol zijn, met name wanneer de downstream-maatschappelijke effecten in aanmerking worden genomen.

