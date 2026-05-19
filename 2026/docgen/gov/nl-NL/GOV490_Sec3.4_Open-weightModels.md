##########
>white|orangered|left|14|30|hr Sectie 3.4
### 3.4. Modellen met open gewichten
>white|orangered|left|24|30|hb Open-weight-modellen

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Belangrijke informatie
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Het niveau van toegang dat AI-bedrijven bieden tot de ‘gewichten’ van hun modellen beïnvloedt de risico's die deze modellen vormen. Gewichten zijn de wiskundige parameters waarmee AI-modellen invoer kunnen verwerken en uitvoer kunnen genereren. Voor elk gegeven model kunnen bedrijven ervoor kiezen om de gewichten volledig privé te houden, aan sommige gebruikers beperkte toegang te geven, of iedereen toe te staan ze volledig te downloaden. Modellen waarvan de gewichten openbaar beschikbaar zijn, worden ‘open-weight-modellen’ genoemd.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Open-gewichtmodellen faciliteren onderzoek en innovatie, maar hun beveiligingen worden eenvoudiger verwijderd. Over de hele wereld kunnen verschillende actoren – vooral actoren met minder middelen – open-gewichtmodellen gebruiken voor onderzoeks- en commerciële doeleinden. In vergelijking met gesloten-gewichtmodellen zijn open-gewichtmodellen echter eenvoudiger aan te passen om mogelijk schadelijk gedrag te vertonen, en is het complexer.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Open-weight model releases zijn onomkeerbaar. Zodra ze zijn uitgebracht, kunnen modelgewichten niet worden teruggeroepen. Dit maakt het moeilijker om mogelijke schadelijke effecten te beperken die kunnen voortvloeien uit de release van een model met gevaarlijke mogelijkheden.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sinds de publicatie van het vorige rapport (januari 2025) hebben grote open-weight releases de capaciteitskloof met toonaangevende gesloten modellen verkleind. Chinese ontwikkelaars DeepSeek en Alibaba brachten respectievelijk hun R1- en Qwen-modellen uit, die qua prestaties vergelijkbaar waren met toonaangevende gesloten modellen, terwijl OpenAI zijn eerste open-weight modellen uitbracht sinds 2019. De mogelijkheden van toonaangevende gesloten modellen worden nu geschat op minder dan 1 jaar voorsprong op toonaangevende open-weight modellen op prominente AI-benchmarks.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Een belangrijke beleidsuitdaging is om toegang te krijgen tot de voordelen die open-weight modellen bieden, terwijl hun kenmerkende risico's worden beheerd. Een aanpak is om open-weight modellen te beoordelen in termen van hun ‘marginaal risico’: in welke mate hun vrijgave op tegenfeitelijke wijze het maatschappelijke risico verhoogt bovenop het risico dat al wordt veroorzaakt door bestaande modellen of andere technologieën. Dit is echter in de praktijk complex. Kleine stijgingen in het marginaal risico in de tijd kunnen zich ook opstapelen tot aanzienlijke stijgingen van het totale risico.
>oldlace|black||11|15|br      


Open-weight modellen, waarvan de parameters publiek beschikbaar zijn om te downloaden, hebben duidelijke implicaties voor veel van de uitdagingen die in de voorgaande secties zijn besproken. De ‘gewichten’ van een AI-model bevatten de cruciale informatie waarmee het nuttige antwoorden kan genereren voor gebruikers. Zodra deze gewichten zijn vrijgegeven, kunnen ze niet meer worden teruggeroepen: iedereen kan ze downloaden, bestuderen, aanpassen, delen en gebruiken op eigen computers of cloud-accounts. Wanneer gewichten openlijk beschikbaar zijn, kunnen anderen het model gemakkelijker uitbreiden en aanpassen, inspelend op diverse behoeften en innovatie stimuleren (‡1317). Echter, via hetzelfde mechanisme kunnen gebruikers met kwade bedoelingen ook gemakkelijker beveiligingen verwijderen en open-weight modellen aanpassen voor schadelijke use-cases (‡1122, ‡1160). Dit heeft de vraag doen rijzen of sommige open-weight modellen aan speciale eisen moeten worden gebonden (bijv. strengere tests vóór vrijgave) of, omgekeerd, speciale vrijstellingen moeten krijgen (bijv. van vereisten voor regelgevingsrapportage) (‡1033).

###@ Achtergrond bij open-weight-modellen

>white|orangered||14|15.5|bb Open-weight modellen kunnen wel, maar hoeven niet per se 'open source' modellen te zijn

