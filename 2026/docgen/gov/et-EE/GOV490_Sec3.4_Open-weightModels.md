##########
>white|orangered|left|14|30|hr Jaotis 3.4
### 3.4. Avatud lähtekoodiga mudelid
>white|orangered|left|24|30|hb Avatud kaaludega mudelid

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb Oluline teave
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Juurdepääsu tase, mida AI-ettevõtted pakuvad oma mudelite „kaaludele“, mõjutab nende mudelitega seotud riske. Kaalud on matemaatilised parameetrid, mis võimaldavad AI-mudelitel töödelda sisendeid ja genereerida väljundeid. Iga konkreetse mudeli puhul saavad ettevõtted valida, kas hoida kaalud täielikult privaatsena, anda mõnele kasutajale piiratud juurdepääs või lubada kellel tahes need täies mahus alla laadida. Selliseid mudeleid, mille kaalud on avalikult kättesaadavad, nimetatakse „open-weight mudeliteks“.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Avatud kaalu (open-weight) mudelid hõlbustavad teadusuuringuid ja innovatsiooni, kuid nende kaitsed on kergemini eemaldatavad. Üle kogu maailma saavad erinevad osalejad – eriti need, kellel on vähem ressursse – kasutada avatud kaalu (open-weight) mudeleid teaduslikel ja kommertseesmärkidel. Siiski, võrreldes suletud kaalu (closed-weight) mudelitega, on avatud kaalu (open-weight) mudelid potentsiaalselt kahjuliku käitumise esiletoomiseks kergemini muudetavad ning s on raskem.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Avatud lähtekoodiga mudelite (open-weight) väljaanded on pöördumatud. Kui need on avaldatud, ei saa mudeli kaalusid tagasi kutsuda. See muudab potentsiaalsete kahjude leevendamise raskemaks, mis tulenevad ohtlike võimetega mudeli avaldamisest.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Alates eelmisest aruandest (jaanuar 2025) on suurema avaliku raskusega (open-weight) mudelite olulised väljaanded vähendanud võimekuse lõhet juhtivate suletud mudelitega. Hiina arendajad DeepSeek ja Alibaba avaldasid vastavalt oma R1 ja Qwen mudelid, mis saavutasid jõudluse, mis on võrreldav juhtivate suletud mudelitega, samal ajal kui OpenAI avaldas oma esimesed avaliku raskusega mudelid alates aastast 2019. Juhtivate suletud mudelite võimekusi hinnatakse nüüd olevat vähem kui ühe aasta võrra ees juhtivatest avaliku raskusega mudelitest silmapaistvatel tehisintellekti võrdlusülesannetel (AI benchmark).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Oluline poliitiline väljakutse on saavutada avatud kaaludega mudelite pakutavad eelised, samal ajal juhtides nende eripäraseid riske. Üks lähenemisviis on hinnata avatud kaaludega mudeleid nende “marginaalse riski” kaudu: mil määral nende avaldamine kontrafaktiliselt suurendab ühiskondlikku riski võrreldes sellega, mida juba põhjustavad olemasolevad mudelid või muud tehnoloogiad. Kuid praktikas on see keeruline. Aja jooksul võivad väikesed suurenemised marginaalses riskis kokku liituda ning viia märkimisväärsete suurenemisteni üldises riskis.
>oldlace|black||11|15|br      


Avaliku allalaadimiseks saadaval olevate parameetritega avatud lähtekoodiga mudelitel on eristatavad mõjud paljudele eelmistes jaotistes käsitletud väljakutsetele. AI-mudeli “kaalud” sisaldavad otsustavat teavet, mis võimaldab tal genereerida kasutajatele kasulikke vastuseid. Kui need on välja antud, ei saa neid enam tagasi kutsuda: igaüks saab need alla laadida, uurida, muuta, jagada ja kasutada oma arvutites või pilvekontodes. Kui kaalud on avalikult kättesaadavad, saavad teised neid kergemini edasi arendada ja muuta, et täita erinevaid vajadusi ning soodustada innovatsiooni (‡1317). Kuid sama mehhanismi tõttu saavad pahatahtliku kavatsusega kasutajad samuti kergemini eemaldada kaitsemeetmed ja muuta avatud lähtekoodiga mudeleid kahjulike kasutusjuhtumite jaoks (‡1122, ‡1160). See on tekitanud küsimuse, kas mõned avatud lähtekoodiga mudelid peaksid alluma erinõuetele (nt rangem testimine enne väljaandmist) või, vastupidi, neile tuleks anda erandkohtlemine (nt regulatiivsest aruandluskohustusest vabastamine) (‡1033).

