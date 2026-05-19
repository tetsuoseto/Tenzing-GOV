##########
>white|orangered|left|14|30|hr 3.2 skyrius
### 3.2. Rizikos valdymo praktikos
>white|orangered|left|24|30|hb Rizikų valdymo praktika

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Svarbiausia informacija
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Bendrosios paskirties dirbtinio intelekto rizikų valdymą sudaro įvairios praktikos, naudojamos identifikuoti, įvertinti ir mažinti rizikas, susijusias su bendrosios paskirties dirbtiniu intelektu. Tai apima modelio lygmens testavimą ir vertinimą (pvz., „red-teaming“), organizacinius procesus, kurie nurodo plėtros ir išleidimo sprendimus, sąlygines apsaugas (pvz., „if-then“ įsipareigojimus) ir incidentų pranešimus.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Keletas AI kūrėjų sukūrė „Frontier“ AI saugos sistemas. Šios sistemos apima informacija apie rizikos vertinimus ir nurodo sąlygines priemones, pavyzdžiui, prieigos apribojimus, kuriuos įmonės planuoja taikyti ketinant gauti pajėgesnius modelius. Jos skiriasi tuo, kokias rizikas apima, kaip apibrėžia pajėgumo ribas ir kokie veiksmai suveikia, kai šios ribos pasiekiamos.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Įrodymai apie realaus pasaulio AI rizikų valdymo praktikų veiksmingumą išlieka riboti. Dėl nepakankamo incidentų registravimo ir stebėsenos sunku įvertinti, kaip gerai esamos praktikos mažina rizikas, arba kaip nuosekliai jos įgyvendinamos.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Nuo paskutinės Ataskaitos paskelbimo (2025 m. sausis) rizikų valdymas tapo labiau struktūrizuotas dėl naujų pramonės ir valdymo iniciatyvų. Nauji instrumentai, tokie kaip ES Bendrosios paskirties AI elgesio kodeksas, Kinijos AI saugos valdymo sistema 2.0 ir G7 Hirošimos AI procesų ataskaitų teikimo sistema, kartu su įmonių iniciatyvomis rodo tendenciją link labiau standartizuotų požiūrių į skaidrumą, vertinimą ir incidentų ataskaitų teikimą.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Rinkos dinamika ir dirbtinio intelekto (DI) plėtros tempas kelia papildomų iššūkių. Dėl konkurencinio spaudimo DI įmonės gali susidurti su kompromisais tarp spartesnio produktų išleidimo ir investicijų į rizikos mažinimo priemones. Daugelė su DI susijusių žalingų padarinių taip pat yra išorinami, o teisinė atsakomybė už juos išlieka neaiški, be to, valdymo procesai gali lėtai prisitaikyti prie pokyčių DI aplinkoje.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Pagrindiniai iššūkiai politikos formuotojams apima prioritetų teikimą tarp įvairių rizikų, kurias kelia bendrosios paskirties dirbtinis intelektas, ir aiškiai nustatyti, kurie veikėjai visoje AI vertės grandinėje yra geriausiai pasirengę tas rizikas mažinti. Šiuos iššūkius dar labiau apsunkina ribotas supratimas, kaip rizikos realiai yra identifikuojamos, įvertinamos ir valdomos, taip pat fragmentuotas informacijos dalijimasis tarp kūrėjų, diegėjų ir infrastruktūros paslaugų teikėjų.
>oldlace|black||11|15|br      


AI rizikų valdymas apima įvairias praktikas, kuriomis siekiama identifikuoti, įvertinti ir sumažinti AI sistemų keliamų rizikų tikimybę ir poveikio sunkumą. Šias praktikas gali įgyvendinti AI kūrėjai, diegėjai, vertintojai ir reguliuotojai. Pavyzdžiai: grėsmių modeliavimas, rizikų klasifikavimas pagal lygius, raudonų komandų testavimas (red-teaming), auditas ir incidentų pranešimas. Šiame skyriuje aprašomos esamos rizikų valdymo praktikos, nauji pokyčiai ir išliekantys apribojimai.

Nuo 2025 metų pradžios buvo parengtos kelios naujos tarptautinės iniciatyvos, skirtos bendrosios paskirties dirbtinio intelekto (AI) rizikų valdymui, įskaitant organizacinio skaidrumo ir rizikų ataskaitų teikimo sistemų kūrimą, taip pat reguliavimo ir valdymo sistemas.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Figūra 3.4: Keturi rizikos valdymo komponentai
>white|black||9|11|br Keturi bendrosios paskirties dirbtinio intelekto rizikos valdymo metodų kategorijų tipai: rizikos nustatymas; rizikos analizė ir vertinimas; rizikos mažinimas; ir rizikos valdymas. Šie veiksmai sudaro iteracinį ir ciklinį procesą. Rizikos valdymas, pavaizduotas centre, palengvina kitų komponentų sėkmę. Šaltinis: International AI Safety Report 2026.


Likę iššūkiai apima ribotą standartizavimą, dėl kurio apsunkinamas atitikties ir vertinimo procesas, taip pat ribotus įrodymus apie realaus pasaulio veiksmingumą. Be to, institucinis, kultūrinis ir politinis kontekstas skiriasi visame pasaulyje, todėl požiūriai į rizikų nustatymą ir valdymą, įskaitant priimtinų rizikos ribų, gali skirtis tarp regionų. Šio skyriaus rizikų valdymo metodų aptarimas yra aprašomojo pobūdžio: juo siekiama informuoti AI ekosistemos dalyvius apie šiuo metu taikomus pasaulinius rizikų valdymo metodus. Kai yra prieinami, aptariami šių metodų veiksmingumo ir ribotumų įrodymai, tačiau šio darbo apimties ribose nėra politikos rekomendacijų.

###@ Rizikos valdymo komponentai

Rizikos valdymas yra iteracinis procesas, apimantis praktikas ir metodus, kurie tęsiasi per visą AI kūrimo ir diegimo ciklą, tačiau tarpusavyje veikia darniai (‡969). Rizikos valdymas bendrosios paskirties AI gali apimti įvairių veikėjų vaidmenis, įskaitant duomenų mokslininkus, modelių inžinierius, auditorius, dalykinės srities ekspertus, vadovus, galutinius naudotojus, paveiktas bendruomenes, trečiųjų šalių tiekėjus, politikos formuotojus, vyriausybes, standartizacijos organizacijas ir pilietinės visuomenės organizacijas (‡970, ‡971, ‡972). Pirmaujantys rizikos valdymo standartai dažnai yra suderinami tarpusavyje, tačiau naudoja skirtingą terminiją rizikos valdymo elementams aprašyti (‡973, ‡974). Paprastai jie turi keturis tarpusavyje susietus komponentus (Figūra 3.4): rizikos nustatymas; rizikos analizavimas ir vertinimas; rizikos mažinimas; ir rizikos valdymas (‡970, ‡973, ‡975, ‡976). Žemiau pateikiamos lentelės pateikia iliustracinius svarbių metodų, technikų ir įrankių pavyzdžius. Praktikos ir toliau tobulėja, todėl lentelės nėra išsamios, o taikymas įvairiuose kontekstuose gali skirtis.

###@ Rizikų identifikavimas

