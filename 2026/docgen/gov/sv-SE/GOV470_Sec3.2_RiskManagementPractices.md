##########
>white|orangered|left|14|30|hr Avsnitt 3.2
### 3.2. Riskhanteringsrutiner
>white|orangered|left|24|30|hb Riskhanteringspraxis

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Viktig information
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Riskhantering för allmänna ändamål inom AI omfattar en rad metoder som används för att identifiera, bedöma och minska risker från allmänna ändamål inom AI. Detta inkluderar tester och utvärdering på modellnivå (t.ex. "red-teaming"), organisatoriska processer som vägleder utvecklings- och lanseringsbeslut, villkorade skyddsåtgärder (t.ex. "if-then"-åtaganden) samt incidentrapportering.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Flera AI-utvecklare har tagit fram Frontier AI Safety Frameworks. Dessa ramverk innehåller information om riskbedömningar och anger villkorade åtgärder, såsom åtkomstrestriktioner som företag planerar att införa för mer kapabla modeller. De skiljer sig åt i vilka risker de täcker, hur de definierar trösklar för förmåga och vilka åtgärder som utlöses när trösklarna nås.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Bevisen för AI-riskhanteringsmetoders verkliga effektivitet i verkliga miljöer är fortfarande begränsade. Avsaknad av incidentrapportering och övervakning gör det svårt att bedöma hur väl nuvarande metoder minskar risker, eller hur konsekvent de implementeras.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sedan publiceringen av den senaste rapporten (januari 2025) har riskhanteringen blivit mer strukturerad genom nya bransch- och styrningsinitiativ. Nya instrument som EU:s allmänna uppförandekod för AI för allmänt ändamål, Kinas ramverk för AI-säkerhetsstyrning 2.0 och G7:s Hiroshima AI-process för rapportering, tillsammans med initiativ som drivs av företag, visar på en trend mot mer standardiserade tillvägagångssätt för transparens, utvärdering och incidentrapportering.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Marknadsdynamik och takten i AI-utvecklingen skapar ytterligare utmaningar. På grund av konkurrenspress kan AI-företag ställas inför avvägningar mellan snabbare produktlanseringar och investeringar i riskreducerande insatser. Många AI-relaterade skador externaliseras dessutom, och det är fortfarande oklart vilken juridisk ansvarsskyldighet som gäller, samtidigt som styrningsprocesser kan vara långsamma att anpassa till förändringar i AI-landskapet.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Viktiga utmaningar för beslutsfattare inkluderar att prioritera bland de olika riskerna som orsakas av allmännyttig AI, och att tydliggöra vilka aktörer i hela AI-värdekedjan som är bäst positionerade för att mildra dem. Dessa utmaningar förstärks av begränsad insyn i hur risker identifieras, utvärderas och hanteras i praktiken, samt av fragmenterat informationsutbyte mellan utvecklare, driftsättare och leverantörer av infrastruktur.
>oldlace|black||11|15|br      


AI-riskhantering omfattar ett antal metoder som syftar till att identifiera, bedöma och minska sannolikheten och allvaret av risker som är förknippade med AI-system. Dessa metoder kan implementeras av AI-utvecklare, de som driftsätter systemen, utvärderare och regulatorer. Exempel inkluderar hotmodellering, risknivåindelning, red-teaming, granskning (auditing) och incidentrapportering. Avsnittet beskriver nuvarande riskhanteringsmetoder, nya utvecklingar och kvarstående begränsningar.

Sedan början av 2025 har flera nya internationella initiativ för riskhantering av allmännyttig AI utvecklats, inklusive organisatorisk transparens och ramverk för riskrapportering samt regulatoriska och styrningsmässiga ramverk.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Figur 3.4: Fyra komponenter i riskhantering
>white|black||9|11|br De fyra kategorierna av metoder för riskhantering för generell AI: riskidentifiering; riskanalys och utvärdering; riskreducering; och riskstyrning. Dessa bildar en iterativ och cyklisk process. Riskstyrning, som visas i mitten, underlättar framgången för de andra komponenterna. Källa: International AI Safety Report 2026.


Återstående utmaningar innefattar begränsad standardisering, vilket försvårar efterlevnad och bedömning, samt begränsad evidens om faktisk effekt i den verkliga världen. Vidare skiljer sig institutionella, kulturella och politiska sammanhang åt globalt, vilket innebär att metoder för att identifiera och hantera risker, inklusive acceptabla tröskelvärden för risk, kan variera mellan regioner. Denna sections genomgång av riskhanteringsmetoder är deskriptiv: den syftar till att informera aktörer i AI-ekosystemet om nuvarande globala tillvägagångssätt för riskhantering. Där sådan finns diskuteras evidens om effektiviteten och begränsningarna hos dessa metoder, men policyrekommendationer ligger utanför ramen för detta arbete.

###@ Komponenter i riskhantering

Riskhantering är en iterativ process med metoder och arbetssätt som sträcker sig över hela livscykeln för utveckling och driftsättning av AI, men som fungerar tillsammans på ett sammanhängande sätt (‡969). Riskhantering för generell AI kan omfatta roller för en bred uppsättning aktörer, inklusive data scientists, model engineers, auditerare, ämnesexperter, chefer, slutanvändare, påverkade samhällen, tredjepartsleverantörer, policyutformare, regeringar, standardorganisationer och civilsamhällesorganisationer (‡970, ‡971, ‡972). Ledande riskhanteringsstandarder är ofta interoperabla, men använder olika terminologi för att beskriva beståndsdelarna i riskhantering (‡973, ‡974). De har typiskt fyra sammankopplade komponenter (Figur 3.4): identifiera; analysera och utvärdera; mildra; och styra risk (‡970, ‡973, ‡975, ‡976). Tabellerna nedan ger illustrativa exempel på relevanta metoder, tekniker och verktyg. Arbetssätten fortsätter att utvecklas, så tabellerna är inte uttömmande, och tillämpbarheten kommer att variera mellan olika sammanhang.

###@ Riskidentifiering