###@ Taust avatud kaalukasutusega mudelite kohta

>white|orangered||14|15.5|bb Avatud kaaludega mudelid võivad olla, kuid ei pea tingimata olema „avatud lähtekoodiga” mudelid

Kuigi neid nimetatakse sageli “avatud lähtekoodiks”, on enamik avalikult välja antud mudeleid täpsemalt kirjeldatav kui “avatud kaalud”. Põhjus on selles, et kuigi arendajad annavad mudeli kaalud, ei avalda nad sellega seotud treeningukoodi ega andmekogumeid. Lisaks on avatud lähtekoodiga tarkvara tavaliselt iseloomustatud litsentsidega, mis seavad minimaalsed nõuded järgnevatele osalistele, kes kasutavad või muudavad tarkvara (‡1318). Näiteks Meta Llama mudelitel on piiravad litsentsitingimused ning need sisaldavad ainult järelduskoodi, mitte treeningukoodi, mistõttu neid tavaliselt ei loeta avatud lähtekoodiks (‡1319, ‡1320). Mudeli väljaandmise võimalused paiknevad spektril alates täielikult suletust kuni täielikult avatud lähtekoodini ning igas punktis on erinevad risk- ja kasueeliste tasakaalud (‡1086*, ‡1320, ‡1321). Tabel 3.9 kirjeldab neid võimalusi.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Täielikult suletud
  Kasutajad ei saa mudeliga üldse otseselt suhelda
  Näited: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Majutatud juurdepääs
  Kasutajad saavad suhelda ainult konkreetse rakenduse või liidese kaudu, näiteks mobiilse vestlusroboti rakenduse kaudu
  Näited: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb Juurdepääs API kaudu mudelile
  Kasutajad saavad saata mudelile päringuid koodi kaudu, võimaldades kasutust väliste rakenduste jaoks
  Näited: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb API juurdepääs peenhäälestusele
  Kasutajad saavad mudelit oma konkreetsete vajaduste jaoks peenhäälestada
  Näited: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Avatud kaalud: allalaadimiseks saadaval olevad kaalud
  Kasutajad saavad mudeli alla laadida ja seda oma arvutites käivitada
  Näited: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Kaalud, andmed ja kood allalaadimiseks saadaval kasutuspiirangutega
  Kasutajad saavad mudeli ning järelduse- ja koolituskoodi alla laadida ja käivitada, kuid selle kasutamisele on kehtestatud teatud litsentsipiirangud
  Näited: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Täielikult avatud: kaalukid, andmed ja kood on allalaadimiseks saadaval ilma kasutuspiiranguteta
  Kasutajatel on täielik vabadus mudel, kogu kood ja andmed alla laadida, kasutada ja muuta
  Näited: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Laud 3.9: Mudeli jagamise valikud alates täielikult suletust kuni täielikult avatuni
>white|black||9|11|br Mudeli jagamise võimaluste näitlik valik, alates täielikult suletud mudelitest (mudelid on privaatsed ja neid hoitakse ainult ettevõttesiseks kasutuseks) kuni täielikult avatud ja avatud lähtekoodiga mudeliteni (mudeli kaalud, andmed ja kood on vabalt ja avalikult kättesaadavad ilma kasutuse, muutmise ja jagamise piiranguteta). Esimesse nelja kategooriasse kuuluvad mudelid on sageli nimetatud kui „suletud”. Käesolev jaotis keskendub kolmele alumisele reale. Allikas: kohandatud Bommasani, 2024 (‡1317).


