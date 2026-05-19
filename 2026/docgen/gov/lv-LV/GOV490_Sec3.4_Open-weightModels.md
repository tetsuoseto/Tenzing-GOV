##########
>white|orangered|left|14|30|hr 3.4. sadaļa
### 3.4. Atvērtā svaru modeļi
>white|orangered|left|24|30|hb Atvērtā pirmkoda modeļi

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Svarīga informācija
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Piekļuve, ko AI uzņēmumi nodrošina savu modeļu “svariem”, ietekmē riskus, ko šie modeļi rada. Svari ir matemātiskie parametri, kas ļauj AI modeļiem apstrādāt ievades un ģenerēt izvades. Jebkuram konkrētam modelim uzņēmumi var izvēlēties sargāt svarus pilnībā privāti, sniegt dažiem lietotājiem zināmu ierobežotu piekļuvi vai ļaut ikvienam tos lejupielādēt pilnā apjomā. Modeļus, kuru svari ir publiski pieejami, sauc par “open-weight modeļiem” (open-weight models).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Atvērtā pirmkoda modeļi veicina pētniecību un inovācijas, taču to aizsardzības līdzekļus ir vieglāk noņemt. Visā pasaulē dažādi dalībnieki – īpaši tie, kuriem ir mazāki resursi – var izmantot atvērtā pirmkoda modeļus pētniecības un komerciāliem nolūkiem. Tomēr, salīdzinot ar slēgtā pirmkoda modeļiem, atvērtā pirmkoda modeļus ir vieglāk pielāgot, lai tie izrādītu iespējami kaitējošu uzvedību, un tas ir grūtāk.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Atvērtā koda modeļa (open-weight) izlaidumi ir neatgriezeniski. Kad tie ir izlaisti, modeļa svari (model weights) vairs nevar tikt atsaukti. Tas apgrūtina iespējamo kaitējumu mazināšanu, kas var rasties, izlaižot modeli ar bīstamām spējām.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kopš pēdējā ziņojuma publicēšanas (2025. gada janvāris) lielākie atvērtā svaru apjoma laidieni ir samazinājuši iespēju plaisu ar vadošajiem slēgtajiem modeļiem. Ķīniešu izstrādātāji DeepSeek un Alibaba izlaida attiecīgi savus R1 un Qwen modeļus, kuri sasniedza vadošajiem slēgtajiem modeļiem salīdzināmu sniegumu, savukārt OpenAI izlaida savus pirmos atvērtā svaru apjoma modeļus kopš 2019. gada. Vadošo slēgto modeļu iespējas pašlaik tiek lēstas kā mazāk nekā gada attālumā no vadošajiem atvērtā svaru apjoma modeļiem nozīmīgos AI etalonuzdevumos.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Galvenais politikas īstenošanas izaicinājums ir piekļuve atvērtā svara (open-weight) modeļu sniegtajām priekšrocībām, vienlaikus pārvaldot to īpatnējos riskus. Viens pieejamais risinājums ir vērtēt atvērtā svara modeļus, ņemot vērā to “marginālo risku”: pakāpi, kādā to izlaide kontrfaktiski palielina sabiedrisko risku salīdzinājumā ar risku, ko jau rada esošie modeļi vai citas tehnoloģijas. Tomēr praksē to ir sarežģīti īstenot. Nelieli marginālā riska pieaugumi laika gaitā var arī summēties līdz būtiskam kopējā riska pieaugumam.
>oldlace|black||11|15|br      


Atvērtās piekļuves modeļiem ar parametriem, kas ir publiski pieejami lejupielādei, ir atšķirīgas sekas daudzām problēmām, kas aplūkotas iepriekšējās sadaļās. Mākslīgā intelekta modeļa “svari” satur būtisko informāciju, kas ļauj tam ģenerēt lietderīgas atbildes lietotājiem. Kad šie svari ir izlaisti, tos vairs nevar atsaukt: ikviens var lejupielādēt, pētīt, modificēt, kopīgot un izmantot tos savos datoros vai mākoņkontos. Ja svari ir atklāti pieejami, citi tos var vieglāk balstīt un modificēt, lai apmierinātu dažādas vajadzības un veicinātu inovācijas (‡1317). Tomēr ar to pašu mehānismu ļaunprātīgiem lietotājiem ir arī vieglāk noņemt drošības ierobežojumus un modificēt atvērtās piekļuves modeļus kaitīgiem izmantošanas gadījumiem (‡1122, ‡1160). Tas ir aktualizējis jautājumu, vai daži atvērtās piekļuves modeļi būtu jāpakļauj īpašām prasībām (piem., stingrākai testēšanai pirms izlaišanas) vai, pretēji, jāpiešķir īpaši atbrīvojumi (piem., no normatīvo atskaišu prasībām) (‡1033).

