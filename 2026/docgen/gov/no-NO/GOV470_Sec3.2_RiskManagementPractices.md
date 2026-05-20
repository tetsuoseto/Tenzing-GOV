##########
>white|orangered|left|14|30|hr Kapittel 3.2
### 3.2. Risikostyringspraksis
>white|orangered|left|24|30|hb Risikostyringspraksis

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb Viktig informasjon
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Risiko for styring av generell-purpose KI omfatter et spekter av praksiser som brukes for å identifisere, vurdere og redusere risikoer fra generell-purpose KI. Dette inkluderer testing og evaluering på modell-nivå (for eksempel «red-teaming»), organisatoriske prosesser som styrer utviklings- og utgivelsesbeslutninger, betingede sikringstiltak (for eksempel «if-then»-forpliktelser), og hendelsesrapportering.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Flere AI-utviklere har utarbeidet Frontier AI Safety Frameworks. Disse rammeverkene inneholder informasjon om risikovurderinger og angir betingede tiltak, som tilgangsbegrensninger selskaper planlegger å innføre for mer kapable modeller. De varierer med hensyn til hvilke risikoer de dekker, hvordan de definerer terskler for kapabilitet, og hvilke handlinger som utløses når terskler nås.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Dokumentasjon av den reelle effekten i verden av AI-risikostyringspraksiser er fortsatt begrenset. Mangel på hendelsesrapportering og overvåking gjør det vanskelig å vurdere hvor godt gjeldende praksiser reduserer risiko, eller hvor konsekvent de implementeres.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Siden publiseringen av forrige rapport (januar 2025) har risikostyring blitt mer strukturert gjennom nye bransje- og styringsinitiativer. Nye virkemidler som EUs kode for praksis for kunstig intelligens til generell bruk, Kinas rammeverk for styring av AI-sikkerhet 2.0, og G7s rapporteringsrammeverk for Hiroshima AI-prosessen, sammen med initiativer drevet av selskaper, illustrerer trenden mot mer standardiserte tilnærminger til transparens, evaluering og rapportering av hendelser.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Markedsdynamikk og tempoet i AI-utviklingen skaper ytterligere utfordringer. På grunn av konkurransepress kan AI-selskaper stå overfor avveininger mellom raskere produktlanseringer og investeringer i tiltak for risikoreduksjon. Mange AI-relaterte skader blir også eksternalisert, og det er fortsatt uklart hvilket juridisk ansvar som gjelder for dem, og styringsprosesser kan ta tid før de tilpasses endringer i AI-landskapet.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Viktige utfordringer for myndigheter er å prioritere mellom de ulike risikoene som generell-purpose AI medfører, og å avklare hvilke aktører i hele AI-verdikjeden som er best posisjonert til å redusere dem. Disse utfordringene forsterkes av begrenset innsyn i hvordan risiko identifiseres, vurderes og håndteres i praksis, samt fragmentert informasjonsdeling mellom utviklere, deployere og infrastrukturoperatører.
>oldlace|black||11|15|br      


Håndtering av AI-risiko omfatter en rekke praksiser som tar sikte på å identifisere, vurdere og redusere sannsynligheten for og alvorlighetsgraden av risikoer knyttet til AI-systemer. Disse praksisene kan implementeres av AI-utviklere, driftsaktører, evaluerere og regulatorer. Eksempler inkluderer trusselmodellering, risikotilordning, rødteamøvelser, revisjon og hendelsesrapportering. Dette avsnittet beskriver gjeldende praksiser for risikohåndtering, nye utviklingstrekk og gjenstående begrensninger.

Siden starten av 2025 har flere nye internasjonale initiativer for risikostyring av generell- formål AI utviklet seg, inkludert rammeverk for organisatorisk åpenhet og risikorapportering samt regulatoriske og styringsmessige rammeverk.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Figur 3.4: Fire komponenter i risikostyring
>white|black||9|11|br De fire kategoriene metoder for risikostyring for generell formål AI: risikokartlegging; risikovurdering og -evaluering; risikoredusering; og risikostyring. Disse utgjør en iterativ og syklisk prosess. Risikostyring, vist i midten, legger til rette for at de andre komponentene lykkes. Kilde: International AI Safety Report 2026.


Gjenværende utfordringer omfatter begrenset standardisering, noe som kompliserer etterlevelse og vurdering, samt begrenset dokumentasjon om reell effekt i praksis. Videre er institusjonelle, kulturelle og politiske kontekster ulike globalt, noe som innebærer at tilnærminger til å identifisere og håndtere risikoer, inkludert akseptable terskler for risiko, kan variere mellom regioner. Denne seksjonens omtale av risikostyringstilnærminger er beskrivende: den tar sikte på å informere aktører i AI-økosystemet om nåværende globale tilnærminger til risikostyring. Der det finnes, drøftes dokumentasjon om effektivitet og begrensninger ved disse tilnærmingene, men politiske anbefalinger ligger utenfor rammen for dette arbeidet.

###@ Komponenter i risikostyring

Risikostyring er en iterativ prosess med praksiser og metoder som spenner over hele AI-utviklings- og distribusjonssyklusen, men som fungerer sammen på en sammenhengende måte (‡969). Risikostyring for general-purpose AI kan omfatte roller for et bredt spekter av aktører, inkludert data scientists, model engineers, revisorer, domeneeksperter, ledere, sluttbrukere, berørte lokalsamfunn, tredjepartsleverandører, beslutningstakere, myndigheter, standardiseringsorganisasjoner og sivilsamfunnsorganisasjoner (‡970, ‡971, ‡972). Ledende risikostyringsstandarder er ofte interoperable, men bruker ulike begreper for å beskrive elementene i risikostyring (‡973, ‡974). De har typisk fire sammenkoblede komponenter (Figur 3.4): identifisering; analyse og evaluering; mitigering; og styring av risiko (‡970, ‡973, ‡975, ‡976). Tabellene nedenfor gir illustrerende eksempler på relevante metoder, teknikker og verktøy. Praksiser fortsetter å utvikle seg, så tabellene er ikke uttømmende, og anvendelighet vil variere på tvers av kontekster.

###@ Risikokartlegging