Riskidentifiering är processen att hitta, känna igen och beskriva risker. Omfattande riskidentifiering brukar omfatta kapacitetsdrivna bedömningar, som testar om modeller har vissa farliga förmågor (‡977), samt riskmodellering (‡978) och prognostisering (‡715*), som används för att undersöka befintliga och framväxande risker. Tabell 3.1 ger olika exempel på riskidentifieringspraxis. Riskidentifiering bygger också på samverkan med relevanta experter och samhällen för att förstå den bredare kontexten för hur risker uppstår (‡979, ‡980). Mekanismer som bug bounty-program kan stödja denna process genom att ge incitament för identifiering av tidigare okända sårbarheter (‡981) (Tabell 3.1). Ett viktigt mål med riskidentifiering är att ta höjd för både väletablerade, välförstådda risker och potentiella framtida risker som fortfarande är osäkra eller bristfälligt karaktäriserade (‡982). Detta är särskilt viktigt för generell AI, där många risker ännu kanske inte är fullt förstådda eller observerbara (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bug bounty-program
  Bug bounty-program eller program för sårbarhetsrapportering uppmuntrar människor att hitta och rapportera sårbarheter i AI-system. Flera utvecklare har implementerat bug bounty-program (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Expertkonsultation
  Domänexperter, användare och berörda gemenskaper ger insikter om sannolika risker. Det finns nya riktlinjer för deltagande och inkluderande AI (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Fiskbensdiagram (Ishikawa)
  Ishikawadiagram är väletablerade verktyg för analys av grundorsaker, och forskare har föreslagit att använda dem för strukturerad analys av AI-riskincidenter (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Prognostisering
  Prognostisering är processen att förutsäga framtida händelser eller trender baserat på analys av tidigare och nuvarande data. Det har använts för att jämföra den relativa sannolikheten för, till exempel, olika ekonomiska utfall på grund av avancerad AI (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risktaxonomi
  Risktaxonomier är ett sätt att kategorisera och organisera risker över flera dimensioner. Det finns flera som beskriver risker för generella ändamål AI (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Scenarioplanering
  Scenarioplanering innebär att man utvecklar trovärdiga framtidsscenarier och analyserar hur risker kan förverkligas. Detta har använts för att utforska riskerna och effekterna av AI-modeller (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hotmodellering
  Hotmodellering är en process för att identifiera hot och sårbarheter i ett system. Många AI-utvecklare lyfter fram sin användning av hotmodellering för att förutse potentiella missbruks-scenarier för AI-system (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 3.1: Riskidentifikations- exempel inom riskhantering för allmänna ändamål AI
>white|black||9|11|br Exempelmetoder för identifiering av AI-risker listade alfabetiskt. Metoderna som ingår
är utformade för att stödja riskidentifiering för många olika risktyper, inklusive risker till följd av illvillig användning, risker till följd av fel och systemiska risker. Med tanke på att riskhantering för generella AI-ändamål fortfarande är i ett tidigt skede kommer inte alla metoder att vara lämpliga för varje AI-utvecklare eller AI-aktör som distribuerar AI.


>white|orangered|left|14|15.5|bb Hotmodellering och risk-taxonomier är framträdande metoder för riskidentifiering

Två framstående metoder för att identifiera riskerna med generell-purpose AI är threat modelling och risk-taxonomier. International AI Safety Report 2026 (en strukturerad process för att kartlägga hur AI-relaterade risker kan ta form) och risk-taxonomier. Meta, till exempel, använder threat modelling-övningar för att förutse potentiella missbruks-scenarier för sina AI-modeller (‡990), och Anthropic inkluderar threat modelling som en del av sitt ASL-3 Deployment Standard (‡991). AI-risk- och hazard-taxonomier, som listar riskkategorier och exempel, kan också fungera som en utgångspunkt för att konceptualisera, identifiera och specificera de mest framträdande riskerna som är förknippade med generell-purpose AI inom specifika tillämpningsdomäner (‡906, ‡988, ‡992, ‡993).

###@ Riskanalys och utvärdering

Riskanalys och utvärdering är processen att fastställa risknivån för en AI-modell eller ett AI-system och jämföra den med etablerade kriterier för att bedöma acceptabilitet eller behovet av riskreducerande åtgärder (‡994, ‡995, ‡996, ‡997). Den omfattar metoder som att mäta modellens prestanda på riktmärken (‡998) och utvärderingar (‡176, ‡715), genomföra red-teaming-övningar (‡999*), konsekvensbedömningar (‡1000) och revisioner (‡1001, ‡1002). Se Tabell 3.2 för exempel på riskanalys och utvärdering av allmännyttig AI. Metoderna är utformade för att stödja analys och utvärdering för många olika risktyper samtidigt.

Nyckelmål för riskanalys och utvärdering är att genomföra utvärderingar av modellers förmågor och sårbarheter (‡1003), att använda robust riskmodellering för att informera beslut om risktrösklar (‡1004, ‡1005) och att förstå hur AI-system används i praktiken för att bedöma efterföljande samhälleliga effekter (‡869, ‡904, ‡905, ‡1006). Riskanalys- och utvärderingsprocesser anses ofta vara mer benägna att identifiera risker när de inkluderar oberoende granskning (‡1001, ‡1007), tar stöd av expertis över sektorer (‡1008) samt inbegriper olika perspektiv från flera domäner och discipliner, liksom från berörda samhällen (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Revisioner
  Granskningar är formella genomgångar av AI-modellers prestanda och effekter och/eller en organisations efterlevnad av standarder, policyer och rutiner, som genomförs internt eller av en extern part. AI-granskning är ett växande område, och många verktyg och metoder finns för att granska AI-modeller och metoderna hos utvecklare av AI-modeller (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Benchmarkar
  Benchmarkar är standardiserade, ofta kvantitativa tester eller mått som används för att utvärdera och jämföra prestandan hos AI-system på en fast uppsättning uppgifter som är utformad för att representera verklig användning (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bowtie-metoden
  Bowtie-metoden är en välkänd metod för att visualisera var kontroller kan läggas till för att mildra riskhändelser. Den ger en tydlig skillnad mellan proaktiv och reaktiv riskhantering (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Delphi-metoden
  Delphi-metoden är en gruppbeslutsmetod som använder en serie frågeformulär för att samla samsyn från en panel av experter (‡1020, ‡1021). Den har använts för att hjälpa till att utforska möjliga framtider med avancerad AI (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Fältprovning
  Fälttestning utvärderar en AI-systems prestanda och påverkan i en verklig, operativ miljö. Viss forskning betonar fälttestning som ett komplement till modellutvärdering för att bedöma verkliga utfall och konsekvenser (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Konsekvensbedömning
  Konsekvensbedömningar bedömer de potentiella konsekvenserna av en teknik eller ett projekt. Detta kan omfatta att kvantifiera, sammanställa och prioritera konsekvenserna. EU:s AI-förordning kräver till exempel att utvecklare av AI-system med hög risk genomför bedömningar av grundläggande rättigheter (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Utvärdering av modell
  Utvärderingar av modeller inkluderar processer och tester för att bedöma och mäta en AI-modells prestanda för en specifik uppgift. Det finns många AI-utvärderingar för att bedöma olika förmågor och risker, inklusive för säkerhet, cybersäkerhet och social påverkan (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Probabilistisk riskbedömning
  Sannolikhetsbaserad riskbedömning är en metodik för att utvärdera risker som är förknippade med komplexa system eller processer som inbegriper osäkerhet. Den har anpassats för avancerade AI-system (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Red-teamning
  Red-teaming är en övning där en grupp människor eller automatiserade system låtsas vara en angripare och angriper en organisations tekniska system för att identifiera sårbarheter. Många AI-företag har interna rutiner för red-teaming av AI-system (‡458, ‡1028). Red-teaming kan även genomföras av aktörer utanför företag. Dessa team ställs inför utmaningar som begränsad åtkomst, men kan också lyfta fram distinkta insikter (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb riskmatriser
  Riskmatriser är ett visuellt verktyg för att hjälpa till att prioritera risker utifrån deras sannolikhet för inträffande och potentiella påverkan (‡1027). Vissa AI-utvecklare inkluderar grundläggande riskmatriser i sina Frontier AI Safety Frameworks (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risktrösklar/ risknivåer
  Risktrösklar eller nivåer är kvantitativa eller kvalitativa gränser som skiljer acceptabla från oacceptabla risker och utlöser specifika riskhanteringsåtgärder när de överskrids. För allmännyttig AI bestäms de av en kombination av förmågor, påverkan, beräkning, räckvidd och andra faktorer (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risk tolerans
  Risk tolerans avser den nivå av risk som en organisation är villig att acceptera. Inom AI anges risktoleranser ofta implicit genom företagsrelaterade policyer och praxis, medan vissa regulatoriska system uttryckligen definierar oacceptabla risker och kopplar rättsliga konsekvenser till dem (‡1032). Vissa företag beskriver sin risk tolerans i termer av en ny modells marginella risk; det vill säga i vilken utsträckning en modell kontrafaktiskt ökar risk utöver den risk som redan skapas av befintliga modeller eller andra tekniker (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Säkerhetsfall
  Ett säkerhetsärende (safety case) är ett strukturerat argument, som stöds av bevis, för att ett system är tillräckligt säkert att använda i ett visst sammanhang. Nyare litteratur (‡1037, ‡1038, ‡1039) har undersökt säkerhetsärenden för AI-system i framkant och vissa ramverk för Frontier AI Safety (Frontier AI Safety Frameworks) hänvisar till dem (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Systemsäkerhetsanalys
  Systemsäkerhetsanalys belyser beroenden mellan komponenter och det system som de ingår i, för att kunna förutse hur systemnivå-hazards kan uppstå till följd av fel i komponenter eller processer, eller genom interaktioner mellan delsystem, mänskliga faktorer och miljöförhållanden. Metoder som tillämpats för AI-system i litteraturen inkluderar systems-theoretic process analysis (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 3.2: Riskanalys/utvärdering i allmän AI-riskhantering
>white|black||9|11|br Exempelmetoder för analys/utvärdering av AI-risker, listade alfabetiskt. Givet den tidiga (nascent) karaktären hos riskhantering för allmännyttig AI, kommer inte alla metoder att vara lämpliga för varje AI-utvecklare eller -utövare.


>white|orangered|left|14|15.5|bb Vanliga verktyg för riskanalys inkluderar riktmärken och modellutvärderingar

Benchmarks och modellutvärderingar är standardiserade tester för att bedöma generella AI-systemens prestanda på specifika uppgifter. Forskare har utvecklat ett brett spektrum av benchmarks och utvärderingar, inklusive uppsättningar med utmanande flervalsfrågor, problem inom mjukvaruingenjörskonst och arbetsrelaterade uppgifter i simulerade kontorsmiljöer (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Skadliga kapacitetsutvärderingar (‡715) används för att bedöma om en generell AI-modell eller ett system har särskilt farlig kunskap eller färdigheter, t.ex. förmågan att bistå vid cyberattacker (se §2.1.3. Cyberattacker).

Högst betydelsefulla beslut av företag och regeringar om modellutsläpp baseras delvis på dessa utvärderingar (‡1050, ‡1051, ‡1052). Emellertid varierar riktmärken kraftigt i kvalitet och omfattning (‡998, ‡1003), och det kan vara svårt att bedöma deras giltighet på grund av många brister i riktmärkesmetodik (‡902, ‡909, ‡1003, ‡1053*). Till exempel kan riktmärken bli ”mättade” – när många modellers poäng närmar sig den högsta poängen – vilket innebär att de inte längre skiljer modeller åt i särskilt hög grad. Modeller är också allt oftare benägna att tolka vissa uppgifter som utvärderingar och uppvisa olika beteenden än vad de skulle göra på liknande uppgifter i driftsättningssammanhang på grund av ”situationsmedvetenhet” (se §2.2.2. Förlust av kontroll). Slutligen har riktmärken och utvärderingar väldokumenterade begränsningar: framför allt misslyckas de med att fånga risker som är förknippade med allmännyttig AI-användning i nya domäner och för nya uppgifter, eftersom testförhållanden skiljer sig från faktisk användning i varierande grad (‡913) (se §1.2. Aktuella förmågor och §3.1. Tekniska och institutionella utmaningar).

>white|orangered|left|14|15.5|bb Red-teaming möjliggör mer domänspecifika bedömningar av risk

En annan vanlig metod för att bedöma risker är red-teaming. Ett “red team” är en grupp utvärderare som får i uppdrag att leta efter sårbarheter, begränsningar eller möjligheter till missbruk. Red-teaming kan vara domänspecifik och utföras av experter inom domänen, eller vara öppen för att utforska nya riskfaktorer. Till exempel kan ett red team utforska “jailbreaking”-attacker som kringgår modellens säkerhetsbegränsningar (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). Till skillnad från benchmarker är en viktig fördel med red-teaming att red teams kan anpassa sina utvärderingar till det specifika system som testas. Till exempel kan red teams utforma anpassade indata för att identifiera värsta-falls-beteenden, möjligheter för skadlig användning och oväntade fel. Däremot kan det kräva särskild åtkomst till modeller och kan misslyckas med att synliggöra viktiga kategorier av risker (‡999, ‡1028).

Viktigt är att avsaknaden av identifierade risker inte innebär att dessa risker är låga: tidigare arbete visar att buggar ofta undgår upptäckt, särskilt när red teams har begränsad tillgång eller begränsade resurser (‡1060). Forskning har också ifrågasatt huruvida red-teaming kan ge tillförlitliga och reproducerbara resultat (‡1061). Sammansättningen av red teamet och de instruktioner som ges till red-teamare (‡1062), antalet angreppsrundor (‡1063) samt modellens tillgång till verktyg (‡1064, ‡1065) kan påverka utfallen avsevärt, inklusive den riskyta som täcks. Omfattande riktlinjer för red-teaming syftar till att hantera en del av dessa utmaningar (‡1066).

###@ Riskminskning

Riskreducering är processen att prioritera, utvärdera och implementera kontroller och motåtgärder för att minska identifierade risker. Exempel är åtkomstkontroller (‡991), kontinuerlig övervakning (‡986) och if-then-åtaganden (‡700). Att reducera risk väcker en central fråga: vilken nivå av risk som är acceptabel? Nya ramverk och företagsriktlinjer har börjat formalisera kriterier för ”riskacceptans” (‡965, ‡1040). Att fastställa lämpliga trösklar förblir dock utmanande, särskilt för risker med omfattande samhällspåverkan (‡986, ‡1067). För närvarande finns det ingen etablerad mekanism för att validera de riskacceptansbeslut som utvecklare fattar före lansering (‡1005).

De riskreducerande metoder som beskrivs i Tabell 3.3 nedan är anpassningsbara och kan mildra en rad risker, inklusive vissa oväntade risker. Tabellen omfattar inte tekniska riskreducerande metoder som adversarial training, innehållsfilter och övervakning av chain-of-thought. Dessa behandlas i §3.3. Tekniska skyddsåtgärder och övervakning, samt genom hela rapporten i avsnitten ”Mitigations” för varje risk i §2. Risks.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Policyer för acceptabel användning
  En policy för acceptabel användning är en uppsättning regler och riktlinjer för ett ansvarsfullt, etiskt och lagligt användande av AI-modeller. Det är vanligt att AI-utvecklare publicerar policyer för acceptabel användning, liksom policyer för förbjuden användning, i samband med nya modellutsläpp (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Åtkomstkontroll / användargranskning
  Åtkomstkontroller inkluderar att använda policyer och regler för att begränsa åtkomst till AI-modeller, data och system baserat på användarroll, attribut och andra villkor för att förhindra obehörig användning, manipulation eller dataintrång. AI-företag inaktiverar ofta konton som påträffas ägna sig åt kriminell verksamhet (‡486) och inkluderar användargranskning samt Know-Your-Customer-kontroller för att säkerställa att modeller endast används av betrodda aktörer (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Beteende-/modellspecifikation
  En specifikation för AI-beteende är ett dokument som definierar hur en AI-modell ska bete sig i olika situationer. Det fungerar som en mall för AI-alignering och säkerhet, och vägleder modellutveckling, träning, utvärdering och utdata. Flera AI-företag använder dokument för modelspecifikationer och gör åtminstone delar av dem offentliga (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kontinuerlig övervakning
  Kontinuerlig övervakning är den pågående, automatiserade processen att observera, analysera och kontrollera AI-system i drift, följa upp deras prestanda och begränsa deras beteende för att säkerställa tillförlitlighet, effektivitet och säkerhet. Det finns många verktyg för kontinuerlig övervakning (‡1073*) samt tekniker för att stödja
AI-obserservability (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb försvar-i-djupet
  Försvar på flera nivåer är idén att flera oberoende och överlappande lager av försvar kan implementeras så att om ett misslyckas, så kommer andra fortfarande att vara effektiva (‡1075, ‡1076). Flera Frontiera AI-säkerhetsramverk hänvisar till det (t.ex. (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ecosystemövervakning
  Det här är processen att övervaka det bredare AI-ekosystemet, inklusive spårning av beräkning och hårdvara, modellens härkomst, datans härkomst och användningsmönster. Den forskningslitteratur som behandlar detta diskuterar sådan övervakning i relation till risker från allmänt tillämpad AI (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Om-då-åtaganden
  If-then-åtaganden är en uppsättning tekniska och organisatoriska protokoll och åtaganden för att hantera risker när AI-modeller blir mer kapabla. Flera AI-utvecklare använder den här typen av åtaganden som en del av sina Frontier AI Safety Frameworks (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Röda linjer eller förbud
  Röda linjer är specifika gränser som uttrycks som förmågor, påverkan eller typer av användning. Konceptet förekommer i offentliga uttalanden och initiativ, såväl som i reglerande förbud (‡1079, ‡1080, ‡1081). Litteraturen noterar också begränsningar med metoder med röda linjer, inklusive utmaningar kring konsensus och verkställbarhet.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Släpp- och distributionsstrategier
  Utgivnings- och distributionsstrategier för allmännyttig AI kan omfatta användning av stegvisa utrullningar eller API-åtkomst så att fler begränsningsalternativ finns tillgängliga i händelse av missbruk eller oväntad skada (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 3.3: Riskhantering för riskreducering i allmän AI-riskhantering
>white|black||9|11|br Exempelmetoder för riskreducering för AI är listade i alfabetisk ordning. Metoderna som ingår är utformade för att stödja riskreducering för många olika risktyper samtidigt, inklusive risker från illvillig användning, risker från fel i funktion och systemrisker. Givet att riskhantering för general-purpose AI fortfarande är i sin linda, kommer inte alla metoder att vara lämpliga för varje AI-utvecklare eller AI-aktör som distribuerar.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Figur 3.5: En “Schweizerost-modell” som illustrerar ett försvar på djupet-tillvägagångssätt
>white|black||9|11|br Flera lager av skydd kan kompensera för brister i enskilda lager. Nuvarande riskhanteringstekniker för AI har brister, men att lägga dem i lager kan ge ett mycket starkare skydd mot risker. Källa: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Försvar-i-djupet- och release-strategier är viktiga skyddsåtgärder

En  “defence-in-depth”-modell kan stödja allmän riskhantering för AI. I detta sammanhang avser “defence-in-depth” en kombination av tekniska, organisatoriska och samhälleliga åtgärder som tillämpas i olika stadier av utveckling och driftsättning (Figur 3.5). Det betyder att skapa lager av oberoende skyddsåtgärder, så att om ett lager fallerar kan andra lager ändå förhindra skada. Ett ofta använt exempel på en defence-in-depth-modell är den uppsättning förebyggande åtgärder som sätts in för att förhindra smittsamma sjukdomar. Vaccin, masker och handtvätt, bland andra åtgärder, kan minska risken för infektion avsevärt i kombination, även om ingen av dessa metoder är 100% effektiv på egen hand (‡1083*). För allmän AI kommer defence-in-depth att omfatta kontroller som inte finns i själva AI-modellen, utan i det bredare ekosystemet. Detta inkluderar (till exempel) kontroller av de material som behövs för att genomföra en biologisk attack, såsom reagenser (‡1084, ‡1085). Däremot handlar defence-in-depth-åtgärder främst om risker som rör olyckor, funktionsfel och illvillig användning, och kan ha mindre betydelse för att hantera systemrisker (se §3.5. Bygga samhällelig motståndskraft).

Ett företags lanserings- och driftsättningsstrategi är en viktig del av riskreducering. Beslut om hur modeller görs tillgängliga för användare kan i betydande grad påverka riskexponeringen (‡1082). Olika alternativ för lansering och driftsättning inkluderar stegvis lansering till begränsade användargrupper, åtkomst via kontrollerade online-tjänster (såsom APIs), samt användning av licensavtal och policyer för acceptabel användning som rättsligt förbjuder vissa skadliga tillämpningar (‡176, ‡1086, ‡1087). §3.4. Öppenviktsmodeller diskuterar mer i detalj hur publicering av modellvikter påverkar risker.

###@ Risk governance

Risk governance är processen genom vilken utvärderingar, beslut och åtgärder inom riskhantering kopplas till en organisations eller annan enhets strategi och mål (‡1088, ‡1089). Tabell 3.4 ger en översikt över vanliga risk governance-tekniker. Som visas i Figur 3.4 kan risk governance förstås som kärnan i riskhantering, eftersom den möjliggör effektiv drift av andra delar inom riskhantering. Den ger ansvarsskyldighet, transparens och tydlighet som stödjer informerade riskhanteringsbeslut. Risk governance kan omfatta metoder som incidentrapportering (‡1090), tilldelning av riskansvar (‡965) och visselblåsarskydd (‡1091). Mer allmänt kan risk governance omfatta vägledning, ramverk, lagstiftning, reglering, nationella och internationella standarder samt utbildnings- och kompetensutvecklingsinsatser. Ett centralt syfte med risk governance är att etablera organisatoriska policyer och mekanismer som klargör hur riskhanteringsansvar fördelas inom en organisation eller annan enhet, för att stödja lämplig tillsyn och ansvarsskyldighet (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dokumentation
  Dokumentationspraxis hjälper till att spåra viktig information om AI-system, såsom träningsdata, designval, avsedda användningsområden, begränsningar och risker. ”Model cards” och ”system cards”, som ger information om hur en AI-modell eller ett AI-system tränades och utvärderades, är exempel på framstående bästa praxis för AI-dokumentation (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Incidentrapportering
  Incidentrapportering är processen att systematiskt dokumentera och dela fall där utveckling eller driftsättning av AI har orsakat direkt eller indirekt skada. Det finns flera plattformar som underlättar incidentrapportering för AI (‡1096, ‡1097), och ramverk för att underlätta mer effektiv incidentrapportering för AI (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskhanteringsramverk
  Riskhanteringsramverk är organisatoriska planer för att minska luckor i risktäckning, samordna olika riskhanteringsaktiviteter och införa kontroller och motvikter. Ramverk som är specifika för allmänna ändamål AI (‡986, ‡1098) hänvisar ofta till de andra åtgärderna som nämns i detta avsnitt.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskregister
  En riskregister är ett arkiv av olika risker, deras prioritering, ägare och åtgärdsplaner för begränsning. Dessa är relativt vanliga i många branscher, inklusive cybersäkerhet (‡1099), och används ibland för att uppfylla krav på regulatorisk efterlevnad.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ansvarsfördelning för risk
  Tilldelningen av roller och ansvarsområden för riskhantering inom en organisation kan strukturera intern granskning av beslutsfattandet (‡1002, ‡1093). Sådana arrangemang återspeglas i vissa styrningsramverk, inklusive EU:s Allmänna uppförandekod för AI för allmänt bruk (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Transparensrapporter
  Transparensrapporter beskriver ett AI-företags riskhanteringspraxis genom att offentligt avslöja viss information eller genom att dela dokumentation med branschorganisationer eller statliga organ. Till exempel lämnar många AI-företag in transparensrapporter för Hiroshima AI Process (HAIP) (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Skyddsordning för visselblåsare
  Eftersom mycket av AI-utvecklingen sker bakom stängda dörrar, inkluderar vissa styrningsramverk skydd för visselblåsare för att möjliggöra att potentiella risker rapporteras till myndigheter (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 3.4: Riskstyrning i riskhantering för allmänändamåls-AI
>white|black||9|11|br Exempelmetoder för AI-riskstyrning listas alfabetiskt. Metoderna som ingår är utformade för att stödja riskstyrning för många olika risktyper samtidigt, inklusive risker från skadlig användning, risker från felmönster och systemrisker. Med tanke på att riskhantering för generativt allmännyttig AI fortfarande är i ett tidigt skede kommer inte alla metoder att vara lämpliga för varje AI-utvecklare eller AI-aktör som driftsätter AI.


>white|orangered|left|14|15.5|bb Dokumentation och transparens är delar av riskstyrning

Dokumentations- och institutionella transparensmekanismer, tillsammans med informationsdelningspraxis, underlättar extern granskning och stödjer insatser för att hantera risker i samband med allmännyttig AI (‡1101, ‡1102). Det har blivit vanlig praxis att publicera resultaten från tester före driftsättning i en ”model card” eller ”system card”, tillsammans med grundläggande uppgifter om modellen eller systemet, inklusive hur det tränades och vilka eventuella begränsningar det har (‡1094, ‡1095). Vissa utvecklare publicerar också transparensrapporter som innehåller mer omfattande uppgifter om deras riskhanteringspraxis (‡1103). Andra delar av dokumentation och transparens omfattar övervakning och incidentrapportering (‡176, ‡1083*, ‡1103) samt informationsdelning, vilket kan underlättas av tredjepartsaktörer som Frontier Model Forum. Vissa regelverksramar, såsom EU AI Act eller Californiens Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53) (‡1081, ‡1104), kräver i vissa fall informationsdelning om risker med allmännyttig AI.

>white|orangered|left|14|15.5|bb Ledarskapsengagemang och incitament formar riskhanteringspraxis

Organisationskultur, ledningsstruktur och incitament påverkar riskhanteringsinsatser på olika sätt (‡1105). Ledningens engagemang och incitamentsstrukturer är ofta relevanta för hur riskhanteringspolicyer fungerar i praktiken. Vissa utvecklare har interna beslutsfattande paneler som överlägger om hur man på ett säkert och ansvarsfullt sätt utformar, utvecklar och granskar nya AI-system. Övervaknings- och rådgivande kommittéer, stiftelser eller AI-etiska nämnder kan också fungera som mekanismer för riskhanteringsvägledning och organisatorisk tillsyn (‡1092*, ‡1106, ‡1107, ‡1108). Forskare har hävdat att utmaningar med frivillig självreglering innebär att extern granskning, verifiering och standardisering kan bidra till att stärka allmän riskhantering för generella AI-system (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Organisatorisk riskhantering, transparens och riskrapporteringsramverk

Flera nya initiativ fokuserar på riskhanteringsprocesser, dokumentation och transparens. I sin nuvarande form fungerar EU:s uppförandekod för allmännyttig AI som en frivillig ram för att vägleda transparens-, upphovsrätts- samt säkerhets- och säkerhetsåtgärdsrutiner för att stödja efterlevnad av EU AI-lagens bestämmelser för allmännyttig AI (‡965). Per december 2025 har mer än två dussin företag† undertecknat. G7:s Hiroshima AI-process (HAIP) rapporteringsram (‡1100) är den första internationella ramen för frivillig offentlig rapportering av organisatoriska riskhanteringsrutiner för avancerade AI-system. Minst 20 utvecklare har publicerat offentliga transparensrapporter som omfattar riskidentifiering, utvärderingsmått, mitigationsstrategier och datorsäkerhetsprocesser.

AI-utvecklare har antagit frivilliga åtaganden om transparens. I Kina släpptes löften från 17 kinesiska AI-företag, samordnade av AI Industry Alliance of China, i december 2024 (‡1113) och uppdaterades 2025 (‡1114). Vid AI Seoul Summit i maj 2024 i Sydkorea undertecknade 16 AI-utvecklare från flera länder frivilliga åtaganden om att publicera Frontier AI Safety Frameworks för sina mest kapabla modeller och system, samt att tillämpa riskhanteringspraxis genom hela utvecklings- och driftsättningsskedena för modeller (‡1052).

    Notera † -- Undertecknare per december 2025 inkluderar: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing, och WRITER.

>white|orangered|left|14|15.5|bb Frontier AI-säkerhetsramverk har blivit ett framträdande organisatoriskt arbetssätt för hantering av AI-risker.

Sedan 2023 har flera ledande utvecklare av AI frivilligt publicerat dokument som beskriver hur de planerar att identifiera och hantera allvarliga risker från sina mest avancerade system. Dessa Frontier AI Safety Frameworks beskriver hur en AI-utvecklare planerar att utvärdera, övervaka och kontrollera sina mest avancerade AI-modeller och system före och under driftsättning. Dessa ramverk har många likheter, men skiljer sig i viktiga avseenden (‡1115, ‡1116). De flesta fokuserar på risker som är förknippade med kemiska, biologiska, radiologiska och nukleära (CBRN) hot, avancerade cyberförmågor och avancerat autonomt beteende (‡1115, ‡1117). En minoritet av ramverken tar upp ytterligare riskdomäner som olaglig diskriminering i stor skala och sexuellt utnyttjande av barn.

Flera utvecklare uppdaterade sina ramverk 2025 och lade till nya avsnitt om skadlig manipulation, felinriktningsrisk och autonom replikering och anpassning (‡1078, ‡1118). Även om många ramverk beskriver liknande metoder för riskhantering – inklusive hotmodellering, rödlagstestning och bedömningar av farliga förmågor – skiljer de sig åt i sina definitioner av risknivåer och trösklar, i hur ofta utvärderingar genomförs, i buffertar mellan utvärderingar och trösklar samt i hur heltäckande deras åtaganden om begränsning är (till exempel om de inkluderar att radera modellvikter eller bara pausar utvecklingen) (‡1115, ‡1119). Se Tabell 3.5 för mer information.

>white|orangered|left|14|15.5|bb Många åtgärder i Frontier AI Safety Frameworks baseras på om-och-sen-åtaganden

En nyckel del i Frontier AI Safety Frameworks är ”if-then-åtaganden”. Dessa är villkorade protokoll som utlöser specifika svar när AI-modeller och system når fördefinierade kapacitetströsklar (‡1120). Till exempel kan ett if-then-åtagande ange att om en modell bedöms ha förmågan att på ett meningsfullt sätt hjälpa noviser att skapa och driftsätta CBRN-vapen, då kommer utvecklaren att införa förstärkta säkerhetsåtgärder, driftsättningskontroller och realtidsövervakning (‡991*).

År 2025 meddelade flera AI-utvecklare att nya modeller utlöste tidiga varningslarm, eller att de inte kunde utesluta möjligheten att ytterligare utvärdering skulle visa att modeller har passerat kapabilitetströsklar. Detta fick dem att tillämpa förstärkta skyddsåtgärder som en försiktighetsåtgärd (‡7, ‡33, ‡1121*). Frontier AI Safety Frameworks kräver ofta en inledande kapabilitetsutvärdering innan riskreducering, samt en kvarvarande riskanalys eller ett säkerhetsfall, ofta informerat av red-teaming, efter riskreducering. Se Tabell 3.5 för detaljerad information.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Beredskapsramverk 2 (‡1078*)
  Risker som omfattas:
1. Biologiska och kemiska förmågor
2. Cybersecurity-förmågor
3. AI:s förbättringsförmåga för sig själv
  Risknivåer eller motsvarande och tillhörande skyddsåtgärder:
- Hög: Kan förstärka befintliga vägar till allvarlig skada (kräver säkerhetskontroller och skyddsåtgärder)
- Kritiskt: Kan introducera tidigare okända nya vägar till allvarlig skada (Stoppa fortsatt utveckling tills angivna skyddsåtgärder och säkerhetskontroller uppfyller en Kritisk standard)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Policy för ansvarsfull skalning 2.2 (‡991*)
  Risker som omfattas:
1. CBRN-vapen
2. Autonom forskning och utveckling av AI (AI R&D)
3. Cyberoperationer (under bedömning)
  Risknivåer eller motsvarande och tillhörande skyddsåtgärder:
  AI-säkerhetsnivåer (ASL)
- ASL-1: Ingen betydande katastrofal risk
- ASL-2: Tidiga tecken på farliga förmågor (Modeller måste uppfylla ASL-2 distributions- och säkerhetsstandarder)
- ASL-3: Avsevärt ökad risk för katastrofal felanvändning (Modeller måste uppfylla ASL-3-implementerings- och/eller säkerhetsstandarderna)
- ASL-4+: Framtida klassificeringar (ännu inte definierade)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Frontier Safety Framework 3.0 (‡1040*)
  Risker som omfattas:
1. Missbruk
    a. CBRN
    b. Cyber
    c. Skadlig manipulation
2. Forskning och utveckling inom maskininlärning
3. Feljustering/ instrumentell resonemang
  Risknivåer eller motsvarande och tillhörande skyddsåtgärder:
  Nivåer för kritisk kapacitet
    Förmågenivåer där, i avsaknad av åtgärder för riskreducering (säkerhetsfall för driftsättningar och säkerhetsåtgärder som är anpassade till RAND säkerhetsnivåerna 2, 3 eller 4 (‡1122)), AI-modeller eller -system kan utgöra en förhöjd risk för allvarlig skada. Förmågenivåerna inkluderar ”tidiga varningsutvärderingar”, med specifika ”varningströsklar”
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Frontier AI Framework 1.1 (‡990*)
  Risker som omfattas:
1. Cybersäkerhet
2. Kemiska och biologiska risker
  Risknivåer eller motsvarande och tillhörande skyddsåtgärder:
  Tröskelnivåer för risk
- Måttlig (släpp med lämpliga säkerhetsåtgärder och riskreduceringar)
- igh (släpp inte)
- Kritisk (stoppa utveckling)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Frontier Model Safety Framework (‡1123*)
  Risker som omfattas:
1. Spridning av CBRN-vapen
2. Offensiva cyberoperationer
3. Automatiserad AI-forskning och utveckling
  Risknivåer eller motsvarande och tillhörande skyddsåtgärder:
  Kritiska funktionsnivåtrösklar
    Modellens kapabiliteter som potentiellt kan orsaka betydande skada för allmänheten om de missbrukas. (Om tröskelvärdena uppnås eller överskrids kommer modellen inte att distribueras offentligt utan lämpliga riskreducerande åtgärder)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Ramverk för gränsöverskridande styrning (‡1124*)
  Risker som omfattas:
1. CBRN-vapen
2. Offensiva cyberoperationer
3. Avancerad autonomi (inklusive AI-forskning och utveckling)
  Risknivåer eller motsvarande och tillhörande skyddsåtgärder:
  Risknivåer
- Låg eller Medel (utplacering tillåten i enlighet med kraven i Program för ansvarsfull AI)
- Hög eller Kritisk (ytterligare granskning och åtgärder)
(krävs)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Bedömning av risker för Frontier AI (‡1029*)
  Risker som omfattas:
1. Cyberbrott
2. CBRN
3. Övertalning och manipulation
4. Olaglig diskriminering i stor skala
  Risknivåer eller motsvarande och tillhörande skyddsåtgärder:
  Risktrösklar – modellrisk (MR)-poäng
- MR1 eller MR2 (Utvärderingsresultat dokumenteras av ingenjörsteam)
- MR3 (riskreducerande åtgärder och utvärderingsresultat dokumenteras av ingenjörsteam och granskas periodvis)
- MR4 (En detaljerad riskbedömning ska genomföras och godkännande från ledare för affärsenheten krävs)
- MR5 (En detaljerad riskbedömning ska genomföras och godkännas av en oberoende kommitté, t.ex. NVIDIA:s kommitté för AI-etik)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Secure AI Frontier Model Framework (‡1125*)
  Risker som omfattas:
1. Skadlig användning (t.ex. skadlig kod, sexuellt utnyttjande av barn)
2. Skada vid vanlig, icke-illvillig användning, t.ex. utdata som leder till ett olagligt diskriminerande utfall eller generering av osäker kod
  Risknivåer eller motsvarande och tillhörande skyddsåtgärder:
  Sannolikhet och allvarlighetsgrad av skada i kontext
- Låg
- Medium
- Hög
- Mycket Hög
    (Riskreducerande åtgärder och säkerhetskontroller finns på plats för alla system och processer; ytterligare åtgärder behöver anpassas till AI-systemet och användningsfallet där en modell distribueras)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: Policy för AGI-redohet (‡1127*)
  Risker som omfattas:
1. Cyberbrott
2. Automatiserad AI-forskning och utveckling
3. Autonom replikering och anpassning
4. Biologiska vapen-bistånd
  Risknivåer eller motsvarande och tillhörande skyddsåtgärder:
  Kritiska funktionsnivåtrösklar
    Kvantitativa tröskelvärden på förmågebedömningar (om de överskrids, genomför farliga förmågeutvärderingar, informationssäkerhetsåtgärder och driftsbegränsningar, eller avbryt utvecklingen)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: AGI Redskapspolicy (‡1127*)
  Risker som omfattas:
1. Cyberbrott
2. Automatiserad AI-forskning och utveckling
3. Autonom replikering och anpassning
4. Biologiska vapen-bistånd
  Risknivåer eller motsvarande samt tillhörande skyddsåtgärder:
  Kritiska funktionsnivåtrösklar
    Kvantitativa tröskelvärden för kapacitetsriktmärken (om de överskrids, genomför farliga kapacitetsutvärderingar, informationssäkerhetsåtgärder och driftsättningsåtgärder, eller avbryt utvecklingen)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: AI-säkerhetsramverk (‡1128*)
  Risker som omfattas:
1. Förlust av kontroll
2. Missbruk (t.ex. biokemisk vapenframställning
  Risknivåer eller motsvarande och tillhörande skyddsåtgärder:
  Risknivåer
- Låg risk (Distribuera AI-system, men utför övervakning efteråt för att hantera risker)
- Risk identifierat (Antingen begränsas åtkomst till öppna AI-system endast till behöriga användare för att minska risker, eller så skjuts driftsättning upp tills ytterligare säkerhetsåtgärder har vidtagits, beroende på användningsfall)
- Hög risk (Distribuera inte AI-system)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Frontier AI Safety Framework (‡1129*)
  Risker som omfattas:
1. Biologiska hot
2. Offensiv cybersäkerhet
3. Autonom drift och avancerad manipulation
  Risknivåer eller motsvarande och tillhörande skyddsåtgärder:
  Risknivåer
- Nivå 1 (Grundläggande skyddsåtgärder för minimala risker och möjlighet till öppen källkodspublicering)
- Nivå 2 (Realtidsövervakning, promptfiltrering, beteendeavvikelsedetektering, åtkomstkontroller, red-teaming och adversarial simuleringar)
- Nivå 3 (Avancerade skyddsåtgärder, inklusive red- teaming, fasade utrullningar, adversariell testning, kryptering, kontroller för flerpartsåtkomst och nolltillit-arkitektur)
- Nivå 4 (Maximala säkerhetsprotokoll för höginsatsmodeller och maximala säkerhetsåtgärder)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 3.5: Ramverk för Frontier AI-säkerhet
>white|black||9|11|br Den första uppsättningen av Frontier AI Safety Frameworks som har släppts av en delmängd av de AI-utvecklare som har signerat Frontier AI Safety Commitments. Ramverken omfattar liknande risker (med smärre variationer) och använder olika risknivåer och riskhanteringsmetoder.


>white|orangered|left|14|15.5|bb Effektiviteten hos Frontier AI Safety Frameworks är osäker

Frontier AI Safety Frameworks kan fungera som verktyg för riskhantering under specifika förutsättningar och för vissa riskkategorier som har en trovärdig väg till skada (‡1117). Samtidigt diskuterar flera analyser frågor om deras tydlighet och omfattning (‡111, ‡986) samt om robustheten i AI-förmåga och risktrösklar (‡1031, ‡1130). Befintliga ramverk tenderar att fokusera på en delmängd av riskdomäner. Som ett resultat får vissa framträdande risker, såsom otillåten övervakning (‡1131, ‡1132) och icke-samtyckesbaserad intim avbildning (‡287), mindre betoning. Till skillnad från riskhanteringsansatser från andra sektorer, såsom flygindustri eller kärnkraft (‡1133*), använder Frontier AI Safety Frameworks typiskt sett inte explicita kvantitativa risktrösklar (‡1134).

Externa bedömningar av utvecklarnas efterlevnad av deras Frontier AI Safety Frameworks hittills är fortfarande begränsade, delvis eftersom de flesta ramverken är nya, offentligt tillgänglig information är knapphändig och det inte finns några standardiserade externa granskningar. Deras effektivitet kommer också att påverkas av hur väl – och i vilken utsträckning – åtaganden genomförs i praktiken. I sig kan dessa ramverk inte säkerställa effektiv riskhantering, eftersom deras praktiska genomslag beror på hur väl och i vilken utsträckning de genomförs. Hittills är de inte fullt ut i linje med internationella standarder för riskhantering (‡1135). En studie av tidigare frivilliga åtaganden fann ojämn uppfyllelse mellan åtgärder, vilket tyder på att efterlevnaden av frivilliga åtaganden sannolikt kommer att variera mellan företag och domäner (‡1109).

Sammantaget representerar Frontier AI Safety Frameworks den mest detaljerade formen av frivillig organisatorisk riskhantering som för närvarande används, men de skiljer sig avsevärt åt i omfattning, tröskelvärden och verkställbarhet.

###@ Regulatoriska och styrningsmässiga initiativ

>white|orangered|left|14|15.5|bb Flera jurisdiktioner har infört lagar med krav på transparens

Flera tidiga reglerande angreppssätt inför lagkrav som är avsedda att öka standardisering och transparens i riskhantering. EU:s AI-förordning, som trädde i kraft 2024, fastställer krav avseende transparens, upphovsrätt och säkerhet för generella AI-modeller. År 2025 publicerades EU:s uppförandekod för AI med allmänna ändamål för att stödja efterlevnaden av dessa skyldigheter genom att ge vägledning om modell-dokumentation och upphovsrätt, samt – för de mest avancerade modellerna – riskhanteringsmetoder såsom utvärderingar, riskbedömning och minimering, informationssäkerhet och rapportering av allvarliga incidenter (‡965).

Andra exempel på nya regulatoriska krav inkluderar Sydkoreas ramlag om utveckling av artificiell intelligens och inrättande av förtroende, som inför krav på ”höginverkande” AI-system inom kritiska sektorer (‡1136), och Californiens SB 53, som fastställer krav på transparens avseende säkerhetsramverk och incidentrapportering (‡1104). Med tanke på hur nyligen dessa krav har införts är det för tidigt att i detalj bedöma hur de kommer att påverka riskhanteringspraxis eller faktiska riskutfall.

>white|orangered|left|14|15.5|bb Bredare initiativ för styrning erbjuder frivillig vägledning

Flera regionala och mellanregionala styrningsramverk beskriver nu gemensamma förväntningar för att hantera risker från generella AI-system genom att tillhandahålla icke-bindande vägledning för beslutsfattare och organisationer. Kinas ramverk för AI-säkerhetsstyrning 2.0, publicerat 2025, ger strukturerad vägledning om riskkategorisering och motåtgärder genom hela AI-utvecklings- och driftsättningsprocessen (‡1137). ASEAN-medlemsstaterna har publicerat ”ASEAN Expanded Guide on AI Governance and Ethics (Generative AI)”, som ger vägledning om styrning och etik för generella AI-system och är avsett att stödja en större policyharmonisering mellan ASEAN-medlemsstaterna (‡1138). Dessutom beskriver expertledda initiativ som Singapore Consensus, utvecklat av AI-forskare från flera länder, forskningsprioriteringar för säkerhet hos generella AI-system inom riskbedömning, utveckling och kontroll (‡690).

###@ Uppdateringar

Sedan publiceringen av den senaste rapporten (January 2025) har riskhanteringsläget för general-purpose AI utvecklats, med publiceringen av nya resurser som EU:s General-Purpose AI Code of Practice, G7 HAIP Reporting Framework, Kinas nationella AI Safety Governance Framework 2.0 samt olika AI-utvecklares Frontier AI Safety Frameworks. Dessa initiativ beskriver tillvägagångssätt och metoder som AI-utvecklare använder för att hantera riskerna i samband med general-purpose AI-system (‡1115). Det finns betydande variation mellan Frontier AI Safety Frameworks och mellan HAIP-ansvarsskyltar för transparens (‡1103), vilket återspeglar skillnader i organisatoriska arbetssätt, riskprioritering och ekosystemets tidiga skede för riskhantering av general-purpose AI. Ett pålitligt ekosystem där olika aktörer inom AI bidrar med kompletterande riskhanteringsmetoder över hela livscykeln kan bidra till en effektiv riskhantering (‡690).

###@ Evidensluckor

Det finns en brist på bevis för: hur man mäter allvarlighetsgrad, förekomst och tidsram för framväxande risker; i vilken utsträckning dessa risker kan mildras i verkliga sammanhang; och hur man effektivt uppmuntrar eller inför att mildrande åtgärder antas av olika aktörer. Mer forskning behövs för att förstå hur vanliga olika risker är och hur mycket de varierar mellan olika regioner i världen, särskilt för regioner som Asien, Afrika och Latinamerika som snabbt digitaliseras. Eftersom AI-modeller ges allt större handlingsutrymme och auktoritet och forskningsläget kring risker med allmännyttig AI utvecklas, kommer riskhanteringsansatser också att behöva utvecklas (‡639, ‡1139).

Vissa riskreducerande åtgärder ökar i popularitet (‡690, ‡956), men mer forskning behövs för att förstå hur robusta riskreduceringar och skyddsåtgärder är i praktiken för olika grupper och AI-aktörer (inklusive små och medelstora företag). Ökad tillgång till data om faktisk driftsättning och användning av modeller är relevant för sådana bedömningar. Vidare varierar riskhanteringsinsatser för närvarande i mycket hög grad mellan ledande AI-företag. Det har hävdats att utvecklarnas incitament inte är väl anpassade till en grundlig riskbedömning och riskhantering (‡934). Det finns fortfarande ett kunskapsgap kring i vilken utsträckning olika frivilliga åtaganden uppfylls, vilka hinder företag stöter på när de fullt ut följer åtagandena, och hur de integrerar Frontier AI Safety Frameworks i bredare rutiner för AI-riskhantering.

###@ Utmaningar för beslutsfattare

Centrala utmaningar inkluderar att avgöra hur man ska prioritera de olika risker som generellt ändamålsenlig AI medför, att tydliggöra vilka aktörer som är bäst positionerade för att mildra dem, och att förstå de incitament och begränsningar som formar deras agerande. Underlag tyder på att beslutsfattare för närvarande har begränsad tillgång till information om hur AI-utvecklare och -användare testar, utvärderar och övervakar framväxande risker, och om effektiviteten hos olika mildringsmetoder (‡1140). Forskare och beslutsfattare har diskuterat transparensinsatser och mer systematisk incidentrapportering som möjliga sätt att informera riskprioritering, främja förtroende och ge incitament till ansvarsfull utveckling (‡957). I praktiken innefattar riskhantering flera aktörer längs AI-värdekedjan – såsom data- och molnleverantörer, modellutvecklare och plattformar för modellhosting – där var och en har skilda möjligheter att bedöma och hantera olika risker (‡1141). Begränsat informationsutbyte mellan dessa aktörer gör det svårt att avgöra vilka risker som är mest sannolika eller mest genomgripande, särskilt när samhälleliga effekter på efterföljande led beaktas.