###@ Pamatojums atvērtā svara modeļiem

>white|orangered||14|15.5|bb Atvērtā svaru modeļi var būt, bet ne vienmēr ir, “atvērtā pirmkoda” modeļi

Lai gan tos bieži dēvē par “atvērto pirmkodu”, lielākā daļa publiski izlaisto modeļu precīzāk ir raksturojami kā “atvērtie svari”. Tas ir tādēļ, ka, lai gan izstrādātāji nodrošina modeļa svarus, tie neizlaiž saistīto apmācības kodu vai datu kopas. Turklāt atvērtā pirmkoda programmatūru parasti raksturo licences, kas nosaka minimālas prasības tālākajiem dalībniekiem, kuri izmanto vai modificē programmatūru (‡1318). Piemēram, Meta Llama modeļiem ir ierobežojoši licences nosacījumi, un tie ietver tikai secināšanas kodu, nevis apmācības kodu, tāpēc tos parasti neuzskata par atvērtā pirmkoda programmatūru (‡1319, ‡1320). Modeļu izlaišanas iespējas pastāv spektrā no pilnībā slēgtas līdz pilnībā atvērtai pirmkoda programmatūrai, un katrā punktā ir atšķirīgas riska–ieguvuma kompromisa attiecības (‡1086*, ‡1320, ‡1321). Tabula 3.9 apraksta šīs iespējas.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Pilnībā noslēgts
  Lietotāji nevar tieši mijiedarboties ar modeli vispār
  Piemēri: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Piekļuve, izmantojot mitināšanu
  Lietotāji var mijiedarboties tikai caur konkrētu lietojumprogrammu vai saskarni, piemēram, mobilās tērzēšanas robota lietojumprogrammu
  Piemēri: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb Piekļuve API modelim
  Lietotāji var sūtīt pieprasījumus uz modeli ar koda palīdzību, tādējādi nodrošinot izmantošanu ārējās lietojumprogrammās
  Piemēri: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb API piekļuve pielāgošanai (fine-tuning)
  Lietotāji var smalki pielāgot modeli savām konkrētajām vajadzībām
  Piemēri: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Atvērtā svaru piekļuve: svari, kas pieejami lejupielādei
  Lietotāji var lejupielādēt un palaist modeli savos datoros
  Piemēri: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Svari, dati un kods pieejami lejupielādei ar izmantošanas ierobežojumiem
  Lietotāji var lejupielādēt un palaist modeli, kā arī secināšanas un apmācības kodu, taču to izmantošanai ir noteikti licences ierobežojumi
  Piemēri: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pilnībā atvērts: svari, dati un kods pieejami lejupielādei bez izmantošanas ierobežojumiem
  Lietotājiem ir pilnīga brīvība lejupielādēt, izmantot un modificēt modeli, pilno kodu un datus
  Piemēri: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.9. tabula: Modeļa koplietošanas iespējas, kas variē no pilnībā slēgtām līdz pilnībā atvērtām
>white|black||9|11|br Ilustratīva modeļu koplietošanas iespēju izvēle, sākot no pilnībā slēgtiem modeļiem (modeļi ir privāti un tiek turēti tikai patentētiem mērķiem) līdz pilnībā atvērtiem un atvērtā pirmkoda modeļiem (modeļa svari, dati un kods ir brīvi un publiski pieejami bez lietošanas, modificēšanas un koplietošanas ierobežojumiem). Modeļi, kas ietilpst pirmajās četrās kategorijās, bieži tiek dēvēti par “slēgtiem”. Šajā sadaļā uzmanība pievērsta trim apakšējām rindām. Avots: pielāgots no Bommasani, 2024 (‡1317).


