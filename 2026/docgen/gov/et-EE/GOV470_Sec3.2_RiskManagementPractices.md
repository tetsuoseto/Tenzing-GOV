##########
>white|orangered|left|14|30|hr 3.2 jaotis
### 3.2. Riskijuhtimise tavad
>white|orangered|left|24|30|hb Riskijuhtimise tavad

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb Oluline teave
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Üldotstarbelise tehisintellekti riskijuhtimine hõlmab mitmesuguseid tegevusi, mida kasutatakse üldotstarbelisest tehisintellektist tulenevate riskide tuvastamiseks, hindamiseks ja vähendamiseks. Nende hulka kuuluvad mudeli-taseme testimine ja hindamine (nt „red-teaming“), organisatsioonilised protsessid, mis suunavad arendamise ja väljalaske otsuseid, tingimusel põhinevad kaitsemeetmed (nt „if-then“ kohustused) ning intsidentidest teavitamine.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Mitmed tehisintellekti arendajad on loonud Frontier AI Safety Frameworks (eesrindliku tehisintellekti ohutuse raamistikud). Need raamistikud sisaldavad teavet riskihindamiste kohta ning määratlevad tingimuslikke meetmeid, nagu juurdepääsupiirangud, mida ettevõtted kavatsevad rakendada võimekamate mudelite puhul. Need erinevad selle poolest, milliseid riske nad hõlmavad, kuidas nad määratlevad võimekuse lävendid ning milliseid tegevusi käivitatakse, kui lävendid on saavutatud.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ AI riskijuhtimise tavade tegeliku mõju kohta päriselus on tõendusmaterjali endiselt piiratud. Intsidendiaruandluse ja seire puudumine muudab raskeks hinnata, kui hästi kehtivad tavad riske vähendavad, või kui järjepidevalt neid rakendatakse.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Pärast eelmise aruande avaldamist (jaanuar 2025) on riskijuhtimine muutunud uute tööstus- ja valitsemisalaste algatuste kaudu struktureeritumaks. Uued instrumendid, nagu ELi üldotstarbelise tehisintellekti käitumisjuhend, Hiina tehisintellekti ohutuse juhtimise raamistik 2.0 ning G7 Hiroshima tehisintellekti protsessi aruanderaamistik, koos ettevõttepõhiste algatustega näitavad suundumust standardiseeritumate lähenemisviiside poole läbipaistvuse, hindamise ja intsidentidest teavitamise vallas.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Turudünaamika ja tehisintellekti arenduse tempo seavad täiendavaid väljakutseid. Konkurentsisurve tõttu võivad tehisintellektiettevõtted seista silmitsi valikutega kiiremate tooteväljalasete ja riskide vähendamisele tehtavate investeeringute vahel. Paljud tehisintellektiga seotud kahjustused jäävad samuti teiste kanda ning nende eest vastutava juriidilise vastutuse ulatus on endiselt ebaselge ning juhtimisprotsessid võivad olla aeglased kohanema muutustega tehisintellekti maastikul.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Poliitikakujundajate peamised väljakutsed hõlmavad prioriteetide seadmist erinevate riskide hulgas, mida tekitab üldotstarbeline tehisintellekt, ning selgitamist, millised osalised kogu AI väärtusahelas on nende leevendamiseks kõige paremini positsioneeritud. Neid väljakutseid süvendab piiratud arusaam sellest, kuidas riske praktikas tuvastatakse, hinnatakse ja hallatakse, samuti arendajate, kasutusele võtjad ja taristu pakkujate vaheline killustunud infovahetus.
>oldlace|black||11|15|br      


AI riskihaldus hõlmab mitmesuguseid tegevusi, mille eesmärk on tuvastada, hinnata ja vähendada AI-süsteemidega seotud riskide tõenäosust ja tõsidust. Neid tegevusi saab rakendada AI arendajate, kasutuselevõtjate, hindajate ja reguleerivate asutuste poolt. Näited hõlmavad ohumodelleerimist, riskide liigistamist, punase meeskonna harjutusi (red-teaming), auditeerimist ja intsidentidest teatamist. Käesolev osa kirjeldab olemasolevaid riskihaldustavasid, uusi arenguid ja allesjäänud piiranguid.

Alates 2025. aasta algusest on välja töötatud mitu uut rahvusvahelist üldotstarbelise tehisintellekti (general-purpose AI) riskijuhtimise algatust, sealhulgas organisatsioonilise läbipaistvuse ja riskidest aruandluse raamistikud ning regulatiivsed ja juhtimisraamistikud.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Kujund 3.4: Riskijuhtimise neli komponenti
>white|black||9|11|br Üldotstarbelise tehisintellekti riskijuhtimise meetodite neli kategooriat: riski tuvastamine; riski analüüs ja hindamine; riski maandamine; ja riskijuhtimine. Need moodustavad iteratiivse ja tsüklilise protsessi. Keskel esitatud riskijuhtimine soodustab teiste komponentide õnnestumist. Allikas: International AI Safety Report 2026.


Järelejäänud väljakutsete hulka kuuluvad piiratud standardiseeritus, mis muudab vastavuse ja hindamise keeruliseks, ning piiratud tõendus materjal reaalse maailma tõhususe kohta. Lisaks on institutsionaalsed, kultuurilised ja poliitilised kontekstid üle maailma erinevad, mis tähendab, et lähenemised riskide tuvastamisele ja haldamisele, sealhulgas aktsepteeritavate riskipiiride määratlemisele, võivad piirkonniti erineda. Selle jaotise arutelu riskijuhtimise lähenemisviiside kohta on kirjeldav: selle eesmärk on teavitada AI ökosüsteemi osalisi praegustest ülemaailmsetest riskijuhtimise lähenemisviisidest. Kui see on olemas, käsitletakse nende lähenemisviiside tõhususe ja piirangute kohta esitatud tõendusmaterjali, kuid poliitikasoovitused ei kuulu käesoleva töö reguleerimisalasse.

###@ Riskijuhtimise komponendid

Riskijuhtimine on iteratiivne protsess, mille praktikaid ja meetodeid rakendatakse kogu AI arendus- ja kasutuselevõtu tsükli vältel, kuid mis töötavad omavahel koherentselt (‡969). Üldotstarbelise AI riskijuhtimisel võib olla rollid väga paljudele osalistele, sealhulgas andmeteadlased, mudeliehitajad, audiitorid, valdkonnaeksperdid, juhid, lõppkasutajad, mõjutatud kogukonnad, kolmandate osapoolte tarnijad, poliitikakujundajad, valitsused, standardiorganisatsioonid ja kodanikuühiskonna organisatsioonid (‡970, ‡971, ‡972). Juhtivad riskijuhtimise standardid on sageli omavahel ühilduvad, kuid kasutavad riskijuhtimise elementide kirjeldamiseks erinevat terminoloogiat (‡973, ‡974). Need sisaldavad tavaliselt nelja omavahel seotud komponenti (Kujund 3.4): riskide tuvastamine; riskide analüüsimine ja hindamine; riskide leevendamine; ja riskide juhtimine (‡970, ‡973, ‡975, ‡976). Allolevad Laudid esitavad asjakohaste meetodite, tehnikate ja tööriistade illustreerivaid näiteid. Praktikad arenevad jätkuvalt, mistõttu Laudid ei ole ammendavad ning rakenduvus sõltub kontekstist.

###@ Riskide tuvastamine

