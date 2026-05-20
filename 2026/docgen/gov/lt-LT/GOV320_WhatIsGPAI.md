###@ Kas yra bendrosios paskirties dirbtinio intelekto sistemos?

Bendrosios paskirties dirbtinio intelekto sistemos yra programinės įrangos programos, kurios išmoksta dėsningumų iš didelių duomenų kiekių, leisdamos joms atlikti įvairias užduotis, o ne būti pritaikytoms vienai konkrečiai funkcijai ar sričiai (žr. Stalo 1.1). Kurdamiesi šias sistemas, dirbtinio intelekto kūrėjai įgyvendina kelių etapų procesą, kuriam reikia reikšmingų skaičiavimo išteklių, didelių duomenų rinkinių ir specializuotos kompetencijos (žr. Stalo 1.2). Skaičiavimo ištekliai (dažnai trumpinami kaip „compute“) reikalingi ir dirbtinio intelekto sistemoms kurti, ir jas diegti, ir apima specializuotus kompiuterio lustus, taip pat programinę įrangą ir infrastruktūrą, reikalingą joms paleisti.† Kadangi jos yra mokomos naudojant didelius, įvairius duomenų rinkinius, bendrosios paskirties dirbtinio intelekto sistemos gali atlikti daug skirtingų užduočių, pavyzdžiui, apibendrinti tekstą, generuoti vaizdus arba rašyti kompiuterinį kodą. Šiame skyriuje paaiškinama, kaip kuriamos bendrosios paskirties dirbtinio intelekto sistemos, kas yra „samprotavimo“ modeliai ir kaip politikos sprendimai veikia bendrosios paskirties dirbtinio intelekto sistemos kūrimą.

    Pastaba † -- Terminas „compute“ taip pat gali reikšti ir matavimą, kiek skaičiavimų gali atlikti procesorius (paprastai matuojama slankaus kablelio operacijomis per sekundę), ir konkrečiai tą aparatūrą (pvz., grafikos procesorius), kuri atlieka tuos skaičiavimus.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Kalbos sistemos
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Komanda A (‡3*)
- EXAONE 4.0 (‡4*)
- Gemini 3 Pro (‡5*)
- GLM-4.5 (‡6*)
- GPT-5(‡7*)
- Hunyuan-Large (‡8*)
- Kimi K2 (‡9*)
- Mistral 3.1 (‡10*)
- Qwen3 (‡11*)
- DeepSeek-V3.2 (‡12*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Vaizdo generatoriai
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Vaizdo generatoriai
- Kosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Skraistė (‡19)
- Mačiau 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotikos ir navigacijos sistemos
- „Gemini Robotics (‡21*)“
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Daugias formų biomolekulinių struktūrų prognozės pagal įvairias klases
- AlphaFold 3 (‡27)
- Padidinti (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ AI agentai
- AlphaEvolve (‡31*)
- „ChatGPT“ agentas (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- AI mokslininkas-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Stalo 1.1: Bendros paskirties AI tipai
>white|black||9|11|br Yra keli skirtingi bendrosios paskirties AI tipai. Šiame pranešime modeliai, galintys prognozuoti struktūrinę informaciją įvairioms molekulių klasėms, laikomi „bendrosios paskirties“ AI, nes juos galima pritaikyti įvairiems uždaviniams. Pavyzdžiui, modeliai, apmokyti prognozuoti baltymų struktūrą, yra taikomi įvairiems kitiems uždaviniams, tokiems kaip baltymų sąveikų prognozavimas, mažų molekulių jungimosi vietų prognozavimas ir ciklinių peptidų (‡40) prognozavimas bei projektavimas.


>white|orangered|left|13|15|bb Gilus mokymasis yra pamatinis bendros paskirties dirbtinio intelekto pagrindas

Tyrėjai kuria bendrosios paskirties AI modelius taikydami procesą, vadinamą „giluminiu mokymusi“, kuris moko modelius mokytis iš pavyzdžių (‡41). Skirtingai nuo programinės įrangos inžinerijos, giluminiu mokymusi pagrįsti modeliai užduotis išmoksta atlikti iš duomenų, o ne remtis ranka parašytomis instrukcijomis. Apdorodami didelius duomenų kiekius, pavyzdžiui, vaizdus, tekstą ar garsą, šie modeliai atranda būdus, kaip tuos duomenis pavaizduoti, taip sukurdami vidines atpažįstamų dėsningumų reprezentacijas (tokias kaip formos, žodžių sąsajos arba garso struktūros), kurios padeda modeliui atpažinti ryšius ir generuoti išvestis, suderintas su jo mokymo tikslu. Tuomet jie šias išmoktąsias vidines reprezentacijas naudoja kaip abstrakčius požymius, kad analizuotų naujus, panašius duomenis ir generuotų išvestis tuo pačiu stiliumi. Pavyzdžiui, bendrosios paskirties AI modelis, apmokytas pakankamai daug pavyzdžių iš 19 a. romantinės anglų poezijos, gali atpažinti naujus tokio stiliaus eilėraščius ir sukurti naują medžiagą panašiu stiliumi.

Savo smulkesniu lygmeniu gilusis mokymasis veikia apdorodamas duomenis per sluoksnius tarpusavyje susietų informacijos apdorojimo mazgų. Šie mazgai dažnai vadinami „neuronais“, nes yra tik laisvai įkvėpti neuronų biologinėse smegenyse („neural networks“) (Figūra 1.1) (‡42). Kai informacija teka iš vieno neuronų sluoksnio į kitą, modelis palaipsniui transformuoja duomenis į vis abstraktesnes reprezentacijas kaip išmoktų požymių grupes – modelio automatiškai duomenyse atrastus šablonus, o ne rankiniu būdu užkoduotus. Pavyzdžiui, vaizdų apdorojimo modelyje pirmieji sluoksniai gali išmokti aptikti paprastus požymius, tokius kaip briaunos ar bazines formas, o gilesni sluoksniai sujungia šiuos požymius, kad išskirtų sudėtingesnius šablonus, tokius kaip veidai ar objektai.

Visuose sluoksniuose esančios ypatybės išaiškinamos optimizavimo proceso metu, kuris apibrėžia mokymo procedūrą. Mokymo metu, kai modelis klysta, giluminio mokymosi algoritmai koreguoja įvairių jungčių tarp neuronų stiprumą, kad pagerintų modelio veikimą. Kiekvienos jungties tarp mazgų stiprumas dažnai vadinamas „svoriu“. Šis sluoksninis metodas ir suteikia giluminiam mokymuisi jo pavadinimą.

Deep learning įrodė esąs labai veiksmingas leidžiant AI sistemoms atlikti užduotis, kurios anksčiau buvo laikomos sudėtingomis tradicinėms rankomis programuojamoms skaičiavimo sistemoms ir kitoms ankstesnėms simbolinėms ar taisyklėmis grįstoms AI metodikoms. Dauguma dabartinių pažangiausių bendrosios paskirties AI modelių dabar remiasi konkrečia neuroninio tinklo architektūra, vadinama „transformer“ (‡43, ‡44). Transformeriai naudoja „attention“ mechanizmą (‡45), kuris padeda modeliui apdorojant informaciją sutelkti dėmesį į labiausiai svarbias įvesties duomenų dalis, pavyzdžiui, nustatant, kurios žodžiai sakinyje yra svarbiausi norint suprasti jo reikšmę. Toks modelių kūrimo būdas lėmė reikšmingus vertimo (‡43), natūralios kalbos apdorojimo (‡46), vaizdų atpažinimo (‡47) ir kalbos atpažinimo (‡48, ‡49) patobulinimus, galiausiai atvedusius prie šiandienos pažangiausių modelių kūrimo.

![fig1.1](images/fig1.1_neural_network.png)

##### Figūra 1.1: Iliustracinis „neuroninio tinklo“ atvaizdavimas
>white|black||9|11|br Šiandienos bendrosios paskirties AI modeliai yra pagrįsti šiais tinklais, kurie tik laisvai įkvėpti biologinių smegenų. Skirtingi tinklai turi skirtingus dydžius ir architektūras. Tačiau visi jie sudaryti iš sujungtų informacijos apdorojimo vienetų, vadinamų „neuronais“, o ryšių tarp neuronų stiprumai vadinami „svoriais“. Svoriai yra atnaujinami mokymo metu naudojant didelius duomenų kiekius. Šaltinis: Tarptautinė AI saugos ataskaita 2025 (‡50) (pakeista).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Figūra 1.2: Scheminis bendrosios paskirties dirbtinio intelekto kūrimo etapų vaizdavimas
>white|black|left|9|11|br Tarptautinė AI saugos ataskaita 2026.


>white|orangered|left|13|15|bb Bendrosios paskirties dirbtinis intelektas yra kuriamas etapais

Bendros paskirties AI sistemos kūrimas apima kelis etapus - nuo pradinio modelio mokymo iki stebėsenos po įdiegimo ir atnaujinimų (Figūra 1.2). Praktikoje šie veiksmai dažnai persidengia iteraciniu būdu. Kiekvienam etapui reikia skirtingų išteklių (pvz., duomenų, darbo jėgos, skaičiavimo pajėgumų) ir skirtingų metodų, o kartais juos atlieka skirtingi kūrėjai (Figūra 1.2 ir Stalo 1.2).

Pavyzdžiui, modelio išankstinis mokymas paprastai reikalauja didelių skaičiavimo ir duomenų kiekių, todėl šis etapas ypač jautrus politikoms, kurios daro įtaką prieigai prie skaičiavimo išteklių ar mokymo duomenų (‡51, ‡52). Panašiai duomenų atranka ir kai kurie modelio tikslaus pritaikymo metodai šiuo metu susiję su dideliais žmogiško darbo kiekiais pradiniam duomenų žymėjimui (‡53). Todėl šis etapas yra jautrus darbo sąnaudų, platformų politikų arba taisyklių, turinčių įtakos tarpvalstybinėms rangos sutarčių sudarymo schemoms, pokyčiams.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Duomenų rinkimas ir parengimas
> 
  Prieš mokant bendrosios paskirties dirbtinio intelekto modelį, kūrėjai ir duomenų specialistai surenka, išvalo, atrenka ir standartizuoja žalius mokymo duomenis į tokį formatą, iš kurio modelis gali mokytis. Tai gali būti daug darbo reikalaujantis procesas. Mokymo duomenų rinkiniai, esantys pažangiausių modelių pagrinde, apima milžinišką skaičių pavyzdžių iš viso interneto.
  Komandos dažnai kuria pažangius filtravimo metodus, kad sumažintų žalingą turinį, pašalintų pasikartojančius duomenis ir pagerintų reprezentatyvumą tarp skirtingų temų bei šaltinių (‡54, ‡55). Duomenų tvarkymas (angl. data curation) taip pat gali padėti sumažinti autorių teisių ir privatumo pažeidimus, pašalinti pavyzdžius, kuriuose yra pavojingų žinių, tvarkyti kelias kalbas ir pagerinti dokumentaciją apie duomenų kilmę (angl. data provenance) (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Išankstinis mokymas (pirmasis mokymo etapas)

  Per išankstinį mokymą kūrėjai modeliams pateikia milžiniškus įvairių duomenų kiekius, kad įdiegtų platų informacijos pagrindą ir kontekstinį supratimą. Šis procesas sukuria „bazinį modelį“. Tai labai duomenų ir skaičiavimų išteklių reikalaujantis procesas.

  Per išankstinį mokymą modeliai yra veikiami milijardų ar trilijonų turinio pavyzdžių, tokių kaip paveikslėliai, tekstai ar garsas. Dėl šio poveikio modelis palaipsniui išmoksta abstrakčių savybių, kurios atvaizduoja duomenis, ir išmoksta, kaip šios savybės yra susijusios, todėl jis gali prasmingai interpretuoti naujus įvesties duomenis atsižvelgdamas į kontekstą. Šis išankstinio mokymo procesas trunka savaites ar mėnesius (‡59) ir naudoja dešimtis ar šimtus tūkstančių grafikos procesorių (GPU) arba tenzorių apdorojimo vienetų (TPU) (‡60) – specializuotus kompiuterinius lustus, sukurtus sparčiai atlikti daug tokių skaičiavimų. Kai kurie kūrėjai atlieka išankstinį mokymą naudodami savo skaičiavimo resursus, o kiti – pasitelkia išteklius, kuriuos teikia specializuoti skaičiavimo paslaugų teikėjai.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Po mokymo ir pritaikymas konkrečiai užduočiai (antrasis mokymo etapas)

  „Po mokymo“ dar labiau patikslina bazinį modelį, kad būtų optimizuotas konkrečiai taikymo sričiai. Tai vidutiniškai daug skaičiavimo išteklių reikalaujantis ir labai daug darbo sąnaudų reikalaujantis procesas. Perėjimas prie „sintetinių duomenų“ – dirbtinai sugeneruotos informacijos, kuri imituoja realaus pasaulio duomenis, bet yra kuriama naudojant algoritmus arba simuliacijas – padeda padaryti šį etapą mažiau reikalaujantį darbo sąnaudų.
  Po mokymo atliekamas įvairių smulkinio tikslinimo metodų ir kitų pakeitimų rinkinys. „Prižiūrimas smulkinis tikslinimas“ apima papildomą jau apmokyto modelio mokymą konkrečiais duomenų rinkiniais, siekiant pagerinti modelio veikimą toje srityje (‡61, ‡62). Pavyzdžiui, bendrosios paskirties modelis galėtų būti papildomai apmokytas dideliame radiologinių vaizdų rinkinyje. „Stiprinamasis mokymasis“ (RL) apima modelio veikimo gerinimą „apdovanojant“ modelį (teikiant teigiamą grįžtamąjį ryšį) už pageidaujamus išėjimus ir „baudžiant“ modelį (teikiant neigiamą grįžtamąjį ryšį) už nepageidaujamus išėjimus. Jis turi dvi iškiliąsias subkategorijas. „Stiprinamasis mokymasis iš žmogaus grįžtamojo ryšio“ apima apdovanojimą išėjimų, kurie atitinka žmogaus pageidavimus, ir baudimą tų, kurie jų neatitinka, remiantis žmogaus grįžtamajame ryšiu (‡63, ‡64*). „Stiprinamasis mokymasis su patikrinamais apdovanojimais“ (RLVR) naudojamas modelio veikimui gerinti užduotyse, kurioms reikia faktinio teisingumo, pavyzdžiui, matematikos arba kodo generavimo. Kūrėjai paprastai kaitalioja po-mokymo metodų taikymą ir testų vykdymą, kol rezultatai rodo, kad modelis atitinka pageidaujamas specifikacijas.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Sistemos integracija

  Kūrėjai sujungia vieną ar daugiau bendros paskirties dirbtinio intelekto (DI) modelių su kitais komponentais, kad sukurtų „DI sistemą“, parengtą naudoti. GPT-5 (pavyzdžiui) yra bendros paskirties dirbtinio intelekto modelis, kuris apdoroja tekstą, vaizdus ir garsą, o ChatGPT yra bendros paskirties dirbtinio intelekto sistema, kuri sujungia kelis skirtingo dydžio ir galimybių modelius su pokalbių sąsaja, turinio apdorojimu, prieiga prie Web ir programų integravimu, kad būtų sukurtas veikiantis produktas.
  Be to, kad AI modeliai būtų eksploatuojami, papildomi komponentai AI sistemoje taip pat siekia pagerinti gebėjimus, naudingumą ir saugą. Pavyzdžiui, sistema gali turėti filtrą, kuris aptinka ir blokuoja modelio įvestis ar išvestis, kuriose yra žalingo turinio (‡65*). Kūrėjai taip pat vis dažniau naudoja „atramos“ (scaffolding) – papildomą programinę įrangą, kuri kuriama aplink bendros paskirties AI modelius ir leidžia jiems iš anksto planuoti, siekti tikslų ir sąveikauti su pasauliu (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Diegimas ir paleidimas
  Diegimas yra procesas, kurio metu integruota AI sistema paruošiama numatytam naudojimui. Kūrėjai ir diegėjai diegia AI sistemas į realaus pasaulio taikomąsias programas, produktus arba paslaugas. Kūrėjai gali diegti AI sistemas viduje (savo reikmėms) arba išorėje (privačioms paslaugų užsakovų grupėms arba viešam naudojimui). Diegiant AI sistemas išorėje, įmonės dažnai suteikia naudotojams prieigą per internetines naudotojo sąsajas arba taikomųjų programų sąsajas (API), kurios leidžia naudotojams pasiekti ir paleisti sistemą. Pavyzdžiui, viena įmonė gali sukurti pagal individualų užsakymą pritaikytą klientų aptarnavimo pokalbių robotą, kurį maitina kitos įmonės bendrosios paskirties AI sistema.
  „AI sistemos diegimas“ reiškia modelio parengimą realiam naudojimui su integruotais įrankiais ir sąsajomis, o „modelio išleidimas“ apima bazinio modelio suteikimą kitiems – arba kaip atvirų svorių (atsisiunčiami parametrai), arba kaip uždarų svorių (tik API prieiga). Žr. §3.4. Atvirų svorių modeliai.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Stebėsena po diegimo ir atnaujinimai

  Kūrėjai dažnai renka ir analizuoja naudotojų atsiliepimus, stebi poveikio ir veikimo metrikas bei atlieka iteracinius patobulinimus, kad spręstų realiame naudojime aptiktas problemas (‡67). Patobulinimai atliekami atnaujinant sistemos integracijas, dažnai atliekant nuolatinį pritaikymą (continual fine-tuning) ir suteikiant modeliams prieigą prie išorinių (naujų) faktų duomenų bazių. Tai leidžia dideliems AI modeliams išlikti naujausiems, nebekartojant viso pradinio mokymo proceso (‡68*). Taip sudaromos sąlygos gebėjimams kauptis per nuoseklius mokymo etapus, kartu išlaikant stabilumą ir mažinant skaičiavimo išlaidas.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 1.2 lentelė: Bendrosios paskirties dirbtinio intelekto kūrimo etapai
>white|black||9|11|br Kiekviename bendrosios paskirties AI kūrimo etape AI modelis tobulinamas tolesniam naudojimui ir galiausiai diegiamas kaip visiškai integruota AI sistema, stebima ir atnaujinama.


>white|orangered|left|13|15|bb Samprotavimo sistemos išvadų metu generuoja „minčių grandines“, kad pagerintų veikimą

Išvada įvyksta tada, kai kas nors naudoja AI modelį po to, kai jis buvo apmokytas. Pavyzdžiui, išvada įvyksta, kai žmogus paprašo AI sistemos suplanuoti kelionę, o modelis, slypintis už jos, remiasi atitinkamais aspektais to, ko jis išmoko apie geografiją, transportą ir virtuvę, kad sugeneruotų maršrutą.

Per pastarąjį dešimtmetį dirbtinio intelekto (DI) galimybių pažanga daugiausia kilo iš didesnių mokymo ciklų; tai yra, didinant skaičiavimų (compute) kiekį, naudojamą DI modeliui apmokyti. Tačiau neseniai tyrėjai pasiekė daugiau rezultatų leisdami modeliams apdoroti informaciją ilgiau ir mokydami juos užduoties atlikimo metu pateikti aiškius samprotavimo žingsnius (‡69*, ‡70). DI sistemos, kurios veikia taip, vadinamos „samprotavimo sistemomis“, o tarpiniai paaiškinimai, kuriuos jos pateikia spręsdamos problemą ar atsakydamos į klausimą, vadinami „samprotavimo grandinėmis“ (chains of thought). Samprotavimo sistemos naudojimo metu, norint sugeneruoti šias sudėtingas samprotavimo grandines, reikalauja daugiau skaičiavimo išteklių (‡71, ‡72, ‡73, ‡74), o mokymo metu – daugiau išteklių, kad jos išmoktų samprotauti geriau. Praktikoje šios samprotavimo galimybės leidžia DI sistemoms spręsti sudėtingesnes problemas iteratyviai skaidant užduotį į mažesnius žingsnius. Stalo 1.3 pateikia pavyzdį, kaip nesamprotavimo sistema ir samprotavimo sistema išsprendžia tą pačią problemą.

Loginimo sistemos pasiekė reikšmingų proveržių gebėjimuose sprendžiant sudėtingas problemas. Pavyzdžiui, 2025 m. loginimo sistemos, specializuotos matematinių uždavinių sprendimui, tokios kaip Google’os Gemini Deep Think ir dar neišleistas eksperimentinis OpenAI modelis, išsprendė Tarptautinės matematikos olimpiados uždavinius (struktūruoto testavimo sąlygomis) tokiu lygiu, kuris prilygo žmonių aukso medalio rezultatams (‡75, ‡76). Loginimo sistemos parodė didelę pažangą formaliose srityse, tokiose kaip matematika, logikos galvosūkiai ir struktūruoti moksliniai klausimai, kur žingsnis po žingsnio loginimas gali būti aiškiai patikrinamas (‡77). Tačiau loginimo sistemos taip pat gali nepavykti, pateikdamos nereikalingas, neproduktyvias ar pasikartojančias mąstymo grandines (‡78, ‡79).

###@ Atnaujinimai mokymo metodų srityje

Nuo paskutinės ataskaitos paskelbimo (2025 m. sausis) mokymo metodas, vadinamas „distiliavimu“, gerokai padidino efektyvumą, kuriuo kai kuriuos modelius galima pritaikyti (fine-tune) tolimesniam mokymui. Distiliavimas apima „studento“ modelio mokymą pagal gautus atsakymus (outputs) galingesnio (ir paprastai didesnio) „mokytojo“ modelio, leidžiant studento modeliui tiesiogiai imituoti mokytojo modelio išvestį (‡80). Pavyzdžiui, „DeepSeek“ sukūrė didelį modelį, pavadintą DeepSeek-R1, kuris pasižymi išskirtiniais grandinės mąstymo (chain-of-thought) argumentavimo gebėjimais. R1 generuotos argumentavimo išvestys buvo panaudotos tuomet mažesnių studentų modelių, įskaitant DeepSeek-V3, pritaikymui. DeepSeek-V3 išlaiko didžiąją dalį R1 matematikos, programavimo (coding) ir dokumentų analizės gebėjimų, ir, kaip pranešama, buvo pritaikytas maždaug už $10,000 USD (nors jo išankstinio mokymo kaštai nebuvo atskleisti) (‡81). Tai, tikėtina, yra keliais dydžiais mažesnė suma nei vienodai pajėgių, didesnių modelių pritaikymo (fine-tuning) kaštai.

![table1.3](images/table1.3_example_reasoning.png)

##### Stalo 1.3: Neužtikimo sistemos pavyzdys (kairėje) palyginti su samprotavimo sistema (dešinėje)
>white|black||9|11|br Sprendžiant tą pačią mįslę, šie pavyzdžiai pritaikyti pagal tikrus AI atsakymus. Samprotavimo sistema daugiau laiko ir skaičiavimo galios skiria „mąstymui“, konstruodama „samprotavimo grandinę“ prieš pateikdama galutinį atsakymą.

![figure.3](images/fig1.3_AI_agent.png)

##### Figūra 1.3: Iliustracinis AI agento vaizdavimas
>white|black||9|11|br Dirbtinio intelekto modelis (centras), sukonfigūruotas iteratyviai planuoti, samprotauti ir naudoti įrankius tikriems darbams atlikti. Šaltinis: Tarptautinė AI saugos ataskaita 2026.


Taigi distiliavimas gali būti pigi ir efektyvi priemonė, kad modeliai įgytų galingesnių gebėjimų (‡82). Kai kurie tyrėjai naudojo distiliavimą, kad pritaikytų (fine-tune) labai pajėgius modelius, pasitelkdami vos 1,000 pavyzdžių, sugeneruotų iš pažangiausių (state-of-the-art) modelių (‡83). Kadangi distiliavimui reikia iš anksto turimo mokytojo modelio, jo negalima tiesiogiai naudoti siekiant paspartinti pažangiausių modelių gebėjimų raidą. Tačiau jis gali paspartinti pažangių dirbtinio intelekto gebėjimų plitimą, net ir naudojant uždaro kodo (closed-source) modelius (‡84*).

Kartu su technologiniais „distribuoto skaičiavimo“ ir decentralizuoto mokymo pažanga (metodais, kai kūrėjai naudoja kelis procesorius, serverius ar duomenų centrus, kurie dirba kartu, kad atliktų AI mokymą arba inferenciją (‡85, ‡86, ‡87)), sumažėjo tai, kiek daugelis AI kūrimo projektų priklauso nuo didelio masto, centralizuotos skaičiavimo infrastruktūros. Tai vis labiau leidžia mažiau išteklių turintiems veikėjams kurti ir diegti galingas sistemas.

###@ Atnaujinimai dėl AI agentų

Nuo paskutinės ataskaitos (January 2025) pažanga, kaip kūrėjai derina AI modelius su įrankiais, leido kurti vis galingesnius AI agentus. AI agentai skirti siekti tikslų, kurie dažnai vartotojų nurodomi natūralia kalba. Norėdami pasiekti šiuos tikslus, jie gauna prieigą prie įrankių, tokių kaip atmintis, kompiuterio sąsaja ir naršyklės. Šie įrankiai ir kodas, naudojamas juos sujungti su modeliu, vadinami „scaffolding“, ir jie padeda AI agentams autonomiškai sąveikauti su pasauliu, sudaryti planus, įsiminti svarbias detales ir siekti tikslų (‡88*, ‡89) su daug mažesne žmonių priežiūra ar pagalba. Pavyzdžiui, Manus AI yra populiarus AI agentas, galintis automatizuoti įvairias užduotis, įskaitant žiniatinklio paiešką, programinės įrangos kūrimą ir internetinius pirkimus (‡90). 1.3 Figūra pateikia paprastą pavyzdį, kaip AI agentas sudarytas iš bendros paskirties AI modelio „brain“, kuris gali iteratyviai planuoti, samprotauti ir naudoti įrankius atminčiai, naršymui internete ir kompiuterio naudojimui.

AI agentų skaitmeninė infrastruktūra plečiasi (‡91), ir jie vis dažniau sutinkami įvairiose pramonės šakose (‡92, ‡93, ‡94). AI agentai buvo sukurti tokioms užduotims kaip tyrimai (‡37), programinės įrangos inžinerija (‡95), robotų valdymas (‡96) ir klientų aptarnavimas (‡97). Nuolatiniai moksliniai tyrimai ir plėtra lėmė, kad vis labiau pajėgūs ir vis labiau autonomiški AI agentai arba daugiagentės sistemos tampa kas kartą labiau gebantys. Tyrėjai yra apskaičiavę, kad programinės įrangos etaloninių užduočių, kurias AI agentai gali atlikti, sudėtingumas maždaug kas septynerius mėnesius padvigubėja (žr. taip pat §1.2. Dabartiniai gebėjimai) (‡98). Ekspertai teigia, kad vis labiau pajėgūs AI agentai sukels ir reikšmingas galimybes, ir rizikas (‡99, ‡100*) (žr. §2.2.1. Patikimumo iššūkiai).

###@ Įrodymų spragos

Pagrindinės įrodymų spragos, susijusios su bendrosios paskirties dirbtinio intelekto (AI) sistemos kūrimo procesu, kyla dėl to, kad nėra viešai prieinamos informacijos apie tai, kaip jos yra kuriamos. Kai kurie kūrėjai labai skaidriai atskleidžia, kaip jie kuria bendrosios paskirties AI sistemas (‡1, ‡101). Tačiau apskritai viešosios ir politikos formuotojų žinios apie tai, kaip dauguma pažangiausių modelių yra kuriami, apsaugomi, vertinami ir diegiami, yra ribotos. Tai ypač būdinga įmonėse viduje diegiamoms AI sistemoms, kurios naudojamos AI kompanijose, bet nėra naudojamos arba suprantamos išorės suinteresuotųjų subjektų (‡102, ‡103). Dėl tokio riboto išorinio matomumo kyla iššūkių skaidrumui ir priežiūrai. Įvairūs tyrėjai nurodė ribotą ir nenuoseklų skaidrumą dėl mokymo duomenų (‡104, ‡105, ‡106), bendrosios paskirties AI modelių (‡107, ‡108), AI agentų (‡92), vertinimų (‡109), kūrimo pakuočių (‡110) ir saugos (‡111). Ribojimai išoriniam atskleidimui kartais yra būtini siekiant apsaugoti kompanijų komercines paslaptis ir intelektinę nuosavybę. Tuo pat metu dėl mažo skaidrumo nepriklausomiems tyrėjams ir politikos formuotojams sunkiau tirti bendrosios paskirties AI modelius ir sistemas.