Risikokartlegging er prosessen med å finne, gjenkjenne og beskrive risikoer. Omfattende risikokartlegging omfatter typisk kapabilitetsdrevne vurderinger, som tester om modeller har bestemte farlige kapabiliteter (‡977), samt risikomodellering (‡978) og prognostisering (‡715*), som brukes for å utforske eksisterende og fremvoksende risikoer. Tabell 3.1 gir ulike eksempler på praksiser for risikokartlegging. Risikokartlegging bygger også på involvering av relevante eksperter og miljøer for å forstå den bredere konteksten for hvordan risikoer oppstår (‡979, ‡980). Mekanismer som bug bounty-ordninger kan støtte denne prosessen ved å stimulere til identifisering av tidligere ukjente sårbarheter (‡981) (Tabell 3.1). Et sentralt mål for risikokartlegging er å ta hensyn til både velkjente, godt forståtte risikoer og potensielle fremtidige risikoer som fortsatt er usikre eller dårlig karakterisert (‡982). Dette er særlig viktig for generell formål-AI, der mange risikoer kanskje ikke ennå er fullt ut forstått eller observerbare (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bug bounty-programmer
  Bug bounty-ordninger eller programmer for sårbarhetsrapportering gir insentiver til å finne og rapportere sårbarheter i AI-systemer. Flere utviklere har implementert bug bounty-programmer (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ekspertrådgivning
  Fagfolk, brukere og berørte lokalsamfunn gir innsikt i sannsynlige risikoer. Det finnes nye retningslinjer for deltakende og inkluderende KI (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ishikawa (fiskebeins) diagram
  Ishikawa-diagrammer er veletablerte verktøy for årsaksanalyse, og forskere har foreslått å bruke dem for strukturert analyse av hendelser knyttet til AI-risiko (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Prediksjon
  Prognostisering er prosessen med å forutsi fremtidige hendelser eller trender basert på analyse av tidligere og nåværende data. Den har blitt brukt til å sammenligne den relative sannsynligheten for for eksempel ulike økonomiske utfall som følge av avansert KI (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risiko-taksonomi
  Risikotaksonomier er en måte å kategorisere og organisere risikoer på tvers av flere dimensjoner. Det finnes flere som beskriver risikoer fra generelle formål med AI (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Scenario planlegging
  Scenario-planlegging innebærer å utvikle plausible fremtidige scenarier og analysere hvordan risiko materialiserer seg. Dette har blitt brukt til å utforske risikoene og virkningene av AI-modeller (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Trusselmodellering
  Trusselmodellering er en prosess for å identifisere trusler og sårbarheter for et system. Tallrike utviklere av kunstig intelligens fremhever bruken av trusselmodellering for å forutse potensielle misbruksscenarier for AI-systemer (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 3.1: Eksempler på risikokartlegging i generell risikostyring for AI til allmennyttige formål
>white|black||9|11|br Eksempler på metoder for risikidentifisering i KI er listet alfabetisk. Metodene som er inkludert
er utformet for å støtte risikofangst for mange ulike risikotyper, inkludert risiko fra ondsinnet bruk, risiko fra feilfunksjoner og systemiske risikoer. Gitt den foreløpige karakteren til risikostyring for generell-purpose AI, vil ikke alle metoder være egnet for hver AI-utvikler eller -utplassering.


>white|orangered|left|14|15.5|bb Trusselmodellering og risikotaksonomier er fremtredende metoder for risikokartlegging

To fremtredende metoder for å identifisere risikoer fra generell-purpose AI er trusselmodellering (International AI Safety Report 2026) (en strukturert prosess for å kartlegge hvordan AI-relaterte risikoer kan materialisere seg) og risik taksonomier. Meta bruker for eksempel trusselmodellering-øvelser for å forutse potensielle misbruksscenarier for sine AI-modeller (‡990), og Anthropic inkluderer trusselmodellering som en del av sin ASL-3 Deployment Standard (‡991). AI-risiko- og hazard taksonomier, som lister kategorier for risiko og eksempler, kan like godt fungere som et utgangspunkt for å konseptualisere, identifisere og spesifisere de sentrale risikoene knyttet til generell-purpose AI i bestemte anvendelsesdomener (‡906, ‡988, ‡992, ‡993).

###@ Risikanalyse og evaluering

Risikanalyse og evaluering er prosessen med å bestemme risikonivået til en AI-modell eller et system og sammenligne det med etablerte kriterier for å vurdere akseptabilitet eller behovet for risikoreduserende tiltak (‡994, ‡995, ‡996, ‡997). Den omfatter praksiser som å måle modellens ytelse på benkmarkeder (‡998) og evalueringer (‡176, ‡715), gjennomføre red-teaming-øvelser (‡999*), konsekvensvurderinger (‡1000) og revisjoner (‡1001, ‡1002). Se Bord 3.2 for eksempler på generell analyse og evaluering av AI-risiko. Metodene er utformet for å støtte analyse og evaluering for mange ulike typer risiko samtidig.

Nøkkelmålene for risikovurdering og evaluering er å gjennomføre evalueringer av modellkapabiliteter og sårbarheter (‡1003), å bruke robust risikomodellering for å informere beslutninger om risikotilpasninger (‡1004, ‡1005), og å forstå hvordan AI-systemer brukes i praksis for å vurdere påfølgende samfunnsmessige virkninger (‡869, ‡904, ‡905, ‡1006). Risikovurderings- og evalueringsprosesser anses ofte for å være mer sannsynlige for å identifisere risikoer når de inkluderer uavhengig gjennomgang (‡1001, ‡1007), bygger på tverrsektoriell ekspertise (‡1008), og omfatter ulike perspektiver fra flere domener og disipliner, samt fra berørte lokalsamfunn (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Revisjoner
  Revisjoner er formelle gjennomganger av ytelsen og virkningene til AI-modeller og/ eller en organisasjons etterlevelse av standarder, retningslinjer og prosedyrer, utført internt eller av en ekstern part. AI-revisjon er et voksende fagfelt, og det finnes en rekke verktøy og praksiser for å revidere AI-modeller og praksisene til utviklere av AI-modeller (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Benchmarks
  Benkemarker er standardiserte, ofte kvantitative tester eller målemetoder som brukes til å evaluere og sammenligne ytelsen til AI-systemer på et fast sett med oppgaver utformet for å representere reell bruk (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bowtie-metoden
  Sløyfemetoden er en velkjent metode for å visualisere hvor kontroller kan legges til for å redusere risikohendelser. Den gir en tydelig differensiering mellom proaktiv og reaktiv risikostyring (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Delphi-metoden
  Delphi-metoden er en gruppebasert beslutningsteknikk som bruker en rekke spørreskjemaer for å innhente enighet fra et panel av eksperter (‡1020, ‡1021). Den har blitt brukt for å bidra til å utforske mulige framtider med avansert KI (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Felt-testing
  Felt-testing vurderer en AI-systems ytelse og innvirkning i et reelt, operasjonelt miljø. Noe forskning fremhever felt-testing som et supplement til modell-evaluering for å vurdere utfall og konsekvenser i den virkelige verden (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Konsekvensvurdering
  Konsekvensvurderinger vurderer de potensielle konsekvensene av en teknologi eller et prosjekt. Dette kan omfatte kvantifisering, aggregering og prioritering av konsekvenser. EU AI-loven krever for eksempel at utviklere av høyrisikable AI-systemer gjennomfører vurderinger av grunnleggende rettigheter (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modellvurdering
  Modellvurderinger inkluderer prosesser og tester for å vurdere og måle en AI-modells ytelse for en bestemt oppgave. Det finnes mange AI-vurderinger for å vurdere ulike evner og risikoer, inkludert for sikkerhet, cybersikkerhet og sosial innvirkning (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sannsynlighetsbasert risikovurdering
  Sannsynlighetsbasert risikovurdering er en metodikk for å vurdere risikoer knyttet til komplekse systemer eller prosesser som inkorporerer usikkerhet. Den har blitt tilpasset for avanserte AI-systemer (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Red-teaming
  Red-teaming er en øvelse der en gruppe mennesker eller automatiserte systemer later som om de er en motstander og angriper en organisasjons teknologiske systemer for å identifisere sårbarheter. Mange AI-selskaper har interne praksiser for red-teaming av AI-systemer (‡458, ‡1028). Red-teaming kan også gjennomføres av aktører utenfor selskaper. Disse teamene står overfor utfordringer som begrenset tilgang, men kan også avdekke distinkte innsikter (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risikomatriser
  Risikomatriser er et visuelt verktøy for å hjelpe med å prioritere risikoer basert på sannsynligheten for forekomst og mulig konsekvens (‡1027). Noen AI-utviklere inkluderer grunnleggende risikomatriser i sine rammeverk for Frontier AI Safety (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risikotoleranser/risikonivåer
  Risikoterskler eller nivåer er kvantitative eller kvalitative grenser som skiller akseptable fra uakseptable risikoer, og som utløser spesifikke risikohåndteringshandlinger når de overskrides. For generelt formål AI bestemmes de av en kombinasjon av kapabiliteter, påvirkning, beregningskapasitet, utbredelse og andre faktorer (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risikotoleranse
  Risikovilje viser til nivået av risiko som en organisasjon er villig til å akseptere. I KI settes risikotoleranser ofte implisitt gjennom selskapets retningslinjer og praksiser, mens noen reguleringsregimer eksplisitt definerer uakseptable risikoer og knytter rettslige konsekvenser til dem (‡1032). Noen selskaper beskriver sin risikovilje i form av en ny modells marginale risiko; det vil si i hvilken grad en modell kontrafaktisk øker risiko utover den som allerede skapes av eksisterende modeller eller andre teknologier (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sikkerhetssaker
  Et sikkerhetsargument er en strukturert argumentasjon, støttet av bevis, som begrunner at et system er akseptabelt trygt å drifte i en bestemt kontekst. Nylig litteratur (‡1037, ‡1038, ‡1039) har undersøkt sikkerhetsargumenter for frontiersystemer for kunstig intelligens, og enkelte Frontier AI Safety Frameworks viser til dem (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb System-sikkerhetsanalyse
  System safety-analyse fremhever avhengigheter mellom komponenter og systemet de inngår i, for å forutse hvordan systemnivårisiko kan oppstå fra komponent- eller prosessfeil, eller fra samspill mellom delsystemer, menneskelige faktorer og miljømessige forhold. Tilnærminger anvendt for AI-systemer i litteraturen inkluderer systemteoretisk prosessanalyse (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 3.2: Risikovurdering/risikoanalyse i generell risikostyring for kunstig intelligens til allmenn bruk
>white|black||9|11|br Eksempler på metoder for AI-risikokartlegging/-vurdering, oppført alfabetisk. Gitt den umodne naturen til risikostyring for generell formål-AI, vil ikke alle metoder være egnet for enhver AI-utvikler eller -utplasserer.


>white|orangered|left|14|15.5|bb Vanlige verktøy for risikoanalyse inkluderer ytelsesbenchmarker og modellevalueringer

Benkmarkeringer og modellvurderinger er standardiserte tester for å vurdere ytelsen til generelle AI-systemer på bestemte oppgaver. Forskere har utviklet et bredt utvalg av benkmakerings- og vurderingsopplegg, inkludert sett med utfordrende flervalgsspørsmål, programvareingeniørproblemer og arbeidsrelaterte oppgaver i simulerte kontormiljøer (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Skadelige kapabilitetsvurderinger (‡715) brukes for å vurdere om en generelle formål AI-modell eller et system har særlig farlig kunnskap eller ferdigheter, slik som evnen til å bistå i cyberangrep (se §2.1.3. Cyberangrep).

Svært konsekvensrike beslutninger fra selskaper og myndigheter om modellutslipp bygger delvis på disse vurderingene (‡1050, ‡1051, ‡1052). Imidlertid varierer benchmarkene betydelig i kvalitet og omfang (‡998, ‡1003), og det kan være vanskelig å vurdere gyldigheten deres på grunn av en rekke mangler i evalueringspraksisen (‡902, ‡909, ‡1003, ‡1053*). For eksempel kan benchmarker bli «mettet» – når mange modellers resultater nærmer seg toppscoren – slik at de ikke lenger skiller tydelig mellom modeller. Modeller blir også i økende grad mer sannsynlige til å gjenkjenne bestemte oppgaver som evalueringer og vise andre atferder enn de ville gjort på lignende oppgaver i driftskontekster, på grunn av «situasjonsbevissthet» (se §2.2.2. Tap av kontroll). Til slutt har benchmarker og vurderinger velkjente begrensninger: særlig klarer de ikke å fange opp risikoer knyttet til bruk av generell formål AI i nye domener og for nye oppgaver, siden testbetingelsene skiller seg fra faktisk bruk i varierende grad (‡913) (se §1.2. Nåværende evner og §3.1. Tekniske og institusjonelle utfordringer).

>white|orangered|left|14|15.5|bb Red-teaming muliggjør mer domene-spesifikke vurderinger av risiko

En annen vanlig metode for å vurdere risikoer er red-teaming. Et «red team» er en gruppe evaluerere som har fått i oppdrag å lete etter sårbarheter, begrensninger eller potensial for misbruk. Red-teaming kan være domenespesifikk og utføres av domeneeksperter, eller være åpen for å utforske nye risikofaktorer. For eksempel kan et red team utforske «jailbreaking»-angrep som undergraver modellens sikkerhetsrestriksjoner (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). I motsetning til benchmarks er en viktig fordel med red-teaming at red teams kan tilpasse evalueringene sine til det spesifikke systemet som testes. For eksempel kan red teams utforme tilpassede inputer for å identifisere verstefalls-atferd, muligheter for ondsinnet bruk og uventede feil. Det kan imidlertid kreve spesialtilgang til modeller og kan mislykkes i å avdekke viktige klasser av risikoer (‡999, ‡1028).

Viktig: Fraværet av identifiserte risikoer betyr ikke at disse risikoene er lave. Tidligere arbeid viser at feil ofte slipper unna deteksjon, særlig når red teams har begrenset tilgang eller ressurser (‡1060). Forskning har også satt spørsmålstegn ved om red-teaming kan gi pålitelige og reproduserbare resultater (‡1061). Sammensetningen av red teamet og instruksjonene som gis til red-teamere (‡1062), antallet angrepsrunder (‡1063) og modellens tilgang til verktøy (‡1064, ‡1065) kan påvirke utfallene betydelig, inkludert risikoflaten som dekkes. Omfattende retningslinjer for red-teaming tar sikte på å håndtere noen av disse utfordringene (‡1066).

###@ Risikoreduksjon

Risikoreduksjon er prosessen med å prioritere, vurdere og implementere kontroller og tiltak for å redusere identifiserte risikoer. Eksempler er tilgangskontroller (‡991), kontinuerlig overvåking (‡986) og if-then-forpliktelser (‡700). Å redusere risiko reiser et sentralt spørsmål: hvilket nivå av risiko som er akseptabelt? Nyere rammeverk og selskapspolicyer har begynt å formalisere kriterier for «risikoaksept» (‡965, ‡1040). Likevel er det å fastsette hensiktsmessige terskler fortsatt utfordrende, særlig for risikoer med brede samfunnsmessige konsekvenser (‡986, ‡1067). Det finnes for øyeblikket ingen etablert mekanisme for å validere beslutninger om risikoaksept som utviklere har tatt før utgivelse (‡1005).

Risikoreduserende metodene beskrevet i Bord 3.3 nedenfor er tilpasningsdyktige og kan redusere en rekke risikoer, inkludert noen uforutsette risikoer. Tabellen omfatter ikke tekniske risikoreduserende metoder som adversarial trening, innholdsfiltre og overvåking av chain-of-thought. Disse dekkes i §3.3 Tekniske sikringstiltak og overvåking, samt gjennom hele rapporten i avsnittene «Mitigations» for hver risiko i §2. Risks.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Retningslinjer for akseptabel bruk
  En akseptabel bruk-policy er et sett med regler og retningslinjer for ansvarlig, etisk og juridisk bruk av AI-modeller. Det er vanlig at AI-utviklere publiserer en policy for akseptabel bruk, samt en policy for forbudt bruk, med nye modellutgivelser (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tilgangskontroll/bruker-vurdering
  Tilgangskontroller inkluderer bruk av retningslinjer og regler for å begrense tilgang til AI-modeller, data og systemer basert på brukerroller, attributter og andre betingelser for å forhindre uautorisert bruk, manipulering eller datainnbrudd. AI-selskaper deaktiverer ofte kontoer som er funnet å være involvert i kriminell aktivitet (‡486) og inkluderer brukervurdering og Know-Your-Customer-kontroller for å sikre at modeller kun brukes av pålitelige aktører (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Atferds-/modellspesifikasjon
  En spesifikasjon for AI-oppførsel er et dokument som definerer hvordan en AI-modell skal oppføre seg i ulike situasjoner. Den fungerer som en mal for AI-tilpasning og sikkerhet, og veileder modellutvikling, opplæring, evaluering og utdata. Flere AI-selskaper bruker modellspesifikasjonsdokumenter og gjør minst deler av dem offentlige (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kontinuerlig overvåking
  Kontinuerlig overvåking er den pågående, automatiserte prosessen med å observere, analysere og kontrollere AI-systemer i bruk, spore deres ytelse og begrense deres atferd for å sikre pålitelighet, effektivitet og sikkerhet. Det finnes mange verktøy for kontinuerlig overvåking (‡1073*) samt teknikker for å støtte
AI-observerbarhet (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Forsvar-i-dybden
  Defence-in-depth er ideen om at flere uavhengige og overlappende forsvarslag kan implementeres slik at hvis ett mislykkes, vil de andre fortsatt være effektive (‡1075, ‡1076). Flere Frontier AI Safety Frameworks viser til det (f.eks. (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Økosystemovervåking
  Dette er prosessen med å overvåke det bredere AI-økosystemet, inkludert sporing av beregning og maskinvare, modellproveniens, dataproveniens og bruks-mønstre. Forskningslitteraturen omtaler slik overvåking i forbindelse med risikoer fra generell formål-AI (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hvis-deretter-forpliktelser
  If-then-forpliktelser er et sett med tekniske og organisatoriske protokoller og forpliktelser for å håndtere risiko etter hvert som AI-modeller blir mer kapable. Flere AI-utviklere benytter denne typen forpliktelser som en del av sine Frontier AI Safety Frameworks (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Røde linjer eller forbud
  Røde linjer er spesifikke grenser uttrykt som kapabiliteter, påvirkning eller typer bruk. Konseptet forekommer i offentlige uttalelser og initiativer, samt i regulatoriske forbud (‡1079, ‡1080, ‡1081). Litteraturen peker også på begrensninger ved tilnærminger med røde linjer, inkludert utfordringer knyttet til enighet og håndhevbarhet.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Utgivelses- og distribusjonsstrategier
  Utgivelses- og distribusjonsstrategier for generell-purpose AI kan omfatte bruk av trinnvise utrullinger eller API-tilgang slik at flere avbøtende tiltak er tilgjengelige i tilfelle misbruk eller uventet skade (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 3.3: Risikoredusering i generell risikostyring for AI til allmenn bruk
>white|black||9|11|br Eksempelmetoder for risikoreduksjon ved AI, oppført alfabetisk. Metodene som er inkludert, er utformet for å støtte risikoreduksjon for mange ulike risikotyper samtidig, inkludert risikoer fra ondsinnet bruk, risikoer fra feilfunksjon og systemiske risikoer. Gitt den umodne naturen til risikostyring for generell AI, vil ikke alle metoder være egnet for enhver AI-utvikler eller AI-innfører.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Figur 3.5: En «ostekake-diagram» som illustrerer forsvar-i-dybden-tilnærmingen
>white|black||9|11|br Flere lag med forsvar kan kompensere for svakheter i individuelle lag. Gjeldende risikostyringsteknikker for AI har svakheter, men å stable dem kan gi mye sterkere beskyttelse mot risiko. Kilde: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Forsvar i dybden og utgivelsesstrategier er viktige risikoreduserende tiltak

En ‘defence-in-depth’-modell kan støtte generell risikostyring for AI. I denne sammenhengen betyr ‘defence-in-depth’ en kombinasjon av tekniske, organisatoriske og samfunnsmessige tiltak som anvendes på tvers av ulike stadier i utvikling og utplassering (Figur 3.5). Dette innebærer å etablere lag med uavhengige beskyttelser, slik at dersom ett lag feiler, kan andre lag fortsatt hindre skade. Et ofte sitert eksempel på en defence-in-depth-modell er den brede samlingen av forebyggende tiltak som settes inn for å hindre smittsomme sykdommer. Vaksiner, munnbind og håndvask, blant annet, kan redusere risikoen for infeksjon betydelig i kombinasjon, selv om ingen av disse metodene er 100% effektive hver for seg (‡1083*). For generell-purpos AI vil defence- in-depth omfatte kontroller som ikke ligger i selve AI-modellen, men i det bredere økosystemet. Dette inkluderer (for eksempel) kontroller på materialene som trengs for å gjennomføre et biologisk angrep, slik som reagenser (‡1084, ‡1085). Imidlertid retter defence- in-depth-tiltak primært oppmerksomheten mot risikoer knyttet til uhell, feilfunksjon og ondsinnet bruk, og kan spille en mindre rolle i håndteringen av systemiske risikoer (se §3.5. Bygge samfunnsmessig robusthet).

En bedrifts lanserings- og distribusjonsstrategi er en viktig del av risikoreduksjon. Beslutninger om hvordan modeller gjøres tilgjengelige for brukere kan påvirke risikobildet betydelig (‡1082). Ulike alternativer for lansering og distribusjon inkluderer trinnvis lansering til avgrensede brukergrupper, tilgang via kontrollerte nettjenester (som API-er), og bruk av lisensavtaler og retningslinjer for akseptabel bruk som juridisk forbyr visse skadelige applikasjoner (‡176, ‡1086, ‡1087). §3.4. Open-weight-modeller drøfter mer detaljert hvordan utlevering av modellvekter påvirker risikoer.

###@ Risikostyring

Risikostyring er prosessen der risikostyringsevalueringer, beslutninger og tiltak kobles til strategi og mål for en organisasjon eller annen enhet (‡1088, ‡1089). Tabell 3.4 gir en oversikt over vanlige teknikker for risikostyring. Som vist i Figur 3.4 kan risikostyring forstås som kjernen i risikostyring, siden det legger til rette for effektiv drift av andre komponenter i risikostyring. Det gir ansvarlighet, åpenhet og tydelighet som støtter informerte beslutninger i risikostyring. Risikostyring kan omfatte praksiser som hendelsesrapportering (‡1090), fordeling av risikansvar (‡965) og beskyttelse av varsleren (‡1091). Mer bredt kan risikostyring omfatte veiledning, rammeverk, lovgivning, regulering, nasjonale og internasjonale standarder, samt opplærings- og utdanningsinitiativer. Et sentralt formål med risikostyring er å etablere organisatoriske retningslinjer og mekanismer som klargjør hvordan risikostyringsansvar fordeles på tvers av en organisasjon eller annen enhet, for å støtte hensiktsmessig tilsyn og ansvarlighet (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dokumentasjon
  Dokumentasjonspraksiser hjelper med å spore nøkkelinformasjon om AI-systemer, som treningsdata, designvalg, tiltenkte bruksområder, begrensninger og risikoer. «Modellkort» og «systemkort», som gir informasjon om hvordan en AI-modell eller et AI-system ble trent og evaluert, er eksempler på fremtredende beste praksiser for AI-dokumentasjon (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hendelsesrapportering
  Incidentrapportering er prosessen med systematisk å dokumentere og dele tilfeller der utvikling eller distribusjon av KI har forårsaket direkte eller indirekte skade. Det finnes flere plattformer som legger til rette for incidentrapportering for KI (‡1096, ‡1097), og rammeverk som legger til rette for mer effektiv incidentrapportering for KI (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risikostyringsrammeverk
  Risikostyringsrammeverk er organisatoriske planer for å redusere hull i risikodekning, koordinere ulike risikostyringsaktiviteter og implementere kontroller og motvekter. Rammeverk som er spesifikke for generell formål AI (‡986, ‡1098) viser ofte til de andre tiltakene som er nevnt i denne seksjonen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Risikoregister
  Et risikoregister er et register over ulike risikoer, deres prioritering, eiere og avbøtende planer. Disse er relativt vanlige i mange bransjer, inkludert cybersikkerhet (‡1099), og brukes noen ganger for å oppfylle krav til regulatorisk etterlevelse.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tildeling av risikans ansvar
  Tildelingen av roller og ansvarsområder for risikostyring i en organisasjon kan strukturere intern kontroll av beslutningstaking (‡1002, ‡1093). Slike ordninger gjenspeiles i enkelte styringsrammeverk, inkludert EUs kode for praksis for allmennformål med kunstig intelligens (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Transparensrapporter
  Gjennomsiktighetsrapporter beskriver en AI-bedrifts risikostyringspraksiser ved offentlig å gjøre visse opplysninger tilgjengelige eller ved å dele dokumentasjon med bransjeorganisasjoner eller statlige organer. For eksempel sender en rekke AI-selskaper inn gjennomsiktighetsrapporter for Hiroshima AI Process (HAIP) (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Varslerbeskyttelse
  Fordi mye av AI-utviklingen skjer bak lukkede dører, inkluderer enkelte styringsrammeverk beskyttelse for varsling for å muliggjøre rapportering av potensielle risikoer til myndighetene (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 3.4: Risikostyring i risikostyring for generell-purpose AI
>white|black||9|11|br Eksempelmetoder for AI-risikostyring er listet alfabetisk. Metodene som er inkludert, er utformet for å støtte risikostyring for mange ulike risikotyper samtidig, inkludert risikoer fra ondsinnet bruk, risikoer fra feilfunksjoner og systemiske risikoer. Gitt den umodne karakteren til risikostyring for generell-purpose AI, vil ikke alle metodene være egnet for enhver AI-utvikler eller -utplassering.


>white|orangered|left|14|15.5|bb Dokumentasjon og åpenhet er komponenter i risikostyring

Dokumentasjons- og institusjonelle åpenhetsmekanismer, sammen med informasjonsdelingspraksiser, legger til rette for ekstern granskning og støtter arbeidet med å håndtere risikoer knyttet til generell-purpose AI (‡1101, ‡1102). Det har blitt vanlig praksis å publisere resultatene fra før-utplasseringstester i en «model card» eller «system card», sammen med grunnleggende opplysninger om modellen eller systemet, inkludert hvordan det ble trent og hvilke potensielle begrensninger det har (‡1094, ‡1095). Noen utviklere publiserer også åpenhetsrapporter som inneholder nærmere detaljer om deres risikostyringspraksiser mer generelt (‡1103). Andre elementer i dokumentasjon og åpenhet omfatter overvåking og hendelsesrapportering (‡176, ‡1083*, ‡1103) samt informasjonsdeling, som kan tilrettelegges av tredjeparter, for eksempel Frontier Model Forum. Noen regelverksrammeverk, som EUs AI Act eller Californias Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53) (‡1081, ‡1104), krever i noen tilfeller informasjonsdeling om risikoer knyttet til generell-purpose AI.

>white|orangered|left|14|15.5|bb Ledelsesforpliktelse og insentiver former risikostyringspraksis

Organisasjonskultur, ledelsesstruktur og insentiver påvirker risikohåndteringsarbeidet på ulike måter (‡1105). Ledelsesforpliktelse og insentivstrukturer er ofte relevante for hvordan risikohåndteringspolicyer fungerer i praksis. Noen utviklere har interne beslutningspaneler som drøfter hvordan man trygt og ansvarlig kan utforme, utvikle og gjennomgå nye AI-systemer. Tilsyns- og rådgivningskomiteer, tillitsordninger eller AI-etikkstyrer kan også fungere som mekanismer for risikohåndteringsveiledning og organisatorisk tilsyn (‡1092*, ‡1106, ‡1107, ‡1108). Forskere har hevdet at utfordringer med frivillig egenstyring betyr at tredjepartsauditering, verifisering og standardisering kan bidra til å styrke generell risikohåndtering for allmennformål-AI (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Organisatorisk risikostyring, åpenhet og risikorapporteringsrammeverk

Flere nye initiativer retter fokus mot risikohåndteringsprosesser, dokumentasjon og åpenhet. I sin nåværende form fungerer EUs retningslinjer for allmennformåls-AI som en frivillig rammeverk for å veilede åpenhets-, opphavsretts- og sikkerhets- og sikkerhetstiltakspraksiser, for å støtte etterlevelse av bestemmelsene i EUs AI-lov for allmennformåls-AI (‡965). Per desember 2025 har mer enn to dusin selskaper† signert. G7 Hiroshima AI-prosessens (HAIP) rapporteringsrammeverk (‡1100) er det første internasjonale rammeverket for frivillig offentlig rapportering av organisatoriske risikohåndteringspraksiser for avanserte AI-systemer. Minst 20 utviklere har publisert offentlige åpenhetsrapporter som dekker risikidentifisering, evalueringsmetrikker, avbøtende strategier og datamessige sikkerhetsprosesser.

AI-utviklere har tatt i bruk frivillige åpenhetsforpliktelser. I Kina ble løfter fra 17 kinesiske AI-selskaper, koordinert av AI Industry Alliance of China, offentliggjort i desember 2024 (‡1113) og oppdatert i 2025 (‡1114). Under AI Seoul Summit i mai 2024 i Sør-Korea signerte 16 AI-utviklere fra flere land frivillige forpliktelser om å publisere Frontier AI Safety Frameworks for sine mest kapable modeller og systemer, og om å ta i bruk risikostyringspraksiser på tvers av modellutviklings- og distribusjonsstadier (‡1052).

    Note † -- Underskrivere per desember 2025 inkluderer: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing, og WRITER.

>white|orangered|left|14|15.5|bb Frontier AI Safety Frameworks har blitt en fremtredende organisatorisk tilnærming for håndtering av AI-risiko

Siden 2023 har flere ledende utviklere av AI frivillig publisert dokumenter som beskriver hvordan de planlegger å identifisere og håndtere alvorlige risikoer fra sine mest avanserte systemer. Disse Frontier AI Safety Frameworks beskriver hvordan en AI-utvikler planlegger å evaluere, overvåke og kontrollere sine mest avanserte AI-modeller og systemer før og under distribusjon. Disse rammeverkene har mange likheter, men skiller seg på viktige punkter (‡1115, ‡1116). De fleste fokuserer på risikoer knyttet til kjemiske, biologiske, radiologiske og kjernefysiske (CBRN) trusler, avanserte cyber-evner og avansert autonom atferd (‡1115, ‡1117). En minoritet av rammeverkene omfatter tilleggsmessige risikoområder som ulovlig diskriminering i stor skala og utnyttelse av barn i seksuelle sammenhenger.

Flere utviklere oppdaterte rammeverkene sine i 2025, og la til nye avsnitt om skadelig manipulasjon, feiljusteringsrisiko og autonom replisering og tilpasning (‡1078, ‡1118). Selv om mange rammeverk beskriver lignende tilnærminger for risikohåndtering – inkludert trusselmodellering, rødteaming og vurderinger av farlige evner – varierer de i definisjonene sine av risikonivåer og terskler, hvor ofte evalueringene gjennomføres, buffere mellom evalueringer og terskler, og hvor helhetlige forpliktelsene deres til avbøtende tiltak er (for eksempel om de inkluderer sletting av modellvekter eller bare pauserer utviklingen) (‡1115, ‡1119). Se Bord 3.5 for mer informasjon.

>white|orangered|left|14|15.5|bb Mange handlinger i Frontier AI Safety Frameworks er basert på hvis-da-forpliktelser

En sentral del av Frontier AI Safety Frameworks er «hvis-og-da»-forpliktelser. Dette er betingede protokoller som utløser bestemte responser når AI-modeller og -systemer når forhåndsdefinerte kapabilitetsterskler (‡1120). For eksempel kan en hvis-og-da-forpliktelse si at hvis det blir funnet at en modell har evnen til på en meningsfull måte å hjelpe nybegynnere med å utvikle og ta i bruk CBRN-våpen, så vil utvikleren implementere forbedrede sikkerhetstiltak, distribusjonskontroller og sanntidsmonitorering (‡991*).

I 2025 kunngjorde flere AI-utviklere at nye modeller utløste tidlige varslingsalarmer, eller at de ikke kunne utelukke at ytterligere evaluering ville vise at modeller har krysset kapabilitetsgrenser. Dette førte til at de anvendte skjerpede sikkerhetstiltak som et føre-var-tiltak (‡7, ‡33, ‡1121*). Frontier AI Safety Frameworks krever ofte en innledende kapabilitetsvurdering før risikoreduserende tiltak, samt en analyse av gjenværende risiko eller en sikkerhetssak, ofte basert på red-teaming, etter tiltak. Se Bord 3.5 for detaljert informasjon.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Beredskapsrammeverk 2 (‡1078*)
  Tilknyttede risikoer:
1. Biologiske og kjemiske evner
2. Cybersecurity-funksjoner
3. AI selvidforbedringsmuligheter
  Risikokategorier eller tilsvarende og tilhørende sikringstiltak:
- Høy: Kunne forsterke eksisterende spor til alvorlig skade (Krever sikkerhetskontroller og -tiltak)
- Kritisk: Kan introdusere enestående nye veier til alvorlig skade (Stans videre utvikling til spesifiserte sikkerhetstiltak og standarder for sikkerhetskontroller oppfyller en Kritisk-standard)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Policy for ansvarlig skalering 2.2 (‡991*)
  Tilknyttede risikoer:
1. CBRN-våpen
2. Autonom forskning og utvikling for AI (AI FoU)
3. Cyberoperasjoner (under vurdering)
  Risikotiere eller tilsvarende og tilhørende sikringstiltak:
  Nivåer for AI-sikkerhet (ASL)
- ASL-1: Ingen vesentlig katastrofal risiko
- ASL-2: Tidlige tegn på farlige kapabiliteter (Modeller må oppfylle ASL-2 distribusjons- og sikkerhetsstandarder)
- ASL-3: Betydelig økt risiko for katastrofalt misbruk (Modeller må oppfylle ASL-3-kravene til utrulling og/eller sikkerhet)
- ASL-4+: Fremtidige klassifiseringer (ikke ennå definert)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Frontier Safety Framework 3.0 (‡1040*)
  Tilknyttede risikoer:
1. Misbruk
    a. CBRN
    b. Cyber
    c. Skadelig manipulasjon
2. Forskning og utvikling innen maskinlæring
3. Feiljustering/ Instrumentell resonnering
  Risikoklasser eller tilsvarende og tilhørende beskyttelsestiltak:
  Kritiske kapabilitetsnivåer
    Kapabilitetsnivåene som, i fravær av avbøtende tiltak (sikkerhetssaker for distribusjoner og sikkerhetsavbøtende tiltak tilpasset RAND-sikkerhetsnivåene 2, 3 eller 4 (‡1122)), hvor AI-modeller eller -systemer kan utgjøre økt risiko for alvorlig skade. Kapabilitetsnivåene omfatter «tidlige varslingsvurderinger», med bestemte «varslingsterskler»
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Frontier AI Framework 1.1 (‡990*)
  Tilknyttede risikoer:
1. Cyber-sikkerhet
2. Kjemiske og biologiske risikoer
  Risiknivåer eller tilsvarende og tilhørende sikringstiltak:
  Risikoterskelnivåer
- Moderat (slipp med hensiktsmessige sikkerhetstiltak og avbøtende tiltak)
- igh (ikke slipp)
- Kritisk (stopp utvikling)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Frontmodell-sikkerhetsrammeverk (‡1123*)
  Tilknyttede risikoer:
1. Spredning av CBRN-våpen
2. Krenkende cyberoperasjoner
3. Automatisert AI-forskning og utvikling
  Risikotier eller tilsvarende og tilhørende sikringstiltak:
  Kritiske kapabilitetsgrenser
    Modellkapabiliteter som kan forårsake betydelig skade for offentligheten hvis de brukes feil. (Hvis tersklene er oppfylt eller oversteget, vil modellen ikke bli distribuert offentlig uten egnede tiltak for risikoredusering)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Rammeverk for styring av Frontier (‡1124*)
  Tilknyttede risikoer:
1. CBRN-våpen
2. Krenkende cyberoperasjoner
3. Avansert autonomi (inkludert AI R&D)
  Risikotierr eller tilsvarende og tilhørende tiltak:
  Risikoklasser
- Lav eller Middels (Distribusjon tillatt i tråd med kravene i Program for ansvarlig kunstig intelligens)
- Høy eller Kritisk (Ytterligere gjennomgang og tiltak)
påkrevd)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Vurdering av risiko for Frontier AI (‡1029*)
  Tilknyttede risikoer:
1. Cyberkriminalitet
2. CBRN
3. Overtalelse og manipulering
4. Ulovlig diskriminering i stor skala
  Risikonivåer eller tilsvarende og tilhørende beskyttelsestiltak:
  Risikoterskler – modellrisiko (MR)-score
- MR1 eller MR2 (vurderingsresultater dokumenteres av ingeniørteam)
- MR3 (Risikoavbøtende tiltak og evalueringsresultater dokumenteres av ingeniørteam, og gjennomgås periodisk)
- MR4 (En detaljert risikovurdering skal gjennomføres, og godkjenning fra leder for forretningsenhet er påkrevd)
- MR5 (En detaljert risikovurdering skal gjennomføres og godkjennes av et uavhengig utvalg, f.eks. NVIDIA sitt AI-etikkomité)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Rammeverk for sikre AI-frontmodeller (‡1125*)
  Tilknyttede risikoer:
1. Skadelig bruk (f.eks. skadevare, utnyttelse av barn seksuelt)
2. Skade ved vanlig, ikke-malisiøs bruk, f.eks. utdata som fører til et ulovlig diskriminerende resultat eller usikker generering av kode
  Risikokategorier eller tilsvarende og tilhørende tiltak:
  Sannsynlighet og alvorlighetsgrad av skade i kontekst
- Lav
- Medium
- Høy
- Svært høy
    (Risikoreduserende tiltak og sikkerhetskontroller er på plass for alle systemer og prosesser; ytterligere tiltak må tilpasses til AI-systemet og bruken der en modell er distribuert)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: Policy for AGI-valmishet (‡1127*)
  Tilknyttede risikoer:
1. Cyberkriminalitet
2. Automatisert AI-forskning og utvikling
3. Autonom replikasjon og adaptasjon
4. Biologiske våpen-bistand
  Risiknivåer eller tilsvarende og tilhørende sikkerhetstiltak:
  Kritiske kapabilitetsgrenser
    Kvantitative terskler for kapasitetsbenchmarks (Hvis de overskrides, gjennomfør farlige kapasitetsvurderinger, informasjons-sikkerhetstiltak og utplasseringsavbøtende tiltak, eller stans utviklingen)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: AGI Readiness Policy (‡1127*)
  Tilknyttede risikoer:
1. Cyberkriminalitet
2. Automatisert AI-forskning og utvikling
3. Autonom replikering og tilpasning
4. Biologiske våpen-bistand
  Risikotrinn eller tilsvarende og tilhørende sikringstiltak:
  Kritiske kapabilitetsgrenser
    Kvantitative terskler for kapabilitetsbenchmarks (Hvis overskredet, gjennomfør farlige kapabilitetsevalueringer, tiltak for informasjonssikkerhet og distribusjonsavbøtende tiltak, eller stans utvikling)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: AI-sikkerhetsrammeverk (‡1128*)
  Tilknyttede risikoer:
1. Tap av kontroll
2. Misbruk (f.eks. biokjemisk våpenproduksjon
  Risiknivåer eller tilsvarende og tilhørende sikkerhetstiltak:
  Risikoklasser
- Lav risiko (Distribuer AI-systemer, men utfør overvåking etterpå for å håndtere risiko)
- Risiko identifisert (Enten bare åpne KI-systemer for autoriserte brukere for å redusere risiko, eller utsette utrulling til ytterligere sikkerhetstiltak er på plass, avhengig av brukstilfellet)
- Høy risiko (Ikke ta i bruk AI-systemer)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Frontier AI Safety Framework (‡1129*)
  Tilknyttede risikoer:
1. Biologiske trusler
2. Offensiv cybersikkerhet
3. Autonom drift og avansert manipulasjon
  Risikonivåer eller tilsvarende og tilhørende sikringstiltak:
  Risikoklasser
- Nivå 1 (Grunnleggende sikkerhetstiltak for minimale risikoer og mulighet for å gi ut som åpen kildekode)
- Nivå 2 (sanntidsovervåking, promptfiltrering, atferdsavviksdeteksjon, tilgangskontroller, red-teaming og adversariale simuleringer)
- Nivå 3 (avanserte sikkerhetstiltak, inkludert red- teaming, fasevis utrulling, adversarial testing, kryptering, flerparts tilgangskontroller og zero-trust-arkitektur)
- Nivå 4 (Maksimale sikkerhetsprotokoller for høyrisiko-modeller og maksimale sikkerhetstiltak)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 3.5: Frontier AI sikkerhetsrammeverk
>white|black||9|11|br Den første serien med Frontier AI Safety Frameworks som er blitt lansert av en delmengde av AI-utviklerne som signerte Frontier AI Safety Commitments. Rammeverkene dekker lignende risikoer (med små variasjoner) og benytter ulike risikonivåer og tilnærminger for risikostyring.


>white|orangered|left|14|15.5|bb Effektiviteten til Frontier AI Safety Frameworks er usikker

Frontier AI Safety-frameworker kan fungere som risikostyringsverktøy under bestemte forutsetninger og for enkelte risikokategorier som har en troverdig vei til skade (‡1117). Samtidig drøfter flere analyser spørsmål knyttet til deres klarhet og omfang (‡111, ‡986) og om robustheten til AI-evner og risikoterskler (‡1031, ‡1130). Eksisterende rammeverk har ofte en tendens til å fokusere på en delmengde av risikodomener. Som et resultat får enkelte fremtredende risikoer, som ulovlig overvåking (‡1131, ‡1132) og ikke-samtykkende intime bilder (‡287), mindre vekt. I motsetning til tilnærminger til risikostyring fra andre sektorer, som luftfart eller kjernekraft (‡1133*), bruker Frontier AI Safety-frameworker typisk ikke eksplisitte kvantitative risikoterskler (‡1134).

Eksterne vurderinger av utvikleres etterlevelse av deres Frontier AI Safety Frameworks så langt er fortsatt begrensede, blant annet fordi de fleste rammeverkene er nye, offentlig tilgjengelig informasjon er sparsom, og det finnes ingen standardiserte eksterne revisjoner. Deres effektivitet vil også bli påvirket av hvor godt – og i hvilken grad – forpliktelsene blir gjennomført i praksis. Alene kan disse rammeverkene ikke sikre effektiv risikohåndtering, siden deres praktiske innvirkning avhenger av hvor godt – og i hvilken grad – de blir implementert. Til dags dato er de ikke fullt ut på linje med internasjonale standarder for risikohåndtering (‡1135). En studie av tidligere frivillige forpliktelser fant ujevn oppfyllelse på tvers av tiltak, noe som tyder på at etterlevelsen av frivillige forpliktelser sannsynligvis vil variere mellom selskaper og domener (‡1109).

Sett under ett representerer Frontier AI Safety Frameworks den mest detaljerte formen for frivillig organisatorisk risikohåndtering som for tiden er i bruk, men varierer betydelig i omfang, terskler og håndhevbarhet.

###@ Regulatoriske og styringsmessige initiativer

>white|orangered|left|14|15.5|bb Flere jurisdiksjoner har innført lover med krav til åpenhet

Flere tidlige regulatoriske tilnærminger introduserer juridiske krav som er ment å øke standardisering og transparens i risikostyring. EUs AI-forordning (EU AI Act), som trådte i kraft i 2024, fastsetter krav knyttet til transparens, opphavsrett og sikkerhet for generelle formålsmodeller for kunstig intelligens. I 2025 ble EUs atferds-/praksiskode for kunstig intelligens med generelle formål (EU General-Purpose AI Code of Practice) publisert for å støtte etterlevelse av disse forpliktelsene ved å gi veiledning om modell-dokumentasjon og opphavsrett, samt – for de mest avanserte modellene – risikostyringspraksiser som evalueringer, risikovurdering og risikoredusering, informasjonssikkerhet og rapportering av alvorlige hendelser (‡965).

Andre eksempler på nye regulatoriske krav inkluderer Sør-Koreas rammelov om utvikling av kunstig intelligens og etablering av tillit, som innfører krav til «høy-effekt» KI-systemer i kritiske sektorer (‡1136), og Californias SB 53, som fastsetter krav til åpenhet om sikkerhetsrammeverk og hendelsesrapportering (‡1104). Siden disse kravene er etablert så nylig, er det for tidlig å vurdere i detalj hvordan de vil påvirke praksis for risikostyring eller faktiske risikoutfall.

>white|orangered|left|14|15.5|bb Bredere styringsinitiativer tilbyr frivillig veiledning

Flere regionale og tverregionale styringsrammeverk artikulerer nå felles forventninger til håndtering av risikoer fra generell-purpose AI ved å gi ikke-bindende veiledning til beslutningstakere og organisasjoner. Kinas AI Safety Governance Framework 2.0, publisert i 2025, gir strukturert veiledning om risikokategorisering og mottiltak på tvers av AI-utviklings- og distribusjonsprosessen (‡1137). ASEAN-medlemsstatene publiserte «ASEAN Expanded Guide on AI Governance and Ethics (Generative AI)», som gir veiledning om generell-purpose AI-styring og etikk, og er ment å støtte økt policy-tilpasning på tvers av ASEAN-medlemsstatene (‡1138). I tillegg beskriver ekspertdrevne initiativer som Singapore Consensus, utviklet av AI-forskere fra flere land, forskningsprioriteringer for generell-purpose AI-sikkerhet på tvers av risikovurdering, utvikling og kontroll (‡690).

###@ Oppdateringer

Siden publiseringen av forrige rapport (januar 2025) har risikostyringslandskapet for general-purpose AI utviklet seg, med publisering av nye ressurser som EUs General-Purpose AI Code of Practice, G7 HAIP Reporting Framework, Kinas nasjonale AI Safety Governance Framework 2.0 og ulike AI-utvikleres Frontier AI Safety Frameworks. Disse initiativene beskriver tilnærminger og praksiser som brukes av AI-utviklere for å håndtere risikoene forbundet med systemer for general-purpose AI (‡1115). Det er betydelige variasjoner på tvers av Frontier AI Safety Frameworks og på tvers av HAIP- åpenhetsrapporter (‡1103), noe som gjenspeiler forskjeller i organisatoriske praksiser, risikoprioritering og den tidlige fasen i økosystemet for risikostyring for general-purpose AI. Et tillitsbasert økosystem der ulike AI-aktører bidrar med komplementære risikostyringspraksiser på tvers av livsløpet, kan bidra til effektiv risikostyring (‡690).

###@ Bevismangler

Det er mangel på evidens for: hvordan man måler alvorlighetsgrad, utbredelse og tidsramme for nye risikoer; i hvilken grad disse risikoene kan reduseres i virkelige kontekster; og hvordan man effektivt kan oppmuntre eller håndheve at risikoreduserende tiltak tas i bruk på tvers av ulike aktører. Mer forskning er nødvendig for å forstå hvor utbredt ulike risikoer er, og hvor mye de varierer på tvers av ulike regioner i verden, særlig for regioner som Asia, Afrika og Latin-Amerika som raskt digitaliseres. Ettersom AI-modeller gis økende grad av handlefrihet og autoritet, og kunnskapsstatusen innen generell-purpose AI-risikoer utvikles, vil også risikostyringstilnærminger måtte endres (‡639, ‡1139).

Visse risikoreduserende tiltak blir stadig mer populære (‡690, ‡956), men mer forskning er nødvendig for å forstå hvor robuste risikoreduserende tiltak og sikkerhetstiltak er i praksis for ulike samfunn og AI-aktører (inkludert for små og mellomstore bedrifter). Økt tilgang til data om reell utplassering og bruk av modeller er relevant for slike vurderinger. Videre varierer risikostyringsarbeidet i dag svært mye på tvers av ledende AI-selskaper. Det er blitt hevdet at utviklernes insentiver ikke er godt tilpasset grundige risikovurderinger og risikostyring (‡934). Det finnes fortsatt et kunnskapsgap knyttet til i hvilken grad ulike frivillige forpliktelser faktisk oppfylles, hvilke hindringer selskaper møter når de fullt ut skal følge forpliktelsene, og hvordan de integrerer Frontier AI Safety Frameworks i bredere praksiser for risikostyring i AI.

###@ Utfordringer for beslutningstakere

Viktige utfordringer omfatter å finne ut hvordan man skal prioritere de ulike risikoene som generell formål-AI medfører, å klargjøre hvilke aktører som er best posisjonert til å redusere dem, og å forstå insentiver og begrensninger som former deres handlinger. Bevis tyder på at politikkutformere for øyeblikket har begrenset tilgang til informasjon om hvordan AI-utviklere og -utplasserere tester, evaluerer og overvåker fremvoksende risikoer, og om hvor effektivt ulike risikoreduserende tiltak er (‡1140). Forskere og politikkutformere har diskutert åpenhetstiltak og mer systematisk hendelsesrapportering som mulige måter å informere om risikoprioritering, fremme tillit og gi insentiver til ansvarlig utvikling (‡957). I praksis innebærer risikohåndtering flere aktører langs AI-verdikjeden – som dataleverandører og skyleverandører, modellutviklere og plattformer for hosting av modeller – og hver har ulike muligheter til å vurdere og håndtere ulike risikoer (‡1141). Begrenset informasjonsdeling mellom disse aktørene gjør det vanskelig å avgjøre hvilke risikoer som er mest sannsynlige eller mest konsekvensfulle, særlig når man tar hensyn til samfunnsmessige virkninger påfølgende ledd.