###@ Eelised ja riskid

>white|orangered|left|14|15.5|bb Avatud lähtekoodiga (open-weight) mudelid on lihtsamalt kohandatavad ja hinnatavad

Avatudkaaluga mudelid pakuvad olulisi eeliseid teadustööks, innovatsiooniks ja juurdepääsuks. Nagu on arutatud jaotises §1.1. Mis on üldotstarbeline tehisintellekt?, üldotstarbeliste tehisintellekti mudelite treenimine on ülikalt kulukas – tipptasemel mudelite arendamine maksab sadu miljoneid dollareid. Mudeli kaalu avatud vabastamine võimaldab vähemate ressurssidega tegijatel olemasolevaid süsteeme kopeerida, uurida ja nendele tugineda. Ilma sellise juurdepääsuta riskivad väheste ressurssidega piirkondade kogukonnad jääda AI eelistele juurdepääsust kõrvale, mistõttu avatud kaalud on kriitilised võimaldamaks globaalset enamuse osalemist AI arenduses (‡1322). Edasised arendajad saavad peenhäälestada mudeleid erinevate rakenduste jaoks, näiteks kohandada neid alarahastatud vähemuskeelte jaoks või optimeerida jõudlust konkreetsete ülesannete jaoks, nagu õigusliku teksti koostamine või meditsiiniliste märkmete tegemine (‡1323, ‡1324*). Nii võivad avatudkaaluga mudelid võimaldada rohkematel inimestel ja kogukondadel kasutada AI-d ja saada sellest kasu, kui see muidu oleks võimalik (‡1325). Mudelite puhul, mis ei ole piisavalt võimekad, et olla ohtlikud, võivad need eelised kaaluda üles täiendava riski, mis kaasneb kaalu avatud avaldamisega, kuigi see sõltub asjakohaste otsustajate riskitaluvusest.

Avatudkaalu (open-weight) väljalase laiendab ka arendajate ja teadlaste hulka, kes saavad mudelit uurida, hinnata selle võimekust, testida haavatavusi ja teha parandusi iteratiivselt (‡1326, ‡1327). See muudab tõenäolisemaks, et tuvastatakse nii kasulikud rakendused kui ka kahjulikud vead, kuigi see pole tagatud (‡1328, ‡1329). Kasutajad saavad avatudkaalu mudeleid käivitada ka oma seadmetes, mis võimaldab neil hoida kontrolli tundlike andmete üle ja vältida nende saatmist kolmandate osapoolte serveritesse.

Lisahüvesid on siis, kui arendajad jagavad teavet, nagu koolitusandmed, kood, hindamistööriistad ja dokumentatsioon, samuti mudelikaalud (‡1320, ‡1330, ‡1331, ‡1332*). Rohkem teavet võimaldab järgnevate arendajatel ja teistel uurijatel avatud kaaludega mudeleid paremini mõista ning kohandada neid uutele rakendustele.

>white|orangered|left|14|15.5|bb Avatud kaalukomplektide mudelite kaitsed on kergemini eemaldatavad, mis võimaldab võimalikku pahatahtlikku kasutust

