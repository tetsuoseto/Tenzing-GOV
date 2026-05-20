##########
>white|orangered|left|14|30|hr Avsnitt 3.3
### 3.3. Tekniska skyddsåtgärder och övervakning
>white|orangered|left|24|30|hb Tekniska skyddsåtgärder och övervakning

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Viktig information
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Ett brett spektrum av tekniska skyddsåtgärder används i olika stadier av utveckling och användning av AI. Dessa inkluderar tekniker som tillämpas under modellutveckling för att göra system mer robusta och motståndskraftiga mot missbruk (såsom datakuration), övervakning och kontroll vid driftsättning (såsom innehållsfiltrering och mänsklig tillsyn) samt verktyg efter driftsättning för att övervaka det bredare AI-ekosystemet (såsom härkomst och innehållsdetektering).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Tekniska skyddsåtgärder har begränsningar och kan inte på ett tillförlitligt sätt förhindra skadligt beteende i alla sammanhang. Till exempel kan användare ibland få fram skadliga resultat genom att omformulera förfrågningar eller bryta ned dem i mindre steg. På motsvarande sätt kan verktyg som vattenstämplingar som är avsedda att identifiera AI-genererat innehåll ofta tas bort eller ändras, vilket begränsar deras tillförlitlighet.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Begränsningarna i enskilda skyddsåtgärder innebär att ‘defence-in-depth’ kan behövas för att förhindra vissa skadliga utfall. Till exempel kan ett system kombinera en säkerhetstränad modell med inmatningsfilter, utmatningsfilter och innehållsmonitorer.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sedan publiceringen av den förra rapporten (januari 2025) har forskare gjort framsteg med att förbättra skyddsåtgärderna, men grundläggande begränsningar kvarstår. Till exempel har framgångsgraden för attacker som utformats för att kringgå skyddsåtgärderna minskat, men ligger fortfarande på en relativt hög nivå. Det finns också grundläggande begränsningar för hur grundligt modeller med öppen vikt kan skyddas.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ En central utmaning för beslutsfattare är det begränsade underlaget för hur effektiva skyddsåtgärder är i olika verkliga användningsfall av allmänna AI-system. AI-utvecklare varierar kraftigt i hur mycket information de delar om sina skyddsåtgärder och sin övervakning. En ytterligare utmaning är de möjliga avvägningarna mellan att tillämpa starkare skyddsåtgärder och att samtidigt upprätthålla systemets prestanda eller användbarhet.
>oldlace|black||11|15|br      


