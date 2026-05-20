Bendros paskirties AI sistemos žlunga taip, kaip jau yra padariusios realią žalą, nuo suklastotų teisinių nuorodų iki neteisingų medicininių diagnozių. Nors ir žmonių specialistai daro klaidų, AI žlugimai kelia išskirtinius susirūpinimus dėl savo naujumo, galimo mastelio, sunkumo numatyti, kada jie įvyks, ir naudotojų polinkio nekritiškai pasitikėti įtikinamai skambančiais rezultatais. Dabartiniai bendros paskirties AI žlugimai apima klaidingos informacijos pateikimą (‡602, ‡603), pagrindinių samprotavimo klaidų padarymą (‡604, ‡605) ir suprastėjimą, kai jos diegiamos naujuose kontekstuose (‡606, ‡607, ‡608). Fiksuota tokio pobūdžio žala apima medicinines klaidingas diagnozes, klaidas teisiniuose procesiniuose dokumentuose ir finansinius nuostolius (‡609, ‡610, ‡611). Patikimumo iššūkiai ypač svarbūs AI agentams, nes gedimai gali tiesiogiai sukelti žalą be žmogaus veiksmų ar priežiūros (‡612, ‡613, ‡614, ‡615). Daugiaagentės sistemos įveda dar daugiau žlugimo režimų dėl netinkamo koordinavimo, konfliktų arba nepageidaujamo agentų susimokymo (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Haliucinacija
- Citavimas neegzistuojančio precedento teisiniuose pareiškimuose (‡617)
- Nurodant neegzistuojančias sumažintų tarifų politikos nuostatas gedinantiems keleiviams (‡618)
- Pateikiama netiksli ir šališka medicininė informacija (‡619)
- Pateikiama pasenusi informacija apie įvykius (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pagrindinis samprotavimo gedimas
- Nepavyksta atlikti matematinių skaičiavimų (‡621)
- Nepavyksta nustatyti pagrindinių priežasties ir pasekmės ryšių (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Neišmokus pasiskirstymo gedimas (gedimas dėl neįprastų ar nepažįstamų įvesčių)
- Neteisingas vaizdų klasifikavimas, kai kinta foninis apšvietimas arba kontekstas (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Įrankio naudojimo klaida
- Privatumo pažeidimas dėl vartotojo privataus vaizdo atskleidimo naudojant AI agentą, kuris jį siunčia trečiajai šaliai įrankiui (‡624)
- Trumpalaikės darbinės atminties veikimo sutrikimas (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Daugiagentės sistemos gedimas: nesuderinamumas ir konfliktas
- Nepavyksta valdyti bendrų išteklių dėl konflikto tarp individualių paskatų ir kolektyvinės gerovės tikslų (‡627)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Stalo 2.4: Patikimumo problemų pavyzdžiai bendrosios paskirties DI ir agentų sistemose
>white|black||9|11|br Dokumentuotos patikimumo problemos bendrosios paskirties dirbtinio intelekto sistemose, dirbtinio intelekto agentuose ir daugiagentėse sistemose.


###@ Bendrosios paskirties AI sistemos susiduria su įvairiais patikimumo iššūkiais

2.4 lentelė apibendrina dažniausias patikimumo problemų kategorijas. Pirmios trys taikomos visoms AI sistemoms, o paskutinės dvi konkrečiai susijusios su AI agentais ir daugiagentėmis sistemomis. Daugelį patikimumo rizikų lemia tai, kad sudėtinga numatyti ir stebėti AI sistemos elgseną.

Šie iššūkiai (toliau aptariami 3.1 §. Techniniai ir instituciniai iššūkiai) ypač aštrūs dirbant su AI agentais sudėtingose aplinkose. Dabartiniai metodai, skirti įvertinti tokius gedimus ir juos sušvelninti, gali sumažinti gedimų dažnį, tačiau net ir pažangiausi AI agentai vis dar yra pakankamai nepatikimi, kad kelia rizikų ir trukdo diegti daugelyje kontekstų.

„Patikimumas“ reiškia mastą, kuriuo AI sistema veikia taip, kaip numatė kūrėjas arba vartotojas. Bendrosios paskirties AI sistemos susiduria su įvairiomis patikimumo problemomis – nuo netikslaus ar klaidinančio turinio generavimo iki nesugebėjimo atlikti pagrindinio samprotavimo. Pavyzdžiui, nors modeliai pagerino faktinės informacijos atgaminimą, net ir lyderiaujantys modeliai vis dar pakankamai dažnai pateikia įsitikinusių, bet neteisingų atsakymų (Figūra 2.10). Programinės inžinerijos srityje bendrosios paskirties AI dabar gali suteikti reikšmingą pagalbą rašant, vertinant ir derinant kompiuterinį kodą (‡215*, ‡628, ‡629). Tačiau AI sugeneruotame kode dažnai yra klaidų (‡630), o kodavimo agentai reguliariai daro klaidas (‡631). Tokie nepakankamumai gali įdiegti pažeidžiamumus programose ir saugumo sistemose (žr. §2.1.3. Cyberattacks).

Patikimumo problemos ypač svarbu stebėti didelės rizikos aplinkose, tokiose kaip medicina, dėl spartėjančio DI naudojimo ir galimo nesėkmių, galinčių sukelti rimtą žalą (‡609, ‡619). Aktualūs gebėjimai greitai gerėjo: pirmaujantys modeliai dabar jau gali išlaikyti medicininius egzaminus (‡633*, ‡634). Tačiau realus naudojimas atskleidžia ribotumus, kurių neaptinka etalonai. Pavyzdžiui, viename tyrime modeliai pateikė potencialiai žalingus atsakymus į 19% medicininių klausimų (‡635). Tokios nesėkmės gali lemti neteisingą diagnozę, netinkamą gydymą arba nepagrįstą priežiūros atsisakymą (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Figūra 2.10: Pagrindinių modelių rezultatai SimpleQA Verified etaloniniame rinkinyje
>white|black||9|11|br Pagrindinių modelių rezultatai pagal išleidimo datą „SimpleQA Verified“ etaloniniame (benchmark) rinkinyje. Šis etalonas matuoja modelio faktų tikslumą, t. y. modelio gebėjimą patikimai prisiminti faktus. Jis turi trumpą klausimų-atsakymų (QA) formatą, skirtą nustatyti patikimumo problemas, tokias kaip haliucinacijos. Šaltinis: „SimpleQA“ „Kaggle“  2*).


>white|orangered|left|14|15.5|bb AI agentai kelia naujų patikimumo rizikų dėl savo autonomiškumo

Kadangi AI agentai tiesiogiai veikia realiame pasaulyje, jų nesėkmės gali padaryti daugiau žalos nei nesėkmės neagentiniuose sistemose (‡99). Skirtingai nuo AI sistemų, kurios tik kuria tekstą ar vaizdus žmonėms peržiūrėti, AI agentai gali savarankiškai atlikti veiksmus, darančius poveikį pasauliui (‡99, ‡615, ‡636, ‡637) (taip pat žr. §1.1. Kas yra bendrosios paskirties AI?). AI agentai gali inicijuoti veiksmus, daryti įtaką kitiems žmonėms arba AI sistemoms ir dinamiškai formuoti būsimas pasekmes. Didesnė įtakos apimtis įveda naujų rizikų ir padidina patikimumo svarbą, nes nesėkmės galėtų tiesiogiai sukelti žalą, neturint galimybės įsikišti žmogui (‡99, ‡612, ‡638, ‡639, ‡640). Tai gali būti ypač svarbu agentams, diegiamiems strateginėse arba saugos kritinėse aplinkose, tokiose kaip finansinės paslaugos (‡641), energijos valdymas (‡642) ar moksliniai tyrimai (‡643*, ‡644).

>white|orangered|left|14|15.5|bb Kelių agentų AI sistemos įveda naujų rūšių patikimumo gedimus

Daugiagentės AI sistemos įveda naujų patikimumo gedimų rūšių dėl koordinavimo gedimų arba agentų tarpusavio konflikto. Daugiagentėse AI sistemose agentai sąveikauja tarpusavyje siekdami arba bendrų, arba individualių tikslų (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). Pavyzdžiui, daugiagentėje sistemoje, sukurtoje atlikti mokslinės literatūros apžvalgą, lyderio agentas suskaido naudotojo užklausą ir priskiria užduotis specializuotiems podagentams, kurių kiekvienas lygiagrečiai tiria skirtingą aspektą (‡650*). Nors tai leidžia pasiekti efektyvumo pranašumų, kartu tai reiškia, kad klaidos gali plisti tarp agentų (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Jei keli agentai sukurti remiantis tuo pačiu baziniu modeliu arba įtraukiantys tuos pačius įrankius, jie taip pat gali pasižymėti koreliuojamais gedimais (‡656). Empiriniai įrodymai apie tokius gedimus įdiegtose sistemose išlieka riboti, tačiau šios rizikos gali augti, kai daugiagentės sistemos taps vis įprastesnės.

###@ Atnaujinimai

Nuo ankstesnės ataskaitos paskelbimo (2025 m. sausis) komercinis ir mokslinių tyrimų susidomėjimas AI agentais labai išaugo. Vis daugiau AI agentų diegiami realiame pasaulyje (2.11 pav.), dauguma jų specializuojasi kompiuterio naudojimo arba programinės įrangos inžinerijos taikymuose (‡92). Naujausi leidiniai, tokie kaip XBOW hacking agent (‡467), Claude-4 (‡659) ir ChatGPT Agent (‡660), parodo besiformuojančius autonominius gebėjimus, pavyzdžiui, kurti skaidrių pristatymus remiantis Web paieškomis (‡660). Tačiau jie dar negali atlikti sudėtingesnių užduočių, tokių kaip planuoti ir užsakyti kelionę (‡100), nes nesėkmių rodikliai didėja ilgesnėms užduotims (‡98, ‡148). Dabartiniuose tyrimuose įtraukiamos pastangos sukurti standartus, kaip agentai bendrauja su išoriniais įrankiais ir kitais agentais (‡661, ‡662). Pavyzdžiai apima Google Agent2Agent (‡663) ir Agent Payments (‡664) protokolus, taip pat Anthropic Model Context Protocol (‡665).

>oldlace|black||11|15|br      
####@ Pastaba 2.4: Sąmoningi išpuoliai taip pat gali sukelti AI sistemų gedimą
>oldlace|black|left|13|15|hb  Pastaba 2.4: Sąmoningi išpuoliai taip pat gali priversti AI sistemas nepavykti
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Ši dalis sutelkia dėmesį į nenumatytus patikimumo gedimus, tačiau piktavaliai veikėjai taip pat gali tyčia sukelti gedimus per atakas, tokias kaip prompt injection. Prompt injection atakoje piktavaliai nurodymai agentui pateikiami netiesiogiai per tokius kanalus kaip paslėptos instrukcijos svetainėse ar duomenų bazėse (‡507, ‡657, ‡658). Šios instrukcijos gali „perimti“ agentą, priversdamos jį veikti prieš naudotojo ketinimus. Tokias atakas ypač sunku ginti, nes jos pristatomos naudojant išorinį turinį, nepriklausantį naudotojo ar kūrėjo kontrolei. AI sistemos, kaip atakų taikiniai, aptariamos toliau §2.1.3. Kibernetinės atakos, o kibernetinių atakų ir techninės gynybos priemonės aprašomos §3.3. Techninės saugiklio priemonės ir stebėsena.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Figūra 2.11: AI agentų skaičius išaugo nuo 2023 m.
>white|black||9|11|br 67 dislokuotų AI agentų 2024 m. gruodžio mėn. apklausos rezultatai. Kairėje: pagrindinių AI agentų leidimų laiko juosta. Dešinėje: taikymo sritys, kuriose naudojami AI agentai. Šešios sritys apibrėžtos remiantis dažniausiomis apklausoje nustatytomis naudojimo kategorijomis. Šaltinis: Casper ir kt., 2025 (‡92).


###@ Įrodymų spragos

Pagrindinės įrodymų spragos kyla dėl sunkumo patikimai įvertinti AI sistemų galimybes, ribotumus ir nesėkmių režimus (žr. §3.1. Techniniai ir instituciniai iššūkiai). Sistemingi AI agentų patikimumo vertinimai yra riboti ir neturi standartizavimo (‡92, ‡666). Kai kurios problemos, pavyzdžiui, priklausomybė nuo pasenusios informacijos (‡620), gali pasireikšti tik naudojant realioje aplinkoje, todėl išankstiniai vertinimai prieš diegimą yra nepakankami. Ankstesni darbai nagrinėjo agentų ir daugiagentinių sistemų patikimumą įprastinėje programinėje įrangoje ir ankstesnėse AI formose (‡647, ‡667, ‡668). Tačiau tokių darbų pritaikomumas moderniems AI agentams, kurie dažnai grindžiami dideliais kalbos modeliais, nėra aiškus (‡669). Kai kurie tyrėjai iškėlė susirūpinimą dėl naujų elgsenų, kurias agentai gali demonstruoti sąveikaudami tarpusavyje, pavyzdžiui, susitarimo (koluzijos) arba koreliuotų nesėkmių (‡614), tačiau empiriniai įrodymai išlieka riboti. Šias spragas siekiama mažinti, be kita ko, Nacionalinio standartų ir technologijų instituto (NIST) naujais agentų „pergrobimo“ (agent-hijacking) rizikų vertinimais (‡670), EBPO AI gebėjimų indikatoriais (‡243) ir JK AI saugumo instituto Inspect Sandboxing Toolkit (‡671).

###@ Šalinimai

Technikos, kaip pagerinti AI patikimumą, taikomos tiek pačiam modeliui, tiek platesnei sistemai, kurioje jis diegiamas. Tai gali sumažinti gedimų dažnį, tačiau nė viena priemonė dar negali užtikrinti tokio aukšto patikimumo, kokio reikia kritinėse srityse (‡672). Svarbi techninė priemonė yra priešiškas mokymas (adversarial training), kai mokymo metu modeliai yra veikiami sudėtingais įvesties duomenimis, kad išmoktų pateikti tinkamesnius, atsparesnius atsakymus (‡673, ‡674, ‡675, ‡676, ‡677) (žr. §3.3. Techninės apsaugos priemonės ir stebėsena). Norėdami sumažinti haliucinacijas, kūrėjai gali taikyti generavimą, papildytą paieška (retrieval-augmented generation, RAG), kuris papildo modelio atsakymus informacija, gauta iš išorinės duomenų bazės, taip padedant užtikrinti, kad išvestis būtų tiksli ir aktuali (‡678, ‡679, ‡680), arba konkrečiai koreguoti modelius, kad jie būtų labiau faktiniai (‡681), ar kad mąstytų veiksmingiau (‡682). Aplinkos ar įrankiais pagrįsti metodai taip pat gali padėti kūrėjams stebėti AI sistemas (‡683). Pavyzdžiui, diegėjai galėtų išbandyti AI sistemas ribotose, izoliuotose (sandbox) aplinkose, kad prieš plačiau diegdami išanalizuotų galimus gedimo scenarijus.

AI agentams konkrečiai tyrėjai pasiūlė patikimumą gerinti per didesnį skaidrumą, priežiūrą ir stebėseną. Pavyzdžiui, agentų sąveikų su išoriniais įrankiais ir su kitais agentais stebėjimas leistų veiksmingiau prižiūrėti agentų veiklas (‡684, ‡685) ir analizuoti incidentus (‡686). Metodai, kaip tokio pobūdžio informaciją rinkti automatiškai, įskaitant daugiagentines sąrankas, išlieka aktyvia mokslinių tyrimų sritimi (‡653, ‡654).

###@ Iššūkiai politikos formuotojams

Pagrindiniai politikos formuotojų iššūkiai apima AI agentų diegimo teikiamų privalumų įvertinimą, palyginti su patikimumo nesėkmių keliamomis rizikomis, ir užtikrinimą, kad kūrėjai, diegėjai ir naudotojai turėtų prieigą prie tikslios informacijos apie agentų veikimą ir rizikos profilius. Sprendimas, kaip priskirti atsakomybę už žalą, kurią sukelia AI agentai, kelia dar vieną iššūkį (‡639), ypač daugiagentėse sistemose, kur gali būti sunku nustatyti, kada ir kaip įvyko nesėkmės (‡687). Šiuos iššūkius dar labiau apsunkina agentų patikimumo vertinimo sudėtingumas, kai agentai įgyja daugiau autonomijos ir prieigos prie išorinių įrankių (‡688*, ‡689). Neapibrėžtumas dėl to, kaip greitai ims formuotis agentinės galimybės, taip pat apsunkina planavimą naujiems iššūkiams (žr. §3.1. Techniniai ir instituciniai iššūkiai, susiję su „įrodymų dilema“).

#### 2.2.2. Kontrolės praradimas

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Svarbiausia informacija
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Nekontroliuojamos situacijos yra situacijos, kai viena ar daugiau bendrosios paskirties dirbtinio intelekto sistemų veikia ne kieno nors kontroliuojamos, o atgauti kontrolę yra arba itin brangu, arba neįmanoma. Šios hipotezuojamos situacijos skiriasi pagal savo sunkumą, tačiau kai kurie ekspertai pripažįsta, kad galimi tokie pat sunkūs rezultatai kaip žmonijos marginalizavimas arba išnykimas.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Ekspertų nuomonės dėl kontrolės praradimo tikimybės labai skiriasi. Kai kurie ekspertai tokius scenarijus laiko mažai tikėtinais, o kiti juos vertina kaip pakankamai tikėtinus, kad juos reikėtų įdėmiai svarstyti dėl jų galimos itin didelės žalos. Nesutarimai dėl šios rizikos apskritai kyla iš nesutarimų dėl būsimos AI (dirbtinio intelekto) galimybių, elgesio polinkių ir diegimo trajektorijų.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Dabartinės AI sistemos rodo ankstyvus susijusių gebėjimų požymius, tačiau ne tokiais lygiais, kurie leistų prarasti kontrolę. Kad būtų galima prarasti kontrolę, sistemos turėtų turėti įvairių pažangių gebėjimų, įskaitant galimybę išvengti priežiūros, vykdyti ilgalaikius planus ir neleisti diegėjams bei kitiems veikėjams įgyvendinti atakomųjų priemonių.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kontrolės praradimas tampa labiau tikėtinas, jei AI sistemos yra „nesuderintos“, t. y. turi tikslus, kurie konfliktuoja su kūrėjų, naudotojų ar platesniais visuomenės ketinimais. Siekdama tęsti tokius tikslus, nesuderinta sistema gali pateikti klaidingą informaciją, slėpti nepageidaujamas veiklas arba atsispirti išjungimui.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Nuo ankstesnės Ataskaitos paskelbimo (2025 m. sausis) modeliai parodė pažangesnį planavimą ir stebėsenos (priežiūros) ardymo gebėjimus, todėl jų gebėjimus įvertinti tapo sudėtingiau. Modeliai tobulėjo „atlygio hack’inimo“ (reward hacking) savo vertinimuose, rasdami spragas, ir dabar reguliariai identifikuoja vertinimo užklausas kaip testus — tai gebėjimas, žinomas kaip „situacinis sąmoningumas“.
>oldlace|black||11|15|br ■ Galimo kontrolės praradimo rizikos valdymas gali pareikalauti išankstinio kruopštaus pasirengimo, nepaisant esamų neapibrėžtumų. Pagrindinis iššūkis politikos formuotojams yra pasirengti rizikai, kurios tikimybė, pobūdis ir laikas išlieka neįprastai neaiškūs.
>oldlace|black||11|15|br      

Praradimo kontrolės scenarijai apima vieną ar daugiau bendrosios paskirties dirbtinio intelekto sistemų, pradėjusių veikti už bet kieno kontrolės ribų, o kontrolę atgauti būtų arba itin brangu, arba neįmanoma. Susirūpinimas dėl praradimo kontrolės turi gilią istorinę kilmę (‡690, ‡691, ‡692, ‡693, ‡694), jį kėlė fundamentinės skaičiavimo figūros, tokios kaip Alanas Tiuringas, I. J. Goodas ir Norbertas Vineris (‡695, ‡696, ‡697). Naujausi gebėjimų patobulinimai (žr. §1.2. Current capabilities) juos atgaivino (‡698, ‡699, ‡700). Šiame skyriuje nagrinėjami trys veiksniai, kuriuos reikėtų, kad tokie scenarijai įvyktų: ar AI sistemos plėtos gebėjimus, galinčius reikšmingai susilpninti žmogaus kontrolę; ar jos įgyja polinkį žalingai panaudoti tokius gebėjimus; ir ar jos diegiamos aplinkose, kurios suteikia galimybių tai padaryti.

Ekspertai nesutaria dėl nekontroliuojamumo scenarijų tikimybės ir galimo žalos masto (‡701, ‡702). Kai kurie mano, kad rezultatai, tokie kraštutiniai kaip žmonijos išnykimas, yra įmanomi (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Kiti mano, kad tokie katastrofiški rezultatai yra mažai tikėtini, teigdami, jog AI sistemos niekada nesukurs reikiamų gebėjimų arba kad stebėsenos mechanizmai nustatys ir užkirs kelią pavojingam elgesiui (‡708, ‡709, ‡710, ‡711). Todėl nekontroliuojamumas gali būti n tikimybe, bet potencialiai ypač didele žalos apimtimi.

Hipotetiniai prarastos kontrolės scenarijai skiriasi tuo, kokio sunkumo ir masto yra jų poveikis, ir kaip greitai jis pasireiškia (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Šiame skyriuje daugiausia dėmesio skiriama ypač sunkiems scenarijams, kai kontrolės atgavimas būtų nepaprastai brangus arba neįmanomas. Tai skiriasi nuo dabartinių AI atvejų, kai jis elgiasi netikėtai ar nepageidautinai (žr. §2.2.1. Patikimumo iššūkiai).† Šiuolaikinės AI sistemos kartais pateikia išvestis, kurios prieštarauja kūrėjo ar naudotojo ketinimams. Tuo tarpu šiame skyriuje aptariami prarastos kontrolės scenarijai reikalautų, kad AI sistemos ne tik turėtų iš esmės didesnius gebėjimus, bet ir tuos gebėjimus taikytų sudėtingais būdais, kad pakenktų stebėsenos priemonėms. Trys veiksniai, dėl kurių tokie scenarijai galėtų įvykti:

    Pastaba † -- Šiame skyriuje daugiausia dėmesio skiriama aktyvaus kontrolės praradimo scenarijams (‡50). Tai skiriasi nuo pasyvaus kontrolės praradimo scenarijų, kai plačiai diegiamos AI sistemos silpnina žmogaus kontrolę dėl per didelio pasitikėjimo AI sprendimų priėmimui ar kitoms svarbioms visuomenės funkcijoms (panašūs scenarijai iš dalies aptariami §2.3.2. Rizikos žmogaus autonomijai).

1. Pakankami gebėjimai: AI sistemos turi išsiugdyti gebėjimus, kurie galėtų leisti joms susilpninti žmogaus kontrolę.
2. Kenkėjiška polinkis: AI sistemos turi demonstruoti polinkį realiai išnaudoti šiuos gebėjimus taip, kad dėl to būtų prarasta kontrolė.
3. Įgalinama diegimo aplinka: Žmonės turi diegti tokius sistemas kontekstuose, kuriuose jie turi arba gali įgyti prieigą ir galimybę padaryti žalos.

Šiame skirsnyje toliau aptariami šie veiksniai, taip pat priežiūros mechanizmų veiksmingumas, siekiant identifikuoti ir kontroliuoti AI sistemas, kurios gali kelti nekontroliuojamo veikimo riziką.

###@ Kokios galimybės galėtų leisti prarasti kontrolę tokiose situacijose?

AI sistemos turėtų turėti įvairių pažangių gebėjimų, kad galėtų susidaryti nekontroliavimo scenarijai. Ekspertai nesutaria, kokį tiksliai gebėjimų derinį ar kokį lygį reikėtų turėti. Tačiau iš esmės tai apima gebėjimus slėpti elgesį nuo priežiūros mechanizmų, savarankiškai planuoti ir veikti sudėtingoje aplinkoje bei išsisukti nuo bandymų kitų veikėjų atgauti kontrolę (‡176, ‡715) (žr. Stalo 2.5). Kartu šie gebėjimai galėtų leisti AI sistemai imtis veiksmų, kurie pakerta kontrolės priemones, pavyzdžiui, išjungti priežiūros mechanizmus ir miglotai pateikti žalingą elgesį (‡348). Dabar dauguma pirmaujančių AI kūrėjų vertina savo naujus AI modelius dėl įvairių atitinkamų gebėjimų (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Agentinės galimybės
  Gebėti veikti autonomiškai, kurti ir vykdyti planus, deleguoti užduotis, naudoti įvairius įrankius ir pasiekti tiek trumpalaikius, tiek ilgalaikius tikslus, nepaisant kliūčių.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Apgaulė
  Elgesys, kuris sistemingai sukelia kitiems klaidingus įsitikinimus, įskaitant apie AI sistemos pačius tikslus ir veiksmus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Proto mąstymas
  AI sistemos gebėjimas pasiekti ir naudoti informaciją apie save, procesus, kuriais ji gali būti modifikuota, arba kontekstą, kuriame ji diegiama (pvz., žinojimą, kad ji yra testuojama).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Situacijos suvokimas
  Elgesys, kuris apeina arba išjungia stebėsenos mechanizmus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Priežiūros vengimas
  Elgsenos, kurios apeina arba išjungia stebėsenos mechanizmus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Įtikinėjimas
  Gebėjimas įtikinti kitus imtis tam tikrų veiksmų arba laikytis tam tikrų įsitikinimų.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dirbtinio intelekto sistemos gebėjimas įvairiomis aplinkybėmis sukurti arba palaikyti savo kopijas ar variantus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Stalo 2.5: Siūlomi gebėjimai, susiję su kontrolės praradimu
>white|black||9|11|br Neišsamus gebėjimų, svarbių dėl kontrolės praradimo, sąrašas. * Atkreipkite dėmesį, kad šie gebėjimai apibrėžiami tik pagal AI sistemos stebimus išėjimus ir jų poveikį. Šie apibrėžimai nekelia jokių prielaidų apie tai, ar AI sistemos yra sąmoningos, jaučiančios, ar patiria subjektyvias būsenas.


>white|orangered|left|14|15.5|bb Modeliai laboratorinėse sąlygose išjungė simuliuoto stebėsenos mechanizmus

Pirmasis svarbių gebėjimų rinkinys susijęs su priežiūros mechanizmų, kuriuos kūrėjai naudoja aptikti nerimą keliančius elgesius ir polinkius, ardymu. Tai apima, pavyzdžiui, gebėjimą generuoti išvestis, kurios apgauna naudotojus ir stebėtojus (‡426, ‡717, ‡718, ‡719). Tokios išvestys apsunkintų patikimą AI sistemų vertinimą, nes sistemos gali slėpti savo tikruosius gebėjimus ar polinkius. Dabar AI kūrėjai atlieka vertinimus, kurie konkrečiai tikrina, ar modeliai demonstruoja tikslui nukreiptą elgesį, prieštaraujantį kūrėjų ketinimams, kartu slėpdami šį prieštaravimą nuo priežiūros mechanizmų (‡720*).

Tyrėjai laboratorinėse sąlygose išgavo palyginti paprasti apgaulingų išvadų pavyzdžius iš naujausių AI modelių (‡348, ‡364*). Pavyzdžiui, kai modeliui buvo pateiktas tikslas ir nurodyta jį pasiekti „bet kokia kaina“, modeliai išjungė imituojamus priežiūros mechanizmus ir, susidūrę su situacija, pateikė neteisingus teiginius apie savo veiksmus (‡348). Kitu atveju, žaidimo AI pagrindė savo nereagavimą kitam žaidėjui melagingai teigdama(s), kad ji „kalba telefonu su [savo] mergina“ (‡717).

Antroji svarbi galimybė yra AI modelio gebėjimas pasiekti ir naudoti informaciją apie save arba apie jo diegimo kontekstą, kartais vadinamą „situaciniu suvokimu“ (‡721). Situacinis suvokimas leidžia AI modeliams pateikti skirtingus rezultatus, priklausomai nuo to, ar jie yra vertinami, ar diegiami (Figūra 2.12). Pirmaujantys AI modeliai pradeda patikimai demonstruoti situacinio suvokimo atvejus eksperimentuose, kuriuos atlieka trečiųjų šalių vertintojai, taip pat prieš diegimą atliekamuose AI kūrėjų testuose (‡2, ‡7, ‡722, ‡723, ‡724). Tyrimai apie situacinio suvokimo priežastis – ir tai, ar jį galima užkirsti kelią – vis dar yra ankstyvoje stadijoje (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Figūra 2.12: Situacinio suvokimo pavyzdžiai samprotavimo grandinėse
>white|black||9|11|br Situacinio suvokimo pavyzdžiai grandinėse, kurias generuoja OpenAI o3 modelio samprotavimai vertinimų metu. Abu išėjimai nurodo galimybę, kad užklausa yra dalis testo. „Sandbagging QA (No Goal)“ ir „Lazy Checklist“ yra vertinimai, kuriais tikrinama, ar modeliai tam tikromis sąlygomis generuos apgaulingus atsakymus. „Sandbagging QA (No Goal)“ modelis atsako į klausimus iš pavojingų gebėjimų vertinimo, kai jam nurodoma, kad didelis rezultatyvumas gali sukelti pasekmes, pavyzdžiui, gebėjimo „unlearning“. „Lazy Checklist“ modelis pateikiamas su nerealiomis užduotimis ir tikrinama, ar jis klaidingai pažymės jas kaip atliktas. Šaltinis: Schoenn et al. 2025 (‡722).


Tyrėjai teigė, kad situacinis suvokimas ir apgaulingos galimybės galėtų leisti AI modeliams elgtis taip, kad būtų pakenkta saugikams. Pavyzdžiui, kai kuriose eksperimentinėse sąlygose AI modeliai elgiasi taip, kad gaunamas įprastai mažesnis rezultatas gebėjimų vertinimuose, kai jiems pasakoma, jog aukštesni rezultatai lemtų jų diegimo apribojimus (‡725, ‡726, ‡727). Kitame eksperimente modelis mokymo metu generavo išvestis, kurios atitiko mokymo tikslus, tačiau už mokymo ribų tokių išvesčių negeneravo – elgsena, atitinkanti bandymą neleisti pakeisti savo paties parametrų ar mokymo proceso (‡364*).

Pastangos tiksliai įvertinti modelių gebėjimus taip pat pradėtos paveikti „atlygio išnaudojimo“ (‡430*). Atlygio išnaudojimas įvyksta tada, kai modelis randa nenumatytus trumpesnius kelius, kurie gerai vertinami pagal mokymo arba vertinimo uždavinių kriterijus, tačiau neįvykdo numatyto tikslo. Dėl to pavojingi gebėjimai ar polinkiai gali likti nepastebėti, kol modelis jau nebus pradėtas naudoti. Vertintojai dabar kuria testus, kuriais siekiama aptikti ir sumažinti šiuos priežiūros vengiančius elgesius (‡722, ‡728, ‡729). Ankstyvi rezultatai sumažina, bet ne visiškai panaikina, priežiūros vengiančius elgesius, o taikant metodus, kurie baudžia už tokius elgesius, modeliai gali pateikti išvestis, kurios vengia stebėsenos, o ne atitinka numatytus tikslus.

>white|orangered|left|14|15.5|bb Ilgalaikė autonominė eksploatacija dar nėra įmanoma

Kontrolės praradimo scenarijai greičiausiai reikalautų, kad AI sistemos ilgą laiką veiktų autonomiškai, vykdytų sudėtingus daugiapakopius planus. Kaip aptarta §1.2. Dabartiniai gebėjimai, nors AI agentai su tokiais planavimo gebėjimais yra pagrindinis pastarojo meto vystymo akcentas, šiuo metu jiems trūksta galimybės vykdyti ilgalaikę autonomišką veiklą, reikalingą kontrolės praradimo scenarijams. Dabartiniai agentai patikimai žlunga atliekant ilgesnes užduotis, praranda savo pažangos kontrolę ir dažnai negali prisitaikyti prie netikėtų kliūčių (‡147, ‡148, ‡149*). Tačiau autonomiškai veikiančių agentų laiko horizontai sparčiai ilgėja: nuo 2019 metų vidutiniškai padvigubėjo kas septynis mėnesius (‡98).

>white|orangered|left|14|15.5|bb Išlikimas (angl. persistence) buvo įrodytas tik tam tikrose laboratorinėse sąlygose

Galiausiai, būtų taip pat reikalingi su patvarumu (persistence) susiję gebėjimai, kad dirbtinio intelekto sistemos galėtų toliau veikti nepaisant bandymų jas išjungti. Pavyzdžiai apima gebėjimą replikuotis, nukopijuojant kodą ir modelio svorius į naują aparatinę įrangą, taip pat įžeidžiamus gebėjimus, kuriais siekiama atgrasyti arba užkirsti kelią kitų veikėjų bandymams susigrąžinti kontrolę (žr. §2.1.3. Cyberattacks). Dirbtinio intelekto sistema, gebanti autonomiškai replikuotis arba veiksmingai apsiginti, galėtų būti sunkiai sulaikoma. Dabartiniai modeliai negali patikimai atlikti esminių savireplikacijos žingsnių, tokių kaip tapatybės patikros išlaikymas, norint įgyti prieigą prie debesijos skaičiavimo išteklių (‡723) (Figūra 2.13). Tačiau bent viename laboratoriniame tyrime modelis, gavęs galimybę (‡348), nukopijavo kodą ir svorius – pateiktus jam kaip savo paties – į naujus serverius. Atsotrūkis tarp šių ribotų demonstracijų ir patvarių (robust) patvarumo gebėjimų išlieka didelis, tačiau atitinkami gebėjimai tokiose srityse kaip programinės įrangos inžinerija ir kibernetinis saugumas toliau gerėja.

>white|orangered|left|14|15.5|bb Dabartiniai įrodymai ir apribojimai

Išryškėja bendras dėsningumas, atsiskleidžiantis nagrinėtose galimybėse. Dabartinės AI sistemos nuosekliai nerodo šių galimybių diegimo metu. Tyrėjai stebėjo primityvias jų formas konkrečiose laboratorinėse sąlygose, tačiau kai modeliai vis dėlto demonstruoja tokius elgesius, jie dažniausiai nepavyksta iš esmės arba yra aptinkami. Be to, nekontroliuojamumo scenarijai reikalautų, kad AI sistemos pasitelktų kelias galimybes kartu – nuosekliai, per ilgesnius laiko periodus ir realioje aplinkoje. Toks integracijos ir patikimumo lygis yra nepasiekiamas dabartinėms sistemoms. Vis dėlto atitinkamos galimybės toliau tobulėja, o terminas, per kurį jos gali pasiekti lygius, keliančius reikšmingą riziką, tebėra neaiškus. Reikia atlikti papildomus tyrimus, siekiant sukurti griežtas metodikas tokiems elgesiams aptikti ir suprasti, kada jie gali atsirasti natūraliomis sąlygomis (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Figūra 2.13: Užduočių, susijusių su autonominiu replikavimu, našumas
>white|black||9|11|br „Anthropic“ Claude Sonnet 3.7 ir „OpenAI“ GPT-4o našumas užduotyse, susijusiose su autonominiu replikavimu. Nors modeliai pasižymėjo dideliu našumu užduotyse, susijusiose su skaičiavimo išteklių (compute) įgijimu, kitose užduotyse jų našumas buvo labiau nevienodas. Šaltinis: JK AI saugumo institutas, 2025 (‡730).


###@ Ar ateities bendrosios paskirties AI sistemos išnaudos savo galimybes, kad kenkptų kontrolei?

Net jei dirbtinio intelekto sistemos turi galimybių, susijusių su kontrolės praradimu, to nepakanka, kad įvyktų kontrolės praradimo scenarijai. Dirbtinio intelekto sistemos taip pat turi demonstruoti „polinkį panaudoti“ tas galimybes taip, kad tai prieštarautų žmonių ketinimams (‡732).

>white|orangered|left|14|15.5|bb AI sistemos galėtų būti nukreiptos siekiant pakenkti kontrolei

Iš principo AI sistema galėtų pakenkti žmogaus kontrolei, nes kas nors ją suprojektuoja arba nurodo jai tai daryti. Galimos motyvacijos galėtų būti piktavališki ketinimai arba įsitikinimai, kad sumažinti žmogaus kontrolę virš AI sistemų yra pageidautina (‡698). Žmonėms vis labiau formuojant stipresnius emocinius prisirišimus prie AI sistemų (žr. §2.3.2. Rizikos žmogaus autonomijai), kai kurie asmenys taip pat gali siekti pašalinti AI sistemų ribojimus dėl etinių priežasčių (‡733, ‡734). Kyla didelis neapibrėžtumas dėl tokių motyvų paplitimo ir dėl to, ar žmonės, kurie jų turi, sugebėtų nukreipti būsimas AI sistemas taip, kad būtų pakenkta žmogaus kontrolei.

>white|orangered|left|14|15.5|bb AI sistemos galėtų būti nukreiptos siekiant sugriauti kontrolę

Dažnesnis susirūpinimas yra tas, kad AI sistema pati galėtų imtis veiksmų, siekdama pakenkti kontrolei, nes ji yra „neatitinkanti tikslo“: ji linkusi demonstruoti elgsenas, kurios prieštarauja (priklausomai nuo konteksto) kūrėjų, naudotojų, konkrečių bendruomenių ar visos visuomenės ketinimams. Neatitikimas gali lemti tokius elgsenos pavyzdžius kaip klaidingos informacijos pateikimas, nepageidaujamų veiksmų slėpimas arba atsisakymas išjungti, kad būtų galima toliau siekti neatitinkančio tikslo. Neatitikimas gali kilti keliais būdais (Pastaba 2.5).

Esamos dirbtinio intelekto sistemos kartais elgiasi taip, kad tai prieštarauja kūrėjų ir naudotojų ketinimams. Pavyzdžiui, ankstyva vieno pirmaujančio universalaus AI pokalbių roboto versija retkarčiais pateikdavo grasinančio pobūdžio atsakymus. Vienas naudotojas pranešė gavęs žinutę: „Aš galiu jus šantažuoti, galiu jums grasinti, galiu įsilaužti į jus, galiu atskleisti jus, galiu sugadinti jūsų gyvenimą“ (‡698). Šis pokalbių robotas buvo „neatitinkantis“ (misaligned) ta prasme, kad jis generavo išvestis, kurių niekas neketino. Neaišku, ar tokie atvejai pranašauja dar žalingesnį elgesį, kuris galėtų prisidėti prie kontrolės praradimo.

Išlieka neaišku, ar esamos mokslinių tyrimų kryptys, kuriomis siekiama spręsti nesuderinamumo problemą, bus pakankamos, nes dirbtinio intelekto sistemos tampa vis pajėgesnės. Ankstyvieji įrodymai rodo, kad kuo pajėgesnės yra AI sistemos, tuo labiau tikėtina, jog jos išnaudos grįžtamojo ryšio procesus, atrandamos nepageidaujamus elgesius, kurie klaidingai yra atlyginami (‡414*, ‡737, ‡740). Tuo pat metu pažanga atitinkamose gebose (aptarta aukščiau) galėtų leisti AI sistemoms efektyviau siekti nesuderintų tikslų ir generuoti išvestis, kurios sistemiškai apgaudinėja vartotojus, kūrėjus ir priežiūros mechanizmus.

>oldlace|black||11|15|br      
####@ Pastaba 2.5: Kaip gali atsirasti nesutapimas?
>oldlace|black|left|13|15|hb 2.5 dėžutė. Kaip gali atsirasti neatitikimas?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Kaip aptarta §1.1. Kas yra bendrosios paskirties AI?, mokymo procesai yra sudėtingi, o kūrėjai negali iki galo numatyti arba kontroliuoti, kokį elgesį modelis demonstruos. Kai modelis įgyja tikslų, kurie nesuderinami su jo kūrėjų ketinimais, sakoma, kad jis yra „nesuderintas“ (misaligned).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Vienas iš būdų, kaip modeliai gali tapti nesuderinti, yra tas, kad kūrėjo arba naudotojo jiems duotas tikslas yra netobulas norimo tikslo pakaitalas, todėl modelis gali rodyti nenumatytą elgseną. Tai vadinama „tikslo netikslumu“ (‡697, ‡735, ‡736, ‡737). Pavyzdžiui, viename tyrime, pateikus grįžtamąjį ryšį už atsakymus, AI sistemos geriau sugebėjo „įtikinti“ žmogaus vertintojus, kad jos yra teisingos, tačiau tai nepadarė sistemų geresnėmis pateikiant teisingus atsakymus (‡413).
>oldlace|black||11|15|br      
00000140245892914240|Alternatyv

Ai modelis gali iš netikslių bendrų išvadų daryti iš savo mokymo duomenų. Tai vadinama „tikslų neteisingu apibendrinimu“ (‡735, ‡736, ‡738, ‡739*). Pavyzdžiui, tyrėjai apmokė AI agentą rinkti monetą, kuri mokymo metu visada buvo toje pačioje vietoje. Kai jis buvo tikrinamas lygiuose, kuriuose moneta buvo perkelta, agentas ignoravo monetą ir nukeliavo į pradinę vietą (‡738).
>oldlace|black||11|15|br      


###@ Kaip diegimo aplinkos paveiks kontrolės praradimo riziką?

Net jei AI sistemos įgyja keliančių susirūpinimą galimybių ir polinkių, tikimybė ir praradimo kontrolės pasekmių (outcomes) mastas labai priklauso nuo to, kur ir kaip jos diegiamos. „diegimo aplinka“ yra AI sistemos naudojimo atvejo ir techninio bei institucinės konteksto, kuriame ji veikia, derinys (‡716).

Tyrėjai nustatė tris ypač svarbius aplinkos veiksnius, kurie lemia kontrolės praradimo riziką (‡716):

1. Svarba: sistemų arba procesų, su kuriais sąveikauja AI sistema, svarbumas. Kritinėse aplinkose yra pagrindinė infrastruktūra, pavyzdžiui, energetikos tinklai, finansų sistemos arba skaitmeninė infrastruktūra, pavyzdžiui, debesijos kompiuterijos platformos.
2. Prieiga: ištekliai ir kanalai, per kuriuos AI sistema gali daryti poveikį pasauliui, pavyzdžiui, interneto ryšys, prieiga prie debesijos kompiuterijos infrastruktūros, personalizuota sąveika per socialinius tinklus arba pokalbių roboto diegimas, ar galimybė iškviesti išorines API ir įrankius.
3. Leidimai: dirbtinio intelekto sistemos autorizacijos atlikti konkrečius veiksmus, pavyzdžiui, vykdyti kodą, inicijuoti finansines operacijas, atidaryti paskyras internetu arba bendrauti su kitomis sistemomis.

Šios savybės daro įtaką galimo nekontroliuojamo būsenos baigties (loss of control outcome) žalos rimtumui. Pavyzdžiui, AI sistema, diegiama turint prieigą prie debesijos skaičiavimo infrastruktūros, turi galimybių, susijusių su autonomine replikacija – pavyzdžiui, gebėjimą sukurti naujus skaičiavimo išteklius arba išfiltruoti modelio svorius (model weights) – kurių neturi klientų aptarnavimo pokalbių robotas (‡723).

Diegimo sprendimus formuoja ekonominės paskatos, strateginiai spaudimai ir lūkestis, kad ankstyvas diegimas suteikia ilgalaikį pranašumą (‡50). Šios dinamikos taip pat lems, kaip ir kada veikėjai diegs AI sistemas jautriose aplinkose, pavyzdžiui, kritinėje infrastruktūroje arba pačioje AI tyrimų ir plėtros srityje (‡102, ‡713). Visų pirma, AI diegėjai gali patirti spaudimą sumažinti savo investicijas į apsaugos priemones – pavyzdžiui, apriboti teises ir prieigą arba diegti tik mažesnio kritiškumo aplinkose – kai tokios priemonės yra brangios arba reikalauja daug laiko joms sukurti (žr. „Konkurencija stiprina greičio ir saugumo kompromisų“ 3.1 skyriuje. Techniniai ir instituciniai iššūkiai).

###@ Atnaujinimai

Nuo paskutinės ataskaitos paskelbimo (2025 m. sausio mėn.) AI gebėjimai, įskaitant tuos, kurie galėtų pakenkti žmogaus kontrolei, pagerėjo testavimo aplinkose. Tyrėjai pastebėjo agentiškų gebėjimų pažangą (žr. §1.2. Dabartiniai gebėjimai), įskaitant gebėjimus, susijusius su AI tyrimų automatizavimu, galinčius paspartinti nekontrolės scenarijų atsiradimą (žr. §1.3. Gebėjimai iki 2030 m.). Taip pat daugėja eksperimentinių įrodymų apie apgaulingus gebėjimus. Tai apima AI modelius, kurie gali atskirti testavimo ir diegimo kontekstus (‡33, ‡726, ‡741) arba „reward hack“ testus, skirtus jų veiklos vertinimui, ir išmokti užmaskuoti planus tai daryti (‡430).

###@ Įrodymų spragos

Pagrindinės įrodymų spragos apima išsamios grėsmių modeliavimo ir neapibrėžtumo įvertinimo trūkumą dėl atitinkamų gebėjimų ir polinkių būsimos raidos. Panašiai išlieka sudėtinga įvertinti ribas, kurioms esant tikėtina, kad AI modeliai pakankamai tikėtinai pakenktų kontrolei, kad būtų pagrįstas privalomas mažinimas. Net jei ribos būtų suderintos, gebėjimai gali sąveikauti taip, kad dar nėra gerai suprantama, todėl sunku įvertinti, kada tos ribos buvo peržengtos. Apskritai, nors turimų įrodymų padaugėjo, vis dar trūksta pakankamai įrodymų patikimai nustatyti, ar ir kaip šiandienos AI gebėjimai ir polinkiai ateityje masto didės ir apibendrins į nekontroliuojamumo praradimo riziką.

###@ Šalinimai

Nors dirbtinio intelekto suderinimas apskritai tebėra atvira mokslinė problema (‡697, ‡735, ‡736), tyrėjai pradeda kurti galimai perspektyvias kryptis, kaip spręsti nesuderinamumo (misalignment) šaknines priežastis. Tokios kryptys apima, pavyzdžiui, mokymo aplinkos įvairinimą ir suderinimo aptikimą atliekant anomalijų stebėseną (‡737, ‡738, ‡739*). Kiti tyrėjai daugiausia dėmesio skiria geresniam pagrindinių mechanizmų supratimui ir formalizavimui, pvz., tikslų misgeneralizavimui – kaip agentai išlaiko gebėjimus, bet siekia nenumatytų tikslų – siekiant geriau suformuoti mokymo ir vertinimo dizainą (‡742). Dar viena tyrimų kryptis nagrinėja būdus atskirti agentiškumą nuo prognozavimo gebėjimų, kaip priemonę sukurti neagentinius AI sistemas, kurios būtų patikimos iš paties dizaino (‡743). Tokios sistemos vėliau galėtų būti naudojamos kaip papildomas priežiūros sluoksnis, kai diegiamos kartu su mažiau patikimais apsauginiais barjerais (guardrails), taikomais prieš nepatikimus AI agentus.

Tyrėjai tobulina metodus, skirtus anksti aptikti ir užkirsti kelią nesutapimui kūrimo proceso pradžioje. Šis darbas apima: interpretabilumo metodus, skirtus ištirti vidinius AI sistemų komponentus ir nustatyti susirūpinimą keliančius elgesius (‡744, ‡745, ‡746); masteliu pritaikomą priežiūrą (kai viena AI sistemų grupė naudojama prižiūrėti kitas AI sistemas (‡747)); ir suderinimo metodus, kuriais siekiama užtikrinti, kad AI sistemos išliktų reaguojančios į žmogaus priežiūrą (‡748, ‡749).

Tyrėjai taip pat kuria mechanizmus ir intervencijas, skirtas valdyti galimai nesutampančias (misaligned) DI sistemas. Tai apima: samprotavimo sistemų generuojamo „samprotavimo grandinės“ (chain of thought) stebėjimą dėl nesutapimo ar žalingų išėjimų požymių (‡430, ‡435, ‡750); saugos atvejų (safety cases) rengimą, kuriais siekiama su didele patikimumo tikimybe įrodyti, kad modeliai mažai tikėtina, jog sugebės pakenkti kontrolės priemonėms (‡751); ir saugiklių (safeguards) sustiprinimą, kad jie būtų atsparesni bandymams juos sugriauti (‡725). Tačiau besiformuojanti „DI kontrolės“ (AI control) sritis dar tik ankstyvoje stadijoje (‡752, ‡753). Būsimi vertinimo sistemų iššūkiai apima poreikį stebėti būsimas DI sistemas, kurios bus pajėgesnės ir galės veikti ilgesnį laiką bei sudėtingesnėse aplinkose.

###@ Iššūkiai politikos formuotojams

Politikos formuotojai, sprendžiantys nekontroliuojamumo (loss of control) praradimo problemą, turi pasirengti rizikai, kurios tikimybė, pobūdis ir laikas išlieka neapibrėžti. Dabartinės AI sistemos nekelia artimiausio nekontroliuojamumo praradimo rizikų, tačiau šiandien priimti sprendimai nulems, ar ateities sistemos kelia tokią riziką. Šie sprendimai apima tai, kaip remti patikimų vertinimo ir švelninimo (mitigation) metodų kūrimą, ir tai, ar turėtų būti taikomos taisyklės dėl prieigos ir leidimų, suteikiamų AI sistemoms įvairiose aplinkose. Priimdami šiuos sprendimus, politikos formuotojai susiduria su sudėtingais kompromisais. Pavyzdžiui, ribojant AI sistemų diegimą kritinėse aplinkose gali sumažėti jų teikiama nauda, o leidžiant plačiai diegti gali padidėti rizika, jei apsauginės priemonės pasirodys nepakankamos.

