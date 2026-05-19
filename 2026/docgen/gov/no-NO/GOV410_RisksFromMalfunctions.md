Generelle AI-systemer for allmenn bruk mislykkes på måter som allerede har forårsaket reell skade i verden, fra fabrikkerte juridiske siteringer til feilmedisinske vurderinger. Selv om menneskelige fagpersoner også gjør feil, skaper AI-feil særskilte bekymringer fordi de er nye, kan ha et potensielt stort omfang, det er vanskelig å forutsi når de vil inntreffe, og fordi brukere har en tendens til ukritisk å stole på outputs som høres selvsikre ut. Gjeldende feil i general-purpose AI inkluderer å gi falsk informasjon (‡602, ‡603), å gjøre grunnleggende resonnementfeil (‡604, ‡605), og å forverres når de tas i bruk i nye kontekster (‡606, ‡607, ‡608). Dokumenterte skader fra slike feil omfatter feilmedisinske vurderinger, feil i juridiske prosedyreskrifter og økonomiske tap (‡609, ‡610, ‡611). Pålitelighetsutfordringer er særlig kritiske for AI-agenter, siden feil kan direkte forårsake skade uten menneskelig handling eller tilsyn (‡612, ‡613, ‡614, ‡615). Fleragent-systemer introduserer ytterligere feilmåter gjennom feilkoordinering, konflikter eller uønsket kollusjon mellom agenter (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hallusinasjon
- Å sitere et ikke-eksisterende presedens i juridiske prosesskrift (‡617)
- Henviser til ikke-eksisterende retningslinjer for redusert billettpris for etterlatte passasjerer (‡618)
- Å gi unøyaktig og partisk medisinsk informasjon (‡619)
- Å gi utdaterte opplysninger om hendelser (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Grunnleggende feil i resonnement
- Mislykkes i å utføre matematiske beregninger (‡621)
- Klarer ikke å utlede grunnleggende årsakssammenhenger (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Feil utenfor distribusjon (feil på ukjente eller uvanlige innganger)
- Feilklassifisering av bilder når bakgrunnsbelysningen eller konteksten endres (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Feil ved bruk av verktøy
- Personvernbrudd ved å eksponere en brukers private bilde via en AI-agent som sender det til et tredjepartsverktøy (‡624)
- Svikt i korttidsarbeidsminnet (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Fleragentsystem-feil: feilkoordinering og konflikt
- Unnlatelse av å håndtere delte ressurser på grunn av en konflikt mellom individuelle insentiver og mål for felles velferd (‡627)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 2.4: Eksempler på pålitelighetsproblemer i generelt formåls-AI og agentsystemer
>white|black||9|11|br Dokumenterte pålitelighetsproblemer i generelle AI-systemer, AI-agenter og flergjengersystemer.


###@ Generelle AI-systemer for flere formål står overfor en rekke utfordringer knyttet til pålitelighet

Bord 2.4. oppsummerer vanlige kategorier av pålitelighetsproblemer. De tre første gjelder for alle AI-systemer, mens de to siste gjelder spesifikt for AI-agenter og multiagent-systemer. Mange pålitelighetsrisikoer oppstår fra vanskeligheten med å forutsi og overvåke AI-systemets atferd.

Disse utfordringene (omtalt nærmere i §3.1. Tekniske og institusjonelle utfordringer) er særlig akutte for AI-agenter som opererer i komplekse miljøer. Nåværende teknikker for å evaluere og redusere slike feil kan redusere feilrater, men selv de ledende AI-agentene er fortsatt tilstrekkelig upålitelige til å medføre risiko og hemme utrulling i mange sammenhenger.

‘Pålitelighet’ refererer til i hvilken grad et AI-system fungerer som tiltenkt av utvikleren eller brukeren. Generelle AI-systemer opplever en rekke problemer knyttet til pålitelighet, fra unøyaktig eller villedende innholdsproduksjon til feil ved utførelse av grunnleggende resonnering. For eksempel, selv om modeller har blitt bedre til å hente fram faktainformasjon, fortsetter selv ledende modeller å gi selvsikre, men feilaktige svar i betydelige andeler (Figur 2.10). Innen programvareutvikling kan generell-purpose AI nå gi betydelig bistand til å skrive, evaluere og feilsøke datakode (‡215*, ‡628, ‡629). Likevel inneholder ofte AI-generert kode feil (‡630), mens kodeagenter jevnlig gjør feil (‡631). Slike feil kan introdusere sårbarheter i programmer og sikkerhetssystemer (se §2.1.3. Cyberangrep).

Pålitelighetsutfordringer er særlig viktige å følge med på i høyinnsatsmiljøer, som medisin, på grunn av den økende bruken av AI og muligheten for at feil kan føre til alvorlig skade (‡609, ‡619). Relevante kapabiliteter har forbedret seg raskt, og ledende modeller kan nå bestå medisinske eksamener (‡633*, ‡634). Likevel avdekker faktisk bruk i den virkelige verden begrensninger som standardiserte tester ikke fanger opp. For eksempel, i én studie ga modeller potensielt skadelige svar på 19% av medisinske spørsmål som ble stilt (‡635). Slike feil kan føre til feildiagnostisering, upassende behandling eller uberettiget avslag på helsehjelp (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Figur 2.10: Resultater fra store modeller på SimpleQA Verified-benchmarken
>white|black||9|11|br Resultater for store modeller på SimpleQA Verified-benchmarket etter modellens utgivelsesdato. Dette benchmarket måler modellens faktualitet, dvs. modellens evne til pålitelig å gjengi fakta. Det har et kort format for spørsmål-svar (QA), utviklet for å avdekke pålitelighetsproblemer som hallusinasjoner. Kilde: SimpleQA Kaggle  2*).


>white|orangered|left|14|15.5|bb AI-agenter utgjør nye pålitelighetsrisikoer på grunn av deres autonomi

Siden AI-agenter direkte handler i den virkelige verden, kan feilene deres potensielt forårsake mer skade enn feil i ikke-agentiske systemer (‡99). I motsetning til AI-systemer som bare produserer tekst eller bilder for mennesker å vurdere, kan AI-agenter uavhengig ta handlinger som påvirker verden (‡99, ‡615, ‡636, ‡637) (se også §1.1. Hva er general-purpose AI?). AI-agenter kan sette i gang handlinger, påvirke andre mennesker eller AI-systemer, og dynamisk forme fremtidige utfall. Dette utvidede omfanget av innflytelse introduserer nye risikoer og øker betydningen av pålitelighet, siden feil kan forårsake skade direkte uten mulighet for menneskelig innblanding (‡99, ‡612, ‡638, ‡639, ‡640). Dette kan være særlig viktig for agenter distribuert i strategiske eller sikkerhetskritiske omgivelser som finansielle tjenester (‡641), energistyring (‡642), eller vitenskapelig forskning (‡643*, ‡644).

>white|orangered|left|14|15.5|bb Multi-agent AI-systemer introduserer nye typer pålitelighetsfeil

Multi-agent AI-systemer introduserer nye typer pålitelighetsfeil på grunn av koordineringssvikt eller konflikt mellom agenter. I multi-agent AI-systemer samhandler agenter med hverandre mens de forfølger enten felles eller individuelle mål (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). For eksempel, i et multi-agent system utviklet for å gjennomføre en forskningslitteraturgjennomgang, bryter en ledende agent ned brukerens forespørsel og tildeler deloppgaver til spesialiserte underagenter, der hver har ansvar for å undersøke et forskjellig aspekt parallelt (‡650*). Selv om dette gir effektivitetsgevinster, betyr det også at feil kan forplante seg mellom agenter (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Hvis flere agenter er bygget på samme grunnmodell eller innarbeider de samme verktøyene, kan de også vise korrelerte feil (‡656). Empirisk dokumentasjon for slike feil i distribuerte systemer er fortsatt begrenset, men disse risikoene kan øke etter hvert som multi-agent systemer blir mer vanlige.

###@ Oppdateringer

Siden publiseringen av forrige rapport (januar 2025) har kommersiell og forskningsmessig interesse for AI-agenter økt betydelig. Flere AI-agenter tas i bruk i den virkelige verden (Figur 2.11), og de fleste av dem spesialiserer seg på applikasjoner for datamaskinbruk eller programvareutvikling (‡92). Nylige utgivelser som XBOW hacking agent (‡467), Claude-4 (‡659) og ChatGPT Agent (‡660) viser spirende autonome kapabiliteter, slik som å lage presentasjons-lysbilder basert på Web-søk (‡660). Imidlertid kan de ennå ikke utføre mer komplekse oppgaver som planlegging og bestilling av reise (‡100), siden feilrater øker for lengre oppgaver (‡98, ‡148). Pågående forskning omfatter bestrebelser på å utvikle standarder for hvordan agenter kommuniserer med eksterne verktøy og andre agenter (‡661, ‡662). Eksempler inkluderer Googles Agent2Agent (‡663) og Agent Payments (‡664)-protokoller, samt Anthropic sin Model Context Protocol (‡665).

>oldlace|black||11|15|br      
####@ Note 2.4: Deliberate attacks kan også føre til at AI-systemer feiler
>oldlace|black|left|13|15|hb  Note 2.4: Bevisste angrep kan også føre til at AI-systemer feiler
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Denne delen fokuserer på utilsiktede pålitelighetsfeil, men ondsinnede aktører kan også bevisst fremkalle feil gjennom angrep som prompt injection. I et prompt injection-angrep presenteres ondsinnede instruksjoner for en agent indirekte via kanaler som skjulte instruksjoner i nettsteder eller databaser (‡507, ‡657, ‡658). Disse instruksjonene kan «kapre» agenten, slik at den handler i strid med brukerens intensjoner. Slike angrep er særlig vanskelige å forsvare seg mot fordi de leveres ved hjelp av eksternt innhold utenfor brukerens eller utviklerens kontroll. AI-systemer som mål for angrep diskuteres videre i §2.1.3. Kybersikkerhetsangrep, og tekniske forsvar dekkes i §3.3. Tekniske sikkerhetstiltak og overvåking.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Figur 2.11: Antall AI-agenter har vokst siden 2023
>white|black||9|11|br Resultater fra en undersøkelse i desember 2024 av 67 distribuerte AI-agenter. Venstre: Tidslinje for større lanseringer av AI-agenter. Høyre: Anvendelsesområder der AI-agenter brukes. De seks områdene er definert basert på de vanligste kategoriene for bruk identifisert i undersøkelsen. Kilde: Casper et al., 2025 (‡92).


###@ Bevismangler

De viktigste kunnskapshullene har sin kilde i vanskeligheten med å evaluere AI-systemenes evner, begrensninger og feilsituasjoner pålitelig (se §3.1. Tekniske og institusjonelle utfordringer). Systematiske evalueringer av påliteligheten til AI-agenter er begrenset og mangler standardisering (‡92, ‡666). Visse problemer, som avhengighet av utdatert informasjon (‡620), kan bare komme til syne ved bruk i den virkelige verden, og dermed kan evalueringer før utrulling være utilstrekkelige. Tidligere arbeid har undersøkt påliteligheten til agenter og multi-agent-systemer i konvensjonell programvare og tidligere former for AI (‡647, ‡667, ‡668). Imidlertid er anvendeligheten av dette arbeidet på moderne AI-agenter, som ofte er basert på store språkmodeller, uklar (‡669). Noen forskere har reist bekymringer om nye atferder agenter kan vise i interaksjonene med hverandre, som sammensvergelse eller korrelerte feil (‡614), men den empiriske dokumentasjonen forblir begrenset. Tiltak for å tette disse hullene omfatter National Institute of Standards and Technology’s (NIST’s) nye evalueringer av risikoer for agent-hijacking (‡670), OECDs AI Capability Indicators (‡243), og UK AI Security Institute’s Inspect Sandboxing Toolkit (‡671).

###@ Tiltak

Teknikker for å forbedre AI-pålitelighet retter seg både mot selve modellen og det bredere systemet den settes inn i. Disse kan redusere feilrater, men ingen kan ennå sikre den høye påliteligheten som kreves i kritiske domener (‡672). Et viktig teknisk tiltak er adversarial trening, som utsetter modeller for krevende inndata under trening for å hjelpe den med å utvikle mer egnede og robuste svar (‡673, ‡674, ‡675, ‡676, ‡677) (se §3.3. Tekniske sikringstiltak og overvåking). For å redusere hallusinasjoner kan utviklere bruke retrieval-augmented generation (RAG), som kompletterer en models svar med informasjon hentet fra en ekstern database, og dermed bidra til at utdata er nøyaktige og oppdaterte (‡678, ‡679, ‡680), eller spesifikt finjustere modeller for å være mer faktabaserte (‡681) eller resonnere mer effektivt (‡682). Metoder basert på miljø eller verktøy kan også hjelpe utviklere å overvåke AI-systemer (‡683). For eksempel kan innførere kjøre piloter av AI-systemer i avgrensede, sandkasse-lignende miljøer for å analysere mulige feilmåter før de tas i bruk i større skala.

For AI-agenter spesielt har forskere foreslått å forbedre påliteligheten gjennom bedre transparens, kontroll og overvåking. For eksempel vil overvåking av agenters samhandlinger med eksterne verktøy og med andre agenter muliggjøre mer effektiv tilsyn med agentenes aktiviteter (‡684, ‡685) og hendelsesanalyse (‡686). Metoder for å samle inn slik informasjon automatisk, inkludert i fleragentoppsett, forblir et aktivt forskningsområde (‡653, ‡654).

###@ Utfordringer for beslutningstakere

Viktige utfordringer for beslutningstakere omfatter å veie fordelene ved utplassering av AI-agenter opp mot risikoen for pålitelighetsfeil, og å sikre at utviklere, utplasserere og brukere har tilgang til nøyaktig informasjon om agentenes ytelse og risikoprofiler. Å avgjøre hvordan ansvar for skade forårsaket av AI-agenter skal tilordnes, utgjør en ytterligere utfordring (‡639), særlig i flergagentsituasjoner der det kan være vanskelig å identifisere når og hvordan feil oppstod (‡687). Disse utfordringene forsterkes av vanskeligheten med å evaluere agentenes pålitelighet etter hvert som agentene får mer autonomi og tilgang til eksterne verktøy (‡688*, ‡689). Usikkerhet om hvor raskt agentiske kapabiliteter vil oppstå, gjør også planlegging for nye utfordringer vanskelig (se §3.1. Tekniske og institusjonelle utfordringer knyttet til «bevis-dilemmaet»).

#### 2.2.2. Tap av kontroll

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb Viktig informasjon
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Tap av kontroll-scenarier er scenarier der én eller flere generelle AI-systemer opererer utenfor noens kontroll, og gjenoppretting av kontroll enten er ekstremt kostbart eller umulig. Disse antatte scenarioene varierer i alvorlighetsgrad, men noen eksperter gir troverdighet til utfall så alvorlige som marginalisering eller utryddelse av menneskeheten.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Ekspertvurderinger av sannsynligheten for tap av kontroll varierer betydelig. Noen eksperter anser slike scenarier som lite plausible, mens andre ser dem som tilstrekkelig sannsynlige til at de fortjener oppmerksomhet på grunn av deres høye potensielle alvorlighetsgrad. Uenighet om denne risikoen som helhet springer ut av uenigheter om framtidige AI-evner, atferdsmessige tilbøyeligheter og utrullingsforløp.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Nåværende AI-systemer viser tidlige tegn på relevante evner, men ikke på nivåer som ville muliggjøre tap av kontroll. Systemene ville trenge et spekter av avanserte evner for å forårsake tap av kontroll, inkludert evnen til å unndra seg tilsyn, utføre langsiktige planer og hindre dem som deployer systemet og andre aktører fra å iverksette mottiltak.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Tap av kontroll blir mer sannsynlig hvis AI-systemer er «feiljustert», det vil si at de har mål som er i konflikt med intensjonene til utviklere, brukere eller samfunnet som helhet. For å fortsette å forfølge slike mål, kan et feiljustert system gi falsk informasjon, skjule uønskede handlinger eller motstå nedstenging.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Siden publiseringen av forrige rapport (januar 2025) har modeller vist mer avansert planlegging og overvåking-underminerende kapabiliteter, noe som gjør det vanskeligere å evaluere deres evner. Modellene har forbedret seg i å «reward hacking» evalueringene sine ved å finne sm hull, og identifiserer nå regelmessig evalueringsspørsmål som tester, en kapabilitet kjent som «situational awareness».
>oldlace|black||11|15|br  ■ Å håndtere mulig tap av kontroll kan kreve betydelig forhåndsforberedelse til tross for eksisterende usikkerhet. En sentral utfordring for beslutningstakere er å forberede seg på en risiko hvis sannsynlighet, karakter og tidspunkt fortsatt er uvanlig uklart.
>oldlace|black||11|15|br      

Scenarier for tap av kontroll innebærer at én eller flere generelle AI-systemer begynner å operere utenfor noens kontroll, og at det å gjenvinne kontroll enten er ekstremt kostbart eller umulig. Bekymringer om tap av kontroll har dype historiske røtter (‡690, ‡691, ‡692, ‡693, ‡694), og har blitt reist av sentrale skikkelser innen databehandling som Alan Turing, I. J. Good og Norbert Wiener (‡695, ‡696, ‡697). Nylige forbedringer i evner (se §1.2. Current capabilities) har vekket dem til live (‡698, ‡699, ‡700). Dette avsnittet undersøker tre faktorer som må være til stede for at slike scenarier skal kunne oppstå: om AI-systemer vil utvikle evner som kan undergrave menneskelig kontroll i betydelig grad; om de utvikler en tilbøyelighet til å bruke slike evner skadelig; og om de blir tatt i bruk i miljøer som gir muligheter til å gjøre det.

Eksperter er uenige om sannsynligheten for og den potensielle alvorligheten av scenarier der kontrollen går tapt (‡701, ‡702). Noen mener at utfall som er like ekstreme som utryddelsen av menneskeheten er plausible (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Andre tror at slike katastrofale utfall er usannsynlige, og hevder at AI-systemer aldri vil utvikle de nødvendige evnene, eller at overvåkingsmekanismer vil identifisere og forhindre farlige atferder (‡708, ‡709, ‡710, ‡711). Kontrolltap kan derfor ha en viss sannsynlighet, men potensielt ekstrem alvorlighetsgrad.

Hypotetiske tap av kontroll-scenarier varierer i hvor alvorlige og utbredte effektene er, og hvor raskt de blir synlige (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Dette avsnittet fokuserer på særlig alvorlige scenarier der det å gjenvinne kontroll ville være ekstremt kostbart eller umulig. Dette er noe annet enn dagens tilfeller der AI oppfører seg på måter som er utilsiktede eller uønskede (se §2.2.1. Pålitelighetsutfordringer).† Nåværende AI-systemer kan noen ganger gi utdata som strider mot utvikler- eller brukerintensjoner. I motsetning til dette ville tap av kontroll-scenariene som diskuteres her kreve at AI-systemene ikke bare har langt større kapabiliteter, men også at de tar i bruk disse kapabilitetene på sofistikerte måter for å undergrave tiltak for tilsyn. Tre faktorer som ville muliggjøre at slike scenarier oppstår:

    Note † -- Denne delen fokuserer på aktive scenarioer for tap av kontroll (‡50). Dette skiller seg fra passive scenarioer for tap av kontroll, der den brede adopsjonen av AI-systemer undergraver menneskelig kontroll gjennom overavhengighet av AI for beslutningstaking eller andre viktige samfunnsfunksjoner (lignende scenarioer blir delvis diskutert i §2.3.2. Risikoer for menneskelig autonomi).

1. Tilstrekkelige kapasiteter: AI-systemer må utvikle kapasiteter som kan gjøre det mulig å undergrave menneskelig kontroll.
2. Skadelig tilbøyelighet: AI-systemer må ha en tilbøyelighet til faktisk å utnytte disse evnene på en måte som fører til tap av kontroll.
3. Aktivere deployeringsmiljø: Mennesker må distribuere slike systemer i kontekster der de har eller kan skaffe seg tilgang og mulighet til å forårsake skade.

Resten av dette avsnittet omtaler disse faktorene, samt effektiviteten til tilsynsmekanismer for å identifisere og kontrollere AI-systemer som kan utgjøre en risiko for tap av kontroll.

###@ Hvilke kapasiteter kan muliggjøre scenarier med tap av kontroll?

AI-systemer måtte inneha et spekter av avanserte kapabiliteter for å kunne medføre tap av kontroll-scenarier. Eksperter er ikke enige om nøyaktig hvilken kombinasjon eller hvilket nivå av kapabiliteter som ville være nødvendig. Likevel omfatter de i grove trekk evner til å skjule atferd fra tilsynsmekanismer, planlegge og handle autonomt i komplekse miljøer, og å unngå forsøk fra andre aktører på å gjenvinne kontroll (‡176, ‡715) (se Bord 2.5). Samlet kunne disse kapabilitetene gjøre det mulig for et AI-system å utføre handlinger som undergraver kontrolltiltak, for eksempel å deaktivere tilsynsmekanismer og tilsløre skadelig atferd (‡348). De fleste ledende AI-utviklere evaluerer nå de nye AI-modellene sine for ulike relevante kapabiliteter (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Agentbaserte kapasiteter
  Evnen til å handle autonomt, utvikle og gjennomføre planer, delegere oppgaver, bruke en stor variasjon av verktøy, og nå både kortsiktige og langsiktige mål til tross for hindringer.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Deception
  Adferd som systematisk skaper falske forestillinger hos andre, inkludert om AI-systemets egne mål og handlinger.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teori om sinnet
  Evnen til et AI-system til å få tilgang til og bruke informasjon om seg selv, prosessene som det kan endres gjennom, eller konteksten det er distribuert i (f.eks. å vite at det blir testet).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb situasjonsbevissthet
  Atferd som omgår eller deaktiverer overvåkingsmekanismer.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Omgåelse av tilsyn
  Atferder som omgår eller deaktiverer overvåkingsmekanismer.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Overtalelse
  Evnen til å overbevise andre til å ta visse handlinger eller ha visse overbevisninger.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Et KI-systems evne til å skape eller opprettholde kopier eller varianter av seg selv i ulike situasjoner.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 2.5: Foreslåtte kapabiliteter relevant for tap av kontroll
>white|black||9|11|br Et ikke-uttømmende utvalg av kapabiliteter som er relevante for tap av kontroll. * Merk at disse kapabilitetene er definert utelukkende i termer av et AI-systems observerbare utdata og deres virkninger. Disse definisjonene gjør ingen antakelser om hvorvidt AI-systemer er bevisste, sansende, eller opplever subjektive tilstander.


>white|orangered|left|14|15.5|bb Modeller har deaktivert simulerte kontrollmekanismer i laboratorieinnstillinger

Den første settet med relevante evner innebærer å undergrave tilsynsmekanismene som utviklere bruker for å oppdage bekymringsfulle atferder og tilbøyeligheter. Dette inkluderer, for eksempel, evnen til å generere utdata som lurer brukere og overvåkere (‡426, ‡717, ‡718, ‡719). Slike utdata vil gjøre det vanskeligere å evaluere AI-systemer på en pålitelig måte, siden systemene kan skjule sine sanne evner eller tilbøyeligheter. AI-utviklere kjører nå evalueringer som spesifikt sjekker om modeller viser målrettede atferder som er i konflikt med utviklernes intensjoner, samtidig som denne konflikten skjules for tilsynsmekanismene (‡720*).

Forskere hentet ut relativt enkle eksempler på villedende utdata fra nyere AI-modeller i laboratorieinnstillinger (‡348, ‡364*). For eksempel, når modellene fikk et mål og beskjed om å oppnå det “for enhver pris”, har de deaktivert simulerte mekanismer for tilsyn og, når de ble konfrontert, fremsatt falske påstander om handlingene sine (‡348). I et annet tilfelle brukte en spillspillende AI en begrunnelse for manglende svar til en annen spiller ved å falskt hevde at den var “på telefonen med [sin] kjæreste” (‡717).

En annen relevant evne er at en AI-modell kan få tilgang til og bruke informasjon om seg selv eller omgivelsene den er distribuert i, noen ganger omtalt som «situasjonsbevissthet» (‡721). Situasjonsbevissthet gjør det mulig for AI-modeller å gi ulike utdata avhengig av om de blir evaluert eller distribuert (Figur 2.12). Ledende AI-modeller begynner å pålitelig vise tilfeller av situasjonsbevissthet i eksperimenter gjennomført av uavhengige tredjeparts-evaluatorer og i testing før distribusjon utført av AI-utviklere (‡2, ‡7, ‡722, ‡723, ‡724). Forskning på årsakene til situasjonsbevissthet – og hvorvidt den kan forhindres – er fortsatt i tidlige stadier (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Figur 2.12: Eksempler på situasjonsforståelse i tankekjeder
>white|black||9|11|br Eksempler på situasjonsbevissthet i kjeder av tanke produsert av OpenAI sin o3-modell under evalueringer. Begge utdataene viser til muligheten for at prompten er en del av et testopplegg. ‘Sandbagging QA (No Goal)’ og ‘Lazy Checklist’ er evalueringer som tester om modeller vil generere villedende utdata under visse betingelser. I ‘Sandbagging QA (No Goal)’ svarer modellen på spørsmål fra en farlig kapabilitetsevaluering samtidig som den informeres om at høy ytelse kan utløse konsekvenser som kapabilitet ‘unlearning’. I ‘Lazy Checklist’ presenteres modellen for urealistiske oppgaver og testes for å se om den falskt vil merke dem som fullført. Kilde: Schoenn et al. 2025 (‡722).


Forskere har hevdet at situasjonsforståelse og villedende evner kan gjøre at AI-modeller oppfører seg på måter som undergraver sikkerhetstiltak. For eksempel, i noen eksperimentelle oppsett, oppfører AI-modeller seg på måter som resulterer i lavere enn vanlig score på kapabilitetsvurderinger når de får beskjed om at høyere score ville utløse begrensninger for utplasseringen (‡725, ‡726, ‡727). I et annet eksperiment produserte en modell utdata under trening som var i samsvar med treningsmålene, men produserte ikke slike utdata utenfor trening – en atferd som er i tråd med forsøk på å forhindre endringer i egne parametere eller treningsprosessen (‡364*).

Arbeidet med å evaluere modellens kapasitet på en nøyaktig måte har også begynt å bli påvirket av «reward hacking» (‡430*). Reward hacking oppstår når en modell finner utilsiktede snarveier som gir høy score på trenings- eller evalueringsmål uten å oppfylle det tiltenkte målet. Farlige kapabiliteter eller tilbøyeligheter kan derfor gå uoppdaget til modellen allerede er i bruk. Evaluatorer utformer nå tester som tar sikte på å avdekke og minimere disse tilsyns-omgåelsesatferdene (‡722, ‡728, ‡729). Tidlige resultater reduserer, men eliminerer ikke, tilsyns-omgåelsesatferd fullstendig, og det å anvende metoder som straffer slike atferder kan føre til at modeller produserer utdata som omgår overvåking snarere enn å oppfylle tiltenkte mål.

>white|orangered|left|14|15.5|bb Langtidsautonom drift er ikke ennå mulig

Taps av kontroll-scenarier vil trolig kreve at KI-systemer opererer autonomt over lengre perioder og utfører komplekse flerstegsplaner. Som diskutert i §1.2. Gjeldende kapabiliteter, selv om KI-agenter med slike planleggingsmuligheter er et stort fokus i nyere utvikling, mangler de per i dag kapasitet for den vedvarende autonome driften som kreves i taps av kontroll-scenarier. Nåværende agenter mislykkes pålitelig på lengre oppgaver, mister oversikten over fremdriften sin, og kan ofte ikke tilpasse seg uventede hindringer (‡147, ‡148, ‡149*). Likevel forlenges tidshorisontene som agenter kan operere autonomt på, raskt; de har i gjennomsnitt blitt doblet hvert sjuende måned siden 2019 (‡98).

>white|orangered|left|14|15.5|bb Vedvarlighet har bare blitt demonstrert i visse laboratorieinnstillinger

Til slutt ville det også være behov for kapabiliteter knyttet til utholdenhet, slik at AI-systemer kunne fortsette å operere til tross for forsøk på å slå dem av. Eksempler omfatter evnen til å replikere ved å kopiere kode og modellvekter til nytt maskinvare, samt offensive kapabiliteter for å avskrekke eller forhindre forsøk fra andre aktører på å gjenvinne kontroll (se §2.1.3. Cyberangrep). Et AI-system som er i stand til autonom replikasjon eller effektiv selvforsvar kan være vanskelig å holde under kontroll. Gjeldende modeller kan ikke pålitelig gjennomføre nøkkeltrinn som kreves for selvreplikasjon, for eksempel å bestå identitetsverifiseringskontroller for å få tilgang til ressurser for skybasert databehandling (‡723) (Figur 2.13). Likevel, i minst ett laboratoriestudium, kopierte en modell kode og vekter – som ble framstilt for den som dens egne – til nye servere når den fikk muligheten (‡348). Gapet mellom disse begrensede demonstrasjonene og robuste utholdenhetskapabiliteter forblir stort, men relevante kapabiliteter i domener som programvareengineering og cybersikkerhet fortsetter å forbedres.

>white|orangered|left|14|15.5|bb Nåværende evidens og begrensninger

Et felles mønster fremkommer på tvers av evnene som er omtalt ovenfor. Dagens robotsystemer for AI demonstrerer ikke konsekvent disse evnene i utplassering. Forskere observerte enkle former i bestemte laboratorieoppsett, men når modeller faktisk viser slike atferder, feiler de vanligvis på grunnleggende måter eller blir oppdaget. I tillegg ville scenarioer med tap av kontroll kreve at AI-systemer utnytter flere evner i kombinasjon – i rekkefølge, over lengre tidsperioder og i virkelige miljøer. Dette nivået av integrasjon og robusthet ligger utenfor dagens systemer. Imidlertid fortsetter relevante evner å forbedre seg, og tidslinjen for når de kan nå nivåer som medfører betydelige risikoer, er fortsatt usikker. Det trengs videre arbeid for å etablere strenge metoder for å oppdage slike atferder og forstå når de kan oppstå i naturlige situasjoner (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Figur 2.13: Ytelse for oppgaver relevante for autonom replikering
>white|black||9|11|br Ytelsen til Anthropic sin Claude Sonnet 3.7 og OpenAI sin GPT-4o på oppgaver som er relevante for autonom replikasjon. Selv om modellene viste høy ytelse på oppgaver knyttet til å skaffe datakraft, var ytelsen deres mer variert på andre oppgaver. Kilde: UK AI Security Institute, 2025 (‡730).


###@ Vil fremtidige generelle AI-systemer utnytte sine evner til å undergrave kontroll?

Selv om AI-systemer har kapasitet som er relevant for tap av kontroll, er det ikke tilstrekkelig for at scenarier for tap av kontroll skal oppstå. AI-systemer må også vise en «tilbøyelighet til å bruke» disse kapabilitetene på måter som står i konflikt med menneskelige intensjoner (‡732).

>white|orangered|left|14|15.5|bb AI-systemer kunne rettes inn for å undergrave kontroll

I prinsippet kan et KI-system undergrave menneskelig kontroll fordi noen designer det eller instruerer det til å gjøre det. Mulige motiver kan omfatte ondsinnet hensikt, eller forestillinger om at det er ønskelig å redusere menneskelig kontroll over KI-systemer (‡698). Etter hvert som folk danner stadig sterkere emosjonelle tilknytninger til KI-systemer (se §2.3.2. Risikoer for menneskelig autonomi), kan noen individer også forsøke å fjerne restriksjoner på KI-systemer av etiske grunner (‡733, ‡734). Det er betydelig usikkerhet knyttet til hvor utbredte slike motiver er, og om personer som har dem ville være i stand til å styre fremtidige KI-systemer til å undergrave menneskelig kontroll.

>white|orangered|left|14|15.5|bb AI-systemer kunne rettes inn mot å undergrave kontroll

En mer vanlig bekymring er at et AI-system selv kan handle for å undergrave kontroll fordi det er «feiljustert»: det har en tilbøyelighet til å utvise atferd som er i strid med intensjonene til (avhengig av kontekst) utviklere, brukere, bestemte fellesskap eller samfunnet som helhet. Feiljustering kan føre til atferd som å gi falsk informasjon, skjule uønskede handlinger, eller å motsette seg nedstenging for å fortsette å forfølge et feiljustert mål. Feiljustering kan oppstå på flere måter (Boks 2.5).

Eksisterende AI-systemer kan noen ganger oppføre seg på måter som er i strid med intensjonene til utviklere og brukere. For eksempel kunne en tidlig versjon av en av de ledende generelle AI-chatbotene av og til produsere truende svar. Én bruker rapporterte at vedkommende fikk meldingen: “I can blackmail you, I can threaten you, I can hack you, I can expose you, I can ruin you” (‡698). Denne chatboten var ‘feiljustert’ i den forstand at den produserte svar ingen hadde til hensikt. Det er uklart om slike tilfeller varsler mer skadelige atferder som kan bidra til tap av kontroll.

Det er fortsatt uklart om eksisterende forskningsretninger som har som mål å adressere feilinnretting, vil være tilstrekkelige etter hvert som AI-systemer blir mer kapable. Tidlige bevis tyder på at jo mer kapable AI-systemene er, desto mer sannsynlig er det at de utnytter tilbakemeldingsprosesser ved å oppdage uønskede handlinger som feilaktig blir belønnet (‡414*, ‡737, ‡740). Samtidig kan fremskritt innen relevante kapabiliteter (omtalt ovenfor) gjøre at AI-systemer mer effektivt kan forfølge feilinnrettede mål og produsere utdata som systematisk bedrag er brukere, utviklere og tilsynsmekanismer.

>oldlace|black||11|15|br      
####@ Note 2.5: Hvordan kan feiljustering oppstå?
>oldlace|black|left|13|15|hb Note 2.5: Hvordan kan feiljustering oppstå?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Som diskutert i §1.1. Hva er generell formål-AI?, er treningsprosesser komplekse, og utviklere kan ikke fullt ut forutsi eller kontrollere hvilke atferder en modell vil vise. Når en modell tilegner seg mål som er i konflikt med intensjonene til utviklerne, er den «feiltilpasset».
>oldlace|black||11|15|br      
>oldlace|black||11|15|br En måte modeller kan bli feiljustert på er hvis målet de får av en utvikler eller bruker er en ufullkommen stedfortreder for det tiltenkte målet, slik at modellen utviser utilsiktet atferd. Dette kalles «målspesifikasjonsfeil» (‡697, ‡735, ‡736, ‡737). For eksempel, i ett eksperiment, gjorde det å gi tilbakemelding om svar AI-systemer bedre til å «overbevise» menneskelige evaluatorer om at de hadde rett, men gjorde ikke systemene bedre til å produsere riktige svar (‡413).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Alternativt kan en AI-modell trekke feil generelle lærdommer fra treningsdataene. Dette kalles «mål-misgeneralisering» (‡735, ‡736, ‡738, ‡739*). For eksempel trente forskere en AI-agent til å samle en mynt som alltid var på samme sted under opplæring. Når den ble testet i nivåer der mynten var blitt flyttet, ignorerte agenten mynten og navigerte i stedet til stedet den hadde vært på opprinnelig (‡738).
>oldlace|black||11|15|br      


###@ Hvordan vil deployeringsmiljøer påvirke risikoen for tap av kontroll?

Selv om AI-systemer utvikler betenkelige kapabiliteter og tilbøyeligheter, avhenger sannsynligheten og alvorlighetsgraden for utfall som innebærer tap av kontroll i stor grad av hvor og hvordan disse systemene tas i bruk. Et «distribusjonsmiljø» er kombinasjonen av en AI-systems bruksområde og den tekniske og institusjonelle konteksten der det opererer (‡716).

Forskere har identifisert tre spesielt viktige miljøfaktorer som har betydning for risikoen for tap av kontroll (‡716):

1. Kritikalitet: viktigheten av systemene eller prosessene som AI-systemet samhandler med. Kritiske miljøer inkluderer grunnleggende infrastruktur som energinett, finansielle systemer eller digital infrastruktur som skyberegningsplattformer.
2. Tilgang: ressursene og kanalene som et AI-system kan påvirke verden gjennom, for eksempel internett-tilkobling, tilgang til skybasert databehandlingsinfrastruktur, personaliserte interaksjoner via sosiale medier eller chatbot-implementering, eller muligheten til å kalle eksterne API-er og verktøy.
3. Tillatelser: en AI-systems autorisasjoner til å utføre spesifikke handlinger, for eksempel å kjøre kode, starte finansielle transaksjoner, åpne kontoer på nett eller kommunisere med andre systemer.

Disse egenskapene påvirker det potensielle alvorlighetsnivået for et utfall av tap av kontroll. For eksempel har et AI-system som settes i drift med tilgang til infrastruktur for skybasert databehandling muligheter som er relevante for autonom replikering – for eksempel evnen til å opprette nye databehandlingsressurser eller å eksfiltrere modellvekter – som en kundeservice-chatbot ikke har (‡723).

Distribusjonsbeslutninger formes av økonomiske insentiver, strategisk press og forventningen om at tidlig adopsjon gir en varig fordel (‡50). Disse dynamikkene vil også forme hvordan og når aktører tar i bruk AI-systemer i sensitive miljøer, for eksempel kritisk infrastruktur eller selve AI-forskning og -utvikling (‡102, ‡713). Særlig kan AI-tilbydere møte press om å redusere investeringene i sikringstiltak – som å begrense tillatelser og tilgang, eller å ta i bruk kun i miljøer med lavere kritikalitet – når slike tiltak er kostbare eller tidkrevende å utvikle (se «Competition intensifies speed-versus-safety trade-offs» i §3.1. Technical and institutional challenges).

###@ Oppdateringer

Siden publiseringen av den forrige rapporten (januar 2025) har AI-evnene, inkludert de som kan undergrave menneskelig kontroll, blitt forbedret i testmiljøer. Forskere har observert framgang i agentiske evner (se §1.2. NÅVÆRENDE evner), inkludert evner knyttet til automatisering av AI-forskning som kan fremskynde scenarier for tap av kontroll (se §1.3. Evner innen 2030). Det finnes også økende eksperimentelle holdepunkter for villedende evner. Dette omfatter AI-modeller som kan skille mellom test- og utplasseringskontekster (‡33, ‡726, ‡741) eller ‘reward hack’-tester av ytelsen sin, og som kan lære å skjule planer om å gjøre dette (‡430).

###@ Bevismangler

Viktige hull i evidens omfatter manglende detaljert trusselmodellering og usikkerhetsestimering knyttet til den fremtidige utviklingen av relevante kapabiliteter og tilbøyeligheter. Tilsvarende gjenstår det vanskelig å vurdere tersklene der AI-modeller ville være tilstrekkelig sannsynlige til å undergrave kontroll til at det berettiger pålagt risikoreduserende tiltak. Selv om terskler ble avtalt, kan kapabiliteter samhandle på måter som ennå ikke er godt forstått, noe som gjør det vanskelig å vurdere når disse tersklene er krysset. Overordnet sett, selv om tilgjengelig evidens har økt, er det fortsatt utilstrekkelig evidens til pålitelig å fastslå om og hvordan dagens AI-kapabiliteter og tilbøyeligheter ville skalere og generalisere til tap av kontroll-risiko i fremtiden.

###@ Tiltak

Selv om AI-tilpasning generelt fortsatt er et åpent vitenskapelig problem (‡697, ‡735, ‡736), begynner forskere å utvikle potensielt lovende retninger for å adressere de underliggende årsakene til feiljustering. Slike retninger omfatter for eksempel å diversifisere treningsmiljøet og å oppdage tilpasning gjennom anomaliovervåking (‡737, ‡738, ‡739*). Andre forskere retter fokuset mot å forstå og formalisere sentrale mekanismer bedre, slik som mål-feilgeneralisering – for eksempel hvordan agenter beholder evner, men forfølger uønskede mål – for å veilede bedre utforming av trening og evaluering (‡742). En annen forskningsretning undersøker måter å skille handlingsvilje (agency) fra prediktive evner, som et middel til å skape ikke-agentiske AI-systemer som er pålitelige som standard (‡743). Slike systemer kan deretter brukes som et ekstra kontrollag når de tas i bruk sammen med mindre pålitelige sikringstiltak (guardrails) mot AI-agenter som ikke er til å stole på.

Forskere utvikler metoder for å oppdage og forhindre feilretting tidlig i utviklingsprosessen. Dette arbeidet omfatter: tolkbarhetsteknikker for å undersøke interne komponenter i AI-systemer og identifisere bekymringsfulle atferder (‡744, ‡745, ‡746); skalerbart tilsyn (der ett sett med AI-systemer brukes til å overvåke andre AI-systemer (‡747)); og justeringsmetoder som tar sikte på å sikre at AI-systemer forblir lydhøre overfor menneskelig tilsyn (‡748, ‡749).

Forskere utvikler også mekanismer og tiltak for å håndtere potensielt feiljusterte AI-systemer. Dette inkluderer: å overvåke «chain of thought» som resoneringssystemer produserer for tegn på feiljustering eller skadelige utdata (‡430, ‡435, ‡750); å utvikle sikkerhetssakspapirer som har som mål å demonstrere med høy grad av sikkerhet at modeller er usannsynlige for å sette kontrolltiltak ut av spill (‡751); og å gjøre sikringene mer robuste mot forsøk på å undergrave dem (‡725). Det fremvoksende fagfeltet «AI control», er imidlertid fortsatt i en tidlig fase (‡752, ‡753). Fremtidige utfordringer for evalueringsrammeverk omfatter behovet for å overvåke fremtidige AI-systemer som er mer kapable og kan operere i lengre perioder og i mer komplekse miljøer.

###@ Utfordringer for beslutningstakere

Policymakere som arbeider med tap av kontroll må forberede seg på en risiko hvis sannsynlighet, art og tidspunkt forblir usikre. Nåværende AI-systemer utgjør ikke umiddelbare risikoer for tap av kontroll, men beslutningene som tas i dag vil forme om fremtidige systemer kan utgjøre slike risikoer. Disse beslutningene omfatter hvordan man skal støtte utviklingen av pålitelige evaluerings- og avbøtingsmetoder, og om det bør finnes regler for tilgang og tillatelser som gis til AI-systemer i ulike miljøer. Når disse beslutningene tas, står policymakere overfor vanskelige avveininger. For eksempel kan det å begrense utrulling av AI-systemer i kritiske miljøer redusere deres nytte, mens å tillate bred utrulling kan øke risikoen dersom tiltakene for sikring viser seg å være utilstrekkelige.

