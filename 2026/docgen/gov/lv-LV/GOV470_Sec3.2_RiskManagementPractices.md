##########
>white|orangered|left|14|30|hr 3.2. sadaļa
### 3.2. Riska pārvaldības prakses
>white|orangered|left|24|30|hb Riska pārvaldības prakses

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Svarīga informācija
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Vispārējas nozīmes AI riska pārvaldība ietver virkni prakšu, ko izmanto, lai identificētu, novērtētu un mazinātu riskus, kas saistīti ar vispārējas nozīmes AI. Tās ietver modeļa līmeņa testēšanu un izvērtēšanu (piemēram, “red-teaming”), organizatoriskos procesus, kas virza izstrādes un izlaišanas lēmumus, nosacījumu aizsardzības mehānismus (piemēram, “if-then” saistības) un incidentu ziņošanu.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Vairāki AI izstrādātāji ir izstrādājuši Frontier AI Safety ietvarstruktūras. Šajās ietvarstruktūrās ir iekļauta informācija par riska novērtējumiem, kā arī tiek noteikti nosacīti pasākumi, piemēram, piekļuves ierobežojumi, ko uzņēmumi plāno ieviest spējīgākiem modeļiem. Tās atšķiras ar to, kādus riskus tās aptver, kā tās definē spēju sliekšņus un kādas darbības tiek aktivizētas, kad sliekšņi tiek sasniegti.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Pierādījumi par AI riska pārvaldības prakses reālo efektivitāti pasaulē joprojām ir ierobežoti. Ziņošanas par incidentiem un uzraudzības trūkums apgrūtina izvērtēt, cik labi pašreizējā prakse samazina riskus, vai arī to, cik konsekventi tā tiek īstenota.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kopš iepriekšējā ziņojuma publicēšanas (January 2025), riska pārvaldība ir kļuvusi strukturētāka, pateicoties jaunām nozares un pārvaldības iniciatīvām. Jauni instrumenti, piemēram, ES vispārējā mērķa AI prakses kodekss, Ķīnas AI drošības pārvaldības ietvars 2.0 un G7 Hirosimas AI procesa ziņošanas ietvars, kopā ar uzņēmumu vadītām iniciatīvām, parāda tendenci uz arvien standartizētāku pieeju pārredzamībai, izvērtēšanai un incidentu ziņošanai.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Tirgus dinamikas un AI attīstības temps rada papildu izaicinājumus. Sakarā ar konkurences spiedienu AI uzņēmumi var saskarties ar kompromisiem starp ātrāku produktu izlaišanu un ieguldījumiem riska mazināšanas pasākumos. Daudzi ar AI saistīti kaitējumi tiek arī nodoti trešajām pusēm, un juridiskā atbildība par tiem joprojām nav skaidra, savukārt pārvaldības procesi var būt lēni pielāgojami izmaiņām AI vidē.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Galvenie izaicinājumi politikas veidotājiem ietver prioritizēšanu starp dažādajiem riskiem, ko rada vispārējas nozīmes AI, un skaidrošanu, kuri dalībnieki AI vērtību ķēdē ir vislabākā pozīcijā, lai tos mazinātu. Šos izaicinājumus pastiprina ierobežota redzamība par to, kā praksē tiek identificēti, izvērtēti un pārvaldīti riski, kā arī sadrumstalota informācijas apmaiņa starp izstrādātājiem, ieviesējiem un infrastruktūras nodrošinātājiem.
>oldlace|black||11|15|br      


AI riska pārvaldība ietver virkni prakses, kuru mērķis ir identificēt, novērtēt un samazināt AI sistēmām saistīto risku iespējamību un ietekmes smagumu. Šīs prakses var īstenot AI izstrādātāji, izvietotāji, novērtētāji un regulatori. Piemēri ir draudu modelēšana, riska līmeņu noteikšana, red-teaming, audits un incidentu ziņošana. Šī sadaļa apraksta pašreizējās riska pārvaldības prakses, jaunos attīstības virzienus un atlikušos ierobežojumus.

Kopš 2025. gada sākuma ir izstrādātas vairākas jaunas starptautiskas iniciatīvas vispārējas nozīmes mākslīgā intelekta riska pārvaldībai, tostarp organizatoriskās pārskatāmības un riska ziņošanas ietvarstruktūras, kā arī normatīvie un pārvaldības ietvari.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Figūra 3.4: Četras riska pārvaldības sastāvdaļas
>white|black||9|11|br Četras vispārējas nozīmes AI riska pārvaldības metožu kategorijas: riska identificēšana; riska analīze un izvērtēšana; riska mazināšana; un riska pārvaldība. Tās veido iteratīvu un ciklisku procesu. Riska pārvaldība, kas attēlota centrā, veicina citu komponentu sekmes. Avots: International AI Safety Report 2026.


Atlikušās problēmas ietver ierobežotu standartizāciju, kas sarežģī atbilstības nodrošināšanu un novērtēšanu, kā arī ierobežotus pierādījumus par efektivitāti reālajā dzīvē. Turklāt institucionālie, kultūras un politiskie konteksti dažādās valstīs ir atšķirīgi, kas nozīmē, ka pieejas risku identificēšanai un pārvaldībai, tostarp pieļaujamajiem riska sliekšņiem, var atšķirties pa reģioniem. Šīs sadaļas diskusija par riska pārvaldības pieejām ir aprakstoša: tās mērķis ir sniegt informāciju AI ekosistēmas dalībniekiem par pašreizējām globālajām pieejām riska pārvaldībai. Ja pieejami, tiek apspriesti pierādījumi par šo pieeju efektivitāti un ierobežojumiem, taču politikas ieteikumi šī darba ietvaros netiek iekļauti.

###@ Riska pārvaldības komponentes

Riska pārvaldība ir iteratīvs process ar prakses un metodēm, kas aptver visu AI izstrādes un ieviešanas ciklu, bet darbojas saskaņoti (‡969). Riska pārvaldība vispārējas nozīmes AI var ietvert lomas ļoti plašam dalībnieku lokam, tostarp datu zinātniekiem, modeļu inženieriem, auditoriem, jomu ekspertiem, izpilddirektoriem, gala lietotājiem, ietekmētajām kopienām, trešo pušu piegādātājiem, politikas veidotājiem, valdībām, standartizācijas organizācijām un pilsoniskās sabiedrības organizācijām (‡970, ‡971, ‡972). Līderošie riska pārvaldības standarti bieži ir savietojami, taču izmanto atšķirīgu terminoloģiju, lai aprakstītu riska pārvaldības elementus (‡973, ‡974). Parasti tiem ir četri savstarpēji saistīti komponenti (Figūra 3.4): riska identificēšana; riska analīze un izvērtēšana; riska mazināšana; un riska pārvaldīšana (‡970, ‡973, ‡975, ‡976). Zemāk esošās tabulas sniedz ilustratīvus piemērus attiecīgajām metodēm, paņēmieniem un rīkiem. Prakses turpina attīstīties, tāpēc tabulas nav izsmeļošas, un piemērojamība dažādos kontekstos var atšķirties.

###@ Riska identificēšana

