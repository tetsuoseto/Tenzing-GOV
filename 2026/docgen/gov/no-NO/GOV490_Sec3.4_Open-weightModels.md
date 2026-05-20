##########
>white|orangered|left|14|30|hr Seksjon 3.4
### 3.4. Modeller med åpen vekt
>white|orangered|left|24|30|hb Åpne vekt-modeller

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb Viktig informasjon
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Nivået på tilgang som AI-selskaper gir til «vektene» til modellene sine påvirker risikoen som disse modellene utgjør. Vekter er de matematiske parameterne som gjør det mulig for AI-modeller å behandle innganger og generere utganger. For enhver gitt modell kan selskaper velge å holde vektene helt private, gi enkelte brukere begrenset tilgang, eller tillate alle å laste dem ned i sin helhet. Modeller hvis vekter er offentlig tilgjengelige, kalles «open-weight-modeller».
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Åpne vektmodeller legger til rette for forskning og innovasjon, men deres sikkerhetstiltak kan lettere fjernes. Over hele verden kan ulike aktører – spesielt de med færre ressurser – bruke åpne vektmodeller til forsknings- og kommersielle formål. Imidlertid, sammenlignet med lukkede vektmodeller, er åpne vektmodeller lettere å modifisere for å vise potensielt skadelige atferder, og  s mer vanskelig.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Åpne vekt-modellutgivelser er irreversible. Når de først er publisert, kan ikke modellvektene tilbakekalles. Dette gjør det vanskeligere å redusere potensielle skader som kan oppstå som følge av utgivelsen av en modell med farlige evner.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Siden publiseringen av den forrige rapporten (januar 2025) har store utgivelser med åpen vekt redusert kapasitetsgapet med ledende lukkede modeller. Utviklere fra Kina, DeepSeek og Alibaba, lanserte henholdsvis sine R1- og Qwen-modeller, som oppnådde ytelse på nivå med ledende lukkede modeller. Samtidig lanserte OpenAI sine første åpne vekt-modeller siden 2019. Kapabilitetene til ledende lukkede modeller anslås nå å ligge mindre enn ett år foran ledende åpne vekt-modeller på fremtredende AI-benchmarker.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ En sentral policy-utfordring er å få tilgang til fordelene åpenvekt-modeller gir, samtidig som man håndterer deres særegne risikoer. En tilnærming er å vurdere åpenvekt-modeller i form av deres «marginale risiko»: i hvilken grad deres lansering kontrafaktisk øker samfunnsrisikoen utover den som allerede er skapt av eksisterende modeller eller andre teknologier. Dette er imidlertid komplekst i praksis. Små økninger i marginal risiko over tid kan også til sammen gi betydelige økninger i total risiko.
>oldlace|black||11|15|br      


Åpne vektmodeller, der parameterne er offentlig tilgjengelige for nedlasting, har tydelige implikasjoner for mange av utfordringene som er omtalt i de foregående avsnittene. En KI-modells «vekter» inneholder den avgjørende informasjonen som gjør at den kan generere nyttige svar for brukere. Når vektene først er utgitt, kan de ikke tilbakekalles: hvem som helst kan laste dem ned, studere dem, endre dem, dele dem og bruke dem på egne datamaskiner eller sky-kontoer. Når vekter er åpent tilgjengelige, kan andre enklere bygge videre på og modifisere modellen, dekke ulike behov og drive innovasjon (‡1317). Samtidig, gjennom samme mekanisme, kan brukere med ondsinnede hensikter også enklere fjerne sikkerhetstiltak og endre åpne vektmodeller for skadelige brukstilfeller (‡1122, ‡1160). Dette har reist spørsmålet om hvorvidt noen åpne vektmodeller bør holdes til særskilte krav (f.eks. mer strenge tester før utgivelse) eller, motsatt, gis særskilte unntak (f.eks. fra rapporteringskrav i regulering) (‡1033).

###@ Bakgrunn for open-weight-modeller

>white|orangered||14|15.5|bb Åpne vektmodeller kan være, men er ikke nødvendigvis, «åpen kildekode»-modeller