Hoewel ze vaak ‘open source’ worden genoemd, kunnen de meeste publiek uitgebrachte modellen nauwkeuriger worden omschreven als ‘open-weight’. Dit komt doordat ontwikkelaars weliswaar de modelgewichten beschikbaar stellen, maar niet de bijbehorende trainingscode of datasets vrijgeven. Bovendien wordt open source-software gewoonlijk gekenmerkt door licenties die minimale vereisten stellen aan downstream-actoren die de software gebruiken of wijzigen (‡1318). Zo hebben Meta’s Llama-modellen beperkende licentievoorwaarden en bevatten ze alleen inferentiecode, niet trainingscode, en worden ze daarom doorgaans niet als open source beschouwd (‡1319, ‡1320). Opties voor modelreleases bestaan op een continuüm van volledig gesloten tot volledig open source, met verschillende afwegingen tussen risico en voordeel bij elk punt (‡1086*, ‡1320, ‡1321). Tafel 3.9 beschrijft deze opties.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Volledig gesloten
  Gebruikers kunnen helemaal niet rechtstreeks met het model interageren
  Voorbeelden: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Gehostete toegang
  Gebruikers kunnen alleen communiceren via een specifieke applicatie of interface, zoals een mobiele chatbotapplicatie
  Voorbeelden: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb API-toegang tot het model
  Gebruikers kunnen via code verzoeken naar het model sturen, waardoor gebruik in externe applicaties mogelijk is
  Voorbeelden: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb API-toegang tot fine-tuning
  Gebruikers kunnen het model bijstellen voor hun specifieke behoeften
  Voorbeelden: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Open-gewichten: gewichten beschikbaar om te downloaden
  Gebruikers kunnen het model downloaden en op hun eigen computers uitvoeren
  Voorbeelden: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Gewichten, gegevens en code beschikbaar om te downloaden, met gebruiksbeperkingen
  Gebruikers kunnen het model en de inferentie- en trainingscode downloaden en uitvoeren, maar er gelden bepaalde licentiebeperkingen voor het gebruik ervan.
  Voorbeelden: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Volledig open: gewichten, gegevens en code beschikbaar om te downloaden zonder gebruiksbeperkingen
  Gebruikers hebben volledige vrijheid om het model, volledige code en gegevens te downloaden, te gebruiken en aan te passen
  Voorbeelden: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 3.9: Opties voor modeldeling variërend van volledig gesloten tot volledig open
>white|black||9|11|br Een illustratieve selectie van modeldelingopties, variërend van volledig gesloten modellen (modellen zijn privé en alleen voor eigen, bedrijfseigen gebruik) tot volledig open en open-source modellen (modelgewichten, data en code zijn vrij en publiek beschikbaar zonder beperkingen voor gebruik, aanpassing en deling). Modellen die in de eerste vier categorieën vallen, worden vaak ‘gesloten’ genoemd. Deze sectie richt zich op de drie onderste rijen. Bron: aangepast van Bommasani, 2024 (‡1317).


###@ Voordelen en risico's

>white|orangered|left|14|15.5|bb Open-weight modellen kunnen gemakkelijker worden aangepast en geëvalueerd

Open-weight-modellen bieden aanzienlijke voordelen voor onderzoek, innovatie en toegang. Zoals besproken in §1.1. Wat is general-purpose AI?, is het trainen van general-purpose AI-modellen uiterst kostbaar – toonaangevende modellen kosten honderden miljoenen dollars om te ontwikkelen. Het openlijk vrijgeven van modelgewichten stelt actoren met minder middelen in staat om bestaande systemen te repliceren, te bestuderen en erop voort te bouwen. Zonder dergelijke toegang lopen gemeenschappen in regio’s met weinig middelen het risico uitgesloten te worden van de voordelen van AI, waardoor open weights van cruciaal belang zijn om deelname door de wereldwijde meerderheid aan AI-ontwikkeling mogelijk te maken (‡1322). Downstream-ontwikkelaars kunnen modellen bijscholen voor uiteenlopende toepassingen; bijvoorbeeld door ze aan te passen voor onderbediende minderheidstalen of door de prestaties te optimaliseren voor specifieke taken, zoals het opstellen van juridische documenten of het maken van medische notities (‡1323, ‡1324*). Op die manier kunnen open-weight-modellen meer mensen en gemeenschappen in staat stellen AI te gebruiken en ervan te profiteren dan anders mogelijk zou zijn (‡1325). In het geval van modellen die niet capabel genoeg zijn om gevaarlijk te zijn, kunnen deze voordelen opwegen tegen het extra risico van het openlijk vrijgeven van gewichten, al hangt dit af van de risicotolerantie van relevante besluitvormers.

