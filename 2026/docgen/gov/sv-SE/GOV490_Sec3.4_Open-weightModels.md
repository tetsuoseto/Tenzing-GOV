##########
>white|orangered|left|14|30|hr Avsnitt 3.4
### 3.4. Öppna viktmodeller
>white|orangered|left|24|30|hb Öppna viktmodeller

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Viktig information
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Åtkomstnivån som AI-företag tillhandahåller till sina modellers “vikter” påverkar de risker som dessa modeller medför. Vikter är de matematiska parametrar som gör att AI-modeller kan bearbeta indata och generera utdata. För varje given modell kan företagen välja att hålla vikterna helt privata, ge vissa användare begränsad åtkomst eller tillåta vem som helst att ladda ner dem i sin helhet. Modeller vars vikter är offentligt tillgängliga kallas “open-weight models”.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Open-weight-modeller underlättar forskning och innovation, men deras skydd är lättare att avlägsna. Runt om i världen kan olika aktörer – särskilt de med färre resurser – använda open-weight-modeller för forsknings- och kommersiella ändamål. Däremot, jämfört med closed-weight-modeller, är open-weight-modeller lättare att modifiera för att uppvisa potentiellt skadliga beteenden, och  s mer svårt.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Öppna viktmodellsleveranser är oåterkalleliga. När de väl har släppts kan modellvikter inte återkallas. Detta gör det svårare att mildra potentiella skador som kan uppstå till följd av att en modell med farliga förmågor släpps.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sedan publiceringen av den senaste rapporten (januari 2025) har större släpp av öppet viktade modeller minskat förmågeklyftan gentemot ledande slutna modeller. Utvecklare i Kina DeepSeek och Alibaba släppte sina R1- respektive Qwen-modeller, vilka uppnådde prestanda som var jämförbar med ledande slutna modeller, medan OpenAI släppte sina första öppet viktade modeller sedan 2019. Förmågorna hos ledande slutna modeller uppskattas nu vara mindre än ett år före ledande öppet viktade modeller på framstående AI-benchmarks.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ En central policyutmaning är att komma åt de fördelar som open-weight-modeller tillhandahåller samtidigt som man hanterar deras unika risker. Ett angreppssätt är att utvärdera open-weight-modeller i termer av deras ”marginella risk”: i vilken utsträckning deras lansering kontrafaktiskt ökar den samhälleliga risken utöver den som redan orsakas av befintliga modeller eller andra tekniker. Detta är dock komplext i praktiken. Små ökningar av den marginella risken över tid kan också summeras till betydande ökningar av den totala risken.
>oldlace|black||11|15|br      


Öppna viktmodeller, vars parametrar är offentligt tillgängliga för nedladdning, får tydliga konsekvenser för många av de utmaningar som behandlats i de föregående avsnitten. En AI-modells ”vikter” innehåller den avgörande informationen som gör att den kan generera användbara svar för användare. När väl dessa vikter har släppts kan de inte återkallas: vem som helst kan ladda ner, studera, modifiera, dela och använda dem på sina egna datorer eller i sina molnkonton. När vikter är öppet tillgängliga kan andra lättare bygga vidare på och modifiera modellen, tillgodose olika behov och driva innovation (‡1317). Men genom samma mekanism kan användare med illvilliga avsikter också lättare ta bort skyddsåtgärder och modifiera öppna viktmodeller för skadliga användningsfall (‡1122, ‡1160). Detta har väckt frågan om huruvida vissa öppna viktmodeller bör omfattas av särskilda krav (t.ex. mer rigorös testning före lansering) eller, omvänt, ges särskilda undantag (t.ex. från krav på regulatorisk rapportering) (‡1033).

###@ Bakgrund om open-weight-modeller

>white|orangered||14|15.5|bb Öppna viktmodeller kan vara, men är inte nödvändigtvis, ”open source”-modeller