Riskide tuvastamine on protsess, mille käigus leitakse, märgatakse ja kirjeldatakse riske. Põhjalik riskide tuvastamine hõlmab tavaliselt võimekeskseid hinnanguid, mis testivad, kas mudelitel on kindlad ohtlikud võimed (‡977), samuti riskimodelleerimist (‡978) ja prognoosimist (‡715*), mida kasutatakse olemasolevate ja esilekerkivate riskide uurimiseks. Tabel 3.1 esitab mitmeid näiteid riskide tuvastamise praktikate kohta. Riskide tuvastamine tugineb ka asjakohaste ekspertide ja kogukondade kaasamisele, et mõista laiemat konteksti, kuidas riskid tekivad (‡979, ‡980). Sellised mehhanismid nagu bug bounty programmid võivad toetada seda protsessi, motiveerides varem tundmatute haavatavuste tuvastamist (‡981) (Tabel 3.1). Riskide tuvastamise üks peamisi eesmärke on arvestada nii hästi tuntud ja hästi mõistetud riskidega kui ka võimalike tulevaste riskidega, mis on endiselt ebakindlad või halvasti kirjeldatud (‡982). See on eriti oluline üldotstarbelise tehisintellekti puhul, kus paljud riskid ei pruugi veel täielikult mõistetavad ega vaadeldavad olla (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Veaotsingu programmid
  Vigade eest makstav preemiaprogramm või haavatavuse avalikustamise programmid motiveerivad inimesi leidma ja raporteerima haavatavusi tehisintellekti süsteemides. Mitmed arendajad on rakendanud vigade eest makstavaid preemiaprogramme (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Eksperdi nõustamine
  Domeeniasjatundjad, kasutajad ja mõjutatud kogukonnad annavad ülevaate tõenäolistest riskidest. Tekkimas on osalus- ja kaasava tehisintellekti suunised (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ishikawa kalaka skeem
  Kalaluuproovid on laialdaselt tunnustatud juurpõhjuste analüüsi tööriistad ning teadlased on pakkunud nende kasutamist AI-riski intsidentide struktureeritud analüüsiks (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Prognoosimine
  Ennustamine on protsess, mille käigus ennustatakse tulevasi sündmusi või suundumusi varasemate ja praeguste andmete analüüsi põhjal. Seda on kasutatud näiteks eri majanduslike tulemuste suhtelise tõenäosuse võrdlemiseks tänu arenenud tehisintellektile (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskitaksomoonia
  Riski taksonoomiad on viis riskide kategoriseerimiseks ja korraldamiseks mitme dimensiooni lõikes. On olemas mitu taksonoomiat, mis kirjeldavad riske üldotstarbelisest tehisintellektist (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Stsenaariumide kavandamine
  Stsenaariumide planeerimine hõlmab tõenäoliste tulevikustsenaariumide väljatöötamist ja analüüsimist, kuidas riskid realiseeruvad. Seda on kasutatud tehisintellektimudelitega (‡989) seotud riskide ja mõjude uurimiseks.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ohumodellimine
  Ohumudel (threat modelling) on protsess süsteemi ähvarduste ja haavatavuste tuvastamiseks. Mitmed tehisintellekti arendajad rõhutavad selle kasutamist, et ette näha võimalikke AI-süsteemide väärkasutamise stsenaariume (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Laud 3.1: Riskide tuvastamise näited üldotstarbelise tehisintellekti riskijuhtimises
>white|black||9|11|br AI riskide tuvastamise näidismeetodid on loetletud tähestikulises järjekorras. Kaasatud meetodid
on loodud toetama riskide tuvastamist paljude erinevate riskitüüpide lõikes, sealhulgas ohud pahatahtlikust kasutusest, ohud riketest ning süsteemsed riskid. Arvestades üldotstarbelise tehisintellekti riskijuhtimise alles varajast arengustaadiumi, ei sobi kõik meetodid igaühele nii tehisintellekti arendajate kui ka kasutuselevõtjate seas.


>white|orangered|left|14|15.5|bb Ohumudega modelleerimine ja riskitaksonoomiad on silmapaistvad riskituvastusmeetodid

Kaks silmapaistvat meetodit üldotstarbelise tehisintellekti riskide tuvastamiseks on ohumodelleerimine ja riskitaksonoomiad. Rahvusvaheline AI-ohutusaruanne 2026 esitab näiteks struktureeritud protsessi, mille kaudu kaardistada, kuidas AI-ga seotud riskid võivad realiseeruda, ning riskitaksonoomiaid. Meta kasutab näiteks ohumodelleerimise harjutusi, et ette näha võimalikke kuritarvitamise stsenaariume oma tehisintellekti mudelite puhul (‡990), ning Anthropic on lisanud ohumodelleerimise oma ASL-3 Deployment Standardisse (‡991). AI riski- ja ohutaksonoomiad, mis loetlevad riskikategooriaid ja näiteid, võivad samavõrd hästi toimida lähtepunktina, et mõtestada, tuvastada ja täpsustada üldotstarbelise tehisintellektiga seotud olulisi riske konkreetsetes rakendusvaldkondades (‡906, ‡988, ‡992, ‡993).

###@ Riskianalüüs ja hindamine

Riskianalüüs ja hindamine on protsess, mille käigus määratakse kindlaks AI-mudeli või -süsteemi riski tase ning võrreldakse seda kehtestatud kriteeriumidega, et hinnata aktsepteeritavust või vajadust leevendusmeetmete järele (‡994, ‡995, ‡996, ‡997). See hõlmab muu hulgas selliseid tegevusi nagu mudeli jõudluse mõõtmine võrdlusülesannete (‡998) ja hindamiste (‡176, ‡715) alusel, läbiviidavad red-teamingu harjutused (‡999*), mõjuhinnangud (‡1000) ning auditid (‡1001, ‡1002). Vaata Laul 3.2 üldotstarbelise AI riskianalüüsi ja hindamise näidete jaoks. Meetodid on ette nähtud selleks, et toetada analüüsi ja hindamist samaaegselt paljude erinevate riskitüüpide puhul.

Riskianalüüsi ja -hindamise võtmeeesmärgid on mudeli suutlikkuse ja haavatavuste hindamine (‡1003), usaldusväärse riskimudeldamise kasutamine otsuste tegemiseks riskilävede osas (‡1004, ‡1005) ning mõistmine, kuidas tehisintellektisüsteeme praktikas kasutatakse, et hinnata tagajärjelisi ühiskondlikke mõjusid (‡869, ‡904, ‡905, ‡1006). Riskianalüüsi ja -hindamise protsesse peetakse sageli tõenäolisemaks viisiks riskide tuvastamiseks siis, kui need hõlmavad sõltumatut läbivaatamist (‡1001, ‡1007), toetuvad valdkondadeülesele asjatundlikkusele (‡1008) ning sisaldavad erinevaid vaatenurki mitmest valdkonnast ja distsipliinist, samuti mõjutatud kogukondadest (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Auditid
  Auditid on ametlikud AI-mudelite toimivuse ja mõju ülevaated ning/ või organisatsiooni vastavuse kontrollid standarditele, poliitikatele ja protseduuridele, mida tehakse kas organisatsiooni siseselt või välise osapoole poolt. AI-auditeerimine on kiiresti kasvav valdkond ning AI-mudelite auditeerimiseks ja AI-mudelite arendajate tegevuste hindamiseks on olemas arvukalt tööriistu ja praktikaid (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Etalontestid
  Mõõdikud on standardiseeritud, sageli kvantitatiivsed testid või näitajad, mida kasutatakse AI-süsteemide jõudluse hindamiseks ja võrdlemiseks kindla ülesannete kogumiga, mis on loodud esindama reaalset kasutust (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bowtie meetod
  Vibuemeetod on laialt tuntud meetod selleks, et visualiseerida, kuhu kontrollid saab lisada riskisündmuste leevendamiseks. See annab selge eristuse proaktiivse ja reaktiivse riskijuhtimise vahel (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Delphi meetod
  Delphi-meetod on rühma otsustamise tehnika, mis kasutab eksperdirühmalt konsensuse kogumiseks mitme küsimustiku seeriat (‡1020, ‡1021). Seda on kasutatud selleks, et aidata uurida võimalikke tulevikke täiustatud tehisintellektiga (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Välikatsed
  Väljaseires testimine hindab tehisintelligentsüsteemi jõudlust ja mõju päris- maailma, töökindlas töökeskkonnas. Mõned uuringud rõhutavad väljaseires testimist kui mudeli hindamise täiendust reaalse maailma tulemuste ja tagajärgede hindamisel (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mõju hindamine
  Mõjuhinnangud hindavad tehnoloogia või projekti võimalikke mõjusid. See võib hõlmata mõjude kvantifitseerimist, koondamist ja prioriseerimist. Näiteks ELi tehisintellekti õigusakt nõuab suure riskiga tehisintellektisüsteemide arendajatelt Põhiõiguste mõjuhinnanguid (‡1024) läbi viia.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mudelihindamine
  Mudeli hindamised hõlmavad protsesse ja teste, et hinnata ning mõõta AI-mudeli sooritust konkreetsel ülesandel. AI-hindamisi on palju, et hinnata erinevaid võimeid ja riske, sealhulgas ohutuse, turvalisuse ja sotsiaalse mõju jaoks (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tõenäosuslik riskihinnang
  Tõenäosuslik riskihindamine on metoodika keeruliste süsteemide või protsessidega seotud riskide hindamiseks, mis hõlmab ebakindlust. Seda on kohandatud täiustatud tehisintellekti süsteemide jaoks (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Red-teaming
  Red-teaming on harjutus, mille käigus rühm inimesi või automatiseeritud süsteemid teesklevad vastast ja ründavad organisatsiooni tehnoloogilisi süsteeme, et tuvastada haavatavusi. Mitmed AI-ettevõtted kasutavad AI-süsteemide red-teamingu sisekordi (‡458, ‡1028). Red-teamingut saab läbi viia ka ettevõtete väliste tegijate poolt. Sellistel meeskondadel on väljakutseid, nagu piiratud juurdepääs, kuid nad saavad ka esile tuua eristavaid teadmisi (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskimaatriksid
  Riskimaatriksid on visuaalne vahend riskide prioriseerimiseks nende esinemise tõenäosuse ja võimaliku mõju alusel (‡1027). Mõned tehisintellekti arendajad lisavad oma Frontier AI Safety Frameworksidesse (‡1029*) põhilised riskimaatriksid.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskiläved / riskitasemed
  Riskiläved või tasemed on kvantitatiivsed või kvalitatiivsed piirangud, mis eristavad aktsepteeritavad ja mitteaktsepteeritavad riskid ning käivitavad konkreetsed riskijuhtimise meetmed, kui need on ületatud. Üldotstarbelise tehisintellekti puhul määratakse need võimekuse, mõju, arvutusressursi (compute), leviku (reach) ja muude tegurite kombinatsiooniga (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskitaluvus
  Riskitaluvus viitab riskitasemele, mida organisatsioon on valmis aktsepteerima. AI valdkonnas seatakse riskitaluvused sageli kaudselt ettevõtte poliitikate ja tegevuspraktikate kaudu, samas kui mõned regulatiivsed režiimid määratlevad selgesõnaliselt lubamatud riskid ja seovad nendega õiguslikud tagajärjed (‡1032). Mõned ettevõtted kirjeldavad oma riskitaluvust uue mudeli marginaalse riski kaudu; see tähendab ulatust, mille võrra mudel kontrafaktiliselt suurendab riski üle selle, mida juba tekitavad olemasolevad mudelid või muud tehnoloogiad (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ohutusjuhtumid
  Ohutusjuhtum on struktureeritud argument, mida toetavad tõendid ja mis näitab, et süsteemi on konkreetses kasutuskontekstis lubatav ohutult kasutada. Viimased kirjandusallikad (‡1037, ‡1038, ‡1039) on uurinud ohutusjuhtumeid piiriala tehisintellekti (frontier AI) süsteemide jaoks ning teatud Frontier AI ohutuse raamistikud viitavad neile (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Süsteemi turvaanalüüs
  Süsteemi ohutuse analüüs toob esile sõltuvused komponentide ja nendest moodustuva süsteemi vahel, et ette näha, kuidas süsteemse tasandi ohud võivad tekkida komponendi- või protsessiriketest või alamsüsteemide vahelistest interaktsioonidest, inimteguritest ja keskkonnatingimustest. Kirjanduses rakendatud lähenemised tehisintellekti süsteemidele hõlmavad süsteemiteoreetilist protsessianalüüsi (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Laud 3.2: Riskianalüüs/hindamine üldotstarbelise tehisintellekti riskijuhtimises
>white|black||9|11|br Näited AI-riski analüüsi/hindamise meetoditest, loetletud tähestikulises järjekorras. Arvestades üldotstarbelise AI riskijuhtimise veel kujunemisjärgus olevat olemust, ei sobi kõik meetodid iga AI arendaja või kasutuselevõtja jaoks.


>white|orangered|left|14|15.5|bb Levinud riskianalüüsi tööriistad hõlmavad võrdlusuuringuid ja mudeli hindamisi

Etalonid ja mudelite hindamised on standardiseeritud testid, et hinnata üldotstarbeliste tehisintellektisüsteemide toimivust konkreetsetes ülesannetes. Teadlased on välja töötanud laia valiku etalone ja hindamisi, sealhulgas rasked valikvastustega küsimustikud, tarkvaraarenduse probleemid ning töökohaga seotud ülesanded simuleeritud kontori keskkondades (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Kahjuliku võimekuse hindamisi (‡715) kasutatakse selleks, et hinnata, kas üldotstarbeline AI-mudel või -süsteem omab eriti ohtlikke teadmisi või oskusi, näiteks võimet aidata küberrünnakutes (vt §2.1.3. Küberrünnakud).

Ettevõtete ja valitsuste poolt mudelite vabastamisega seotud kõrgelt mõjukaid otsuseid tehakse osaliselt nende hinnangute põhjal (‡1050, ‡1051, ‡1052). Siiski on võrdlusaluste (benchmarkide) kvaliteet ja ulatus oluliselt erinevad (‡998, ‡1003) ning nende paikapidavust võib olla raske hinnata paljude puuduste tõttu võrdlusaluste koostamise ja kasutamise praktikas (‡902, ‡909, ‡1003, ‡1053*). Näiteks võivad võrdlusalused muutuda „küllastunuks“ – kui paljude mudelite skoorid lähenevad tipp-skoorile – mis tähendab, et need ei erista enam mudelite vahel selgelt. Samuti on mudelitel üha suurem tõenäosus tuvastada teatud ülesandeid hindamistena ja käituda erinevalt sellest, kuidas nad sarnastel ülesannetel toimiksid rakenduse (deployment) kontekstis, tulenevalt „olukorrateadlikkusest“ (vt §2.2.2. Kontrolli kaotus). Lõpuks on võrdlusalustel ja hinnangutel hästi dokumenteeritud piirangud: eelkõige ei suuda need tabada ohte, mis on seotud üldotstarbelise tehisintellekti kasutamisega uutes valdkondades ja uudsetes ülesannetes, sest katseseaded erinevad reaalsest kasutusest erineval määral (‡913) (vt §1.2. Current capabilities ja §3.1. Technical and institutional challenges).

>white|orangered|left|14|15.5|bb Red-teaming võimaldab teha riskidest rohkem valdkonnaspetsiifilisi hinnanguid

Teine levinud meetod riskide hindamiseks on red-teaming. ‘Red team’ on hindajate rühm, kelle ülesanne on otsida haavatavusi, piiranguid või võimalikku kuritarvitamist. Red-teaming võib olla valdkonnapõhine ja seda teevad valdkonna eksperdid, või ka avatud lähenemine uute riskitegurite uurimiseks. Näiteks võib red team uurida ‘jailbreaking’u’ rünnakuid, mis rikuvad mudeli ohutuspiiranguid (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). Erinevalt võrdlusülesannetest (benchmarks) on red-teamingu üks peamisi eeliseid see, et red team’id saavad kohandada oma hindamisi konkreetsele testitavale süsteemile. Näiteks saavad red team’id kujundada kohandatud sisendeid, et tuvastada halvimad käitumismustrid, pahatahtliku kasutuse võimalused ja ootamatud tõrked. Samas võib see nõuda mudelitele eripääsu ja võib ebaõnnestuda oluliste riskiliikide esiletoomisel (‡999, ‡1028).

Oluline on see, et tuvastatud riskide puudumine ei tähenda, et need riskid oleksid madalad: varasem töö näitab, et vead jäävad sageli avastamata, eriti kui red meeskondadel on piiratud ligipääs või ressursid (‡1060). Uuringud on samuti seadnud kahtluse alla, kas red-teaming suudab anda usaldusväärseid ja korratavaid tulemusi (‡1061). Red-meeskonna koosseis ja red-teameritele antud juhised (‡1062), rünnakukierdude arv (‡1063) ning mudeli ligipääs tööriistadele (‡1064, ‡1065) võivad oluliselt mõjutada tulemusi, sealhulgas kaetud riskipinna ulatust. Põhjalikud juhised red-teamingu jaoks püüavad lahendada mõningaid neist väljakutsetest (‡1066).

###@ Riskide maandamine

Riskide maandamine on protsess, mille käigus seatakse prioriteedid, hinnatakse ning rakendatakse kontrollimeetmeid ja vastumeetmeid, et vähendada tuvastatud riske. Näited on juurdepääsukontrollid (‡991), pidev seire (‡986) ja kui-siis kohustused (‡700). Riskide maandamine tekitab olulise küsimuse: milline on aktsepteeritav riskitase? Hiljutised raamistikud ja ettevõtte eeskirjad on hakanud vormistama „riskiga nõustumise“ (risk acceptance) kriteeriume (‡965, ‡1040). Siiski on sobivate läviväärtuste määramine endiselt keeruline, eriti riskide puhul, millel on laialdane ühiskondlik mõju (‡986, ‡1067). Hetkel puudub väljakujunenud mehhanism riskiga nõustumise otsuste valideerimiseks, mille on teinud arendajad enne väljalaset (‡1005).

Allpool kirjeldatud Tabel 3.3 riskide maandamise meetodid on kohandatavad ja võivad maandada mitmesuguseid riske, sealhulgas mõningaid ettenägematuid riske. Tabel ei sisalda tehnilisi maandamisviise, nagu vastandlik treening, sisufiltrid ja mõttekäigu jälgimine. Nendega on kaetud §3.3. Tehnilised kaitsed ja järelevalve ning kogu Raportis jaotise „Mitigations” lõikudes iga §2. Riskide all oleva riski puhul.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Aktsepteeritava kasutamise eeskirjad
  Lubamatu kasutuse poliitika on reeglite ja juhiste kogum AI-mudelite vastutustundlikuks, eetiliseks ja õiguslikult nõuetekohaseks kasutamiseks. On tavaline, et AI arendajad avaldavad uute mudeliväljalasetega (‡1068, ‡1069) lubatava kasutuse poliitikaid ning ka keelatud kasutuse poliitikaid.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Juurdepääsukontroll/kasutaja kontrollimine
  Juurdepääsukontroll hõlmab eeskirjade ja reeglite kasutamist, et piirata juurdepääsu AI-mudelitele, andmetele ja süsteemidele kasutaja rollide, atribuutide ning muude tingimuste alusel, et vältida volitamata kasutust, manipuleerimist või andmetega seotud rikkumisi. AI-ettevõtted keelavad sageli kontod, mis on tuvastatud tegelemas kriminaalse tegevusega (‡486) ning lisavad kasutajate taustakontrolli ja Know-Your-Customer-i kontrollid, et tagada, et mudeleid kasutatakse üksnes usaldusväärsete osapoolte poolt (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Käitumise/mudeli spetsifikatsioon
  Tehisintellekti käitumisspetsifikatsioon on dokument, mis määratleb, kuidas tehisintellekti mudel peaks erinevates olukordades käituma. See toimib plaanina tehisintellekti ühitamise (alignment) ja ohutuse tagamisel, suunates mudeli arendust, koolitust, hindamist ja väljundeid. Mitmed tehisintellekti ettevõtted kasutavad mudeli spetsifikatsioonidokumente ja teevad vähemalt osa neist avalikuks (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pidev seire
  Pidev seire on pidev, automatiseeritud protsess, mille käigus jälgitakse, analüüsitakse ja kontrollitakse kasutusel olevaid tehisintellekti süsteeme, jälgitakse nende toimivust ning piiratakse nende käitumist, et tagada usaldusväärsus, tõhusus ja ohutus. Pidevaks seireks on saadaval arvukalt tööriistu (‡1073*) ning samuti on olemas tehnikaid toetuseks
AI jälgitavus (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sügavkaitse
  Kaitse sügavuti on idee, et võimalik on rakendada mitu sõltumatut ja kattuvat kaitsekihti, nii et kui üks neist ebaõnnestub, on teised ikkagi tõhusad (‡1075, ‡1076). Mitmed Frontier AI Safety Frameworks viitavad sellele (nt (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ökosüsteemi seire
  See on laiemat tehisintellekti ökosüsteemi jälgimise protsess, sealhulgas andmetöötlusvõime ja riistvara jälgimine, mudeli päritolu, andmete päritolu ning kasutusmustrid. Teaduskirjandus käsitleb sellist jälgimist seoses üldotstarbelise tehisintellekti (‡690) riskidega.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kui-siis kohustused
  Kui-siis-kohustused on tehniliste ja organisatsiooniliste protokollide ning kohustuste kogum riskide haldamiseks, kui tehisintellekti mudelid muutuvad võimekamaks. Mitmed tehisintellekti arendajad kasutavad seda tüüpi kohustusi osana oma Frontier AI Safety Frameworks’idest (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Punased jooned või keeldud
  Punased jooned on konkreetsed piirid, mis on väljendatud võimete, mõju või kasutusviiside liikidena. Mõiste esineb avalikes avaldustes ja algatustes, samuti regulatiivsetes keeludes (‡1079, ‡1080, ‡1081). Kirjandus toob samuti välja punasjoonte lähenemisviiside piirangud, sealhulgas väljakutsed seoses üksmeele saavutamise ja rakendatavusega.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Väljalaske- ja juurutamisstrateegiad
  Üldotstarbelise tehisintellekti (AI) väljalaske- ja juurutamisstrateegiates võib kasutada astmelisi väljalaskeid või API-le juurdepääsu, et väärkasutuse või ettenägematu kahju korral oleks saadaval rohkem leevendusvõimalusi (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Laud 3.3: Riskide maandamine üldotstarbelise AI riskihalduse kontekstis
>white|black||9|11|br AI riskide maandamiseks loetletud näidismeetodid on järjestatud tähestikulises järjekorras. Kaasatud meetodid on mõeldud selleks, et toetada riskide maandamist paljude eri riskitüüpide korral üheaegselt, sealhulgas pahatahtlikust kasutusest tulenevate riskide, rikketest tulenevate riskide ja süsteemsete riskide korral. Arvestades üldotstarbelise tehisintellekti riskijuhtimise esialgset (alles kujunemisjärgus) olemust, ei pruugi kõik meetodid sobida igale AI arendajale või kasutuselevõtjale.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Kujund 3.5: “Šveitsi juustu” skeem, mis illustreerib kaitse mitmekihilisuse lähenemist
>white|black||9|11|br Mitmekihilised kaitsed võivad korvata üksikute kihtide puudusi. Praegustel AI riskijuhtimise tehnikatel on puudusi, kuid nende kihistamine võib pakkuda tunduvalt tugevamat kaitset riskide vastu. Allikas: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Kaitse sügavuti ja vabastamisstrateegiad on olulised maandamismeetmed

„Kaitse mitmekihilisuse“ mudel võib toetada üldotstarbelise tehisintellekti riskihaldust. Selles kontekstis „kaitse mitmekihilisus“ viitab tehniliste, organisatsiooniliste ja ühiskondlike meetmete kombinatsioonile, mida rakendatakse arengu ja kasutuselevõtu erinevatel etappidel (Kujund 3.5). See tähendab sõltumatute kaitsekihtide loomist, nii et kui üks kiht peaks ebaõnnestuma, saavad teised kihid siiski ära hoida kahju. Üks sageli viidatud näide kaitse mitmekihilisuse mudelist on nakkushaiguste ennetamiseks kasutatav ennetusmeetmete valik. Vaktsiinid, maskid ja kätepesu ning muud meetmed võivad koos vähendada nakatumise riski märkimisväärselt, kuigi ükski neist meetoditest ei ole iseenesest 100% tõhus (‡1083*). Üldotstarbelise tehisintellekti puhul hõlmab kaitse mitmekihilisus kontrollseadmeid, mis ei ole tehisintellekti mudelis endas, vaid laiemas ökosüsteemis. See hõlmab näiteks kontrollseadmeid bioloogilise ründe teostamiseks vajalike materjalide, nagu reaktiivid, osas (‡1084, ‡1085). Kuid kaitse mitmekihilisuse meetmed tegelevad eelkõige õnnetuste, rikke ja pahatahtliku kasutamisega seotud riskidega ning võivad mängida väiksemat rolli süsteemsete riskide ohjamisel (vt §3.5. Ühiskondliku vastupanuvõime kujundamine).

Ettevõtte väljalaske ja kasutusele võtmise strateegia on oluline osa riskide maandamisel. Otsused selle kohta, kuidas mudeleid kasutajatele kättesaadavaks tehakse, võivad oluliselt mõjutada riskipositsiooni (‡1082). Erinevad väljalaske ja kasutusele võtmise võimalused hõlmavad etapiviisilist avaldamist piiratud kasutajate rühmadele, juurdepääsu kontrollitud veebiteenuste kaudu (näiteks API-de kaudu) ning litsentsilepingute ja aktsepteeritava kasutuse poliitikate kasutamist, mis õiguslikult keelavad teatud kahjuliku kasutuse (‡176, ‡1086, ‡1087). §3.4. Open-weight models käsitleb üksikasjalikumalt, kuidas mudeli kaalu(te) avaldamine riske mõjutab.

###@ Riskijuhtimine

Riskijuhtimine on protsess, mille kaudu riskijuhtimise hindamised, otsused ja tegevused seotakse organisatsiooni või muu üksuse strateegia ja eesmärkidega (‡1088, ‡1089). Tabel 3.4 annab ülevaate levinud riskijuhtimise tehnikatest. Nagu on näidatud joonisel 3.4, on riskijuhtimist võimalik mõista kui riskijuhtimise tuuma, kuna see võimaldab teiste riskijuhtimise komponentide tõhusat toimimist. See tagab vastutuse, läbipaistvuse ja selguse, mis toetavad põhjendatud riskijuhtimisotsuseid. Riskijuhtimine võib hõlmata selliseid tavasid nagu juhtumistest teavitamine (‡1090), riskivastutuse jaotuse määramine (‡965) ning teavitaja kaitse (‡1091). Laialdasemalt võib riskijuhtimine hõlmata juhiseid, raamistikku, õigusakte, regulatsioone, riiklikke ja rahvusvahelisi standardeid, samuti koolitus- ja haridusalgatusi. Riskijuhtimise üks peamisi eesmärke on kehtestada organisatsiooni poliitikad ja mehhanismid, mis selgitavad, kuidas riskijuhtimise vastutused jaotatakse organisatsiooni või muu üksuse lõikes, et toetada asjakohast järelevalvet ja vastutust (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dokumentatsioon
  Dokumenteerimistavad aitavad jälgida AI-süsteemide jaoks olulist teavet, nagu treeningandmed, disainiotsused, kavandatud kasutusviisid, piirangud ja riskid. „Model cards“ (mudelikaardid) ja „system cards“ (süsteemikaardid), mis annavad teavet selle kohta, kuidas AI-mudel või -süsteem treeniti ja hinnati, on näited silmapaistvatest AI dokumenteerimistavade parimatest praktikatest (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Juhtumist teatamine
  Hendekaarditeate esitamine on protsess, mille käigus dokumenteeritakse süstemaatiliselt ja jagatakse juhtumeid, kus arenev või kasutusele võetud AI on põhjustanud otsest või kaudset kahju. On mitmeid platvorme, mis hõlbustavad AI-i hendekaarditeate esitamist (‡1096, ‡1097), ning raamistikke, mis võimaldavad tõhusamat AI-i hendekaarditeate esitamist (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskijuhtimise raamistikud
  Riskijuhtimise raamistikud on organisatsioonilised plaanid riskikatte lünkade vähendamiseks, erinevate riskijuhtimise tegevuste koordineerimiseks ning kontroll- ja tasakaalumeetmete rakendamiseks. Üldotstarbelisele tehisintellektile (‡986, ‡1098) spetsiifilised raamistikud viitavad sageli käesolevas jaotises mainitud teistele meetmetele.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskiregister
  Riskiregister on erinevate riskide, nende prioriseerimise, vastutajate ja leevendusplaanide hoidla. Need on paljudes valdkondades suhteliselt levinud, sealhulgas küberturvalisus (‡1099), ja neid kasutatakse mõnikord selleks, et täita regulatiivse vastavuse nõudeid.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskide vastutuse jaotamine
  Rollide ja vastutuste jaotamine riskijuhtimise jaoks organisatsioonis võib kujundada sisemise järelevalve otsuste tegemise üle (‡1002, ‡1093). Sellised korraldused kajastuvad mõnes juhtimisraamistikus, sealhulgas ELi üldotstarbelise tehisintellekti tegevusjuhises (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Läbipaistvusaruanded
  Läbipaistvusaruanded kirjeldavad AI-ettevõtte riskijuhtimise tavasid, avalikustades teatud teavet või jagades dokumentatsiooni tööstusharu ühenduste või valitsusasutustega. Näiteks esitab arvukalt AI-ettevõtteid Hiroshima AI Process (HAIP) läbipaistvusaruandeid (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teavitaja kaitse
  Kuna suur osa AI arendusest toimub suletud uste taga, sisaldavad mõned valitsemisraamistikud teavitaja kaitset, et võimaldada potentsiaalsete ohtude avalikustamist ametiasutustele (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Laud 3.4: Riskihaldus üldotstarbelise AI riskijuhtimises
>white|black||9|11|br Alustelised AI riskijuhtimise näidismeetodid on loetletud tähestikulises järjestuses. Kaasatud meetodid on kavandatud toetama riskijuhtimist korraga paljude erinevate riskitüüpide jaoks, sealhulgas pahatahtlikust kasutusest tulenevad riskid, riketest tulenevad riskid ja süsteemsed riskid. Arvestades üldotstarbelise tehisintellekti riskijuhtimise alles kujunemisjärgus olevat olemust, ei sobi kõik meetodid iga tehisintellekti arendaja või kasutuselevõtja jaoks.


>white|orangered|left|14|15.5|bb Dokumenteerimine ja läbipaistvus on riskijuhtimise komponendid

Dokumenteerimise ja institutsionaalse läbipaistvuse mehhanismid koos teabejagamise tavadega hõlbustavad välist kontrolli ja toetavad üldotstarbelise tehisintellektiga (‡1101, ‡1102) seotud riskide haldamise jõupingutusi. On saanud tavapäraseks avaldada enne kasutuselevõttu tehtud testide tulemused „model card’i“ või „system card’i“ vormis koos põhiteabega mudeli või süsteemi kohta, sealhulgas selle kohta, kuidas see on treenitud, ning millised on selle võimalikud piirangud (‡1094, ‡1095). Mõned arendajad avaldavad ka läbipaistvusaruandeid, mis sisaldavad üksikasju nende riskihalduse tavade kohta laiemalt (‡1103). Teised dokumendi- ja läbipaistvuse elemendid hõlmavad seiret ja intsidentidest teavitamist (‡176, ‡1083*, ‡1103) ning teabejagamist, mida võivad toetada kolmandad osapooled, näiteks Frontier Model Forum. Mõned regulatiivsed raamistikud, nagu ELi AI Act või California’s Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53) (‡1081, ‡1104), näevad mõnel juhul ette teabe jagamise üldotstarbelise tehisintellektiga seotud riskide kohta.

>white|orangered|left|14|15.5|bb Juhtkonna pühendumus ja stiimulid kujundavad riskijuhtimise tavasid

Organisatsioonikultuur, juhtimisstruktuur ja stiimulid mõjutavad riskijuhtimisealaseid jõupingutusi mitmel viisil (‡1105). Juhtkonna pühendumus ja stiimulite ülesehitus on sageli asjakohased selle suhtes, kuidas riskijuhtimise poliitikad praktikas toimivad. Mõnel arendajal on sisemised otsustuskomisjonid, mis arutlevad selle üle, kuidas kavandada, välja töötada ja uute tehisintelligentsussüsteemide üle ohutult ja vastutustundlikult järele vaadata. Järelevalve- ja nõuandekomiteed, usalduskogud või tehisintellekti eetikapõhimõtete juhatused võivad samuti toimida mehhanismidena riskijuhtimise juhiste ja organisatsioonilise järelevalve tagamiseks (‡1092*, ‡1106, ‡1107, ‡1108). Teadlased on väitnud, et vabatahtliku eneseregulatsiooni probleemid tähendavad, et kolmandate osapoolte auditeerimine, verifitseerimine ja standardiseerimine võiks aidata tugevdada üldotstarbelise tehisintelligentsi riskijuhtimist (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Organisatsiooniline riskijuhtimine, läbipaistvus ja riskidest teavitamise raamistikud

Mitu uut algatust keskendub riskijuhtimise protsessidele, dokumenteerimisele ja läbipaistvusele. Oma praegusel kujul toimib ELi üldotstarbelise tehisintellekti tegevusjuhis (General-Purpose AI Code of Practice) vabatahtliku raamistikuna, mis juhib läbipaistvuse, autoriõiguse ning ohutuse ja küberjulgeoleku (safety and security) tavade järgimist, et toetada vastavust ELi tehisintellekti käsitleva õigusakti (EU AI Act) üldotstarbelist tehisintellekti puudutavatele sätetele (‡965). Alates detsembrist 2025 on selle alla kirjutanud rohkem kui kaks tosinat ettevõtet†. G7 Hiroshima tehisintellekti protsessi (HAIP) aruandlusraamistik (‡1100) on esimene rahvusvaheline raamistik vabatahtlikuks avalikuks aruandluseks organisatsioonide riskijuhtimise tavade kohta arenenud tehisintellektisüsteemide puhul. Vähemalt 20 arendajat on avaldanud avalikud läbipaistvusaruanded, mis käsitlevad riskide tuvastamist, hindamis( hindamis )mõõdikuid, leevendusstrateegiaid ning andmekaitse protsesse.

AI arendajad on võtnud kasutusele vabatahtlikud läbipaistvuse lubadused. Hiinas avaldati 17 Hiina AI-ettevõtte kohustused, mida koordineeris Hiina AI tööstusliit, detsembris 2024 (‡1113) ning neid uuendati 2025. aastal (‡1114). Lõuna-Koreas toimunud 2024. aasta maisel AI Seoul Summit’il leppis 16 mitmest riigist pärit AI arendajat vabatahtlikult kokku, et avaldavad Frontier AI Safety Frameworks (Frontier’i AI ohutuse raamistikud) oma kõige võimekamate mudelite ja süsteemide jaoks ning võtavad kasutusele riskijuhtimise tavad kogu mudeli arendamise ja kasutuselevõtu etappides (‡1052).

    Märkus † -- Allakirjutajad alates detsembrist 2025 hõlmavad: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing ja WRITER.

>white|orangered|left|14|15.5|bb Ešeloni tehisintellekti ohutuse raamistikud on saanud AI-riski juhtimise silmapaistvaks organisatsiooniliseks lähenemisviisiks

Alates 2023. aastast on mitmed juhtivad tehisintellekti arendajad avaldanud vabatahtlikult dokumendid, milles kirjeldatakse, kuidas nad kavatsevad tuvastada ja reageerida tõsistele riskidele oma kõige arenenumatest süsteemidest. Need Frontier AI Safety Frameworks (eesrindliku tehisintellekti ohutuse raamistikud) kirjeldavad, kuidas tehisintellekti arendaja kavatseb oma kõige arenenumaid tehisintellekti mudeleid ja süsteeme enne kasutuselevõttu ja selle ajal hinnata, jälgida ning kontrollida. Nendel raamistikudel on palju sarnasusi, kuid need erinevad oluliste poolte poolest (‡1115, ‡1116). Enamik keskendub riskidele, mis on seotud keemiliste, bioloogiliste, radioloogiliste ja tuumarünnakute (CBRN) ohtudega, täiustatud kübertõrjevõimekusega ning täiustatud autonoomse käitumisega (‡1115, ‡1117). Väike osa raamistikest käsitleb täiendavaid riskivaldkondi, nagu ebaseaduslik mastaabis diskrimineerimine ja laste seksuaalne ärakasutamine.

Mitu arendajat uuendasid oma raamistikke 2025. aastal, lisades uusi jaotisi kahjuliku manipuleerimise, valejoondumise riski ning autonoomse replikatsiooni ja kohandamise kohta (‡1078, ‡1118). Kuigi paljud raamistike kirjeldavad sarnaseid riskijuhtimise lähenemisviise – sealhulgas ohumudelite koostamine, punameeskonna testimine (red-teaming) ja ohtlike võimekuste hindamine – erinevad need riskitõhtede ja läviväärtuste määratlustes, hindamiste sageduses, puhvrites hindamiste ja läviväärtuste vahel ning leevenduslike kohustuste põhjalikkuses (näiteks kas need hõlmavad mudeli kaalukogumite kustutamist või ainult arenduse peatamist) (‡1115, ‡1119). Lisateavet leiate Tabelist 3.5.

>white|orangered|left|14|15.5|bb Paljud toimingud Frontier AI Safety Frameworks raamistikus põhinevad tingimuslikel kohustustel "kui-siis"

Frontier AI-ohutuse raamistikest on ‘kui-siis’ kohustused võtmetähtsusega. Need on tingimuslikud protokollid, mis käivitavad kindlad vastused, kui tehisintellekti mudelid ja süsteemid jõuavad etteantud suutlikkuse lävenditeni (‡1120). Näiteks võib ‘kui-siis’ kohustus öelda, et kui mudelil tuvastatakse võime, mis võimaldab algajatel sisukalt abistada CBRN-relvade loomisel ja kasutuselevõtul, siis rakendab arendaja täiustatud turvameetmeid, kasutuselevõtu juhtimisi ja reaalajas seiret (‡991*).

Aastal 2025 teatasid mitmed AI arendajad, et uued mudelid käivitasid varajase hoiatuse alarme või et nad ei saanud välistada võimalust, et edasine hindamine näitaks, et mudelid on ületanud võimekuse läve. See ajendas neid rakendama suurendatud kaitsemeetmeid ettevaatusabinõuna (‡7, ‡33, ‡1121*). Frontier AI ohutuse raamistikud nõuavad tavaliselt esmast võimekuse hindamist enne riskide maandamist, samuti jääkriski analüüsi või ohutusjuhtu (safety case), mis on sageli pärast maandamist informeeritud red-teaming’ust. Täpsemat teavet vt Laud 3.5.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Valmiduse raamistik 2 (‡1078*)
  Hõlmatud riskid:
1. Bioloogilised ja keemilised võimed
2. Küberturvalisuse võimekused
3. AI isetäiendamise võimalused
  Riskitasemed või samaväärne ning nendega seotud kaitsemeetmed:
- Kõrge: Võib võimendada olemasolevaid teid tõsise kahju tekitamiseks (Nõuab turvakontrolle ja kaitsemeetmeid)
- Kriitiline: Võib kasutusele tuua enneolematuid uusi teid tõsise kahju tekitamiseks (Peatada edasine arendus kuni täpsustatud kaitsemeetmete ja tarkvaraturbe kontrollide standardid on saavutatud Kriitilisel tasemel)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: vastutustundliku skaleerimise poliitika 2.2 (‡991*)
  Hõlmatud riskid:
1. CBRN relvad
2. Autonoomse tehisintellekti uurimis- ja arendustegevus (AI R&D)
3. Kübertöösed toimingud (hindamisel)
  Riskitasemed või samaväärne ja nendega seotud kaitsemeetmed:
  AI ohutustasemed (ASL)
- ASL-1: Ei olulist katastroofilist riski
- ASL-2: Ohtlike võimekuste varased märgid (Mudelid peavad vastama ASL-2 kasutuselevõtu ja turvastandarditele)
- ASL-3: Oluliselt suurenenud katastroofilise väärkasutuse risk (mudelid peavad vastama ASL-3 kasutuselevõtu ja/ või turvastandarditele)
- ASL-4+: Tulevased klassifikatsioonid (pole veel määratletud)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Frontier Safety Framework 3.0 (‡1040*)
  Hõlmatud riskid:
1. Kuritarvitamine
    a. CBRN
    b. Küberturvalisus
    c. Kahjulik manipuleerimine
2. Masinõppe teadus- ja arendustegevus
3. Ebatäpsus/ instrumentaalne arutlus
  Riskitasemed või samaväärne ja nendega seotud kaitsemeetmed:
  Kriitilised võimekuse tasemed
    Võimekuse tasemed, mille puhul puuduvate leevendusmeetmete korral (kasutuselevõttude ohutusjuhtumid ja turvameetmed, mis on kooskõlas RAND-i turvatasemetega 2, 3 või 4 (‡1122)), võivad tehisintellekti mudelid või süsteemid kujutada suurenenud riski tõsise kahju tekkeks. Võimekuse tasemed hõlmavad „varajase hoiatuse hindamisi“, millel on konkreetsed „hoiatusläved“
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Frontier AI Framework 1.1 (‡990*)
  Hõlmatud riskid:
1. Küberturvalisus
2. Keemilised ja bioloogilised ohud
  Riskitasemed või samaväärsed ning nendega seotud kaitsemeetmed:
  Riskitalaseme tasemed
- Mõõdukas (väljalase koos asjakohaste turvameetmete ja leevendusmeetmetega)
- igh (ära vabasta)
- Kriitiline (peata arendus)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Frontier Model Safety Framework (‡1123*)
  Hõlmatud riskid:
1. CBRN relvade levik
2. Ründavad küberoperatsioonid
3. Automatiseeritud tehisintellekti teadus- ja arendustöö
  Riskitasemed või samaväärsed andmed ning nendega seotud kaitsemeetmed:
  Olulised võimekuse künnised
    Mudeli võimekused, mis võivad valesti kasutamisel põhjustada märkimisväärset kahju avalikkusele. (Kui läved on saavutatud või ületatud, ei võeta mudelit avalikult kasutusele ilma asjakohaste riskide leevendamise meetmeteta)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Frontier Governance Framework (‡1124*)
  Hõlmatud riskid:
1. CBRN relvad
2. Ründavad küberoperatsioonid
3. Täiustatud autonoomia (sealhulgas AI teadus- ja arendustegevus)
  Riskitasemed või samaväärne ning nendega seotud kaitsemeetmed:
  Riskitasemed
- Madal või Keskmine (Töötamine lubatud kooskõlas vastutustundliku tehisintellekti programmi nõuetega)
- Kõrge või kriitiline (täiendav ülevaatus ja maandamised
nõutav)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Frontier AI riskihinnang (‡1029*)
  Hõlmatud riskid:
1. Küberkuritegevus
2. CBRN
3. Veenmine ja mõjutamine
4. Ebaseaduslik diskrimineerimine mastaabis
  Riskitasemed või samaväärne teave ja nendega seotud kaitsemeetmed:
  Riskiläved – mudeli riski (MR) skoorid
- MR1 või MR2 (hindamistulemused on dokumenteeritud insenerimeeskondade poolt)
- MR3 (Riskide maandamise meetmed ja hindamistulemused dokumenteeritakse insenerimeeskondade poolt ning vaadatakse perioodiliselt üle)
- MR4 (Täpsem riskihindamine tuleb läbi viia ja nõutav on ärivaldkonna juhi kinnitus)
- MR5 (Täpne riskihinnang tuleb läbi viia ja kinnitada sõltumatu komisjoni poolt, nt NVIDIA AI eetika komitee)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Turvalise tehisintellekti eesrindliku mudeli raamistiku (‡1125*)
  Hõlmatud riskid:
1. Kuritahtlik kasutus (nt pahavara, laste seksuaalne ärakasutamine)
2. Kahju tavapärases, mitte-kahata eesmärgiga kasutuses, nt väljundid, mis põhjustavad ebaseadusliku diskrimineeriva tulemuse või ebaturvalise koodi genereerimise
  Riskitasemed või samaväärsed ning nendega seotud kaitsemeetmed:
  Kahju tõenäosus ja raskus kontekstis
- Low
- Keskmine
- Kõrge
- Väga kõrge
    (Riski maandamised ja turvakontrollid on olemas kõigi süsteemide ja protsesside jaoks; täiendavad maandamised tuleb kohandada tehisintellekti süsteemile ja kasutusjuhule, millesse mudel on rakendatud)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: AGI Valmidus_poliitika (‡1127*)
  Hõlmatud riskid:
1. Küberkuritegevus
2. Automatiseeritud tehisintellekti teadus- ja arendustöö
3. Autonoomne paljunemine ja kohanemine
4. Bioloogiliste relvade abi
  Riskitasemed või samaväärne ning nendega seotud kaitsemeetmed:
  Olulised võimekuse künnised
    Kvantitatiivsed läved võimekuse võrdlusalustel (Kui need on ületatud, vii läbi ohtlikud võimekuse hindamised, teabe turvameetmed ja kasutuselevõtu leevendamised või peata arendus)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: AGI Valmidusprogrammi (‡1127*)
  Hõlmatud riskid:
1. Küberkuritegevus
2. Automatiseeritud tehisintellekti teadus- ja arendustöö
3. Autonoomne replikeerimine ja kohandamine
4. Bioloogiliste relvade abi
  Riskitasemed või vastav kategooria ja nendega seotud kaitsemeetmed:
  Olulised võimekuse künnised
    Võimekuse võrdlusaluste kvantitatiivsed läviväärtused (kui need on ületatud, viige läbi ohtliku võimekuse hindamised, teabe turvameetmed ja kasutuselevõtu leevendusmeetmed või lõpetage arendustegevus)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: AI ohutuse raamistik (‡1128*)
  Hõlmatud riskid:
1. Kontrolli kaotus
2. Kuritarvitamine (nt biokeemiline relvastamine
  Riskitasemed või vastav samaväärne klassifikatsioon ja sellega seotud kaitsemeetmed:
  Riskitasemed
- Madal risk (Juhtige AI-süsteemide juurutamist, kuid teosta seejärel seiret, et riske hallata)
- Risk tuvastatud (kas avatud AI-süsteeme tohib ainult volitatud kasutajatele, et riske maandada, või jätta kasutuselevõtt tegemata kuni täiendavad turvameetmed on rakendatud, sõltuvalt kasutusjuhtumist)
- Suur risk (Ära juuruta tehisintellekti süsteeme)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Frontier AI ohutuse raamistik (‡1129*)
  Hõlmatud riskid:
1. Bioloogilised ohud
2. Ründav küberjulgeolek
3. Autonoomne töö ja täiustatud manipuleerimine
  Riskitasemed või samaväärsed meetmed ja nendega seotud kaitsemeetmed:
  Riskitasemed
- Tase 1 (Põhilised kaitsemeetmed minimaalsete riskide korral ja võimalus avalikuks lähtekoodina avaldamiseks)
- Tase 2 (reaalajas jälgimine, promptide filtreerimine, käitumuslike anomaaliate tuvastamine, juurdepääsukontrollid, red-teaming ja advesariaalsed simulatsioonid)
- Tase 3 (Täpsemad kaitsemeetmed, sh red-meeskondamine, etappilised kasutuselevõtud, vastandlik testimine, krüpteerimine, mitme osapoole juurdepääsukontrollid ja nullusaldus- (zero-trust) arhitektuur)
- Tase 4 (Maksimaalsed ohutusprotokollid kõrge riskiga mudelite jaoks ja maksimaalsed turvameetmed)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Laud 3.5: Frontier AI ohutuse raamistikud
>white|black||9|11|br Esimene Frontier AI Safety Frameworks-i komplekt, mille on välja andnud osa AI arendajatest, kes on alla kirjutanud Frontier AI Safety Commitments-idele. Raamistikud käsitlevad sarnaseid riske (kergete erinevustega) ning kasutavad erinevaid riskitasemeid ja riskijuhtimise lähenemisviise.


>white|orangered|left|14|15.5|bb Frontier AI turvaraamistike tõhusus on ebakindel

Frontier AI ohutuse raamistikud võivad teatud tingimustel ja kindlate riskikategooriate puhul toimida riskijuhtimise vahenditena, millel on usutav tee kahjuni (‡1117). Samal ajal käsitlevad mitmed analüüsid nende selguse ja ulatuse puudutavaid küsimusi (‡111, ‡986) ning tehisintellekti võimekuse ja riskiläviväärtuste vastupidavust (‡1031, ‡1130). Olemasolevad raamistikud kipuvad keskenduma riskivaldkondade alamhulgale. Selle tulemusena saavad mõned silmapaistvad riskid, nagu ebaseaduslik jälgimine (‡1131, ‡1132) ja nõusolekuta intiimne kujutis (‡287), vähem rõhku. Erinevalt riskijuhtimise lähenemistest teistest sektoritest, nagu lennundus või tuumaenergia (‡1133*), ei kasuta Frontier AI ohutuse raamistikud tavaliselt selgesõnalisi kvantitatiivseid riskiläviväärtusi (‡1134).

Arendajate vastavuse välised hindamised nende Frontier AI Safety Frameworksidele on seni jäänud piiratud, osaliselt seetõttu, et enamik raamistikest on hiljutised, avalikult kättesaadav teave on vähene ning puuduvad standardiseeritud välisauditid. Nende tõhusust mõjutab samuti see, kui hästi ja mil määral võetud kohustusi praktikas rakendatakse. Üksi ei pruugi need raamistikud tagada tõhusat riskijuhtimist, kuna nende praktiline mõju sõltub sellest, kui hästi ja mil määral need rakendatakse. Tänaseni ei ole need täielikult kooskõlas rahvusvaheliste riskijuhtimise standarditega (‡1135). Uuring varasemate vabatahtlike kohustuste kohta leidis ebaühtlast täitmist eri meetmete lõikes, mis viitab sellele, et vabatahtlike kohustuste järgimine tõenäoliselt erineb ettevõtete ja valdkondade vahel (‡1109).

Kokku võttes kujutavad Frontier AI Safety raamistikud endast praegu kasutusel oleva vabatahtliku organisatsioonilise riskijuhtimise kõige üksikasjalikumat vormi, kuid nende ulatus, läved ja rakendatavus erinevad märkimisväärselt.

###@ Regulatiivsed ja valitsemisalased algatused

>white|orangered|left|14|15.5|bb Mitmes jurisdiktsioonis on kehtestatud seadused läbipaistvusnõuetega

Mitmed varased regulatiivsed lähenemisviisid kehtestavad õiguslikud nõuded, mille eesmärk on suurendada riskijuhtimise standardiseeritust ja läbipaistvust. ELi tehisintellekti käsitlev õigusakt (AI Act), mis jõustus 2024. aastal, sätestab nõuded, mis puudutavad läbipaistvust, autoriõigust ja ohutust üldotstarbeliste tehisintellektimudelite puhul. 2025. aastal avaldati ELi üldotstarbelise tehisintellekti tegevusjuhis (Code of Practice), et toetada nende kohustuste täitmist, pakkudes suuniseid mudeli dokumenteerimise ja autoriõiguse kohta ning lisaks – kõige arenenumate mudelite puhul – riskijuhtimise praktikate, nagu hindamised, riskihindamine ja maandamine, infokaitse ning tõsiste intsidentide raporteerimine (‡965).

Muude näidete hulka kuuluvad Lõuna-Korea raamseadus tehisintellekti arendamise ja usalduse loomise kohta, mis toob sisse nõuded “suure mõjuga” tehisintellekti süsteemidele kriitilistes sektorites (‡1136), ning California SB 53, mis sätestab läbipaistvusnõuded ohutusalastele raamistikele ja intsidentidest teavitamisele (‡1104). Arvestades, kui hiljuti need nõuded kehtestati, on liiga vara hinnata üksikasjalikult, kuidas need mõjutavad riskijuhtimise tavasid või tegelikke riskitulemusi.

>white|orangered|left|14|15.5|bb Ulatuslikumad juhtimisalased algatused pakuvad vabatahtlikku suunamist.

Mitmed piirkondlikud ja piirkondadevahelised valitsemisraamistikud sõnastavad nüüd ühised ootused üldotstarbelisest tehisintellektist tulenevate riskide haldamiseks, pakkudes sidumatut suunist poliitikakujundajatele ja organisatsioonidele. Hiina AI ohutuse valitsemisraamistik 2.0, mis avaldati 2025. aastal, annab struktureeritud suunised riskide liigitamiseks ja leevendusmeetmeteks kogu AI väljatöötamise ja kasutuselevõtu protsessis (‡1137). ASEANi liikmesriigid avaldasid „ASEANi laiendatud juhendi AI valitsemise ja eetika kohta (generatiivne AI)”, mis annab suunised üldotstarbelise AI valitsemiseks ja eetikaks ning mille eesmärk on toetada suuremat poliitikakõla ASEANi liikmesriikide vahel (‡1138). Lisaks kirjeldavad eksperdijuhitud algatused, nagu Singapuri konsensus, mille on välja töötanud AI teadlased mitmest riigist, uurimisprioriteete üldotstarbelise AI ohutuse tagamiseks riskihinnangus, väljatöötamises ja kontrollis (‡690).

###@ Värskendused

Alates eelmise aruande avaldamisest (jaanuar 2025) on üldotstarbelise tehisintellekti riskijuhtimise maastik arenenud: on avaldatud uusi ressursse, nagu ELi üldotstarbelise tehisintellekti tegevusjuhend (General-Purpose AI Code of Practice), G7 HAIP-i aruanderaamistik (G7 HAIP Reporting Framework), Hiina riiklik tehisintellekti ohutuse juhtimise raamistik 2.0 ning mitmed AI-taristu- või -arendajate Frontier AI Safety Frameworkid. Need algatused kirjeldavad lähenemisviiseid ja tavasid, mida AI arendajad kasutavad üldotstarbelise tehisintellekti süsteemidega seotud riskide maandamiseks (‡1115). Frontier AI Safety Frameworkide ning HAIP-i läbipaistvusaruannete vahel (‡1103) esineb märkimisväärset varieeruvust, mis peegeldab erinevusi organisatsioonilistes tavades, riskide prioriseerimisel ja üldotstarbelise tehisintellekti riskijuhtimise ökosüsteemi varases arengustaadiumis. Usaldusväärne ökosüsteem, kus erinevad AI-osalised panustavad kogu elutsükli vältel täiendavate riskijuhtimise tavadega, võib aidata kaasa tõhusale riskijuhtimisele (‡690).

###@ Tõenduslüngad

Puuduvad tõendid selle kohta: kuidas mõõta esilekerkivate riskide raskusastet, esinemissagedust ja ajaraami; mil määral neid riske saab maandada reaalses maailmas kasutatavates olukordades; ning kuidas tõhusalt soodustada või kohustada maandamise kasutuselevõttu eri osapoolte seas. Vajalik on rohkem uurimistööd, et mõista, kui levinud on erinevad riskid ja kui palju need varieeruvad eri maailma piirkondades, eelkõige nende piirkondade puhul nagu Aasia, Aafrika ja Ladina-Ameerika, mis digitiseerivad kiiresti. Kuna tehisintellekti (AI) mudelitele antakse üha suuremat tegutsemisvõimet ja autoriteeti ning üldotstarbelise AI riskide teaduslik seisund areneb, peavad ka riskijuhtimise lähenemisviisid muutuma (‡639, ‡1139).

Teatud riskide maandamise meetmed on muutumas üha populaarsemaks (‡690, ‡956), kuid rohkem on vaja uurida, et mõista, kui vastupidavad on riskide maandamise meetmed ja kaitsemeetmed praktikas eri kogukondade ja AI osaliste puhul (sealhulgas väikeste ja keskmise suurusega ettevõtete puhul). Andmetele juurdepääs reaalelulise mudelite kasutuselevõtu ja kasutamise kohta on selliste hinnangute puhul asjakohane. Lisaks on riskijuhtimise alased jõupingutused praegu juhtivate AI ettevõtete lõikes väga erinevad. On väidetud, et arendajate stiimulid ei ole piisavalt hästi kooskõlas põhjaliku riskihindamise ja -juhtimisega (‡934). Endiselt puudub tõendus selle kohta, mil määral erinevaid vabatahtlikke kohustusi täidetakse, milliste takistustega ettevõtted kokku puutuvad kohustustest täielikult kinnipidamisel ning kuidas nad integreerivad Frontier AI Safety Frameworks’i laiematesse AI riskijuhtimise tavadesse.

###@ Väljakutsed poliitikakujundajatele

Peamised väljakutsed hõlmavad seda, kuidas seada üldotstarbelise AI poolt põhjustatud erinevad riskid tähtsuse järjekorda, selgitada välja, millised osalised on nende leevendamiseks kõige paremini positsioneeritud, ning mõista stiimuleid ja piiranguid, mis kujundavad nende tegevust. Tõendid viitavad sellele, et poliitikakujundajatel on praegu piiratud juurdepääs teabele, kuidas AI arendajad ja kasutuselevõtjad testivad, hindavad ja jälgivad tekkivaid riske, ning milline on erinevate leevenduspraktikate tõhusus (‡1140). Teadlased ja poliitikakujundajad on arutanud läbipaistvuse suurendamise püüdlusi ja võimaliku viisina ka ühtlasemat juhtumite raporteerimist, et saada teavet riskide tähtsuse järjekorda seadmiseks, edendada usaldust ja motiveerida vastutustundlikku arendust (‡957). Praktikas hõlmab riskijuhtimine mitut osalist AI väärtusahelas – näiteks andme- ja pilveteenuse pakkujaid, mudelite arendajaid ja mudelite majutamise platvorme –, kellalgi on erinevad võimalused hinnata ja hallata erinevaid riske (‡1141). Piiratud teabevahetus nende osaliste vahel muudab keeruliseks kindlaks teha, millised riskid on kõige tõenäolisemad või mõjukamad, eriti kui arvesse võtta järeltulevaid ühiskondlikke mõjusid.