Avatud kaaludega mudelid kujutavad endast täiendavaid riske, kuna nende kaitsemeetmeid on lihtsam eemaldada. Ehkki nii avatud kui ka kinniste kaaludega mudelitel võivad olla kaitsemeetmed, mis keelduvad kahjulike kasutajapäringute täitmisest, on need avatud kaaludega mudelite puhul palju lihtsamalt eemaldatavad. Kuritahtlikud osalised saavad mudelit peenhäälestada, et optimeerida selle jõudlust kahjulike rakenduste jaoks, eemaldada koodiosad, mis on mõeldud kahjulike kasutuste ennetamiseks, või tühistada varasema ohutuse peenhäälestamise (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Selle tulemusena võivad avatud mudeli kaalud süvendada §2.1 arutatud kuritarvitamise riske. Kahjulikust kasutusest tulenevad ohud võivad kasvada, kuna rohkem osalisi saab olemasolevaid võimeid kuritahtlikel eesmärkidel ära kasutada ja täiustada ilma järelevalveta (‡1122, ‡1315). Kuigi paljudel kasutajatel ei pruugi olla oskust ega motivatsiooni avatud kaaludega mudelite kaitsemeetmeid eemaldada, on probleemiks eriti motiveeritud kuritahtlikud osalised. Lisaks võivad kuritahtlikud osalised olla võimelised kasutama avatud kaaludega mudeleid, et tuvastada sarnastes kinnistes mudelites haavatavusi (‡1055*). Selliseid puudusi on raskem leida ainult kinniseid mudeleid käivitades, kuna kinnis-mudelite pakkujad saavad rakendada ulatuslikumat kontrolli ja jälgimismeetmeid.

>white|orangered|left|14|15.5|bb Mudeli kaalukogumi jagamine on pöördumatu

Kui mudeli kaalud on avalikuks allalaadimiseks saadaval, ei ole võimalik teostada kõigi olemasolevate koopiate täielikku tagasipööramist. Interneti-hostingu platvormid, nagu GitHub ja Hugging Face, võivad mudeleid oma platvormidelt eemaldada, mistõttu on mõnel osalejal raskem leida allalaaditavaid koopiaid ning see loob olulise tõkke paljudele juhuslikele pahatahtlikele kasutajatele (‡1339). Ometi saavad motiveeritud osalejad endiselt koopiaid hankida, kui mudel on juba alla laaditud ja mujale üles riputatud või kohapeale salvestatud. Lisaks pärivad edasiarendajad, kes integreerivad avatud-kaaluga mudeleid oma süsteemidesse, samuti kõik puudused, näiteks haavatavused vastandlike rünnakute suhtes (‡1055) või mudeli võime hiilida mööda seirest (vt §2.2.2. Kontrolli kaotus) (‡1315). Erinevalt suletud mudelitest, kus hostid saavad universaalselt parandusi välja rullida, ei saa avatud-kaaluga mudelite arendajad tagada, et uuendused võtavad kasutajad kasutusele.

###@ Värskendused

Pärast viimase aruande avaldamist (jaanuar 2025) on juhtivate avatud kaaludega mudelite ja suletud mudelite vaheline suutlikkuse lõhe vähenenud. Hiina arendajad on muutunud eriti oluliseks avatud kaaludega mudelite pakkujaks. 2025. aasta jaanuaris avaldas DeepSeek oma R1 mudeli, mis saavutas mitmel võrdlusel (‡1340) OpenAI o1-ga võrreldava jõudluse. Alibaba Qwen’i mudelid on samuti hoogu kogunud, olles alates 2025. aasta augustist Chatbot Arenal, mis on laialdaselt kasutatav jõudluse võrdlusnäitaja, hõivanud avatud kaaludega mudeli esikoha (‡1341, ‡1342*). 2025. aasta augustis avaldas OpenAI oma esimesed avatud kaaludega mudelid pärast GPT-2 avaldamist 2019. aastal: gpt-oss-120b ja gpt-oss-20b. Meta on jätkanud Llama mudelite avaldamist avatud kaaludega. Juhtivate suletud mudelite suutlikkust hinnatakse nüüd, et see jääb enam-vähem alla üheaastase ajavahega juhtivate avatud mudelite suhtes tuntud tehisintellekti võrdlusnäitajatel (Kujund 3.10).

###@ Tõenduslüngad

Oluline tõenduslik lünk puudutab tehniliste lahenduste tegeliku tõhususe küsimust avatud lähtekoodiga mudelite väärkasutuse ennetamisel. Uurijad on pakkunud välja mitmesuguseid lähenemisi, et muuta mudelid rikkumise suhtes vastupidavaks. Siia kuuluvad uued treeningumeetodid, mis on loodud tegema mudeleid kahjulikule muutmisele vastupidavaks (‡1276), kahjuliku sisu filtreerimine treeningandmetest (‡55) ning kaitsed jailbreakide vastu (‡675, ‡676). Neid tehnikaid võetakse nüüd kasutusele reaalse maailma avaldustes suurte arendajate poolt. Näiteks kasutas OpenAI mõningaid neist tehnikatest oma gpt-oss mudelites, teatades, et vaenuliku (adversarial) viimistlusega versioonid ei saavutanud kõrget võimekuse künnist (‡1344*). Siiski on uuringud näidanud, et pahatahtlikud osalised saavad turvameetmed keelata, treenides mudeleid uuesti kahjulike näidete põhjal (‡1345, ‡1346). Lisaks on endiselt keeruline hinnata kaitsemeetmete vastupidavust usaldusväärselt, mistõttu nende tõhusus reaalse maailma rünnakute vastu on ebakindel (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Kujund 3.10: Võimekuse puudujääk juhtivate avatud lähtekoodiga ning kinniste AI-mudelite vahel
>white|black||9|11|br Epoch’ide võimekuse indeks (ECI) skoorid kõige paremini toimivatest avatud kaaluga (tumesinine) ja suletud (helesinine) mudelitest ajas. ECI koondab skoorid 39 testilt ühte üldise võimekuse skaalasse. Parimad avatud kaaluga mudelid jäävad suletud mudelitest maha ligikaudu ühe aasta võrra. Allikas: Epoch AI, 2025 (‡1343).


###@ Leevendusmeetmed

Avatud kaaludega mudelite riskide tehnilised maandusmeetmed toimivad kogu tehisintellekti arendus- ja kasutuselevõtu protsessi vältel (‡1141, ‡1195, ‡1347). Näiteks arenduse faasis saavad arendajad ja järeltöötluse kohandajad filtreerida treeningandmetest tundliku sisu, et minimeerida kahjulikke võimeid. Kahjulike näidete eemaldamine mudeli treeningandmetest võib vältida ründavat peenhäälestamist 10 korda tõhusamalt kui kaitsete lisamine pärast treeningut, kuigi see võib samal ajal mõjutada kasulikke võimeid (‡55). Tehisintellekti rakenduste pakkujad saavad samuti rakendada intsidentidest teavitamise ja reageerimise mehhanisme (‡1348).

Lisaks saavad majutusplatvormid, nagu HuggingFace ja GitHub, kehtestada platvormi kasutustingimused, et eemaldada mudelid, mida on muudetud kahjulikul otstarbel (‡1141, ‡1324). Mudeliarendajad saavad anda audiitoritele enne avaldamist täieliku ligipääsu või valida „etapilise” avaldamise strateegia – avaldades mudeleid järk-järgult üha suurematele sihtrühmadele (‡1086). See võib aidata tuvastada võimalikke tõrkeid või haavatavusi enne, kui mudel on laialdaselt kättesaadav (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Märkus 3.1: Mudeli kaalu turve
>oldlace|black|left|13|15|hb Märkus 3.1: Mudeli kaalu turvalisus
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Selles jaotises käsitletud riskid eeldavad, et mudeli kaalud avaldatakse tahtlikult. Kuid suletud mudeli kaalud võivad saada kättesaadavaks ka varguse või lekke kaudu. Suletud mudelite väljatöötamine maksab sadu miljoneid dollareid (§1.1. What is general-purpose AI?) ja keskmiselt on need võimekamad kui avatud-kaa lude mudelid (‡1343). See muudab need atraktiivseteks sihtmärkideks tegutsejatele alates harrastushäkkeritest kuni riikide tasandi osalejateni, kes püüavad omandada juhtivaid tehisintellekti mudeleid.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Varastatud suletud mudeli kaalud tooksid kaasa sarnased ohud, nagu eespool kirjeldatud avatud mudelite puhul, kuid potentsiaalselt ilma ühegi leevendusmeetmeta. Kuritahtlikud osalejad võiksid eemaldada kaitsed kõige võimekamatest mudelitest. Erinevalt õiguspärastest arendajatest ei peaks sellised osalejad arvestama maine-, õigus- ega kaubanduslike piirangutega, mis praegu motiveerivad tipptasemel tehisintellekti ettevõtteid oma mudeleid turvaliselt kasutusele võtma.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Turvalisuse tasemed on tööstusharude lõikes erinevad ning võivad olla ebapiisavad keerukate ründajate vastu. Mõned arendajad on võtnud kohustuse kaitsta mudeli kaalusid küberkuritegevuse sündikaatide ja siseringi ohtude eest (‡582), samas kui teised pole teinud ühtegi avalikku turvakohustust (‡1109, ‡1349). Uuringud viitavad, et tehisintellekti andmekeskused ei pruugi olla võimelised vastu pidama rünnakutele kõige keerukamate ja paremini ressurssidega varustatud osaliste poolt (‡582, ‡1350, ‡1351). Alates detsembrist 2025 ei ole kinnitatud, avalikult dokumenteeritud juhtumeid mudeli kaalu vargusest. Siiski on raporteeritud teiste turvarikkumiste kohta juhtivates tehisintellekti ettevõtetes, sealhulgas Microsofti meilisuhtluse süsteemide sissetung (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Nende turvaaukude sulgemine nõuaks märkimisväärseid investeeringuid riistvarasse, tarkvarasse, personali ja rajatiste turvalisusesse. Mõningaid turvaparandusi saaks suhteliselt kiiresti ellu rakendada koordineeritud tegevusega (‡1122). Muud olulised meetmed, nagu näiteks riistvara tarneahelate ja rajatiste kindlustamine, võtaksid aga tõenäoliselt aastaid (‡1122). Ka eraettevõtetel võivad puududa vajalikud ressursid või teave, et töötada kaitsed üksi välja piisaval tasemel. Näiteks tehisintellekti arendajatel ei ole ligipääsu salastatud ohuteabele, mis on valitsustel (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Väljakutsed poliitikakujundajatele

Poliitikakujundajate jaoks on üks peamisi väljakutseid kindlustada avatute kaalukogumite mudelite jagamisega kaasnevad hüved ilma riskide märkimisväärse suurenemiseta. Katastroofilise kahju vältimiseks ei tohiks avatute kaalukogumitega mudelite arendajad mudeleid välja anda ilma riske hindamata, nii kasutades väljakujunenud hindamismeetodeid, mida kasutatakse suletud mudelite puhul, kui ka lisatestimisega, arvestades, et pahatahtlikud osalejad saavad mudeleid peenhäälestada ja eemaldada turvakaitsed. Praktikas võib see olla keeruline, sest võimekuse arengud võivad olla ettearvamatud, avatute kaalukogumite väljalasked on pöördumatud ning hindamistoimingud on vajalikud selleks, et prognoosida, millal tooks väljalase kaasa olulise potentsiaalse kahju. Üks lähenemisviis on hinnata avatute väljalasete “piirrisk’i” (marginal risk): ulatust, mil määral suurendab väljalase vastutõsises plaanis ühiskondlikku riski võrreldes riskiga, mida juba põhjustavad olemasolevad mudelid või muud tehnoloogiad (‡556, ‡1033, ‡1354, ‡1355) (vt §3.2. Riskijuhtimise tavad). Siiski on keeruline hinnata, kuidas süsteem pärast kasutuselevõttu suurendab või vähendab järeltulevat (downstream) riski, ning see sõltub kontekstist. Riskide järkjärgulised suurenemised järjestikuste väljalasete käigus võivad aja jooksul kuhjuda märkimisväärseks kasvuks koguriski tasemes, isegi kui iga väljalaske piirrisk näib olevat aktsepteeritav (‡1356, ‡1357). AI võimekuste kahesugusus (dual-use) muudab valitsemise veelgi keerulisemaks: tunnused, mis võimaldavad kasulikke rakendusi meditsiinis või teadusuuringutes, saab suunata kahju tekitamiseks ümber ning kui kaalukogumid on avalikud, võib olla raske eristada õiguspäraseid ja pahatahtlikke kasutusviise. Samuti pole selge, kelle kanda peaks vastutus jääma, kui avatute kaalukogumitega mudeleid muudetakse kahjulikel eesmärkidel.

