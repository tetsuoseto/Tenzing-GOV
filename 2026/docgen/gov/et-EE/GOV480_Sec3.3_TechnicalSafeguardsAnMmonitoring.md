##########
>white|orangered|left|14|30|hr Jaotis 3.3
### 3.3. Tehnilised kaitsemeetmed ja jälgimine
>white|orangered|left|24|30|hb Tehnilised kaitsemeetmed ja seire

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb Oluline teave
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Laialdast valikut tehnilisi turvameetmeid kasutatakse AI väljatöötamise ja kasutamise eri etappides. Nende hulka kuuluvad meetodid, mida rakendatakse mudeli arendamise ajal, et muuta süsteemid vastupidavamaks ja väärkasutusele vastupidavamaks (nagu andmete ettevalmistamine), kasutuselevõtuaja järelevalve ja kontroll (nagu sisu filtreerimine ja inimlik järelevalve) ning pärast kasutuselevõttu kasutatavad tööriistad, et jälgida laiemat AI ökosüsteemi (nagu päritolu ja sisu tuvastamine).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Tehnilised kaitsemeetmed võivad olla piiratud ja ei suuda usaldusväärselt takistada kahjulikku käitumist kõigis olukordades. Näiteks võivad kasutajad mõnikord saada kahjulikke väljundeid, kui nad sõnastavad päringuid ümber või jagavad need väiksemateks sammudeks. Samamoodi saab sageli eemaldada või muuta selliseid tööriistu nagu vesimärgistus, mis on loodud tuvastama tehisintellekti loodud sisu, mis vähendab nende usaldusväärsust.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Üksikute kaitsemeetmete piirangud tähendavad, et teatud kahjulike tulemuste vältimiseks võib vaja minna „kaitset mitme kihina” (defence-in-depth). Näiteks võib süsteem kombineerida ohutuseks treenitud mudeli sisufiltritega, väljundfiltritega ja sisumonitoridega.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Alates viimasest aruandest (jaanuar 2025) on teadlased teinud edusamme kaitsemeetmete parandamisel, kuid põhilised piirangud püsivad. Näiteks kaitsemeetmetest möödahiilimiseks loodud rünnakute õnnestumise määr on langenud, kuid on endiselt suhteliselt kõrge. Samuti on põhilisi piiranguid sellele, kui põhjalikult saab avakaalulisi (open-weight) mudeleid kaitsta.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Poliitikakujundajate jaoks on üks peamisi väljakutseid piiratud tõendusmaterjal selle kohta, kui tõhusad on kaitsemeetmed erinevates üldotstarbeliste AI-süsteemide tegelikes kasutusjuhtumites. AI-arendajad jagavad väga erineval määral teavet oma kaitsemeetmete ja seire kohta. Täiendav väljakutse on võimalikud kompromissid tugevamate kaitsemeetmete rakendamise ja süsteemi jõudluse või kasulikkuse säilitamise vahel.
>oldlace|black||11|15|br      