Open-weight release vergroot ook de groep ontwikkelaars en onderzoekers die in staat zijn het model te bestuderen, de mogelijkheden ervan te evalueren, te testen op kwetsbaarheden en iteratief verbeteringen door te voeren (‡1326, ‡1327). Hierdoor is de kans groter dat zowel nuttige toepassingen als schadelijke gebreken worden geïdentificeerd, hoewel dit niet gegarandeerd is (‡1328, ‡1329). Gebruikers kunnen open-weight-modellen ook op hun eigen apparaten draaien, waardoor ze de controle over gevoelige gegevens kunnen behouden en voorkomen dat deze naar servers van derden worden verzonden.

Er zijn extra voordelen wanneer ontwikkelaars informatie delen, zoals trainingsdata, code, evaluatiehulpmiddelen en documentatie, evenals modelgewichten (‡1320, ‡1330, ‡1331, ‡1332*). Met meer informatie kunnen downstream-ontwikkelaars en andere onderzoekers open-weight-modellen beter begrijpen en aanpassen aan nieuwe toepassingen.

>white|orangered|left|14|15.5|bb Beveiligingen van modellen met open weights zijn eenvoudiger te verwijderen, waardoor mogelijk kwaadwillend gebruik wordt gefaciliteerd

Open-weight-modellen vormen ook extra risico's, omdat hun beveiligingen eenvoudiger te verwijderen zijn. Hoewel zowel open-weight- als gesloten modellen beveiligingen kunnen hebben om schadelijke verzoeken van gebruikers te weigeren, zijn die beveiligingen bij open-weight-modellen veel eenvoudiger te verwijderen. Kwaadwillende actoren kunnen een model fijn-afstellen om de prestaties voor schadelijke toepassingen te optimaliseren, onderdelen van de code verwijderen die bedoeld zijn om schadelijke toepassingen te voorkomen, of eerdere veiligheids-fijn-afstellingen ongedaan maken (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Als gevolg kunnen open model-gewichten de misbruikrisico's die in §2.1 worden besproken verergeren. Risico's door kwaadwillig gebruik doordat meer actoren zonder toezicht bestaande mogelijkheden kunnen aanwenden en uitbreiden voor kwaadaardige doeleinden (‡1122, ‡1315). Hoewel veel gebruikers niet de vaardigheid of motivatie hebben om beveiligingen op open-weight-modellen te verwijderen, vormen zeer gemotiveerde kwaadwillende actoren een zorg. Bovendien kunnen kwaadwillende actoren open-weight-modellen ook gebruiken om kwetsbaarheden in vergelijkbare gesloten modellen te identificeren (‡1055*). Dergelijke tekortkomingen zijn moeilijker te vinden door uitsluitend gesloten modellen uit te voeren, vanwege de grotere mate van controle en monitoringmaatregelen die aanbieders van gesloten modellen kunnen implementeren.

>white|orangered|left|14|15.5|bb Het delen van modelgewichten is onomkeerbaar

Zodra modelgewichten beschikbaar zijn voor publieke download, is er geen manier om een volledige rollback van alle bestaande exemplaren uit te voeren. Internethostingplatforms zoals GitHub en Hugging Face kunnen modellen van hun platforms verwijderen, waardoor het voor sommige actoren lastig wordt om downloadbare kopieën te vinden en waardoor een aanzienlijke drempel ontstaat voor veel incidentele kwaadaardige gebruikers (‡1339). Gemotiveerde actoren kunnen echter nog steeds kopieën verkrijgen als het model is gedownload en elders opnieuw is gehost of lokaal is opgeslagen. Bovendien nemen ontwikkelaars stroomafwaarts die open-weight-modellen in hun systemen integreren ook alle gebreken over, zoals kwetsbaarheden voor adversarial attacks (‡1055) of modelmogelijkheden om controlesystemen te omzeilen (zie §2.2.2. Loss of control) (‡1315). In tegenstelling tot gesloten modellen waarbij hosts universeel fixes kunnen uitrollen, kunnen ontwikkelaars van open-weight-modellen niet garanderen dat updates door gebruikers worden geadopteerd.

###@ Updates

