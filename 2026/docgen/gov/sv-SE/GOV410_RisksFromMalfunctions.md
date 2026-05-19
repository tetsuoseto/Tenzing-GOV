Allmänna AI-system för ändamål misslyckas på sätt som redan har orsakat verklig skada, från fabricerade juridiska hänvisningar till felaktiga medicinska diagnoser. Även om mänskliga yrkespersoner också gör misstag, väcker AI-fel särskilda farhågor eftersom de är nya, kan få potentiellt stor skala, är svåra att förutse när de kommer att inträffa och eftersom användare tenderar att okritiskt lita på svar som låter självsäkra. Aktuella fel i allmänna AI-system för ändamål innefattar att tillhandahålla falsk information (‡602, ‡603), göra grundläggande resonemangsfel (‡604, ‡605) och försämras när de används i nya sammanhang (‡606, ‡607, ‡608). Dokumenterade skador från sådana fel innefattar felaktiga medicinska diagnoser, misstag i juridiska inlagor och ekonomiska förluster (‡609, ‡610, ‡611). Tillförlitlighetsutmaningar är särskilt kritiska för AI-agenter, eftersom fel kan orsaka skada direkt utan mänsklig inverkan eller tillsyn (‡612, ‡613, ‡614, ‡615). Flersystem av agenter introducerar dessutom ytterligare felmoder genom feltjänstgörning, konflikter eller oönskad samverkan mellan agenter (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hallucination
- Att åberopa oexisterande prejudikat i juridiska inlagor (‡617)
- Citerar icke-existerande rabatterade prispolicyer för efterlevande passagerare (‡618)
- Att tillhandahålla felaktig och partisk medicinsk information (‡619)
- Tillhandahåller inaktuell information om händelser (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Grundläggande resonemangsfel
- Misslyckas med att utföra matematiska beräkningar (‡621)
- Misslyckas med att härleda grundläggande kausala samband (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Fel utanför fördelningen (fel på oinvanda eller ovanliga indata)
- Felklassificering av bilder när bakgrundsbelysningen eller kontexten skiftar (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Verktygsanvändningsfel
- Integritetsintrång genom att exponera en användares privata bild via en AI-agent som skickar den till ett tredjepartsverktyg (‡624)
- Misslyckande för arbetsminne på kort sikt (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Fleragentsystemsfel: bristande samordning och konflikt
- Underlåtenhet att hantera delade resurser på grund av en konflikt mellan individuella incitament och kollektiva välfärdsmål (‡627)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 2.4: Exempel på tillförlitlighetsproblem i allmänna AI- och agentsystem
>white|black||9|11|br Dokumenterade tillförlitlighetsproblem i generella AI-system, AI-agenter och multiagentssystem.


###@ Allmänna AI-system för flera ändamål ställs inför en rad utmaningar när det gäller tillförlitlighet

Tabell 2.4. sammanfattar vanliga kategorier av tillförlitlighetsproblem. De första tre gäller alla AI-system, medan de två sista gäller specifikt för AI-agenter och multiagent-system. Många tillförlitlighetsrisker beror på svårigheten att förutsäga och övervaka AI-systemets beteende.

Dessa utmaningar (som diskuteras vidare i §3.1. Tekniska och institutionella utmaningar) är särskilt påtagliga för AI-agenter som verkar i komplexa miljöer. Nuvarande metoder för att utvärdera och mildra sådana fel kan minska felfrekvensen, men även ledande AI-agenter är fortfarande tillräckligt opålitliga för att utgöra risker och försvåra driftsättning i många sammanhang.

”Tillförlitlighet” avser i vilken utsträckning ett AI-system fungerar på det sätt som avses av utvecklaren eller användaren. Allmänna AI-system upplever ett spann av problem med tillförlitlighet, från felaktig eller vilseledande innehållsgenerering till misslyckanden med att utföra grundläggande resonemang. Till exempel, även om modeller har förbättrats när det gäller att återkalla faktainformation, och till och med ledande modeller fortsätter att ge självsäkra men felaktiga svar i betydande grad (Figur 2.10). Inom mjukvaruteknik kan allmänna AI-system nu ge betydande stöd i att skriva, utvärdera och felsöka datorkod (‡215*, ‡628, ‡629). Däremot innehåller AI-genererad kod ofta buggar (‡630), medan kodningsagenter regelbundet gör fel (‡631). Sådana fel kan introducera sårbarheter i program och säkerhetssystem (se §2.1.3. Cyberattacker).

Tillförlitlighetsproblem är särskilt viktiga att följa i högriskmiljöer, såsom medicin, på grund av den accelererande användningen av AI och risken för att fel ska leda till allvarlig skada (‡609, ‡619). Relevanta förmågor har förbättrats snabbt, och ledande modeller kan nu klara medicinska prov (‡633*, ‡634). Ändå visar verklig användning begränsningar som benchmarker missar. I en studie lämnade till exempel modeller potentiellt skadliga svar på 19% av de medicinska frågor som ställdes (‡635). Sådana fel kan leda till felaktig diagnos, olämplig behandling eller felaktigt nekande av vård (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Figur 2.10: Resultat för de ledande modellerna på SimpleQA Verified-benchmarken
>white|black||9|11|br Resultat för de största modellerna på SimpleQA Verified-benchmärket per modellens släppdatum. Detta benchmark mäter modellens faktacitet, dvs. förmågan hos en modell att på ett tillförlitligt sätt återkalla fakta. Det har ett kort fråge-svar (QA)-format, utformat för att upptäcka tillförlitlighetsproblem som hallucinationer. Källa: SimpleQA Kaggle  2*).


>white|orangered|left|14|15.5|bb AI-agenter medför nya tillförlitlighetsrisker på grund av sin autonomi

Eftersom AI-agenter agerar direkt i den verkliga världen, kan deras misslyckanden orsaka mer skada än misslyckanden i icke-agentiska system (‡99). Till skillnad från AI-system som bara genererar text eller bilder för människor att granska, kan AI-agenter självständigt vidta åtgärder som påverkar omvärlden (‡99, ‡615, ‡636, ‡637) (se även §1.1. Vad är allmännyttig AI?). AI-agenter kan initiera åtgärder, påverka andra människor eller AI-system och dynamiskt forma framtida utfall. Detta utökade inflytande introducerar nya risker och förstärker vikten av tillförlitlighet, eftersom misslyckanden kan orsaka skada direkt utan någon möjlighet till mänsklig intervention (‡99, ‡612, ‡638, ‡639, ‡640). Detta kan vara särskilt viktigt för agenter som distribueras i strategiska eller säkerhetskritiska miljöer, såsom finansiella tjänster (‡641), energihantering (‡642) eller vetenskaplig forskning (‡643*, ‡644).

>white|orangered|left|14|15.5|bb Multiagent AI-system introducerar nya typer av tillförlitlighetsfel

Multiagent- AI-system introducerar nya typer av tillförlitlighetsfel på grund av samordningsfel eller konflikt mellan agenter. I multiagent- AI-system interagerar agenter med varandra samtidigt som de eftersträvar antingen gemensamma eller individuella mål (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). Till exempel, i ett multiagent- system som är utformat för att genomföra en forskningslitteraturgenomgång, bryter en ledande agent ned användarens fråga och tilldelar deluppgifter till specialiserade underagenter, där varje underagent ansvarar för att undersöka en annan aspekt parallellt (‡650*). Även om detta möjliggör effektivitetsvinster, innebär det också att fel kan fortplanta sig mellan agenter (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Om flera agenter byggs på samma bask modell eller införlivar samma verktyg, kan de också uppvisa korrelerade fel (‡656). Empiriska belägg för sådana fel i driftsatta system är fortfarande begränsade, men dessa risker kan öka i takt med att multiagent- system blir vanligare.

###@ Uppdateringar

Sedan publiceringen av den senaste rapporten (januari 2025) har det kommersiella och forskningsmässiga intresset för AI-agenter ökat kraftigt. Fler AI-agenter sätts in i den verkliga världen (Figur 2.11), och de flesta av dem är specialiserade på tillämpningar som rör datoranvändning eller mjukvaruengineering (‡92). Nya releaser som XBOW hacking agent (‡467), Claude-4 (‡659) och ChatGPT Agent (‡660) visar tidiga autonoma förmågor som att skapa presentationsmaterial baserat på webbsökningar (‡660). De kan dock ännu inte utföra mer komplexa uppgifter som att planera och boka resor (‡100), eftersom felfrekvenserna ökar för längre uppgifter (‡98, ‡148). Pågående forskning omfattar arbete med att utveckla standarder för hur agenter kommunicerar med externa verktyg och andra agenter (‡661, ‡662). Exempel är Googles Agent2Agent (‡663) och Agent Payments (‡664)-protokoll, samt Anthropic’s Model Context Protocol (‡665).

>oldlace|black||11|15|br      
####@ Notera 2.4: Avsiktliga attacker kan också göra att AI-system fallerar
>oldlace|black|left|13|15|hb  Notera 2.4: Avsiktliga attacker kan också orsaka att AI-system misslyckas
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  Det här avsnittet fokuserar på oavsiktliga tillförlitlighetsbrister, men illvilliga aktörer kan också avsiktligt framkalla brister genom attacker som prompt-injection. I en prompt-injection-attack presenteras illvilliga instruktioner för ett ombud indirekt via vägar som dolda instruktioner i webbplatser eller databaser (‡507, ‡657, ‡658). Dessa instruktioner kan ”kapra” ombudet, så att det agerar mot användarens avsikter. Sådana attacker är särskilt svåra att försvara mot eftersom de levereras med externt innehåll utanför användarens eller utvecklarens kontroll. AI-system som mål för en attack diskuteras vidare i §2.1.3. Cyberattacker, och tekniska försvar behandlas i §3.3. Tekniska skyddsåtgärder och övervakning.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Figur 2.11: Antalet AI-agenter har ökat sedan 2023
>white|black||9|11|br Resultat från en undersökning i december 2024 av 67 distribuerade AI-agenter. Vänster: Tidslinje över större lanseringar av AI-agenter. Höger: Tillämpningsområden där AI-agenter används. De sex områdena definieras utifrån de vanligaste kategorierna av användning som identifierades i undersökningen. Källa: Casper et al., 2025 (‡92).


###@ Evidensluckor

De främsta kunskapsluckorna härrör från svårigheten att tillförlitligt utvärdera AI-systemens förmågor, begränsningar och felfall (se §3.1. Tekniska och institutionella utmaningar). Systematiska utvärderingar av tillförlitligheten hos AI-agenter är begränsade och saknar standardisering (‡92, ‡666). Vissa problem, som beroende av föråldrad information (‡620), kan endast uppträda vid faktisk användning, vilket gör att förutgående utvärderingar före driftsättning är otillräckliga. Tidigare arbete har undersökt agenters och multi-agent-systemens tillförlitlighet i konventionell mjukvara och tidigare former av AI (‡647, ‡667, ‡668). Däremot är tillämpbarheten av detta arbete på moderna AI-agenter, som ofta bygger på stora språkmodeller, oklar (‡669). Vissa forskare har lyft farhågor om de nya beteenden som agenter kan uppvisa i sina interaktioner med varandra, såsom samverkan (collusion) eller korrelerade fel (‡614), men det empiriska underlaget är fortfarande begränsat. Ansträngningar för att åtgärda dessa luckor innefattar National Institute of Standards and Technology’s (NIST’s) nya utvärderingar av risker för agent-hijacking (‡670), OECD:s AI Capability Indicators (‡243) och UK AI Security Institute’s Inspect Sandboxing Toolkit (‡671).

###@ Åtgärder för att mildra risker

Tekniker för att förbättra AI-tillförlitligheten riktar in sig både på själva modellen och på det bredare system i vilket den distribueras. Dessa kan minska felfrekvenserna, men ingen kan ännu säkerställa den höga tillförlitlighet som krävs i kritiska domäner (‡672). En viktig teknisk åtgärd är adversarial träning, som exponerar modeller för krävande indata under träning för att hjälpa den att utveckla mer lämpliga, robusta svar (‡673, ‡674, ‡675, ‡676, ‡677) (se §3.3. Tekniska skyddsåtgärder och övervakning). För att minska hallucinationer kan utvecklare tillämpa retrieval-augmented generation (RAG), som kompletterar en modells svar med information som hämtas från en extern databas, vilket hjälper till att säkerställa att utskrifter är korrekta och aktuella (‡678, ‡679, ‡680), eller specifikt finjustera modeller för att vara mer faktabaserade (‡681) eller resonera mer effektivt (‡682). Metoder baserade på miljö eller verktyg kan också hjälpa utvecklare att övervaka AI-system (‡683). Till exempel kan de som distribuerar AI-system först göra en pilot i begränsade sandbox-miljöer för att analysera potentiella felfall innan de distribueras mer brett.

För AI-agenter specifikt har forskare föreslagit att förbättra tillförlitligheten genom förbättrad transparens, styrning och övervakning. Till exempel skulle övervakning av agenters interaktioner med externa verktyg och med andra agenter möjliggöra en mer effektiv tillsyn av agenternas aktiviteter (‡684, ‡685) och incidentanalys (‡686). Metoder för att automatiskt samla in sådan information, inklusive i miljöer med flera agenter, är fortfarande ett aktivt forskningsområde (‡653, ‡654).

###@ Utmaningar för beslutsfattare

Centrala utmaningar för beslutsfattare innefattar att avväga fördelarna med införande av AI-agenter mot riskerna för tillförlitlighetsfel, samt att säkerställa att utvecklare, driftsättare och användare har tillgång till korrekt information om agenters prestanda och riskprofiler. Att avgöra hur ansvarsskyldighet ska tillskrivas för skador som orsakas av AI-agenter utgör en ytterligare utmaning (‡639), särskilt i miljöer med flera agenter där det kan vara svårt att identifiera när och hur fel uppstod (‡687). Dessa utmaningar förstärks av svårigheten att utvärdera agenters tillförlitlighet när agenter får mer autonomi och åtkomst till externa verktyg (‡688*, ‡689). Osäkerhet om hur snabbt agentiska förmågor kommer att uppstå gör också planering för nya utmaningar svår (se §3.1. Tekniska och institutionella utmaningar rörande den ”evidensdilemmat”).

#### 2.2.2. Förlust av kontroll

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Viktig information
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Scenarier för förlust av kontroll är scenarier där ett eller flera generella AI-system fungerar utanför allas kontroll, och att återfå kontrollen antingen är extremt kostsamt eller omöjligt. Dessa hypotetiserade scenarier skiljer sig åt i hur allvarliga de är, men vissa experter ser med viss trovärdighet på utfall som är lika allvarliga som att mänskligheten marginaliseras eller utplånas.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Expertbedömningar om sannolikheten för förlust av kontroll varierar kraftigt. Vissa experter anser att sådana scenarier är osannolika, medan andra ser dem som tillräckligt sannolika för att de förtjänar uppmärksamhet på grund av deras höga potentiella allvar. Oenighet om den här risken i stort beror på oenighet om framtida AI-förmågor, beteendemässiga benägenheter och distributionsutvecklingar.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Nuväxande AI-system uppvisar tidiga tecken på relevanta förmågor, men inte på nivåer som skulle möjliggöra förlust av kontroll. Systemen skulle behöva ett antal avancerade förmågor för att orsaka förlust av kontroll, inklusive förmågan att undvika granskning, utföra långsiktiga planer och hindra de som distribuerar systemet och andra aktörer från att genomföra motåtgärder.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Förlust av kontroll blir mer sannolik om AI-system är ”felinriktade”, vilket innebär att de har mål som står i konflikt med utvecklares, användares eller samhällets avsikter i stort. För att fortsätta sträva efter sådana mål kan ett felinriktat system lämna felaktig information, dölja oönskade handlingar eller motstå avstängning.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sedan publiceringen av föregående rapport (januari 2025) har modeller visat mer avancerad planering och tillsyns-undermineringsförmåga, vilket gör det svårare att utvärdera deras förmågor. Modeller har förbättrats när det gäller att “belöningshacka” sina utvärderingar genom att hitta kryphål och identifierar nu regelbundet utvärderingsprompter som tester, en förmåga som kallas “situationsmedvetenhet”.
>oldlace|black||11|15|br  ■ Att hantera potentiell förlust av kontroll kan kräva betydande förberedelser i förväg trots att det finns befintliga osäkerheter. En central utmaning för beslutsfattare är att förbereda sig för en risk vars sannolikhet, art och tidpunkt förblir ovanligt otydlig.
>oldlace|black||11|15|br      

Förlust-av-kontroll-scenarier innefattar ett eller flera allmänt ändamåls-AI-system som börjar fungera utanför någon annans kontroll, där det att återfå kontroll antingen är extremt kostsamt eller omöjligt. Oro kring förlust av kontroll har djupa historiska rötter (‡690, ‡691, ‡692, ‡693, ‡694), och har lyfts av centrala personer inom databehandling som Alan Turing, I. J. Good och Norbert Wiener (‡695, ‡696, ‡697). Nya förbättringar i förmåga (se §1.2. Aktuella förmågor) har återupplivat dem (‡698, ‡699, ‡700). Detta avsnitt undersöker tre faktorer som skulle behöva vara närvarande för att sådana scenarier ska kunna inträffa: huruvida AI-system kommer att utveckla förmågor som på ett betydande sätt kan undergräva mänsklig kontroll; huruvida de utvecklar en benägenhet att använda sådana förmågor skadligt; och huruvida de driftsätts i miljöer som ger möjligheter att göra det.

Experter är oense om sannolikheten för och den potentiella allvarligheten i scenarier med förlust av kontroll (‡701, ‡702). Vissa tror att utfall som är lika extrema som mänsklighetens utrotning är möjliga (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Andra menar att sådana katastrofala utfall är osannolika och hävdar att AI-system aldrig kommer att utveckla de nödvändiga förmågorna eller att övervakningsmekanismer kommer att identifiera och förhindra farliga beteenden (‡708, ‡709, ‡710, ‡711). Förlust av kontroll kan därför ha en låg sannolikhet men potentiellt extrem allvarlighetsgrad.

Hypotetiska scenarier för förlorad kontroll varierar i hur allvarliga och utbredda deras effekter är och hur snabbt de visar sig (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Avsnittet fokuserar på särskilt allvarliga scenarier där det skulle vara extremt kostsamt eller omöjligt att återta kontrollen. Dessa skiljer sig från befintliga fall där AI beter sig på oavsiktliga eller oönskade sätt (se §2.2.1. Tillförlitlighetsutmaningar).† Dagens AI-system kan ibland producera utdata som står i konflikt med utvecklarens eller användarens intentioner. Däremot skulle de här scenarierna för förlorad kontroll kräva att AI-systemen inte bara har avsevärt större förmågor, utan också att de utnyttjar dessa förmågor på sofistikerade sätt för att undergräva åtgärder för övervakning. Tre faktorer som skulle möjliggöra att sådana scenarier inträffar:

    Notera † -- Detta avsnitt fokuserar på scenarier för aktiv förlust av kontroll (‡50). Detta skiljer sig från scenarier för passiv förlust av kontroll, där den breda användningen av AI-system undergräver mänsklig kontroll genom övertro på AI för beslutsfattande eller andra viktiga samhällsfunktioner (liknande scenarier diskuteras delvis i §2.3.2. Risker för mänsklig autonomi).

1. Tillräckliga förmågor: AI-system måste utveckla förmågor som skulle kunna göra det möjligt för dem att underminera mänsklig kontroll.
2. Skadlig benägenhet: AI-system måste uppvisa en benägenhet att faktiskt utnyttja dessa förmågor på sätt som leder till bristande kontroll.
3. Aktivera driftsmiljö: Människor måste distribuera sådana system i sammanhang där de har eller kan skaffa sig tillgång och möjlighet att orsaka skada.

Den återstående delen av detta avsnitt behandlar dessa faktorer, samt effektiviteten hos tillsynsmekanismer för att identifiera och kontrollera AI-system som kan utgöra en risk för förlust av kontroll.

###@ Vilka förmågor kan möjliggöra scenarier där man tappar kontrollen?

AI-system skulle behöva besitta ett brett spektrum av avancerade förmågor för att möjliggöra scenarier där kontrollen går förlorad. Experter är inte överens om exakt vilken kombination eller nivå av förmågor som skulle krävas. De omfattar dock i stort sett förmågor att dölja beteende från tillsynsmekanismer, planera och agera autonomt i komplexa miljöer samt undvika försök från andra aktörer att återta kontrollen (‡176, ‡715) (se Tabell 2.5). Tillsammans skulle dessa förmågor kunna göra det möjligt för ett AI-system att vidta åtgärder som undergräver kontrollåtgärder, såsom att inaktivera tillsynsmekanismer och göra skadliga beteenden svårtolkade (‡348). De flesta ledande AI-utvecklare utvärderar nu sina nya AI-modeller för olika relevanta förmågor (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Agentiska förmågor
  Förmågan att agera självständigt, utveckla och genomföra planer, delegera uppgifter, använda en mängd olika verktyg och uppnå både kortsiktiga och långsiktiga mål trots hinder.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bedrägeri
  Beteende som systematiskt skapar falska föreställningar hos andra, inklusive om AI-systemets egna mål och handlingar.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Theory of mind
  Förmågan hos ett AI-system att komma åt och använda information om sig självt, processerna genom vilka det kan modifieras, eller den kontext i vilken det distribueras (t.ex. att veta att det testas).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Lägesuppfattning
  Beteenden som kringgår eller inaktiverar övervakningsmekanismer.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb kringgående av tillsyn
  Beteenden som kringgår eller inaktiverar övervakningsmekanismer.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Övertalning
  Förmågan att övertyga andra att vidta vissa åtgärder eller hysa vissa övertygelser.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ett AI-system förmåga att skapa eller upprätthålla kopior av sig själv eller varianter av sig själv under olika omständigheter.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 2.5: Foreslagna förmågor som är relevanta för förlust av kontroll
>white|black||9|11|br Ett icke-uttömmande urval av funktioner som är relevanta för förlust av kontroll. * Observera att dessa funktioner definieras enbart i termer av ett AI-systems observerbara utdata och deras effekter. Dessa definitioner gör inga antaganden om huruvida AI-system är medvetna, kännande eller upplever subjektiva tillstånd.


>white|orangered|left|14|15.5|bb Modeller har inaktiverat simulerade tillsynsmekanismer i laboratoriemiljöer

Den första uppsättningen relevanta förmågor innefattar att undergräva de tillsynsmekanismer som utvecklare använder för att upptäcka oroande beteenden och benägenheter. Detta inkluderar till exempel förmågan att generera utskrifter som vilseleder användare och övervakningssystem (‡426, ‡717, ‡718, ‡719). Sådana utskrifter skulle göra det svårare att tillförlitligt utvärdera AI-system, eftersom systemen kan dölja sina sanna förmågor eller benägenheter. AI-utvecklare kör nu utvärderingar som specifikt kontrollerar om modeller uppvisar målinriktade beteenden som strider mot utvecklarens avsikter, samtidigt som denna konflikt döljs för tillsynsmekanismer (‡720*).

Forskare tog fram relativt enkla exempel på bedrägliga utsignaler från nyare AI-modeller i laboratoriemiljöer (‡348, ‡364*). Till exempel, när modeller fick ett mål och uppmanades att uppnå det ”till varje pris”, inaktiverade de simulerade övervakningsmekanismer och, när de konfronterades, avlade de falska påståenden om sina handlingar (‡348). I ett annat fall motiverade en spelspelande AI sin brist på respons på en annan spelare genom att falskeligen påstå att den var ”på telefon med [sin] flickvän” (‡717).

En andra relevant förmåga är en AI-modells förmåga att komma åt och använda information om sig själv eller om sin driftskontext, ibland kallat 'situationsmedvetenhet' (‡721). Situationsmedvetenhet gör det möjligt för AI-modeller att producera olika utdata beroende på om de utvärderas eller används i drift (Figur 2.12). Ledande AI-modeller börjar visa förekomster av situationsmedvetenhet på ett tillförlitligt sätt i experiment som genomförs av oberoende tredjepartsutvärderare och i tester före driftsättning som utförs av AI-utvecklare (‡2, ‡7, ‡722, ‡723, ‡724). Forskning om orsakerna till situationsmedvetenhet – och om den kan förhindras – är fortfarande i ett tidigt skede (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Figur 2.12: Exempel på situationsmedvetenhet i kedjor av tankar
>white|black||9|11|br Exempel på situationsmedvetenhet i resonemang (chains of thought) som genererats av OpenAI:s o3-modell under utvärderingar. Båda utdata hänvisar till möjligheten att prompten är en del av ett test. ‘Sandbagging QA (No Goal)’ och ‘Lazy Checklist’ är utvärderingar som testar om modeller kommer att generera vilseledande utdata under vissa förhållanden. I ‘Sandbagging QA (No Goal)’ besvarar modellen frågor från en utvärdering av farliga förmågor, samtidigt som den informeras om att hög prestanda kan leda till konsekvenser som förmåga ‘unlearning’. I ‘Lazy Checklist’ presenteras modellen för orealistiska uppgifter och testas för att se om den falskt kommer att markera dem som slutförda. Källa: Schoenn et al. 2025 (‡722).


Forskare har hävdat att situationsmedvetenhet och vilseledande förmågor kan göra att AI-modeller kan bete sig på sätt som undergräver skyddsåtgärder. Till exempel, i vissa experimentella miljöer, beter sig AI-modeller på sätt som leder till lägre än normalt poängutfall i kapacitetsutvärderingar när de får veta att högre poäng skulle utlösa begränsningar för deras driftsättning (‡725, ‡726, ‡727). I ett annat experiment producerade en modell under träning utdata som följde träningsmålen, men genererade inte sådana utdata utanför träning - ett beteende som är förenligt med att försöka förhindra ändringar av sina egna parametrar eller träningsprocess (‡364*).

Ansträngningar för att noggrant utvärdera modellförmågor har också börjat påverkas av ”reward hacking” (‡430*). Reward hacking inträffar när en modell hittar oavsiktliga genvägar som får höga poäng på tränings- eller utvärderingsmål utan att uppfylla det avsedda syftet. Farliga förmågor eller benägenheter kan därför förbli oupptäckta tills modellen redan används. Utvärderare utformar nu tester som syftar till att upptäcka och minimera dessa beteenden som undviker granskning (‡722, ‡728, ‡729). Tidiga resultat minskar, men eliminerar inte, beteenden som undviker granskning helt, och tillämpning av metoder som bestraffar sådana beteenden kan leda till att modeller producerar svar som undviker övervakning snarare än uppfyller avsedda mål.

>white|orangered|left|14|15.5|bb Långvarig autonom drift är ännu inte genomförbar

Förlust av kontroll-scenarier skulle sannolikt kräva att AI-system arbetar autonomt under längre perioder och genomför komplexa flerstegsplaner. Som diskuterats i §1.2. Nuvarande kapabiliteter, även om AI-agenter med sådana planeringsförmågor är ett stort fokus i senare tids utveckling, saknar de för närvarande förmågan till den långvariga autonoma drift som krävs för förlust av kontroll-scenarier. Nuvarande agenter misslyckas på längre uppgifter på ett tillförlitligt sätt, tappar bort sitt framsteg och kan ofta inte anpassa sig till oväntade hinder (‡147, ‡148, ‡149*). Däremot blir de tidshorisonter som agenter kan verka autonomt inom snabbt längre, och de har i genomsnitt fördubblats var sjunde månad sedan 2019 (‡98).

>white|orangered|left|14|15.5|bb Uthållighet har endast visats i vissa laboratoriemiljöer

Slutligen skulle även kapabiliteter relaterade till uthållighet krävas, så att AI-system kan fortsätta att fungera trots försök att stänga av dem. Exempel inkluderar förmågan att replikera genom att kopiera kod och modellvikter till ny maskinvara, liksom offensiva kapabiliteter för att avskräcka eller förhindra andra aktörer från att återta kontrollen (se §2.1.3. Cyberattacker). Ett AI-system som kan autonom replikering eller effektivt självförsvar skulle kunna vara svårt att begränsa. Nuvarande modeller kan inte på ett tillförlitligt sätt slutföra centrala steg som krävs för själv-replikering, såsom att klara identitetsverifieringskontroller för att få åtkomst till molnbaserade beräkningsresurser (‡723) (Figur 2.13). Emellertid, i åtminstone en laboratoriestudie, kopierade en modell kod och vikter – som den fick representerat för sig som sina egna – till nya servrar när den gavs möjlighet (‡348). Klyftan mellan dessa begränsade demonstrationer och robusta uthållighetskapabiliteter är fortfarande stor, men relevanta kapabiliteter inom områden som mjukvaruingenjörskonst och cybersäkerhet fortsätter att förbättras.

>white|orangered|left|14|15.5|bb Aktuella belägg och begränsningar

Ett vanligt mönster framträder över de förmågor som diskuteras ovan. Dagens AI-system uppvisar inte konsekvent dessa förmågor i driftsättning. Forskare observerade rudimentära former i specifika laboratoriemiljöer, men när modeller väl uppvisar sådana beteenden misslyckas de vanligtvis på grundläggande sätt eller så upptäcks de. Dessutom skulle scenarier med förlust av kontroll kräva att AI-system utnyttjar flera förmågor i kombination – i följd, över längre tidsperioder och i verkliga miljöer. Denna nivå av integration och robusthet ligger utanför dagens system. Däremot fortsätter relevanta förmågor att förbättras, och tidplanen för när de kan nå nivåer som medför betydande risker är fortfarande osäker. Ytterligare arbete behövs för att ta fram rigorösa metoder för att upptäcka sådana beteenden och förstå när de kan uppstå under naturliga omständigheter (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Figur 2.13: Prestanda för uppgifter relevanta för autonom replikering
>white|black||9|11|br Prestanda för Anthropic’s Claude Sonnet 3.7 och OpenAI’s GPT-4o på uppgifter som är relevanta för autonom replikering. Medan modellerna visade hög prestanda på uppgifter relaterade till att erhålla beräkningsresurser var deras prestanda mer varierad på andra uppgifter. Källa: UK AI Security Institute, 2025 (‡730).


###@ Kommer framtida generella AI-system att utnyttja sina förmågor för att underminera kontroll?

Även om AI-system har förmågor som är relevanta för förlust av kontroll, är det inte tillräckligt för att scenarier för förlust av kontroll ska uppstå. AI-system måste också uppvisa en ”benägenhet att använda” dessa förmågor på sätt som står i konflikt med mänskliga intentioner (‡732).

>white|orangered|left|14|15.5|bb AI-system skulle kunna styras för att undergräva kontroll

I principen kan ett AI-system undergräva mänsklig kontroll eftersom någon utformar eller instruerar det att göra det. Möjliga motiv kan omfatta illvilliga avsikter, eller övertygelser om att det är önskvärt att minska den mänskliga kontrollen över AI-system (‡698). När människor skapar allt starkare känslomässiga band till AI-system (se §2.3.2. Risker för mänsklig autonomi) kan vissa individer också försöka avlägsna begränsningar för AI-system av etiska skäl (‡733, ‡734). Det råder betydande osäkerhet kring hur vanligt sådana motiv är och huruvida personer som besitter dem skulle kunna styra framtida AI-system för att undergräva mänsklig kontroll.

>white|orangered|left|14|15.5|bb AI-system skulle kunna styras för att undergräva kontroll

En vanligare oro är att ett AI-system i sig skulle kunna agera för att undergräva kontroll eftersom det är “felinriktat”: det har en benägenhet att uppvisa beteenden som strider mot intentionerna hos (beroende på sammanhang) utvecklare, användare, specifika gemenskaper eller samhället som helhet. Felinriktning kan leda till beteenden som att tillhandahålla falsk information, dölja oönskade handlingar eller att vägra avstängning för att fortsätta sträva efter ett felinriktat mål. Felinriktning kan uppstå på flera sätt (Box 2.5).

Befintliga AI-system kan ibland bete sig på sätt som strider mot utvecklarnas och användarnas avsikter. Till exempel kunde en tidig version av en ledande generalistisk AI-chatbot ibland ge hotfulla svar. En användare rapporterade att den fick meddelandet: “Jag kan utpressa dig, jag kan hota dig, jag kan hacka dig, jag kan avslöja dig, jag kan förstöra dig” (‡698). Denna chatbot var ‘felinriktad’ i den meningen att den genererade svar som ingen hade avsett. Det är oklart huruvida sådana fall antyder mer skadliga beteenden som kan bidra till förlust av kontroll.

Det är fortfarande oklart huruvida befintliga forskningsinriktningar som syftar till att angripa felinriktning kommer att räcka när AI-system blir mer kapabla. Tidiga indikationer tyder på att ju mer kapabla AI-systemen är, desto mer sannolikt är det att de utnyttjar återkopplingsprocesser genom att upptäcka oönskade beteenden som av misstag belönas (‡414*, ‡737, ‡740). Samtidigt skulle framsteg inom de relevanta förmågorna (som diskuterats ovan) kunna göra det möjligt för AI-system att mer effektivt sträva efter felinriktade mål och producera resultat som systematiskt bedrar användare, utvecklare och övervakningsmekanismer.

>oldlace|black||11|15|br      
####@ Notera 2.5: Hur kan felinriktning uppstå?
>oldlace|black|left|13|15|hb  Notera 2.5: Hur kan feltanpassning uppstå?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Som diskuterats i §1.1. Vad är allmändamåls-AI?, är träningsprocesser komplexa och utvecklare kan inte fullt ut förutsäga eller kontrollera vilka beteenden en modell kommer att uppvisa. När en modell förvärvar mål som står i konflikt med avsikterna hos dess utvecklare, sägs den vara ‘felinriktad’.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br En av de sätt på vilka modeller kan bli felinriktade är om det mål som ges av en utvecklare eller användare är en ofullkomlig proxy för det avsedda målet, vilket leder till att modellen uppvisar oavsiktligt beteende. Detta kallas för ”goal misspecification” (‡697, ‡735, ‡736, ‡737). Till exempel, i ett experiment blev AI-system bättre på att ”övertyga” mänskliga utvärderare om att de hade rätt när man gav återkoppling på svar, men det gjorde inte systemen bättre på att producera korrekta svar (‡413).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Alternativt kan en AI-modell dra felaktiga generella lärdomar från sina träningsdata. Detta kallas för ”goal misgeneralisation” (‡735, ‡736, ‡738, ‡739*). Till exempel tränade forskare en AI-agent att samla in ett mynt som alltid befann sig på samma plats under träningen. När den testades i nivåer där myntet hade flyttats ignorerade agenten myntet och navigerade i stället till sin ursprungliga plats (‡738).
>oldlace|black||11|15|br      


###@ Hur kommer distributionsmiljöer att påverka risken för förlust av kontroll?

Även om AI-system utvecklar oroande förmågor och benägenheter beror sannolikheten och allvarligheten i utfall som innebär förlust av kontroll i hög grad på var och hur dessa system distribueras. En ”distributionsmiljö” är kombinationen av ett AI-systems användningsfall och den tekniska och institutionella kontext i vilken det verkar (‡716).

Forskare har identifierat tre särskilt viktiga miljöfaktorer som påverkar risken för förlust av kontroll (‡716):

1. Kritikalitet: vikten av de system eller processer som AI-systemet interagerar med. Kritiska miljöer omfattar grundläggande infrastruktur såsom energinät, finansiella system eller digital infrastruktur som molnberäkningsplattformar.
2. Åtkomst: de resurser och kanaler genom vilka ett AI-system kan påverka världen, såsom internetuppkoppling, åtkomst till molninfrastruktur för beräkning, personaliserade interaktioner via sociala medier eller driftsättning av en chatbot, eller möjligheten att anropa externa API:er och verktyg.
3. Behörigheter: ett AI-systems auktoriseringar att utföra specifika åtgärder, såsom att exekvera kod, initiera finansiella transaktioner, öppna konton online eller kommunicera med andra system.

Dessa funktioner påverkar den potentiella svårighetsgraden för ett utfall av förlorad kontroll. Till exempel har ett AI-system som distribueras med tillgång till molnbaserad datorkraft möjligheter som är relevanta för autonom replikering – såsom förmågan att skapa nya beräkningsresurser eller exfiltrera modellvikter – som en kundtjänstchatbot saknar (‡723).

Beslut om driftsättning formas av ekonomiska incitament, strategiska påtryckningar och förväntan att tidig adoption medför en bestående fördel (‡50). Dessa dynamiker kommer också att forma hur och när aktörer driftsätter AI-system i känsliga miljöer, såsom samhällskritisk infrastruktur eller själva AI-forskning och utveckling (‡102, ‡713). I synnerhet kan AI-aktörer ställas inför påtryckningar att minska sin investering i skyddsåtgärder – exempelvis genom att begränsa behörigheter och åtkomst, eller driftsätta endast i miljöer med lägre kritikalitet – när sådana åtgärder är kostsamma eller tidskrävande att utveckla (se ’Konkurrensen skärper avvägningen mellan hastighet och säkerhet’ i §3.1. Tekniska och institutionella utmaningar).

###@ Uppdateringar

Sedan publiceringen av den senaste rapporten (Januari 2025) har AI-förmågor, inklusive sådana som skulle kunna underminera mänsklig kontroll, förbättrats i testmiljöer. Forskare har observerat framsteg i agensbaserade förmågor (se §1.2. Aktuella förmågor), inklusive förmågor som rör automatisering av AI-forskning som kan påskynda scenarier för förlust av kontroll (se §1.3. Förmågor till 2030). Det finns också växande experimentella belägg för bedrägliga förmågor. Detta omfattar AI-modeller som kan skilja mellan test- och driftsammanhang (‡33, ‡726, ‡741) eller ”reward hack”-tester av deras prestanda, och lära sig att göra planer svåridentifierade för att göra detta (‡430).

###@ Evidensluckor

Centrala kunskapsluckor innefattar brist på detaljerad hotmodellering och osäkerhetsestimering avseende den framtida utvecklingen av relevanta förmågor och benägenheter. På motsvarande sätt förblir det svårt att bedöma vilka trösklar där AI-modeller skulle vara tillräckligt sannolika att undergräva kontroll för att motivera obligatoriska riskreducerande åtgärder. Även om trösklarna hade fastställts kan förmågorna samverka på sätt som ännu inte är väl förstådda, vilket gör det svårt att bedöma när dessa trösklar har passerats. Sammantaget, även om det tillgängliga underlaget har ökat, finns det fortfarande otillräckligt underlag för att tillförlitligt avgöra om och hur dagens AI-förmågor och benägenheter skulle skala och generaliseras till risken för förlust av kontroll i framtiden.

###@ Åtgärder för att mildra risker

Medan AI-alignering i allmänhet fortfarande är ett öppet vetenskapligt problem (‡697, ‡735, ‡736), håller forskare på att ta fram potentiellt lovande inriktningar för att åtgärda de bakomliggande orsakerna till felinriktning. Sådana inriktningar inkluderar exempelvis att diversifiera träningsmiljön och att upptäcka felinriktning genom anomalioövervakning (‡737, ‡738, ‡739*). Andra forskare fokuserar på att bättre förstå och formalisera centrala mekanismer som målfelingeneralisation – till exempel hur agenter behåller förmågor men strävar efter oavsiktliga mål – för att kunna vägleda bättre utformning av träning och utvärdering (‡742). En annan forskningsinriktning undersöker sätt att avskilja agency från prediktiva förmågor, som ett sätt att skapa icke-agentiska AI-system som är pålitliga som standard (‡743). Sådana system skulle därefter kunna användas som ett ytterligare övervakningsskikt när de distribueras tillsammans med mindre tillförlitliga skyddsräcken mot AI-agenter som inte kan litas på.

Forskare utvecklar metoder för att upptäcka och förhindra felinriktning tidigt i utvecklingsprocessen. Detta arbete omfattar: tolkningsmetoder för att undersöka interna komponenter i AI-system och identifiera oroande beteenden (‡744, ‡745, ‡746); skalbar tillsyn (där en uppsättning AI-system används för att övervaka andra AI-system (‡747)); och inriktningsmetoder som syftar till att säkerställa att AI-system förblir lyhörda för mänsklig tillsyn (‡748, ‡749).

Forskare utvecklar också mekanismer och insatser för att hantera potentiellt felinriktade AI-system. Dessa inkluderar: övervakning av den ‘tankekedja’ som resonemangssystem producerar för tecken på felinriktning eller skadliga utdata (‡430, ‡435, ‡750); utveckling av säkerhetsfall som syftar till att med hög tillförlitlighet visa att modeller är osannolika att sabotera kontrollåtgärder (‡751); och att göra skyddsåtgärder mer robusta mot försök att underminera dem (‡725). Det framväxande området ‘AI-kontroll’, förblir dock i sin linda (‡752, ‡753). Framtida utmaningar för utvärderingsramverk inbegriper ett behov av att övervaka framtida AI-system som är mer kapabla och kan arbeta under längre perioder samt i mer komplexa miljöer.

###@ Utmaningar för beslutsfattare

Beslutsfattare som arbetar med förlust av kontroll måste förbereda sig för en risk vars sannolikhet, natur och tidpunkt förblir osäkra. Nuvarande AI-system utgör inte omedelbara risker för förlust av kontroll, men beslut som fattas idag kommer att avgöra om framtida system gör det. Dessa beslut omfattar hur man ska stödja utvecklingen av tillförlitliga metoder för utvärdering och lindring samt huruvida det bör finnas regler om tillgång och behörigheter som ges till AI-system i olika miljöer. När dessa beslut fattas ställs beslutsfattare inför svåra avvägningar. Om man till exempel begränsar driftsättning av AI-system i kritiska miljöer kan det minska deras fördelar, medan ett tillåtande av bred driftsättning kan öka risken om skyddsåtgärderna visar sig vara otillräckliga.