###@ Ieguvumi un riski

>white|orangered|left|14|15.5|bb Atvērtā pirmkoda modeļus var vieglāk pielāgot un izvērtēt

Atvērtā koda (open-weight) modeļi sniedz nozīmīgas priekšrocības pētniecībai, inovācijai un piekļuvei. Kā apspriests §1.1. Kas ir vispārīgas nozīmes AI?, vispārīgas nozīmes AI modeļu apmācība ir ārkārtīgi dārga – vadošie modeļi izstrādei maksā simtiem miljonu dolāru. Atklāta modeļu svaru (weights) izpaušana ļauj mazāk ar resursiem nodrošinātajiem dalībniekiem replicēt, pētīt un būvēt uz esošajām sistēmām. Bez šādas piekļuves kopienas reģionos ar zemiem resursiem riskē tikt izslēgtas no AI sniegtajām priekšrocībām, tādēļ atvērtie svari ir kritiski svarīgi globālas vairākuma līdzdalības nodrošināšanai AI izstrādē (‡1322). Pakārtotie izstrādātāji var pielāgot modeļus (fine-tune) dažādiem lietojuma scenārijiem, piemēram, pielāgojot tos nepietiekami nodrošinātām mazākumtautību valodām vai optimizējot veiktspēju konkrētiem uzdevumiem, piemēram, juridisku dokumentu sagatavošanai vai medicīnisku piezīmju pierakstīšanai (‡1323, ‡1324*). Tādējādi atvērtā svara (open-weight) modeļi var ļaut vairāk cilvēkiem un kopienām izmantot AI un gūt no tā labumu, nekā tas būtu iespējams citādi (‡1325). Attiecībā uz modeļiem, kas nav pietiekami spējīgi, lai radītu bīstamību, šīs priekšrocības var pārsvērt papildu risku, atklāti izpaužot svarus, lai gan tas ir atkarīgs no attiecīgo lēmumu pieņēmēju riska tolerances.

Atvērtā svaru izlaišana arī paplašina izstrādātāju un pētnieku loku, kas spēj pētīt modeli, novērtēt tā iespējas, pārbaudīt ievainojamības un iterēt uz uzlabojumiem (‡1326, ‡1327). Tas palielina varbūtību, ka tiek identificētas gan noderīgas lietojumprogrammas, gan kaitīgas nepilnības, kaut arī tas netiek garantēts (‡1328, ‡1329). Lietotāji var arī palaist atvērtā svara modeļus savās ierīcēs, ļaujot tiem saglabāt kontroli pār sensitīviem datiem un izvairīties no to nosūtīšanas trešo pušu serveriem.

Ir papildu priekšrocības, ja izstrādātāji dalās ar tādu informāciju kā apmācības dati, kods, novērtēšanas rīki un dokumentācija, kā arī modeļu svari (‡1320, ‡1330, ‡1331, ‡1332*). Ar vairāk informācijas lejupstream izstrādātāji un citi pētnieki var labāk izprast atvērtā svara modeļus un pielāgot tos jaunām lietojumprogrammām.

>white|orangered|left|14|15.5|bb Atvērtā svara modeļu drošības pasākumus ir vieglāk noņemt, tādējādi ļaujot iespējamai ļaunprātīgai izmantošanai

