###@ Mis on üldotstarbelised tehisintellekti süsteemid?

Üldotstarbelised tehisintellekti süsteemid on tarkvaraprogrammid, mis õpivad mustreid suurest andmemahust, võimaldades neil täita mitmesuguseid ülesandeid, mitte ei ole spetsialiseerunud ühele konkreetsele funktsioonile või valdkonnale (vt Laud 1.1). Nende süsteemide loomiseks viivad tehisintellekti arendajad läbi mitmeastmelise protsessi, mis nõuab märkimisväärseid arvutusressursse, suuri andmestikke ja spetsialiseeritud teadmisi (vt Laud 1.2). Arvutusressursse (mida sageli lühendatakse ’compute’-iks) on vaja nii tehisintellekti süsteemide arendamiseks kui ka kasutuselevõtuks ning need hõlmavad nii spetsialiseeritud arvutikiipe kui ka tarkvara ja infrastruktuuri, mida nende käitamiseks vaja läheb.† Kuna neid treenitakse suurte ja mitmekesiste andmestike põhjal, suudavad üldotstarbelised tehisintellekti süsteemid täita paljusid erinevaid ülesandeid, näiteks kokku võtta teksti, genereerida pilte või kirjutada arvutikoodi. Käesolev jaotis selgitab, kuidas üldotstarbelisi tehisintellekti süsteeme luuakse, mis on ’reasoning’ mudelid ning kuidas poliitikavalikud kujundavad üldotstarbeliste tehisintellekti süsteemide arendust.

    Märkus † -- Termin ‘arvutus’ võib samuti viidata kas protsessori poolt teostatavate arvutuste hulga mõõtmisele (tavaliselt mõõdetuna ujukomaarvutuste operatsioonides sekundis) või konkreetselt sellele riistvarale (nagu graafikaprotsessorid), mis need arvutused teostab.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Keele-süsteemid
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Käsk A (‡3*)
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
###@ Pildigeneraatorid
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Videogeneraatorid
- Cosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Näen 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotika ja navigatsioonisüsteemid
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Biomolekulaarsete struktuuride eri klasside ennustajad
- AlphaFold 3 (‡27)
- Võimenda (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ AI agendid
- AlphaEvolve (‡31*)
- ChatGPT Agent (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- Tehisintellekti teadlane-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Laud 1.1: Üldotstarbelise tehisintellekti tüübid
>white|black||9|11|br On mitu erinevat üldotstarbelise tehisintellekti (AI) tüüpi. Selles aruandes käsitletakse mudeleid, mis suudavad ennustada struktuurset teavet erinevate molekulide klasside jaoks, kui „üldotstarbelist” AI-d, kuna neid saab kohandada mitmesuguste ülesannete jaoks. Näiteks mudelid, mis on treenitud valgu struktuuri ennustama, sobivad paljudeks muudeks ülesanneteks, nagu valkude vastasmõjude ennustamine, väikeste molekulide seondumispaikade ennustamine ning tsükliliste peptiidide (‡40) ennustamine ja kujundamine.


>white|orangered|left|13|15|bb Sügavõpe on üldotstarbelise tehisintellekti põhiline alustala

Teadlased loovad üldotstarbelisi tehisintellekti mudeleid protsessiga, mida nimetatakse „sügavõppeks“, mis treenib mudeleid näidete põhjal õppima (‡41). Erinevalt tarkvarainseneriteadusest õpivad sügavõppe mudelid täitma ülesandeid andmete põhjal, mitte ei toetu käsitsi kirjutatud juhistele. Töötledes suuri andmehulkasid, näiteks pilte, teksti või heli, avastavad need mudelid viise, kuidas andmeid esitada, luues sisemisi mustrite esitusviise (nagu kujundid, seosed sõnade vahel või helistruktuurid), mis aitavad mudelil ära tunda seoseid ja genereerida väljundeid, mis on kooskõlas selle treenimise eesmärgiga. Seejärel kasutavad nad neid õpitud sisemisi esitusviise abstraktsete tunnustena, et analüüsida uut, sarnast andmestikku ja genereerida väljundeid samas stiilis. Näiteks üldotstarbeline tehisintellekti mudel, mida on treenitud piisavalt palju näiteid 19. sajandi romantilisest inglise luulest, suudab ära tunda uusi selles stiilis luuletusi ja toota uut materjali sarnases stiilis.

Peenemas mastaabis toimib süvaõpe nii, et töötleb andmeid läbi kihtide vastastikku ühendatud teabe töötlemise sõlmede. Neid sõlmi nimetatakse sageli ‘neuroniteks’, sest need on vaid laias laastus inspireeritud bioloogiliste ajude neuronitest (‘neuraalvõrgud’) (Kujund 1.1) (‡42). Kui teave voolab ühest neuronite kihist järgmisse, muudab mudel andmeid järk-järgult abstraktsemateks esitusteks kui õpitud tunnuste rühmadeks – mustriteks, mille mudel on andmetest automaatselt leidnud, mitte käsitsi kodeeritud mustriteks. Näiteks pilditöötlusmudelis võivad esimesed kihid õppida tuvastama lihtsaid tunnuseid, nagu servad või põhilised kujundid, samal ajal kui sügavamad kihid ühendavad need tunnused, et esile tuua keerukamaid mustreid, nagu näod või objektid.

Kõigi kihtide tunnused avastatakse optimeerimisprotsessi käigus, mis määratleb treeningprotseduuri. Treeningu ajal, kui mudel teeb vigu, kohandavad süvaõppe algoritmid neuronite vaheliste erinevate ühenduste tugevust, et parandada mudeli toimivust. Iga ühenduse tugevust sõlmede vahel nimetatakse sageli „kaaluks“. See kihiline lähenemine annab süvaõppele selle nime.

Sügavõpe on osutunud väga tõhusaks, võimaldades tehisintellektil (AI) süsteemidel täita ülesandeid, mida varem peeti traditsiooniliste käsitsi programmeeritud arvutuslike süsteemide ja ka teiste varasemate sümbolistlike või reeglitel põhinevate AI meetodite jaoks keerukaks. Enamik tänapäeva tipptasemel üldotstarbelisi AI mudeleid põhineb nüüd konkreetse närvivõrgu arhitektuuril, mida tuntakse kui „transformer“ (‡43, ‡44). Transformerid kasutavad „attention“ mehhanismi (‡45), mis aitab mudelil info töötlemisel keskenduda kõige asjakohasematele osadele sisendandmetes, näiteks määrata, millised sõnad lauses on selle tähenduse mõistmiseks kõige olulisemad. Just selline mudelite ülesehitamise viis on viinud märkimisväärsete edusammudeni tõlkes (‡43), loomuliku keele töötlemises (‡46), pildituvastuses (‡47) ja kõnetuvastuses (‡48, ‡49), mis on lõpuks viinud tänapäeval kõige arenenumate mudelite väljatöötamiseni.

![fig1.1](images/fig1.1_neural_network.png)

##### Kujund 1.1: Illustratiivne kujutis „neuraalvõrgust”
>white|black||9|11|br Tänapäeva üldotstarbelised tehisintellekti mudelid põhinevad neil võrkudel, mis on vaid lõdvalt inspireeritud bioloogilistest ajudest. Erinevatel võrkudel on erinevad suurused ja arhitektuurid. Samas kõik need koosnevad omavahel seotud info töötlevatest ühikutest, mida nimetatakse “neuroniteks”, kus neuronitevaheliste ühenduste tugevusi nimetatakse “kaaludeks”. Kaalusid uuendatakse treeningu käigus suure hulga andmetega. Allikas: International AI Safety Report 2025 (‡50) (muudetud).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Kujund 1.2: Üldotstarbelise tehisintellekti arendamise etappide skeemiline kujutis
>white|black|left|9|11|br Rahvusvaheline tehisintellekti ohutuse aruanne 2026.


>white|orangered|left|13|15|bb Üldotstarbeline tehisintellekt töötatakse välja etappide kaupa

Üldotstarbelise tehisintellekti süsteemi väljatöötamine hõlmab mitut etappi alates esmasest mudeli treenimisest kuni kasutusejärgse monitooringu ja uuendusteni (Kujund 1.2). Praktikas kattuvad need sammud sageli iteratiivsel moel. Iga etapp nõuab erinevaid ressursse (nt andmed, tööjõud, arvutusvõimsus) ja erinevaid tehnikaid ning neid viiakse mõnikord läbi erinevate arendajate poolt (Kujund 1.2 ja Laud 1.2).

Näiteks mudeli eelkoolitus nõuab üldjuhul suures koguses arvutusvõimsust ja andmeid, mistõttu see etapp on eriti tundlik poliitikate suhtes, mis mõjutavad juurdepääsu arvutusressurssidele või koolitusandmetele (‡51, ‡52). Samuti hõlmavad andmete ettevalmistamine ja mõned mudeli peenhäälestamise meetodid praegu algse andmete märgendamise puhul suuri hulki inimtööd (‡53). Seetõttu on see etapp tundlik tööjõukulude, platvormipoliitikate või regulatsioonide muutuste suhtes, mis mõjutavad piiriüleseid tellimuslepingute korraldusi.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Andmete kogumine ja ettevalmistus
> 
  Enne üldotstarbelise tehisintellekti mudeli treenimist koguvad arendajad ja andmetöötajad, puhastavad, kureerivad ning ühtlustavad toorandmed sellises vormis, millest mudel saab õppida. See võib olla töömahukas protsess. Tipptasemel mudelite taga olevad treeningandmestikud koosnevad tohutust hulgast näidetest üle kogu interneti.
  Tiimid töötavad sageli välja keerukaid filtreerimismeetodeid, et vähendada kahjulikku sisu, kõrvaldada dubleeriv andmestik ning parandada esindatust eri teemade ja allikate lõikes (‡54, ‡55). Andmete kureerimine võib samuti aidata vähendada autoriõiguse ja privaatsuse rikkumisi, eemaldada näiteid, mis sisaldavad ohtlikku teadmist, käsitleda mitut keelt ning parandada andmete päritolule (data provenance) viitavat dokumentatsiooni (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Eelõpe (treeningu esimene etapp)

  Eelõpetuse käigus annavad arendajad mudelitele tohututes kogustes mitmekesist andmestikku, et juurutada lai baas teadmisi ja kontekstuaalne arusaam. See protsess loob niinimetatud „baasmudeli“. Tegemist on väga andmetemahuka ja arvutusmahuka protsessiga.

  Eelõpetuse ajal puutuvad mudelid kokku miljardite või triljonite näidetega sisust, nagu pildid, tekstid või heli. Selle kokkupuute kaudu avastab mudel järk-järgult andmeid esindavaid abstraktseid tunnuseid ning õpib, kuidas need tunnused on omavahel seotud, mis võimaldab tal teha uute sisendite puhul kontekstis mõtestatud järeldusi. See eelõpetuse protsess kestab nädalaid või kuid (‡59) ning kasutab kümneid või sadu tuhandeid graafilisi töötlusüksusi (GPU-sid) või tensori töötlusüksusi (TPU-sid) (‡60) – spetsialiseeritud arvutuskiipe, mis on loodud selliste arvutuste sujuvaks ja kiireks teostamiseks suures mahus. Mõned arendajad teevad eelõpetust oma arvutusvõimega, samas kui teised kasutavad spetsialiseeritud arvutusteenuse pakkujate poolt pakutavaid ressursse.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Järeleõpe ja peenhäälestus (treeningu teine etapp)

  „Järeltreening“ täpsustab põhimudelit, et optimeerida see konkreetseks rakenduseks. Tegemist on mõõdukalt suurt arvutusressurssi nõudva ja väga töömahuka protsessiga. Üleminek „sünteetilistele andmetele“ – tehislikult loodud teabele, mis jäljendab reaalmaailma andmeid, kuid on koostatud algoritmide või simulatsioonide abil – aitab muuta see etapp vähem töömahukaks.
  Järeltreening hõlmab mitmesuguseid peenhäälestamise tehnikaid ja muid muudatusi. ‘Juhendatud peenhäälestamine’ tähendab treenitud mudeli täiendavat treenimist konkreetsetel andmekogumitel, et parandada mudeli jõudlust selles valdkonnas (‡61, ‡62). Näiteks üldotstarbeline mudel võiks olla täiendavalt treenitud suurel hulgal radioloogiliste piltide andmeid sisaldaval korpusel. ‘Tugevdusõpe’ (RL) hõlmab mudeli jõudluse parandamist ‘premeerimise’ kaudu (positiivse tagasiside andmine) soovitud väljundite eest ning ‘karistamise’ kaudu (negatiivse tagasiside andmine) soovimatute väljundite eest. Sellel on kaks silmapaistvat alaliiki. ‘Tugevdusõpe inimeste tagasisidega’ hõlmab väljundite premeerimist, mis vastavad inimeste eelistustele, ja nende karistamist, mis ei vasta, tuginedes inimeste tagasisidele (‡63, ‡64*). ‘Tugevdusõpe kontrollitavate preemiatega’ (RLVR) kasutatakse mudeli jõudluse parandamiseks ülesannetes, mis nõuavad faktilist korrektsust, nagu matemaatika või koodi genereerimine. Arendajad vaheldavad tavaliselt järeltöötluse tehnikate rakendamist ja testide käivitamist, kuni tulemused näitavad, et mudel vastab soovitud nõuetele.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Süsteemi integreerimine

  Arendajad ühendavad ühe või mitu üldotstarbelist tehisintellekti mudelit teiste komponentidega, et luua “tehisintellekti süsteem”, mis on kasutamiseks valmis. GPT-5 (näiteks) on üldotstarbeline tehisintellekti mudel, mis töötleb teksti, pilte ja heli, samal ajal kui ChatGPT on üldotstarbeline tehisintellekti süsteem, mis ühendab mitu erineva suuruse ja võimekusega mudelit koos vestlusliidese, sisutöötluse, veebiühenduse ja rakenduste integratsiooniga, et luua toimiv toode.
  Lisaks sellele, et tehisintellekti mudelid tehakse töövõimeliseks, püüavad AI-süsteemi täiendavad komponendid samuti suurendada võimekust, kasulikkust ja ohutust. Näiteks võib süsteemiga kaasneda filter, mis tuvastab ja blokeerib mudeli sisendid või väljundid, mis sisaldavad kahjulikku sisu (‡65*). Arendajad kasutavad üha enam ka „tugistruktuure“ (scaffolding) – täiendavat tarkvara, mis on ehitatud üldotstarbeliste tehisintellekti mudelite ümber ja võimaldab neil ette planeerida, eesmärke taotleda ning maailmaga suhelda (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. E juurutamine ja väljalase
  Kasutuselevõtt on protsess, mille käigus tehakse integreeritud tehisintelligentsuse süsteem kättesaadavaks selleks ettenähtud kasutuseks. Arendajad ja kasutuselevõtjad juurutavad tehisintelligentsuse süsteeme reaalsesse keskkonda rakendustena, toodetena või teenustena. Arendajad saavad tehisintelligentsuse süsteeme kasutusele võtta nii ettevõttesiseselt (oma tarbeks) kui ka väliselt (era- või avalikuks kasutuseks eraklientidele). Kui tehisintelligentsuse süsteemid võetakse kasutusele väliselt, pakuvad ettevõtted kasutajatele sageli juurdepääsu veebipõhiste kasutajaliideste või rakendusprogrammeerimisliideste (API-de) kaudu, mis võimaldavad kasutajatel süsteemile ligi pääseda ja seda käivitada. Näiteks võib üks ettevõte kujundada eritellimusel loodud klienditeeninduse vestlusroboti, mida juhib teise ettevõtte üldotstarbeline tehisintelligentsuse süsteem.
  “AI-süsteemi juurutamine” viitab mudeli kättesaadavaks tegemisele reaalse maailma kasutuseks koos integreeritud tööriistade ja liidestega, samas kui “mudeli avaldamine” hõlmab baas-mudeli kättesaadavaks tegemist teistele – kas avatud kaalu vormis (allalaaditavad parameetrid) või suletud kaalu vormis (ainult API kaudu). Vt §3.4. Avatud kaalu mudelid.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Järelevalve pärast kasutuselevõttu ja uuendused

  Arendajad koguvad sageli kasutajate tagasisidet ja analüüsivad seda, jälgivad mõju- ja jõudlusmõõdikuid ning teevad iteratiivseid parandusi, et lahendada probleeme, mis avastatakse tegelikus kasutuses (‡67). Parandused tehakse süsteemi integratsioone uuendades, sageli pideva peenhäälestuse abil ja pakkudes mudelitele juurdepääsu välistele (värsketele) faktide andmebaasidele. Nii püsivad suured tehisintellekti mudelid ajakohased ilma kogu eelneva treeningu protsessi kordamata (‡68*). See võimaldab võimetel kuhjuda järjestikuste treeningvoorude jooksul, säilitades samal ajal stabiilsuse ja vähendades arvutuslikke kulusid.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Laud 1.2: Üldotstarbelise tehisintellekti arendusetapid
>white|black||9|11|br Igal üldotstarbelise AI arendusetapil täiustatakse tehisintellekti mudelit järeltöötluseks ja seejärel võetakse see lõpuks kasutusele täielikult integreeritud AI-süsteemina, mida jälgitakse ja uuendatakse.


>white|orangered|left|13|15|bb Põhjendussüsteemid genereerivad järelduse käigus „mõttekäike“, et jõudlust parandada

Järeldamine toimub siis, kui keegi kasutab AI-mudelit pärast selle treenimist. Näiteks järeldamine toimub siis, kui inimene palub AI-süsteemil planeerida reis ja selle taga olev mudel tugineb asjakohastele aspektidele, mida ta on õppinud geograafia, transpordi ja köögi kohta, et koostada marsruut.

Viimase kümnendi jooksul on edusammud tehisintellekti võimekustes suuresti tulnud suurematest treeningutest; see tähendab, et suurendatakse arvutusvõimsust, mida kasutatakse tehisintellekti mudeli treenimiseks. Hiljuti on teadlased siiski saavutanud rohkem edusamme, võimaldades mudelitel töödelda teavet kauem ning treenides neid tootma ülesande täitmisel üles selgedut mõttekäigu samme (‡69*, ‡70). Seda tüüpi tehisintellektisüsteeme nimetatakse ‘põhjendussüsteemideks’ ning vahepealseid selgitusi, mida need probleem lahendades või küsimusele vastates läbivad, nimetatakse ‘mõttekäigu ahelateks’ (chains of thought). Põhjendussüsteemid nõuavad nende keerukate mõttekäigu ahelate genereerimiseks rohkem arvutusressursse kasutamise hetkel (‡71, ‡72, ‡73, ‡74) ning rohkem ressursse treeningu ajal, et need õpiksid paremini põhjendama. Praktikas võimaldavad need põhjendusvõimed tehisintellektisüsteemidel lahendada keerukamaid probleeme, jaotades ülesande iteratiivselt väiksemateks sammudeks. Tabel 1.3 näitab näidet mittpõhjendussüsteemist ja põhjendussüsteemist, mis lahendavad sama probleemi.

Põhjendus- ja arutlussüsteemid on saavutanud suuri läbimurdeid võimekustes keeruliste probleemide lahendamisel. Näiteks 2025. aastal lahendasid matemaatiliste probleemide lahendamisele spetsialiseerunud põhjendus- ja arutlussüsteemid, nagu Google’i Gemini Deep Think ja OpenAI avaldamata eksperimentaalne mudel, Rahvusvahelise matemaatikaolümpiaadi ülesandeid (struktureeritud testitingimustes) tasemel, mis vastab inimese kuldmedaliga võrreldavale sooritusele (‡75, ‡76). Põhjendus- ja arutlussüsteemid on näidanud märkimisväärset edasiminekut formaalsetes valdkondades, nagu matemaatika, loogikamõistatused ja struktureeritud teadusküsimused, kus samm-sammult arutluskäiku saab selgesõnaliselt kontrollida (‡77). Samas võivad põhjendus- ja arutlussüsteemid ka ebaõnnestuda, tekitades ebaolulisi, mitteproduktiivseid või korduvaid arutluskäike (‡78, ‡79).

###@ Uuendused koolitusmeetodites

Pärast eelmise aruande avaldamist (jaanuar 2025) on koolitusmeetod nimega „distillatsioon” oluliselt suurendanud tõhusust, millega mõningaid mudeleid saab järeleõppe abil kohandada. Distillatsioon tähendab „õpilas”-mudeli treenimist võimsama (ja tavaliselt suurema) „õpetaja”-mudeli väljundite põhjal, võimaldades õpilas mudelil jäljendada õpetaja mudeli väljundeid otse (‡80). Näiteks töötas DeepSeek välja suure mudeli nimega DeepSeek-R1, mis on eriti tugev chain-of-thought (samm-sammuline arutlus) tüüpi põhjenduste koostamisel. R1 genereeris arutluste väljundeid, mida kasutati seejärel väiksemate õpilas mudelite, sh DeepSeek-V3, järeleõppeks. DeepSeek-V3 säilitab suure osa R1 matemaatilistest, kodeerimis- ja dokumendianalüüsi võimekusest ning selle kohta teatati, et see kohandati ligikaudu $10,000 USD (kuigi selle eelkoolituse kulusid ei avaldatud) (‡81). Tõenäoliselt on see suurusjärkudega väiksem kui sellise samavõimelise, kuid suurema mudeli järeleõppe hind.

![table1.3](images/table1.3_example_reasoning.png)

##### Laud 1.3: Näide mittepõhjendavast süsteemist (vasakul) versus põhjendavast süsteemist (paremal)
>white|black||9|11|br Sama mõistatuse lahendamine: need näited on kohandatud päris AI vastustest. Põhjendussüsteem kulutab rohkem aega ja arvutusvõimsust „mõtlemisele“, koostades enne lõpliku vastuse esitamist „mõttekäigu“ („chain of thought“).

![figure.3](images/fig1.3_AI_agent.png)

##### Kujund 1.3: AI agendi illustreeriv kujutis
>white|black||9|11|br AI-mudel (keskel), mis on konfigureeritud ülesandeid reaalses maailmas täitma iteratiivselt planeerides, arutledes ja kasutades tööriistu. Allikas: International AI Safety Report 2026.


Seega võib destilleerimine olla odav ja tõhus viis, kuidas mudelid omandavad võimekamad võimed (‡82). Mõned teadlased on kasutanud destilleerimist, et peenhäälestada väga võimekaid mudeleid, kasutades vaid 1,000 näidet, mis on genereeritud tipptasemel mudelitest (‡83). Kuna destilleerimine eeldab olemasolevat õpetajmudelit, ei saa seda otse kasutada tipptasemel mudelite võimekuse edendamiseks. Siiski võib see kiirendada arenenud tehisintellekti võimete levikut, isegi suletud lähtekoodiga mudelitest (‡84*).

Koos tehnoloogiliste edusammudega „jaotatud arvutusvõimsuse” ja detsentraliseeritud treenimisega (lähenemisviisid, kus arendajad kasutavad mitut protsessorit, serverit või andmekeskust, mis töötavad koos, et teostada tehisintellekti treenimist või inferentsi (‡85, ‡86, ‡87)), on vähenenud määr, mil määral paljud AI-arenduse projektid sõltuvad suuremahulisest tsentraliseeritud arvutusvõimsuse taristust. See võimaldab üha enam vähemate vahenditega osalistel arendada ja kasutusele võtta võimsaid süsteeme.

###@ Uuendused tehisintellekti agentide kohta

Alates viimasest aruandest (jaanuar 2025) on arengud selles, kuidas arendajad ühendavad AI-mudeleid tööriistadega, võimaldanud välja töötada järjest võimsamaid AI-agente. AI-agendid on loodud eesmärkide poole püüdlemiseks, mida sageli määravad kasutajad loomulikus keeles. Nende eesmärkide saavutamiseks antakse neile ligipääs tööriistadele, nagu mälu, arvuti liides ja veebibrauserid. Neid tööriistu ning koodi, mida kasutatakse nende koos mudeliga ühendamiseks, nimetatakse „tugistruktuuriks“ (scaffolding) ning need aitavad AI-agentidel iseseisvalt maailmaga suhelda, plaane teha, olulisi detaile meeles pidada ja eesmärkide poole püüelda (‡88*, ‡89) palju väiksema inimeste järelevalve või abiga. Näiteks Manus AI on populaarne AI-agent, mis suudab automatiseerida mitmesuguseid ülesandeid, sealhulgas veebipäringuid, tarkvaraarendust ja veebis oste (‡90). Kujund 1.3 illustreerib lihtsat näidet AI-agendist, mis koosneb üldotstarbelisest AI-mudelist „ajuna“ (brain), mis suudab iteratiivselt planeerida, arutleda ja kasutada tööriistu mälu, veebisirvimise ja arvutikasutuse jaoks.

Tehisintellekti agentide digitaristu laieneb (‡91) ning need on muutunud üha tavalisemaks eri valdkondades (‡92, ‡93, ‡94). Tehisintellekti agendid on välja töötatud selliste ülesannete jaoks nagu teadusuuringud (‡37), tarkvaraarendus (‡95), robotjuhtimine (‡96) ja klienditeenindus (‡97). Käimasolev uurimis- ja arendustegevus on viinud selleni, et tehisintellekti agendid või mitmeagendilised süsteemid on muutunud järjepidevalt võimekamaks ja autonoomsemaks. Uurijad on hinnanud, et tarkvaraliste võrdlusülesannete keerukus, mida tehisintellekti agendid suudavad täita, kahekordistub ligikaudu iga seitsme kuu järel (vt ka §1.2. Current capabilities) (‡98). Eksperdid väidavad, et üha võimekamad tehisintellekti agendid toovad kaasa nii märkimisväärseid võimalusi kui ka riske (‡99, ‡100*) (vt §2.2.1. Reliability challenges).

###@ Tõenduslüngad

Peamised tõenduslüngad üldotstarbelise tehisintellekti süsteemide arendamise protsessi osas tulenevad avalikult kättesaadava teabe puudumisest selle kohta, kuidas neid arendatakse. Mõned arendajad on väga läbipaistvad selle suhtes, kuidas nad arendavad üldotstarbelisi tehisintellekti süsteeme (‡1, ‡101). Siiski on üldiselt avalike ja poliitikakujundajate teadmiste määr selle kohta, kuidas enamik täiustatud mudeleid on arendatud, kaitstud, hinnatud ja kasutusele võetud, piiratud. See kehtib eriti ettevõtete sees kasutusele võetud tehisintellekti süsteemide puhul, mida kasutatakse AI-ettevõtetes, kuid mida ei kasutata ega mõisteta väljaspoolseid sidusrühmi (‡102, ‡103). See piiratud välise nähtavuse tase tekitab välise läbipaistvuse ja järelevalvega seotud väljakutseid. Mitmed uurijad on osutanud koolitusandmete (‡104, ‡105, ‡106), üldotstarbeliste tehisintellekti mudelite (‡107, ‡108), tehisintellekti agentide (‡92), hindamiste (‡109), arendusliinide (‡110) ja ohutuse (‡111) osas esinevale piiratud ja ebaühtlasele läbipaistvusele. Piiratud võimalus väljastada teavet on mõnikord vajalik ettevõtete ärisaladuste ja intellektuaalomandi kaitseks. Samal ajal muudab madal läbipaistvus sõltumatutel uurijatel ja poliitikakujundajatel üldotstarbeliste tehisintellekti mudelite ja süsteemide uurimise raskemaks.


