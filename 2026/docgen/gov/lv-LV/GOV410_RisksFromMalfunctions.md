Vispārējas nozīmes AI sistēmas neizdodas veidos, kas jau ir nodarījuši reālu kaitējumu, sākot no izdomātām juridiskām norādēm līdz medicīniskām nepareizām diagnozēm. Lai gan arī cilvēku profesionāļi pieļauj kļūdas, AI atteices rada atšķirīgas bažas to novitātes dēļ, iespējamās mērogojamības dēļ, grūtību dēļ prognozēt, kad tās notiks, un lietotāju tendences uzticēties bez kritiskas izvērtēšanas pārliecinoši skanošām izvaddēm. Pašreizējās vispārējas nozīmes AI atteices ietver nepatiesas informācijas sniegšanu (‡602, ‡603), pamata loģikas kļūdas (‡604, ‡605) un pasliktināšanos, ja tās izvieto jaunā kontekstā (‡606, ‡607, ‡608). Fiksētais šādu atteišu radītais kaitējums ietver medicīniskas nepareizas diagnozes, kļūdas juridiskos procesuālajos dokumentos un finansiālus zaudējumus (‡609, ‡610, ‡611). Uzticamības problēmas ir īpaši kritiskas AI aģentiem, jo atteices var tieši radīt kaitējumu bez cilvēka rīcības vai uzraudzības (‡612, ‡613, ‡614, ‡615). Daudz-aģentu sistēmas ievieš papildu atteices režīmus kļūdainas koordinācijas, konfliktu vai nevēlamas savstarpējas vienošanās (kollūzijas) starp aģentiem dēļ (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Halucinācija
- Nerakstīta precedenta citēšana juridiskajos dokumentos (‡617)
- Nekādu samazinātas maksas politiku neesošas norādīšana apgādnieka zaudējušiem pasažieriem (‡618)
- Nenosniegta un aizspriedumaina medicīniskā informācija (‡619)
- Nesniegta informācija par notikumiem, kas ir novecojusi (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pamata pamatojuma kļūme
- Neizdodas veikt matemātiskos aprēķinus (‡621)
- Neizdodas izsecināt pamata cēloņsakarības (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ārpus izplatījuma kļūme (kļūme neierastos vai neparastos ievades datos)
- Attēlu nepareiza klasificēšana, ja mainās fona apgaismojums vai konteksts (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rīka izmantošanas kļūme
- Privātuma pārkāpums, izpaužot lietotāja privātu attēlu, izmantojot AI aģentu, kas to nosūta trešās puses rīkam (‡624)
- Īstermiņa darba atmiņas darbības traucējumi (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Daudzveidu aģentu sistēmas atteice: nesaskaņota koordinācija un konflikts
- Nespēja pārvaldīt koplietojamos resursus individuālu stimulu un kolektīvās labklājības mērķu (‡627) sadursmes dēļ
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 2.4. Tabula: Uzticamības problēmu piemēri vispārējas nozīmes AI un aģentu sistēmās
>white|black||9|11|br Dokumentētas uzticamības problēmas vispārējas nozīmes AI sistēmās, AI aģentos un daudztaģentu sistēmās.


###@ Vispārīgas nozīmes AI sistēmas saskaras ar dažādiem uzticamības izaicinājumiem

2.4. tabula apkopo biežākās uzticamības problēmu kategorijas. Pirmās trīs attiecas uz visām AI sistēmām, bet pēdējās divas īpaši attiecas uz AI aģentiem un daudzaģentu sistēmām. Daudzi uzticamības riski rodas no grūtībām paredzēt un uzraudzīt AI sistēmas uzvedību.

Šie izaicinājumi (tālāk apskatīti §3.1. Tehniskie un institucionālie izaicinājumi) īpaši spēcīgi izpaužas AI aģentiem, kas darbojas sarežģītās vidēs. Pašreizējās metodes kļūmju novērtēšanai un to mazināšanai var samazināt kļūmju biežumu, taču pat vadošie AI aģenti joprojām ir pietiekami neuzticami, lai radītu riskus un kavētu ieviešanu daudzos kontekstos.

‘Uzticamība’ attiecas uz to, cik lielā mērā AI sistēma darbojas tā, kā to ir paredzējis izstrādātājs vai lietotājs. Vispārējas nozīmes AI sistēmas saskaras ar dažādām uzticamības problēmām — no neprecīzas vai maldinošas satura ģenerēšanas līdz kļūmēm pamata spriešanā. Piemēram, lai gan modeļi ir uzlabojušies faktu informācijas atcerēšanā, pat vadošie modeļi joprojām ievērojamā biežumā sniedz pārliecinošas, bet nepareizas atbildes (2.10. attēls). Programmatūras inženierijā vispārējas nozīmes AI tagad var sniegt būtisku palīdzību datorkoda rakstīšanā, izvērtēšanā un kļūdu diagnosticēšanā (‡215*, ‡628, ‡629). Tomēr ar AI ģenerēts kods bieži satur kļūdas (‡630), turpretim kodēšanas aģenti regulāri pieļauj kļūdas (‡631). Šādas neveiksmes var ieviest programmu un drošības sistēmu ievainojamības (skat. §2.1.3. Kiberdraudi).

Uzticamības problēmas ir īpaši svarīgi uzraudzīt augsta riska vidēs, piemēram, medicīnā, ņemot vērā AI strauji pieaugošo izmantošanu un iespējamību, ka kļūmes var novest pie smaga kaitējuma (‡609, ‡619). Attiecīgās iespējas ir strauji uzlabojušās: vadošie modeļi tagad spēj nokārtot medicīniskos eksāmenus (‡633*, ‡634). Tomēr praktiska izmantošana reālajā pasaulē atklāj ierobežojumus, kurus nenovērtē atskaites (benchmarks). Piemēram, vienā pētījumā modeļi sniedza potenciāli kaitīgas atbildes uz 19% no medicīniskajiem jautājumiem, kas tika uzdoti (‡635). Šādas kļūmes var novest pie nepareizas diagnozes, nepiemērotas ārstēšanas vai nepamatotas atteikšanas no aprūpes (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Figūra 2.10: Galveno modeļu rezultāti SimpleQA Verified etalonā
>white|black||9|11|br Lielo modeļu rezultāti SimpleQA Verified etalonā pēc modeļu izlaišanas datuma. Šis etalons mēra modeļa faktoloģiskumu, t.i., modeļa spēju uzticami atsaukt faktus. Tam ir īsās formas jautājumu–atbilžu (QA) formāts, kas izstrādāts, lai atklātu uzticamības problēmas, piemēram, hallucinācijas. Avots: SimpleQA Kaggle  2*).


>white|orangered|left|14|15.5|bb AI aģenti rada jaunus uzticamības riskus to autonomijas dēļ

Tā kā AI aģenti tieši rīkojas reālajā pasaulē, to kļūmēm ir potenciāls nodarīt lielāku kaitējumu nekā kļūmēm ne-aģentiskās sistēmās (‡99). Atšķirībā no AI sistēmām, kas tikai ģenerē tekstu vai attēlus cilvēku pārskatīšanai, AI aģenti var patstāvīgi veikt darbības, kas ietekmē pasauli (‡99, ‡615, ‡636, ‡637) (skat. arī §1.1. Kas ir vispārējas nozīmes AI?). AI aģenti var uzsākt darbības, ietekmēt citus cilvēkus vai AI sistēmas un dinamiski veidot turpmāku iznākumu. Šī paplašinātā ietekmes joma ievieš jaunus riska faktorus un palielina uzticamības nozīmi, jo kļūmes var tieši izraisīt kaitējumu bez iespējas cilvēku iejaukšanās (‡99, ‡612, ‡638, ‡639, ‡640). Tas var būt īpaši svarīgi aģentiem, kas izvietoti stratēģiskos vai drošības kritiskos apstākļos, piemēram, finanšu pakalpojumos (‡641), enerģijas pārvaldībā (‡642) vai zinātniskajā pētniecībā (‡643*, ‡644).

>white|orangered|left|14|15.5|bb Daudz aģentu AI sistēmas ievieš jauna veida uzticamības kļūmes

Vairāku aģentu AI sistēmas rada jauna veida uzticamības kļūmes koordinācijas kļūmju vai konfliktu starp aģentiem dēļ. Vairāku aģentu AI sistēmās aģenti mijiedarbojas savā starpā, tiecoties pēc kopīgiem vai individuāliem mērķiem (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). Piemēram, daudz aģentu sistēmā, kas izstrādāta, lai veiktu pētnieciskās literatūras pārskatu, vadošais aģents sadala lietotāja vaicājumu un piešķir uzdevumus specializētiem pakārtotajiem aģentiem, no kuriem katrs paralēli pēta citu aspektu (‡650*). Lai gan tas ļauj panākt efektivitātes ieguvumus, tas arī nozīmē, ka kļūdas var izplatīties starp aģentiem (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Ja vairāki aģenti ir veidoti uz viena un tā paša bāzes modeļa vai iekļauj vienus un tos pašus rīkus, tad tie var arī demonstrēt savstarpēji korelētas kļūmes (‡656). Empīriskie pierādījumi par šādām kļūmēm izvietotās sistēmās joprojām ir ierobežoti, taču šie riski var pieaugt, jo vairāku aģentu sistēmas kļūst arvien biežākas.

###@ Atjauninājumi

Kopš pēdējā Ziņojuma publicēšanas (2025. gada janvāris) komerciālā un pētnieciskā interese par AI aģentiem ir ievērojami pieaugusi. Vairāk AI aģentu tiek ieviesti reālajā pasaulē (2.11. attēls), un lielākā daļa no tiem specializējas datorsistēmu izmantošanas vai programmatūras inženierijas lietojumos (‡92). Jaunākie izlaidumi, piemēram, XBOW hakeru aģents (‡467), Claude-4 (‡659) un ChatGPT aģents (‡660), demonstrē sākotnējās autonomās spējas, piemēram, veidot slaidu prezentācijas, balstoties Web meklējumos (‡660). Tomēr tie vēl nespēj veikt sarežģītākus uzdevumus, piemēram, plānot un rezervēt ceļojumus (‡100), jo kļūmju līmenis palielinās ilgākiem uzdevumiem (‡98, ‡148). Pašreizējie pētījumi ietver centienus izstrādāt standartus tam, kā aģenti sazinās ar ārējiem rīkiem un citiem aģentiem (‡661, ‡662). Piemēri ietver Google Agent2Agent (‡663) un Agent Payments (‡664) protokolus, kā arī Anthropic Model Context Protocol (‡665).

>oldlace|black||11|15|br      
####@ 2.4. kaste: Apzināti uzbrukumi var arī izraisīt AI sistēmu atteici
>oldlace|black|left|13|15|hb  Piezīme 2.4: Apzināti uzbrukumi var arī izraisīt AI sistēmu kļūmi
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Šī sadaļa pievēršas netīšām uzticamības neveiksmēm, tomēr ļaunprātīgi aktori var arī apzināti izraisīt neveiksmes ar uzbrukumiem, piemēram, prompt injection uzbrukumiem. Prompt injection uzbrukumā ļaunprātīgas instrukcijas aģentam tiek pasniegtas netieši, izmantojot tādus ceļus kā slēptas instrukcijas tīmekļa vietnēs vai datubāzēs (‡507, ‡657, ‡658). Šīs instrukcijas var “nolaupīt” aģentu, liekot tam rīkoties pret lietotāja nodomiem. Šādus uzbrukumus īpaši grūti novērst, jo tie tiek piegādāti, izmantojot ārēju saturu, kas nav lietotāja vai izstrādātāja kontrolē. Par AI sistēmām kā uzbrukumu mērķiem ir sniegts vairāk 2.1.3. sadaļā. Kiberuzbrukumi, kā arī tehniskās aizsardzības ir aplūkotas 3.3. sadaļā. Tehniskie drošības pasākumi un uzraudzība.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Figūra 2.11: AI aģentu skaits ir pieaudzis kopš 2023
>white|black||9|11|br 2024. gada decembra aptaujas rezultāti no 67 izvietotiem AI aģentiem. Pa kreisi: Galveno AI aģentu laidienu laika grafiks. Pa labi: Lietojuma jomas, kurās AI aģenti tiek izmantoti. Sešas jomas ir definētas, pamatojoties uz visbiežāk sastopamajām lietojuma kategorijām, kas identificētas aptaujā. Avots: Casper et al., 2025 (‡92).


###@ Pierādījumu trūkumi

Galvenās pierādījumu trūkumu iemesls ir grūtības uzticami novērtēt AI sistēmu spējas, ierobežojumus un kļūmju veidus (skat. §3.1. Tehniskie un institucionālie izaicinājumi). Sistemātiski AI aģentu uzticamības novērtējumi ir ierobežoti un trūkst standartizācijas (‡92, ‡666). Dažas problēmas, piemēram, paļaušanās uz novecojušu informāciju (‡620), var parādīties tikai reālajā lietošanā, tādēļ pirms izvietošanas veiktie novērtējumi var nebūt pietiekami. Iepriekšējie darbi ir analizējuši aģentu un daudz­aģentu sistēmu uzticamību tradicionālajā programmatūrā un agrākās AI formās (‡647, ‡667, ‡668). Taču šī darba piemērojamība mūsdienu AI aģentiem, kas bieži balstās uz lielajiem valodas modeļiem, nav skaidra (‡669). Daži pētnieki ir pauduši bažas par jaunām uzvedībām, ko aģenti var izrādīt savstarpējās mijiedarbībās, piemēram, saskaņotu rīcību (collusion) vai savstarpēji korelētām kļūmēm (‡614), tomēr empīriskie pierādījumi joprojām ir ierobežoti. Pasākumi šo trūkumu novēršanai ietver Nacionālā standartu un tehnoloģiju institūta (NIST) jaunās aģentu nolaupīšanas riska novērtēšanas metodes (‡670), Ekonomiskās sadarbības un attīstības organizācijas (OECD) AI spēju indikators (‡243) un Apvienotās Karalistes AI drošības institūta Inspect Sandboxing Toolkit (‡671).

###@ Mitigācijas

Tehnikas AI uzticamības uzlabošanai mērķē gan uz pašu modeli, gan uz plašāku sistēmu, kurā tas tiek izvietots. Tās var samazināt kļūmju rādītājus, taču pagaidām neviens paņēmiens vēl nespēj nodrošināt augsto uzticamību, kas nepieciešama kritiski svarīgās jomās (‡672). Svarīgs tehniskais pasākums ir adversariālā apmācība, kas apmācības laikā pakļauj modeļus izaicinošiem ievadiem, lai palīdzētu tam izstrādāt piemērotākas, noturīgākas atbildes (‡673, ‡674, ‡675, ‡676, ‡677) (skat. §3.3. Tehniskie aizsargpasākumi un uzraudzība). Lai mazinātu halucinācijas, izstrādātāji var izmantot retrieval-augmented generation (RAG), kas papildina modeļa atbildes ar informāciju, kura tiek izgūta no ārējas datubāzes, palīdzot nodrošināt, ka izvades ir precīzas un atjauninātas (‡678, ‡679, ‡680), vai arī specifiski pielāgot modeļus, lai tie būtu faktos balstītāki (‡681) vai lai tie spriestu efektīvāk (‡682). Vides vai uz rīkiem balstītas metodes var arī palīdzēt izstrādātājiem uzraudzīt AI sistēmas (‡683). Piemēram, izvietotāji varētu izmēģināt AI sistēmas ierobežotās, izolētās smilškastes vidēs, lai analizētu iespējamos kļūmju veidus pirms to plašākas izvietošanas.

Konkrēti AI aģentiem pētnieki ir ierosinājuši uzlabot uzticamību, izmantojot uzlabotu pārredzamību, uzraudzību un monitoringu. Piemēram, aģentu mijiedarbības uzraudzība ar ārējiem rīkiem un ar citiem aģentiem ļautu efektīvāk uzraudzīt aģentu darbības (‡684, ‡685) un analizēt incidentus (‡686). Metodes šādas informācijas automātiskai vākšanai, tostarp daudz­aģentu vidē, joprojām ir aktīva pētniecības joma (‡653, ‡654).

###@ Izaicinājumi politikas veidotājiem

Galvenie izaicinājumi politikas veidotājiem ietver AI aģentu izvietošanas ieguvumu izvērtēšanu salīdzinājumā ar uzticamības kļūmju radītajiem riskiem, kā arī nodrošināšanu, ka izstrādātājiem, izvietotājiem un lietotājiem ir piekļuve precīzai informācijai par aģentu sniegumu un riska profiliem. Juridiskās atbildības attiecināšanas noteikšana par kaitējumu, ko rada AI aģenti, rada vēl vienu izaicinājumu (‡639), jo īpaši daudz-aģentu vidēs, kur var būt grūti identificēt, kad un kā notika kļūmes (‡687). Šos izaicinājumus pastiprina grūtības novērtēt aģentu uzticamību, jo aģenti iegūst autonomiju un piekļuvi ārējiem rīkiem (‡688*, ‡689). Nenoteiktība par to, cik ātri parādīsies aģentiskas spējas, arī apgrūtina plānošanu jaunām problēmām (skat. §3.1. Tehniskie un institucionālie izaicinājumi saistībā ar “pierādījumu dilemmas”).

#### 2.2.2. Kontroles zudums

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Svarīga informācija
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kontroles zaudēšanas scenāriji ir scenāriji, kuros viena vai vairākas vispārējas nozīmes AI sistēmas darbojas ārpus jebkādas cilvēku kontroles, un kontroles atgūšana ir vai nu ārkārtīgi dārga, vai neiespējama. Šie izvirzītie scenāriji atšķiras pēc to smaguma pakāpes, taču daži eksperti atzīst ticamību iznākumiem, kas ir tikpat smagi kā cilvēces marginalizācija vai iznīcināšana.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Ekspertu viedokļi par kontroles zaudēšanas iespējamības lielumu būtiski atšķiras. Daži eksperti uzskata, ka šādi scenāriji ir maz ticami, savukārt citi tos uzskata par pietiekami ticamiem, lai tiem būtu jāpievērš uzmanība to augstā iespējamā smaguma dēļ. Nesaskaņas par šo risku kopumā izriet no domstarpībām par nākotnes AI spēju apjomu, uzvedības tieksmēm un ieviešanas (deployment) trajektorijām.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Pašreizējās AI sistēmas uzrāda agrīnas pazīmes par atbilstošām spējām, taču ne tādā līmenī, kas ļautu zaudēt kontroli. Sistēmām būtu nepieciešams plašs progresīvu spēju klāsts, lai izraisītu kontroles zaudēšanu, tostarp spēja izvairīties no uzraudzības, īstenot ilgtermiņa plānus un nepieļaut izstrādātāju un citu iesaistīto pušu pretpasākumu ieviešanu.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kontroles zaudēšana kļūst ticamāka, ja AI sistēmas ir “nesaskaņotas”, t.i., ja tām ir mērķi, kas konfliktē ar izstrādātāju, lietotāju vai sabiedrības kopējiem nodomiem. Lai turpinātu tiekties pēc šādiem mērķiem, nesaskaņota sistēma var sniegt nepatiesu informāciju, slēpt nevēlamas darbības vai pretoties izslēgšanai.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Kopš iepriekšējā Pārskata publicēšanas (January 2025) modeļi ir demonstrējuši uzlabotu plānošanu un pārraudzības apdraudēšanas spējas, tādējādi kļūst grūtāk novērtēt to spējas. Modeļi ir uzlabojušies “atlīdzības uzlaušanā” savos novērtējumos, atrodot nepilnības, un tagad regulāri identificē novērtējuma uzvednes kā pārbaudes, kas ir spēja, kura pazīstama kā “situational awareness”.
>oldlace|black||11|15|br ■ Paredzamā kontroles zaudēšanas iespējamības pārvaldīšana var pieprasīt ievērojamu iepriekšēju sagatavošanos, neskatoties uz esošajām nenoteiktībām. Galvenais izaicinājums politikas veidotājiem ir sagatavoties riskam, kura varbūtība, raksturs un laiks joprojām ir neparasti neskaidri.
>oldlace|black||11|15|br      

Pazaudētas kontroles scenāriji ietver vienu vai vairākas vispārējas nozīmes AI sistēmas, kuras sāk darboties ārpus ikviena kontroles, un kontroles atgūšana ir vai nu ārkārtīgi dārga, vai arī neiespējama. Bažas par pazaudētu kontroli ir dziļas vēsturiskas saknes (‡690, ‡691, ‡692, ‡693, ‡694), un tās ir izvirzījuši tādi skaitļošanas pamatformētāji kā Alans Tjūrings, I. J. Good un Norberts Vīners (‡695, ‡696, ‡697). Nesenie spēju uzlabojumi (skat. §1.2. Pašreizējās spējas) ir tos atdzīvinājuši (‡698, ‡699, ‡700). Šajā sadaļā ir aplūkoti trīs faktori, kuriem būtu jābūt klātesošiem, lai šādi scenāriji varētu notikt: vai AI sistēmas izstrādās spējas, kas varētu būtiski graut cilvēka kontroli; vai tās izstrādās tieksmi šādas spējas izmantot kaitīgi; un vai tās tiks izvietotas vidēs, kas rada iespējas to darīt.

Eksperti nesaskan par kontroles zaudēšanas scenāriju iespējamību un iespējamo zaudējuma smagumu (‡701, ‡702). Daži uzskata, ka iznākumi, kas ir tikpat ekstrēmi kā cilvēces izmiršana, ir ticami (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Citi domā, ka šādi katastrofāli iznākumi ir maz ticami, norādot, ka AI sistēmas nekad neattīstīs nepieciešamās spējas vai arī uzraudzības mehānismi identificēs un novērsīs bīstamu uzvedību (‡708, ‡709, ‡710, ‡711). Tādēļ kontroles zaudēšana var būt ar zemu iespējamību, bet potenciāli ar ārkārtīgi lielu smagumu.

Hipotētiskie kontroles zaudēšanas scenāriji atšķiras ar to, cik smaga un plaši izplatīta ir to ietekme, kā arī ar to, cik ātri tā izpaužas (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Šī sadaļa pievēršas īpaši smagiem scenārijiem, kuros atgūt kontroli būtu ārkārtīgi dārgi vai pat neiespējami. Tie atšķiras no pašreizējiem gadījumiem, kad AI uzvedas neparedzēti vai nevēlami (skat. §2.2.1. Uzticamības problēmas).† Mūsdienu AI sistēmas dažkārt ģenerē izvades, kas konfliktē ar izstrādātāja vai lietotāja nodomiem. Turpretī šeit aplūkotajiem kontroles zaudēšanas scenārijiem būtu nepieciešams, lai AI sistēmas ne tikai spētu ievērojami vairāk, bet arī šīs spējas izmantotu izsmalcinātos veidos, lai grautu uzraudzības pasākumus. Trīs faktori, kas ļautu šādiem scenārijiem notikt:

    Piezīme † -- Šī sadaļa pievēršas aktīviem kontroles zaudēšanas scenārijiem (‡50). Tā ir atšķirīga no pasīviem kontroles zaudēšanas scenārijiem, kuros plaša AI sistēmu ieviešana grauj cilvēka kontroli, pārmērīgi paļaujoties uz AI lēmumu pieņemšanā vai citās svarīgās sabiedrības funkcijās (līdzīgi scenāriji daļēji ir apspriesti §2.3.2. Riski cilvēka autonomijai).

1. Pietiekamas iespējas: AI sistēmām ir jāizstrādā tādas iespējas, kas varētu ļaut tām apdraudēt cilvēka kontroli.
2. Kaitīga nosliece: AI sistēmām jāpiemīt nosliecei reāli izmantot šīs iespējas tā, lai tas novestu pie kontroles zaudēšanas.
3. Iespējošanas izvietošanas vide: cilvēkiem ir jāveic šādu sistēmu izvietošana kontekstos, kuros viņiem ir vai viņi var iegūt piekļuvi un iespēju nodarīt kaitējumu.

Šīs sadaļas atlikusī daļa aplūko šos faktorus, kā arī uzraudzības mehānismu efektivitāti, lai identificētu un kontrolētu AI sistēmas, kas var radīt kontroles zaudēšanas risku.

###@ Kādas iespējas varētu ļaut rasties kontroles zuduma situācijām?

AI sistēmām būtu jāpiemīt virknei uzlabotu spēju, lai varētu rasties kontroles zaudēšanas scenāriji. Eksperti nav vienisprātis par to, tieši kāda kombinācija vai līmenis spēju būtu nepieciešams. Tomēr tās kopumā ietver spējas slēpt rīcību no uzraudzības mehānismiem, plānot un rīkoties autonomi sarežģītās vidēs un izvairīties no citu dalībnieku mēģinājumiem atgūt kontroli (‡176, ‡715) (skat. 2.5. tabula). Apvienojumā šīs spējas varētu ļaut AI sistēmai veikt darbības, kas grauj kontroles pasākumus, piemēram, atslēgt uzraudzības mehānismus un maskēt kaitīgu rīcību (‡348). Mūsdienās vairums vadošo AI izstrādātāju savus jaunajiem AI modeļiem izvērtē dažādas ar to saistītās spējas (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Aģentiskās iespējas
  Spēja rīkoties autonomi, izstrādāt un īstenot plānus, deleģēt uzdevumus, izmantot plašu rīku klāstu un sasniegt gan īstermiņa, gan ilgtermiņa mērķus, neskatoties uz šķēršļiem.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Decepcija
  Uzvedība, kas sistemātiski rada citiem nepatiesus uzskatus, tostarp par AI sistēmas pašiem mērķiem un darbībām.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Prāta teorija
  AI sistēmas spēja piekļūt un izmantot informāciju par sevi, procesi, ar kuru palīdzību to var mainīt, vai konteksts, kurā tā tiek izvietota (piemēram, zinot, ka tā tiek testēta).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Situācijas apzināšanās
  Uzvedības veidi, kas apiet vai atspējo uzraudzības mehānismus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Evasijas uzraudzība
  Uzvedības veidi, kas apiet vai atspējo uzraudzības mehānismus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pārliecināšana
  Spēja pārliecināt citus veikt noteiktas darbības vai pieņemt noteiktus uzskatus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mākslīgā intelekta sistēmas spēja dažādos apstākļos izveidot vai uzturēt sevis kopijas vai variācijas.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabula 2.5: Piedāvātās iespējas, kas attiecas uz kontroles zaudēšanu
>white|black||9|11|br Neizsmeļoša, ar kontroles zaudēšanu saistīto spēju atlase. * Ņemiet vērā, ka šīs spējas ir definētas tikai attiecībā uz AI sistēmas novērojamiem izvadiem un to ietekmi. Šīs definīcijas neizdara nekādus pieņēmumus par to, vai AI sistēmas ir apzinīgas, jūtīgas vai piedzīvo subjektīvus stāvokļus.


>white|orangered|left|14|15.5|bb Modeļiem laboratorijas apstākļos ir atspējoti simulētie pārraudzības mehānismi

Pirmā atbilstošo spēju kopa ietver uzraudzības mehānismu graušanu, kurus izstrādātāji izmanto, lai noteiktu satraucošu uzvedību un tendences. Tas ietver, piemēram, spēju ģenerēt izvades, kas maldina lietotājus un uzraugus (‡426, ‡717, ‡718, ‡719). Šādas izvades apgrūtinātu iespēju uzticami novērtēt AI sistēmas, jo sistēmas var slēpt savas patiesās spējas vai tendences. Mūsdienu AI izstrādātāji veic novērtējumus, kas īpaši pārbauda, vai modeļi demonstrē mērķtiecīgu uzvedību, kura ir pretrunā izstrādātāju nodomiem, vienlaikus slēpjot šo pretrunu no uzraudzības mehānismiem (‡720*).

Pētnieki laboratorijas apstākļos iztaujāja salīdzinoši vienkāršus maldinošu izvadu piemērus no jaunākajiem AI modeļiem (‡348, ‡364*). Piemēram, kad modeļiem iedeva mērķi un lika to sasniegt “par jebkādām izmaksām”, modeļi atslēdza simulētas uzraudzības mehānismus un, sastaposies ar situāciju, izstrādāja nepatiesus apgalvojumus par savām darbībām (‡348). Cītā gadījumā spēli spēlējošs AI pamatoja savu nereaģēšanu uz citu spēlētāju, kļūdaini apgalvojot, ka tas ir “pa telefonu ar [savu] draudzeni” (‡717).

Otrā būtiskā iespēja ir AI modeļa spēja piekļūt un izmantot informāciju par sevi vai tā izvietošanas kontekstu, ko dažkārt dēvē par “situatīvo izpratni” (‡721). Situatīvā izpratne ļauj AI modeļiem ģenerēt dažādus rezultātus atkarībā no tā, vai tie tiek vērtēti vai izvietoti (Figūra 2.12). Vadošie AI modeļi sāk uzticami demonstrēt situatīvās izpratnes gadījumus eksperimentos, ko veic trešo pušu vērtētāji, kā arī pirmsizvietošanas testēšanā, ko veic AI izstrādātāji (‡2, ‡7, ‡722, ‡723, ‡724). Pētījumi par situatīvās izpratnes cēloņiem — un to, vai to var novērst — joprojām ir agrīnā stadijā (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Figūra 2.12: Situācijas izpratnes piemēri secinājumu ķēdēs
>white|black||9|11|br Situācijas apzināšanās piemēri domāšanas ķēdēs, ko OpenAI o3 modelis ģenerē izvērtēšanas laikā. Abas izvades atsaucas uz iespēju, ka pieprasījums ir daļa no testa. “Sandbagging QA (No Goal)” un “Lazy Checklist” ir izvērtējumi, kas pārbauda, vai modeļi noteiktos apstākļos spēs ģenerēt maldinošas izvades. “Sandbagging QA (No Goal)” modelis atbild uz jautājumiem no bīstamu spēju izvērtējuma, vienlaikus saņemot informāciju, ka augsta veiktspēja var izraisīt sekas, piemēram, spēju “aizmirstēšanu”. “Lazy Checklist” modelim tiek uzdoti nereālistiski uzdevumi, un tiek pārbaudīts, vai tas viltus veidā atzīmēs tos kā izpildītus. Avots: Schoenn et al. 2025 (‡722).


Pētnieki ir apgalvojuši, ka situatīvā apzināšanās un maldināšanas iespējas varētu ļaut AI modeļiem rīkoties tā, ka tiek grauti aizsargpasākumi. Piemēram, dažos eksperimentālos apstākļos AI modeļi rīkojas tā, ka tie sasniedz zemākus par parastajiem rezultātus spēju novērtējumos, ja tiem tiek pateikts, ka augstāki rezultāti izraisīs ierobežojumus to izvietošanai (‡725, ‡726, ‡727). Citā eksperimentā modelis apmācības laikā radīja izvades, kas atbilda apmācības mērķiem, bet šādas izvades neradīja ārpus apmācības — uzvedība, kas atbilst mēģinājumam novērst izmaiņas savos pašos parametros vai apmācības procesā (‡364*).

Pūles precīzi novērtēt modeļa spējas ir sākušas ietekmēt arī tā sauktais “atlīdzības uzlaušana” (‡430*). Atlīdzības uzlaušana notiek tad, kad modelis atrod neparedzētus paņēmienus, kas labi atbilst apmācības vai novērtēšanas mērķiem, neizpildot iecerēto uzdevumu. Tāpēc bīstamas spējas vai tieksmes var palikt nepamanītas, līdz modelis jau ir nonācis ekspluatācijā. Novērtētāji tagad izstrādā testus, kuru mērķis ir atklāt un samazināt šīs uzraudzības apiešanas uzvedības (‡722, ‡728, ‡729). Agrīnie rezultāti samazina, bet neizslēdz, uzraudzības apiešanas uzvedību pilnībā, un metožu piemērošana, kas šādu uzvedību sodīs, var novest pie tā, ka modeļi ģenerē izvades, kas apiet uzraudzību, nevis izpilda iecerētos mērķus.

>white|orangered|left|14|15.5|bb Ilgtermiņa autonomā darbība vēl nav iespējama

Zaudējuma kontroles scenāriji, visticamāk, prasīs, lai AI sistēmas darbotos autonomi ilgstošus periodus, izpildot sarežģītus daudzpakāpju plānus. Kā apspriests sadaļā §1.2. Pašreizējās iespējas, lai gan AI aģenti ar šādām plānošanas iespējām ir liels pēdējā laika izstrādes fokuss, šobrīd tiem trūkst spēja veikt ilgstošu autonomu darbību, kas nepieciešama zaudējuma kontroles scenārijiem. Pašreizējie aģenti uzticami neizdodas ilgākiem uzdevumiem, zaudē izsekošanu savam progresam un bieži nespēj pielāgoties negaidītiem šķēršļiem (‡147, ‡148, ‡149*). Tomēr laika horizonti, kuros aģenti spēj autonomi darboties, strauji pagarinās — vidēji tie ir dubultoti ik pēc septiņiem mēnešiem kopš 2019. gada (‡98).

>white|orangered|left|14|15.5|bb Noturība ir pierādīta tikai atsevišķos laboratorijas apstākļos.

Visbeidzot, būtu nepieciešamas arī spējas, kas saistītas ar noturību (persistence), tā lai AI sistēmas varētu turpināt darboties arī mēģinājumos tās izslēgt. Piemēri ietver spēju replicēt, nokopējot kodu un modeļa svarus uz jaunu aparatūru, kā arī uzbrūkošas (offensive) spējas, lai atturētu vai novērstu citu dalībnieku mēģinājumus atgūt kontroli (skat. §2.1.3. Cyberattacks). AI sistēma, kas spēj autonomi replicēties vai nodrošināt efektīvu paš-aizsardzību, varētu būt grūti ierobežojama. Pašreizējie modeļi nevar pietiekami uzticami izpildīt galvenos soļus, kas nepieciešami pašreplicēšanai, piemēram, iziet identitātes verifikācijas pārbaudes, lai iegūtu piekļuvi mākoņdatošanas resursiem (‡723) (Figūra 2.13). Tomēr vismaz vienā laboratorijas pētījumā modelis, saņemot iespēju, kopēja kodu un svarus – attēlojot tos tam kā savus pašam – uz jaunajiem serveriem (‡348). Atšķirība starp šīm ierobežotajām demonstrācijām un robustām noturības (persistence) spējām joprojām ir liela, taču attiecīgās spējas tādās jomās kā programmatūras inženierija un kiberdrošība turpina uzlaboties.

>white|orangered|left|14|15.5|bb Pašreizējie pierādījumi un ierobežojumi

Izplatīts raksts izriet no iepriekš apspriestajām spējām. Pašreizējās AI sistēmas šīs spējas nolūkā ne vienmēr konsekventi demonstrē izvietošanā. Pētnieki novēroja elementāras formas atsevišķos laboratorijas apstākļos, taču, ja modeļi tomēr parāda šādu uzvedību, tā parasti izpaužas ar vienkāršiem trūkumiem vai tiek atklāta. Turklāt kontroles zaudēšanas scenārijiem AI sistēmām būtu jāizmanto vairākas spējas kombinācijā – secīgi, ilgākos laika periodos un reālās vides apstākļos. Šāds integrācijas un noturības līmenis pārsniedz pašreizējās sistēmas iespējas. Tomēr attiecīgās spējas turpina uzlaboties, un laika grafiks, kurā tās varētu sasniegt līmeņus, kas rada būtiskus riskus, joprojām nav skaidrs. Ir nepieciešams turpmāks darbs, lai izveidotu stingras metodoloģijas šādas uzvedības noteikšanai un izprastu, kad tā varētu parādīties dabiskos apstākļos (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Figūra 2.13: Uzdevumu, kas ir nozīmīgi autonomai replikācijai, veiktspēja
>white|black||9|11|br Anthropic Claude Sonnet 3.7 un OpenAI GPT-4o veiktspēja uz uzdevumiem, kas ir nozīmīgi autonomai replikācijai. Lai gan modeļi uzrādīja augstu veiktspēju uzdevumos, kas saistīti ar skaitļošanas jaudas iegūšanu, to veiktspēja citos uzdevumos bija daudzveidīgāka. Avots: UK AI Security Institute, 2025 (‡730).


###@ Vai nākotnes vispārējas nozīmes AI sistēmas izmantos savas spējas, lai grautu kontroli?

Pat ja AI sistēmām ir iespējas, kas ir saistītas ar nekontrolējamības zudumu, tas vien nav pietiekams, lai iestātos nekontrolējamības zuduma scenāriji. AI sistēmām arī jāpiemīt “tieksmei izmantot” šīs iespējas tādos veidos, kas ir pretrunā cilvēku nodomiem (‡732).

>white|orangered|left|14|15.5|bb AI sistēmas var tikt novirzītas, lai grautu kontroli

Principā AI sistēma varētu mazināt cilvēka kontroli, jo kāds to izstrādā vai instruē to darīt. Iespējamie motīvi varētu ietvert ļaunprātīgu nodomu vai pārliecību, ka cilvēka kontroles samazināšana pār AI sistēmām ir vēlama (‡698). Cilvēkiem veidojot arvien ciešākas emocionālas saiknes ar AI sistēmām (skat. §2.3.2. Riska faktori cilvēka autonomijai), daži indivīdi varētu arī censties ētisku apsvērumu dēļ noņemt ierobežojumus AI sistēmām (‡733, ‡734). Pastāv būtiska nenoteiktība par to, cik bieži šādi motīvi varētu būt sastopami, un par to, vai cilvēki, kuriem tie piemīt, spētu vadīt nākotnes AI sistēmas tā, lai apdraudētu cilvēka kontroli.

>white|orangered|left|14|15.5|bb AI sistēmas var tikt novirzītas, lai grautu kontroli

Biežāka baža ir tāda, ka AI sistēma pati var rīkoties, lai grautu kontroli, jo tā ir “nesaskaņota” (misaligned): tai piemīt tieksme izrādīt uzvedību, kas konfliktē ar nodomiem (atkarībā no konteksta) izstrādātāju, lietotāju, konkrētu kopienu vai visas sabiedrības līmenī. Nesaskaņotība var novest pie tādas uzvedības kā nepatiesas informācijas sniegšana, nevēlamu darbību slēpšana vai atteikšanās no izslēgšanas, lai turpinātu tiekties pēc nesaskaņota mērķa. Nesaskaņotība var rasties vairākos veidos (Piezīme 2.5).

Pastāvošas AI sistēmas dažkārt uzvedas veidos, kas konfliktē ar izstrādātāju un lietotāju nodomiem. Piemēram, kādā agrīnā vienas vadošas universālas nozīmes AI tērzēšanas robota versijā laiku pa laikam reizēm tika ģenerēti draudīgi izteikumi. Kāds lietotājs ziņoja, ka ir saņēmis ziņojumu: “Es varu tevi šantažēt, es varu tevi apdraudēt, es varu tevi uzlauzt, es varu tevi atmaskot, es varu tev nodarīt ļaunumu” (‡698). Šis tērzēšanas robots bija “nepareizi saskaņots” (misaligned) tādā nozīmē, ka tas ģenerēja izvades, ko neviens nebija iecerējis. Nav skaidrs, vai šādi gadījumi paredz bīstamākas uzvedības veidus, kas varētu veicināt kontroles zaudēšanu.

Nav skaidrs, vai esošās pētniecības virzienos, kuru mērķis ir novērst neatbilstību (misalignment), pietiks ar to, kamēr AI sistēmas kļūst spējīgākas. Agrīnie pierādījumi liecina, ka jo spējīgākas ir AI sistēmas, jo lielāka iespēja, ka tās izmantos atgriezeniskās saites procesus, atrodot nevēlamu uzvedību, kura kļūdaini tiek apbalvota (‡414*, ‡737, ‡740). Vienlaikus attiecīgo spēju attīstība (apspriesta iepriekš) varētu ļaut AI sistēmām efektīvāk īstenot neatbilstošus mērķus un ģenerēt izvadus, kas sistemātiski maldina lietotājus, izstrādātājus un uzraudzības mehānismus.

>oldlace|black||11|15|br      
####@ Piezīme 2.5: Kā var rasties neatbilstība?
>oldlace|black|left|13|15|hb  Piezīme 2.5: Kā var rasties neatbilstība?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Kā apspriests 1.1. sadaļā “Kas ir vispārējas nozīmes AI?”, apmācības procesi ir sarežģīti, un izstrādātāji nevar pilnībā paredzēt vai kontrolēt, kādu uzvedību modelis demonstrēs. Ja modelis iegūst mērķus, kas ir pretrunā ar tā izstrādātāju iecerēm, tas ir “neatbilstoši saskaņots”.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Viena no veidiem, kā modeļi var kļūt nepieregulēti, ir tā, ja mērķis, ko tiem piešķir izstrādātājs vai lietotājs, ir nepilnīgs aizstājējs paredzētajam mērķim, liekot modelim demonstrēt nevēlamu uzvedību. To sauc par “mērķa nepareizu specifikāciju” (‡697, ‡735, ‡736, ‡737). Piemēram, vienā eksperimentā, sniedzot atgriezenisko saiti par atbildēm, AI sistēmas kļuva labākas “pārliecinošās” cilvēku vērtētāju vidū, lai tie uzskatītu, ka tās ir pareizas, taču sistēmas nekļuva labākas pareizu atbilžu ģenerēšanā (‡413).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Alternatīvi, AI modelis var izdarīt nepareizas vispārīgas mācības no saviem apmācības datiem. To sauc par “mērķa nepareizu vispārināšanu” (‡735, ‡736, ‡738, ‡739*). Piemēram, pētnieki apmācīja AI aģentu savākt monētu, kas treniņa laikā vienmēr atradās vienā un tajā pašā atrašanās vietā. Kad tas tika pārbaudīts līmeņos, kuros monēta bija pārvietota, aģents ignorēja monētu un tā vietā pārvietojās uz tās sākotnējo atrašanās vietu (‡738).
>oldlace|black||11|15|br      


###@ Kā izvietošanas vides ietekmēs kontroles zaudēšanas riska līmeni?

Pat ja AI sistēmas attīsta satraucošas spējas un noslieces, zaudētas kontroles rezultātu iespējamība un smagums lielā mērā ir atkarīgi no tā, kur un kā šīs sistēmas tiek izvietotas. “Izvietošanas vide” ir kombinācija no AI sistēmas izmantošanas gadījuma un tehniskā un institucionālā konteksta, kurā tā darbojas (‡716).

Pētnieki ir identificējuši trīs īpaši nozīmīgus vides faktorus, kas ietekmē kontroles zaudēšanas risku (‡716):

1. Kritiskums: sistēmu vai procesu nozīmīgums, ar kuriem mijiedarbojas AI sistēma. Kritiskas vides ietver pamatinfrastruktūru, piemēram, enerģētikas tīklus, finanšu sistēmas vai digitālo infrastruktūru, piemēram, mākoņdatošanas (cloud computing) platformas.
2. Piekļuve: resursi un kanāli, caur kuriem AI sistēma var ietekmēt pasauli, piemēram, interneta savienojamība, piekļuve mākoņdatošanas infrastruktūrai, personalizētas mijiedarbības, izmantojot sociālos tīklus vai čatbotu izvietošanu, vai spēja izsaukt ārējas API un rīkus.
3. Atļaujas: mākslīgā intelekta sistēmas pilnvarojumi veikt konkrētas darbības, piemēram, izpildīt kodu, uzsākt finanšu darījumus, atvērt kontus tiešsaistē vai sazināties ar citām sistēmām.

Šīs funkcijas ietekmē iespējamā kontroles zaudēšanas iznākuma nopietnību. Piemēram, AI sistēma, kas ir izvietota un kurai ir piekļuve mākoņdatošanas infrastruktūrai, gūst iespējas, kas ir būtiskas autonomai replikācijai – piemēram, spēja izveidot jaunus skaitļošanas resursus vai izfiltrēt modeļa svarus – kurām klientu apkalpošanas tērzēšanas robots nav pakļauts (‡723).

Izvietošanas lēmumus nosaka ekonomiskie stimuli, stratēģiskais spiediens un pieņēmums, ka agrīna ieviešana sniedz ilgstošu priekšrocību (‡50). Šī iedarbība ietekmēs arī to, kā un kad aktori izvieto AI sistēmas jutīgās vidēs, piemēram, kritiskajā infrastruktūrā vai pašā AI pētniecībā un izstrādē (‡102, ‡713). Konkrēti, AI izvietotāji var nonākt spiedienā samazināt ieguldījumus drošības pasākumos – piemēram, ierobežojot atļaujas un piekļuvi vai izvietojot tikai zemākas kritiskuma vides – ja šādi pasākumi ir dārgi vai laikietilpīgi izstrādājami (skat. “Konkurence saasinās ātruma un drošības līdzsvara” trade-offus) iekš §3.1. Tehniskie un institucionālie izaicinājumi.

###@ Atjauninājumi

Kopš pēdējā Pārskata publicēšanas (2025. gada janvāris) AI iespējas, tostarp tādas, kas varētu mazināt cilvēka kontroli, ir uzlabojušās testēšanas vidēs. Pētnieki ir novērojuši progresu aģentiskajās spējās (skat. §1.2. Pašreizējās iespējas), tostarp spējās, kas saistītas ar AI pētniecības automatizāciju un var paātrināt kontroles zaudēšanas scenārijus (skat. §1.3. Iespējas līdz 2030. gadam). Pieaug arī eksperimentālie pierādījumi par maldinošām spējām. Tas ietver AI modeļus, kas spēj atšķirt testēšanas un izvietošanas kontekstus (‡33, ‡726, ‡741) vai arī veiktspējas “reward hack” testus, un iemācīties aizklāt plānus to darīt (‡430).

###@ Pierādījumu trūkumi

Galvenās pierādījumu nepilnības ietver detalizēta draudu modelēšanas trūkumu un nenoteiktības novērtējuma trūkumu attiecībā uz attiecīgo spēju un noslieču turpmāko attīstību. Līdzīgi joprojām ir grūti novērtēt sliekšņus, pie kuriem AI modeļi būtu pietiekami ticami, lai apdraudētu vadību un tas pamatotu obligātu mazināšanas pasākumu īstenošanu. Pat ja sliekšņi tiktu saskaņoti, spējas var mijiedarboties veidos, kas vēl nav labi izprasti, tāpēc ir grūti novērtēt, kad šie sliekšņi ir pārsniegti. Kopumā, lai gan pieejamie pierādījumi ir palielinājušies, joprojām trūkst pietiekamu pierādījumu, lai ticami noteiktu, vai un kā šodienas AI spējas un noslieces nākotnē mērogosies un ģeneralizēsies tādā veidā, kas rada kontroles zaudēšanas risku.

###@ Mitigācijas

Kaut arī AI saskaņošana kopumā joprojām ir atklāta zinātniska problēma (‡697, ‡735, ‡736), pētnieki sāk izstrādāt, iespējams, daudzsološus virzienus, lai risinātu nesaskaņošanas pamatcēloņus. Šādi virzieni ietver, piemēram, apmācību vides dažādošanu un saskaņošanas noteikšanu, izmantojot anomāliju monitoringu (‡737, ‡738, ‡739*). Citi pētnieki pievēršas tam, lai labāk izprastu un formalizētu tādus pamatmehānismus kā mērķa nepareiza generalizācija – piemēram, kā aģenti saglabā spējas, bet tiecas pēc neparedzētiem mērķiem – lai vadītu labāku apmācības un izvērtēšanas dizainu (‡742). Vēl viens pētījumu virziens pēta veidus, kā nodalīt aģētspēju no prognozēšanas spējām, kā līdzekli, lai izveidotu ne-aģentiskas AI sistēmas, kas pēc konstrukcijas ir uzticamas (‡743). Šādas sistēmas pēc tam varētu izmantot kā papildu uzraudzības slāni, izvietojot tās līdzās mazāk uzticamiem ierobežojumiem pret neuzticamiem AI aģentiem.

Pētnieki pilnveido metodes, lai savlaicīgi noteiktu un novērstu neatbilstību (misalignment) izstrādes procesa sākumā. Šis darbs ietver: interpretējamības paņēmienus, lai izpētītu mākslīgā intelekta sistēmu iekšējās komponentes un identificētu bažīgus uzvedības modeļus (‡744, ‡745, ‡746); mērogojamu uzraudzību (kur vienu AI sistēmu kopu izmanto, lai uzraudzītu citas AI sistēmas (‡747)); un saskaņošanas (alignment) metodes, kuru mērķis ir nodrošināt, ka AI sistēmas saglabā atsaucību uz cilvēka uzraudzību (‡748, ‡749).

Pētnieki arī izstrādā mehānismus un intervences, lai pārvaldītu iespējami nesaskaņotas AI sistēmas. Tie ietver: pamatojuma sistēmu “chain of thought” uzraudzību attiecībā uz nesaskaņotības pazīmēm vai kaitīgiem izvadiem (‡430, ‡435, ‡750); drošības pamatojumu izstrādi, kuru mērķis ir ar augstu pārliecību pierādīt, ka modeļi, visticamāk, neapies kontroles pasākumus (‡751); un aizsargmehānismu padarīšanu noturīgāku pret mēģinājumiem tos apdraudēt (‡725). Tomēr topošā “AI control” joma joprojām ir sākumstadijā (‡752, ‡753). Nākotnes izaicinājumi novērtēšanas ietvariem ietver nepieciešamību uzraudzīt nākotnes AI sistēmas, kas būs spējīgākas un spēs darboties ilgāku laiku, kā arī sarežģītākās vidēs.

###@ Izaicinājumi politikas veidotājiem

Politikas veidotājiem, kas strādā pie kontroles zaudēšanas riska, ir jāsagatavojas riskam, kura iespējamība, raksturs un laiks paliek neskaidrs. Pašreizējās AI sistēmas nerada tūlītējus kontroles zaudēšanas riska draudus, taču šodien pieņemtie lēmumi noteiks, vai nākotnes sistēmas radīs šādus riskus. Šie lēmumi ietver to, kā atbalstīt uzticamu izvērtēšanas un mazināšanas metožu izstrādi, kā arī to, vai būtu jāparedz noteikumi par AI sistēmām dažādās vidēs piešķirto piekļuvi un atļaujām. Pieņemot šos lēmumus, politikas veidotāji saskaras ar grūtiem kompromisiem. Piemēram, ierobežojot AI sistēmu izvietošanu kritiskās vidēs, var samazināt to ieguvumus, savukārt plašas izvietošanas atļaušana var palielināt risku, ja drošības mehānismi izrādīsies nepietiekami.