Riska identifikācija ir process, kurā tiek atrasti, atpazīti un aprakstīti riski. Visaptveroša riska identifikācija parasti ietver spēju virzītas novērtēšanas pieejas, kas pārbauda, vai modeļiem ir konkrētas bīstamas spējas (‡977), kā arī riska modelēšanu (‡978) un prognozēšanu (‡715*), kuras izmanto, lai izpētītu esošos un jaunos riskus. 3.1. tabula sniedz dažādus riska identifikācijas prakses piemērus. Riska identifikācija arī balstās uz sadarbību ar atbilstošiem ekspertiem un kopienām, lai izprastu plašāku kontekstu, kā riski rodas (‡979, ‡980). Tādi mehānismi kā kļūdu atlīdzības programmas var atbalstīt šo procesu, motivējot identificēt iepriekš nezināmas ievainojamības (‡981) (3.1. tabula). Viens no galvenajiem riska identifikācijas mērķiem ir aptvert gan labi zināmus un labi izprastus riskus, gan arī iespējamos nākotnes riskus, kas joprojām ir neskaidri vai vāji raksturoti (‡982). Tas ir īpaši svarīgi vispārējas nozīmes AI gadījumā, kur daudzi riski vēl nav pilnībā saprasti vai novērojami (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bug bounty programmas
  Būg-bounty programmas vai ievainojamību paziņošanas programmas motivē cilvēkus atrast un ziņot par ievainojamībām AI sistēmās. Vairāki izstrādātāji ir ieviesuši būg-bounty programmas (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ekspertu konsultācija
  Dinamisku jomu eksperti, lietotāji un ietekmētās kopienas sniedz ieskatus iespējamajos riskos. Ir izstrādes stadijā esošas vadlīnijas par līdzdalīgu un iekļaujošu AI (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Zivs skeleta (Išikavas) diagramma
  Zivskaula diagrammas ir labi izveidoti cēloņu analīzes rīki, un pētnieki ir ierosinājuši izmantot tās mākslīgā intelekta riska incidentu strukturētai analīzei (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Prognozēšana
  Prognozēšana ir process, kas paredz nākotnes notikumus vai tendences, pamatojoties uz pagātnes un pašreizējo datu analīzi. To ir izmantojuši, lai salīdzinātu dažādu, piemēram, ekonomisko iznākumu relatīvo varbūtību, pateicoties progresīvai AI (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riska taksonomija
  Riska taksonomijas ir veids, kā kategorizēt un organizēt riskus vairākās dimensijās. Ir vairākas, kas izklāsta riskus vispārējas nozīmes mākslīgajā intelektā (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Scenāriju plānošana
  Scenāriju plānošana ietver ticamu nākotnes scenāriju izstrādi un analīzi, kā riski materializējas. To ir izmantoti, lai izpētītu mākslīgā intelekta modeļu (‡989) riskus un to ietekmi.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Draudzie modelēšana
  Draududu modelēšana ir process, kurā identificē draudus un ievainojamības konkrētai sistēmai. Daudzi AI izstrādātāji uzsver tās izmantošanu, lai prognozētu iespējamos AI sistēmu ļaunprātīgas izmantošanas scenārijus (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.1. tabula: Riska identificēšanas piemēri vispārējas nozīmes AI riska pārvaldībā
>white|black||9|11|br Piemēra metodes AI riska identificēšanai ir uzskaitītas alfabētiskā secībā. Iekļautās metodes
ir izstrādātas, lai atbalstītu riska identificēšanu daudziem dažādiem riska veidiem, tostarp riskiem saistībā ar ļaunprātīgu izmantošanu, riskiem saistībā ar darbības traucējumiem un sistēmiskiem riskiem. Ņemot vērā ģenerālpielietojuma AI riska pārvaldības agrīno attīstības posmu, ne visas metodes būs piemērotas katram AI izstrādātājam vai izvietotājam.


>white|orangered|left|14|15.5|bb Draudu modelēšana un riska taksonomijas ir nozīmīgas riska identifikācijas metodes

Divas ievērojamas metodes vispārējas nozīmes AI risku identificēšanai ir draudu modelēšana un risku taksonomijas. International AI Safety Report 2026 (Starptautiskais AI drošības ziņojums 2026) piedāvā draudu modelēšanu kā strukturētu procesu, lai kartētu, kā AI saistītie riski var īstenoties, savukārt risku taksonomijas klasificē riskus. Piemēram, Meta izmanto draudu modelēšanas vingrinājumus, lai paredzētu iespējamos savas AI modeļu ļaunprātīgas izmantošanas scenārijus (‡990), un Anthropic iekļauj draudu modelēšanu savā ASL-3 Deployment Standard (‡991). AI riska un bīstamību taksonomijas, kas uzskaita riska kategorijas un piemērus, tikpat labi var kalpot kā sākumpunkts, lai konceptualizētu, identificētu un precizētu būtiskos riskus, kas saistīti ar vispārējas nozīmes AI konkrētās lietojuma jomās (‡906, ‡988, ‡992, ‡993).

###@ Riska analīze un novērtēšana

Riska analīze un novērtēšana ir process, kurā nosaka AI modeļa vai sistēmas riska līmeni un salīdzina to ar noteiktiem kritērijiem, lai izvērtētu pieņemamību vai nepieciešamību pēc mazināšanas (‡994, ‡995, ‡996, ‡997). Tā ietver tādas prakses kā modeļa veiktspējas mērīšana uz etaloniem (‡998) un novērtējumiem (‡176, ‡715), sarkano komandu (red-teaming) vingrinājumu veikšana (‡999*), ietekmes novērtējumi (‡1000) un auditi (‡1001, ‡1002). Skatiet Tabula 3.2 piemērus vispārējas nozīmes AI riska analīzei un novērtēšanai. Metodes ir izstrādātas, lai vienlaikus atbalstītu analīzi un novērtēšanu daudziem dažādiem riska veidiem.

Galvenie riska analīzes un novērtēšanas mērķi ir veikt modeļa spēju un ievainojamību novērtēšanu (‡1003), izmantot noturīgu riska modelēšanu, lai pieņemtu lēmumus par riska sliekšņiem (‡1004, ‡1005), un izprast, kā AI sistēmas tiek izmantotas praksē, lai izvērtētu turpmākās (lejupējās) sabiedriskās ietekmes (‡869, ‡904, ‡905, ‡1006). Riska analīzes un novērtēšanas procesus bieži uzskata par tādiem, kas daudz biežāk spēj identificēt riskus, ja tie ietver neatkarīgu izvērtēšanu (‡1001, ‡1007), balstās uz starpnozaru kompetenci (‡1008) un iekļauj dažādus skatpunktus no vairākām jomām un disciplīnām, kā arī no skartajām kopienām (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Auditi
  Auditi ir formālas AI modeļu veiktspējas un ietekmes pārbaudes un/ vai organizācijas atbilstības pārbaudes standartiem, politikām un procedūrām, ko veic organizācijas iekšienē vai ārēja puse. AI auditi ir strauji augoša joma, un pastāv daudzi rīki un prakses AI modeļu un AI modeļu izstrādātāju prakses auditēšanai (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Etaloni
  Benchmarks ir standartizēti, bieži vien kvantitatīvi testi vai metrikas, ko izmanto, lai novērtētu un salīdzinātu AI sistēmu veiktspēju pēc fiksēta uzdevumu kopuma, kas izstrādāts, lai atspoguļotu reālu lietojumu (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bowtie metode
  Lāpstveida (bowtie) metode ir labi zināma metode, lai vizualizētu, kur kontrolēm var pievienot, lai mazinātu riska notikumus. Tā nodrošina skaidru nošķīrumu starp proaktīvu un reaktīvu riska pārvaldību (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Delphi metode
  Delphi metode ir grupas lēmumu pieņemšanas paņēmiens, kas izmanto virkni anketu, lai iegūtu vienprātību no ekspertu paneļa (‡1020, ‡1021). Tā ir izmantota, lai palīdzētu izpētīt iespējamās nākotnes ar progresīvu AI (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Lauka pārbaude
  Lauka testēšana novērtē AI sistēmas veiktspēju un ietekmi reālā, operacionālā vidē. Daži pētījumi uzsver lauka testēšanu kā papildinājumu modeļa novērtēšanai, lai izvērtētu reālas pasaules iznākumus un sekas (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ietekmes novērtējums
  Ietekmes novērtējumi izvērtē tehnoloģijas vai projekta iespējamo ietekmi. Tas var ietvert ietekmes kvantificēšanu, apkopošanu un prioritizēšanu. Piemēram, ES AI akts nosaka, ka augsta riska AI sistēmu izstrādātājiem ir jāveic Pamattiesību ietekmes novērtējumi (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modeļa novērtēšana
  Modeļa novērtējumi ietver procesus un testus, lai novērtētu un izmērītu AI modeļa veiktspēju konkrētā uzdevumā. Ir daudz dažādu AI novērtējumu, lai novērtētu dažādas iespējas un riskus, tostarp drošību, kiberdrošību un sociālo ietekmi (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Varbūtiskā riska novērtēšana
  Varbūtību riska novērtējums ir metodoloģija risku, kas saistīti ar sarežģītām sistēmām vai procesiem, izvērtēšanai, kura ietver nenoteiktību. Tas ir pielāgots uzlabotām AI sistēmām (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sarkankomandēšana
  Red-teaming ir vingrinājums, kurā cilvēku grupa vai automatizētas sistēmas iztēlojas sevi kā pretinieku un uzbrūk organizācijas tehnoloģiskajām sistēmām, lai identificētu ievainojamības. Daudziem AI uzņēmumiem ir iekšējas prakses red-teaming veikšanai AI sistēmām (‡458, ‡1028). Red-teaming var veikt arī organizāciju ārpusē esoši dalībnieki. Šīm komandām ir tādi izaicinājumi kā ierobežota piekļuve, taču tās var arī sniegt atšķirīgus ieskatus (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riska matricas
  Riska matricas ir vizuāls rīks, kas palīdz noteikt riska prioritātes, ņemot vērā to rašanās iespējamību un iespējamo ietekmi (‡1027). Daži AI izstrādātāji savos Frontier AI Safety Frameworks (‡1029*) iekļauj pamata riska matricas.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riska sliekšņi/ riska līmeņi
  Riska sliekšņi vai līmeņi ir kvantitatīvi vai kvalitatīvi ierobežojumi, kas nošķir pieņemamos riskus no nepieņemamiem riskiem un iedarbina konkrētas riska pārvaldības darbības, kad tie tiek pārsniegti. Vispārējas nozīmes AI tie tiek noteikti, kombinējot spējas, ietekmi, skaitļošanas resursus, sasniedzamību un citus faktorus (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riska tolerance
  Riska tolerances attiecas uz riska līmeni, ko organizācija ir gatava pieņemt. AI gadījumā riska tolerances bieži tiek noteiktas netieši, izmantojot uzņēmuma politikas un prakses, savukārt dažās regulatīvajās režīmos nepārprotami tiek definēti nepieņemami riski un tiem tiek piesaistītas juridiskas sekas (‡1032). Daži uzņēmumi apraksta savu riska toleranci jauna modeļa robežriska izteiksmē; proti, apmēru, kādā modelis kontrafaktiski palielina risku salīdzinājumā ar risku, ko jau rada esošie modeļi vai citas tehnoloģijas (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Drošības pamatojums
  Drošības lieta ir strukturēts arguments, ko pamato pierādījumi, ka sistēmu konkrētā kontekstā ir pieņemami droši ekspluatēt. Jaunākā literatūra (‡1037, ‡1038, ‡1039) ir pētījusi drošības lietas attiecībā uz progresīvām AI sistēmām, un noteikti Frontier AI Safety Frameworks tās ir norādījušas (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sistēmas drošības analīze
  Sistēmas drošības analīze izceļ atkarības starp komponentēm un sistēmu, kuras daļa tās ir, lai paredzētu, kā sistēmas līmeņa apdraudējumi var rasties no komponentu vai procesu kļūmēm, vai mijiedarbībām starp apakšsistēmām, cilvēkfaktoriem un vides apstākļiem. Pieejas, kas literatūrā piemērotas AI sistēmām, ietver sistēmu teorētisko procesu analīzi (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.2. tabula: Riska analīze/novērtējums vispārējas nozīmes AI riska pārvaldībā
>white|black||9|11|br Piemēra metodes AI riska analīzei/novērtēšanai, uzskaitītas alfabētiskā secībā. Ņemot vērā ģenerāliska nozīmes AI riska pārvaldības agrīno attīstības stadiju, ne visas metodes būs piemērotas katram AI izstrādātājam vai izvietotājam.


>white|orangered|left|14|15.5|bb Bieži izmantoti riska analīzes rīki ietver etalonus un modeļu izvērtējumus

Etaloni un modeļu izvērtējumi ir standartizēti testi, lai novērtētu vispārējas nozīmes AI sistēmu veiktspēju konkrētos uzdevumos. Pētnieki ir izstrādājuši plašu etalonu un izvērtējumu klāstu, tostarp kopas ar izaicinošiem daudzizvēles jautājumiem, programmatūras izstrādes problēmām un ar darbu saistītus uzdevumus simulētās biroja vidēs (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Kaitīgu spēju izvērtējumi (‡715) tiek izmantoti, lai noteiktu, vai vispārējas nozīmes AI modelim vai sistēmai piemīt īpaši bīstamas zināšanas vai prasmes, piemēram, spēja palīdzēt kiberuzbrukumos (sk. §2.1.3. Kiberuzbrukumi).

Ļoti nozīmīgi uzņēmumu un valdību lēmumi par modeļu izlaišanu daļēji balstās uz šiem novērtējumiem (‡1050, ‡1051, ‡1052). Tomēr etaloni būtiski atšķiras pēc kvalitātes un tvēruma (‡998, ‡1003), un to derīgumu var būt grūti izvērtēt, ņemot vērā daudzos trūkumus etalonvērtēšanas praksē (‡902, ‡909, ‡1003, ‡1053*). Piemēram, etaloni var kļūt “piesātināti” – kad daudzu modeļu rādītāji tuvojas augstākajam rādītājam – tādējādi tie vairs būtiski neatšķir modeļus. Modeļi arī arvien biežāk var identificēt noteiktus uzdevumus kā novērtējumus un demonstrēt atšķirīgu uzvedību nekā līdzīgos uzdevumos izvietošanas kontekstos “situatīvās apzināšanās” dēļ (skat. §2.2.2. Kontroles zudums). Visbeidzot, etaloniem un novērtējumiem ir labi dokumentēti ierobežojumi: jo īpaši tie nespēj aptvert riskus, kas saistīti ar vispārējas nozīmes AI izmantošanu jaunās jomās un jauniem uzdevumiem, jo pārbaudes apstākļi dažādās pakāpēs atšķiras no reālās izmantošanas (‡913) (skat. §1.2. Pašreizējās iespējas un §3.1. Tehniskie un institucionālie izaicinājumi).

>white|orangered|left|14|15.5|bb Red-teaming ļauj veikt detalizētākus risku novērtējumus konkrētajai jomai

Vēl viena izplatīta metode risku izvērtēšanai ir “red-teaming”. “Red team” ir vērtētāju grupa, kuras uzdevums ir meklēt ievainojamības, ierobežojumus vai ļaunprātīgas izmantošanas potenciālu. Red-teaming var būt domēnam specifisks un to var veikt jomas eksperti, vai arī tas var būt atvērts, lai izpētītu jaunus riska faktorus. Piemēram, red team var pētīt “jailbreaking” uzbrukumus, kas apiet modeļa drošības ierobežojumus (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). Atšķirībā no etaloniem (benchmarks), galvenā red-teaming priekšrocība ir tā, ka red teams var pielāgot savus izvērtējumus konkrētai testējamai sistēmai. Piemēram, red teams var izstrādāt pielāgotas ievades, lai identificētu sliktākās iespējamās uzvedības, ļaunprātīgas izmantošanas iespējas un neparedzētas kļūmes. Tomēr tas var prasīt īpašu piekļuvi modeļiem un var neizdoties atklāt būtiskas riska klases (‡999, ‡1028).

Svarīgi ir tas, ka identificētu risku neesamība nenozīmē, ka šie riski ir zemi: iepriekšējie darbi rāda, ka kļūdas bieži izvairās no atklāšanas, īpaši tad, ja sarkanās komandas rīcībā ir ierobežota piekļuve vai resursi (‡1060). Pētījumi arī ir apšaubījuši, vai sarkanā teimošana (red-teaming) spēj radīt uzticamus un reproducējamus rezultātus (‡1061). Sarkanās komandas sastāvs un sarkanās komandas dalībniekiem sniegtie norādījumi (‡1062), uzbrukumu kārtu skaits (‡1063) un modeļa piekļuve rīkiem (‡1064, ‡1065) var būtiski ietekmēt iznākumus, tostarp to, kāds risks iegūst segumu aptvertajā riska virsmā. Visaptverošas vadlīnijas par sarkano teimošanu (red-teaming) ir vērstas uz dažu no šiem izaicinājumiem risināšanu (‡1066).

###@ Riska mazināšana

Riska mazināšana ir process, kurā tiek noteikta prioritāte, izvērtēti un īstenoti kontroles pasākumi un pretpasākumi, lai samazinātu identificētos riskus. Piemēri ir piekļuves kontroles (‡991), nepārtraukta uzraudzība (‡986) un nosacījumu “ja-tad” saistības (‡700). Riska mazināšana rada būtisku jautājumu: kāds ir pieņemams riska līmenis? Jaunākie ietvari un uzņēmumu politikas ir sākušas formalizēt “riska akcepta” kritērijus (‡965, ‡1040). Tomēr piemērotu robežvērtību noteikšana joprojām ir sarežģīta, īpaši riskiem ar plašu sabiedrisku ietekmi (‡986, ‡1067). Pašlaik nepastāv izveidots mehānisms, lai pirms izlaišanas validētu izstrādātāju pieņemtos riska akcepta lēmumus (‡1005).

Zemāk tabulā 3.3 aprakstītie riska mazināšanas paņēmieni ir pielāgojami un var mazināt dažāda veida riskus, tostarp dažus neparedzētus riskus. Tabulā nav iekļauti tādi tehniski mazināšanas paņēmieni kā pretinieku (adversarial) apmācība, satura filtri un ķēdes domāšanas uzraudzība (chain-of-thought monitoring). Tie ir aplūkoti sadaļā §3.3. Tehniskie drošības pasākumi un uzraudzība, kā arī visā Pārskatā sadaļās ar “Mazināšanas līdzekļi” (Mitigations) katram riskam 2. sadaļas §2. Risks.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pieļaujamās izmantošanas politikas
  Pieņemamas izmantošanas politika ir noteikumu un vadlīniju kopums atbildīgai, ētiskai un likumīgai AI modeļu izmantošanai. Ir ierasts, ka AI izstrādātāji kopā ar jaunu modeļu izlaišanu publicē pieņemamas izmantošanas politikas, kā arī aizliegtas izmantošanas politikas (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Piekļuves kontrole / lietotāju pārbaude
  Piekļuves kontrole ietver politiku un noteikumu izmantošanu, lai ierobežotu piekļuvi AI modeļiem, datiem un sistēmām, pamatojoties uz lietotāju lomām, atribūtiem un citiem nosacījumiem, lai novērstu nesankcionētu izmantošanu, manipulāciju vai datu noplūdes. AI uzņēmumi bieži deaktivē kontus, kas konstatēti iesaistāmies noziedzīgā darbībā (‡486), un iekļauj lietotāju pārbaudi un Know-Your-Customer izvērtējumus (KYC), lai nodrošinātu, ka modeļus izmanto tikai uzticami aktori (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Uzvedības/modela specifikācija
  AI uzvedības specifikācija ir dokuments, kas nosaka, kā AI modelim vajadzētu uzvesties dažādās situācijās. Tā kalpo kā plānojums AI saskaņošanai un drošībai, virzot modeļa izstrādi, apmācību, izvērtēšanu un izvades. Vairākas AI kompānijas izmanto modeļa specifikāciju dokumentus un publisko vismaz to daļas (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pastāvīga uzraudzība
  Nepārtraukta uzraudzība ir nepārtraukts, automatizēts process, kurā novēro, analizē un kontrolē ekspluatācijā esošas AI sistēmas, izseko to veiktspēju un ierobežo to uzvedību, lai nodrošinātu uzticamību, efektivitāti un drošību. Ir pieejami daudzi rīki nepārtrauktai uzraudzībai (‡1073*) , kā arī metodes, kas to atbalsta
AI novērojamība (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Aizsardzība ar slāņiem
  Aizsardzība dziļumā ir ideja, ka var īstenot vairākus neatkarīgus un pārklājošus aizsardzības slāņus, lai, ja viens neizdodas, citi joprojām būtu efektīvi (‡1075, ‡1076). Vairākas Frontier AI Safety Frameworks atsaucas uz to (piem. (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ekosistēmas uzraudzība
  Šis ir process, kurā tiek uzraudzīta plašāka AI ekosistēma, tostarp skaitļošanas un aparatūras uzskaite, modeļu izcelsme, datu izcelsme un izmantošanas modeļi. Pētnieciskajā literatūrā tiek apspriesta šāda uzraudzība saistībā ar riskiem, ko rada vispārējas nozīmes AI (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb “Ja-tad” saistības
  Nosacījuma "ja-tad" saistības ir tehnisku un organizatorisku protokolu kopums un apņemšanās pārvaldīt riskus, AI modeļiem kļūstot arvien spējīgākiem. Vairāki AI izstrādātāji izmanto šāda veida saistības kā daļu no saviem Frontier AI Safety Frameworks (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sarkanas līnijas vai aizliegumi
  Sarkanās līnijas ir konkrētas robežas, kas izteiktas kā spējas, ietekme vai lietošanas veidi. Šis jēdziens parādās publiskos paziņojumos un iniciatīvās, kā arī normatīvos aizliegumos (‡1079, ‡1080, ‡1081). Literatūrā arī tiek norādīti sarkano līniju pieejas ierobežojumi, tostarp grūtības panākt vienprātību un nodrošināt izpildāmību.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Izlaišanas un izvietošanas stratēģijas
  Vispārējas nozīmes AI izlaišanas un izvietošanas stratēģijas var ietvert pakāpeniskas izlaišanas vai API piekļuves izmantošanu, lai ļautu pieejam vairāk mazināšanas iespēju gadījumā, ja notiek ļaunprātīga izmantošana vai neparedzēts kaitējums (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabula 3.3: Riska mazināšana vispārējas nozīmes AI riska pārvaldībā
>white|black||9|11|br Piemēru metodes AI riska mazināšanai, kas uzskaitītas alfabētiskā secībā. Metodes ir izstrādātas, lai vienlaikus atbalstītu riska mazināšanu daudziem dažādiem riska veidiem, tostarp riskus no ļaunprātīgas izmantošanas, riskus no darbības traucējumiem un sistēmiskos riskus. Ņemot vērā vispārējas nozīmes AI riska pārvaldības sākotnējo stadiju, ne visas metodes būs piemērotas katram AI izstrādātājam vai izvietotājam.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Figūra 3.5: “Šveices siera diagramma”, kas ilustrē aizsardzību daudzslāņu (defense-in-depth) pieejā
>white|black||9|11|br Vairāki aizsardzības slāņi var kompensēt trūkumus atsevišķos slāņos. Pašreizējām mākslīgā intelekta riska pārvaldības metodēm ir trūkumi, taču to kombinēšana var nodrošināt daudz spēcīgāku aizsardzību pret riskiem. Avots: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Aizsardzība dziļumā un izlaiduma stratēģijas ir svarīgi mazināšanas rīki

“aizsardzība daudzslāņos” modelis var atbalstīt vispārējas nozīmes mākslīgā intelekta (AI) riska pārvaldību. Šajā kontekstā “aizsardzība daudzslāņos” attiecas uz tehnisku, organizatorisku un sabiedrisku pasākumu kombināciju, kas tiek piemērota dažādos izstrādes un ieviešanas posmos (3.5. att.). Tas nozīmē neatkarīgu aizsargpasākumu slāņu izveidi, lai, ja viens slānis neizdodas, citi slāņi joprojām var novērst kaitējumu. Bieži minēts “aizsardzības daudzslāņos” modeļa piemērs ir virkne preventīvu pasākumu, kas tiek īstenoti infekcijas slimību novēršanai. Vakcīnas, maskas un roku mazgāšana, cita starpā, kombinācijā var būtiski samazināt inficēšanās risku, pat ja neviena no šīm metodēm pati par sevi nav 100% efektīva (‡1083*). Vispārējas nozīmes AI gadījumā “aizsardzība daudzslāņos” ietver kontroles, kas neatrodas pašā AI modelī, bet gan plašākā ekosistēmā. Tas ietver (piemēram) kontroles uz materiāliem, kas nepieciešami bioloģiska uzbrukuma īstenošanai, piemēram, reaģentiem (‡1084, ‡1085). Tomēr “aizsardzības daudzslāņos” pasākumi galvenokārt vērsti uz riskiem, kas saistīti ar negadījumiem, darbības traucējumiem un ļaunprātīgu izmantošanu, un tiem var būt mazāka nozīme sistēmisku risku pārvaldībā (skat. §3.5. Sabiedrības noturības stiprināšana).

Uzņēmuma izlaišanas un izvietošanas stratēģija ir svarīga riska mazināšanas sastāvdaļa. Lēmumi par to, kā modeļi tiek darīti pieejami lietotājiem, var būtiski ietekmēt riska pakļautību (‡1082). Dažādas izlaišanas un izvietošanas iespējas ietver pakāpenisku izlaišanu ierobežotām lietotāju grupām, piekļuvi ar kontrolētiem tiešsaistes pakalpojumiem (piemēram, API) un licencēšanas līgumu un pieņemamas izmantošanas politiku izmantošanu, kas juridiski aizliedz noteiktas kaitīgas lietojumprogrammas (‡176, ‡1086, ‡1087). §3.4. Atvērtā svaru modeļi detalizētāk apspriež, kā modeļa svaru izlaišana ietekmē riskus.

###@ Riska pārvaldība

Riska pārvaldība ir process, kurā riska pārvaldības izvērtējumi, lēmumi un darbības tiek saistītas ar organizācijas vai citas vienības stratēģiju un mērķiem (‡1088, ‡1089). 3.4. tabula sniedz pārskatu par biežāk lietotajām riska pārvaldības metodēm. Kā parādīts 3.4. attēlā, riska pārvaldību var saprast kā riska pārvaldības kodolu, jo tā atvieglo citu riska pārvaldības komponentu efektīvu darbību. Tā nodrošina atbildību, pārskatāmību un skaidrību, kas atbalsta pamatotus riska pārvaldības lēmumus. Riska pārvaldība var ietvert tādas prakses kā incidentu ziņošana (‡1090), riska atbildības sadalīšana (‡965) un trauksmes cēlēju aizsardzība (‡1091). Plašākā nozīmē riska pārvaldība var ietvert vadlīnijas, ietvarus, likumdošanu, regulējumus, valsts un starptautiskos standartus, kā arī apmācību un izglītojošas iniciatīvas. Galvenais riska pārvaldības mērķis ir izveidot organizācijas politikas un mehānismus, kas precizē, kā riska pārvaldības atbildības tiek sadalītas organizācijā vai citā vienībā, lai atbalstītu atbilstošu uzraudzību un atbildību (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dokumentācija
  Dokumentācijas prakses palīdz izsekot būtisku informāciju par AI sistēmām, piemēram, apmācības datiem, dizaina izvēlēm, paredzētajiem izmantošanas mērķiem, ierobežojumiem un riskiem. “Model cards” un “system cards”, kas sniedz informāciju par to, kā AI modelis vai sistēma tika apmācīta un novērtēta, ir nozīmīgu AI dokumentācijas labāko prakšu piemēri (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Incidentu paziņošana
  Incidentu ziņošana ir process, kurā sistemātiski dokumentē un dalās ar gadījumiem, kuros, izstrādājot vai ieviešot AI, ir nodarīts tiešs vai netiešs kaitējums. Ir vairākas platformas, kas atvieglo incidentu ziņošanu par AI (‡1096, ‡1097), un ietvari, kas nodrošina efektīvāku AI incidentu ziņošanu (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riska pārvaldības ietvari
  Riska pārvaldības ietvari ir organizatoriski plāni, lai samazinātu nepilnības riska pārklājumā, koordinētu dažādas riska pārvaldības aktivitātes un ieviestu pārbaudes un līdzsvaru. Ietvari, kas ir specifiski vispārējas nozīmes AI (‡986, ‡1098), bieži atsaucas uz citām šajā sadaļā minētajām attiecīgajām izmaiņām.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riska reģistrs
  Riska reģistrs ir dažādu risku repozitorijs, kas ietver to prioritizēšanu, atbildīgos un mazināšanas plānus. Tie ir salīdzinoši izplatīti daudzās nozarēs, tostarp kiberdrošībā (‡1099), un dažkārt tiek izmantoti, lai izpildītu normatīvās atbilstības prasības.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riska atbildības sadalījums
  Riska pārvaldības lomu un pienākumu piešķiršana organizācijā var strukturēt iekšējo uzraudzību attiecībā uz lēmumu pieņemšanu (‡1002, ‡1093). Šādi izkārtojumi atspoguļojas dažās pārvaldības struktūrās, tostarp ES Vispārējā mērķa AI prakses kodeksā (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pārskatāms atklātības pārskati
  Pārredzamības pārskati raksturo AI uzņēmuma riska pārvaldības prakses, publiski izpaužot noteiktu informāciju vai daloties ar dokumentāciju nozares grupās vai valdības iestādēs. Piemēram, daudzi AI uzņēmumi iesniedz Hirosimas AI procesa (HAIP) pārredzamības pārskatus (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Virsinieka aizsardzība
  Tā kā liela daļa AI izstrādes notiek aiz slēgtām durvīm, dažos pārvaldības ietvaros ir iekļautas ziņotāju aizsardzības garantijas, lai nodrošinātu iespējamo risku paziņošanu iestādēm (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.4. tabula: Riska pārvaldība vispārējas nozīmes AI riska pārvaldībā
>white|black||9|11|br Piemēra metodes AI riska pārvaldībai, kas uzskaitītas alfabētiskā secībā. Iekļautās metodes ir izstrādātas, lai vienlaikus atbalstītu riska pārvaldību daudziem dažādiem riska veidiem, tostarp riskiem ļaunprātīgas izmantošanas dēļ, riskiem darbības traucējumu dēļ un sistēmiskiem riskiem. Ņemot vērā vispārīga mērķa AI riska pārvaldības sākotnējo (nākotnes) raksturu, ne visas metodes būs piemērotas katram AI izstrādātājam vai ieviesējam.


>white|orangered|left|14|15.5|bb Dokumentēšana un pārredzamība ir riska pārvaldības komponentes

Dokumentācijas un institucionālās pārredzamības mehānismi, kā arī informācijas apmaiņas prakses, atvieglo ārējo pārbaudi un atbalsta centienus pārvaldīt riskus, kas saistīti ar vispārējas nozīmes AI (‡1101, ‡1102). Ir kļuvis par ierastu praksi publicēt pirms izvietošanas testu rezultātus “model card” jeb “modeļa kartē” vai “system card” jeb “sistēmas kartē”, kopā ar pamatinformāciju par modeli vai sistēmu, tostarp ar to, kā tas tika apmācīts, un kādi ir tā iespējamie ierobežojumi (‡1094, ‡1095). Daži izstrādātāji arī publicē pārredzamības ziņojumus, kuros plašāk iekļautas to riska pārvaldības prakses (‡1103). Citi dokumentācijas un pārredzamības elementi ietver uzraudzību un incidentu ziņošanu (‡176, ‡1083*, ‡1103), kā arī informācijas apmaiņu, ko var veicināt trešās puses, piemēram, Frontier Model Forum. Dažas regulatīvās sistēmas, piemēram, ES AI Akts vai Kalifornijas “Transparency in Frontier Artificial Intelligence Act” - Senate Bill No. 53 (SB 53) (‡1081, ‡1104), dažos gadījumos uzliek pienākumu veikt informācijas apmaiņu par vispārējas nozīmes AI riskiem.

>white|orangered|left|14|15.5|bb Līderības apņemšanās un motivējoši pasākumi veido riska pārvaldības praksi

Organizācijas kultūra, vadības struktūra un stimuli dažādos veidos ietekmē riska pārvaldības centienus (‡1105). Vadības apņemšanās un stimulēšanas struktūras bieži vien ir būtiskas tam, kā praksē darbojas riska pārvaldības politikas. Dažiem izstrādātājiem ir iekšējie lēmumu pieņemšanas paneļi, kas apspriež, kā droši un atbildīgi projektēt, izstrādāt un pārskatīt jaunas AI sistēmas. Uzraudzības un konsultatīvās komitejas, uzticības struktūras vai AI ētikas padomes var arī kalpot kā riska pārvaldības vadlīniju un organizācijas uzraudzības mehānismi (‡1092*, ‡1106, ‡1107, ‡1108). Pētnieki ir apgalvojuši, ka problēmas ar brīvprātīgu pašregulāciju nozīmē, ka trešo pušu audits, verifikācija un standartizācija varētu palīdzēt stiprināt vispārējas nozīmes AI riska pārvaldību (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Organizācijas riska pārvaldības, pārskatāmības un riska ziņošanas sistēmas

Vairākas jaunas iniciatīvas koncentrējas uz riska pārvaldības procesiem, dokumentēšanu un pārredzamību. Pašreizējā veidā ES Vispārējā mērķa AI kodeksa prakse darbojas kā brīvprātīgs ietvars, lai vadītu pārredzamības, autortiesību un drošības un kiberdrošības prakses, kas palīdz nodrošināt atbilstību ES AI likuma noteikumiem par vispārēja mērķa AI (‡965). No 2025. gada decembra vairāk nekā divdesmit uzņēmumi† ir parakstījuši. G7 Hirosimas AI procesa (HAIP) ziņošanas ietvars (‡1100) ir pirmais starptautiskais ietvars brīvprātīgai publiskai ziņošanai par organizāciju riska pārvaldības praksēm progresīviem AI sistēmu risinājumiem. Vismaz 20 izstrādātāji ir publicējuši publiskus pārredzamības pārskatus, kas aptver riska identificēšanu, novērtēšanas metriku, mazināšanas stratēģijas un datu drošības procesus.

AI izstrādātāji ir pieņēmuši brīvprātīgas pārredzamības saistības. Ķīnā 17 Ķīnas AI uzņēmumu apņemšanās, kuras koordinēja Ķīnas AI nozares alianse (AI Industry Alliance of China), tika izziņotas 2024. gada decembrī (‡1113) un atjauninātas 2025. gadā (‡1114). 2024. gada maijā AI Seulas samitā Dienvidkorejā 16 AI izstrādātāji no vairākām valstīm parakstīja brīvprātīgas saistības publicēt Frontier AI Safety Frameworks saviem spējīgākajiem modeļiem un sistēmām, kā arī ieviest riska pārvaldības prakses visos modeļa izstrādes un izvietošanas posmos (‡1052).

    Piezīme † -- Parakstītāji no 2025. gada decembra ietver: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing un WRITER.

>white|orangered|left|14|15.5|bb Frontier AI drošības ietvari ir kļuvuši par ievērojamu organizatorisku pieeju AI riska pārvaldībai

Kopš 2023. gada vairāki progresīvo AI izstrādātāji ir brīvprātīgi publicējuši dokumentus, kuros aprakstīts, kā viņi plāno identificēt un reaģēt uz nopietniem riskiem no savām visprogresīvākajām sistēmām. Šie Frontier AI Safety Frameworks (progresīvās AI drošības ietvari) apraksta, kā AI izstrādātājs plāno novērtēt, uzraudzīt un kontrolēt savus visprogresīvākos AI modeļus un sistēmas pirms un darbības laikā izvietošanas laikā. Šiem ietvariem ir daudz līdzību, taču tie atšķiras būtiskos aspektos (‡1115, ‡1116). Lielākā daļa koncentrējas uz riskiem, kas saistīti ar ķīmiskajiem, bioloģiskajiem, radioloģiskajiem un kodolapdraudējumiem (CBRN), progresīvām kiberspējām un progresīvu autonomu rīcību (‡1115, ‡1117). Mazākums ietvaru aplūko papildu riska jomas, piemēram, nelikumīgu diskrimināciju mērogā un bērnu seksuālu izmantošanu.

Vairāki izstrādātāji 2025. gadā atjaunināja savus ietvarus, pievienojot jaunas sadaļas par kaitīgu manipulāciju, nepareizas atbilstības (misalignment) risku un autonomu replikāciju un adaptāciju (‡1078, ‡1118). Lai gan daudzi ietvari apraksta līdzīgas riska pārvaldības pieejas – tostarp draudu modelēšanu, “red-teaming” un bīstamu spēju novērtējumus – tie atšķiras savās riska līmeņu un sliekšņu definīcijās, novērtējumu biežumā, buferos starp novērtējumiem un sliekšņiem, kā arī savu mazināšanas saistību visaptverošībā (piemēram, vai tās ietver modeļa svaru dzēšanu, nevis tikai izstrādes apturēšanu) (‡1115, ‡1119). Lai iegūtu vairāk informācijas, skatiet Tabula 3.5.

>white|orangered|left|14|15.5|bb Daudzas darbības Frontier AI drošības ietvarstruktūrās balstās uz nosacījuma “ja-tad” saistībām.

Svarīga daļa no Frontier AI Safety Frameworks ir “if-then commitments”. Tās ir nosacītas procedūras, kas aktivizē konkrētas darbības, kad AI modeļi un sistēmas sasniedz iepriekš definētas spēju robežvērtības (‡1120). Piemēram, “if-then” apņemšanās varētu noteikt, ka, ja tiek konstatēts, ka modelim ir spēja jēgpilni palīdzēt iesācējiem izveidot un izvietot CBRN ieročus, tad izstrādātājs ieviesīs uzlabotus drošības pasākumus, izvietošanas kontroles un reāllaika uzraudzību (‡991*).

2025. gadā vairāki AI izstrādātāji paziņoja, ka jauni modeļi izraisījuši agrīnas brīdinājuma trauksmes vai ka viņi nevarēja izslēgt iespēju, ka turpmāks izvērtējums parādīs, ka modeļi ir pārsnieguši spēju robežsliekšņus. Tas pamudināja viņus piemērot pastiprinātus drošības pasākumus kā piesardzības līdzekli (‡7, ‡33, ‡1121*). Frontier AI Safety Frameworks parasti pieprasa sākotnēju spēju izvērtējumu pirms riska mazināšanas, kā arī atlikušā riska analīzi vai drošības pamatojumu (safety case), ko bieži informē red-teaming pēc mazināšanas. Plašāku informāciju skatiet Tabula 3.5.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Sagatavotības ietvars 2 (‡1078*)
  Aptvertie riski:
1. Bioloģiskās un ķīmiskās spējas
2. Kiberdrošības iespējas
3. AI pašuzlabošanas iespējas
  Riska līmeņi vai ekvivalenti un saistītās drošības prasības:
- Augsts: Var pastiprināt esošos ceļus uz smagu kaitējumu (nepieciešamas drošības kontroles un aizsardzības pasākumi)
- Kritiski: Var radīt nepieredzētus jaunus ceļus uz smagu kaitējumu (Pārtraukt turpmāku izstrādi, līdz ir izpildīti norādītie drošības pasākumi un drošības kontroles standarti sasniedz Kritiski līmeni)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Atbildīgās mērogošanas politika 2.2 (‡991*)
  Aptvertie riski:
1. CBRN ieroči
2. Autonomās AI izpēte un izstrāde (AI I&D)
3. Kiberoperācijas (vērtēšanā)
  Riska līmeņi vai līdzvērtīgi un ar tiem saistītie aizsardzības pasākumi:
  AI drošības līmeņi (ASL)
- ASL-1: Nav nozīmīga katastrofāla riska
- ASL-2: Bīstamu spēju agrīnas pazīmes (Modeļiem jāatbilst ASL-2 izvietošanas un drošības standartiem)
- ASL-3: Būtiski palielināts katastrofālas ļaunprātīgas izmantošanas risks (Modeļiem jāatbilst ASL-3 izvietošanas un/ vai drošības standartiem)
- ASL-4+: Nākotnes klasifikācijas (vēl nav definētas)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Frontier Safety Framework 3.0 (‡1040*)
  Aptvertie riski:
1. Nepareiza izmantošana
    a. CBRN
    b. Kiber
    c. Kaitīga manipulācija
2. Mašīnmācību pētniecība un izstrāde
3. Nesakritība/ Instrumentālā spriešana
  Riska pakāpes vai ekvivalenti un saistītie aizsardzības pasākumi:
  Kritiskās spēju līmeņi
    Spējas līmeņi, kuros, nepiemērojot mazināšanas pasākumus (drošības pamatojumi izvietojumiem un drošības mazināšanas pasākumi, kas saskaņoti ar RAND drošības līmeņiem 2, 3 vai 4 (‡1122)), AI modeļi vai sistēmas var radīt paaugstinātu risku izraisīt smagu kaitējumu. Spējas līmeņi ietver “agrīnās brīdināšanas novērtējumus”, ar konkrētiem “brīdinājuma sliekšņiem”
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Frontier AI ietvars 1.1 (‡990*)
  Aptvertie riski:
1. Kiberdrošība
2. Ķīmiskie un bioloģiskie riski
  Riska līmeņi vai ekvivalenti un ar tiem saistītie aizsardzības pasākumi:
  Riska sliekšņa līmeņi
- Mēreni (izlaidums ar atbilstošiem drošības pasākumiem un mazinājumiem)
- igh (neatlaidiet)
- Kritisks (pārtraukt izstrādi)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Frontiera modeļa drošības ietvars (‡1123*)
  Aptvertie riski:
1. CBRN ieroču izplatīšana
2. Ļaunprātīgas kiberoperācijas
3. Automatizēta AI pētniecība un izstrāde
  Riska pakāpes vai ekvivalents līmenis un saistītās aizsardzības pasākumi:
  Kritiskās spēju sliekšņvērtības
    Modeļa iespējas, kas var radīt būtisku kaitējumu sabiedrībai, ja tās tiek ļaunprātīgi izmantotas. (Ja sliekšņi ir sasniegti vai pārsniegti, modelis netiks publiski izvietots bez atbilstošiem riska mazināšanas pasākumiem)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Frontier pārvaldības ietvars (‡1124*)
  Aptvertie riski:
1. CBRN ieroči
2. Ļaunprātīgas kiberoperācijas
3. Papildu autonomija (t.sk. AI pētniecība un izstrāde)
  Riska līmeņi vai līdzvērtīgas kategorijas un attiecīgie aizsardzības pasākumi:
  Riska līmeņi
- Zema vai Vidēja (Izvietošana atļauta saskaņā ar Atbildīgas mākslīgā intelekta programmas prasībām)
- Augsta vai Kritiska (turpmāka pārskatīšana un mazināšanas pasākumi)
(nepieciešams)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Frontier AI riska novērtējums (‡1029*)
  Aptvertie riski:
1. Kiberdelikts
2. CBRN
3. Pārliecināšana un manipulēšana
4. Nelegāla diskriminācija mērogā
  Riska līmeņi vai līdzvērtīgi un ar tiem saistītie aizsardzības pasākumi:
  Riska sliekšņi – modeļa riska (MR) rādītāji
- MR1 vai MR2 (Novērtējuma rezultātus dokumentē inženierijas komandas)
- MR3 (Riska mazināšanas pasākumi un izvērtēšanas rezultāti tiek dokumentēti inženierijas komandās un periodiski pārskatīti)
- MR4 (Jāveic detalizēta riska novērtēšana un ir nepieciešams biznesa vienības vadītāja apstiprinājums)
- MR5 (Detalizēts riska novērtējums ir jāveic un jāapstiprina neatkarīgai komisijai, piemēram, NVIDIA AI ētikas komitejai)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Droša AI priekšējās līnijas modeļa ietvara struktūra (‡1125*)
  Aptvertie riski:
1. Ļaunprātīga izmantošana (piem., ļaunprogrammatūra, bērnu seksuāla izmantošana)
2. Kaitējums parastā, ne ļaunprātīgā izmantošanā, piem., izvades, kas rada nelikumīgu diskriminējošu iznākumu vai nedrošu koda ģenerēšanu
  Riska līmeņi vai līdzvērtīgi un saistītās aizsardzības:
  Bojājuma iespējamība un smagums kontekstā
- Zems
- Vidējs
- Augsts
- Ļoti augsts
    (Riska mazināšanas pasākumi un drošības kontroles ir ieviestas visām sistēmām un procesiem; papildu mazināšanas pasākumi ir jāpielāgo AI sistēmai un lietošanas gadījumam, kurā modelis tiek izvietots)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: AGI gatavības politika (‡1127*)
  Aptvertie riski:
1. Kiberdelikts
2. Automatizēta AI pētniecība un izstrāde
3. Autonomā replikācija un adaptācija
4. Bioloģisko ieroču atbalsts
  Riska pakāpes vai līdzvērtīgas kategorijas un saistītās aizsardzības pasākumi:
  Kritiskās spēju sliekšņvērtības
    Kvantitatīvi sliekšņi spēju etalonrādītājos (ja tiek pārsniegti, veikt bīstamu spēju novērtējumus, informācijas drošības pasākumus un izvietošanas mazinājumus vai apturēt izstrādi)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: AGI Gatavības politika (‡1127*)
  Aptvertie riski:
1. Kiberdelikts
2. Automatizēta AI pētniecība un izstrāde
3. Autonomā replikācija un adaptācija
4. Bioloģisko ieroču atbalsts
  Riska līmeņi vai līdzvērtīgi un tiem atbilstošas aizsardzības:
  Kritiskās spēju sliekšņvērtības
    Kvantitatīvi sliekšņi kompetenču etalonos (Ja tie tiek pārsniegti, veikt bīstamas kompetenču izvērtēšanas, informācijas drošības pasākumus un izvietošanas mazināšanas pasākumus vai pārtraukt izstrādi)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: AI drošības ietvars (‡1128*)
  Aptvertie riski:
1. Kontroles zudums
2. Nepareiza izmantošana (piemēram, bioķīmisko ieroču radīšana
  Riska līmeņi vai ekvivalenti un saistītie drošības pasākumi:
  Riska līmeņi
- Zems risks (Ievietojiet AI sistēmas, bet pēc tam veiciet uzraudzību, lai pārvaldītu riska faktorus)
- Risks identificēts (vai nu atvērt tikai AI sistēmas autorizētiem lietotājiem, lai mazinātu riskus, vai aizkavēt izvietošanu līdz tiek veiktas papildu drošības pasākumi, atkarībā no lietošanas gadījuma)
- Augsts risks (Nedrīkst izvietot AI sistēmas)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Frontier AI drošības ietvars (‡1129*)
  Aptvertie riski:
1. Bioloģiski apdraudējumi
2. Ļaunprātīga kiberdrošība
3. Autonomā darbība un uzlabota manipulācija
  Riska pakāpes vai ekvivalents un ar tām saistītie aizsardzības pasākumi:
  Riska līmeņi
- 1. līmenis (Pamata aizsardzības pasākumi minimāliem riskiem un iespējamai atklātā pirmkoda izlaišanai)
- 2. līmenis (reāllaika uzraudzība, pieprasījumu filtrēšana, uzvedības anomāliju noteikšana, piekļuves kontroles, sarkano komandu pārbaudes un pretinieka simulācijas)
- 3. līmenis (Papildu uzlabotas aizsardzības, tostarp sarkanās komandas izstrāde, pakāpeniski izvietojumi, pretinieka pārbaudes, šifrēšana, daudzpušu piekļuves kontroles un nulles uzticēšanās arhitektūra)
- 4. līmenis (Maksimāli drošības protokoli augstas nozīmes modeļiem un maksimāli drošības pasākumi)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabula 3.5: Frontier AI drošības ietvari
>white|black||9|11|br Pirmie Frontier AI Safety Frameworks komplekti, ko laidusi klajā apakškopa AI izstrādātāju, kuri parakstīja Frontier AI Safety Commitments. Šie ietvari aptver līdzīgus riskus (ar nelielām atšķirībām) un izmanto atšķirīgas riska pakāpes (risk tiers) un riska pārvaldības pieejas.


>white|orangered|left|14|15.5|bb Frontier AI drošības ietvarstruktūru efektivitāte nav skaidra

Frontier AI Safety Frameworks var kalpot kā riska pārvaldības rīki noteiktos apstākļos un noteiktām riska kategorijām, kurām ir ticams ceļš uz kaitējumu (‡1117). Tajā pašā laikā vairākas analīzes aplūko jautājumus par to skaidrību un tvērumu (‡111, ‡986) un par AI spēju izturību un riska sliekšņiem (‡1031, ‡1130). Esošās ietvarstruktūras bieži koncentrējas uz daļu riska jomu. Līdz ar to dažiem nozīmīgiem riskiem, piemēram, nelikumīgai uzraudzībai (‡1131, ‡1132) un ne-saskaņotam intīmam tēlam (‡287), tiek pievērsta mazāka uzmanība. Atšķirībā no riska pārvaldības pieejām citās nozarēs, piemēram, aviācijā vai kodolenerģijā (‡1133*), Frontier AI Safety Frameworks parasti neizmanto skaidrus kvantitatīvus riska sliekšņus (‡1134).

Ārējie vērtējumi par izstrādātāju atbilstību to Frontier AI Safety Frameworks (augstākā līmeņa AI drošības ietvariem) līdz šim joprojām ir ierobežoti, daļēji tāpēc, ka lielākā daļa ietvaru ir neseni, publiski pieejamā informācija ir nepietiekama un nav standartizētu ārēju auditu. To efektivitāti ietekmēs arī tas, cik labi – un kādā mērā – apņemšanās tiek īstenotas praksē. Pašiem par sevi šie ietvari var negarantēt efektīvu riska pārvaldību, jo to praktiskā ietekme ir atkarīga no tā, cik labi – un kādā mērā – tie tiek īstenoti. Līdz šim tie pilnībā nesakrīt ar starptautiskajiem riska pārvaldības standartiem (‡1135). Pētījumā par iepriekšējām brīvprātīgām apņemšanām tika konstatēta nevienmērīga izpilde dažādos pasākumos, kas liecina, ka brīvprātīgo apņemšanos ievērošana, visticamāk, atšķirsies starp uzņēmumiem un jomām (‡1109).

Kopā ņemot, Frontier AI Safety Frameworks pārstāv visdetalizētāko brīvprātīgo organizatoriskā riska pārvaldības formu, kas pašlaik ir plaši izmantota, taču būtiski atšķiras pēc tvēruma, sliekšņiem un izpildāmības.

###@ Regulatīvas un pārvaldības iniciatīvas

>white|orangered|left|14|15.5|bb Vairākas jurisdikcijas ir ieviesušas tiesību aktus ar pārredzamības prasībām

Vairāki agrīni regulatīvi pieejas ievieš tiesiskas prasības, kuru mērķis ir palielināt standartizāciju un pārskatāmību riska pārvaldībā. ES AI akts, kas stājās spēkā 2024. gadā, nosaka prasības attiecībā uz pārskatāmību, autortiesībām un drošību vispārējas nozīmes AI modeļiem. 2025. gadā tika publicēts ES Vispārējas nozīmes AI kodekss praksei, lai atbalstītu atbilstību šīm saistībām, sniedzot norādījumus par modeļu dokumentēšanu un autortiesībām, kā arī – vismodernākajiem modeļiem – riska pārvaldības prakses, piemēram, izvērtējumus, riska novērtēšanu un mazināšanu, informācijas drošību un nopietnu incidentu ziņošanu (‡965).

Citi piemēri jaunu regulatīvo prasību ir Dienvidkorejas “Framework Act on the Development of Artificial Intelligence and Establishment of Trust”, kas ievieš prasības “augstas ietekmes” AI sistēmām kritiski svarīgās nozarēs (‡1136), un Kalifornijas SB 53, kas nosaka pārredzamības prasības attiecībā uz drošības ietvariem un incidentu ziņošanu (‡1104). Tā kā šīs prasības tika izveidotas pavisam nesen, ir par agru, lai detalizēti novērtētu, kā tās ietekmēs riska pārvaldības prakses vai faktisko riska iznākumu.

>white|orangered|left|14|15.5|bb Plašākas pārvaldības iniciatīvas sniedz brīvprātīgas vadlīnijas

Vairāki reģionālās un starpreģionālās pārvaldības ietvari tagad formulē kopējas gaidas attiecībā uz risku pārvaldību, ko rada vispārīga nozīmes AI, nodrošinot nesaistošas vadlīnijas politikas veidotājiem un organizācijām. Ķīnas AI drošības pārvaldības ietvars 2.0, kas publicēts 2025. gadā, sniedz strukturētas vadlīnijas par risku kategorizāciju un pretpasākumiem visā AI izstrādes un ieviešanas procesā (‡1137). ASEAN dalībvalstis publicēja ‘ASEAN paplašināto ceļvedi par AI pārvaldību un ētiku (ģeneratīvā AI)’, kas sniedz vadlīnijas par vispārīga nozīmes AI pārvaldību un ētiku un ir paredzēts, lai atbalstītu lielāku politiku saskaņotību starp ASEAN dalībvalstīm (‡1138). Turklāt ar ekspertu vadītām iniciatīvām, piemēram, Singapūras konsensu, ko izstrādājuši AI zinātnieki no vairākām valstīm, tiek noteiktas pētniecības prioritātes vispārīga nozīmes AI drošībai, aptverot risku novērtēšanu, izstrādi un kontroli (‡690).

###@ Atjauninājumi

Kopš pēdējā Pārskata publicēšanas (2025. gada janvāris) vispārējas nozīmes AI riska pārvaldības vide ir mainījusies, līdz ar jaunu resursu publicēšanu, piemēram, ES Vispārējas nozīmes AI rīcības kodeksa, G7 HAIP ziņošanas ietvara, Ķīnas nacionālā AI drošības pārvaldības ietvara 2.0 un dažādu AI izstrādātāju Frontier AI Safety ietvaru. Šīs iniciatīvas apraksta pieejas un prakses, ko AI izstrādātāji izmanto, lai pārvaldītu riskus, kas saistīti ar vispārējas nozīmes AI sistēmām (‡1115). Frontier AI Safety ietvaros un HAIP pārredzamības ziņojumos (‡1103) pastāv būtiskas atšķirības, kas atspoguļo atšķirīgas organizatoriskās prakses, riska prioritizēšanu un visai agrīno vispārējas nozīmes AI riska pārvaldības ekosistēmas attīstības stadiju. Uzticama ekosistēma, kurā dažādi AI dalībnieki visā dzīves ciklā sniedz papildinošas riska pārvaldības prakses, var sekmēt efektīvu riska pārvaldību (‡690).

###@ Pierādījumu trūkumi

Ir trūkst pierādījumu par: kā izmērīt jauno risku smagumu, izplatību un laika ietvaru; kādā mērā šos riskus var mazināt reālās dzīves kontekstos; un kā efektīvi veicināt vai panākt mazināšanas pasākumu ieviešanu dažādu pušu vidū. Ir nepieciešami papildu pētījumi, lai saprastu, cik izplatīti ir dažādi riski un cik lielā mērā tie atšķiras dažādos pasaules reģionos, jo īpaši reģionos, kas strauji digitilizējas, piemēram, Āzijā, Āfrikā un Latīņamerikā. Tā kā AI modeļiem tiek piešķirta pieaugoša rīcībspēja un autoritāte, un vispārējas nozīmes AI risku zinātniskais stāvoklis attīstās, arī riska pārvaldības pieejām būs jāattīstās (‡639, ‡1139).

Dažas riska mazināšanas pieejas kļūst arvien populārākas (‡690, ‡956), taču nepieciešami papildu pētījumi, lai izprastu, cik noturīgas praksē ir riska mazināšanas un aizsardzības pasākumi dažādām kopienām un AI dalībniekiem (tostarp maziem un vidējiem uzņēmumiem). Novērtējumiem ir būtiska lielāka piekļuve datiem par reālu modeļu izvietošanu un izmantošanu dzīvē. Turklāt riska pārvaldības pasākumi pašlaik ievērojami atšķiras starp vadošajiem AI uzņēmumiem. Ir izteikts arguments, ka izstrādātāju stimuli nav pietiekami saskaņoti ar rūpīgu riska novērtēšanu un pārvaldību (‡934). Vēl joprojām pastāv pierādījumu nepietiekamība par to, kādā mērā tiek izpildītas dažādas brīvprātīgās saistības, ar kādiem šķēršļiem uzņēmumi saskaras, lai pilnībā ievērotu saistības, un kā tie integrē Frontier AI Safety Frameworks plašākās AI riska pārvaldības praksēs.

###@ Izaicinājumi politikas veidotājiem

Galvenie izaicinājumi ietver to, kā noteikt dažādu vispārējas nozīmes AI radīto risku prioritātes, noskaidrot, kuri aktori ir vislabākajā pozīcijā tos mazināt, un izprast stimulus un ierobežojumus, kas nosaka viņu rīcību. Pierādījumi liecina, ka politikas veidotāji pašlaik saskaras ar ierobežotu piekļuvi informācijai par to, kā AI izstrādātāji un ieviesēji testē, novērtē un uzrauga topošos riskus, kā arī par dažādu riska mazināšanas prakšu efektivitāti (‡1140). Pētnieki un politikas veidotāji ir apsprieduši pārredzamības iniciatīvas un sistemātiskāku incidentu ziņošanu kā iespējamos veidus, kā informēt par riska prioritizēšanu, veicināt uzticēšanos un stimulēt atbildīgu izstrādi (‡957). Reāli risku pārvaldība ietver vairākus aktorus visā AI vērtību ķēdē – piemēram, datu un mākoņpakalpojumu sniedzējus, modeļu izstrādātājus un modeļu mitināšanas platformas – un katram ir atšķirīgas iespējas izvērtēt un pārvaldīt dažādus riskus (‡1141). Ierobežota informācijas apmaiņa starp šiem aktoriem apgrūtina noteikt, kuri riski ir visdrīzākie vai visietekmīgākie, jo īpaši tad, ja tiek ņemtas vērā lejupējās sabiedriskās sekas.