Atvērtās svēruma (open-weight) modeļi rada arī papildu riskus, jo to aizsardzības mehānismus ir vieglāk noņemt. Lai gan gan atvērtie svēruma, gan slēgtie modeļi var būt aprīkoti ar aizsardzībām, lai atteiktu kaitīgas lietotāju pieprasījumus, atvērtajiem svēruma modeļiem šie aizsardzības mehānismi ir daudz vieglāk noņemami. Ļaunprātīgiem dalībniekiem ir iespējams pielāgot (fine-tune) modeli, lai optimizētu tā veiktspēju kaitīgām lietojumprogrammām, noņemt koda daļas, kas paredzētas kaitīgas izmantošanas novēršanai, vai atsaukt iepriekšējo drošības pielāgošanu (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Tā rezultātā atvērtā modeļa svēruma var pastiprināt nepareizas izmantošanas riskus, kas apspriesti §2.1. Riska palielināšanās ļaunprātīgas izmantošanas gadījumā izriet no tā, ka tiek iesaistīts lielāks dalībnieku skaits, lai, bez uzraudzības, izmantotu un papildinātu esošās iespējas ļaunprātīgiem mērķiem (‡1122, ‡1315). Lai gan daudzi lietotāji nespēs vai arī nebūs motivēti noņemt aizsardzības mehānismus atvērtā svēruma modeļos, augsti motivēti ļaunprātīgi dalībnieki ir būtams apsvērums. Turklāt ļaunprātīgie dalībnieki var arī spēt izmantot atvērtā svēruma modeļus, lai identificētu ievainojamības līdzīgos slēgtajos modeļos (‡1055*). Šādus trūkumus ir grūtāk atrast, balstoties tikai uz slēgtajiem modeļiem, jo slēto modeļu nodrošinātāji spēj īstenot lielāku kontroli un uzraudzības pasākumus.

>white|orangered|left|14|15.5|bb Modeļa svaru koplietošana ir neatgriezeniska

Kad modeļa svari būs pieejami publiskai lejupielādei, nav iespējams veikt pilnīgu visu esošo kopiju atcelšanu (wholesale rollback). Interneta mitināšanas platformas, piemēram, GitHub un Hugging Face, var noņemt modeļus no savām platformām, tādējādi dažiem aktoriem ir grūtāk atrast lejupielādējamas kopijas un tas rada būtisku šķērsli daudziem nejaušiem ļaunprātīgiem lietotājiem (‡1339). Tomēr motivēti aktori joprojām var iegūt kopijas, ja modelis ir lejupielādēts un pārsūtīts (rehosted) citur vai arī saglabāts lokāli. Turklāt lejupielādes (downstream) izstrādātāji, kuri savās sistēmās integrē open-weight modeļus, arī pārņem jebkādas nepilnības, piemēram, ievainojamības pret pretinieku (adversarial) uzbrukumiem (‡1055) vai modeļa spēju apiet uzraudzības sistēmas (skat. §2.2.2. Kontroles zudums) (‡1315). Atšķirībā no slēgtiem modeļiem, kur mitinātāji var vienveidīgi izplatīt labojumus, open-weight modeļu izstrādātāji nevar garantēt, ka atjauninājumi tiks pieņemti lietotāju vidū.

###@ Atjauninājumi

Kopš pēdējā ziņojuma publicēšanas (2025. gada janvāris) spējām atpalicības plaisa starp vadošajiem atvērtā svara modeļiem un slēgtajiem modeļiem ir samazinājusies. Ķīniešu izstrādātāji ir kļuvuši par īpaši nozīmīgiem atvērtā svara modeļu nodrošinātājiem. 2025. gada janvārī DeepSeek izlaida savu R1 modeli, kas uzrādīja sniegumu, kas vairākos testos bija salīdzināms ar OpenAI o1 (‡1340). Alibaba Qwen modeļi ir līdzīgi ieguvuši ievērību, ieņemot vadošo vietu atvērtā svara modelim Chatbot Arena, plaši izmantotā veiktspējas etalona ietvaros, līdz 2025. gada augustam (‡1341, ‡1342*). 2025. gada augustā OpenAI izlaida savus pirmos atvērtā svara modeļus kopš GPT-2 izdošanas 2019. gadā — gpt-oss-120b un gpt-oss-20b. Meta turpināja izlaist Llama modeļus ar atvērtiem svariem. Vadošo slēgto modeļu spējas tagad tiek lēstas kā mazāk nekā gadu priekšā vadošajiem atvērtā modeļiem nozīmīgos AI etalonos (Figūra 3.10).

###@ Pierādījumu trūkumi

Galvenais pierādījumu trūkums attiecas uz reālās pasaules efektivitāti, lai tehniskie risinājumi novērstu atvērtā svaru modeļu (open-weight models) ļaunprātīgu izmantošanu. Pētnieki ir ierosinājuši dažādas pieejas, lai padarītu modeļus izturīgus pret iejaukšanos. Tas ietver jaunas apmācības metodes, kas izstrādātas, lai padarītu modeļus noturīgus pret kaitīgu modifikāciju (‡1276), kaitīga satura filtrēšanu no apmācības datiem (‡55) un aizsardzību pret jailbreaks (‡675, ‡676). Šīs metodes tagad tiek ieviestas reālās pasaules izlaidumos no lielākajiem izstrādātājiem. Piemēram, OpenAI izmantoja dažas no šīm metodēm savos gpt-oss modeļos, ziņojot, ka pretinieciski (adversarially) smalki noregulētās versijas nesasniedza augstus spēju sliekšņus (‡1344*). Tomēr pētījumi ir parādījuši, ka ļaunprātīgi aktori var atslēgt aizsardzības līdzekļus, pārapmācot modeļus uz kaitīgiem piemēriem (‡1345, ‡1346). Turklāt joprojām ir grūti uzticami novērtēt aizsardzības līdzekļu noturīgumu, tādējādi to efektivitāte pret uzbrukumiem reālajā pasaulē ir neskaidra (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Figūra 3.10: Iespēju atšķirība starp vadošajiem atvērtā svara un slēgtā modeļiem AI
>white|black||9|11|br Epoch Capabilities Index (ECI) rezultāti vislabākajiem atvērtā svara (tumši zilajiem) un slēgtajiem (gaiši zilajiem) modeļiem laika gaitā. ECI apvieno punktu skaitu no 39 etaloniem vienā vispārējās spēju skalā. Labākie atvērtā svara modeļi atpaliek aptuveni par vienu gadu no slēgtajiem modeļiem. Avots: Epoch AI, 2025 (‡1343).


###@ Mitigācijas

Tehniskie mazināšanas pasākumi atvērtā svara modeļu riskiem darbojas visā AI izstrādes un izvietošanas procesā (‡1141, ‡1195, ‡1347). Piemēram, izstrādājot modeļus, izstrādātāji un pakārtotie adapteri var filtrēt sensitīvu saturu no apmācības datiem, lai mazinātu kaitīgas iespējas. Kaitīgo piemēru noņemšana modeļa apmācības datos var novērst pretinieku pielāgošanu (adversarial fine-tuning) 10 reizes efektīvāk nekā aizsardzību pievienošana pēc apmācības, lai gan tas var ietekmēt arī noderīgas iespējas (‡55). AI lietojumprogrammu nodrošinātāji var arī ieviest incidentu paziņošanas un reaģēšanas mehānismus (‡1348).

Turklāt tādas mitināšanas platformas kā HuggingFace un GitHub var noteikt platformas lietošanas noteikumus, lai izņemtu modeļus, kas ir modificēti kaitnieciskos nolūkos (‡1141, ‡1324). Modeļu izstrādātāji var nodrošināt pilnu piekļuvi revidentiem pirms izlaišanas vai izvēlēties “pakāpenas” izlaišanas stratēģiju – izlaist modeļus pakāpeniski lielākām lietotāju grupām (‡1086). Tas var palīdzēt identificēt iespējamas darbības kļūmes vai ievainojamības pirms modeļa plašas pieejamības (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Piezīme 3.1: Modeļa svaru drošība
>oldlace|black|left|13|15|hb  Piezīme 3.1: Modeļa svaru drošība
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Šajā sadaļā apspriestie riski pieņem, ka modeļa svari tiek izlaisti apzināti. Tomēr slēgtie modeļa svari var kļūt pieejami arī zādzības vai noplūdes rezultātā. Slēgtie modeļi maksā simtiem miljonu dolāru, lai tos izstrādātu (§1.1. Kas ir vispārējas nozīmes AI?), un vidēji ir spējīgāki nekā atvērtā svara modeļi (‡1343). Tas padara tos par pievilcīgiem mērķiem aktoriem, sākot no amatieru hakeriem līdz valstu aģentiem, kuri vēlas iegūt vadošus AI modeļus.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Nzagāti noslēgtu modeļu svaru zādzība radītu riskus, kas būtu līdzīgi iepriekš aprakstītajiem atvērto modeļu gadījumā, bet, iespējams, bez jebkādām šādu risku mazināšanas iespējām. Ļaunprātīgi rīkotāji varētu noņemt drošības pasākumus no visspējīgākajiem modeļiem. Atšķirībā no leģitīmiem izstrādātājiem šādi rīkotāji nesaskartos ar reputācijas, juridiskiem vai komerciāliem ierobežojumiem, kas pašlaik mudina “frontier AI” uzņēmumus izvietot savus modeļus droši.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Pašreizējie drošības līmeņi dažādās nozarēs atšķiras, un tie var nebūt pietiekami pret izsmalcinātiem uzbrucējiem. Daži izstrādātāji apņemas nodrošināt modeļa svaru (model weights) aizsardzību pret kibernoziedzības sindikātiem un iekšējiem draudiem (‡582), savukārt citi nav izteikuši nekādas publiskas drošības apņemšanās (‡1109, ‡1349). Pētījumi liecina, ka AI datu centri var nespēt pretoties uzbrukumiem no visizsmalcinātākajiem un vislabāk resursētajiem dalībniekiem (‡582, ‡1350, ‡1351). Līdz 2025. gada decembrim nav apstiprinātu, publiski dokumentētu gadījumu, kuros notiktu modeļa svaru zādzība. Tomēr ir ziņots par citām drošības pārkāpuma epizodēm vadošajos AI uzņēmumos, tostarp Microsoft e-pasta sistēmu ielaušanos (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Šo drošības nepilnību novēršanai būtu nepieciešami ievērojami ieguldījumi aparatūrā, programmatūrā, personālā un objektu drošībā. Dažus drošības uzlabojumus varētu īstenot salīdzinoši ātri ar koordinētu rīcību (‡1122). Tomēr citi kritiski pasākumi, piemēram, aparatūras piegādes ķēžu un objektu nodrošināšana, visticamāk prasītu gadus (‡1122). Privātie uzņēmumi var arī trūkt resursu vai informācijas, lai vieni paši izstrādātu atbilstošas aizsardzības. Piemēram, AI izstrādātājiem nav piekļuves klasificētai apdraudējumu izlūkošanai, kāda ir valdībām (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Izaicinājumi politikas veidotājiem

Viena no galvenajām problēmām politikas veidotājiem ir nodrošināt atvērtā svaru modeļu koplietošanas sniegto ieguvumu izmantošanu, būtiski nepalielinot risku. Lai izvairītos no katastrofāla kaitējuma, atvērtā svaru modeļu izstrādātāji nedrīkst izlaist modeļus, iepriekš neizvērtējot riskus, gan izmantojot izveidotas novērtēšanas metodes, kas paredzētas slēgtiem modeļiem, gan arī veicot papildu testēšanu, ņemot vērā, ka ļaunprātīgi aktori var smalki noregulēt modeļus un atņemt tiem drošības aizsardzības mehānismus. Reālajā praksē tas var būt grūti, jo spēju attīstība var būt neparedzama, atvērtā svaru modeļu izlaidumi ir neatgriezeniski, un ir nepieciešami novērtēšanas centieni, lai prognozētu, kad izlaidums varētu radīt būtisku iespējamo kaitējumu. Viena pieeja ir izvērtēt atvērtu izlaidumu “robežrisku”: pakāpi, kādā izlaidums kontrfaktiski palielina sabiedrisko risku salīdzinājumā ar risku, ko jau rada esošie modeļi vai citas tehnoloģijas (‡556, ‡1033, ‡1354, ‡1355) (skat. §3.2. Riska pārvaldības prakses). Tomēr ir sarežģīti aplēst, kā sistēma pēc tās ieviešanas palielinās vai samazinās pakārtoto (downstream) risku, un tas ir atkarīgs no konteksta. Pakāpeniski pieaugošs risks ar secīgiem izlaidumiem var laika gaitā sakumulēties līdz ievērojamam kopējā riska pieaugumam, pat ja katra atsevišķā izlaiduma robežrisks šķiet pieņemams (‡1356, ‡1357). AI spēju divējādais (dual-use) raksturs vēl vairāk sarežģī pārvaldību: iezīmes, kas ļauj veidot labvēlīgus lietojumus medicīnā vai pētniecībā, var tikt pārveidotas ļaunprātīgiem mērķiem, un, tiklīdz svari ir publiski pieejami, atšķirt leģitīmu no ļaunprātīgas izmantošanas var būt grūti. Tāpat nav skaidrs, kam būtu jāuzņemas atbildība, ja atvērtā svaru modeļi tiek modificēti kaitnieciskiem nolūkiem.