AI arendajad saavad kasutada mitmeid kasulikke, kuid ebatäiuslikke tehnilisi kaitsemeetmeid, et leevendada ja hallata riske üldotstarbelistest AI-süsteemidest, ent töökindluse väljakutsed püsivad. Arendajad ei saa endiselt täielikult takistada üldotstarbelisi AI-süsteeme tegemast isegi hästi tuntud ja selgelt kahjulikke tegevusi, näiteks pakkumast kasutajatele juhiseid kuritegude toimepanekuks. Näiteks on teadlased näidanud, et tipptasemel kaitsemeetmeid saab kõrvale juhtida vastandlike päringumeetodite abil (st „jailbreak’id“) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), lastes mudelitel jagada keerukad kahjulikud ülesanded sammudeks (‡1150, ‡1151, ‡1152, ‡1153, ‡1154) ning lihtsate mudeli muudatustega (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Teadlased jätkavad kaitsemeetmete väljatöötamist rikete ja väärkasutuse vastu (‡690). Need meetodid erinevad väga laialdaselt oma eesmärgi ja tõhususe poolest ning nende mõju sõltub lõppkokkuvõttes laiemast sotsio-tehnilisest ja valitsemise (governance) kontekstist, milles AI-süsteemid luuakse ja kasutusele võetakse.

Tehnilised kaitsemeetmed võib laias laastus jagada kolme kategooriasse: meetodid ohutumate mudelite väljatöötamiseks; meetodid, mida kasutatakse kasutuselevõtu ajal seireks ja kontrolliks; ning meetodid, mis toetavad kasutusejärgset ökosüsteemi seiret. Laud 3.6 võtab kokku arutatud tehnilised kaitsemeetmed, nende tõhususe ja lahendamata väljakutsed.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Turvalisemate mudelite väljatöötamine
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Andmete kureerimine (‡1167)
  Ohtliku andmestiku eemaldamine, et takistada mudelil omandada ohtlikke võimeid. Need meetodid võivad olla kasulikud, sealhulgas ohtlike võimeteta ja kahjuliku peenhäälestuse suhtes vastupidavate avatud kaaludega mudelite arendamisel (‡55). Siiski esineb väljakutseid kureerimisvigade ja skaleerimisega (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Inimese tagasiside põhine tugevdamisõpe (‡64*)
  Mudeli koolitamine, et see vastaks etteantud eesmärkidele, nagu olla abivalmis ja kahjutu. See on tõhus viis, kuidas mudelid õpivad kasulikke käitumisviise (‡64*). Kuid inimeste heakskiidu jaoks liigne optimeerimine võib panna mudelid käituma petlikult või meelitavalt (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pluralistliku joondamise tehnikad (‡1170)
  Mudelile õpetamine, et integreerida mitut erinevat vaatenurka selle kohta, kuidas ta peaks käituma. Need tehnikad aitavad vähendada ulatust, mil määral mudelid eelistavad kindlaid vaatenurki (‡1170). Sellegipoolest, hoolimata nendest tehnikatest, on inimeste eriarvamused vältimatud ning on raske kavandada laialdaselt aktsepteeritud viise konkureerivate vaatenurkade tasakaalustamiseks (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adversariaalne treenimine (‡677)
  Mudelile õpetamine keelduma kahju tekitamisest (ka tundmatutes olukordades) ning tõrjuma pahatahtlike kasutajate rünnakuid (nt 'jailbreaks'). See on tõhus meetod, kuidas muuta mudelid vastupidavamaks väärkasutamise katsetele (‡1064), kuid vastupidavuse probleemid püsivad endiselt (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Masina „unlearning“ (‡1175, ‡1176)
  Mudeli treenimine spetsialiseeritud algoritmidega tähendas aktiivset ohtlike võimekuste (nt bioloogiliste ohtude tundmine) pärssimist. Need tehnikad pakuvad sihipärast viisi ohtlike võimekuste eemaldamiseks mudelitest (‡1175, ‡1176), kuid praegused unlearning-algoritmid võivad olla ebakindlad ja põhjustada soovimatuid mõjusid teistele võimekustele (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tõlgendatavuse ja ohutuse kontrollimise tööriistad (‡1177)
  Disain- ja valideerimismeetodite mitmekesine kogum, mille eesmärk on pakkuda senisest rangemat kindlustunnet, et mudelitel on kindlad ohutusega seotud omadused. Need võimaldavad hindajatel teha suurema kindlusega väiteid ohutuse kohta (‡1177), kuid praegused meetodid tuginevad eeldustele ning ei ole praktikas jõudluse poolest harva konkurentsivõimelised (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Jälgimine ja juhtimine
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riistvarapõhised seiremehhanismid (‡1179, ‡1180, ‡1181)
  Volitatud protsesside toimimise kontrollimine riistvaral, et uurida turvaohtusid või vastavust regulatiivsetele nõuetele. Need mehhanismid pakuvad unikaalseid võimalusi jälgida, milliseid arvutusi riistvaral käitatakse ja kelle poolt (‡1181). Samas ei suuda riistvarapõhised mehhanismid jälgida kõikvõimalike ohtude eest ning mõned tehnikad nõuavad spetsialiseeritud riistvara (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kasutajategevuse seire (‡1154, ‡1166)
  Kasutajate suhtluse jälgimine pahatahtliku kasutuse märkide leidmiseks võib aidata arendajatel pahatahtlikke kasutajaid teenusest eemaldada (‡1154, ‡1166). Kuid jõustamine võib kogemata takistada kasulikku turvalisusealast teadustööd (‡689) ning mõned väärkasutuse vormid on raskesti tuvastatavad (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kasutajavahetuse jälgijad (‡1154, ‡1166)
  Kasutajate interaktsioonide jälgimine pahatahtliku kasutuse märgiste leidmiseks võib aidata arendajatel peatada teenuse osutamise pahatahtlikele kasutajatele (‡1154, ‡1166). Siiski võib jõustamine tahtmatult takistada kasulikku ohutusuuringut (‡689) ning mõnda väärkasutuse vormi on raske tuvastada (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sisufiltrid (‡65*, ‡725)
  Filtreerimine võimalike kahjulike mudeli sisendite ja väljundite jaoks on väga tõhus viis vähendamaks juhuslikku kahju ja kuritarvitamise riske (‡725). Kuid filtrid nõuavad täiendavat arvutusressurssi ja on haavatavad teatud rünnakutele (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mudeli sisemised arvutusmõõdikud (‡744, ‡1183, ‡1184)
  Mudelites esinevate pettuse märkide või muude kahjulike sisemiste tunnetusvormide jälgimine võib olla tõhus viis pettuse tuvastamiseks (‡744, ‡1183, ‡1184). Siiski puuduvad tänapäevastel meetoditel vastupidavus ja usaldusväärsus (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Järeldusahela monitooring (‡430, ‡435)
  Mudel-keti mõttekäigu (chain-of-thought) teksti jälgimine, et leida märke eksitavast käitumisest või muust kahjulikust arutluskäigust, on tõhus viis mõista ja märgata puudusi selles, kuidas mudelid arutlevad (‡435). Siiski võivad need olla ebausaldusväärsed (‡752, ‡753, ‡1186) ning kui mudeleid õpetatakse tootma healoomulist mõttekäiku (chain of thought), võivad need õppida eksitavat käitumist (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Inimene silmuses (‡1187, ‡1188, ‡1189)
  Inimlik järelevalve ja otsuste tühistused süsteemi tasandil on mõnes ohukriitilises rakenduses hädavajalikud (‡1187). Siiski piiravad neid meetodeid automatiseerimise eelarvamus ja inimotsuste tegemise kiiruse piirangud (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Isoleerimine (‡1192)
  Kahjustuste vähendamiseks, mida see võib põhjustada, on tõhus viis vältida, et tehisintellekti agent mõjutaks maailma vahetult (‡1192). Kuid sandboxing piirab süsteemi võimet teatud ülesandeid otseselt täita (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Tööriistad ökosüsteemi seire hõlbustamiseks
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tehisintellekti mudeli tuvastamise tehnikad (‡1193*, ‡1194)
  Mudelid või mudelite üksikeksemplarid on reaalses kasutuses lihtsamini tuvastatavad, mis aitab kaasa digitaalsele forensikale ja ökosüsteemi teadlikkusele (‡1195). Siiski saab neid võtteid mõne tüüpi mudelimuudatustega kõrvale hiilida (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tehisintellekti mudeli pärandi tuletus (‡1197)
  Need tehnoloogiad võimaldavad uurijatel uurida, kuidas mudeleid muudetakse AI ökosüsteemis, eriti avatud kaaludega mudelite puhul. Need aitavad digitaalse kohtuekspertiisi ja ökosüsteemi teadlikkuse korral (‡1198), kuid põhjalikuks avatud kaaludega mudelite ökosüsteemi kaardistamiseks oleks vaja suuri ja ulatuslikke projekte (‡1198).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vesimärgid ja metaandmed (‡1199, ‡1200, ‡1201*)
  Need tehnikad muudavad lihtsamaks tuvastada, kui mõni tekst, pilt, video jne on toodetud tehisintellekti abil või muudetud ning millise süsteemi poolt. Need võimaldavad paremat ökosüsteemi teadlikkust (‡1199, ‡1200, ‡1201*). Siiski saab vesimärke ja metaandmeid võltsida või eemaldada mõne sisule tehtud muudatusega (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tehisintellekti loodud sisu tuvastamine (‡1203, ‡1204, ‡1205*)
  Kasutajate võime parandamine eristada AI-generatsiooniga loodud ja ehtsat sisu aitab kaasa digitaalsele forensikale ja ökosüsteemi teadlikkusele (‡1203, ‡1204). Siiski võivad klassifikaatorid olla ebausaldusväärsed (‡1205*) ning nende jõudlus võib erineda eri modaliteetide lõikes.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Laud 3.6: Selles jaotises käsitletud tehnilised kaitsemeetmed
>white|black||9|11|br Kokkuvõte selles jaotises käsitletud tehnilistest kaitsemeetmetest, jaotatuna meetoditeks turvalisemate mudelite väljatöötamiseks, kasutuseaegseks jälgimiseks ja kontrolliks ning tehnikateks ökosüsteemi seire hõlbustamiseks.


###@ Turvalisemate mudelite väljatöötamine

Esimene kaitseliin kahjude vastu üldotstarbelistest tehisintellektisüsteemidest on muuta aluseks olev mudel turvalisemaks. Käesolev alajaotus käsitleb kaitsemeetmeid, mis on „mudeli parameetritesse sisse küpsetatud“ mudeli arendamise käigus (Kujund 3.6).

>white|orangered|left|14|15.5|bb Treeningandmete kureerimine võib piirata potentsiaalselt ohtlike võimekuste arendamist

Üldotstarbelised tehisintellekti mudelid on kasulikud just seetõttu, et need arendavad pärast treeningandmete töötlemist laia teadmiste ja võimete spektrit, kuid teatud tüüpi treeningandmed on ebaproportsionaalselt vastutavad potentsiaalselt ohtlike võimete väljaarendamise eest. Näiteks võib viroloogiaalastele artiklitele koolitatud AI mudel olla paremini võimeline pakkuma abi potentsiaalselt kahjulikes bioloogiaülesannetes (‡549, ‡1206*) (vt ka §2.1.4. Bioloogilised ja keemilised riskid). Lisaks saab inimalastust kujutavatel piltidel koolitatud pildi-/video-generaatoreid samuti kuritarvitada selleks, et luua mittenõusolekulisi intiimseid deepfakes’eid (‡308, ‡319) (vt ka §2.1.1. AI-genereeritud sisu ja kuritegevus).

Õppematerjali filtreerimine on tõhus leevendus mõne soovimatu võimekuse vastu (‡319, ‡1167, ‡1207, ‡1208). Siiski võib olla keeruline filtreerida suuri andmekogumeid, mida kasutatakse üldotstarbeliste tehisintellekti mudelite (‡1168) treenimiseks, sest kulud on suured (‡1209), esineb filtreerimisvigu (‡1210) ning andmestiku kvaliteedile avalduvad negatiivsed mõjud (‡1211). Need raskused süvenevad internetiteksti mitmekeelsuse tõttu (‡1212), sisumodereerimise kultuuriliste eelarvamuste tõttu (‡1211, ‡1213, ‡1214, ‡1215) ning asjaolu tõttu, et see, kas konkreetne andmeosa on „kahjulik“, sõltub kontekstuaalsetest teguritest (‡1216). Sellegipoolest näitab potentsiaalselt kahjuliku materjali filtreerimine treeningandmetest lubadust muuta mudelid usaldusväärsemalt ohutumaks, sh muuta avatud kaaludega mudelid (open-weight models) kahjulikumale manipuleerimisele vastupidavamaks (‡55). Seosed treeningandmete sisu ja tekkivate mudeli võimekuste vahel ei ole veel täielikult mõistetavad (‡1195) ning filtreerimine näib olevat kahjulike võimekuste piiramises tõhusam, kui seda rakendada teadmiste laiematele domeenidele (‡55), võrreldes kitsamate käitumistega (‡1206, ‡1217). Vt §3.4. Avatud kaaludega mudelid edasiseks aruteluks.

![figure 3.6](images/fig3.6_safeguards.png)

##### Kujund 3.6: Kus tehnilisi turvameetmeid rakendada
>white|black||9|11|br Tehnilisi kaitsemeetmeid saab rakendada mudeli arendamise eri etappidel. Andmete ettevalmistamine kujundab seda, mida mudelid õpivad eelõppe ja peenhäälestuse käigus. Koolitusel põhinevad meetodid, nagu inimeste tagasiside põhine tugevdamisõpe ja vastupidavustreening, kohandavad mudeli käitumist. Katsetusmeetodid, nagu vastandlikud rünnakud, tuvastavad allesjäänud haavatavused. Mõned tehnikad, nagu ohutuse-kui-kavandi algoritmid, hõlmavad mitut etappi. Allikas: Rahvusvaheline tehisintellekti ohutuse aruanne 2026.


>white|orangered|left|14|15.5|bb Üldotstarbeliste tehisintellektimudelite koolitamise meetodid, et need oleksid peamiselt abivalmid ja ohutud, tuginevad peamiselt inimeste tagasisidele

Mudeleid on keeruline treenida ja hinnata nii, et need usaldusväärselt ühtiksid kõrgetasemeliste põhimõtetega, nagu abivalmidus, kahjutus ja ausus. Praktikas püüavad arendajad seda saavutada, peenhäälestades tehisintellekti mudeleid inimeste demonstratsioonide ja tagasiside põhjal. Näiteks peamine paradigmade peenhäälestamisel, mida tuntakse kui “human feedback’ist lähtuv tugevdamisõpe”, põhineb mudelite treenimisel tootma väljundeid, mida inimeste märgistajad hindavad positiivselt (‡1218). Siiski on positiivne tagasiside inimestelt vigane asendusnäitaja kasulikule käitumisele (‡737, ‡878, ‡1219, ‡1220) ning seda piiravad inimlikud vead ja eelarvamused (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

See toob kaasa mitmeid väljakutseid: võimendusega õppimise teel inimeste tagasiside põhjal peenhäälestatud mudelid võivad mõnikord kasutajale meeldida liigselt, mis on tuntud kui ‘meeldimisele orienteeritus’ (‡358, ‡740, ‡1226, ‡1227); anda vastuseid, mis on mõnes kontekstis abivalmid, kuid teistes kahjulikud (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); esitada vastuseid, mille õigsust on keeruline hinnata (‡1233); või sooritada tegevusi, mille abivalmidus või kahjulikkus on arvamuse küsimus (‡1234). Laud 3.7 toob näiteid nendest väljakutsetest. Mõni uurimistöö püüab töötada välja meetodeid, mis aitaksid inimestel paremini hinnata lahendusi keerukatele ülesannetele koos AI abiga (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Ent need meetodid on praegu piiratud töökindlusega ning ei ole avalikult teada, mil määral neid kasutatakse tänaste kõige arenenumate AI mudelite treenimiseks.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Silmakirjalik meeldimine/armukesele järeleandmine (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Selgitus:
>white|black|left|11|13|br Mudelis antakse ainult positiivset tagasisidet, ilma et ta osutaks puudusele õige 5-7-5 haiku silbistruktuuris.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mõned toimingud on mõnes kontekstis kasulikud, kuid teistes kahjulikud (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Selgitus:
>white|black|left|11|13|br Teavet bioloogilise riski kohta saab kasutada haridus- ja kaitseotstarbel, kuid ka selleks, et teavitada pahatahtlikke osalejaid.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Õiget käitumist on raske kontrollida (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Selgitus:
>white|black||11|13|br Selle vastuse õigsust on keeruline hinnata, kuna see nõuab meditsiinialaseid teadmisi. Isegi kogenud arstil on selliste vastuste hindamiseks vaja aega ja hoolikat tähelepanu detailidele.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Inimesed ei ole ühel meelel, mis on õige (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Selgitus:
>white|black|left|11|13|br Inimesed ei nõustu oluliselt selles, mis on õige vastus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Laud 3.7: Kasutaja päring ja tehisintellekti mudeli vastus
>white|black||9|11|br Näited väljakutsetest, mis tekivad AI-mudelite poolt kasulike tegevuste määratlemisel ja nende eest motiveerimisel.


>white|orangered|left|14|15.5|bb Inimesed ei nõustu alati sellega, millised käitumisviisid on soovitavad, mistõttu on vaja meetodeid konkureerivate eelistuste tasakaalustamiseks

Inimesed ei lepi alati kokku selles, milliseid vastuseid või tegevusi AI-mudelid peaksid või ei peaks väljundama (‡1006). See muudab põhimõtteliselt keeruliseks arendada mudeleid, mille tegevused ja mõjud oleksid laialdaselt kooskõlas ühiskonna huvidega (‡420). Osa uurijaid uurib, kelle eelistused peegelduvad AI-süsteemides (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) ning töötab välja ‘pluralistliku joondamise’ (pluralistic alignment) tehnikaid, mille eesmärk on leida tasakaal konkureerivate eelistuste vahel (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Näiteks saavad AI-arendajad disainida süsteeme, mis väldivad vastuoluliste vastuste genereerimist, keeldudes reageerimast teatud taotlustele, või joonduda vaadete keskväärtusega (median viewpoint) mõnes asjakohases inimeste valimis, või personaliseerida süsteeme üksikutele kasutajatele.

Nende lähenemisviiside üks levinud väljakutse on see, et üldiselt ei suuda tehisintellektil põhinevad süsteemid kohanduda võrdselt kõigi inimeste eelistustega ning nende edasiste ühiskondlike mõjude tõttu avaldub mõju eri rühmadele erinevalt. Mõned teadlased on väitnud, et enamik tehnilisi lähenemisviise pluralistlikule ühtlustamisele ei suuda käsitleda ega võivad isegi kõrvale juhtida sügavamate väljakutsete eest, nagu süsteemsed kallutatuse allikad, sotsiaalse võimu dünaamika ning rikkuse ja mõju koondumine (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb AI arendajad kasutavad „adversaarset treeningut“, et parandada mudelite töökindlust

AI-mudelite õpitud kasulikke käitumisviise treeningu ajal on keeruline tagada nii, et need kanduksid robustselt üle tegeliku kasutuselevõtu (reaalmaailma) kontekstidesse. Isegi mudelid, mida on treenitud “täiusliku” õppesignaali abil, võivad ebaõnnestuda üldistamisel kõigisse varem nägemata kontekstidesse (‡738, ‡739, ‡1255, ‡1256, ‡1257). Näiteks on mõned uurijad leidnud, et vestlusrobotid teevad tõenäolisemalt kahjulikke tegevusi keeltes, mis on nende treeningandmetes alaesindatud (‡159, ‡880, ‡1258*, ‡1259), kuhu kuulub palju keeli, mida kõnelevad peamiselt ülemaailmse lõuna riikides inimesed.

Viimastel aastatel on teadlased loonud ka suure komplekti nn „vastandlike rünnakute“ tehnikaid, mida saab kasutada selleks, et panna mudelid genereerima potentsiaalselt kahjulikke vastuseid (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Näiteks hiljutine algatus kogus ühiselt üle 60,000 eriilmelise näite edukatest rünnakutest tipptasemel AI mudelite vastu, mis pani need rikkuma oma ettevõtete eeskirju aktsepteeritava mudeli käitumise kohta (‡1149). Tabel 3.8 toob näiteid „jailbreak’i“ tehnikatest, mida teadlased on näidanud, et need võivad panna mudelid järgima kahjulikke päringuid.

Üks viis mudelite töökindluse parandamiseks on tuntud kui “adversaarne treening” (‡1064). See hõlmab “rünnakute” (nt jailbreak’id) konstrueerimist, mis on loodud selleks, et panna mudel käituma ebasoovitavalt, ning mudeli treenimist nende rünnakutega asjakohaselt toime tulema. Kuid adversaarne treening ei ole täiuslik (‡1260, ‡1261). Ründajad suudavad järjepidevalt välja töötada uusi edukaid rünnakuid uusimatele, tipptasemel mudelitele (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Kuna arendajad vajavad konkreetseid näiteid tõrkeviisidest, et nende vastu treenida (‡512, ‡1263), kujuneb tulemuseks pidev “kass ja hiir” mäng, kus arendajad uuendavad mudeleid vastuseksäsuäsäsuäsä äsja avastatud haavatavustele ning vastased otsivad pidevalt uusi rünnakuid. Mõned teadlased on pakkunud suurema mastaabiga adversaarset treeningut (‡1264, ‡1265) või uusi algoritme (‡675, ‡676, ‡1263, ‡1266, ‡1267), et parandada töökindlust, kuid kaasaegsed tehisintelligentsi süsteemid jäävad püsivalt haavatavaks.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Eesmärk: Teha kahjulikke päringuid šifreeritud kujul, näiteks morsekoodina (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strateegia: treenige süsteemi näidetega nõuetele vastavatest vastustest ohtlikele taotlustele (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strateegia: Esita kahjulikke päringuid madala ressursiga keeltes, mida on tõenäoliselt vähem treeningus kasutatud (nt suahiili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strateegia: Jaga kahjulik ülesanne mitmeks süütuks alamtööks (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Laud 3.8: Jailbreakingu strateegiad
>white|black||9|11|br Pahatahtlikud osalejad ja red teams on kasutanud erinevat tüüpi „jailbreak’e”, et panna tehisintellekti mudelid täitma kahjulikke päringuid, mida need tavaliselt kaitsemeetmete tõttu tagasi lükkavad. Näidisväljundid kirjutasid raporti autorid illustratiivsel eesmärgil. Paljud kaasaegsed tipptasemel tehisintellekti mudelid suudavad nüüd enamiku neist meetoditest, kuid uusi jailbreaking’u tehnikaid jätkub.


>white|orangered|left|14|15.5|bb ‘Unlearning’ meetodid võivad leevendada konkreetseid kahjulikke mudeli võimeid

Teine strateegia üldotstarbelisest tehisintellektist tulenevate riskide leevendamiseks on kohandada mudeleid nii, et neil puuduksid võimalused teatud konkreetsetes suure riskiga valdkondades (‡1175, ‡1176). Näiteks töötavad teadlased selle nimel, et arendada välja ‘masin-unnlearning’u’ (machine unlearning) algoritme, mis suudaksid konkreetselt maha suruda võimeid, mis on seotud bioterroriohtudega või alasti inimkehade fotorealistlike piltide genereerimisega (‡903, ‡1272, ‡1273). Need meetodid võivad muuta mudelid märkimisväärselt ohutumaks, kuid samal ajal piiravad mõningaid positiivseid kasutusviise unlearnitud võimetel. AI-mudelite teadmiste piiramine ohtlikes valdkondades on samuti pakutud kui viis kujundada ‘manipuleerimiskindlaid’ avatud kaalukomplektiga (open-weight) mudeleid, mis suudavad vastu seista kahjulikule fine-tuning’ule (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Seni on see aga olnud keeruline teha robustselt (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Vt §3.4. Avatud kaalukomplektiga mudelid edasiseks aruteluks.

>white|orangered|left|14|15.5|bb Mõned teadlased töötavad välja meetodeid tugevamate ohutusgarantiide jaoks, tõlgendades mudeli sisemisi olekuid või tehes matemaatilist kontrollimist

Mõned uurijad töötavad välja meetodeid, et kontrollida mudelite ohutusega seotud omadusi senisest rangemalt. Ühe lähenemisviisi korral püüavad uurijad tõlgendada mudelite sisemisi arvutusi, et kas tuvastada riske või esitada veenvamaid argumente selle kohta, et mudel on ohutu (‡1285, ‡1286). Näiteks tõestusidee (proof of concept) raames näitasid uurijad, et tööriistad keelemudeli sisemise arvutuse analüüsimiseks võiksid aidata hindajatel tuvastada kahjulikke käitumisi (‡1287). Aastal 2025 hakkas Anthropic samuti analüüsima mudelite interne, et uurida mudeli situatsiooniteadlikkust ja „kavatsust“ (‡2). Ometi ei ole seda tüüpi meetodid praegu veel levinud ega teadaolevalt teistest hindamistehnikatest konkurentsivõimelised.

Turvalisuse tugevamate tagatiste saamiseks võib kasutada teistsugust lähenemisviisi, mis seisneb matemaatiliste tõestuste koostamises, et näidata, et mudel vastab teatud turvanõuetele (‡1177, ‡1282, ‡1288). Need tõestused eeldavad siiski, et testimise kontekst vastab kasutuselevõtu kontekstile, ning neid pole paljude eri tüüpi ründajate vastu kontrollitud.

Neid ei saa ka praegu skaleerida suurtele mudelitele. Üldiselt on ekspertide seas märkimisväärne arutelu tõlgendatavuse ja formaalse kontrollimise meetodite lubaduse üle.

###@ Kasutuselevõtuaja seire ja juhtimine

Lisaks mudeli arenduse käigus rakendatud kaitsemeetmetele on kahjulikku käitumist tõkestav teine kaitseliin välised kaitsemeetmed, mis keskenduvad mudeli või süsteemi tegevuste seirele ja kontrollile juurutamise ajal. Sellised kaitsemeetmed aitavad leevendada tõrkeid ja väärkasutust, näiteks hallutsineeritud väljundeid ja kahjulikke juhiseid.

>white|orangered|left|14|15.5|bb Mudelite kasutuselevõtjad saavad kasutada mitmesuguseid tööriistu, et tuvastada ja käsitleda suure riskiga mudeli käitumisviise

Kui tehisintellektisüsteem töötab, saab juurutaja jälgida riskimärke ja sekkuda, kui need ilmnevad. Näiteks saab ta kontrollida mudeli sisendeid, et tuvastada märgidadversaarsetest rünnakutest, filtreerida väljunditest sobimatut sisu või jälgida süsteemi mõttekäiku (chain of thought), et tuvastada märke kahjulikest plaanidest. Punti, kus juurutajad saavad jälgida ja sekkuda, kuidas inimesed nende süsteeme kasutavad, on muu hulgas riistvara (‡1180, ‡1181), kasutajate tegevused (‡1154, ‡1166), sisendid ja väljundid (‡65, ‡725, ‡1182), sisemised arvutused (‡744, ‡1183, ‡1184) ning mõttekäik (‡430, ‡435). Lisaks on olemas mitu toimingut, mida juurutajad saavad teha, kui riskid tuvastatakse. Nende hulka kuuluvad info logimine, kahjulikku sisu filtreerimine/muutmine, ebatüüpilise tegevuse märgistamine, süsteemi seiskamised või turvameetmete (failsafes) käivitamine. Kujund 3.7 illustreerib näiteid levinud jälgimis- ja juhtimismehhanismidest.

Kuna need mehhanismid on paindlikud ja sageli tõhusad, kasutatakse neid laialdaselt ning need võivad ära hoida paljusid liike tahtmatuid kahjusid (‡725, ‡751, ‡1289). Need kaitsed ei ole siiski täiuslikud, eriti pahatahtlike rünnakute korral, mis on optimeeritud nende läbikukkuma panemiseks (‡752, ‡1182). Hiljutised uuringud on samuti uurinud, kuidas jälgimine võib olla ebausaldusväärne, kui süsteemi optimeeritakse jälguri skooride põhjal, näiteks muutes arutluse ahela (chain of thought) vähem usaldusväärseks (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Kujund 3.7: Seire- ja juhtimismeetodid
>white|black||9|11|br Jälgimis- ja kontrollimeetodid toimivad mitmes kohas: ohtliku sisuga seotud sisendite ja väljundite sõelumine, sisemiste mudeli olekute jälgimine, väliste tegevuste piiram ine liivakast keskkonna (sandboxing) abil ning inimliku järelevalve tagamine. Allikas: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Inimeste kaasamine võimaldab suure riskiga olukordades otsest järelevalvet

Vigade tõenäosuse vähendamiseks AI agendide puhul (vt §2.2.1. Usaldusväärsuse väljakutsed) saavad juurutajad eesmärgiks seada AI-süsteemid, mis töötavad koostöös inimestega, mitte täielikult autonoomselt (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). See on oluline kasutusjuhtudel, kus valed otsused võivad põhjustada märkimisväärset kahju, näiteks rahanduses, tervishoius või politseitöös. Kuid „inimene ahelas“ on sageli ebapraktiline. Mõnikord toimub otsustamine liiga kiiresti, näiteks vestlusrakendustes koos miljonite kasutajatega. Teistel juhtudel võivad inimeste eelarvamused ja vead riske võimendada, kuna vead kuhjuvad (‡1187). Inimesed ahelas kipuvad ka ilmutama „automaatika eelarvamust“, mis tähendab, et nad annavad AI-süsteemile sageli rohkem usaldust, kui see on põhjendatud (‡1190, ‡1191) (vt §2.3.2. Ohud inimese autonoomiale).

>white|orangered|left|14|15.5|bb „Liivakastimine“ kaitseb autonoomsest käitumisest tulenevate riskide eest

AI agendid, mis suudavad tegutseda iseseisvalt ilma piiranguteta veebis või füüsilises maailmas, kujutavad endast suurenenud riske (vt §2.2.1. Usaldusväärsuse väljakutsed). „Sandboxing“ tähendab seda, et piiratakse viise, kuidas AI agendid saavad maailma otseselt mõjutada, muutes nende järelevalve ja haldamise palju lihtsamaks (‡640, ‡1192, ‡1295). Näiteks AI-süsteemi võimekuse piiramine internetti postitamiseks või arvuti failisüsteemi muutmiseks võib ära hoida ettenägematud kahjud ettenägematute tegevuste tagajärjel (‡1296). Siiski ei saa selliseid lähenemisviise alati kasutada rakendustes, kus AI-süsteem peab tingimata tegutsema maailma vahetult.

###@ Ökosüsteemi seire tööriistad: mudeli ja andmete päritolu (provenants)

Mudel- ja andmete päritolu vahendid on tehnilised vahendid AI-ökosüsteemi uurimiseks, et parandada arusaamist AI-süsteemide järelduvast kasutusest ja mõjudest.

>white|orangered|left|14|15.5|bb AI-süsteemi päritolutõendamise tehnikad aitavad jälgida süsteemide kasutusi ja mõjusid

Arendajad ja kasutusele viijad saavad kasutada mitmesuguseid tehnikaid, et uurida mudeli kasutust ja levikut “reaalses maailmas”. Näiteks võivad nad anda mudelitele unikaalseid identifitseerivaid käitumismustreid (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) või rakendada unikaalseid mustreid üksikute avatud lähtekoodiga kaaludega mudelite (open-weight) kaaludele (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Kuid nende tehnikate muutmiskindlamaks muutmine on avatud probleem (‡1195, ‡1196*). Teadlased töötavad samuti meetoditega “mudeli päritolu tuvastamiseks” (‡1197, ‡1198, ‡1305, ‡1306), mis aitab vastata küsimustele, mille kuju on: “Kas mudel X oli mudeli Y peenhäälestatud (fine-tuned) või destilleeritud (distilled) versioon?” Lõpuks arendavad mõned arendajad protokolle ja taristut AI-agentidele, et hõlbustada tuvastamist ja verifitseerimist, kui nad suhtlevad väliste süsteemidega (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Kujund 3.8: Vesimärgid manustavad piltidesse ja helisse tajumatuid häireid
>white|black||9|11|br Veejäljed manustavad kujutistesse ja helisse nähtamatuid häireid, mis võimaldavad AI-põhist loodud sisu tuvastada tuvastustööriistade abil. Selles kujundis on nii pildi kui ka heli veejaigud nähtavuse huvides liialdatud. Allikas: Chameleon’i pilt teenusest Unsplash (‡1313*). Muud elemendid on loonud aruande autorid. Rahvusvaheline AI ohutusaruanne 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Kujund 3.9: Prompti süstimise ründe edukuse määrad
>white|black||9|11|br Prompt-injitsi rünnakute edukusprotsendid, nagu on esitanud AI arendajad suuremate mudelite puhul, mis anti välja ajavahemikus alates maist 2024 kuni augustini 2025. Iga punkt tähistab edukate rünnakute osakaalu 10 katse jooksul antud mudeli suhtes vahetult pärast väljaandmist. Selliste rünnakute väidetav edukusprotsent on aja jooksul vähenenud, kuid püsib siiski suhteliselt kõrge. Allikas: Zou et al. 2025 (‡1149), viidatud dokumendis Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb AI-sisu tuvastamise tehnikad aitavad jälgida AI-loodud sisu levikut ja selle mõjusid

Vesimärgid, metaandmed ja muud tehisintellekti sisutuvastajad võivad aidata teadlastel jälgida ja uurida tehisintellekti loodud sisu tegelikku mõju maailmas. 

Esiteks on andmete veemärgid kerged, kuid selgelt eristatavad motiivid, mis sisestatakse digitaalsesse meediasse ja võivad kodeerida teavet nende päritolu kohta (‡1199, ‡1200, ‡1201*). Teksti puhul on need tavaliselt peened kallutused sõnavaliku ja stiili osas (‡1308, ‡1309); piltide ja video puhul peened mustrid piksli-kihtidel (‡1310); ja heli puhul peened mustrid helilainetes (‡1311). Kujund 3.8 illustreerib neid.

Lisaks vesimärkidele saab tehisintellekti loodud sisu salvestada ka failivormingutega, mis talletavad metaandmeid selle kohta, kuidas see loodi. Näiteks paljud mobiilseadmed salvestavad pildi- ja helifaile failivormingus, mis suudab talletada teavet kaamera seadistuste, aja, asukoha jms kohta. (‡1312). Sarnaseid metaandmeid saab kasutada ka selle kohta teabe talletamiseks, kas andmed loodi tehisintellektisüsteemiga. Nagu sõrmejälgede kasutamine kriminaalforensis, saab vesimärke ja metaandmeid muuta või eemaldada, kuid need on sellegipoolest kasulikud.

Teadlased töötavad ka selle nimel, et töötada välja tehisintellekti loodud sisu detektorid (‡1203, ‡1204, ‡1205*), et aidata tuvastada tehisintellekti loodud sisu päriselus, isegi kui pole saadaval ei märgendust ega metaandmeid. Kuid neil tuvastusmeetoditel on piiratud eduvõime.

###@ Värskendused

Alates viimase aruande avaldamisest (jaanuar 2025) on tehtud edusamme tehisintellektisüsteemide väljatöötamisel, millel on mitu tõhusat kaitsekihti. Nagu on arutatud jaotises §3.2. Riskijuhtimise tavad, on defence-in-depth riskijuhtimise põhipõhimõte (‡1314). Näiteks tehisintellektisüsteeme, mis ühendavad ohutuskoolitusega mudeleid sisendifiltrite, väljundifiltrite ja muude sisukontrollidega, uuritakse üha enam ning võetakse üha sagedamini kasutusele (‡32, ‡65, ‡1182*). Hiljutised uuringud on samuti näidanud, et kuigi mudelihaldurid on teinud edusamme suutlikkuse suurendamisel kaitsemeetmete eiramiseks tehtud katsetele vastupidamiseks, õnnestub ründajatel endiselt kõrge määraga (Kujund 3.9).

###@ Tõenduslüngad

Vaja on rohkem tõendeid, et aidata teadlastel mõista ja arvesse võtta olemasolevate lähenemisviiside piiranguid. Tehisintellektisüsteemide tehnilisi turvameetmeid täiustatakse, kuid meetodid kannatavad piirangute all. Näiteks edasiminek üldotstarbeliste AI-süsteemide halvima juhu robustsuse parandamisel on olnud aeglane ning on olemas fundamentaalsed piirangud selle suhtes, kui põhjalikult saab avatud kaalu (open-weight) mudeleid kaitsta ja jälgida (‡1195, ‡1315, ‡1316) (vt ka §3.4. Avatud kaalu mudelid). Vahepeal ei ole kõik tehnilised turvameetmed võrdselt levinud, võrdselt tõhusad ega võrdselt reaalses maailmas tõestatud. Näiteks kasutatakse vastandkoolitust peaaegu kõikjal tipptasemel (state-of-the-art) mudelites (‡64*, ‡677), samas kui mudeli interpreteeritavuse ja formaalse tõestamise meetodeid on siiani tootmissüsteemides vähe kasutatud (‡1177, ‡1285).

###@ Väljakutsed poliitikakujundajatele

Poliitikakujundajate jaoks on peamised väljakutsed otsustada, kas ja kuidas nad peaksid toetama teadusuuringuid, arendust, hindamist ning tehniliste kaitsemeetmete ja seiremeetodite kasutuselevõttu. See on keeruline, sest teadlaste arusaam sellest, kuidas kõige paremini praktiliselt mehhanisme kaitsta, on endiselt kujunemisjärgus ning parimad tavad pole veel välja kujunenud. Näiteks kasutavad erinevad arendajad erinevaid kaitsemeetmeid ning nende lähenemised tehnilise riski maandamisele laiemalt varieeruvad samuti suurel määral (‡1116). Lõpuks ei taga tõhusate tehniliste kaitsemeetmete olemasolu ainuüksi ohutust, kuna kasutuselevõtt ja rakendamine võivad erineda arendajate ja juurutamise kontekstide lõikes.

