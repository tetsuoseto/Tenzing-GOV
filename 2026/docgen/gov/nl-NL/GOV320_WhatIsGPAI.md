###@ Wat zijn algemene-purpose AI-systemen?

General-purpose AI-systemen zijn softwareprogramma’s die patronen leren uit grote hoeveelheden data, waardoor ze een verscheidenheid aan taken kunnen uitvoeren in plaats van gespecialiseerd te zijn voor één specifieke functie of één specifiek domein (zie Tafel 1.1). Om deze systemen te maken, voeren AI-ontwikkelaars een proces in meerdere fasen uit dat aanzienlijke rekenkracht vereist, grote datasets en gespecialiseerde expertise (zie Tafel 1.2). Rekenkracht (vaak afgekort tot ‘compute’) is nodig zowel om AI-systemen te ontwikkelen als om ze in te zetten, en omvat gespecialiseerde computerchips evenals de software en infrastructuur die nodig zijn om ze te laten draaien.† Omdat ze worden getraind op grote, diverse datasets, kunnen general-purpose AI-systemen veel verschillende taken uitvoeren, zoals het samenvatten van tekst, het genereren van afbeeldingen, of het schrijven van computercode. In deze sectie wordt uitgelegd hoe general-purpose AI-systemen worden gemaakt, wat ‘reasoning’-modellen zijn, en hoe beleidsbeslissingen de ontwikkeling van general-purpose AI-systemen vormgeven.

    Opmerking † -- De term ‘compute’ kan ook verwijzen naar ofwel een meting van het aantal berekeningen dat een processor kan uitvoeren (meestal gemeten in floating-point bewerkingen per seconde) of specifiek naar de hardware (zoals grafische processors) die die berekeningen uitvoert.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Taalsystemen
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Command A (‡3*)
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
###@ beeldgeneratoren
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Videogeneratoren
- Cosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Ik zie 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotica- en navigatiesystemen
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Voorspellers van diverse klassen van biomoleculaire structuren
- AlphaFold 3 (‡27)
- Versterken (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ AI-agenten
- AlphaEvolve (‡31*)
- ChatGPT-agent (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- De AI Scientist-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 1.1: Algemeen inzetbare AI-typen
>white|black||9|11|br Er zijn verschillende typen general-purpose AI. In dit Rapport worden modellen die structurele informatie kunnen voorspellen voor diverse klassen van moleculen beschouwd als ‘general-purpose’ AI, omdat ze kunnen worden aangepast voor uiteenlopende taken. Modellen die bijvoorbeeld zijn getraind om eiwitstructuur te voorspellen, zijn toepasbaar voor een verscheidenheid aan andere taken, zoals het voorspellen van eiwitinteracties, het voorspellen van bindingsplaatsen voor kleine moleculen, en het voorspellen en ontwerpen van cyclische peptiden (‡40).


>white|orangered|left|13|15|bb Deep learning vormt de basis voor AI voor algemeen doel

Onderzoekers bouwen algemeen toepasbare AI-modellen met behulp van een proces dat ‘deep learning’ wordt genoemd, waarbij modellen worden getraind om te leren van voorbeelden (‡41). In tegenstelling tot software engineering leren deep learning-modellen taken uit data te vervullen in plaats van te steunen op met de hand geschreven instructies. Door grote hoeveelheden data te verwerken, zoals afbeeldingen, tekst of audio, ontdekken deze modellen manieren om die data voor te stellen, waardoor interne representaties van patronen ontstaan (zoals vormen, woordassociaties of geluidsstructuren) die het model helpen verbanden te herkennen en uitvoer te genereren die aansluit op het trainingsdoel. Vervolgens gebruiken ze deze geleerde interne representaties als abstracte kenmerken om nieuwe, vergelijkbare data te analyseren en uitvoer te genereren in dezelfde stijl. Een algemeen toepasbaar AI-model dat bijvoorbeeld voldoende voorbeelden van 19e-eeuwse romantische Engelse poëzie is getraind, kan nieuwe gedichten in die stijl herkennen en nieuw materiaal produceren in een vergelijkbare stijl.

Op een meer granular niveau werkt deep learning door gegevens te verwerken via lagen van onderling verbonden informatieverwerkingsknopen. Deze knopen worden vaak ‘neuronen’ genoemd omdat ze losjes zijn geïnspireerd door neuronen in biologische hersenen (‘neural networks’) (Figuur 1.1) (‡42). Naarmate informatie stroomt van de ene laag neuronen naar de volgende, transformeert het model de gegevens stapsgewijs tot meer abstracte representaties als groepen aangeleerde kenmerken – patronen die het model automatisch in de gegevens heeft ontdekt, in plaats van handmatig gecodeerde patronen. In een beeldverwerkingsmodel zouden de eerste lagen bijvoorbeeld eenvoudige kenmerken kunnen leren detecteren, zoals randen of basisvormen, terwijl diepere lagen deze kenmerken combineren om complexere patronen te herkennen, zoals gezichten of objecten.

De kenmerken op alle lagen worden ontdekt via het optimalisatieproces dat de trainingsprocedure definieert. Tijdens de training, wanneer het model fouten maakt, passen deep learning-algoritmen de sterkte van verschillende verbindingen tussen neuronen aan om de prestaties van het model te verbeteren. De sterkte van elke verbinding tussen knopen wordt vaak een ‘gewicht’ genoemd. Deze gelaagde aanpak geeft deep learning zijn naam.

Deep learning heeft zich zeer effectief bewezen in het mogelijk maken voor AI-systemen om taken uit te voeren die voorheen als moeilijk werden beschouwd voor traditionele handmatig geprogrammeerde computationele systemen en andere eerdere symbolische of op regels gebaseerde AI-methoden. De meeste state-of-the-art algemene AI-modellen zijn nu gebaseerd op een specifieke neurale netwerkarchitectuur die bekendstaat als de ‘transformer’ (‡43, ‡44). Transformers gebruiken een ‘attention’-mechanisme (‡45) dat het model helpt om zich bij het verwerken van informatie te richten op de meest relevante delen van de invoergegevens, zoals het bepalen welke woorden in een zin het belangrijkst zijn voor het begrijpen van de betekenis ervan. Deze specifieke manier van modellen bouwen heeft geleid tot aanzienlijke verbeteringen in vertaling (‡43), verwerking van natuurlijke taal (‡46), beeldherkenning (‡47) en spraakkherkenning (‡48, ‡49), wat uiteindelijk heeft geleid tot de ontwikkeling van de meest geavanceerde modellen van vandaag.

![fig1.1](images/fig1.1_neural_network.png)

##### Figuur 1.1: Een illustratieve weergave van een ‘neurale netwerk’
>white|black||9|11|br Tegenwoordig zijn algemeen-toepasbare AI-modellen gebaseerd op deze netwerken, die losjes zijn geïnspireerd door biologische hersenen. Verschillende netwerken hebben verschillende groottes en architecturen. Ze zijn echter allemaal opgebouwd uit verbonden informatieverwerkende eenheden die ‘neuronen’ worden genoemd, waarbij de sterktes van verbindingen tussen neuronen ‘gewichten’ worden genoemd. Gewichten worden bijgewerkt via training met grote hoeveelheden data. Bron: International AI Safety Report 2025 (‡50) (aangepast).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Figuur 1.2: Een schematische weergave van de stadia van de ontwikkeling van algemeen-doeleinden AI
>white|black|left|9|11|br Internationaal AI-veiligheidsrapport 2026.


>white|orangered|left|13|15|bb Algemene-doel-AI wordt in fasen ontwikkeld

Het ontwikkelen van een algemeen inzetbaar AI-systeem omvat meerdere fasen, van de initiële modeltraining tot monitoring en updates na de ingebruikname (Figuur 1.2). In de praktijk overlappen deze stappen vaak iteratief. Elke fase vereist verschillende middelen (bijv. data, arbeid, rekenkracht) en verschillende technieken, en ze worden soms uitgevoerd door verschillende ontwikkelaars (Figuur 1.2 en Tafel 1.2).

Bijvoorbeeld, pre-training van modellen vereist doorgaans grote hoeveelheden rekenkracht en data, waardoor deze fase bijzonder gevoelig is voor beleid dat van invloed is op de toegang tot rekenbronnen of trainingsdata (‡51, ‡52). Evenzo omvatten gegevenscuratie en sommige methoden voor het verfijnen van modellen momenteel grote hoeveelheden menselijke arbeid voor aanvankelijke datalabeling (‡53). Deze fase is daarom gevoelig voor veranderingen in arbeidskosten, platformbeleid of regelgeving die van invloed is op grensoverschrijdende contracteringsafspraken.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Gegevensverzameling en -curatie
> 
  Voordat ontwikkelaars een AI-model voor algemeen gebruik trainen, verzamelen en bewerken datawerkers ruwe trainingsdata: ze verzamelen, opschonen, cureren en standaardiseren de data tot een formaat waar het model van kan leren. Dit kan een arbeidsintensief proces zijn. De trainingsdatasets achter state-of-the-art-modellen bestaan uit een immens aantal voorbeelden uit heel het internet.
  Teams ontwikkelen vaak geavanceerde filtermethoden om schadelijke inhoud te verminderen, dubbele gegevens te elimineren en de representatie over verschillende onderwerpen en bronnen te verbeteren (‡54, ‡55). Datacuratie kan ook helpen om schendingen van auteursrecht en privacy te verminderen, voorbeelden te verwijderen die gevaarlijke kennis bevatten, meerdere talen af te handelen en de documentatie voor dataprovenance te verbeteren (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Pre-training (eerste fase van training)

  Tijdens de pre-training voeren ontwikkelaars modellen enorme hoeveelheden diverse data toe om een brede basis aan informatie en contextueel begrip bij te brengen. Dit proces levert een ‘basismodel’ op. Dit is een proces dat zeer data- en rekenintensief is.

  Tijdens de pre-training worden modellen blootgesteld aan miljarden of triljarden voorbeelden van content zoals afbeeldingen, teksten of audio. Door deze blootstelling ontdekt het model geleidelijk abstracte kenmerken om data te representeren en leert het hoe deze kenmerken samenhangen, waardoor het nieuwe input in context kan begrijpen. Dit pre-trainingsproces duurt weken of maanden (‡59) en gebruikt tientallen of honderden duizenden grafische verwerkingseenheden (GPU's) of tensorverwerkingseenheden (TPU's) (‡60) – gespecialiseerde computerchips die zijn ontworpen om dit soort berekeningen snel te verwerken. Sommige ontwikkelaars voeren pre-training uit met hun eigen rekenkracht, terwijl anderen gebruikmaken van resources die worden aangeboden door gespecialiseerde compute-providers.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Nabetraining en fine-tuning (tweede trainingsfase)

  ‘Post-training’ verfijnt het basismodel verder om het te optimaliseren voor een specifieke toepassing. Het is een proces dat matig rekenintensief en zeer arbeidsintensief is. Een verschuiving naar het gebruik van ‘synthetische data’ – kunstmatig gegenereerde informatie die lijkt op data uit de echte wereld, maar wordt gemaakt met behulp van algoritmen of simulaties – helpt om deze fase minder arbeidsintensief te maken.
  Nabewerking omvat verschillende fine-tuning technieken en andere aanpassingen. ‘Gedeeltelijk begeleide fine-tuning’ houdt in dat een getraind model verder wordt getraind op specifieke datasets om de prestaties van het model in dat domein te verbeteren (‡61, ‡62). Een algemeen inzetbaar model zou bijvoorbeeld verder kunnen worden getraind op een grote verzameling radiologische afbeeldingen. ‘Versterkend leren’ (RL) houdt in dat de prestaties van het model worden verbeterd door het model ‘te belonen’ (positieve feedback geven) voor wenselijke uitkomsten en het model ‘te bestraffen’ (negatieve feedback geven) voor onwenselijke uitkomsten. Het heeft twee prominente subcategorieën. ‘Versterkend leren met menselijke feedback’ houdt in dat uitkomsten worden beloond die overeenkomen met menselijke voorkeuren en die worden bestraft die dat niet doen, op basis van menselijke feedback (‡63, ‡64*). ‘Versterkend leren met verifieerbare beloningen’ (RLVR) wordt gebruikt om de prestaties van het model te verbeteren voor taken die feitelijke juistheid vereisen, zoals wiskunde- of codegeneratie. Ontwikkelaars schakelen doorgaans afwisselend tussen het toepassen van nabewerkingstechnieken en het uitvoeren van tests totdat de resultaten aantonen dat het model voldoet aan de gewenste specificaties.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Systeemintegratie

  Ontwikkelaars combineren een of meer algemeen inzetbare AI-modellen met andere componenten om een ‘AI-systeem’ te creëren dat klaar is voor gebruik. GPT-5 (bijvoorbeeld) is een algemeen inzetbaar AI-model dat tekst, afbeeldingen en audio verwerkt, terwijl ChatGPT een algemeen inzetbaar AI-systeem is dat verschillende modellen van verschillende groottes en mogelijkheden combineert met een chatinterface, inhoudverwerking, Web-toegang en applicatie-integratie om een functioneel product te maken.
  Naast het operationeel maken van AI-modellen, zijn de aanvullende componenten in een AI-systeem ook bedoeld om de capaciteit, bruikbaarheid en veiligheid te verbeteren. Zo kan een systeem worden geleverd met een filter dat modelinputs of -outputs detecteert en blokkeert die schadelijke inhoud bevatten (‡65*). Ontwikkelaars gebruiken daarnaast steeds vaker ‘scaffolding’ – aanvullende software die is gebouwd rond algemene AI-modellen, waarmee ze vooruit kunnen plannen, doelen kunnen nastreven en met de wereld kunnen interacteren (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Implementatie en release
  Implementatie is het proces waarbij het geïntegreerde AI-systeem beschikbaar wordt gemaakt voor het beoogde gebruik. Ontwikkelaars en implementatiepartners zetten AI-systemen in binnen toepassingen, producten of diensten in de echte wereld. Ontwikkelaars kunnen AI-systemen intern implementeren (voor eigen gebruik) of extern (voor particuliere klanten of voor openbaar gebruik). Bij het extern implementeren van AI-systemen bieden bedrijven gebruikers vaak toegang via onlinegebruikersinterfaces of via application programming interfaces (APIs) waarmee gebruikers het systeem kunnen benaderen en uitvoeren. Een bedrijf kan bijvoorbeeld een op maat gemaakte chatbot voor klantenservice ontwerpen die wordt aangedreven door het algemene AI-systeem van een ander bedrijf.
  ‘AI-systeemplooiing’ verwijst naar het beschikbaar maken van een model voor gebruik in de echte wereld met geïntegreerde tools en interfaces, terwijl ‘modelrelease’ inhoudt dat het basismodel voor anderen toegankelijk wordt gemaakt – hetzij als open-weight (downloadbare parameters) of als closed-weight (alleen API-toegang). Zie §3.4. Open-weight-modellen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Monitoring en updates na de ingebruikname

  Ontwikkelaars verzamelen vaak gebruikersfeedback en analyseren die, volgen impact- en prestatiemetrieken en doen iteratieve verbeteringen om problemen aan te pakken die worden ontdekt bij werkelijk gebruik (‡67). Verbeteringen worden aangebracht door systeemkoppelingen bij te werken, vaak via voortdurende fine-tuning en door modellen toegang te geven tot externe databases met (recente) feiten. Dit houdt grote AI-modellen up-to-date zonder het volledige pre-trainingsproces te herhalen (‡68*). Dit stelt in staat dat capaciteiten zich kunnen opstapelen over opeenvolgende trainingsrondes, terwijl stabiliteit behouden blijft en de computationele kosten worden verlaagd.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tafel 1.2: Ontwikkelingsfasen van algemene-purpose AI
>white|black||9|11|br In elke general-purpose AI-ontwikkelingsfase wordt het AI-model verbeterd voor downstream-gebruik en uiteindelijk ingezet als een volledig geïntegreerd AI-systeem, bewaakt en bijgewerkt.


>white|orangered|left|13|15|bb Redeneringssystemen genereren tijdens de inferentie ‘ketens van gedachten’ om de prestaties te verbeteren

Inferentie gebeurt wanneer iemand het AI-model gebruikt nadat het is getraind. Er ontstaat bijvoorbeeld inferentie wanneer een persoon een AI-systeem vraagt om een reis te plannen en het model daarachter put uit relevante aspecten van wat het heeft geleerd over geografie, vervoer en keuken om een reisroute te genereren.

In the afgelopen decennium zijn vooruitgangen in AI-capaciteiten voor een groot deel tot stand gekomen door grotere trainingsrondes; dat wil zeggen: door de hoeveelheid rekenkracht te verhogen die wordt gebruikt om een AI-model te trainen. Recentelijk hebben onderzoekers echter meer vooruitgang geboekt door modellen informatie langer te laten verwerken en door ze te trainen om expliciete redeneerstappen te produceren terwijl ze een taak uitvoeren (‡69*, ‡70). AI-systemen die op deze manier werken worden ‘redeneringssystemen’ genoemd, en de tussenliggende toelichtingen die ze doorlopen bij het oplossen van een probleem of het beantwoorden van een vraag worden ‘ketens van gedachtegang’ genoemd. Redeneringssystemen vereisen bij gebruik meer rekenmiddelen om deze geavanceerde ketens van gedachtegang te genereren (‡71, ‡72, ‡73, ‡74), en ook meer middelen tijdens de training zodat ze beter leren redeneren. In de praktijk stellen deze redeneercapaciteiten AI-systemen in staat om complexere problemen op te lossen door iteratief een taak op te delen in kleinere stappen. Tafel 1.3 toont een voorbeeld van een niet-redenerend systeem en een redenerend systeem dat hetzelfde probleem oplost.

Redeneringssystemen hebben grote doorbraken bereikt in vermogens op uitdagende problemen. In 2025 konden bijvoorbeeld redeneringssystemen die gespecialiseerd zijn in het oplossen van wiskundige problemen, zoals Google’s Gemini Deep Think en een niet-uitgebracht, experimenteel model van OpenAI, problemen van de Internationale Wiskunde Olympiade oplossen (in een gestructureerde testomgeving) op een niveau dat gelijkwaardig is aan menselijke prestaties op goudmedaille-niveau (‡75, ‡76). Redeneringssystemen hebben aanzienlijke vooruitgang laten zien in formele domeinen zoals wiskunde, logische puzzels en gestructureerde wetenschappelijke vragen, waar redeneren stap voor stap expliciet kan worden geverifieerd (‡77). Redeneringssystemen kunnen echter ook falen door irrelevante, onproductieve of repetitieve ketens van gedachtegang te produceren (‡78, ‡79).

###@ Updates over trainingsmethoden

Sinds de publicatie van het laatste rapport (januari 2025) heeft een trainingsmethode genaamd ‘distillation’ de efficiëntie waarmee sommige modellen kunnen worden verfijnd aanzienlijk verhoogd. Distillation houdt in dat een ‘student’-model wordt getraind op de outputs van een krachtiger (en meestal groter) ‘teacher’-model, waardoor het student-model de outputs van de teacher direct kan imiteren (‡80). DeepSeek ontwikkelde bijvoorbeeld een groot model genaamd DeepSeek-R1, dat uitblinkt in chain-of-thought reasoning. R1 genereerde redeneer-outputs die vervolgens werden gebruikt om kleinere student-modellen te verfijnen, waaronder DeepSeek-V3. DeepSeek-V3 behoudt veel van R1’s wiskundige, programmeer- en documentanalyse-mogelijkheden en werd naar verluidt verfijnd voor ongeveer $10,000 USD (hoewel de kosten voor de pre-training niet zijn gerapporteerd) (‡81). Dit is waarschijnlijk een orde van grootte lager dan de kosten van het verfijnen van vergelijkbaar capabele, grotere modellen.

![table1.3](images/table1.3_example_reasoning.png)

##### Tafel 1.3: Een voorbeeld van een niet-redenerend systeem (links) versus een redenerend systeem (rechts)
>white|black||9|11|br Het oplossen van dezelfde raadsels, deze voorbeelden zijn aangepast uit echte AI-antwoorden. Het redeneersysteem besteedt meer tijd en rekenkracht aan “denken” door een “chain of thought” op te bouwen voordat het zijn definitieve antwoord geeft.

![figure.3](images/fig1.3_AI_agent.png)

##### Figuur 1.3: Een illustratieve weergave van een AI-agent
>white|black||9|11|br Een AI-model (midden) dat is geconfigureerd om iteratief te plannen, te redeneren en tools te gebruiken om taken in de echte wereld uit te voeren. Bron: International AI Safety Report 2026.


Distillatie kan dus een goedkope en efficiënte manier zijn voor modellen om krachtigere mogelijkheden te verwerven (‡82). Sommige onderzoekers hebben distillatie gebruikt om zeer capabele modellen bij te stellen met zo weinig als 1,000 voorbeelden die zijn gegenereerd door state-of-the-art-modellen (‡83). Omdat distillatie een vooraf bestaand docentmodel vereist, kan het niet rechtstreeks worden gebruikt om de mogelijkheden van state-of-the-art modellen te verbeteren. Het kan echter de verspreiding van geavanceerde AI-mogelijkheden versnellen, zelfs vanuit gesloten-source modellen (‡84*).

Samen met technologische vooruitgang in ‘distributed compute’ en gedecentraliseerde training (benaderingen waarbij ontwikkelaars meerdere processors, servers of datacenters gebruiken die samenwerken om AI-training of inferentie uit te voeren (‡85, ‡86, ‡87)), is de mate waarin veel AI-ontwikkelprojecten afhankelijk zijn van grootschalige, gecentraliseerde rekeninfrastructuur verminderd. Dit maakt het steeds vaker mogelijk dat minder goed gefinancierde actoren krachtige systemen ontwikkelen en inzetten.

###@ Updates over AI-agents

Sinds het laatste rapport (January 2025) hebben ontwikkelingen in hoe ontwikkelaars AI-modellen combineren met hulpmiddelen geleid tot de ontwikkeling van steeds krachtigere AI-agenten. AI-agenten zijn ontworpen om doelen na te streven, die vaak door gebruikers in natuurlijke taal worden gespecificeerd. Om deze doelen te bereiken, krijgen ze toegang tot hulpmiddelen, zoals geheugen, een computerinterface en webbrowsers. Deze hulpmiddelen en de code die wordt gebruikt om ze te combineren met het model worden ‘scaffolding’ genoemd, en ze helpen AI-agenten om autonoom met de wereld te interacteren, plannen te maken, belangrijke details te onthouden en doelen na te streven (‡88*, ‡89) met veel minder toezicht of ondersteuning van mensen. Manus AI is bijvoorbeeld een populaire AI-agent die verschillende taken kan automatiseren, waaronder webzoeken, softwareontwikkeling en online aankopen (‡90). Figuur 1.3 illustreert een eenvoudig voorbeeld van een AI-agent die is samengesteld uit een algemeen inzetbaar AI-model ‘brain’, dat iteratief kan plannen, redeneren en hulpmiddelen kan gebruiken voor geheugen, webbrowsen en computergebruik.

Digitale infrastructuur voor AI-agenten breidt zich uit (‡91), en ze komen steeds vaker voor in uiteenlopende sectoren (‡92, ‡93, ‡94). AI-agenten zijn ontwikkeld voor taken zoals onderzoek (‡37), software engineering (‡95), robotbesturing (‡96) en klantenservice (‡97). Voortdurend onderzoek en ontwikkeling hebben geleid tot steeds capabelere en autonomere AI-agenten of multi-agent-systemen. Onderzoekers hebben geschat dat de complexiteit van software benchmarktaken die AI-agenten kunnen uitvoeren ongeveer elke zeven maanden verdubbelt (zie ook §1.2. Huidige mogelijkheden) (‡98). Experts stellen dat steeds capabelere AI-agenten zowel grote kansen als risico's zullen opleveren (‡99, ‡100*) (zie §2.2.1. Betrouwbaarheidsuitdagingen).

###@ Bewijsleemtes

De belangrijkste hiaten in het bewijsmateriaal rond het ontwikkelproces van AI-systemen voor algemeen gebruik komen voort uit een gebrek aan publiek beschikbare informatie over hoe ze worden ontwikkeld. Sommige ontwikkelaars zijn zeer transparant over hoe ze AI-systemen voor algemeen gebruik ontwikkelen (‡1, ‡101). In het algemeen is er echter sprake van een beperkte mate van publieke en beleidsmatige kennis over hoe de meeste geavanceerde modellen worden ontwikkeld, beveiligd, geëvalueerd en ingezet. Dit geldt met name voor intern ingezette AI-systemen die binnen AI-bedrijven worden gebruikt maar niet door externe belanghebbenden worden gebruikt of begrepen (‡102, ‡103). Deze beperkte externe zichtbaarheid vormt uitdagingen voor transparantie en toezicht. Verschillende onderzoekers hebben gewezen op beperkte en inconsistente transparantie rond trainingsdata (‡104, ‡105, ‡106), AI-modellen voor algemeen gebruik (‡107, ‡108), AI-agenten (‡92), evaluaties (‡109), ontwikkelpijplijnen (‡110) en veiligheid (‡111). Beperkingen op externe openbaarmaking zijn soms noodzakelijk om bedrijfsgeheimen en intellectuele eigendom te beschermen. Tegelijkertijd maakt lage transparantie het moeilijker voor onafhankelijke onderzoekers en beleidsmakers om AI-modellen en systemen voor algemeen gebruik te bestuderen.


