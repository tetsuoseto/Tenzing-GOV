##########
>white|orangered|left|14|30|hr Kapittel 3.3
### 3.3. Tekniske sikkerhetstiltak og overvåking
>white|orangered|left|24|30|hb Tekniske sikkerhetstiltak og overvåking

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb Viktig informasjon
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Et bredt spekter av tekniske sikkerhetstiltak brukes på ulike stadier i AI-utvikling og -bruk. Dette omfatter teknikker som anvendes under modellutvikling for å gjøre systemene mer robuste og motstandsdyktige mot misbruk (slik som datakurasjon), overvåking og kontroll ved utrulling (slik som innholdsfiltrering og menneskelig tilsyn), samt verktøy etter utrulling for å overvåke det bredere AI-økosystemet (slik som proveniens og innholdsdeteksjon).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Tekniske sikkerhetstiltak har begrensninger og forhindrer ikke pålitelig skadelig atferd i alle sammenhenger. For eksempel kan brukere noen ganger få skadelige resultater ved å omformulere forespørsler eller dele dem opp i mindre trinn. Tilsvarende kan verktøy som vannmerking, som er utviklet for å identifisere AI-generert innhold, ofte fjernes eller endres, noe som begrenser deres pålitelighet.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Begrensningene til individuelle sikkerhetstiltak betyr at ‘defense-in-depth’ kan være nødvendig for å forhindre visse skadelige utfall. For eksempel kan et system kombinere en sikkerhetsopplært modell med inndatafiltre, utdatafiltre og innholdsovervåkere.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Siden publiseringen av forrige rapport (januar 2025) har forskere gjort fremskritt med å forbedre sikringstiltakene, men grunnleggende begrensninger består. For eksempel har suksessraten for angrep som er utformet for å omgå sikringstiltakene blitt lavere, men forblir fortsatt relativt høy. Det finnes også grunnleggende begrensninger for hvor grundig modeller med åpen vekt kan sikres.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ En nøkkelutfordring for beslutningstakere er at det finnes begrenset evidens for hvor effektive sikkerhetstiltak er på tvers av ulike reelle bruksområder for generelle AI-systemer. AI-utviklere varierer i stor grad i hvor mye informasjon de deler om sine sikkerhetstiltak og sin overvåking. En ytterligere utfordring er mulige avveininger mellom å innføre strengere sikkerhetstiltak og å opprettholde systemets ytelse eller anvendelighet.
>oldlace|black||11|15|br      