Selv om de ofte omtales som «open source», er de fleste offentlig utgitte modeller mer presist beskrevet som «open-weight». Dette er fordi, selv om utviklere leverer modellvektene, frigir de ikke den tilhørende treningskoden eller datasettene. Videre kjennetegnes open source-programvare vanligvis av tillatelige lisenser som stiller minimale krav til aktører nedstrøms som bruker eller endrer programvaren (‡1318). For eksempel har Metas Llama-modeller restriktive lisensbetingelser og inkluderer bare inferenskode, ikke treningskode, og blir derfor vanligvis ikke ansett som open source (‡1319, ‡1320). Alternativer for modellutgivelse finnes langs et spekter fra fullstendig lukket til fullstendig open source, med ulike avveininger mellom risiko og nytte i hvert punkt (‡1086*, ‡1320, ‡1321). Bord 3.9 beskriver disse alternativene.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Helt lukket
  Brukere kan ikke samhandle direkte med modellen i det hele tatt
  Eksempler: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Vertikalt tilgang
  Brukere kan bare samhandle via en bestemt applikasjon eller et bestemt grensesnitt, for eksempel en mobil chatbot-applikasjon
  Eksempler: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb API-tilgang til modell
  Brukere kan sende forespørsler til modellen via kode, slik at den kan brukes i eksterne applikasjoner
  Eksempler: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb API-tilgang til finjustering
  Brukere kan finjustere modellen for sine spesifikke behov
  Eksempler: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Åpen vekt: vekter tilgjengelig for nedlasting
  Brukere kan laste ned og kjøre modellen på sine egne datamaskiner
  Eksempler: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Vekter, data og kode tilgjengelig for nedlasting med bruksrestriksjoner
  Brukere kan laste ned og kjøre modellen samt inferens- og opplæringskoden, men det finnes visse lisensbegrensninger for bruken av den
  Eksempler: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Fullt åpen: vekter, data og kode tilgjengelig for nedlasting uten bruksbegrensninger
  Brukere har full frihet til å laste ned, bruke og endre modellen, full kode og data
  Eksempler: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 3.9: Delingsalternativer for modeller, fra helt lukket til helt åpen
>white|black||9|11|br Et illustrerende utvalg av alternativer for deling av modeller, fra fullstendig lukkede modeller (modellene er private og holdes kun for proprietær bruk) til fullstendig åpne og åpenkilde-modeller (modellvekter, data og kode er fritt og offentlig tilgjengelig uten restriksjoner på bruk, modifisering og deling). Modeller som faller i de første fire kategoriene omtales ofte som «lukkede». Denne delen fokuserer på de tre nederste radene. Kilde: tilpasset fra Bommasani, 2024 (‡1317).


###@ Fordeler og risikoer

>white|orangered|left|14|15.5|bb Åpne vektormodeller kan enklere tilpasses og evalueres

Åpen-vektsmodeller tilbyr betydelige fordeler for forskning, innovasjon og tilgang. Som diskutert i §1.1. Hva er generell- formåls AI?, det å trene generell- formåls AI-modeller er svært kostbart - ledende modeller koster hundrevis av millioner dollar å utvikle. Ved å slippe modellvekter åpent kan aktører med mindre ressurser replikere, studere og bygge videre på eksisterende systemer. Uten slik tilgang risikerer fellesskap i regioner med lave ressurser å bli holdt utenfor fra fordelene med AI, noe som gjør åpne vekter avgjørende for å muliggjøre bred deltakelse fra den globale majoriteten i AI-utvikling (‡1322). Videreutviklere kan finjustere modeller for ulike anvendelser; for eksempel å tilpasse dem for underressursede minoritetsspråk eller optimalisere ytelsen for bestemte oppgaver, som juridisk utforming eller innskriving av medisinske notater (‡1323, ‡1324*). På denne måten kan åpen-vektsmodeller gjøre det mulig for flere mennesker og fellesskap å bruke og ha nytte av AI enn det som ellers ville vært mulig (‡1325). For modeller som ikke er i stand til å være tilstrekkelig farlige, kan disse fordelene oppveie den økte risikoen ved å slippe vekter åpent, selv om dette avhenger av risikotoleransen til relevante beslutningstakere.