Även om de ofta benämns ”open source”, beskrivs de flesta offentligt släppta modeller mer korrekt som ”open-weight”. Detta beror på att även om utvecklare tillhandahåller modellvikterna så släpper de inte den tillhörande träningskoden eller dataseten. Vidare kännetecknas öppen källkod-mjukvara vanligtvis av tillåtande licenser som ställer minimikrav på efterföljande aktörer som använder eller modifierar mjukvaran (‡1318). Till exempel har Metas Llama-modeller restriktiva licensvillkor och innehåller endast inferenskod, inte träningskod, och betraktas därför vanligtvis inte som open source (‡1319, ‡1320). Modellsläppsalternativ finns längs ett spektrum från helt slutet till helt open source, med olika risk-nyttighetstrade-offs i varje läge (‡1086*, ‡1320, ‡1321). Tabell 3.9 beskriver dessa alternativ.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Helt stängd
  Användare kan inte interagera direkt med modellen alls
  Exempel: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Hanterad åtkomst
  Användare kan endast interagera via en specifik applikation eller ett specifikt gränssnitt, till exempel en mobil chattbotapplikation
  Exempel: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb API-åtkomst till modellen
  Användare kan skicka förfrågningar till modellen via kod, vilket möjliggör användning i externa applikationer
  Exempel: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb API-åtkomst för finjustering
  Användare kan finjustera modellen för sina specifika behov
  Exempel: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Öppna vikter: vikter tillgängliga för nedladdning
  Användare kan ladda ner och köra modellen på sina egna datorer
  Exempel: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Vikter, data och kod finns tillgängliga för nedladdning med användningsbegränsningar
  Användare kan ladda ner och köra modellen samt inferens- och träningskoden, men det finns vissa licensbegränsningar för användningen
  Exempel: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Fullt öppen: vikter, data och kod tillgängliga för nedladdning utan användningsbegränsningar
  Användare har full frihet att ladda ner, använda och modifiera modellen, full kod och data
  Exempel: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 3.9: Alternativ för modell-delning som sträcker sig från helt sluten till helt öppen
>white|black||9|11|br Ett illustrativt urval av modelleringsdelningsalternativ, från helt slutna modeller (modeller är privata och hålls endast för proprietär användning) till helt öppna och open source-modeller (modellvikter, data och kod är fritt och offentligt tillgängliga utan begränsningar i användning, modifiering och delning). Modeller som faller inom de första fyra kategorierna benämns ofta som ”slutna”. Detta avsnitt fokuserar på de tre nedersta raderna. Källa: anpassad från Bommasani, 2024 (‡1317).


###@ Fördelar och risker

>white|orangered|left|14|15.5|bb Öppna viktmodeller kan anpassas och utvärderas mer enkelt

Öppna modeller med vikter erbjuder betydande fördelar för forskning, innovation och tillgång. Som diskuteras i §1.1. Vad är allmännyttig AI? är det extremt dyrt att träna allmännyttiga AI-modeller – ledande modeller kostar hundratals miljoner dollar att utveckla. Att öppet släppa modellvikter gör att aktörer med sämre resurser kan replikera, studera och bygga vidare på befintliga system. Utan sådan tillgång riskerar samhällen i lågresursregioner att stängas ute från AI:s fördelar, vilket gör öppna vikter avgörande för att möjliggöra deltagande för den globala majoriteten i AI-utveckling (‡1322). Underleverantörsutvecklare kan finjustera modeller för olika tillämpningar, till exempel genom att anpassa dem för underresurssatta minoritetsspråk eller optimera prestanda för specifika uppgifter som juridisk framställning eller medicinsk journalanteckning (‡1323, ‡1324*). På så sätt kan modeller med öppna vikter göra det möjligt för fler människor och samhällen att använda och dra nytta av AI än vad som annars skulle vara möjligt (‡1325). När det gäller modeller som inte är tillräckligt kapabla för att vara farliga kan dessa fördelar väga tyngre än den ökade risken med att släppa vikterna öppet, även om detta beror på relevanta beslutsfattares riskbenägenhet.

