###@ Hva er generell-purpose AI-systemer?

Generelle AI-systemer er programvare som lærer mønstre fra store mengder data, slik at de kan utføre en rekke oppgaver i stedet for å være spesialisert for én bestemt funksjon eller et domene (se Bord 1.1). For å skape slike systemer gjennomfører AI-utviklere en flerstegsprosess som krever betydelige beregningsressurser, store datasett og spesialisert kompetanse (se Bord 1.2). Beregningsressurser (ofte forkortet til «compute») er nødvendig både for å utvikle og for å distribuere AI-systemer, og inkluderer spesialiserte databrikker samt programvare og infrastruktur som trengs for å kjøre dem.† Siden de trenes på store, varierte datasett, kan generelle AI-systemer utføre mange ulike oppgaver, for eksempel å oppsummere tekst, generere bilder eller skrive datakode. Dette avsnittet forklarer hvordan generelle AI-systemer lages, hva «resonnerende» modeller er, og hvordan policy-beslutninger påvirker utviklingen av generelle AI-systemer.

    Note † -- Begrepet ‘compute’ kan også referere til enten en måling av antall beregninger en prosessor kan utføre (typisk målt i flyttallsoperasjoner per sekund) eller spesifikt maskinvaren (slik som grafikkbehandlingsenheter) som utfører disse beregningene.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Språksystemer
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
###@ bildegeneratorer
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
- Ser ut til å være 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotikk og navigasjonssystemer
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Prediktorer for ulike klasser av biomolekylære strukturer
- AlphaFold 3 (‡27)
- Forsterk (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ AI-agenter
- AlphaEvolve (‡31*)
- ChatGPT Agent (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- AI Scientist-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 1.1: Generelle typer for kunstig intelligens
>white|black||9|11|br Det finnes flere ulike typer generell formåls-AI. I denne rapporten regnes modeller som kan predikere strukturell informasjon for ulike klasser av molekyler, som «generell formåls-AI», fordi de kan tilpasses til et mangfold av oppgaver. For eksempel er modeller trent for å predikere proteinsstruktur anvendelige for en rekke andre oppgaver, som å predikere proteininteraksjoner, predikere bindingssteder for små molekyler, og å predikere og designe cykliske peptider (‡40).


>white|orangered|left|13|15|bb Dyp læring er grunnleggende for generell formåls-AI

Forskere bygger generelle AI-modeller ved hjelp av en prosess kalt «deep learning», som trener modeller til å lære av eksempler (‡41). I motsetning til programvareutvikling lærer deep learning-modeller å utføre oppgaver fra data i stedet for å være avhengige av håndskrevne instruksjoner. Ved å behandle store mengder data, som bilder, tekst eller lyd, oppdager disse modellene måter å representere dataene på, og skaper interne representasjoner av mønstre (som former, ordassosiasjoner eller lydstrukturer) som hjelper modellen med å gjenkjenne sammenhenger og generere utdata i tråd med treningsmålet. Deretter bruker de disse lærte interne representasjonene som abstrakte trekk til å analysere ny, liknende data og generere utdata i samme stil. For eksempel kan en generell- purpose AI-modell som er trent på tilstrekkelig mange eksempler av 19.-århundres romantisk engelsk poesi, gjenkjenne nye dikt i denne stilen og produsere nytt materiale i en tilsvarende stil.

På et mer detaljert nivå fungerer dyp læring ved å behandle data gjennom lag av sammenkoblede informasjonsbehandlingsnoder. Disse nodene kalles ofte «nevroner» fordi de er løst inspirert av nevroner i biologiske hjerner («nevrale nettverk») (Figur 1.1) (‡42). Når informasjon flyter fra ett lag med nevroner til det neste, omdanner modellen gradvis dataene til mer abstrakte representasjoner som grupper av lærte egenskaper – mønstre som modellen har oppdaget automatisk i dataene, i stedet for håndkodede. For eksempel, i en modell for bildebehandling kan de første lagene lære å detektere enkle trekk som kanter eller grunnleggende former, mens dypere lag kombinerer disse trekkene for å finne mer komplekse mønstre som ansikter eller objekter.

Funksjonene på alle nivåer oppdages gjennom optimaliseringsprosessen som definerer treningsprosedyren. Under trening, når modellen gjør feil, justerer algoritmer for dyp læring styrken til ulike forbindelser mellom nevroner for å forbedre modellens ytelse. Styrken til hver forbindelse mellom noder kalles ofte en «vekt». Denne lagdelte tilnærmingen gir dyp læring navnet sitt.

Dyp læring har vist seg å være svært effektivt for å la AI-systemer utføre oppgaver som tidligere ble ansett som vanskelige for tradisjonelle håndprogrammerte beregningssystemer og andre tidligere symbolske eller regelbaserte AI-metoder. De fleste av dagens toppmoderne generelle AI-modeller er nå basert på en bestemt nevralt nettverksarkitektur kjent som «transformer» (‡43, ‡44). Transformere bruker en «oppmerksomhets»-mekanisme (‡45) som hjelper modellen å fokusere på de mest relevante delene av inndataene når den behandler informasjon, for eksempel ved å avgjøre hvilke ord i en setning som er viktigst for å forstå betydningen. Denne måten å bygge modeller på har ført til betydelige forbedringer i oversettelse (‡43), behandling av naturlig språk (‡46), bildegjenkjenning (‡47) og talegjenkjenning (‡48, ‡49), og har i siste instans ført til utviklingen av dagens mest avanserte modeller.

![fig1.1](images/fig1.1_neural_network.png)

##### Figur 1.1: En illustrerende framstilling av en «nevralt nettverk»
>white|black||9|11|br Dagens generelle AI-modeller er basert på disse nettverkene, som løselig er inspirert av biologiske hjerner. Ulike nettverk har ulike størrelser og arkitekturer. Imidlertid er alle sammensatt av sammenkoblede informasjonsbehandlingsenheter kalt «neuroner», der styrkene i forbindelsene mellom nevronene kalles «weights» (vekter). Vekter oppdateres gjennom trening med store mengder data. Kilde: International AI Safety Report 2025 (‡50) (modifisert).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Figur 1.2: En skjematisk framstilling av stadiene i utvikling av generell formål-AI
>white|black|left|9|11|br Internasjonal AI-sikkerhetsrapport 2026.


>white|orangered|left|13|15|bb Generell-purpose AI utvikles i etapper

Å utvikle et generelt anvendelig AI-system innebærer flere trinn, fra innledende modelltrening til overvåking etter utrulling og oppdateringer (Figur 1.2). I praksis overlapper disse stegene ofte hverandre på en iterativ måte. Hvert trinn krever ulike ressursbidrag (f.eks. data, arbeidskraft, beregning) og ulike teknikker, og de gjennomføres noen ganger av ulike utviklere (Figur 1.2 og Bord 1.2).

For eksempel krever modellforhåndstrening generelt store mengder beregning og data, noe som gjør dette stadiet særlig sårbart for retningslinjer som påvirker tilgang til beregningsressurser eller treningsdata (‡51, ‡52). På samme måte innebærer datasanering og noen metoder for finjustering av modeller for tiden store mengder menneskelig arbeidskraft for innledende datamerking (‡53). Dette stadiet er derfor sårbart for endringer i arbeidskostnader, plattformretningslinjer eller regler som påvirker kontraktsinngåelse på tvers av landegrenser.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Datainnsamling og kuratering
> 
  Før utvikling av en generell AI-modell samler utviklere og databehandlere inn, rengjør, kuraterer og standardiserer rå treningsdata til et format modellen kan lære fra. Dette kan være en arbeidskrevende prosess. Treningsdatasettene bak banebrytende modeller består av et enormt antall eksempler fra hele internett.
  Team utvikler ofte avanserte filtreringsmetoder for å redusere skadelig innhold, eliminere dupliserte data og forbedre representasjonen på tvers av ulike temaer og kilder (‡54, ‡55). Datasanering kan også bidra til å redusere brudd på opphavsrett og personvern, fjerne eksempler som inneholder farlig kunnskap, håndtere flere språk og forbedre dokumentasjonen for dataproveniens (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Fortrening (første fase av opplæringen)

  Under forhåndstrening mater utviklere modeller enorme mengder variert data for å gi et bredt grunnlag av informasjon og kontekstuell forståelse. Denne prosessen danner en ‘grunnmodell’. Dette er en svært datar- og beregningsintensiv prosess.

  Under fortrening blir modeller eksponert for milliarder eller billioner av eksempler på innhold, for eksempel bilder, tekster eller lyd. Gjennom denne eksponeringen oppdager modellen gradvis abstrakte egenskaper som kan representere data, og lærer om hvordan disse egenskapene henger sammen. Dette gjør at den kan gi mening til nye innganger i en kontekst. Denne fortreningsprosessen tar uker eller måneder (‡59) og bruker titalls eller hundretalls tusen grafikkbehandlingsenheter (GPUs) eller tensorbehandlingsenheter (TPUs) (‡60) – spesialiserte databrikker som er utviklet for raskt å utføre mange slike beregninger. Noen utviklere gjennomfører fortrening med egen beregningskapasitet, mens andre bruker ressurser levert av spesialiserte leverandører av beregningskapasitet.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Ettertrening og finjustering (andre treningsfase)

  «Ettertrening» foredler videre grunnmodellen for å optimalisere den for en bestemt anvendelse. Det er en prosess som er moderat beregningsintensiv og svært arbeidsintensiv. Et skifte mot å bruke «syntetiske data» – kunstig generert informasjon som etterligner data fra den virkelige verden, men som skapes ved hjelp av algoritmer eller simuleringer – bidrar til å gjøre denne fasen mindre arbeidsintensiv.
  Etter-trening inkluderer ulike finjusteringsteknikker og andre modifikasjoner. «Veiledet finjustering» innebærer videre trening av en trent modell på spesifikke datasett for å forbedre modellens ytelse innen det domenet (‡61, ‡62). For eksempel kan en generell modell trenes videre på en stor samling av radiologiske bilder. «Forsterkende læring» (RL) innebærer å forbedre modellens ytelse ved å «belønne» en modell (gi positiv tilbakemelding) for ønskede utdata og «straffe» en modell (gi negativ tilbakemelding) for uønskede utdata. Den har to fremtredende underkategorier. «Forsterkende læring fra menneskelig tilbakemelding» innebærer å belønne utdata som samsvarer med menneskelige preferanser og straffe dem som ikke gjør det, basert på menneskelig tilbakemelding (‡63, ‡64*). «Forsterkende læring med verifiserbare belønninger» (RLVR) brukes for å forbedre modellens ytelse på oppgaver som krever faktamessig korrekthet, slik som matte- eller kodegenerering. Utviklere veksler vanligvis mellom å anvende etter-treningsteknikker og å kjøre tester til resultatene viser at modellen oppfyller ønskede spesifikasjoner.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Systemintegrasjon

  Utviklere kombinerer én eller flere generelle AI-modeller med andre komponenter for å lage et «AI-system» som er klart til bruk. GPT-5 (for eksempel) er en generell AI-modell som behandler tekst, bilder og lyd, mens ChatGPT er et generelt AI-system som kombinerer flere modeller i ulike størrelser og med ulike kapabiliteter med en chatteflate, innholdsbehandling, Web-tilgang og integrasjon i applikasjoner for å skape et funksjonelt produkt.
  I tillegg til å gjøre AI-modeller operative, tar de ekstra komponentene i et AI-system også sikte på å forbedre kapasitet, nytte og sikkerhet. For eksempel kan et system leveres med et filter som oppdager og blokkerer modellinnganger eller -utganger som inneholder skadelig innhold (‡65*). Utviklere bruker også i økende grad «scaffolding» – ekstra programvare bygget rundt generelle AI-modeller som gjør det mulig å planlegge fremover, forfølge mål og samhandle med verden (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Distribusjon og utgivelse
  Distribusjon er prosessen med å gjøre det integrerte AI-systemet tilgjengelig for den tiltenkte bruken. Utviklere og distributører implementerer AI-systemer i virkelige applikasjoner, produkter eller tjenester. Utviklere kan distribuere AI-systemer internt (for egen bruk) eller eksternt (for private kunder eller offentlig bruk). Når AI-systemer distribueres eksternt, gir ofte selskaper brukere tilgang via nettbaserte brukergrensesnitt eller programmeringsgrensesnitt (APIs) som lar brukere få tilgang til og kjøre systemet. For eksempel kan ett selskap utforme en skreddersydd chatbot for kundeservice som drives av et annet selskaps generelle AI-system.
  ‘Distribusjon av AI-system’ refererer til å gjøre en modell tilgjengelig for bruk i den virkelige verden med integrerte verktøy og grensesnitt, mens ‘modellutgivelse’ innebærer å gjøre grunnmodellen tilgjengelig for andre – enten som åpen vekt (nedlastbare parametere) eller som lukket vekt (kun tilgang via API). Se §3.4. Modeller med åpen vekt.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Overvåking etter utrulling og oppdateringer

  Utviklere samler ofte inn og analyserer tilbakemeldinger fra brukere, følger med på påvirkning og ytelsesmålinger, og gjør iterative forbedringer for å løse problemer som oppdages under reell bruk (‡67). Forbedringene gjøres ved å oppdatere systemintegrasjoner, ofte via kontinuerlig finjustering og ved å gi modeller tilgang til eksterne databaser med (nylige) fakta. Dette holder store AI-modeller oppdaterte uten å gjenta hele forhåndstreningsprosessen (‡68*). Dette gjør det mulig for evner å bygge seg opp på tvers av påfølgende treningsrunder samtidig som stabilitet opprettholdes, og samtidig redusere beregningskostnader.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 1.2: Utviklingssteg for generell-purpose AI
>white|black||9|11|br Ved hvert generelt utviklingsstadium for kunstig intelligens blir AI-modellen forbedret for videre bruk, og til slutt distribuert som et fullt integrert AI-system, overvåket og oppdatert.


>white|orangered|left|13|15|bb Resonneringssystemer genererer «kjeder av tanke» under inferens for å forbedre ytelsen

Inferens skjer når noen bruker AI-modellen etter at den er trent. For eksempel skjer inferens når en person ber et AI-system om å planlegge en reise, og modellen bak dette trekker på relevante deler av det den har lært om geografi, transport og mat for å generere en reiserute.

I løpet av det siste tiåret har fremskritt i AI-kapasiteter i stor grad kommet fra større treningskjøringer; det vil si å øke mengden beregningskraft som brukes til å trene en AI-modell. Nylig har imidlertid forskere oppnådd flere gevinster ved å la modeller behandle informasjon i lengre tid, og ved å trene dem til å produsere eksplisitte resonnementstrinn mens de utfører en oppgave (‡69*, ‡70). AI-systemer som fungerer på denne måten kalles «resonneringssystemer», og de mellomliggende forklaringene de går gjennom når de løser et problem eller besvarer et spørsmål, kalles «chains of thought». Resonneringssystemer krever mer beregningsressurser ved brukstidspunktet for å generere disse avanserte resonnementskjedene (‡71, ‡72, ‡73, ‡74), og flere ressurser under trening slik at de lærer å resonnere bedre. I praksis gjør disse resonneringskapasitetene at AI-systemer kan løse mer komplekse problemer ved iterativt å dekomponere en oppgave i mindre trinn. Bord 1.3 viser et eksempel på et ikke-resonnerende system og et resonneringssystem som løser det samme problemet.

Resoneringssystemer har oppnådd store gjennombrudd i evner for krevende oppgaver. For eksempel, i 2025 løste resoneringssystemer som er spesialisert på matematisk problemløsning, som Googles Gemini Deep Think og en ikke-utgitt, eksperimentell modell fra OpenAI, problemer fra International Mathematical Olympiad (i et strukturert testsituasjon) på et nivå som tilsvarer menneskelig gullmedaljeprestasjon (‡75, ‡76). Resoneringssystemer har vist betydelig framgang i formelle domener som matematikk, logiske gåter og strukturerte vitenskapelige spørsmål, der steg-for-steg-resonnering kan verifiseres eksplisitt (‡77). Imidlertid kan resoneringssystemer også feile ved å produsere irrelevante, uproduktive eller repeterende tankerekker (‡78, ‡79).

###@ Oppdateringer om treningsmetoder

Siden publiseringen av forrige rapport (januar 2025) har en treningsmetode kalt «distillation» økt effektiviteten som enkelte modeller kan finjusteres med, betraktelig. Distillation innebærer å trene en «student»-modell på utdataene fra en mer kraftfull (og vanligvis større) «teacher»-modell, slik at studentmodellen direkte kan etterligne teacher-modellens utdata (‡80). For eksempel utviklet DeepSeek en stor modell kalt DeepSeek-R1, som utmerker seg i chain-of-thought resonnement. R1 produserte resonnement- utdata som deretter ble brukt til å finjustere mindre studentmodeller, inkludert DeepSeek-V3. DeepSeek-V3 viderefører mye av R1s matematiske-, kode- og dokument- analysekapabiliteter, og ble angivelig finjustert for omtrent $10,000 USD (selv om kostnadene for forhåndstrening ikke ble rapportert) (‡81). Dette er trolig en størrelsesorden lavere enn kostnaden for å finjustere tilsvarende kapable, større modeller.

![table1.3](images/table1.3_example_reasoning.png)

##### Bord 1.3: Et eksempel på et ikke-resonnerende system (venstre) versus et resonnerende system (høyre)
>white|black||9|11|br Å løse den samme gåten, er disse eksemplene tilpasset fra faktiske AI-svar. Resonneringssystemet bruker mer tid og beregningskraft på «tenkning» ved å konstruere en «chain of thought» før det gir sitt endelige svar.

![figure.3](images/fig1.3_AI_agent.png)

##### Figur 1.3: En illustrativ framstilling av en AI-agent
>white|black||9|11|br En AI-modell (senter) som er konfigurert til iterativt å planlegge, resonnere og bruke verktøy for å utføre oppgaver i den virkelige verden. Kilde: International AI Safety Report 2026.


Derfor kan destillasjon være en billig og effektiv måte for modeller å få mer kraftfulle egenskaper (‡82). Noen forskere har brukt destillasjon til å finjustere svært kapable modeller ved å bruke så få som 1,000 eksempler generert fra state-of- the-art-modeller (‡83). Siden destillasjon krever en eksisterende lærermodell, kan den ikke brukes direkte til å videreutvikle state-of-the-art-modellers egenskaper. Derimot kan den øke spredningen av avanserte AI-egenskaper, selv fra proprietære (closed-source) modeller (‡84*).

Sammen med teknologiske fremskritt innen «distribuert databehandling» og desentralisert trening (tilnærminger der utviklere bruker flere prosessorer, servere eller datasentre som arbeider sammen for å utføre AI-trening eller -inferens (‡85, ‡86, ‡87)), har graden i hvilken mange AI-utviklingsprosjekter er avhengige av stor-skala, sentralisert databehandlingsinfrastruktur blitt redusert. Dette gjør det i økende grad mulig for aktører med svakere tilgang til ressurser å utvikle og distribuere kraftige systemer.

###@ Oppdateringer om AI-agenter

Siden forrige rapport (January 2025), har fremskritt i hvordan utviklere kombinerer AI-modeller med verktøy gjort det mulig å utvikle stadig kraftigere AI-agenter. AI-agenter er utviklet for å forfølge mål, som ofte er spesifisert av brukere i naturlig språk. For å oppnå disse målene får de tilgang til verktøy, som minne, et datamaskin-grensesnitt og nettlesere. Disse verktøyene og koden som brukes til å kombinere dem med modellen omtales som ‘scaffolding’, og de hjelper AI-agenter med å samhandle autonomt med omverdenen, lage planer, huske viktige detaljer og forfølge mål (‡88*, ‡89) med betydelig mindre tilsyn eller bistand fra mennesker. For eksempel er Manus AI en populær AI-agent som kan automatisere ulike oppgaver, inkludert nettsøk, programvareutvikling og nettkjøp (‡90). Figur 1.3 viser et enkelt eksempel på en AI-agent sammensatt av en generell AI-modell ‘brain’ som kan planlegge, resonnere og bruke verktøy iterativt for minne, nettlesing og datamaskinbruk.

Digital infrastruktur for AI-agenter utvides (‡91), og de blir stadig mer vanlige på tvers av bransjer (‡92, ‡93, ‡94). AI-agenter har blitt utviklet for oppgaver som forskning (‡37), programvareingeniørarbeid (‡95), robotstyring (‡96) og kundeservice (‡97). Pågående forskning og utvikling har ført til jevnt mer kapable og mer autonome AI-agenter, eller fleragent-systemer. Forskere har anslått at kompleksiteten i programvarebenchmarks-oppgaver som AI-agenter kan utføre, omtrent dobles hver sjuende måned (se også §1.2. Nåværende kapabiliteter) (‡98). Eksperter hevder at stadig mer kapable AI-agenter vil skape både store muligheter og risikoer (‡99, ‡100*) (se §2.2.1. Pålitelighetsutfordringer).

###@ Bevismangler

De viktigste kunnskapshullene rundt utviklingsprosessen for generelle AI-systemer oppstår fra mangel på offentlig tilgjengelig informasjon om hvordan de utvikles. Noen utviklere er svært åpne om hvordan de utvikler generelle AI-systemer (‡1, ‡101). Likevel er det generelt en begrenset grad av offentlig og politikkutformende kunnskap om hvordan de fleste avanserte modeller utvikles, sikres, evalueres og tas i bruk. Dette gjelder særlig for internt distribuerte AI-systemer som brukes innen AI-selskaper, men ikke brukes eller forstås av eksterne interessenter (‡102, ‡103). Denne begrensede eksterne synligheten skaper utfordringer for åpenhet og tilsyn. Ulike forskere har pekt på begrenset og inkonsistent åpenhet knyttet til treningsdata (‡104, ‡105, ‡106), generelle AI-modeller (‡107, ‡108), AI-agenter (‡92), evalueringer (‡109), utviklingspipeliner (‡110) og sikkerhet (‡111). Begrensninger i ekstern offentliggjøring er noen ganger nødvendig for å beskytte selskapenes forretningshemmeligheter og immaterielle rettigheter. Samtidig gjør lav åpenhet det vanskeligere for uavhengige forskere og politikkutformere å studere generelle AI-modeller og -systemer.