Åpne vektutgivelser utvider også gruppen av utviklere og forskere som kan studere modellen, evaluere dens egenskaper, teste for sårbarheter og iterere på forbedringer (‡1326, ‡1327). Dette gjør det mer sannsynlig at nyttige anvendelser og skadelige feil blir identifisert, selv om dette ikke er garantert (‡1328, ‡1329). Brukere kan også kjøre open-weight-modeller på egne enheter, slik at de kan opprettholde kontroll over sensitiv data og unngå å sende den til tredjepartsservere.

Det finnes flere fordeler når utviklere deler informasjon som treningsdata, kode, evalueringsverktøy og dokumentasjon samt modellvekter (‡1320, ‡1330, ‡1331, ‡1332*). Med mer informasjon kan nedstrømsutviklere og andre forskere bedre forstå open-weight-modeller og tilpasse dem til nye bruksområder.

>white|orangered|left|14|15.5|bb Sikkerhetstiltakene i modeller med åpne vekter er enklere å fjerne, noe som muliggjør potensiell ondsinnet bruk

Åpne vektmodeller medfører også ekstra risikoer fordi sikkerhetstiltakene deres er lettere å fjerne. Selv om både åpne vektmodeller og lukkede modeller kan ha sikkerhetstiltak for å avslå skadelige brukerspørsmål, er disse tiltakene mye lettere å fjerne for åpne vektmodeller. Ondsinnede aktører kan finjustere en modell for å optimalisere ytelsen for skadelige bruksområder, fjerne deler av koden som er utformet for å hindre skadelig bruk, eller angre tidligere sikkerhetsfinjustering (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Som et resultat kan åpne modellvekter forsterke misbruksrisikoene som er omtalt i §2.1. Risikoer ved ondsinnet bruk ved å tillate at flere aktører kan dra nytte av og bygge videre på eksisterende kapabiliteter for ondsinnede formål uten tilsyn (‡1122, ‡1315). Selv om mange brukere ikke vil ha ferdigheten eller insentivet til å fjerne sikkerhetstiltak på åpne vektmodeller, er svært motiverte ondsinnede aktører en bekymring. I tillegg kan ondsinnede aktører også være i stand til å bruke åpne vektmodeller til å identifisere sårbarheter i lignende lukkede modeller (‡1055*). Slike feil er vanskeligere å oppdage ved å bare kjøre lukkede modeller, på grunn av den større kontrollen og overvåkingen som tilbydere av lukkede modeller kan implementere.

>white|orangered|left|14|15.5|bb Å dele modellvekter er irreversibelt

Når modellvekter er tilgjengelige for offentlig nedlasting, finnes det ingen måte å gjennomføre en fullstendig tilbakestilling av alle eksisterende kopier. Internett-vertsplattformer som GitHub og Hugging Face kan fjerne modeller fra sine plattformer, noe som gjør det vanskelig for noen aktører å finne nedlastbare kopier, og som skaper en betydelig terskel for mange tilfeldige ondsinnede brukere (‡1339). Motiverte aktører kan imidlertid fortsatt skaffe seg kopier dersom modellen er lastet ned og rehostet andre steder, eller lagret lokalt. Videre arver etterfølgende utviklere som integrerer åpen-vekt-modeller i sine systemer også eventuelle svakheter, som sårbarheter for målrettede (adversarial) angrep (‡1055) eller modellkapasiteter til å omgå overvåkingssystemer (se §2.2.2. Tap av kontroll) (‡1315). I motsetning til lukkede modeller der verter kan rulle ut rettelser universelt, kan utviklere av åpen-vekt-modeller ikke garantere at oppdateringer blir tatt i bruk av brukere.

###@ Oppdateringer

Siden publiseringen av forrige rapport (januar 2025) har kapabilitetsgapet mellom ledende åpne vekt-modeller og lukkede modeller blitt mindre. Kinesiske utviklere har blitt spesielt viktige leverandører av åpne vekt-modeller. I januar 2025 ga DeepSeek ut sin R1-modell, som oppnådde resultater på nivå med OpenAIs o1 på en rekke beregningsbenchmarker (‡1340). Alibabas Qwen-modeller har også fått økt gjennomslag og inntar per august 2025 førsteplassen for en åpen vekt-modell i Chatbot Arena, et mye brukt ytelsesbenchmark (‡1341, ‡1342*). I august 2025 ga OpenAI ut sine første åpne vekt-modeller siden utgivelsen av GPT-2 i 2019, gpt-oss-120b og gpt-oss-20b. Meta har fortsatt å gi ut Llama-modeller med åpne vekter. Kapabilitetene til de ledende lukkede modellene anslås nå å ligge mindre enn ett år foran de ledende åpne modellene på sentrale AI-benchmarker (Figur 3.10).

###@ Bevismangler

Et sentralt kunnskapshull gjelder den reelle effekten i verden for tekniske løsninger som skal hindre misbruk av åpen-vekts-modeller. Forskere har foreslått ulike tilnærminger for å gjøre modeller manipulasjonssikre. Dette omfatter nye treningsteknikker som er utformet for å gjøre modeller motstandsdyktige mot skadelig endring (‡1276), filtrering av skadelig innhold fra treningsdata (‡55), og forsvar mot jailbreaks (‡675, ‡676). Disse teknikkene tas nå i bruk i utgivelser i den virkelige verden fra store utviklere. For eksempel tok OpenAI i bruk noen av disse teknikkene i gpt-oss-modellene sine, og rapporterte at adversarialt finjusterte versjoner ikke nådde høye kapabilitetsterskler (‡1344*). Imidlertid har forskning vist at ondsinnede aktører kan deaktivere sikkerhetsmekanismer ved å trene modeller på skadelige eksempler (‡1345, ‡1346). Videre er det fortsatt vanskelig å evaluere robustheten til sikkerhetsmekanismer pålitelig, noe som gjør deres effektivitet mot angrep i den virkelige verden usikker (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Figur 3.10: Kapasitetsgap mellom de ledende åpenvekt- og lukkede AI-modellene
>white|black||9|11|br Epoch Capabilities Index (ECI)-score for topppresterende open-weight (mørkeblå) og closed (lyseblå) modeller over tid. ECI kombinerer score fra 39 benchmarktester til en enkelt generell kapabilitetsskala. De beste open-weight-modellene ligger omtrent ett år etter closed-modellene. Kilde: Epoch AI, 2025 (‡1343).


###@ Tiltak

Tekniske tiltak for risiko knyttet til åpen-vektsmodeller fungerer gjennom hele AI-utviklings- og distribusjonsprosessen (‡1141, ‡1195, ‡1347). For eksempel, når modeller utvikles, kan utviklere og nedstrømsadaptere filtrere sensitivt innhold fra treningsdata for å minimere skadelige egenskaper. Å fjerne skadelige eksempler fra en models treningsdata kan forhindre adversarial fine-tuning 10 ganger mer effektivt enn forsvar som legges til etter opplæring, selv om det også kan påvirke nyttige egenskaper (‡55). Leverandører av AI-applikasjoner kan også implementere mekanismer for hendelsesrapportering og -respons (‡1348).

I tillegg kan vertsplattformer som HuggingFace og GitHub fastsette plattformens vilkår for bruk for å fjerne modeller som er endret for skadelige formål (‡1141, ‡1324). Modellutviklere kan gi full tilgang til revisorer før lansering, eller velge en «trinnvis» lanseringsstrategi – å lansere modeller til gradvis større grupper (‡1086). Dette kan bidra til å identifisere potensielle feilfunksjoner eller sårbarheter før en modell blir tilgjengelig i stor skala (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Note 3.1: Sikring av modellvekter
>oldlace|black|left|13|15|hb  Note 3.1: Sikring av modellvekter
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Risikoene som diskuteres i denne delen antar at modellvekter slippes bevisst. Lukkede modellvekter kan imidlertid også bli tilgjengelige gjennom tyveri eller lekkasje. Lukkede modeller koster hundrevis av millioner dollar å utvikle (§1.1. What is general-purpose AI?) og er i gjennomsnitt mer kapable enn open-weight-modeller (‡1343). Dette gjør dem til attraktive mål for aktører som spenner fra hobbyhackere til statlige aktører som søker å skaffe seg ledende AI-modeller.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Stjålne lukkede modellvekter ville medføre risikoer som ligner dem som er beskrevet ovenfor for åpne modellvekter, men potensielt uten noen av avbøtende tiltakene. Ondsinnede aktører kunne fjerne sikkerhetstiltak fra de mest kapable modellene. I motsetning til legitime utviklere, ville slike aktører ikke være underlagt omdømmemessige, juridiske eller kommersielle begrensninger som i dag insentiverer toppselskaper innen kunstig intelligens til å distribuere modellene sine på en trygg måte.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Gjeldende sikkerhetsnivåer varierer i bransjen, og kan være utilstrekkelige mot sofistikerte angripere. Noen utviklere forplikter seg til å sikre modellvekter mot kriminelle nettverk og interne trusler (‡582), mens andre ikke har gjort noen offentlige sikkerhetsforpliktelser (‡1109, ‡1349). Forskning indikerer at AI-databaser kan være ute av stand til å motstå angrep fra de mest sofistikerte og best ressurssterke aktørene (‡582, ‡1350, ‡1351). Per desember 2025 finnes det ingen bekreftede, offentlig dokumenterte tilfeller av tyveri av modellvekter. Imidlertid er det rapportert om andre sikkerhetsbrudd hos ledende AI-selskaper, inkludert en inntrenging i Microsofts e-postsystemer (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Å lukke disse sikkerhetshullene vil kreve betydelige investeringer i maskinvare, programvare, personell og fasilitetssikkerhet. Noen sikkerhetsforbedringer kan implementeres relativt raskt med koordinert innsats (‡1122). Andre kritiske tiltak, derimot, som å sikre maskinvareforsyningskjeder og fasiliteter, vil trolig ta år (‡1122). Private selskaper kan også mangle ressursene eller informasjonen som trengs for å utvikle tilstrekkelige beskyttelser alene. For eksempel har ikke AI-utviklere tilgang til gradert trusselintelligens som regjeringer har (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Utfordringer for beslutningstakere

En sentral utfordring for beslutningstakere er å sikre fordelene ved deling av open-weight-modeller uten å øke risikoen betydelig. For å unngå katastrofal skade bør utviklere av open-weight-modeller ikke utgi modeller uten å evaluere risiko, både ved hjelp av etablerte vurderingsmetoder som brukes for lukkede modeller, samt ved ytterligere testing, gitt at ondsinnede aktører kan finjustere modeller og fjerne sikkerhetsbeskyttelser. I praksis kan dette være vanskelig fordi kapabilitetsutvikling kan være uforutsigbar, open-weight-utgivelser er irreversible, og evalueringsinnsats er nødvendig for å forutsi når en utgivelse vil utgjøre betydelig potensiell skade. En tilnærming er å evaluere «marginal risiko» ved åpne utgivelser: i hvilken grad utgivelsen kontrafaktisk øker samfunnsrisiko utover den som allerede skapes av eksisterende modeller eller andre teknologier (‡556, ‡1033, ‡1354, ‡1355) (se §3.2. Risikostyringspraksis). Imidlertid er det komplekst og kontekstavhengig å anslå hvordan et system vil øke eller redusere risiko i etterkant når det først er tatt i bruk. Trinnvise økninger i risiko med påfølgende utgivelser kan kumulere over tid til betydelige økninger i total risiko, selv om den marginale risikoen knyttet til hver utgivelse fremstår som akseptabel (‡1356, ‡1357). AI-kapabiliteters dual-use-natur kompliserer også styring ytterligere: funksjoner som muliggjør gunstige anvendelser i medisin eller forskning kan omformateres for skade, og når vekter er offentlige, kan det være vanskelig å skille mellom legitime og ondsinnede bruksområder. Det er også uklart hvem som bør holdes ansvarlig når open-weight-modeller endres for skadelige formål.