Open-weight-utsläpp breddar också den pool av utvecklare och forskare som kan studera modellen, utvärdera dess förmågor, testa efter sårbarheter och iterera på förbättringar (‡1326, ‡1327). Detta gör det mer sannolikt att både nyttiga tillämpningar och skadliga brister identifieras, även om det inte är garanterat (‡1328, ‡1329). Användare kan också köra open-weight-modeller på sina egna enheter, vilket gör att de kan behålla kontrollen över känslig data och undvika att skicka den till tredjepartsservrar.

Det finns ytterligare fördelar när utvecklare delar med sig av information såsom träningsdata, kod, utvärderingsverktyg och dokumentation samt modellvikter (‡1320, ‡1330, ‡1331, ‡1332*). Med mer information kan efterföljande utvecklare och andra forskare bättre förstå öppetviktsmodeller och anpassa dem till nya tillämpningar.

>white|orangered|left|14|15.5|bb Skydden i öppna viktmodeller är enklare att ta bort, vilket möjliggör potentiellt skadlig användning

Öppenviktsmodeller med öppen vikt utgör också ytterligare risker eftersom deras skyddsåtgärder är lättare att ta bort. Även om både öppenvikts- och slutna modeller kan ha skyddsåtgärder för att vägra skadliga användarförfrågningar, är dessa skydd mycket lättare att ta bort för öppenviktsmodeller. Skadliga aktörer kan finjustera en modell för att optimera dess prestanda för skadliga tillämpningar, ta bort delar av koden som är avsedda att förhindra skadliga användningar, eller ångra tidigare säkerhetsfinjustering (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Som ett resultat kan öppna modellvikter förvärra missbruksriskerna som diskuteras i §2.1. Risker från skadlig användning genom att ge fler aktörer möjlighet att utnyttja och förstärka befintliga förmågor för skadliga ändamål utan tillsyn (‡1122, ‡1315). Även om många användare varken kommer att ha färdigheten eller incitamentet att ta bort skyddsåtgärder i öppenviktsmodeller, är högt motiverade skadliga aktörer ett problem. Dessutom kan skadliga aktörer också kunna använda öppenviktsmodeller för att identifiera sårbarheter i liknande slutna modeller (‡1055*). Sådana brister är svårare att hitta genom att endast köra slutna modeller, på grund av den större kontroll och den övervakning som leverantörer av slutna modeller kan införa.

>white|orangered|left|14|15.5|bb Att dela modellvikter är oåterkalleligt

När modellvikter finns tillgängliga för publik nedladdning finns det inget sätt att genomföra en total återställning (rollback) av alla befintliga kopior. Internetvärdplattformar som GitHub och Hugging Face kan ta bort modeller från sina plattformar, vilket gör det svårare för vissa aktörer att hitta nedladdningsbara kopior och skapar en betydande spärr för många tillfälliga illvilliga användare (‡1339). Motiverade aktörer kan dock fortfarande skaffa kopior om modellen har laddats ned och återpublicerats någon annanstans eller sparats lokalt. Dessutom är utvecklare på nedströmsnivå som integrerar open-weight-modeller i sina system ocksåver ett arv av eventuella brister, såsom sårbarheter för adversarial-attacker (‡1055) eller modellförmågor att kringgå övervakningssystem (se §2.2.2. Förlust av kontroll) (‡1315). Till skillnad från slutna modeller där värdar kan rulla ut korrigeringar universellt, kan utvecklare av open-weight-modeller inte garantera att uppdateringar kommer att antas av användare.

###@ Uppdateringar

Sedan publiceringen av den senaste rapporten (januari 2025) har kapacitetsgapet mellan ledande open-weight-modeller och slutna modeller minskat. Kinesiska utvecklare har blivit särskilt viktiga leverantörer av open-weight-modeller. I januari 2025 släppte DeepSeek sin R1-modell, som uppnådde prestanda som var jämförbar med OpenAI:s o1 på ett antal benchmarktester (‡1340). Alibabas Qwen-modeller har också fått ökat genomslag och intar från och med augusti 2025 förstaplatsen för en open-weight-modell på Chatbot Arena, ett ofta använt prestanda-benchmarktest (‡1341, ‡1342*). I augusti 2025 släppte OpenAI sina första open-weight-modeller sedan lanseringen av GPT-2 2019, gpt-oss-120b och gpt-oss-20b. Meta har fortsatt att släppa Llama-modeller med öppna vikter. Kapaciteten hos de ledande slutna modellerna uppskattas nu vara mindre än ett år före de ledande open-weight-modellerna på framträdande AI-benchmarktest (Figur 3.10).

###@ Evidensluckor

En viktig kunskapslucka gäller den verkliga effekten av tekniska lösningar för att förhindra missbruk av open-weight-modeller. Forskare har föreslagit olika tillvägagångssätt för att göra modeller manipulationsresistenta. Detta omfattar nya träningstekniker som syftar till att göra modeller motståndskraftiga mot skadlig ändring (‡1276), filtrering av skadligt innehåll från träningsdata (‡55) och försvar mot jailbreaks (‡675, ‡676). Dessa tekniker håller nu på att tas i bruk i verkliga lanseringar från stora utvecklare. Till exempel använde OpenAI några av dessa tekniker i sina gpt-oss-modeller och rapporterade att adversarialt fine-tunade versioner inte nådde höga kapacitetströsklar (‡1344*). Forskning har dock visat att illvilliga aktörer kan inaktivera skydd genom att återträna modeller på skadliga exempel (‡1345, ‡1346). Dessutom är det fortfarande svårt att på ett tillförlitligt sätt utvärdera robustheten hos skydden, vilket gör deras effektivitet mot verkliga attacker osäker (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Figur 3.10: Kapacitetsgap mellan de ledande open-weight- och closed AI-modellerna
>white|black||9|11|br Epoch Capabilities Index (ECI)-poäng för topprankade open-weight (mörkblå) och closed (ljusblå) modeller över tid. ECI sammanställer poäng från 39 benchmarker till en enda allmän förmågeskala. De bästa open-weight-modellerna ligger cirka ett år efter de closed-modellerna. Källa: Epoch AI, 2025 (‡1343).


###@ Åtgärder för att mildra risker

Tekniska motåtgärder för risker med open-weight-modeller verkar under hela processen för AI-utveckling och -distribution (‡1141, ‡1195, ‡1347). Till exempel, när modeller utvecklas kan utvecklare och downstream-adaptrar filtrera känsligt innehåll från träningsdata för att minimera skadliga förmågor. Att ta bort skadliga exempel från en modells träningsdata kan förhindra adversarial fine-tuning 10 gånger mer effektivt än försvar som läggs till efter träning, även om det också kan påverka förmågor som är nyttiga (‡55). Leverantörer av AI-applikationer kan också införa mekanismer för incidentrapportering och respons (‡1348).

Dessutom kan värdplattformar som HuggingFace och GitHub fastställa villkor för tjänsten för att ta bort modeller som har modifierats för skadliga ändamål (‡1141, ‡1324). Modellutvecklare kan ge full åtkomst till granskare innan lansering, eller välja en ”stegvis” lanseringsstrategi – där modeller släpps till successivt större grupper (‡1086). Detta kan hjälpa till att identifiera potentiella felaktiga beteenden eller sårbarheter innan en modell blir brett tillgänglig (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Notera 3.1: Modelsäkerhet för modellvikter
>oldlace|black|left|13|15|hb  Notera 3.1: Säkerhet för modellvikter
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Riskerna som diskuteras i det här avsnittet utgår från att modellvikter släpps avsiktligt. Stängda modellvikter kan dock också bli åtkomliga genom stöld eller läckage. Stängda modeller kostar hundratals miljoner dollar att utveckla (§1.1. Vad är allmän AI?) och är i genomsnitt mer kapabla än öppenviktsmodeller (‡1343). Detta gör dem till attraktiva mål för aktörer som sträcker sig från amatörhackare till nationalstater som vill skaffa ledande AI-modeller.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Stulna stängda modellvikter skulle innebära risker som liknar dem som beskrivs ovan för öppna modellvikter, men potentiellt utan någon av de skyddsåtgärder. Skadliga aktörer skulle kunna ta bort skyddsmekanismer från de mest kapabla modellerna. Till skillnad från legitima utvecklare skulle sådana aktörer inte omfattas av de rykte-, juridiska eller kommersiella begränsningar som idag motiverar företag inom frontlinje-AI att distribuera sina modeller på ett säkert sätt.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Nuvarande säkerhetsnivåer varierar inom branschen och kan vara otillräckliga mot sofistikerade angripare. Vissa utvecklare åtar sig att säkra modellvikter mot cyberkriminella syndikat och interna hot (‡582), medan andra inte har gjort några offentliga säkerhetsåtaganden (‡1109, ‡1349). Forskning indikerar att AI-datacentra kan sakna förmåga att stå emot attacker från de mest sofistikerade och välinvesterade aktörerna (‡582, ‡1350, ‡1351). Per december 2025 finns inga bekräftade, offentligt dokumenterade fall av stöld av modellvikter. Däremot har andra säkerhetsintrång hos ledande AI-företag rapporterats, inklusive ett intrång i Microsofts e-postsystem (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Att täppa till dessa säkerhetsluckor skulle kräva betydande investeringar i hårdvara, programvara, personal och anläggningssäkerhet. Vissa säkerhetsförbättringar skulle kunna genomföras relativt snabbt med samordnade insatser (‡1122). Andra kritiska åtgärder, som att säkra hårdvaruleveranskedjor och anläggningar, skulle dock sannolikt ta flera år (‡1122). Privata företag kan också sakna resurser eller information för att utveckla adekvata skydd på egen hand. Till exempel har AI-utvecklare inte tillgång till klassificerad hotbildsinformation som regeringar har (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Utmaningar för beslutsfattare

En nyckelutmaning för beslutsfattare är att säkra fördelarna med delning av öppna viktmodeller utan att avsevärt öka risken. För att undvika katastrofal skada bör utvecklare av öppna viktmodeller inte släppa modeller utan att utvärdera riskerna, både med etablerade bedömningsmetoder som används för slutna modeller, samt med ytterligare tester, med tanke på att illasinnade aktörer kan finjustera modeller och ta bort säkerhetsskydd. I praktiken kan detta vara svårt eftersom kapabilitetsutveckling kan vara oförutsägbar, öppna viktutsläpp är oåterkalleliga och utvärderingsinsatser krävs för att förutsäga när ett utsläpp skulle innebära betydande potentiell skada. Ett angreppssätt är att utvärdera den ”marginella risken” för öppna utsläpp: i vilken utsträckning utsläppet kontrafaktiskt ökar samhällelig risk utöver den som redan orsakas av befintliga modeller eller andra teknologier (‡556, ‡1033, ‡1354, ‡1355) (se §3.2. Riskhanteringsmetoder). Att uppskatta hur ett system kommer att öka eller minska nedströmsrisk efter att det har distribuerats är dock komplext och kontextberoende. Inkrementella ökningar av risk med successiva utsläpp kan ackumuleras över tid till betydande ökningar av total risk, även om den marginella risken för varje enskilt utsläpp tycks vara acceptabel (‡1356, ‡1357).

AI-kapabiliteternas dubbla användningsområde komplicerar dessutom styrningen ytterligare: funktioner som möjliggör nyttiga tillämpningar inom medicin eller forskning kan återanvändas för skada, och när vikterna är offentliga kan det vara svårt att skilja legitima från illasinnade användningar. Det är också oklart vem som bör hållas ansvarig när öppna viktmodeller modifieras för skadliga ändamål.