Rizikų identifikavimas yra procesas, kurio metu randami, atpažįstami ir aprašomi rizikos veiksniai. Išsamus rizikų identifikavimas paprastai apima į galimybes (capability) orientuotus vertinimus, kurie tikrina, ar modeliai turi konkrečių pavojingų galimybių (‡977), taip pat rizikų modeliavimą (‡978) ir prognozavimą (‡715*), naudojamus nagrinėti esamas ir kylančias rizikas. Stalo 3.1 pateikia įvairių rizikų identifikavimo praktikų pavyzdžių. Rizikų identifikavimas taip pat remiasi bendravimu su atitinkamais ekspertais ir bendruomenėmis, kad būtų suprastas platesnis kontekstas, kaip rizikos atsiranda (‡979, ‡980). Tokie mechanizmai kaip bug bounty programos gali padėti šiame procese, skatindami identifikuoti anksčiau nežinomas pažeidžiamybes (‡981) (Stalo 3.1). Pagrindinis rizikų identifikavimo tikslas yra atsižvelgti tiek į gerai žinomas, gerai suprantamas rizikas, tiek į galimus būsimos rizikos atvejus, kurie išlieka neapibrėžti arba prastai apibūdinti (‡982). Tai ypač svarbu bendrosios paskirties AI (general-purpose AI), kai daugelio rizikų dar nėra iki galo suprasta arba jos nėra stebimos (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Klaidų atlyginimo programos
  „Bug bounties“ arba pažeidžiamumų pranešimo programos skatina žmones rasti ir pranešti apie pažeidžiamumus AI sistemose. Keli kūrėjai įdiegė „bug bounty“ programas (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ekspertų konsultacija
  Domeno ekspertai, naudotojai ir paveiktos bendruomenės pateikia įžvalgas apie galimas rizikas. Atsiranda dalyvaujamojo ir įtraukaus DI (‡985) gairės.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Žuvies kaulo (Išikavos) diagrama
  Žuvies kaulo diagramos yra gerai žinomos priežasties ir pasekmės analizės (root cause analysis) priemonės, o tyrėjai siūlė jas naudoti struktūrizuotai analizuojant AI rizikos incidentus (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Prognozavimas
  Prognozavimas yra procesas, kai remiantis praeities ir esamų duomenų analize numatomi būsimi įvykiai arba tendencijos. Jis buvo taikomas skirtingų, pavyzdžiui, ekonominių rezultatų santykinės tikimybės palyginimui dėl pažangios dirbtinio intelekto (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rizikų taksonomija
  Rizikų taksonomijos yra būdas suskirstyti ir organizuoti rizikas pagal kelias dimensijas. Yra keletas, kurios aprašo rizikas iš bendrosios paskirties dirbtinio intelekto (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Scenarijų planavimas
  Scenarijų planavimas apima tikėtinų ateities scenarijų parengimą ir analizę, kaip kyla rizikos. Jis buvo taikomas siekiant ištirti AI modelių rizikas ir jų poveikį (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Grėsmių modeliavimas
  Grėsmių modeliavimas yra procesas, skirtas nustatyti grėsmes ir pažeidžiamumus sistemai. Daugybė AI kūrėjų pabrėžia, kad jį naudoja siekdami numatyti galimus AI sistemų netinkamo panaudojimo scenarijus (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Stalo 3.1: Rizikų identifikavimo pavyzdžiai bendrosios paskirties AI rizikų valdyme
>white|black||9|11|br Pavyzdiniai AI rizikų identifikavimo metodai išvardyti abėcėlės tvarka. Įtraukti metodai
yra sukurti taip, kad palaikytų rizikų identifikavimą daugeliui skirtingų rizikos tipų, įskaitant rizikas, kylančias dėl piktnaudžiavimo, rizikas, kylančias dėl gedimų, ir sistemines rizikas. Atsižvelgiant į tai, kad bendrosios paskirties AI rizikos valdymas dar tik formuojasi, ne visi metodai bus tinkami kiekvienam AI kūrėjui ar diegėjui.


>white|orangered|left|14|15.5|bb Grėsmių modeliavimas ir rizikos taksonomijos yra svarbios rizikos identifikavimo metodikos

Dvi iškiliausios metodikos, skirtos nustatyti rizikas, kylančias iš bendrosios paskirties AI, yra grėsmių modeliavimas (International AI Safety Report 2026) (struktūruotas procesas, kuriuo sudaroma, kaip gali materializuotis su AI susijusios rizikos) ir rizikų taksonomijos. Pavyzdžiui, „Meta“ naudoja grėsmių modeliavimą, kad prognozuotų galimus savo AI modelių piktnaudžiavimo scenarijus (‡990), o „Anthropic“ įtraukia grėsmių modeliavimą į savo ASL-3 diegimo standartą (‡991). AI rizikų ir pavojų taksonomijos, kurios pateikia rizikos kategorijas ir pavyzdžius, taip pat gali būti tinkamas pradinis taškas konceptualizuoti, identifikuoti ir apibrėžti reikšmingas rizikas, susijusias su bendrosios paskirties AI konkrečiuose taikymo domenų kontekstuose (‡906, ‡988, ‡992, ‡993).

###@ Rizikos analizė ir vertinimas

Rizikos analizė ir vertinimas yra procesas, kurio metu nustatomas dirbtinio intelekto (DI) modelio ar sistemos rizikos lygis, ir jis palyginamas su nustatytais kriterijais, siekiant įvertinti priimtinumą arba būtinybę taikyti mažinimo priemones (‡994, ‡995, ‡996, ‡997). Jis apima tokias praktikas kaip modelio veiksmingumo matavimas pagal vertinimo rinkinius (‡998) ir vertinimus (‡176, ‡715), „red-teaming“ pratybų atlikimą (‡999*), poveikio vertinimus (‡1000) ir auditus (‡1001, ‡1002). Daugiau pavyzdžių, kaip atliekama bendros paskirties DI rizikos analizė ir vertinimas, žr. 3.2 lentelę. Metodai skirti vienu metu palaikyti analizę ir vertinimą daugeliui skirtingų rizikos tipų.

Pagrindiniai rizikos analizės ir vertinimo tikslai yra atlikti modelio gebėjimų ir pažeidžiamumų vertinimus (‡1003), taikyti patikimą rizikos modeliavimą sprendimams dėl rizikos slenksčių priimti (‡1004, ‡1005) ir suprasti, kaip AI sistemos realiai naudojamos, siekiant įvertinti tolesnius visuomeninius padarinius (‡869, ‡904, ‡905, ‡1006). Rizikos analizės ir vertinimo procesai dažnai laikomi labiau linkusiais identifikuoti rizikas tada, kai jie apima nepriklausomą peržiūrą (‡1001, ‡1007), remiasi tarpsektorine kompetencija (‡1008) ir apima įvairias perspektyvas iš skirtingų sričių bei disciplinų, taip pat iš paveiktų bendruomenių (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Auditai
  Auditas yra formalus AI modelių veikimo ir poveikio bei/ ar organizacijos atitikties standartams, politikoms ir procedūroms įvertinimas, atliekamas organizacijos viduje arba išorinio subjekto. AI auditas yra sparčiai auganti sritis, ir yra daugybė įrankių bei praktikų, skirtų AI modelių audito atlikimui ir AI modelių kūrėjų praktikų vertinimui (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Etalonai
  Etalonai yra standartizuoti, dažnai kiekybiniai testai arba rodikliai, naudojami įvertinti ir palyginti AI sistemų veikimą pagal fiksuotą užduočių rinkinį, skirtą atspindėti realaus pasaulio naudojimą (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bowtie metodas
  Lankinės varlytės (bowtie) metodas yra gerai žinomas metodas, skirtas vizualizuoti, kur galima pridėti kontrolės priemones, siekiant sumažinti rizikos įvykius. Jis aiškiai atskiria proaktyvų ir reaktyvų rizikos valdymą (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Delphi metodas
  Delphi metodas yra grupinio sprendimų priėmimo metodika, kuri naudoja eilę klausimynų sutarčiai surinkti iš ekspertų grupės (‡1020, ‡1021). Jis buvo taikomas siekiant padėti ištirti galimas ateitis naudojant pažangų DI (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bandymai lauke
  Lauko bandymai įvertina AI sistemos našumą ir poveikį realioje, operacinėje aplinkoje. Kai kurie tyrimai pabrėžia, kad lauko bandymai yra papildinys modelių vertinimui, siekiant įvertinti realaus pasaulio rezultatus ir pasekmes (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Poveikio įvertinimas
  Poveikio vertinimai įvertina galimą technologijos ar projekto poveikį. Tai gali apimti poveikio kiekybinį įvertinimą, suvienodinimą ir prioritetų nustatymą. Pavyzdžiui, ES AI aktas reikalauja didelės rizikos dirbtinio intelekto sistemų kūrėjų atlikti Pagrindinių teisių poveikio vertinimus (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modelio vertinimas
  Modelio vertinimai apima procesus ir testus, kuriais siekiama įvertinti bei pamatuoti AI modelio našumą konkrečiai užduočiai. Yra daugybė AI vertinimų, skirtų įvertinti skirtingus gebėjimus ir rizikas, įskaitant saugą, saugumą ir socialinį poveikį (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tikimybinė rizikos analizė
  Tikimybinis rizikų vertinimas yra metodika, skirta įvertinti rizikas, susijusias su sudėtingomis sistemomis ar procesais, kuri apima neapibrėžtumą. Jis buvo pritaikytas pažangiems AI sistemoms (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Red-teamavimas
  Red-teaming yra pratybos, kurių metu žmonių grupė arba automatizuotos sistemos apsimeta priešininku ir atakuoja organizacijos technologines sistemas, kad būtų nustatytos pažeidžiamybės. Daugelyje AI įmonių yra vidinės praktikos, skirtos AI sistemų red-teamingui (‡458, ‡1028). Red-teamingą taip pat gali vykdyti veikėjai už įmonių ribų. Tokios komandos susiduria su iššūkiais, pavyzdžiui, ribota prieiga, tačiau taip pat gali atskleisti savitus įžvalgus (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rizikos matricos
  Rizikos matricos yra vizualus įrankis, padedantis prioritetizuoti rizikas pagal jų tikėtinumo atsirasti ir galimo poveikio dydį (‡1027). Kai kurie AI kūrėjai į savo „Frontier AI Safety Frameworks“ (‡1029*) įtraukia pagrindines rizikos matricas.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rizikos slenksčiai / rizikos lygiai
  Rizikos slenksčiai arba lygiai yra kiekybinės arba kokybinės ribos, kurios atskiria priimtinas nuo nepriimtinų rizikas ir suaktyvina konkrečius rizikos valdymo veiksmus, kai jos viršijamos. Bendrosios paskirties dirbtiniam intelektui jie nustatomi pagal gebėjimų, poveikio, skaičiavimo išteklių, aprėpties ir kitų veiksnių derinį (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rizikos toleravimas
  Rizikos tolerancija reiškia rizikos lygį, kurį organizacija yra pasirengusi priimti. Dirbtinio intelekto (DI) srityje rizikos tolerancijos dažnai nustatomos netiesiogiai per įmonės politiką ir praktiką, o kai kuriose reguliavimo sistemose aiškiai apibrėžiamos nepriimtinos rizikos ir taikomos teisinės pasekmės (‡1032). Kai kurios įmonės aprašo savo rizikos toleranciją pagal naujo modelio ribinę riziką; t. y. kiek modelis kontrafaktiškai padidina riziką, viršijančią tą, kurią jau kelia esami modeliai arba kitos technologijos (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Saugos bylos
  Saugos argumentas yra struktūruotas argumentas, kurį pagrindžia įrodymai, kad sistema yra priimtinai saugi eksploatuoti tam tikrame kontekste. Naujausia literatūra (‡1037, ‡1038, ‡1039) tyrinėjo saugos argumentus dėl pažangių AI sistemų, o tam tikros Pažangios AI saugos sistemos su jais susijusias nuorodas (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sistemos saugos analizė
  Sistemos saugos analizė pabrėžia priklausomybes tarp komponentų ir sistemos, kurios dalimi jie yra, siekiant numatyti, kaip sistemos lygmens pavojai gali atsirasti dėl komponentų ar procesų gedimų, arba dėl sąveikų tarp posistemių, žmogiškųjų veiksnių ir aplinkos sąlygų. Literatūroje taikomi požiūriai AI sistemoms apima sisteminę teorinę procesų analizę (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Stalo 3.2: Rizikos analizė/vertinimas bendrosios paskirties AI rizikos valdyme
>white|black||9|11|br Pavyzdiniai AI rizikos analizės / vertinimo metodai, pateikti abėcėlės tvarka. Atsižvelgiant į ankstyvą bendrosios paskirties AI rizikos valdymo pobūdį, ne visi metodai tiks kiekvienam AI kūrėjui ar diegėjui.


>white|orangered|left|14|15.5|bb Dažniausiai naudojamos rizikos analizės priemonės apima etalonus ir modelio vertinimus

Etalonai ir modelių vertinimai yra standartizuoti testai, skirti įvertinti bendrosios paskirties AI sistemų veikimą atliekant konkrečias užduotis. Tyrėjai sukūrė platų etalonų ir vertinimų spektrą, įskaitant rinkinį sudėtingų klausimų su pasirinkimais, programinės inžinerijos uždavinius ir su darbu susijusias užduotis imituotose biuro aplinkose (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Kenksmingų gebėjimų vertinimai (‡715) naudojami siekiant nustatyti, ar bendrosios paskirties AI modelis ar sistema turi ypač pavojingų žinių ar įgūdžių, pavyzdžiui, gebėjimą padėti vykdant kibernetines atakas (žr. §2.1.3. Kibernetinės atakos).

Labai svarbūs įmonių ir vyriausybių sprendimai dėl modelių išleidimo iš dalies remiasi šiomis vertinimo priemonėmis (‡1050, ‡1051, ‡1052). Tačiau etalonai reikšmingai skiriasi savo kokybe ir apimtimi (‡998, ‡1003), ir gali būti sunku įvertinti jų pagrįstumą dėl daugybės trūkumų vertinimo etalonų taikymo praktikoje (‡902, ‡909, ‡1003, ‡1053*). Pavyzdžiui, etalonai gali tapti „sotūs“ – kai daugelio modelių rezultatai artėja prie didžiausio rezultato – vadinasi, jie nebegali patikimai atskirti skirtingų modelių. Modeliai taip pat vis dažniau gali „atpažinti“ konkrečias užduotis kaip vertinimus ir rodyti kitokį elgesį, nei rodytų panašiose užduotyse diegimo (eksploatavimo) kontekstuose, dėl „situacinio suvokimo“ (žr. §2.2.2. Kontrolės praradimas). Galiausiai etalonai ir vertinimai turi gerai dokumentuotas ribas: svarbiausia, kad jie neapima rizikų, susijusių su bendros paskirties AI naudojimu naujose srityse ir naujoms užduotims, nes bandymo sąlygos skiriasi nuo realaus naudojimo skirtingais laipsniais (‡913) (žr. §1.2. Dabartiniai gebėjimai ir §3.1. Techniniai ir instituciniai iššūkiai).

>white|orangered|left|14|15.5|bb „Red teaming“ leidžia atlikti tikslesnius, su konkrečia sritimi susietus rizikos vertinimus

Kitas dažnas metodas rizikoms įvertinti yra „red-teaming“. „Red team“ – tai vertintojų grupė, kuriai pavesta ieškoti pažeidžiamumų, ribotumų ar galimo piktnaudžiavimo. „Red-teaming“ gali būti taikomas konkrečiai sričiai ir atliekamas sričių ekspertų, arba būti atviras, kad būtų ištirti nauji rizikos veiksniai. Pavyzdžiui, „red team“ gali tirti „jailbreaking“ atakas, kurios apeina modelio saugos apribojimus (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). Skirtingai nuo vertinimo su užduočių rinkiniais (benchmark’ų), pagrindinis „red-teaming“ pranašumas yra tas, kad „red team“ gali pritaikyti savo vertinimus konkrečiai testuojamai sistemai. Pavyzdžiui, „red team“ gali sukurti pasirinktinius įvesties duomenis, kad nustatytų blogiausio atvejo elgsenas, kenkėjiško naudojimo galimybes ir netikėtus gedimus. Vis dėlto tai gali reikalauti specialios prieigos prie modelių ir gali neatskleisti svarbių rizikų klasių (‡999, ‡1028).

Svarbu tai, kad nustatytų rizikų nebuvimas nereiškia, jog tos rizikos yra mažos: ankstesni tyrimai rodo, kad klaidos dažnai išvengia aptikimo, ypač kai red teams turi ribotą prieigą arba išteklius (‡1060). Tyrimai taip pat kėlė abejonių dėl to, ar red-teaming gali duoti patikimus ir pakartojamus rezultatus (‡1061). Red komandos sudėtis ir red-teameriams pateiktos instrukcijos (‡1062), atakų raundų skaičius (‡1063) ir modelio prieiga prie įrankių (‡1064, ‡1065) gali reikšmingai paveikti rezultatus, įskaitant rizikų paviršių, kurį aprėpia testavimas. Išsamios rekomendacijos, skirtos red-teaming, siekia išspręsti kai kuriuos iš šių iššūkių (‡1066).

###@ Rizikų mažinimas

Rizikos mažinimas yra procesas, kai prioritetizuojama, įvertinama ir įgyvendinama kontrolė bei atsakomųjų priemonių rinkinys, siekiant sumažinti nustatytas rizikas. Pavyzdžiai: prieigos kontrolės (‡991), nuolatinis stebėjimas (‡986) ir if-then įsipareigojimai (‡700). Rizikos mažinimas kelia esminį klausimą: kokia yra priimtina rizikos lygio riba? Pastarieji pagrindiniai modeliai ir įmonių politika pradėjo formalizuoti „rizikos priėmimo“ kriterijus (‡965, ‡1040). Vis dėlto tinkamų ribų nustatymas išlieka sudėtingas, ypač rizikoms, turinčioms plačius visuomeninius padarinius (‡986, ‡1067). Šiuo metu nėra nusistovėjusio mechanizmo, skirto patvirtinti rizikos priėmimo sprendimus, kuriuos kūrėjai priima prieš išleidimą (‡1005).

Žemiau pateiktos 3.3 lentelėje aprašytos rizikos mažinimo priemonės yra pritaikomos ir gali sumažinti įvairias rizikas, įskaitant kai kurias netikėtas rizikas. Lentelėje nėra pateiktos techninės mažinimo priemonės, tokios kaip priešiškas mokymas, turinio filtrai ir grandinės mąstymo stebėsena. Jos aprašomos 3.3 skyriuje „Techninės apsaugos ir stebėsena“, taip pat visame Pranešime skiltyje „Mažinimo priemonės“ kiekvienos rizikos 2 skyriuje „Rizikos“ paragrafuose.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Priimtino naudojimo politika
  Priimtino naudojimo politika yra taisyklių ir gairių rinkinys, skirtas atsakingam, etiškam ir teisėtam AI modelių naudojimui. AI kūrėjams įprasta, kartu su naujais modelių išleidimais (‡1068, ‡1069), skelbti priimtino naudojimo politiką, taip pat draudžiamo naudojimo politiką.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Prieigos kontrolė / vartotojo patikra
  Prieigos kontrolė apima politikų ir taisyklių naudojimą prieigai prie AI modelių, duomenų ir sistemų riboti pagal naudotojų vaidmenis, atributus ir kitas sąlygas, kad būtų išvengta neįgalioto naudojimo, manipuliavimo ar duomenų nutekėjimo. AI įmonės dažnai išjungia paskyras, nustatytas kaip susijusias su nusikalstama veikla (‡486), ir įtraukia naudotojų patikrinimą bei „Know-Your-Customer“ patikras, kad būtų užtikrinta, jog modeliai būtų naudojami tik patikimų subjektų (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Elgsenos/modelio specifikacija
  AI elgesio specifikacija yra dokumentas, kuriame apibrėžiama, kaip AI modelis turėtų elgtis įvairiose situacijose. Ji tarnauja kaip AI suderinimo ir saugos gairės, nurodančios modelio kūrimą, mokymą, vertinimą ir išvestis. Kelios AI įmonės naudoja modelio specifikacijų dokumentus ir paskelbia bent dalį jų viešai (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Nuolatinė stebėsena
  Nuolatinis stebėjimas yra nenutrūkstamas, automatizuotas procesas, skirtas stebėti, analizuoti ir valdyti naudojamas AI sistemas, sekti jų veikimą ir riboti jų elgesį, kad būtų užtikrintas patikimumas, efektyvumas ir sauga. Yra daugybė įrankių nuolatiniam stebėjimui (‡1073*) taip pat metodų, skirtų palaikyti
AI stebimumas (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Gynyba sluoksniais
  Gynyba gynyboje (angl. defence-in-depth) yra idėja, kad galima įdiegti kelis nepriklausomus ir persidengiančius gynybos sluoksnius taip, jog jei vienas iš jų nepavyksta, kiti vis tiek išliktų veiksmingi (‡1075, ‡1076). Keli Frontier AI saugos sistemos (angl. Multiple Frontier AI Safety Frameworks) ją mini (pvz. (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ekosistemos stebėsena
  Tai yra platesnės AI ekosistemos stebėsenos procesas, įskaitant skaičiavimo ir aparatinės įrangos stebėjimą, modelio kilmę, duomenų kilmę ir naudojimo modelius. Mokslinėje literatūroje aptariama tokia stebėsena, siejant ją su rizikomis, kylančiomis iš bendrosios paskirties AI (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Įsipareigojimai „jei-tai“
  „Jei–tada“ įsipareigojimai yra techninių ir organizacinių protokolų bei įsipareigojimų rinkinys rizikoms valdyti, kai AI modeliai tampa pajėgesni. Keli AI kūrėjai taiko tokio tipo įsipareigojimus kaip savo Frontier AI saugos sistemų (‡991, ‡1040, ‡1078*) dalį.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Raudonos linijos arba draudimai
  Raudonos linijos yra konkrečios ribos, išreikštos kaip gebėjimai, poveikis arba naudojimo tipai. Ši sąvoka pasirodo viešuose pareiškimuose ir iniciatyvose, taip pat reguliavimo draudimuose (‡1079, ‡1080, ‡1081). Literatūroje taip pat pažymimi raudonų linijų taikymo ribotumai, įskaitant sunkumus pasiekti sutarimą ir užtikrinti įgyvendinamumą.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Išleidimo ir diegimo strategijos
  Bendrosios paskirties dirbtinio intelekto išleidimo ir diegimo strategijos gali apimti laipsniškus išleidimus arba prieigą per API, kad būtų galima pasitelkti daugiau švelninimo (mitigavimo) galimybių tuo atveju, jei įvyktų piktnaudžiavimas ar netikėta žala (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Stalo 3.3: Rizikos mažinimas bendrosios paskirties dirbtinio intelekto rizikos valdyme
>white|black||9|11|br Pavyzdiniai AI rizikos mažinimo metodai pateikiami abėcėlės tvarka. Įtraukti metodai yra skirti vienu metu paremti rizikos mažinimą daugeliui skirtingų rizikos tipų, įskaitant rizikas, kylančias dėl piktnaudžiavimo, rizikas dėl sutrikimų ir sistemines rizikas. Atsižvelgiant į ankstyvą bendros paskirties AI rizikos valdymo pobūdį, ne visi metodai tiks kiekvienam AI kūrėjui ar diegėjui.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Figūra 3.5: „Šveicariško sūrio diagrama“, iliustruojanti gynybos-sluoksniais (defence-in-depth) požiūrį
>white|black||9|11|br Keli gynybos sluoksniai gali kompensuoti trūkumus atskiruose sluoksniuose. Dabartinės AI rizikos valdymo technikos turi trūkumų, tačiau jų taikymas sluoksniais gali užtikrinti daug stipresnę apsaugą nuo rizikų. Šaltinis: Tarptautinė AI saugos ataskaita 2026.


>white|orangered|left|14|15.5|bb Gynybos sluoksniavimas ir išleidimo strategijos yra svarbios mažinimo priemonės

„Gynybos gilynėjimo“ modelis gali palaikyti bendrosios paskirties dirbtinio intelekto rizikų valdymą. Šiuo atveju „gynybos gilynėjimo“ terminas reiškia techninių, organizacinių ir visuomeninių priemonių derinį, taikomą skirtingais plėtros ir diegimo etapais (Figūra 3.5). Tai reiškia nepriklausomų apsaugos sluoksnių kūrimą, kad vienam sluoksniui sugedus kiti sluoksniai vis tiek galėtų užkirsti kelią žalai. Dažnai cituojamas gynybos gilynėjimo modelio pavyzdys yra prevencinių priemonių, taikomų siekiant užkirsti kelią infekcinėms ligoms, rinkinys. Vakcinos, kaukės ir rankų plovimas, be kitų priemonių, gali reikšmingai sumažinti infekcijos riziką kartu, net jei nė viena iš šių metodų nėra 100% veiksminga savaime (‡1083*). Bendrosios paskirties dirbtiniam intelektui gynybos gilynėjimas apims kontrolės priemones, kurios nėra pačiame dirbtinio intelekto modelyje, o susijusios su platesne ekosistema. Tai apima (pavyzdžiui) kontrolės priemones, taikomas medžiagoms, reikalingoms biologiniam išpuoliui vykdyti, pavyzdžiui, reagentams (‡1084, ‡1085). Vis dėlto gynybos gilynėjimo priemonės pirmiausia sprendžia su incidentais, gedimais ir piktybiniu naudojimu susijusią riziką ir gali atlikti mažesnį vaidmenį valdant sistemines rizikas (žr. §3.5. Visuomenės atsparumo stiprinimas).

Įmonės išleidimo ir diegimo strategija yra svarbi rizikos mažinimo sudedamoji dalis. Sprendimai dėl to, kaip modeliai tampa prieinami naudotojams, gali reikšmingai paveikti rizikos lygį (‡1082). Skirtingos išleidimo ir diegimo galimybės apima laipsnišką išleidimą ribotoms naudotojų grupėms, prieigą per kontroliuojamas internetines paslaugas (pvz., API) ir licencijavimo sutarčių bei priimtino naudojimo politikų taikymą, kurios teisiškai draudžia tam tikras žalingas taikymo sritis (‡176, ‡1086, ‡1087). §3.4. Atviro svorio modeliai išsamiau aptaria, kaip išleidžiant modelių svorius daromos rizikos.

###@ Rizikų valdymas

Rizikos valdymas yra procesas, kuriuo rizikos valdymo vertinimai, sprendimai ir veiksmai susiejami su organizacijos ar kito subjekto strategija ir tikslais (‡1088, ‡1089). 3.4 lentelėje pateikiama įprastų rizikos valdymo metodų apžvalga. Kaip parodyta Figūra 3.4, rizikos valdymą galima suprasti kaip rizikos valdymo pagrindą, nes jis palengvina veiksmingą kitų rizikos valdymo komponentų veikimą. Jis suteikia atskaitomybę, skaidrumą ir aiškumą, kurie palaiko informuotus rizikos valdymo sprendimus. Rizikos valdymas gali apimti tokias praktikas kaip incidentų pranešimas (‡1090), rizikos atsakomybės paskirstymas (‡965) ir pranešėjų apsauga (‡1091). Plačiau rizikos valdymas gali apimti gaires, sistemas, teisės aktus, reglamentavimą, nacionalinius ir tarptautinius standartus, taip pat mokymo ir švietimo iniciatyvas. Pagrindinis rizikos valdymo tikslas yra nustatyti organizacines politikos nuostatas ir mechanizmus, kurie aiškiai apibrėžia, kaip rizikos valdymo atsakomybės paskirstomos visoje organizacijoje ar kitame subjekte, siekiant užtikrinti tinkamą priežiūrą ir atskaitomybę (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dokumentacija
  Dokumentavimo praktikos padeda sekti svarbiausią informaciją apie AI sistemas, pavyzdžiui, mokymo duomenis, projektavimo sprendimus, numatytą paskirtį, apribojimus ir rizikas. „Modelio kortelės“ ir „sistemos kortelės“, kurios pateikia informaciją apie tai, kaip AI modelis ar sistema buvo apmokyti ir įvertinti, yra pavyzdžiai žinomų AI dokumentavimo gerųjų praktikų (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Incidentų registravimas
  Incidentų registravimas yra procesas, kurio metu sistemiškai dokumentuojami ir dalijamasi atvejais, kai kuriant arba diegiant AI buvo padaryta tiesioginė ar netiesioginė žala. Yra kelios platformos, kurios palengvina AI incidentų registravimą (‡1096, ‡1097), ir taikomos gairės, skirtos efektyvesniam AI incidentų registravimui (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rizikos valdymo sistemos
  Rizikos valdymo sistemos yra organizaciniai planai, skirti sumažinti spragas rizikos aprėptyje, koordinuoti įvairias rizikos valdymo veiklas ir įdiegti kontrolės bei balanso mechanizmus. Su bendrosios paskirties dirbtiniu intelektu susijusios sistemos (‡986, ‡1098) dažnai nurodo kitas šiame skyriuje paminėtas priemones.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rizikų registras
  Rizikų registras yra įvairių rizikų saugykla, kurioje nurodomas jų prioritetizavimas, atsakingi asmenys ir mažinimo planai. Tai gana įprasta daugelyje pramonės šakų, įskaitant kibernetinį saugumą (‡1099), ir kartais naudojama atitikčiai reguliavimo reikalavimams užtikrinti.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rizikų atsakomybės paskirstymas
  Vaidmenų ir atsakomybių paskirstymas rizikų valdymui organizacijoje gali suformuoti vidinę sprendimų priėmimo priežiūrą (‡1002, ‡1093). Tokie susitarimai atsispindi kai kuriose valdymo sistemose, įskaitant ES bendrosios paskirties DI elgesio kodeksą (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Skaidrumo ataskaitos
  Skaidrumo ataskaitos aprašo AI įmonės rizikos valdymo praktikas viešai atskleisdamos tam tikrą informaciją arba dalydamosi dokumentacija su pramonės grupėmis ar vyriausybinėmis įstaigomis. Pavyzdžiui, daugelis AI įmonių teikia Hirošimos AI procesą (HAIP) skaidrumo ataskaitas (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pranešėjų apsauga
  Kadangi dauguma AI kūrimo darbų vyksta už uždarų durų, kai kuriose valdymo sistemose numatomos pranešėjų apsaugos, kad būtų galima pranešti kompetentingoms institucijoms apie galimą riziką (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.4 lentelė. Bendrosios paskirties dirbtinio intelekto rizikos valdymo rizikos valdymas
>white|black||9|11|br Pavyzdiniai dirbtinio intelekto (DI) rizikų valdymo metodai pateikiami abėcėlės tvarka. Įtraukti metodai skirti tuo pat metu remti rizikų valdymą daugeliui skirtingų rizikų tipų, įskaitant rizikas, susijusias su piktnaudžiavimu, rizikas dėl veikimo sutrikimų ir sistemines rizikas. Atsižvelgiant į dar tik besiformuojantį bendrosios paskirties DI rizikų valdymą, ne visi metodai tiks kiekvienam DI kūrėjui ar diegėjui.


>white|orangered|left|14|15.5|bb Dokumentavimas ir skaidrumas yra rizikos valdymo sudedamosios dalys

Dokumentavimo ir institucinės skaidrumo priemonės, kartu su informacijos dalijimosi praktikomis, palengvina išorinį vertinimą ir padeda valdyti rizikas, susijusias su bendrosios paskirties AI (‡1101, ‡1102). Tapo įprasta skelbti išankstinių diegimo testų rezultatus „modelio kortelėje“ arba „sistemos kortelėje“, kartu pateikiant pagrindinę informaciją apie modelį ar sistemą, įskaitant tai, kaip ji buvo apmokyta, ir kokie yra galimi jos apribojimai (‡1094, ‡1095). Kai kurie kūrėjai taip pat skelbia skaidrumo ataskaitas, kuriose plačiau aprašomos jų rizikos valdymo praktikos (‡1103). Kiti dokumentavimo ir skaidrumo elementai apima stebėseną ir incidentų registravimą (‡176, ‡1083*, ‡1103) bei informacijos dalijimąsi, kurį gali palengvinti trečiosios šalys, pavyzdžiui, Frontier Model Forum. Kai kurios reguliavimo sistemos, pavyzdžiui, ES AI Aktas arba Kalifornijos Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53) (‡1081, ‡1104), kai kuriais atvejais įpareigoja dalytis informacija apie bendrosios paskirties AI keliamas rizikas.

>white|orangered|left|14|15.5|bb Lyderystės įsipareigojimas ir skatinamosios priemonės formuoja rizikos valdymo praktiką

Organizacinė kultūra, vadovavimo struktūra ir skatinimo priemonės įvairiais būdais veikia rizikos valdymo pastangas (‡1105). Vadovybės įsipareigojimas ir skatinimo struktūros dažnai yra svarbios tam, kaip rizikos valdymo politika praktiškai veikia. Kai kurie kūrėjai turi vidines sprendimų priėmimo komisijas, kurios svarsto, kaip saugiai ir atsakingai projektuoti, kurti ir peržiūrėti naujas AI sistemas. Priežiūros ir konsultaciniai komitetai, pasitikėjimo organai ar AI etikos tarybos taip pat gali veikti kaip rizikos valdymo gairių ir organizacinės priežiūros mechanizmai (‡1092*, ‡1106, ‡1107, ‡1108). Tyrėjai teigė, kad savanoriško savireguliavimo iššūkiai reiškia, jog trečiųjų šalių auditas, patikrinimas ir standartizavimas galėtų padėti sustiprinti bendrosios paskirties AI rizikos valdymą (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Organizacinės rizikų valdymo, skaidrumo ir rizikų atskaitomybės sistemos

Keli nauji iniciatyvų projektai dėmesį skiria rizikos valdymo procesams, dokumentavimui ir skaidrumui. Dabartine forma ES bendrosios paskirties DI kodeksas (AI Code of Practice) veikia kaip savanoriška sistema, skirta skaidrumo, autorių teisių bei saugos ir kibernetinio saugumo praktikoms, kurios padeda užtikrinti atitiktį ES DI akto nuostatoms dėl bendrosios paskirties DI (‡965). Nuo 2025 m. gruodžio daugiau nei dvi dešimtys įmonių† yra pasirašiusios. G7 Hirošimos DI procesas (HAIP) pateikimo sistema (‡1100) yra pirmoji tarptautinė sistema savanoriškam viešam organizacinės rizikos valdymo praktikų, taikomų pažangiems DI sistemoms, atskleidimui. Bent 20 kūrėjų paskelbė viešus skaidrumo pranešimus, apimančius rizikos identifikavimą, vertinimo metrikas, mažinimo strategijas ir duomenų saugumo procesus.

AI kūrėjai priėmė savanoriško skaidrumo įsipareigojimus. Kinijoje 17 Kinijos AI bendrovių pažadai, koordinuojami Kinijos AI pramonės aljanso (AI Industry Alliance of China), buvo paskelbti 2024 m. gruodį (‡1113) ir atnaujinti 2025 m. (‡1114). 2024 m. gegužę Pietų Korėjoje vykusiame AI Seoul Summit pasirašė 16 AI kūrėjų iš kelių šalių savanoriškus įsipareigojimus skelbti Frontier AI Safety Frameworks savo pažangiausiems modeliams ir sistemoms bei taikyti rizikos valdymo praktikas visuose modelio kūrimo ir diegimo etapuose (‡1052).

    Pastaba † -- Pasirašiusieji nuo 2025 metų gruodžio mėn. apima: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing ir WRITER.

>white|orangered|left|14|15.5|bb „Frontier“ AI saugos sistemos tapo išskirtiniu organizaciniu požiūriu į AI rizikos valdymą

Nuo 2023 m. keli pažangūs AI kūrėjai savanoriškai paskelbė dokumentus, kuriuose aprašo, kaip planuoja nustatyti ir reaguoti į rimtas rizikas, kylančias iš jų pažangiausių sistemų. Šios Pažangiojo AI saugos sistemos aprašo, kaip AI kūrėjas planuoja įvertinti, stebėti ir kontroliuoti savo pažangiausius AI modelius ir sistemas prieš diegimą ir jo metu. Šios sistemos daug kuo panašios, tačiau skiriasi esminiais aspektais (‡1115, ‡1116). Dauguma dėmesio skiria rizikoms, susijusioms su cheminėmis, biologinėmis, radiologinėmis ir branduolinėmis (CBRN) grėsmėmis, pažangiais kibernetiniais gebėjimais ir pažangiu autonominiu elgesiu (‡1115, ‡1117). Mažuma sistemų apima papildomas rizikų sritis, tokias kaip neteisėta diskriminacija mastu ir vaikų seksualinis išnaudojimas.

Keli kūrėjai 2025 m. atnaujino savo sistemas (frameworks), pridėdami naujus skyrius apie žalingą manipuliavimą, nesuderinimo (misalignment) riziką bei autonominį replikavimą ir adaptaciją (‡1078, ‡1118). Nors daugelis sistemų aprašo panašius rizikos valdymo metodus – įskaitant grėsmių modeliavimą, red-team'ų (raudonųjų komandų) bandymus ir pavojingų galimybių (capabilities) įvertinimus – jos skiriasi tuo, kaip apibrėžia rizikos lygius ir slenksčius, kaip dažnai atliekami vertinimai, kokie yra rezervai tarp vertinimų ir slenksčių, taip pat kiek išsamiai įtraukiami jų įsipareigojimai dėl mažinimo (mitigation) (pavyzdžiui, ar jos apima modelio svorių (model weights) ištrynimą, ar tik kūrimo pristabdymą) (‡1115, ‡1119). Daugiau informacijos rasite Stalo 3.5.

>white|orangered|left|14|15.5|bb Daug veiksmų „Frontier AI Safety Frameworks“ pagrįsti įsipareigojimais „jeigu-tai“

Svarbi „Frontier AI Safety Frameworks“ dalis yra „if-then“ įsipareigojimai. Tai sąlyginiai protokolai, kurie suaktyvina konkrečius veiksmus, kai AI modeliai ir sistemos pasiekia iš anksto nustatytus gebėjimų slenksčius (‡1120). Pavyzdžiui, „if-then“ įsipareigojimas galėtų teigti, kad jei nustatoma, jog modelis geba reikšmingai padėti pradedantiesiems kuriant ir diegiant CBRN ginklus, tuomet kūrėjas įdiegs sustiprintas saugumo priemones, diegimo kontrolę ir realaus laiko stebėseną (‡991*).

2025 m. keli AI kūrėjai paskelbė, kad nauji modeliai išprovokavo ankstyvo įspėjimo signalus arba kad jie negalėjo atmesti galimybės, jog tolesnis vertinimas parodys, jog modeliai peržengė gebėjimų ribas. Dėl to jie, kaip atsargumo priemonę, ėmėsi sustiprintų apsaugos priemonių (‡7, ‡33, ‡1121*). „Frontier“ AI saugos pagrindų sistemos paprastai reikalauja atlikti pradinį gebėjimų vertinimą prieš taikant rizikos mažinimą, taip pat likutinės rizikos analizę arba saugos argumentą (safety case), dažnai pagrįstą red-teaming po mitigavimo. Daugiau informacijos rasite 3.5 lentelėje.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Parengties sistema 2 (‡1078*)
  Įtrauktos rizikos:
1. Biologiniai ir cheminiai pajėgumai
2. Kibernetinio saugumo gebėjimai
3. AI savęs tobulinimo galimybės
  Rizikos lygiai arba atitinkami rodikliai ir susijusios apsaugos priemonės:
- Aukštas: Gali sustiprinti esamus kelius į rimtą žalą (Reikia saugumo kontrolės ir apsaugos priemonių)
- Kritinis: Gali sukurti precedento neturinčius naujus kelius į sunkų pakenkimą (Sustabdyti tolesnę plėtrą, kol nurodytos apsaugos priemonės ir saugumo kontrolės atitiks Kritinį standartą)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Atsakingo mastelio didinimo politika 2.2 (‡991*)
  Įtrauktos rizikos:
1. CBRN ginklai
2. Autonominių dirbtinio intelekto tyrimų ir plėtros (AI T&P)
3. Kibernetinės operacijos (vertinimo etape)
  Rizikos lygių sistema arba lygiavertis modelis ir susijusios apsaugos priemonės:
  AI saugos lygiai (ASL)
- ASL-1: Nėra reikšmingos katastrofinės rizikos
- ASL-2: Ankstyvieji pavojingų galimybių požymiai (modeliai turi atitikti ASL-2 diegimo ir saugumo standartus)
- ASL-3: Iš esmės padidėjusi katastrofiško netinkamo naudojimo rizika (Modeliai turi atitikti ASL-3 diegimo ir/ ar saugumo standartus)
- ASL-4+: Būsimos klasifikacijos (dar neapibrėžtos)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Frontier Safety Framework 3.0 (‡1040*)
  Įtrauktos rizikos:
1. Piktnaudžiavimas
    a. CBRN
    b. Cyber
    c. Kenksmingas manipuliavimas
2. Mašininio mokymosi MTTP
3. Nesutapimas / instrumentinis samprotavimas
  Rizikos lygiai arba lygiavertis ir su jais susijusios apsaugos priemonės:
  Kritiniai gebėjimų lygiai
    Gebėjimų lygiai, kuriuose, nesant švelninančių priemonių (saugos atvejai diegimams ir saugumo švelninančios priemonės, suderintos su RAND saugumo lygiais 2, 3 arba 4 (‡1122)), AI modeliai arba sistemos gali kelti padidėjusią didelės žalos riziką. Gebėjimų lygiai apima „ankstyvojo įspėjimo vertinimus“, su konkrečiais „įspėjimo slenksčiais“
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Frontier AI Framework 1.1 (‡990*)
  Įtrauktos rizikos:
1. Kibernetinis saugumas
2. Cheminės ir biologinės rizikos
  Rizikos lygiai arba atitinkami ir susijusios apsaugos priemonės:
  Rizikos slenksčio lygiai
- Vidutinis (išleidimas taikant atitinkamas saugumo priemones ir švelninimo priemones)
- igh (neatleiskite)
- Kritinis (sustabdyti kūrimą)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Frontier Model Safety Framework (‡1123*)
  Įtrauktos rizikos:
1. CBRN ginklų platinimas
2. Kenksmingos kibernetinės operacijos
3. Automatizuoti AI moksliniai tyrimai ir plėtra
  Rizikos lygiai arba atitinkami ir susijusios apsaugos priemonės:
  Kritinės gebėjimų ribos
    Modelio gebėjimai, kurie turi potencialą daryti didelę žalą visuomenei, jei bus piktnaudžiaujama. (Jei slenksčiai yra pasiekti arba viršyti, modelis nebus viešai diegiamas be tinkamų rizikos mažinimo priemonių)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Frontier Governance Framework (‡1124*)
  Įtrauktos rizikos:
1. CBRN ginklai
2. Kenksmingos kibernetinės operacijos
3. Pažangi autonomija (įskaitant AI mokslinius tyrimus ir plėtrą)
  Rizikos lygiai arba lygiavertės priemonės ir susijusios apsaugos priemonės:
  Rizikos lygiai
- Žemas arba Vidutinis (Įdiegimas leidžiamas pagal Atsakingo dirbtinio intelekto programos reikalavimus)
- Aukštas arba Kritinis (tolimesnė peržiūra ir švelninimo priemonės)
(reikalinga)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Frontier AI Rizikos vertinimas (‡1029*)
  Įtrauktos rizikos:
1. Kibernetinis nusikaltimas
2. CBRN
3. Įtikinėjimas ir manipuliavimas
4. Netinkama diskriminacija mastuodama
  Rizikos lygiai arba atitinkami ir susijusios apsaugos priemonės:
  Rizikos slenksčiai – modelio rizikos (MR) balai
- MR1 arba MR2 (Vertinimo rezultatai yra dokumentuojami inžinerijos komandų)
- MR3 (Rizikos mažinimo priemonės ir vertinimo rezultatai yra dokumentuojami inžinerijos komandų ir periodiškai peržiūrimi)
- MR4 (Išsamus rizikos vertinimas turi būti atliktas ir reikalingas verslo padalinio vadovo patvirtinimas)
- MR5 (Išsamus rizikos vertinimas turi būti atliktas ir patvirtintas nepriklausomo komiteto, pvz., NVIDIA AI etikos komiteto)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Saugus AI pažangiausio modelio sistemos pagrindas (‡1125*)
  Įtrauktos rizikos:
1. Kenksmingas naudojimas (pvz., kenkėjiška programinė įranga, vaikų seksualinis išnaudojimas)
2. Žala įprastame, nekenksmingame naudojime, pvz. išvestys, dėl kurių gaunamas neteisėtas diskriminacinis rezultatas, arba nesaugaus kodo generavimas
  Rizikos lygiai arba atitinkamas terminas ir susijusios apsaugos priemonės:
  Kenkimo tikimybė ir sunkumas kontekste
- Žema
- Vidutinis
- Aukštas
- Labai aukštas
    (Rizikos mažinimo priemonės ir saugumo kontrolės yra įdiegtos visoms sistemoms ir procesams; papildomos priemonės turi būti pritaikytos AI sistemai ir naudojimo atvejui, kuriame modelis yra diegiamas)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: AGI Pasirengimo politika (‡1127*)
  Įtrauktos rizikos:
1. Kibernetinis nusikaltimas
2. Automatizuoti AI moksliniai tyrimai ir plėtra
3. Autonominis replikavimas ir adaptacija
4. Biologinių ginklų pagalba
  Rizikos lygiai arba lygiavertės kategorijos ir susijusios apsaugos priemonės:
  Kritinės gebėjimų ribos
    Kiekybinės ribos pagal pajėgumų etalonus (jei viršijamos, atlikite pavojingų pajėgumų įvertinimus, informacijos saugumo priemones ir diegimo mažinimus, arba sustabdykite kūrimą)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: AGI pasirengimo politika (‡1127*)
  Įtrauktos rizikos:
1. Kibernetinis nusikaltimas
2. Automatizuoti AI moksliniai tyrimai ir plėtra
3. Autonominis dauginimasis ir pritaikymas
4. Biologinių ginklų pagalba
  Rizikos lygiai arba atitinkami lygiaverčiai rodikliai ir susijusios apsaugos priemonės:
  Kritinės gebėjimų ribos
    Kiekybiniai pajėgumų etalonų slenksčiai (Jei viršijami, atlikti pavojingų pajėgumų vertinimus, informacijos saugumo priemones ir diegimo mažinimo veiksmus arba nutraukti kūrimą)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: AI saugos sistema (‡1128*)
  Įtrauktos rizikos:
1. Kontrolės praradimas
2. Netinkamas naudojimas (pvz., biocheminis ginklų gaminimas
  Rizikos pakopos arba atitinkamas lygis ir susijusios apsaugos priemonės:
  Rizikos lygiai
- Maža rizika (Įdiegti AI sistemas, bet vėliau atlikti stebėseną, kad būtų galima valdyti rizikas)
- Rizika nustatyta (arba taikyti tik leistiniems naudotojams „OpenAI“ sistemas, kad būtų sušvelnintos rizikos, arba atidėti diegimą, kol bus imtasi papildomų saugos priemonių, atsižvelgiant į naudojimo atvejį)
- Didelė rizika (N diegti AI sistemas)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Pažangios AI saugos sistema „Frontier“ (‡1129*)
  Įtrauktos rizikos:
1. Biologinės grėsmės
2. Įžeidžiantis kibernetinis saugumas
3. Autonominis veikimas ir pažangus manipuliavimas
  Rizikos lygiai arba lygiavertės reikšmės ir susijusios apsaugos priemonės:
  Rizikos lygiai
- 1 lygis (Pagrindinės apsaugos priemonės dėl minimalių rizikų ir galimybės išleisti atvirojo kodo)
- 2 lygis (realiojo laiko stebėsena, užklausų filtravimas, elgsenos anomalijų aptikimas, prieigos kontrolė, raudonojo komandos testavimas ir priešiškos simuliacijos)
- 3 lygis (pažangios saugiklio priemonės, įskaitant „red-teaming“, etapinius diegimus, priešišką testavimą, šifravimą, kelių šalių prieigos valdiklius ir nulinio pasitikėjimo architektūrą)
- 4 lygis (Maksimalūs saugos protokolai aukštos svarbos modeliams ir maksimalios saugumo priemonės)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.5 lentelė. Ribinės AI saugos sistemos
>white|black||9|11|br Pirmasis Frontier AI Safety Frameworks rinkinys, kurį išleido dalis AI kūrėjų, pasirašiusių Frontier AI Safety Commitments. Šie frameworks apima panašias rizikas (su nežymiais skirtumais) ir taiko skirtingus rizikos lygius bei rizikos valdymo metodus.


>white|orangered|left|14|15.5|bb „Frontier AI Safety Frameworks“ veiksmingumas nėra aiškus.

„Frontier AI Safety Frameworks“ gali būti naudojami kaip rizikos valdymo priemonės tam tikromis sąlygomis ir tam tikroms rizikos kategorijoms, turinčioms pagrįstą kelią į žalą (‡1117). Tuo pat metu keliuose tyrimuose aptariami klausimai dėl jų aiškumo ir apimties (‡111, ‡986) bei dėl AI galimybių ir rizikos slenksčių patvarumo (‡1031, ‡1130). Esamos sistemos dažniausiai koncentruojasi į dalį rizikos sričių. Dėl to kai kurios ryškios rizikos, pavyzdžiui, neteisėtas stebėjimas (‡1131, ‡1132) ir ne sutikimu grįsti intymūs vaizdai (‡287), sulaukia mažiau dėmesio. Skirtingai nei rizikos valdymo metodai iš kitų sektorių, pavyzdžiui, aviacijos ar branduolinės energetikos (‡1133*), „Frontier AI Safety Frameworks“ paprastai nenaudoja aiškių kiekybinių rizikos slenksčių (‡1134).

Išoriniai kūrėjų atitikties jų Frontier AI Safety Frameworks vertinimai kol kas išlieka riboti, iš dalies todėl, kad dauguma šių sistemų yra naujos, viešai prieinamos informacijos stinga, o standartizuotų išorinių auditų nėra. Jų veiksmingumas taip pat priklausys nuo to, kaip gerai – ir kokiu mastu – įsipareigojimai įgyvendinami praktikoje. Vien tik šios sistemos gali neužtikrinti veiksmingo rizikų valdymo, nes jų praktinis poveikis priklauso nuo to, kaip gerai – ir kokiu mastu – jos įgyvendinamos. Iki šiol jos nevisiškai atitinka tarptautinius rizikų valdymo standartus (‡1135). Tyrimas dėl ankstesnių savanoriškų įsipareigojimų nustatė netolygų įgyvendinimą tarp priemonių, o tai rodo, kad laikymasis savanoriškų įsipareigojimų greičiausiai skirsis tarp įmonių ir sričių (‡1109).

Kartu paėmus, „Frontier AI Safety Frameworks“ atstovauja išsamiausiai šiuo metu naudojamai savanoriško organizacinės rizikos valdymo formai, tačiau reikšmingai skiriasi apimtimi, ribinėmis vertėmis ir vykdomumu.

###@ Reguliavimo ir valdymo iniciatyvos

>white|orangered|left|14|15.5|bb Keli jurisdikcijos priėmė įstatymus, kuriuose numatyti skaidrumo reikalavimai

Keli ankstyvieji reguliavimo metodai įveda teisines prievoles, skirtas didinti standartizavimą ir skaidrumą rizikos valdyme. ES AI įstatymas, įsigaliojęs 2024 m., nustato reikalavimus, susijusius su skaidrumu, autorių teisėmis ir sauga bendrosios paskirties AI modeliams. 2025 m. buvo paskelbtas ES bendrosios paskirties AI praktikos kodeksas, skirtas padėti laikytis šių įsipareigojimų, pateikiant gaires dėl modelio dokumentavimo ir autorių teisių, taip pat – pažangiausiems modeliams – rizikos valdymo praktikas, kaip antai vertinimai, rizikos įvertinimas ir mažinimas, informacijos sauga ir pranešimų apie rimtus incidentus teikimas (‡965).

Kiti naujų reguliavimo reikalavimų pavyzdžiai apima Pietų Korėjos sistemos įstatymą dėl dirbtinio intelekto plėtros ir pasitikėjimo užtikrinimo, kuris įveda reikalavimus „didelio poveikio“ dirbtinio intelekto sistemoms kritiniuose sektoriuose (‡1136), taip pat Kalifornijos SB 53, nustatančią skaidrumo reikalavimus saugos sistemoms ir incidentų registravimui (‡1104). Atsižvelgiant į tai, kaip neseniai šie reikalavimai buvo įtvirtinti, dar per anksti išsamiai įvertinti, kaip jie paveiks rizikos valdymo praktiką ar faktinius rizikos rezultatus.

>white|orangered|left|14|15.5|bb Plačios apimties valdymo iniciatyvos siūlo savanorišką gaires

Keli regioninio ir tarpregioninio valdymo pagrindai dabar išdėsto bendrus lūkesčius, kaip valdyti rizikas, kylančias iš bendrosios paskirties dirbtinio intelekto, pateikdami neprivalomas gaires politikos formuotojams ir organizacijoms. Kinijos AI saugos valdymo sistema 2.0, paskelbta 2025 m., pateikia struktūruotas gaires dėl rizikų kategorizavimo ir priemonių visame AI kūrimo ir diegimo procese (‡1137). ASEAN valstybės narės paskelbė „Išplėstinį ASEAN vadovą dėl AI valdymo ir etikos (generatyvusis AI)“, kuris pateikia gaires dėl bendrosios paskirties dirbtinio intelekto valdymo ir etikos ir yra skirtas padėti užtikrinti didesnį politikos suderinamumą tarp ASEAN valstybių narių (‡1138). Be to, ekspertų inicijuotos iniciatyvos, pavyzdžiui, Singapūro konsensusas, kurį parengė AI mokslininkai iš kelių šalių, išdėsto mokslinių tyrimų prioritetus bendrosios paskirties AI saugai, apimančiai rizikos vertinimą, kūrimą ir kontrolę (‡690).

###@ Atnaujinimai

Nuo paskutinės Ataskaitos paskelbimo (2025 m. sausis) bendrosios paskirties dirbtinio intelekto rizikos valdymo aplinka pasikeitė: paskelbti nauji ištekliai, tokie kaip ES Bendrosios paskirties dirbtinio intelekto elgesio kodeksas, G7 HAIP atskaitomybės sistema, Kinijos nacionalinė dirbtinio intelekto saugos valdymo sistema 2.0 ir įvairūs AI kūrėjų Frontier AI Safety Frameworks. Šios iniciatyvos aprašo metodus ir praktiką, kuriuos AI kūrėjai taiko valdydami rizikas, susijusias su bendrosios paskirties AI sistemomis (‡1115). Yra reikšmingų skirtumų tarp Frontier AI Safety Frameworks ir tarp HAIP skaidrumo ataskaitų (‡1103), atspindinčių skirtingą organizacinę praktiką, rizikų prioritetizavimą ir ankstyvą bendrosios paskirties AI rizikos valdymo ekosistemos raidos etapą. Patikima ekosistema, kurioje skirtingi AI veikėjai prisideda papildoma rizikos valdymo praktika per visą gyvavimo ciklą, gali prisidėti prie veiksmingo rizikos valdymo (‡690).

###@ Įrodymų spragos

Trūksta įrodymų apie: kaip matuoti kylančių rizikų sunkumą, paplitimą ir laiko horizontą; kokiu mastu šias rizikas galima sumažinti realiomis sąlygomis; ir kaip veiksmingai paskatinti arba įpareigoti rizikos mažinimo diegimą įvairių tipų subjektams. Reikia daugiau tyrimų, siekiant suprasti, kaip dažnai pasitaiko skirtingos rizikos ir kiek jos skiriasi skirtinguose pasaulio regionuose, ypač tokiuose regionuose kaip Azija, Afrika ir Lotynų Amerika, kurie sparčiai skaitmenizuojasi. Kadangi AI modeliams suteikiama vis didesnė veikimo savarankiškumas ir autoritetas, o bendrosios paskirties AI rizikų mokslo būklė progresuoja, rizikos valdymo metodai taip pat turės keistis (‡639, ‡1139).

Tam tikros rizikos mažinimo priemonės vis populiarėja (‡690, ‡956), tačiau reikia daugiau tyrimų, kad būtų suprasta, kaip praktiškai yra tvirtos rizikos mažinimo priemonės ir apsaugos priemonės skirtingoms bendruomenėms ir AI veikėjams (įskaitant mažas ir vidutines įmones). Prieiga prie duomenų apie realaus gyvenimo diegimą ir modelių naudojimą yra svarbi tokiems vertinimams. Be to, rizikos valdymo pastangos šiuo metu labai skiriasi tarp pirmaujančių AI įmonių. Teigta, kad kūrėjų paskatos nėra gerai suderintos su išsamiu rizikos vertinimu ir valdymu (‡934). Vis dar trūksta įrodymų apie tai, kokiu mastu skirtingi savanoriški įsipareigojimai yra įgyvendinami, su kokiomis kliūtimis įmonės susiduria, kai visapusiškai laikosi įsipareigojimų, ir kaip jos integruoja Frontier AI Safety Frameworks į platesnes AI rizikos valdymo praktikas.

###@ Iššūkiai politikos formuotojams

Pagrindiniai iššūkiai apima tai, kaip prioritetizuoti įvairią bendrosios paskirties AI keliamų rizikų spektrą, išaiškinti, kurie veikėjai yra geriausiai pasirengę jas mažinti, ir suprasti paskatas bei suvaržymus, kurie formuoja jų veiksmus. Įrodymai rodo, kad politikos formuotojai šiuo metu turi ribotą prieigą prie informacijos apie tai, kaip AI kūrėjai ir diegėjai testuoja, vertina ir stebi kylančias rizikas, taip pat apie tai, kokio veiksmingumo turi skirtingos rizikos mažinimo praktikos (‡1140). Tyrėjai ir politikos formuotojai yra aptarę, kad skaidrumo iniciatyvos ir nuoseklesnis incidentų (incident) pranešimas galėtų padėti informuoti apie rizikų prioritetizavimą, stiprinti pasitikėjimą ir skatinti atsakingą kūrimą (‡957). Praktikoje rizikos valdymas apima kelis veikėjus visoje AI vertės grandinėje – pavyzdžiui, duomenų ir debesijos paslaugų teikėjus, modelių kūrėjus ir modelių talpinimo platformas – kurių kiekvienas turi skirtingas galimybes vertinti ir valdyti skirtingas rizikas (‡1141). Ribotas informacijos dalijimasis tarp šių veikėjų apsunkina nustatyti, kurios rizikos yra labiausiai tikėtinos ar reikšmingos, ypač kai atsižvelgiama į poveikį visuomenei downstream'e.