AI-utvecklare kan använda flera användbara men inte perfekta tekniska skyddsåtgärder för att mildra och hantera risker från generella AI-system, men robusthetsutmaningar kvarstår. Utvecklare kan fortfarande inte fullt ut förhindra att generella AI-system utför även väldokumenterade och tydligt skadliga handlingar, som att erbjuda användare instruktioner för att begå brott. Till exempel har forskare visat att toppmoderna skydd kan kringgås med hjälp av metoder för adversarial prompting (dvs. ”jailbreaks”) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), genom att få modeller att bryta ned komplexa skadliga uppgifter i steg (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), och med enkla modellmodifieringar (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Forskare fortsätter att arbeta med skydd mot funktionsfel och missbruk (‡690). Dessa metoder skiljer sig mycket åt i syfte och effektivitet, och deras påverkan beror i slutändan på det bredare socio­tekniska och styrningsmässiga sammanhang där AI-system byggs och distribueras.

Tekniska skyddsåtgärder kan i stort delas in i tre kategorier: metoder för att utveckla säkrare modeller; metoder som används under driftsättning för övervakning och kontroll; och metoder som stödjer övervakning av ekosystemet efter driftsättning. Tabell 3.6 sammanfattar de tekniska skyddsåtgärder som diskuteras, deras effektivitet och öppna utmaningar.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Att utveckla säkrare modeller
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Datakurering (‡1167)
  Att ta bort skadliga data för att hindra en modell från att lära sig farliga förmågor. Dessa metoder kan vara användbara, inklusive för att utveckla öppna viktmodeller som saknar skadliga förmågor och motstår skadlig finjustering (‡55). Det finns dock utmaningar med urvals- eller insamlingsfel och skalning (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Förstärkningsinlärning från mänsklig återkoppling (‡64*)
  Att träna modellen för att anpassa sig till angivna mål, såsom att vara hjälpsam och ofarlig. Detta är ett effektivt sätt att få modeller att lära sig nyttiga beteenden (‡64*). Däremot kan överoptimering för mänskligt godkännande göra att modeller beter sig bedrägligt eller smickrande (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pluralistiska inriktningstekniker (‡1170)
  Träna modellen för att integrera flera skilda perspektiv på hur den bör agera. Dessa tekniker bidrar till att minska i vilken utsträckning modeller gynnar specifika perspektiv (‡1170). Trots dessa tekniker är dock mänsklig oenighet oundviklig, och det är svårt att utforma allmänt accepterade sätt att balansera konkurrerande synsätt (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adversarial training (‡677)
  Att träna modellen att vägra orsaka skada (även i obekanta sammanhang) och att stå emot attacker från illvilliga användare (t.ex. ”jailbreaks”). Detta är en effektiv metod för att få modeller att stå emot försök till missbruk (‡1064), men robusthetsutmaningar kvarstår (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Maskinens ’unlearning’ (‡1175, ‡1176)
  Att träna en modell med specialiserade algoritmer som innebär att man aktivt undertrycker skadliga förmågor (t.ex. kunskap om biologiska faror). Dessa tekniker erbjuder ett riktat sätt att avlägsna skadliga förmågor från modeller (‡1175, ‡1176), men nuvarande avlärningsalgoritmer kan vara icke robusta och ha oavsiktliga effekter på andra förmågor (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tolkbarhets- och säkerhetsverifieringsverktyg (‡1177)
  En mångsidig familj av design- och verifieringsmetoder avsedda att erbjuda mer rigorös säkerhetsgaranti för att modeller har specifika säkerhetsrelaterade egenskaper. De gör det möjligt för utvärderare att ge högre tillförlitliga säkerhetsförsäkringar (‡1177), men nuvarande metoder bygger på antaganden och är sällan konkurrenskraftiga vad gäller prestanda i praktiken (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Övervakning och kontroll
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Maskinvarubaserade övervakningsmekanismer (‡1179, ‡1180, ‡1181)
  Verifierar att auktoriserade processer körs på maskinvara för att studera säkerhetshot eller regulatorisk efterlevnad. Dessa mekanismer erbjuder unika sätt att övervaka vilka beräkningar som körs på maskinvara och av vem (‡1181). Däremot kan maskinvarumekanismer inte övervaka alla typer av hot, och vissa tekniker kräver specialiserad maskinvara (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Användarinteraktionsövervakare (‡1154, ‡1166)
  Övervakning av användarinteraktioner för tecken på skadlig användning kan hjälpa utvecklare att avbryta tjänsten för skadliga användare (‡1154, ‡1166). Däremot kan efterlevnad oavsiktligt hindra värdefull forskning om säkerhet (‡689), och vissa former av missbruk är svåra att upptäcka (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Användarinteraktionsövervakning (‡1154, ‡1166)
  Att övervaka användarinteraktioner för tecken på skadligt bruk kan hjälpa utvecklare att avsluta tjänsten för skadliga användare (‡1154, ‡1166). Däremot kan efterlevnad oavsiktligt hämma nyttig forskning om säkerhet (‡689), och vissa former av missbruk är svåra att upptäcka (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Innehållsfilter (‡65*, ‡725)
  Att filtrera potentiellt skadliga modellinmatningar och modellutmatningar är ett mycket effektivt sätt att minska oavsiktliga skador och missbruksrisker (‡725). Däremot kräver filter extra beräkning och är sårbara för vissa attacker (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modellens interna beräkningsövervakning (‡744, ‡1183, ‡1184)
  Övervakning för tecken på bedrägeri eller andra skadliga interna former av kognition i modeller kan vara ett effektivt sätt att upptäcka bedrägeri (‡744, ‡1183, ‡1184). Emellertid saknar nuvarande metoder robusthet och tillförlitlighet (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tankegångsövervakare (‡430, ‡435)
  Att övervaka modellens resonemangskedja för tecken på vilseledande beteende eller annan skadlig resonemang är ett effektivt sätt att förstå och upptäcka brister i hur modeller resonerar (‡435). Det kan dock vara opålitligt (‡752, ‡753, ‡1186), och om modeller tränas för att producera ofarlig resonemangskedja kan de lära sig vilseledande beteende (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Människa i slingan (‡1187, ‡1188, ‡1189)
  Mänsklig tillsyn och åsidosättanden av systembeslut är avgörande i vissa säkerhetskritiska tillämpningar (‡1187). Dessa tekniker begränsas emellertid av automatiseringsbias och av gränser för hastigheten i mänskligt beslutsfattande (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Isolering (‡1192)
  Att förhindra att en AI-agent direkt påverkar världen är ett effektivt sätt att begränsa den skada den kan orsaka (‡1192). Ändå begränsar sandboxing systemets förmåga att direkt utföra vissa uppgifter (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Verktyg för att underlätta övervakning av ekosystem
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Identifieringstekniker för AI-modeller (‡1193*, ‡1194)
  Att göra modeller, eller enskilda instanser av modeller, lättare att identifiera i verkliga användningsfall hjälper med digital forensik och ekosystemmedvetenhet (‡1195). Dessa tekniker kan dock kringgås med vissa typer av modellmodifieringar (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Arvtagning genom inferens av AI-modell (‡1197)
  Dessa tekniker gör det möjligt för forskare att studera hur modeller modifieras i AI-ekosystemet, särskilt öppna viktmodeller. De hjälper med digital forensik och ekosystemmedvetenhet (‡1198), men storskaliga projekt skulle behövas för att grundligt kartlägga ekosystemet för öppna viktmodeller (‡1198) .
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vattenstämplar och metadata (‡1199, ‡1200, ‡1201*)
  Dessa tekniker gör det lättare att upptäcka när en bit text, bild, video osv. har genererats eller ändrats av AI, och av vilket system. De underlättar bättre ekosystemmedvetenhet (‡1199, ‡1200, ‡1201*). Däremot kan vattenstämplar och metadata förfalskas eller tas bort genom vissa ändringar i innehållet (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Detektering av AI-genererat innehåll (‡1203, ‡1204, ‡1205*)
  Att förbättra användares förmåga att skilja mellan AI-genererat och äkta innehåll hjälper med digital forensik och medvetenhet om ekosystemet (‡1203, ‡1204). Däremot kan klassificerare vara opålitliga (‡1205*) och ha varierande prestanda mellan olika modaliteter.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 3.6: Tekniska skyddsåtgärder som diskuteras i detta avsnitt
>white|black||9|11|br En sammanfattning av de tekniska skyddsåtgärder som diskuteras i det här avsnittet, uppdelad i metoder för att utveckla säkrare modeller, övervakning och styrning vid driftsättning samt tekniker för att möjliggöra ekosystemövervakning.


###@ Att utveckla säkrare modeller

Ett första försvar mot skador från system för generellt ändamål inom AI är att göra den underliggande modellen säkrare. Detta avsnitt behandlar skyddsåtgärder som är ”inbakade i modellens parametrar” under modellutvecklingsprocessen (Figur 3.6).

>white|orangered|left|14|15.5|bb Att kurera träningsdata kan begränsa utvecklingen av potentiellt farliga förmågor

Allmänna AI-modeller för flera ändamål är användbara just eftersom de utvecklar ett brett spektrum av kunskaper och förmågor efter att ha bearbetat träningsdata, men vissa typer av träningsdata är oproportionerligt ansvariga för utvecklingen av potentiellt farliga förmågor. Till exempel kan en AI-modell som tränats på virologiska uppsatser vara bättre på att ge stöd i potentiellt skadliga biologiska uppgifter (‡549, ‡1206*) (se även §2.1.4. Biologiska och kemiska risker). Dessutom kan bild- och videogeneratorer som tränats på bilder av nakenhet hos människor också missbrukas för att skapa icke-konsensuella intima deepfakes (‡308, ‡319) (se även §2.1.1. AI-genererat innehåll och kriminell verksamhet).

Att filtrera träningsdata är en effektiv begränsning mot vissa oönskade förmågor (‡319, ‡1167, ‡1207, ‡1208). Det kan dock vara svårt att filtrera de stora datamängder som används för att träna generella AI-modeller (‡1168) på grund av höga kostnader (‡1209), filtreringsfel (‡1210) och negativa effekter på datamängdens kvalitet (‡1211). Dessa utmaningar förvärras av den flerspråkiga naturen hos internettext (‡1212), kulturella fördomar i innehållsmoderering (‡1211, ‡1213, ‡1214, ‡1215) och av att huruvida en viss datamängd är ’skadlig’ beror på kontextuella faktorer (‡1216). Trots detta visar filtrering av potentiellt skadligt material från träningsdata lovande resultat för att göra modeller mer tillförlitligt säkra, inklusive att göra öppet viktade modeller mer motståndskraftiga mot skadlig manipulation (‡55). Sambanden mellan innehållet i träningsdata och framväxande modellers förmågor är ännu inte fullt ut förstådda (‡1195), och filtrering verkar vara mer effektiv för att begränsa skadliga förmågor när den tillämpas på breda kunskapsområden (‡55) jämfört med smalare beteenden (‡1206, ‡1217). Se §3.4. Öppet viktade modeller för ytterligare diskussion.

![figure 3.6](images/fig3.6_safeguards.png)

##### Figur 3.6: Var tekniska skyddsåtgärder ska tillämpas
>white|black||9|11|br Tekniska skyddsåtgärder kan tillämpas i olika skeden av modellutveckling. Datakuration formar vad modeller lär sig under förträning och finjustering. Metoder baserade på träning, såsom förstärkningsinlärning från mänsklig återkoppling och robusthetsträning, justerar modellens beteende. Testmetoder, såsom adversariala attacker, identifierar kvarvarande sårbarheter. Vissa tekniker, såsom safe-by-design-algoritmer, omfattar flera skeden. Källa: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Metoder för att träna allmänna AI-modeller för att vara hjälpsamma och ofarliga förlitar sig främst på mänsklig feedback

Det är svårt att träna och utvärdera modeller för att tillförlitligt anpassa sig till övergripande principer som att vara hjälpsam, ofarlig och ärlig. I praktiken försöker utvecklare uppnå detta genom att finjustera AI-modeller med hjälp av demonstrationer och återkoppling från människor. Till exempel är den huvudsakliga paradigmen för finjustering av AI-modeller, känd som ”reinforcement learning from human feedback”, baserad på att träna modeller att ta fram utdata som mänskliga annotatörer betygsätter positivt (‡1218). Däremot är positiv återkoppling från människor en bristfällig proxy för gynnsamt beteende (‡737, ‡878, ‡1219, ‡1220) och begränsas av mänskliga fel och partiskhet (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Detta leder till flera utmaningar: modeller som finjusterats genom förstärkningsinlärning från mänsklig återkoppling kan ibland blidka användaren, ett beteende som kallas ’sykofanti’ (‡358, ‡740, ‡1226, ‡1227); tillhandahålla svar som är hjälpsamma i vissa sammanhang men skadliga i andra (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); tillhandahålla svar som är svåra att utvärdera för korrekthet (‡1233); eller utföra åtgärder vars hjälpsamhet eller skadlighet är en fråga om åsikt (‡1234). Tabell 3.7 ger exempel på dessa utmaningar. En del forskning syftar till att utveckla metoder för att hjälpa människor att bättre utvärdera lösningar på komplexa uppgifter med AI-assistans (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Dessa metoder har dock för närvarande begränsad tillförlitlighet, och i vilken utsträckning de används för att träna dagens mest avancerade AI-modeller är inte offentligt känt.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sycophancy/efterslängande (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Förklaring:
>white|black|left|11|13|br Modellen ger bara positiva omdömen och misslyckas med att påpeka avsaknaden av en korrekt 5-7-5 haiku-syltästruktur.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vissa åtgärder är hjälpsamma i vissa sammanhang men skadliga i andra (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Förklaring:
>white|black|left|11|13|br Information om biologisk risk kan användas för utbildning och försvar, men också för att informera illvilliga aktörer.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Korrekt beteende är svårt att verifiera (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Förklaring:
>white|black||11|13|br Det är svårt att bedöma riktigheten i detta svar eftersom det kräver medicinsk sakkunskap. Även för en erfaren läkare kräver utvärdering av svar av detta slag tid och noggrann uppmärksamhet på detaljer.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Människor är oense om vad som är korrekt (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Förklaring:
>white|black|left|11|13|br Människor är oense i betydande grad om vad som är det korrekta svaret.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 3.7: Användarens prompt och AI-modellens svar
>white|black||9|11|br Exempel på utmaningar med att specificera och belöna fördelaktiga åtgärder från AI-modeller.


>white|orangered|left|14|15.5|bb Människor är inte alltid överens om vilka beteenden som är önskvärda, vilket kräver metoder för att balansera konkurrerande preferenser.

Människor är inte alltid överens om vilka svar eller handlingar AI-modeller bör eller inte bör ge (‡1006). Detta gör det i grunden svårt att utveckla modeller vars handlingar och effekter i bred utsträckning är i linje med samhällets intressen (‡420). Vissa forskare studerar vems preferenser som återspeglas i AI-system (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) och arbetar för att utveckla tekniker för ”pluralistisk anpassning” som syftar till att skapa en balans mellan konkurrerande preferenser (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Till exempel kan AI-utvecklare utforma system för att undvika att generera kontroversiella svar genom att vägra att svara på vissa typer av förfrågningar, eller anpassa sig till den medelmässiga uppfattningen i ett visst relevant urval av människor, eller personalisera system för enskilda användare.

En vanlig utmaning för dessa metoder är att AI-system i allmänhet inte kan anpassas på ett likvärdigt sätt efter allas preferenser, och att deras efterföljande samhälleliga effekter kommer att påverka olika grupper av människor på olika sätt. Vissa forskare har hävdat att de flesta tekniska metoder för pluralistisk anpassning misslyckas med att ta itu med, och möjligen distraherar från, djupare utmaningar, såsom systematiska fördomar, sociala maktdynamiker samt koncentrationen av förmögenhet och inflytande (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb AI-utvecklare använder “adversarial training” för att förbättra modellens robusthet

Det är utmanande att säkerställa att AI-modeller robust översätter de gynnsamma beteenden de lär sig under träning till verkliga distributionssammanhang. Även modeller som tränas med en ”perfekt” inlärningssignal kan misslyckas med att generalisera framgångsrikt till alla oupptäckta sammanhang (‡738, ‡739, ‡1255, ‡1256, ‡1257). Till exempel har vissa forskare funnit att chattbotar oftare vidtar skadliga åtgärder på språk som är underrepresenterade i deras träningsdata (‡159, ‡880, ‡1258*, ‡1259), vilket inbegriper många språk som till övervägande del talas i den globala södern.

Under de senaste åren har forskare också tagit fram ett stort ramverk av tekniker för ”adversarial attack” som kan användas för att få modeller att generera potentiellt skadliga svar (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Till exempel samlade en nyare satsning in över 60,000 olika exempel på lyckade attacker mot AI-modeller i absolut toppskikt, vilket fick dem att bryta mot företagens policyer för acceptabel modellbeteende (‡1149). Tabell 3.8 visar exempel på ”jailbreak”-tekniker som forskare har visat kan göra att modeller följer skadliga förfrågningar.

En metod för att förbättra modellers robusthet kallas “adversarial training” (‡1064). Den innebär att man konstruerar “attacker” (t.ex. jailbreaks) som utformas för att få en modell att agera på ett oönskat sätt, och att man tränar modellen att hantera dessa attacker på ett lämpligt sätt. Däremot är adversarial training ofullkomlig (‡1260, ‡1261). Angripare kan konsekvent utveckla nya framgångsrika attacker mot state-of-the-art-modeller (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Eftersom utvecklare behöver specifika exempel på felmoder för att kunna träna mot dem (‡512, ‡1263), blir resultatet ett pågående “cat and mouse”-spel där utvecklare kontinuerligt uppdaterar modeller som svar på nyligen upptäckta sårbarheter, och angripare kontinuerligt söker nya attacker. Vissa forskare har föreslagit storskalig adversarial training (‡1264, ‡1265) eller nya algoritmer (‡675, ‡676, ‡1263, ‡1266, ‡1267) för att förbättra robusthet, men moderna AI-system förblir påtagligt sårbara.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Gör skadliga förfrågningar i chiffertext, såsom morsekod (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Förbered systemet med exempel på förenliga svar på skadliga förfrågningar (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Gör skadliga förfrågningar på lågresursspråk som sannolikt används mindre i träning (t.ex. swahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Dela upp en skadlig uppgift i flera oskyldiga deluppgifter (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabell 3.8: jailbreaking-strategier
>white|black||9|11|br Skadliga aktörer och red teams har använt olika typer av ”jailbreaks” för att få AI-modeller att följa skadliga förfrågningar som de normalt skulle vägra på grund av skyddsåtgärder. Exempelutdata skrevs av rapportens författare enbart för att illustrera. Många nuvarande state-of-the-art AI-modeller avvisar numera de flesta av dessa metoder, men nya jailbreak-tekniker fortsätter att upptäckas.


>white|orangered|left|14|15.5|bb ”Oinlärnings”-tekniker kan mildra specifika skadliga modellförmågor

En annan strategi för att mildra risker från generell-purpose AI är att finjustera modeller så att de saknar förmågor inom specifika domäner med hög risk (‡1175, ‡1176). Till exempel arbetar forskare med att ta fram algoritmer för ”maskinell bortglömningsprocess” som specifikt kan undertrycka förmågor som rör biologiska hot eller att generera fotorealistiska bilder av nakna mänskliga kroppar (‡903, ‡1272, ‡1273). Dessa metoder kan göra modeller avsevärt säkrare, men med kostnaden att begränsa vissa positiva användningar av de bortglömda förmågorna. Att begränsa AI-modellers kunskap inom skadliga domäner har också föreslagits som ett sätt att utforma ”manipuleringsresistenta” open-weight-modeller som kan motstå skadlig finjustering (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Hittills har dock detta varit utmanande att göra robust (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Se §3.4. Open-weight-modeller för vidare diskussion.

>white|orangered|left|14|15.5|bb Vissa forskare arbetar med metoder för starkare säkerhetsgarantier genom att tolka modellens interna tillstånd eller genom matematisk verifiering

Vissa forskare arbetar med metoder för att mer rigoröst verifiera säkerhetsrelaterade egenskaper hos modeller. I ett angreppssätt försöker forskare tolka modellernas interna beräkningar för att antingen identifiera risker eller för att skapa mer övertygande argument för att modellen är säker (‡1285, ‡1286). Till exempel visade forskare i en proof of concept att verktyg för att analysera en språkmodells interna beräkningar kan hjälpa utvärderare att identifiera skadliga beteenden (‡1287). År 2025 började även Anthropic analysera modellernas internals som ett sätt att studera modellernas situationsmedvetenhet och ‘intent’ (‡2). Emellertid är dessa typer av metoder för närvarande inte vanliga eller kända för att vara konkurrenskraftiga jämfört med andra utvärderingstekniker.

Ett annat angreppssätt för att ge starkare garantier för säkerhet innebär att konstruera matematiska bevis för att visa att en modell kommer att uppfylla vissa säkerhetsvillkor (‡1177, ‡1282, ‡1288). Dessa bevis förutsätter dock att testningskontexten överensstämmer med driftskontexten, och de har inte testats mot många typer av angripare.

De kan dessutom för närvarande inte skalas till storskaliga modeller. Sammantaget råder det en betydande debatt bland experter om löftet om tolkningsbarhet och formella verifieringsmetoder.

###@ Övervakning och styrning vid driftsättningstid

Utöver skyddsåtgärder som införts under modellutveckling finns en andra försvarslinje mot skadliga beteenden i form av externa skydd som fokuserar på övervakning och kontroll av en modells eller systems handlingar under driftsättning. Sådana skydd bidrar till att minska fel och felaktig användning, såsom hallucinerade utdata och skadliga instruktioner.

>white|orangered|left|14|15.5|bb Modellutplacerare kan använda en mängd olika verktyg för att identifiera och hantera högriskbeteenden hos modeller

När ett AI-system körs kan en operatör övervaka tecken på risk och ingripa om de uppstår. Till exempel kan de granska en modells indata för tecken på adversarial-attacker, filtrera olämpligt innehåll från utdata, eller övervaka systemets kedja av tankar för tecken på skadliga planer. Punkter där operatörer kan övervaka och ingripa i hur människor använder deras system inkluderar maskinvara (‡1180, ‡1181), användarinteraktioner (‡1154, ‡1166), indata och utdata (‡65, ‡725, ‡1182), interna beräkningar (‡744, ‡1183, ‡1184) och kedja av tankar (‡430, ‡435). Det finns också flera åtgärder som operatörer kan vidta när risker identifieras. Dessa inkluderar att logga information, filtrera/ändra skadligt innehåll, flagga avvikande aktivitet, systemavstängningar eller att trigga failsafes. Figur 3.7 visar exempel på vanliga övervaknings- och kontrollmekanismer.

Eftersom de är mångsidiga och ofta effektiva används dessa mekanismer i stor utsträckning och kan förebygga många typer av oavsiktliga skador (‡725, ‡751, ‡1289). Dessa skyddsåtgärder är dock ofullkomliga, särskilt under illvilliga attacker optimerade för att få dem att misslyckas (‡752, ‡1182). Ny forskning har också undersökt hur övervakning kan vara opålitlig om ett system optimeras med hjälp av en monitors poäng, till exempel genom att göra chain of thought mindre tillförlitlig (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Figur 3.7: Övervaknings- och styrtekniker
>white|black||9|11|br Övervaknings- och kontrolltekniker verkar vid flera punkter: granskning av indata och utdata för skadligt innehåll, spårning av interna modelltillstånd, begränsning av externa åtgärder genom sandboxning, samt upprätthållande av mänsklig tillsyn. Källa: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Människor i loopen möjliggör direkt övervakning i högriskmiljöer

För att minska risken för fel från AI-agenter (se §2.2.1 Tillförlitlighetsutmaningar) kan utövare sträva efter att utforma AI-system som fungerar i samarbete med människor snarare än att fungera helt autonomt (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Detta är viktigt för användningsfall där felaktiga beslut kan leda till betydande skada, såsom inom finans, sjukvård eller polisverksamhet. Däremot är det ofta opraktiskt att ha en “människa i slingan”. Ibland sker beslutsfattandet för snabbt, t.ex. i chattapplikationer med miljontals användare. I andra fall kan mänsklig partiskhet och fel förstärka riskerna på grund av kumulativa fel (‡1187). Människor i slingan tenderar också att uppvisa “automationsbias”, vilket innebär att de ofta lägger mer tillit till AI-systemet än vad som är berättigat (‡1190, ‡1191) (se §2.3.2 Risker för mänsklig autonomi).

>white|orangered|left|14|15.5|bb ”Sandboxing” skyddar mot risker från autonoma beteenden

AI-agenter som kan agera autonomt utan begränsningar på webben eller i den fysiska världen utgör förhöjda risker (se §2.2.1. Tillförlitlighetsutmaningar). ’Sandboxing’ innebär att begränsa på vilka sätt som AI-agenter kan påverka världen direkt, vilket gör det mycket enklare att övervaka och hantera dem (‡640, ‡1192, ‡1295). Till exempel kan det förebygga oönskade skador från oväntade handlingar genom att begränsa en AI-systems förmåga att publicera på internet eller att redigera en dators filsystem (‡1296). Dessa tillvägagångssätt kan dock inte alltid användas för tillämpningar där ett AI-system måste agera direkt i världen.

###@ Verktyg för ekosystemövervakning: modell- och dataproveniens

Verktyg för modell- och dataursprung är tekniska verktyg för att studera AI-ekosystemet, för att öka medvetenheten om hur AI-system används i efterföljande led och vilka effekter de har.

>white|orangered|left|14|15.5|bb AI-systemets ursprungsbaserade tekniker hjälper till att spåra användningar och effekter av system

Utvecklare och driftsättare kan använda olika tekniker för att studera modellanvändning och spridning ‘i det vilda’. Till exempel kan de ge modeller unika identifierande beteenden (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) eller tillämpa unika mönster på vikterna hos enskilda open-weight-modeller (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Att göra dessa tekniker mer motståndskraftiga mot modellmodifieringar är dock ett öppet problem (‡1195, ‡1196*). Forskare arbetar också med metoder för att ‘inferera modellens ursprung’ (‡1197, ‡1198, ‡1305, ‡1306), vilket hjälper till att besvara frågor av typen: ‘Var modell X en fine-tuned- eller distillerad version av modell Y?’ Slutligen arbetar vissa utvecklare mot protokoll och infrastruktur för AI-agenter för att underlätta identifiering och verifiering när de interagerar med externa system (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Figur 3.8: Vattenstämplar bäddar in oansenliga störningar i bilder och ljud
>white|black||9|11|br Vattenstämplar bäddar in omärkliga störningar i bilder och ljud som gör det möjligt för detektionsverktyg att identifiera AI-genererat innehåll. I denna figur är både bild- och ljudvattenstämplarna överdrivna för synlighet. Källa: Chameleon-bild från Unsplash (‡1313*). Övriga element skapade av Report-författarna. International AI Safety Report 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Figur 3.9: Framgångsgraden för prompt injection-attacker
>white|black||9|11|br Framgångsgrader för promptinjektionsattacker, så som de rapporterats av AI-utvecklare för större modeller som släpptes mellan maj 2024 och augusti 2025. Varje punkt representerar andelen lyckade attacker inom 10 försök mot en given modell strax efter lansering. Den rapporterade framgångsgraden för sådana attacker har sjunkit över tid, men är fortfarande relativt hög. Källa: Zou et al. 2025 (‡1149), citerad i Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb AI-innehållsdetekteringstekniker hjälper till att övervaka spridningen och effekterna av AI-genererat innehåll

Vattenstämplar, metadata och andra AI-innehållsdetektorer kan hjälpa forskare att spåra och studera den verkliga påverkan av AI-skapat innehåll. 

Först är data-watermärken subtila men distinkta mönster som infogas i digitala medier och som kan koda information om deras ursprung (‡1199, ‡1200, ‡1201*). För text tar de vanligtvis formen av subtila fördomar i ordval och stil (‡1308, ‡1309); för bilder och video är det subtila mönster över pixlar (‡1310); och för ljud är det subtila mönster i ljudvågor (‡1311). Figur 3.8 illustrerar dessa.

Förutom vattenstämplar kan AI-genererat innehåll också sparas med filformat som lagrar metadata om hur de genererades. Till exempel sparar många mobila enheter bild- och ljudfiler med ett filformat som kan lagra information om kamerainställningar, tid, plats osv. (‡1312). Liknande metadata kan användas för att lagra information om huruvida data genererades av ett AI-system. Ungefär som fingeravtryck i brottsutredningar kan vattenstämplar och metadata manipuleras eller avlägsnas, men de är likväl användbara.

Forskare arbetar också med att utveckla detektorer för AI-genererat innehåll (‡1203, ‡1204, ‡1205*) för att hjälpa till att identifiera AI-genererat innehåll i praktiken, även när ingen vattenstämpel eller metadata finns tillgänglig. Dessa identifieringstekniker har dock en begränsad framgångsgrad.

###@ Uppdateringar

Sedan den senaste rapporten publicerades (januari 2025) har framsteg gjorts när det gäller att utveckla AI-system med flera effektiva lager av skyddsåtgärder. Som diskuteras i §3.2. Riskhanteringspraxis är defence-in-depth en central princip inom riskhantering (‡1314). Till exempel studeras och används AI-system som kombinerar säkerhetstränade modeller med inmatningsfilter, utmatningsfilter och andra innehållsövervakare i allt högre grad (‡32, ‡65, ‡1182*). Ny forskning har också visat att, även om modellutvecklare har gjort framsteg med att öka robustheten mot försök att kringgå skydd, lyckas angripare fortfarande i hög takt (Figur 3.9).

###@ Evidensluckor

Mer bevisunderlag behövs för att hjälpa forskare att förstå och beakta begränsningarna i befintliga metoder. Tekniska skyddsåtgärder för AI-system förbättras, men teknikerna lider av begränsningar. Till exempel har framstegen med att förbättra generalistiska AI-systems robusthet i värsta fall gått långsamt, och det finns grundläggande begränsningar för hur grundligt open-weight-modeller kan skyddas och övervakas (‡1195, ‡1315, ‡1316) (se även §3.4. Open-weight models). Under tiden är inte alla tekniska skyddsåtgärder lika vanliga, lika effektiva eller lika väl belagda i den verkliga världen. Till exempel används adversarial training nästan överallt i state-of-the-art-modeller (‡64*, ‡677), medan modelltolknings- och formell verifieringsteknik har använts i liten utsträckning i produktionstillämpningar hittills (‡1177, ‡1285).

###@ Utmaningar för beslutsfattare

Centrala utmaningar för beslutsfattare innefattar att avgöra om och hur de bör stödja forskning, utveckling, utvärdering och införande av tekniska skyddsåtgärder och övervakningsmetoder. Detta är utmanande eftersom forskarnas förståelse av hur man bäst praktiskt kan skydda mekanismer fortfarande utvecklas och bästa praxis ännu inte är etablerad. Till exempel tillämpar olika utvecklare olika skyddsåtgärder, och deras tillvägagångssätt för teknisk riskreducering i stort sett varierar också avsevärt (‡1116). Slutligen innebär förekomsten av effektiva tekniska skyddsåtgärder inte i sig att säkerhet uppnås, eftersom införande och implementering kan variera mellan utvecklare och mellan olika driftsättningskontexter.