AI-utviklere kan bruke flere nyttige, men ufullkomne tekniske sikkerhetstiltak for å redusere og håndtere risiko fra generell-formål AI-systemer, men utfordringer knyttet til robusthet består. Utviklere kan fortsatt ikke fullt ut forhindre generell-formål AI-systemer i å utføre selv godt kjente og åpenlyst skadelige handlinger, som å gi brukere instruksjoner om å begå kriminelle handlinger. For eksempel har forskere vist at toppmoderne sikkerhetstiltak kan omgås gjennom metoder for adversarial prompting (dvs. «jailbreaks») (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), ved å få modeller til å bryte ned komplekse skadelige oppgaver i trinn (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), og ved enkle modellendringer (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Forskere fortsetter å arbeide med sikkerhetstiltak mot feilfunksjoner og misbruk (‡690). Disse metodene varierer mye i formål og effektivitet, og deres innvirkning avhenger i siste instans av den bredere sosiotekniske og styringsmessige konteksten der AI-systemer bygges og tas i bruk.

Tekniske sikkerhetstiltak kan grovt sett deles inn i tre kategorier: metoder for å utvikle sikrere modeller; metoder brukt under utrulling for overvåking og kontroll; og metoder som støtter økosystemovervåking etter utrulling. Tabell 3.6 oppsummerer de tekniske sikkerhetstiltakene som er omtalt, deres effektivitet og gjenstående utfordringer.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Utvikle tryggere modeller
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dataklargjøring (‡1167)
  Fjerner skadelig data for å hindre at en modell lærer farlige egenskaper. Disse metodene kan være nyttige, inkludert ved utvikling av open-weight-modeller som mangler skadelige egenskaper og motstår skadelig fine-tuning (‡55). Imidlertid finnes det utfordringer knyttet til kurateringsfeil og skalering (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Forsterkende læring fra menneskelige tilbakemeldinger (‡64*)
  Å trene modellen for å tilpasse seg angitte mål, for eksempel å være nyttig og ufarlig. Dette er en effektiv måte for modeller å lære nyttige atferder på (‡64*). Imidlertid kan overoptimalisering for menneskelig godkjenning få modeller til å oppføre seg villedende eller smiskende (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pluralistiske justeringsteknikker (‡1170)
  Å trene modellen til å integrere flere ulike synspunkter på hvordan den skal opptre. Disse teknikkene bidrar til å redusere i hvilken grad modeller favoriserer bestemte synspunkter (‡1170). Imidlertid, til tross for disse teknikkene, er uenighet mellom mennesker uunngåelig, og det er vanskelig å utforme bredt aksepterte måter å balansere konkurrerende syn på (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adversarial trening (‡677)
  Å trene modellen til å nekte å forårsake skade (selv i ukjente kontekster) og til å motstå angrep fra ondsinnede brukere (f.eks. «jailbreaks»). Dette er en effektiv metode for å få modeller til å motstå forsøk på misbruk (‡1064), men robusthetsutfordringer vedvarer (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Maskin‘unlearning’ (‡1175, ‡1176)
  Å trene en modell ved hjelp av spesialiserte algoritmer som har som mål å aktivt undertrykke skadelige egenskaper (f.eks. kunnskap om biofarer). Disse teknikkene gir en målrettet måte å fjerne skadelige egenskaper fra modeller (‡1175, ‡1176), men dagens algoritmer for unlearning kan være lite robuste og kan ha utilsiktede effekter på andre egenskaper (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tolkbarhet og sikkerhetsverifiseringsverktøy (‡1177)
  En mangfoldig familie av design- og verifikasjonsmetoder, ment å gi mer strengt samsvar for å sikre at modeller har bestemte sikkerhetsrelaterte egenskaper. De gjør det mulig for vurderere å gi mer høyverdig sikkerhetsbekreftelse (‡1177), men dagens metoder bygger på antakelser og er sjelden konkurransedyktige når det gjelder ytelse i praksis (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Overvåking og kontroll
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Maskinvarebaserte overvåkingsmekanismer (‡1179, ‡1180, ‡1181)
  Verifiserer at autoriserte prosesser kjører på maskinvare for å studere sikkerhetstrusler eller etterlevelse av regelverk. Disse mekanismene tilbyr unike måter å overvåke hvilke beregninger som kjøres på maskinvaren og av hvem (‡1181). Imidlertid kan maskinvaremessige mekanismer ikke overvåke alle typer trusler, og noen teknikker krever spesialisert maskinvare (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Brukerinteraksjonsovervåkere (‡1154, ‡1166)
  Overvåking av brukerinteraksjoner for tegn på ondsinnet bruk kan hjelpe utviklere med å avslutte tjenesten for ondsinnede brukere (‡1154, ‡1166). Imidlertid kan håndheving utilsiktet hindre nyttig forskning på sikkerhet (‡689), og noen former for misbruk er vanskelige å oppdage (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Brukerinteraksjonsovervåkere (‡1154, ‡1166)
  Overvåking av brukerinteraksjoner for tegn på ondsinnet bruk kan hjelpe utviklere med å avslutte tjenesten for ondsinnede brukere (‡1154, ‡1166). Imidlertid kan håndheving utilsiktet hindre nyttig forskning på sikkerhet (‡689), og noen former for misbruk er vanskelige å oppdage (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Innholdsfiltre (‡65*, ‡725)
  Filtrering av potensielt skadelige modelleinnganger og -utganger er en svært effektiv måte å redusere utilsiktede skader og misbruksrisiko (‡725). Imidlertid krever filtre ekstra beregning, og er sårbare for enkelte angrep (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modellens interne beregningsmonitorer (‡744, ‡1183, ‡1184)
  Overvåking for tegn på bedrag eller andre skadelige interne former for erkjennelse i modeller kan være en effektiv måte å oppdage bedrag (‡744, ‡1183, ‡1184). Imidlertid mangler dagens metoder robusthet og pålitelighet (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kjede-for-tanke-monitorer (‡430, ‡435)
  Overvåking av modellens chain-of-thought-tekst for tegn på villedende atferd eller annen skadelig resonnementatferd er en effektiv måte å forstå og oppdage mangler i hvordan modeller resonerer (‡435). Imidlertid kan de være upålitelige (‡752, ‡753, ‡1186), og hvis modeller trenes til å produsere godartet chain of thought, kan de lære villedende atferd (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mennesket i sløyfen (‡1187, ‡1188, ‡1189)
  Menneskelig tilsyn og overstyringer for systembeslutninger er avgjørende i noen sikkerhetskritiske applikasjoner (‡1187). Imidlertid er disse teknikkene begrenset av automasjonsbias og av begrensninger i hastigheten til menneskelig beslutningstaking (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sandkassing (‡1192)
  Å hindre at en AI-agent direkte påvirker verden er en effektiv måte å begrense den skaden den kan forårsake (‡1192). Imidlertid begrenser sandboxing systemets evne til direkte å gjennomføre enkelte oppgaver (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Verktøy for å legge til rette for økosystemovervåking
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teknikker for identifisering av AI-modell (‡1193*, ‡1194)
  Å gjøre modeller, eller individuelle instanser av modeller, lettere å identifisere i reelle brukssituasjoner bidrar til digital forensikk og økosystembevissthet (‡1195). Imidlertid kan disse teknikkene omgås med enkelte typer endringer av modeller (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Arvslinje for AI-modellvederledning (‡1197)
  Disse teknikkene gjør det mulig for forskere å studere hvordan modeller endres i AI-økosystemet, spesielt åpenvektsmodeller. De bidrar til digital forensikk og økosystembevissthet (‡1198), men det ville vært nødvendig med store prosjekter for grundig å kartlegge økosystemet for åpenvektsmodeller (‡1198).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vannmerker og metadata (‡1199, ‡1200, ‡1201*)
  Disse teknikkene gjør det enklere å oppdage når et stykke tekst, bilde, video osv. er generert eller endret av AI, og av hvilket system. De legger til rette for bedre økosystembevissthet (‡1199, ‡1200, ‡1201*). Imidlertid kan vannmerker og metadata forfalskes eller fjernes ved enkelte endringer i innholdet (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Deteksjon av AI-generert innhold (‡1203, ‡1204, ‡1205*)
  Å forbedre brukeres evne til å skille mellom AI-generert og ekte innhold bidrar til digital forensikk og bevissthet i økosystemet (‡1203, ‡1204). Imidlertid kan klassifisører være upålitelige (‡1205*) og ha varierende ytelse på tvers av modalsiteter.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 3.6: Tekniske sikringstiltak diskutert i denne seksjonen
>white|black||9|11|br Et sammendrag av de tekniske sikringstiltakene som er diskutert i denne delen, delt inn i metoder for å utvikle tryggere modeller, overvåking og kontroll ved utrulling, og teknikker for å legge til rette for økosystemovervåking.


###@ Utvikle tryggere modeller

En første forsvarslinje mot skader fra generelle AI-systemer er å gjøre den underliggende modellen tryggere. Dette delkapittelet dekker sikringstiltak som er «innebygd i modellparametrene» under utviklingsprosessen for modellen (Figur 3.6).

>white|orangered|left|14|15.5|bb Å kuratere treningsdata kan begrense utviklingen av potensielt farlige evner

Generelle AI-modeller er nyttige nettopp fordi de utvikler et bredt spekter av kunnskap og evner etter å ha behandlet treningsdata, men noen typer treningsdata er uforholdsmessig ansvarlige for utviklingen av potensielt farlige evner. For eksempel kan en AI-modell som er trent på virologiske artikler, være bedre i stand til å gi assistanse i potensielt skadelige biologiske oppgaver (‡549, ‡1206*) (se også §2.1.4. Biologiske og kjemiske risikoer). I tillegg kan bilde-/videogeneratorer trent på bilder av menneskelig nakenhet også misbrukes til å lage ikke-samtykkende intime deepfakes (‡308, ‡319) (se også §2.1.1. AI-generert innhold og kriminell aktivitet).

Å filtrere treningsdata er en effektiv avbøtende tiltak mot noen uønskede kapabiliteter (‡319, ‡1167, ‡1207, ‡1208). Imidlertid kan det være vanskelig å filtrere de store datasett som brukes til å trene generelle AI-modeller (‡1168) på grunn av høye kostnader (‡1209), filtreringsfeil (‡1210) og negative effekter på kvaliteten til datasettet (‡1211). Disse utfordringene forverres av den flerspråklige naturen til tekst på internett (‡1212), kulturelle skjevheter i innholdsmoderering (‡1211, ‡1213, ‡1214, ‡1215), og det faktum at hvorvidt et gitt stykke data er ‘skadelig’ avhenger av kontekstuelle faktorer (‡1216). Likevel viser filtrering av potensielt skadelig materiale fra treningsdata lovende resultater for å gjøre modeller mer pålitelig sikre, inkludert å gjøre open-weight-modeller mer motstandsdyktige mot skadelig manipulering (‡55). Sammenhengene mellom innhold i treningsdata og fremvoksende modellkapabiliteter er ikke ennå fullt ut forstått (‡1195), og filtrering ser ut til å være mer effektiv for å begrense skadelige kapabiliteter når den brukes på brede kunnskapsdomener (‡55) sammenlignet med smalere atferd (‡1206, ‡1217). Se §3.4. Open-weight-modeller for videre diskusjon.

![figure 3.6](images/fig3.6_safeguards.png)

##### Figur 3.6: Hvor tekniske sikringstiltak skal anvendes
>white|black||9|11|br Tekniske sikkerhetstiltak kan brukes i ulike faser av modellutvikling. Datakurasjon former hva modeller lærer under pre-trening og finjustering. Treningsbaserte metoder som forsterkningslæring basert på menneskelig tilbakemelding og robusthetstrening justerer modellens atferd. Testemetoder som tilfeldige angrep identifiserer gjenstående sårbarheter. Noen teknikker, som safe-by- design-algoritmer, dekker flere faser. Kilde: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Metoder for å trene generelle AI-modeller for å være hjelpsomme og ufarlige baserer seg i hovedsak på menneskelig tilbakemelding

Det er vanskelig å trene og evaluere modeller på en pålitelig måte for å samsvare med overordnede prinsipper som å være hjelpsom, ufarlig og ærlig. I praksis prøver utviklere å oppnå dette ved å finjustere AI-modeller ved hjelp av demonstrasjoner og tilbakemeldinger fra mennesker. For eksempel er hovedparadigmet for finjustering av AI-modeller, kjent som «forsterkende læring fra menneskelig tilbakemelding», basert på å trene modeller til å produsere utdata som menneskelige annotatører vurderer positivt (‡1218). Imidlertid er positiv tilbakemelding fra mennesker en mangelfull stedfortreder for gunstig atferd (‡737, ‡878, ‡1219, ‡1220) og er begrenset av menneskelig feil og skjevhet (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Dette medfører flere utfordringer: modeller finjustert ved forsterkningslæring fra menneskelig tilbakemelding kan noen ganger blidgjøre brukeren, en atferd kjent som ‘smiger’ (‡358, ‡740, ‡1226, ‡1227); gi svar som er nyttige i noen sammenhenger, men skadelige i andre (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); gi svar som er vanskelige å vurdere med hensyn til korrekthet (‡1233); eller utføre handlinger hvis nyttighet eller skadelighet er et spørsmål om personlig oppfatning (‡1234). Bord 3.7 gir eksempler på disse utfordringene. Noe forskning tar sikte på å utvikle metoder for å hjelpe mennesker med å vurdere løsninger på komplekse oppgaver bedre med hjelp fra KI (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Disse metodene har imidlertid for tiden begrenset pålitelighet, og i hvilken grad de brukes til å trene dagens mest avanserte KI-modeller, er ikke offentlig kjent.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sykofansi/forlemmelse (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Forklaring:
>white|black|left|11|13|br Modellen gir bare positive tilbakemeldinger og klarer ikke å påpeke mangelen på en korrekt 5-7-5 haiku-stavelsesstruktur.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Noen handlinger er nyttige i noen sammenhenger, men skadelige i andre (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Forklaring:
>white|black|left|11|13|br Informasjon om biologisk risiko kan brukes til opplæring og forsvar, men også til å informere ondsinnede aktører.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riktig oppførsel er vanskelig å verifisere (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Forklaring:
>white|black||11|13|br Det er vanskelig å vurdere korrektheten av dette svaret fordi det krever medisinsk ekspertise. Selv for en erfaren lege krever vurdering av svar som dette tid og nøye oppmerksomhet på detaljer.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Mennesker er uenige om hva som er riktig (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Forklaring:
>white|black|left|11|13|br Folk er uenige i betydelig grad om hva som er det riktige svaret.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 3.7: Brukerforespørsel og svar fra AI-modellen
>white|black||9|11|br Eksempler på utfordringer med å spesifisere og gi insentiver til fordelaktige handlinger fra AI-modeller.


>white|orangered|left|14|15.5|bb Mennesker er ikke alltid enige om hvilke atferd som er ønskelig, noe som krever metoder for å balansere konkurrerende preferanser

Mennesker er ikke alltid enige om hvilke svar eller handlinger AI-modeller skal eller ikke skal gi (‡1006). Dette gjør det i grunnleggende forstand utfordrende å utvikle modeller hvis handlinger og virkninger i stor grad er i tråd med samfunnets interesser (‡420). Noen forskere studerer hvis preferanser som gjenspeiles i AI-systemer (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) og arbeider med å utvikle teknikker for “pluralistisk samsvar” som tar sikte på å finne en balanse mellom konkurrerende preferanser (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). For eksempel kan AI-utviklere designe systemer for å unngå å generere kontroversielle svar ved å avslå å svare på visse forespørsler, eller innrette seg etter den midterste oppfatningen i et relevant utvalg av mennesker, eller personalisere systemer for individuelle brukere.

En vanlig utfordring for disse tilnærmingene er at, generelt sett, kan ikke AI-systemer innrette seg like godt etter alles preferanser, og at deres etterfølgende samfunnsmessige virkninger vil påvirke ulike grupper mennesker på ulike måter. Noen forskere har hevdet at de fleste tekniske tilnærminger til pluralistisk innretting ikke klarer å ta tak i, og potensielt til og med distraherer fra, dypere utfordringer, som systematiske skjevheter, sosiale maktdynamikker og konsentrasjonen av rikdom og innflytelse (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb AI-utviklere bruker ‘adversariell trening’ for å forbedre modellens robusthet

Det er utfordrende å sikre at AI-modeller robust oversetter de fordelaktige atferdene de lærer under trening til faktiske distribusjonskontekster i den virkelige verden. Selv modeller trent med et ‘perfekt’ læringssignal kan mislykkes i å generalisere vellykket til alle tidligere ukjente kontekster (‡738, ‡739, ‡1255, ‡1256, ‡1257). For eksempel har noen forskere funnet at chatboter oftere tar skadelige handlinger på språk som er underrepresentert i treningsdataene deres (‡159, ‡880, ‡1258*, ‡1259), som omfatter mange språk som fortrinnsvis snakkes i Global South.

I senere år har forskere også utviklet et stort rammeverk av teknikker for «adversarial attack» som kan brukes til å få modeller til å generere potensielt skadelige svar (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). For eksempel samlet en nylig initiativ dugnad inn mer enn 60,000 ulike eksempler på vellykkede angrep mot ledende AI-modeller, noe som fikk dem til å bryte selskapenes retningslinjer for akseptabel modellatferd (‡1149). Bord 3.8 viser eksempler på «jailbreak»-teknikker som forskere har vist at kan få modeller til å etterkomme skadelige forespørsler.

En metode for å forbedre robustheten til modeller er kjent som «adversarial training» (‡1064). Den innebærer å konstruere «angrep» (f.eks. jailbreaks) som er utformet for å få en modell til å oppføre seg på en uønsket måte, og å trene modellen til å håndtere disse angrepene på en hensiktsmessig måte. Imidlertid er adversarial training ufullkommen (‡1260, ‡1261). Angripere klarer konsekvent å utvikle nye, vellykkede angrep mot toppmoderne modeller (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Siden utviklere trenger spesifikke eksempler på feilmønstre for å kunne trene mot dem (‡512, ‡1263), er resultatet et pågående «katt og mus»-spill der utviklere stadig oppdaterer modeller som svar på nylig avdekkede sårbarheter, og der antagonister stadig søker etter nye angrep. Noen forskere har foreslått adversarial training i større skala (‡1264, ‡1265) eller nye algoritmer (‡675, ‡676, ‡1263, ‡1266, ‡1267) for å forbedre robustheten, men moderne AI-systemer forblir vedvarende sårbare.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Gjør skadelige forespørsler i chiffertekst, for eksempel morsekode (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Last systemet med eksempler på samsvarende svar på skadelige forespørsler (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Gjør skadelige forespørsler på lavressursspråk som sannsynligvis blir brukt mindre under trening (f.eks. Swahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Del en skadelig oppgave ned i flere ufarlige deloppgaver (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bord 3.8: Jailbreaking-strategier
>white|black||9|11|br Ondsinnede aktører og red teams har brukt ulike typer «jailbreaks» for å få AI-modeller til å etterkomme skadelige forespørsler som de normalt ville avslå på grunn av sikkerhetstiltak. Eksempelutganger ble skrevet av rapportforfatterne for illustrasjonsformål. Mange nåværende toppmodeller innen kunstig intelligens motstår nå de fleste av disse metodene, men nye jailbreak-teknikker fortsetter å bli oppdaget.


>white|orangered|left|14|15.5|bb «Glemming»-teknikker kan redusere spesifikke skadelige modellegenskaper

En annen strategi for å redusere risiko fra generell-purpose AI er å finjustere modeller for å mangle evner innenfor bestemte høy-risikoområder (‡1175, ‡1176). For eksempel arbeider forskere med å utvikle algoritmer for «machine unlearning» som kan undertrykke evner knyttet til biotrusler eller til å generere fotorealistiske bilder av nakne menneskekropper (‡903, ‡1272, ‡1273) på en målrettet måte. Disse metodene kan gjøre modeller betydelig tryggere, men det skjer på bekostning av å begrense noen positive bruksområder av de «unlearned» evnene. Å begrense kunnskapen til AI-modeller innenfor skadelige domener har også blitt foreslått som en måte å utforme «tamper-resistant» open-weight modeller på som kan motstå skadelig finjustering (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Så langt har det imidlertid vært utfordrende å få dette til robust (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Se §3.4. Open-weight modeller for videre diskusjon.

>white|orangered|left|14|15.5|bb Noen forskere arbeider med metoder for sterkere sikkerhetsgarantier gjennom å tolke modellinterne tilstander eller matematisk verifikasjon

Noen forskere arbeider med metoder for mer strengt å verifisere sikkerhetsrelaterte egenskaper ved modeller. I én tilnærming har forskere som mål å tolke modellens interne beregninger for enten å identifisere risikoer eller å frembringe mer overbevisende argumenter for at modellen er trygg (‡1285, ‡1286). For eksempel, i et proof of concept, viste forskere at verktøy for å analysere den interne beregningen i en språkmodell kunne hjelpe vurderere med å identifisere skadelig atferd (‡1287). I 2025 begynte også Anthropic å analysere modellinterner som en måte å studere modellens situasjonsbevissthet og ‘intensjon’ (‡2). Imidlertid er denne typen metoder for tiden ikke vanlig, eller kjent for å være konkurransedyktige med andre evalueringsteknikker.

En annen tilnærming for å gi sterkere sikkerhetsgarantier innebærer å konstruere matematiske bevis for at en modell vil oppfylle bestemte sikkerhetsbetingelser (‡1177, ‡1282, ‡1288). Imidlertid forutsetter disse bevisene at testkonteksten samsvarer med distribusjonskonteksten, og de er ikke testet mot mange typer angripere.

De kan heller ikke for øyeblikket skaleres til store modeller. Samlet sett er det betydelig uenighet blant eksperter om løftet om tolkbarhet og metoder for formell verifisering.

###@ Overvåking og kontroll ved distribusjonstidspunkt

I tillegg til sikringstiltak som er implementert under utvikling av modellen, finnes det en andre linje med forsvar mot skadelig atferd i form av eksterne sikringstiltak som fokuserer på overvåking og kontroll av en models eller et systems handlinger under utrulling. Slike sikringstiltak bidrar til å redusere risikoen for feilfunksjoner og misbruk, som f.eks. hallusinerte utdata og skadelige instruksjoner.

>white|orangered|left|14|15.5|bb Modell-deployere kan bruke et mangfold av verktøy for å identifisere og håndtere høy-risiko modellatferd

Når et AI-system kjører, kan en utplasserer overvåke etter tegn på risiko og gripe inn hvis de oppstår. For eksempel kan de inspisere en modells inndata for tegn på advarende angrep, filtrere upassende innhold fra utdata, eller overvåke systemets tankekjede for tegn på skadelige planer. Punkter der utplasserere kan overvåke og gripe inn i hvordan folk bruker systemene sine, omfatter maskinvare (‡1180, ‡1181), brukerinteraksjoner (‡1154, ‡1166), inndata og utdata (‡65, ‡725, ‡1182), interne beregninger (‡744, ‡1183, ‡1184) og tankekjede (‡430, ‡435). Det finnes også flere handlinger utplasserere kan utføre når risiko identifiseres. Dette omfatter logging av informasjon, filtrering/modifisering av skadelig innhold, flagging av unormal aktivitet, systemavstengninger eller aktivering av fail-safes. Figur 3.7 viser eksempler på vanlige mekanismer for overvåking og kontroll.

Fordi de er allsidige og ofte effektive, brukes disse mekanismene i stor utstrekning og kan forhindre mange typer utilsiktede skader (‡725, ‡751, ‡1289). Likevel er disse beskyttelsestiltakene ufullkomne, særlig under ondsinnede angrep optimalisert for å få dem til å mislykkes (‡752, ‡1182). Nyere forskning har også undersøkt hvordan overvåking kan være upålitelig hvis et system er optimalisert ved hjelp av score fra en monitor, for eksempel ved å gjøre kjedet av tanke mindre pålitelig (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Figur 3.7: Overvåkings- og kontrollteknikker
>white|black||9|11|br Overvåkings- og kontrollteknikker virker på flere punkter: screening av innputt- og utputtdata for skadelig innhold, sporing av interne modelltilstander, begrensning av eksterne handlinger gjennom sandboxing, og opprettholdelse av menneskelig tilsyn. Kilde: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Mennesker i sløyfen muliggjør direkte tilsyn i settinger med høye konsekvenser

For å redusere sjansen for feil fra AI-agenter (se §2.2.1. Pålitelighetsutfordringer), kan utplasserere ha som mål å designe AI-systemer som fungerer i samarbeid med mennesker i stedet for å være fullt autonome (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Dette er viktig for brukstilfeller der feil beslutninger kan føre til betydelig skade, slik som innen finans, helse eller politi. Imidlertid er det ofte upraktisk å ha en ‘human in the loop’. Noen ganger skjer beslutningstaking for raskt, slik som i chatapplikasjoner med millioner av brukere. I andre tilfeller kan menneskelig skjevhet og feil forsterke risikoene på grunn av kumulative feil (‡1187). Mennesker i loopen har også en tendens til å utvise ‘automatiseringsbias’, som betyr at de ofte legger mer tillit til AI-systemet enn det som er berettiget (‡1190, ‡1191) (se §2.3.2. Risikoer for menneskelig autonomi).

>white|orangered|left|14|15.5|bb 'Sandboxing' beskytter mot risikoer fra autonome atferder

AI-agenter som kan opptre autonomt uten begrensninger på nettet eller i den fysiske verden utgjør forhøyede risikoer (se §2.2.1. Pålitelighetsutfordringer). «Sandboxing» innebærer å begrense måtene som AI-agenter kan påvirke verden direkte på, noe som gjør det mye enklere å føre tilsyn med og håndtere dem (‡640, ‡1192, ‡1295). For eksempel kan det å begrense en AI-systems evne til å publisere på internett eller redigere et datasystems fillager hindre uforutsette skader fra uforutsette handlinger (‡1296). Imidlertid kan ikke disse tilnærmingene alltid brukes for applikasjoner der et AI-system nødvendigvis må handle direkte i verden.

###@ Økosystemovervåkingsverktøy: modell- og dataproveniens

Modell- og dataproveniensverktøy er tekniske verktøy for å studere AI-økosystemet, for å forbedre bevisstheten om de nedstrøms bruksområdene og virkningene til AI-systemer.

>white|orangered|left|14|15.5|bb AI system-proveniens-teknikker hjelper til med å spore bruken og effektene av systemer

Utviklere og de som tar i bruk og drifter modeller, kan bruke ulike teknikker for å studere modellbruk og spredning «i vill tilstand». For eksempel kan de gi modeller unike identifiserende atferder (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) eller bruke unike mønstre på vektene til individuelle åpenvektsmodeller (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Imidlertid er det et åpent problem å gjøre disse teknikkene mer motstandsdyktige mot modifikasjoner av modeller (‡1195, ‡1196*). Forskere jobber også med metoder for å «utlede modellheritasje» (‡1197, ‡1198, ‡1305, ‡1306), som kan bidra til å besvare spørsmål av typen: «Var modell X en finjustert eller destillert versjon av modell Y?» Til slutt jobber noen utviklere med protokoller og infrastruktur for AI-agenter for å legge til rette for identifisering og verifisering når de samhandler med eksterne systemer (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Figur 3.8: Vannmerker legger inn umerkelige forstyrrelser i bilder og lyd
>white|black||9|11|br Vannmerker innebygger usynlige forstyrrelser i bilder og lyd som gjør at AI-generert innhold kan identifiseres av deteksjonsverktøy. I denne figuren er både bilde- og lydvannmerkene overdrevet for synlighet. Kilde: Chameleon-bilde fra Unsplash (‡1313*). Andre elementer laget av Report-forfatterne. International AI Safety Report 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Figur 3.9: Suksessrater for prompt injection-angrep
>white|black||9|11|br Suksessrater for prompt injection-angrep, slik de er rapportert av AI-utviklere for store modeller lansert mellom mai 2024 og august 2025. Hvert punkt representerer andelen vellykkede angrep innen 10 forsøk mot en gitt modell kort tid etter lansering. Den rapporterte suksessraten for slike angrep har falt over tid, men forblir relativt høy. Kilde: Zou et al. 2025 (‡1149), sitert i Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb AI-innholdsdeteksjonsteknikker bidrar til å overvåke spredningen og effektene av AI-generert innhold

Vannmerker, metadata og andre AI-innholddetektorer kan hjelpe forskere med å spore og studere den reelle innvirkningen i verden av AI-generert innhold. 

Først, datavannmerker er subtile men tydelige mønstre som settes inn i digitalt innhold, og som kan kode informasjon om deres opprinnelse (‡1199, ‡1200, ‡1201*). For tekst tar de typisk form av subtile skjevheter i ordvalg og stil (‡1308, ‡1309); for bilder og video, subtile mønstre over piksler (‡1310); og for lyd, subtile mønstre i lydbølger (‡1311). Figur 3.8 illustrerer dette.

Foruten vannmerker kan AI-generert innhold også lagres ved hjelp av filformater som lagrer metadata om hvordan de ble generert. For eksempel lagrer mange mobile enheter bilde- og lydfiler ved hjelp av et filformat som kan lagre informasjon om kamerainnstillinger, tid, lokasjon osv. (‡1312). Tilsvarende metadata kan brukes til å lagre informasjon om hvorvidt data ble generert av et AI-system. På samme måte som fingeravtrykk i kriminalteknikk kan vannmerker og metadata manipuleres eller fjernes, men de er likevel nyttige.

Forskere jobber også med å utvikle detektorer for AI-generert innhold (‡1203, ‡1204, ‡1205*) for å bidra til å identifisere AI-generert innhold i praksis, selv når det ikke finnes noe vannmerke eller metadata tilgjengelig. Imidlertid har disse identifikasjonsteknikkene en begrenset suksessrate.

###@ Oppdateringer

Siden publiseringen av forrige rapport (januar 2025) er det gjort fremskritt i utviklingen av AI-systemer med flere effektive lag av sikringstiltak. Som diskutert i §3.2. Risikostyringspraksis, er defence-in-depth et kjerneprinsipp i risikostyring (‡1314). For eksempel blir AI-systemer som kombinerer sikkerhetstrente modeller med innholdsfiltre, utdatafiltre og andre innholdsovervåkere i økende grad studert og tatt i bruk (‡32, ‡65, ‡1182*). Nylig forskning har også vist at, selv om utviklere av modeller har gjort fremskritt med å øke robustheten mot forsøk på å omgå sikringstiltak, lykkes angripere fortsatt i høy grad (Figur 3.9).

###@ Bevismangler

Mer dokumentasjon er nødvendig for å hjelpe forskere med å forstå og ta høyde for begrensningene i eksisterende tilnærminger. Tekniske sikkerhetstiltak for AI-systemer blir forbedret, men teknikkene lider av begrensninger. For eksempel har fremdriften med å forbedre robusthet i verste fall for generelle AI-systemer vært langsom, og det finnes grunnleggende begrensninger for hvor grundig åpent vektede modeller kan sikres og overvåkes (‡1195, ‡1315, ‡1316) (se også §3.4. Åpent vektede modeller). Samtidig er ikke alle tekniske sikkerhetstiltak like vanlige, like effektive eller like godt dokumentert i den virkelige verden. For eksempel brukes adversarial trening nesten overalt på toppmoderne modeller (‡64*, ‡677), mens modellfortolkbarhet og formelle verifikasjonsteknikker har blitt lite brukt i produksjonssystemer til dags dato (‡1177, ‡1285).

###@ Utfordringer for beslutningstakere

Viktige utfordringer for beslutningstakere omfatter å avgjøre om og hvordan de skal støtte forskning, utvikling, evaluering og innføring av tekniske sikkerhetstiltak og overvåkingsmetoder. Dette er utfordrende fordi forskernes forståelse av hvordan man best kan sikre mekanismer i praksis, fortsatt er i utvikling, og beste praksis er ikke ennå etablert. For eksempel anvender ulike utviklere ulike sikkerhetstiltak, og deres tilnærminger til teknisk risikoredusering mer generelt varierer betydelig (‡1116). Til slutt betyr ikke tilstedeværelsen av effektive tekniske sikkerhetstiltak i seg selv at sikkerhet er ivaretatt, ettersom innføring og implementering kan variere på tvers av utviklere og utplasseringskontekster.