Sinds de publicatie van het laatste rapport (januari 2025) is de capaciteitskloof tussen toonaangevende open-weight-modellen en gesloten modellen kleiner geworden. Chinese ontwikkelaars zijn in het bijzonder belangrijke aanbieders van open-weight-modellen geworden. In januari 2025 bracht DeepSeek zijn R1-model uit, dat op een aantal benchmarks (‡1340) prestaties bereikte die vergelijkbaar zijn met OpenAI’s o1. Alibaba’s Qwen-modellen hebben eveneens aan momentum gewonnen en bezetten vanaf augustus 2025 de toppositie voor een open-weight-model op Chatbot Arena, een veelgebruikte prestatiebenchmark (‡1341, ‡1342*). In augustus 2025 bracht OpenAI zijn eerste open-weight-modellen uit sinds de release van GPT-2 in 2019: gpt-oss-120b en gpt-oss-20b. Meta is doorgegaan met het uitbrengen van Llama-modellen met open weights. De capaciteiten van de toonaangevende gesloten modellen worden nu geschat op minder dan een jaar achterstand ten opzichte van de toonaangevende open modellen op prominente AI-benchmarks (Figuur 3.10).

###@ Bewijsleemtes

Een belangrijke lacune in het bewijs betreft de effectiviteit in de echte wereld van technische oplossingen om misbruik van open-weight modellen te voorkomen. Onderzoekers hebben verschillende benaderingen voorgesteld om modellen bestand te maken tegen manipulatie. Hierbij gaat het om nieuwe trainingstechnieken die bedoeld zijn om modellen resistent te maken tegen schadelijke aanpassingen (‡1276), het filteren van schadelijke inhoud uit trainingsdata (‡55) en verdedigingen tegen jailbreaks (‡675, ‡676). Deze technieken worden nu toegepast in releases in de echte wereld door grote ontwikkelaars. OpenAI heeft bijvoorbeeld enkele van deze technieken ingezet in hun gpt-oss-modellen en gerapporteerd dat adversarieel fijn-afgestemde versies geen hoge capaciteitsdrempels haalden (‡1344*). Onderzoek heeft echter aangetoond dat kwaadwillenden beveiligingen kunnen uitschakelen door modellen opnieuw te trainen op schadelijke voorbeelden (‡1345, ‡1346). Bovendien blijft het nog steeds lastig om de robuustheid van beveiligingen betrouwbaar te evalueren, waardoor hun effectiviteit tegen aanvallen in de echte wereld onzeker is (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Figuur 3.10: Vermogenskloof tussen de leidende open-weight en gesloten AI-modellen
>white|black||9|11|br Epoch Capabilities Index (ECI)-scores van top-presterende open-weight (donkerblauw) en gesloten (lichtblauw) modellen in de tijd. De ECI combineert scores van 39 benchmarks tot één algemene capaciteitsschaal. De beste open-weight-modellen lopen ongeveer een jaar achter op gesloten modellen. Bron: Epoch AI, 2025 (‡1343).


###@ Mitigaties

Technische mitigaties voor risico’s van open-weight modellen werken gedurende het volledige AI-ontwikkel- en uitzettingsproces (‡1141, ‡1195, ‡1347). Bijvoorbeeld, wanneer modellen worden ontwikkeld, kunnen ontwikkelaars en downstream-adapters gevoelig materiaal uit de trainingsdata filteren om schadelijke mogelijkheden te minimaliseren. Het verwijderen van schadelijke voorbeelden uit de trainingsdata van een model kan aanvallende fine-tuning 10 keer effectiever voorkomen dan verdedigingsmaatregelen die na de training worden toegevoegd, hoewel dit ook invloed kan hebben op nuttige mogelijkheden (‡55). AI-toepassingsproviders kunnen ook incidentrapportage- en responsmechanismen implementeren (‡1348).

Bovendien kunnen hostingplatforms zoals HuggingFace en GitHub platformvoorwaarden opstellen om modellen die zijn aangepast voor schadelijke doeleinden te verwijderen (‡1141, ‡1324). Modelontwikkelaars kunnen auditors volledige toegang geven voorafgaand aan de release, of kiezen voor een ‘gefaseerde’ release-strategie – waarbij modellen worden vrijgegeven aan steeds grotere groepen (‡1086). Dit kan helpen bij het identificeren van mogelijke storingen of kwetsbaarheden voordat een model breed beschikbaar wordt (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Opmerking 3.1: Beveiliging van modelgewichten
>oldlace|black|left|13|15|hb  Opmerking 3.1: Beveiliging van modelgewichten
>oldlace|black||11|15|br      
>oldlace|black||11|15|br De risico's die in dit onderdeel worden besproken, gaan ervan uit dat modelgewichten opzettelijk worden vrijgegeven. Gesloten modelgewichten kunnen echter ook toegankelijk worden via diefstal of uitlek. Gesloten modellen kosten honderden miljoenen dollars om te ontwikkelen (§1.1. Wat is algemene-purpose AI?) en zijn gemiddeld gezien vaardiger dan modellen met open gewichten (‡1343). Hierdoor zijn ze aantrekkelijke doelen voor actoren variërend van amateur-hackers tot natiestaten die proberen toonaangevende AI-modellen te verkrijgen.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Gestolen gesloten modelgewichten zouden risico's met zich meebrengen die vergelijkbaar zijn met die welke hierboven zijn beschreven voor open-weight modellen, maar mogelijk zonder een van de mitigerende maatregelen. Kwaadwillende actoren zouden beveiligingen kunnen verwijderen uit de meest capabele modellen. In tegenstelling tot legitieme ontwikkelaars zouden dergelijke actoren niet te maken krijgen met de reputatie-, juridische- of commerciële beperkingen die momenteel frontier AI-bedrijven stimuleren om hun modellen veilig in te zetten.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br De huidige beveiligingsniveaus verschillen per sector en kunnen onvoldoende zijn tegen geavanceerde aanvallers. Sommige ontwikkelaars committeren zich aan het beveiligen van modelgewichten tegen cybercriminele syndicaten en insiderbedreigingen (‡582), terwijl anderen geen openbare beveiligingscommittering hebben gedaan (‡1109, ‡1349). Onderzoek wijst erop dat AI-datacentra mogelijk niet bestand zijn tegen aanvallen van de meest geavanceerde en goed gefinancierde actoren (‡582, ‡1350, ‡1351). Met ingang van december 2025 zijn er geen bevestigde, publiek gedocumenteerde incidenten van diefstal van modelgewichten. Andere inbreuken op de beveiliging bij toonaangevende AI-bedrijven zijn echter wel gemeld, waaronder een infiltratie van Microsofts e-mailsystemen (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Het dichten van deze beveiligingslacunes zou aanzienlijke investeringen vereisen in hardware, software, personeel en beveiliging van de faciliteiten. Sommige beveiligingsverbeteringen kunnen relatief snel worden doorgevoerd met gecoördineerde inzet (‡1122). Andere kritieke maatregelen, zoals het beveiligen van toeleveringsketens voor hardware en faciliteiten, zouden echter waarschijnlijk jaren in beslag nemen (‡1122). Private bedrijven beschikken mogelijk ook niet over de middelen of informatie om op zichzelf voldoende bescherming te ontwikkelen. Zo hebben AI-ontwikkelaars bijvoorbeeld niet de toegang tot geclassificeerde dreigingsinformatie die overheden wel hebben (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Uitdagingen voor beleidsmakers

Een belangrijke uitdaging voor beleidsmakers is het veiligstellen van de voordelen van het delen van open-weight modellen, zonder het risico aanzienlijk te vergroten. Om catastrofale schade te voorkomen, mogen ontwikkelaars van open-weight modellen geen modellen vrijgeven zonder de risico’s te evalueren, zowel met behulp van de gevestigde beoordelingsmethoden die worden gebruikt voor gesloten modellen als met aanvullend testen, aangezien kwaadwillenden modellen kunnen fine-tunen en veiligheidsbeschermingen kunnen verwijderen. In de praktijk kan dit lastig zijn omdat capaciteitsontwikkelingen onvoorspelbaar kunnen zijn, open-weight releases onomkeerbaar zijn en er evaluatie-inspanningen nodig zijn om te voorspellen wanneer een release een aanzienlijk potentieel risico op schade zou vormen. Een benadering is om het ‘marginale risico’ van open releases te evalueren: de mate waarin de release, in tegenfeitelijke zin, het maatschappelijke risico verhoogt bovenop datgene dat al wordt veroorzaakt door bestaande modellen of andere technologieën (‡556, ‡1033, ‡1354, ‡1355) (zie §3.2. Risicobeheerspraktijken). Het inschatten van hoe een systeem het risico stroomafwaarts zal verhogen of verlagen nadat het is ingezet, is echter complex en context-afhankelijk. Incrementen in risicotoename bij opeenvolgende releases kunnen na verloop van tijd uitgroeien tot aanzienlijke stijgingen van het totale risico, zelfs wanneer het marginale risico dat aan elke release is verbonden acceptabel lijkt (‡1356, ‡1357). De dual-use aard van AI-capaciteiten maakt governance verder ingewikkeld: kenmerken die nuttige toepassingen in de geneeskunde of in onderzoek mogelijk maken, kunnen worden omgebogen voor schade, en zodra weights openbaar zijn, kan het lastig zijn om legitiem van kwaadaardig gebruik te onderscheiden. Ook is niet duidelijk wie verantwoordelijk moet worden gehouden wanneer open-weight modellen worden aangepast voor schadelijke doeleinden.

