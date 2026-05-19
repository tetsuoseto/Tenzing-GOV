###@ Vad är generella AI-system?

Allmänna AI-system är mjukvaruprogram som lär sig mönster från stora mängder data, vilket gör att de kan utföra en mängd olika uppgifter i stället för att vara specialiserade för en enda specifik funktion eller domän (se Tabell 1.1). För att skapa dessa system genomför AI-utvecklare en flerstegsprocess som kräver betydande datorkraft, stora datamängder och specialiserad kompetens (se Tabell 1.2). Datorkraft (ofta förkortat till ”compute”) krävs både för att utveckla och för att distribuera AI-system, och omfattar specialiserade datorkretsar samt den mjukvara och den infrastruktur som behövs för att köra dem.† Eftersom de tränas på stora, varierade datamängder kan allmänna AI-system utföra många olika uppgifter, såsom att sammanfatta text, generera bilder eller skriva dator kod. Avsnittet förklarar hur allmänna AI-system byggs, vad ”resonerande” modeller är, och hur policybeslut formar utvecklingen av allmänna AI-system.

    Notera † -- Termen “compute” kan också avse antingen en mätning av antalet beräkningar en processor kan utföra (typiskt mätt i flyttalsoperationer per sekund) eller specifikt den hårdvara (såsom grafikkretsar) som utför dessa beräkningar.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Språkbaserade system
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Kommando A (‡3*)
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
###@ Bildgeneratorer
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Videogeneratorer
- Cosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Veo 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotik- och navigationssystem
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Prediktorer för olika klasser av biomolekylära strukturer
- AlphaFold 3 (‡27)
- Förstärk (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ AI-agenter
- AlphaEvolve (‡31*)
- ChatGPT-agent (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- AI Scientist-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 1.1: Allmänna AI-typer
>white|black||9|11|br Det finns flera olika typer av allmänna AI-system. I denna rapport betraktas modeller som kan förutsäga strukturell information för olika klasser av molekyler som ”allmänna” AI-system eftersom de kan anpassas för en mängd olika uppgifter. Till exempel är modeller som tränats för att förutsäga proteinsstruktur tillämpbara för en mängd andra uppgifter, såsom att förutsäga proteininteraktioner, förutsäga bindningsställen för små molekyler samt att förutsäga och utforma cykliska peptider (‡40).


>white|orangered|left|13|15|bb Djupinlärning är grundläggande för allmänna AI-system

Forskare bygger allmänna AI-modeller med en process som kallas 'deep learning', som tränar modeller att lära sig från exempel (‡41). Till skillnad från mjukvaruutveckling lär sig deep learning-modeller att utföra uppgifter från data i stället för att förlita sig på handskrivna instruktioner. Genom att bearbeta stora mängder data, såsom bilder, text eller ljud, upptäcker dessa modeller sätt att representera datan, vilket skapar interna representationer av mönster (såsom former, ordassociationer eller ljudstrukturer) som hjälper modellen att känna igen samband och generera utdata som är i linje med dess träningsmål. Därefter använder de dessa inlärda interna representationer som abstrakta funktioner för att analysera ny, liknande data och generera utdata i samma stil. Till exempel kan en allmän- purpose AI-modell som tränats på tillräckligt många exempel av 19th-century romantisk engelsk poesi känna igen nya dikter i den stilen och ta fram nytt material i en liknande stil.

På en mer granular nivå fungerar djupinlärning genom att bearbeta data via lager av sammankopplade informationsbehandlingsnoder. Dessa noder kallas ofta för 'neuroner' eftersom de löst inspirerats av neuroner i biologiska hjärnor ('neural networks') (Figur 1.1) (‡42).När information flödar från ett lager av neuroner till nästa omvandlar modellen gradvis data till mer abstrakta representationer som grupper av inlärda egenskaper - mönster som modellen automatiskt har upptäckt i datan, snarare än sådana som har handkodats. Till exempel i en bildbearbetningsmodell kan de första lagren lära sig att detektera enkla egenskaper som kanter eller grundformer, medan djupare lager kombinerar dessa egenskaper för att identifiera mer komplexa mönster som ansikten eller objekt.

Funktionerna i alla lager upptäcks genom optimeringsprocessen som definierar träningsproceduren. Under träning, när modellen gör fel, justerar algoritmer för djupinlärning styrkan i olika kopplingar mellan neuroner för att förbättra modellens prestanda. Styrkan i varje koppling mellan noder kallas ofta en ”vikt”. Detta skiktade angreppssätt är det som ger djupinlärning dess namn.

Deep learning har visat sig vara mycket effektivt för att göra det möjligt för AI-system att utföra uppgifter som tidigare ansågs svåra för traditionella handprogrammerade beräkningssystem och andra tidigare symboliska eller regelbaserade AI-metoder. De flesta moderna allmänna AI-modellerna bygger nu på en specifik neuronnätsarkitektur som kallas för ”transformer” (‡43, ‡44). Transformers använder en ”attention”-mekanism (‡45) som hjälper modellen att fokusera på de mest relevanta delarna av indata när information bearbetas, till exempel genom att avgöra vilka ord i en mening som är viktigast för att förstå dess betydelse. Detta specifika sätt att bygga modeller har lett till betydande förbättringar inom översättning (‡43), bearbetning av naturligt språk (‡46), bildigenkänning (‡47) och taligenkänning (‡48, ‡49), vilket i slutändan har lett till utvecklingen av dagens mest avancerade modeller.

![fig1.1](images/fig1.1_neural_network.png)

##### Figur 1.1: En illustrativ representation av en "neuronnätverk"
>white|black||9|11|br Dagens allmänna AI-modeller bygger på dessa nätverk, som löst är inspirerade av biologiska hjärnor. Olika nätverk har olika storlekar och arkitekturer. Samtliga består dock av sammankopplade informationsbehandlingsenheter som kallas ”neuroner”, där styrkorna i kopplingarna mellan neuronerna kallas ”vikter”. Vikter uppdateras genom träning med stora mängder data. Källa: International AI Safety Report 2025 (‡50) (modifierad).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Figur 1.2: En schematisk representation av stegen i utvecklingen av allmännyttig AI
>white|black|left|9|11|br Internationell AI-säkerhetsrapport 2026.


>white|orangered|left|13|15|bb Allmännyttig AI utvecklas i etapper

Att utveckla ett generellt AI-system för allmänt bruk innebär flera steg, från inledande modellträning till uppföljning och uppdateringar efter driftsättning (Figur 1.2). I praktiken överlappar dessa steg ofta varandra på ett iterativt sätt. Varje steg kräver olika resursinsatser (t.ex. data, arbetskraft, beräkning) och olika tekniker, och de genomförs ibland av olika utvecklare (Figur 1.2 och Tabell 1.2).

Till exempel kräver modellförinlärning generellt stora mängder beräkning och data, vilket gör detta skede särskilt känsligt för policyer som påverkar tillgången till beräkningsresurser eller träningsdata (‡51, ‡52). På liknande sätt innebär datakurerering och vissa metoder för modellfinjustering för närvarande stora mängder mänskligt arbete för initial datamärkning (‡53). Detta skede är därför känsligt för förändringar i arbetskraftskostnader, plattformspolicyer eller regler som påverkar gränsöverskridande avtalsarrangemang.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Datainsamling och kuratering
> 
  Innan man tränar en allmänanvänd AI-modell samlar utvecklare och dataarbetare in, rensar, kuraterar och standardiserar rå träningsdata till ett format som modellen kan lära sig från. Detta kan vara en arbetsintensiv process. Träningsdatamängderna bakom state-of-the-art-modeller består av ett oerhört stort antal exempel från hela internet.
  Team utvecklar ofta sofistikerade filtreringsmetoder för att minska skadligt innehåll, eliminera dubbletter av data och förbättra representationen över olika ämnen och källor (‡54, ‡55). Datahushållning kan också bidra till att minska upphovsrätts- och integritetsöverträdelser, ta bort exempel som innehåller farlig kunskap, hantera flera språk och förbättra dokumentationen för dataproveniens (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Förträning (första steget av träning)

  Under förträning matar utvecklare modeller med enorma mängder av varierad data för att skapa en bred kunskapsbas och kontextuell förståelse. Denna process resulterar i en ”basmodell”. Detta är en mycket datu- och beräkningsintensiv process.

  Under förutträning exponeras modeller för miljarder eller biljoner exempel på innehåll som bilder, texter eller ljud. Genom denna exponering upptäcker modellen gradvis abstrakta egenskaper för att representera data och lär sig hur dessa egenskaper hänger ihop, vilket gör att den kan tolka nya indata i sitt sammanhang. Denna förutträningsprocess tar veckor eller månader (‡59) och använder tiotals eller hundratals tusen grafikkort (GPUs) eller ten sorkprocessorer (TPUs) (‡60) – specialiserade datorkretsar som är utformade för att snabbt utföra många sådana beräkningar. Vissa utvecklare genomför förutträning med sin egen beräkningskapacitet, medan andra använder resurser som tillhandahålls av specialiserade leverantörer av beräkning.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Eftertränning och finjustering (andra träningsfasen)

  ”Post-training” förädlar vidare baskedjan för att optimera den för en specifik tillämpning. Det är en process som är måttligt beräkningsintensiv och mycket arbetsintensiv. Ett skifte mot att använda ”syntetiska data” – artificiellt genererad information som efterliknar data från verkliga miljöer men som skapas med hjälp av algoritmer eller simuleringar – bidrar till att göra detta steg mindre arbetsintensivt.
  Efterträning omfattar olika finjusteringstekniker och andra modifieringar. ”Övervakad finjustering” innebär att ytterligare träna en tränad modell på specifika datamängder för att förbättra modellens prestanda inom det området (‡61, ‡62). Till exempel kan en generell modell tränas vidare på en stor samling av radiologiska bilder. ”Förstärkningsinlärning” (RL) innebär att förbättra modellens prestanda genom att ”belöna” en modell (ge positiv återkoppling) för önskvärda utdata och ”straffa” en modell (ge negativ återkoppling) för oönskade utdata. Det har två framträdande underkategorier. ”Förstärkningsinlärning från mänsklig feedback” innebär att belöna utdata som stämmer överens med mänskliga preferenser och straffa sådana som inte gör det, baserat på mänsklig feedback (‡63, ‡64*). ”Förstärkningsinlärning med verifierbara belöningar” (RLVR) används för att förbättra modellens prestanda på uppgifter som kräver faktamässig korrekthet, såsom matematik eller kodgenerering. Utvecklare växlar typiskt mellan att tillämpa efterträningsmetoder och att köra tester tills resultaten visar att modellen uppfyller önskade specifikationer.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Systemintegration

  Utvecklare kombinerar en eller flera generella AI-modeller med andra komponenter för att skapa ett “AI-system” som är redo att användas. GPT-5 (till exempel) är en generell AI-modell som bearbetar text, bilder och ljud, medan ChatGPT är ett generellt AI-system som kombinerar flera modeller i olika storlekar och med olika kapabiliteter med ett chattgränssnitt, innehållsbehandling, webåtkomst och applikationsintegration för att skapa en fungerande produkt.
  Utöver att göra AI-modeller operativa syftar även de ytterligare komponenterna i ett AI-system till att förbättra förmåga, användbarhet och säkerhet. Till exempel kan ett system ha ett filter som upptäcker och blockerar modellindata eller -utdata som innehåller skadligt innehåll (‡65*). Utvecklare använder också i allt högre grad ”scaffolding” – ytterligare mjukvara som byggs runt generella AI-modeller och som gör att de kan planera i förväg, sträva mot mål och interagera med världen (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Distribution och release
  Implementering är processen att göra det integrerade AI-systemet tillgängligt för dess avsedda användning. Utvecklare och driftsättare implementerar AI-system i verkliga applikationer, produkter eller tjänster. Utvecklare kan driftsätta AI-system internt (för egen användning) eller externt (för privata kunder eller publikt bruk). När AI-system driftsätts externt tillhandahåller företag ofta användare åtkomst via online-användargränssnitt eller via applikationsprogrammeringsgränssnitt (APIs) som gör att användare kan komma åt och köra systemet. Till exempel kan ett företag utforma en skräddarsydd kundtjänstchattbot som drivs av ett annat företags generella AI-system.
  ”AI system deployment” avser att göra en modell tillgänglig för verklig användning med integrerade verktyg och gränssnitt, medan ”model release” innebär att göra baskomponenten tillgänglig för andra – antingen som open-weight (nedladdningsbara parametrar) eller closed-weight (endast API-åtkomst). Se §3.4. Open-weight-modeller.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Övervakning efter driftsättning och uppdateringar

  Utvecklare samlar ofta in och analyserar användarfeedback, följer påverkan- och prestandamått och gör iterativa förbättringar för att åtgärda problem som upptäcks vid verklig användning (‡67). Förbättringar görs genom att uppdatera systemintegrationer, ofta via kontinuerlig finjustering och genom att ge modeller tillgång till externa databaser med (nyligen) verifierade fakta. Detta håller stora AI-modeller uppdaterade utan att upprepa hela den fullständiga förträningsprocessen (‡68*). Detta gör att förmågor kan byggas upp över på varandra följande träningsomgångar samtidigt som stabiliteten bibehålls och beräkningskostnaderna minskar.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 1.2: Utvecklingssteg för allmännyttig AI
>white|black||9|11|br I varje allmänt använd AI-utvecklingssteg förbättras AI-modellen för användning i efterföljande led och till slut distribueras den som ett fullt integrerat AI-system, som övervakas och uppdateras.


>white|orangered|left|13|15|bb Resonemangssystem genererar “tankekedjor” under inferens för att förbättra prestanda

Inferens sker när någon använder AI-modellen efter att den har tränats. Till exempel inträffar inferens när en person ber ett AI-system att planera en resa och modellen bakom detta använder relevanta delar av det den har lärt sig om geografi, transport och mat för att generera ett resprogram.

Under det senaste decenniet har framsteg i AI-förmågor till stor del kommit från större träningskörningar; det vill säga att öka den beräkningskraft som används för att träna en AI-modell. Nyligen har dock forskare gjort fler framsteg genom att låta modeller bearbeta information under längre tid och genom att träna dem att producera explicita resonemangssteg när de utför en uppgift (‡69*, ‡70). AI-system som fungerar på detta sätt kallas 'resoneringssystem', och de mellanliggande förklaringar de går igenom när de löser ett problem eller besvarar en fråga kallas 'tankekedjor'. Resoneringssystem kräver mer beräkningsresurser vid användning för att generera dessa avancerade tankekedjor (‡71, ‡72, ‡73, ‡74), och fler resurser under träning så att de lär sig resonera bättre. I praktiken gör dessa resonemangsförmågor att AI-system kan lösa mer komplexa problem genom att iterativt bryta ned en uppgift i mindre steg. Tabell 1.3 visar ett exempel på ett icke-resonerande system och ett resonerande system som löser samma problem.

Resonerande system har uppnått stora genombrott i förmåga för svåra problem. Till exempel, under 2025, löste resonerande system som specialiserats på matematiska problem, som Googles Gemini Deep Think och en ännu inte släppt, experimentell modell från OpenAI, problem från International Mathematical Olympiad (i en strukturerad testsituation) på en nivå som motsvarar mänsklig prestation på guldmedaljnivå (‡75, ‡76). Resonerande system har visat betydande framsteg i formella domäner som matematik, logikpussel och strukturerade vetenskapliga frågor, där steg-för-steg-resonemang kan verifieras uttryckligen (‡77). Däremot kan resonerande system också misslyckas genom att generera irrelevanta, oproduktivt eller repetitiva kedjor av tankeverksamhet (‡78, ‡79).

###@ Uppdateringar om träningsmetoder

Sedan publiceringen av den senaste rapporten (Januari 2025) har en träningsmetod som kallas ’distillation’ i hög grad ökat effektiviteten med vilken vissa modeller kan finjusteras. Distillation innebär att man tränar en ’student’-modell på utdata från en mer kraftfull (och vanligtvis större) ’lärare’-modell, så att studentmodellen direkt kan imitera lärarens utdata (‡80). Till exempel utvecklade DeepSeek en stor modell som heter DeepSeek-R1, som utmärker sig på resonemang i kedjor (chain-of-thought). R1 genererade resonemangsutdata som sedan användes för att finjustera mindre studentmodeller, inklusive DeepSeek-V3. DeepSeek-V3 bibehåller mycket av R1:s matematiska, kodnings- och dokumentanalysförmåga och uppgavs ha finjusterats för ungefär $10,000 USD (även om kostnaderna för förträning inte rapporterades) (‡81). Detta är troligen flera storleksordningar lägre än kostnaden för att finjustera liknande kapabla, större modeller.

![table1.3](images/table1.3_example_reasoning.png)

##### Tabell 1.3: Ett exempel på ett icke-resonerande system (vänster) jämfört med ett resonerande system (höger)
>white|black||9|11|br Att lösa samma gåta använder dessa exempel, anpassade från verkliga AI-svar. Resonemangssystemet lägger mer tid och beräkningsresurser på “tänkande” genom att konstruera en “chain of thought” innan det ger sitt slutliga svar.

![figure.3](images/fig1.3_AI_agent.png)

##### Figur 1.3: En illustrativ representation av ett AI-agent
>white|black||9|11|br En AI-modell (centrum) som har konfigurerats att iterativt planera, resonera och använda verktyg för att genomföra uppgifter i verkligheten. Källa: International AI Safety Report 2026.


Distillation kan alltså vara ett billigt och effektivt sätt för modeller att skaffa sig mer kraftfulla förmågor (‡82). Vissa forskare har använt distillation för att finjustera mycket kapabla modeller med så få som 1,000 exempel som genererats från state-of- the-art-modeller (‡83). Eftersom distillation kräver en i förväg befintlig lärarmodell kan den inte användas direkt för att föra fram state-of-the-art-modellernas kapabiliteter. Däremot kan den påskynda spridningen av avancerade AI-kapabiliteter, även från slutna källkodsmodeller (‡84*).

Tillsammans med tekniska framsteg inom “distribuerad beräkning” och decentraliserad träning (metoder där utvecklare använder flera processorer, servrar eller datacenter som arbetar tillsammans för att utföra AI-träning eller inferens (‡85, ‡86, ‡87)) har graden i vilken många AI-utvecklingsprojekt är beroende av storskalig, centraliserad beräkningsinfrastruktur minskat. Detta möjliggör i allt högre grad för aktörer med sämre resurser att utveckla och distribuera kraftfulla system.

###@ Uppdateringar om AI-agenter

Sedan den senaste Rapporten (January 2025) har framsteg i hur utvecklare kombinerar AI-modeller med verktyg möjliggjort utvecklingen av alltmer kraftfulla AI-agenter. AI-agenter är utformade för att sträva efter mål, som ofta anges av användare i naturligt språk. För att uppnå dessa mål ges de tillgång till verktyg, såsom minne, ett datorgränssnitt och webbläsare. Dessa verktyg och den kod som används för att kombinera dem med modellen kallas för ”scaffolding”, och de hjälper AI-agenter att självständigt interagera med omvärlden, göra planer, komma ihåg viktiga detaljer och sträva efter mål (‡88*, ‡89) med betydligt mindre övervakning eller assistans från människor. Till exempel är Manus AI en populär AI-agent som kan automatisera olika uppgifter, inklusive webbsökning, mjukvaruutveckling och onlineinköp (‡90). Figur 1.3 visar ett enkelt exempel på en AI-agent bestående av en allmän AI-modell ”brain” som iterativt kan planera, resonera och använda verktyg för minne, webbläsning och dators användning.

Digital infrastruktur för AI-agenter expanderar (‡91), och de blir allt vanligare i branscher (‡92, ‡93, ‡94). AI-agenter har utvecklats för uppgifter som forskning (‡37), mjukvaruteknik (‡95), robotstyrning (‡96) och kundservice (‡97). Pågående forskning och utveckling har lett till gradvis mer kapabla och mer autonoma AI-agenter, eller multi-agentsystem. Forskare har uppskattat att komplexiteten i mjukvarubenchmark-uppgifter som AI-agenter kan genomföra fördubblas ungefär var sjunde månad (se även §1.2. Nuvarande förmågor) (‡98). Experter hävdar att allt mer kapabla AI-agenter kommer att ge upphov till både stora möjligheter och risker (‡99, ‡100*) (se §2.2.1. Tillförlitlighetsutmaningar).

###@ Evidensluckor

De främsta kunskapsluckorna i samband med utvecklingsprocessen för generella AI-system uppstår till stor del på grund av brist på offentligt tillgänglig information om hur de utvecklas. Vissa utvecklare är mycket transparenta med hur de utvecklar generella AI-system (‡1, ‡101). I allmänhet finns dock en begränsad grad av offentlig och policyrelevant kunskap om hur de flesta avancerade modeller utvecklas, skyddas, utvärderas och driftsätts. Detta gäller särskilt internt driftsatta AI-system som används inom AI-företag men inte används eller förstås av externa intressenter (‡102, ‡103). Denna begränsade externa synlighet skapar utmaningar för transparens och tillsyn. Olika forskare har pekat på begränsad och inkonsekvent transparens kring träningsdata (‡104, ‡105, ‡106), generella AI-modeller (‡107, ‡108), AI-agenter (‡92), utvärderingar (‡109), utvecklingspipelines (‡110) och säkerhet (‡111). Begränsningar i extern offentliggörelse är ibland nödvändiga för att skydda företags affärshemligheter och immateriella rättigheter. Samtidigt gör låg transparens det svårare för oberoende forskare och beslutsfattare att studera generella AI-modeller och system.


