##########
>white|orangered|left|14|30|hr 3.4 skirsnis
### 3.4. Atvirojo svorio modeliai
>white|orangered|left|24|30|hb Atviros prieigos modeliai

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Svarbiausia informacija
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Prieigos lygis, kurį AI įmonės suteikia savo modelių „svoriams“, turi įtakos rizikoms, kurias šie modeliai kelia. Svoriai yra matematiniai parametrai, leidžiantys AI modeliams apdoroti įvestis ir generuoti išvestis. Kiekvienam konkrečiam modeliui įmonės gali pasirinkti svorius laikyti visiškai privačius, suteikti kai kuriems vartotojams ribotą prieigą arba leisti bet kam juos atsisiųsti visiškai. Modeliai, kurių svoriai yra viešai prieinami, vadinami „open-weight models“.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Atviro svorio modeliai palengvina mokslinius tyrimus ir inovacijas, tačiau jų apsaugos gali būti lengviau pašalintos. Visame pasaulyje įvairūs veikėjai – ypač tie, kurie turi mažiau išteklių – gali naudoti atviro svorio modelius moksliniais ir komerciniais tikslais. Tačiau, palyginti su uždaro svorio modeliais, atviro svorio modelius lengviau modifikuoti taip, kad jie demonstruotų galimai žalingą elgseną, ir   sunkiau.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Atviro tipo (open-weight) modelių išleidimas yra negrįžtamas. Kai modelio svoriai yra išleisti, jų atsiimti neįmanoma. Dėl to tampa sunkiau sušvelninti galimą žalą, atsirandančią dėl modelio, turinčio pavojingų gebėjimų, išleidimo.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Nuo praėjusios ataskaitos paskelbimo (2025 m. sausis) pagrindiniai atvirojo kodo (open-weight) leidimai susiaurino galimybių atotrūkį su pirmaujančiais uždaros prieigos (closed) modeliais. Kinijos kūrėjai „DeepSeek“ ir „Alibaba“ išleido atitinkamai savo R1 ir Qwen modelius, kurie pasiekė panašų į pirmaujančius uždaros prieigos modelius našumą, o „OpenAI“ išleido pirmuosius atvirojo svorio (open-weight) modelius nuo 2019 m. Dabar pirmaujančių uždaros prieigos modelių galimybės vertinamos kaip mažesnės nei vienerių metų pranašumas, palyginti su pirmaujančiais atvirojo svorio (open-weight) modeliais pagrindiniuose AI etalonuose.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Vienas pagrindinių politikos iššūkių – pasiekti naudos, kurią atviro svorio (open-weight) modeliai teikia, kartu valdant jų išskirtinę riziką. Vienas požiūris – vertinti atviro svorio modelius pagal jų „ribinę riziką“: mastą, kuriuo jų išleidimas prieštariškai (counterfactually) padidina visuomeninę riziką, palyginti su ta, kurią jau kelia esami modeliai ar kitos technologijos. Tačiau tai praktiškai sudėtinga. Net ir nedideli ribinės rizikos padidėjimai laikui bėgant gali susikaupti ir lemti reikšmingą bendros rizikos išaugimą.
>oldlace|black||11|15|br      


Atviro kodo modeliai, kurių parametrai yra viešai prieinami atsisiuntimui, turi ryškias pasekmes daugeliui iššūkių, aptartų ankstesniuose skyriuose. Dirbtinio intelekto modelio „svoriai“ (weights) turi esminę informaciją, leidžiančią jam generuoti naudingus atsakymus vartotojams. Išleidus šiuos svorius, jų neįmanoma atsiimti: kiekvienas gali atsisiųsti, išstudijuoti, modifikuoti, dalytis ir naudoti juos savo kompiuteriuose ar debesijos paskyrose. Kai svoriai yra viešai prieinami, kiti gali lengviau kurti ant esamo modelio ir jį modifikuoti, tenkindami įvairius poreikius ir skatindami inovacijas (‡1317). Vis dėlto dėl to paties mechanizmo vartotojams, turintiems piktavalių ketinimų, taip pat tampa lengviau pašalinti apsaugos priemones ir modifikuoti atviro svorio modelius žalingiems naudojimo atvejams (‡1122, ‡1160). Dėl to kyla klausimas, ar kai kuriems atviro svorio modeliams turėtų būti taikomi specialūs reikalavimai (pvz., griežtesni testavimai prieš išleidimą), ar, priešingai, suteikiamos specialios išimtys (pvz., nuo reguliavimo ataskaitų teikimo reikalavimų) (‡1033).

###@ Atvirųjų svorių modelių kontekstas

>white|orangered||14|15.5|bb Atviro svorio modeliai gali būti, bet nebūtinai yra „atviro kodo“ modeliai

Nors dažnai vadinami „atvirojo kodo“ sprendimais, dauguma viešai išleistų modelių tiksliau apibūdinami kaip „atvirieji svoriai“ (angl. open-weight). Taip yra todėl, kad nors kūrėjai pateikia modelio svorius, jie neišleidžia susijusio mokymo kodo ar duomenų rinkinių. Be to, atvirojo kodo programinė įranga paprastai pasižymi leidimų (licencijų) tipais, kurie kelia minimalusius reikalavimus tolimesniems veikėjams, naudojantiems ar modifikuojantiems programinę įrangą (‡1318). Pavyzdžiui, „Meta“ Llama modeliams taikomos ribojančios licencijos sąlygos, o įtraukiamas tik išvados (inference) kodas, o ne mokymo kodas, todėl jie paprastai nelaikomi atvirojo kodo sprendimais (‡1319, ‡1320). Modelio išleidimo galimybės egzistuoja nuo visiškai uždaro iki visiškai atvirojo kodo spektre, o kiekviename taške taikomi skirtingi rizikos ir naudos kompromisai (‡1086*, ‡1320, ‡1321). Stalo 3.9 aprašo šias galimybes.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Visiškai uždaryta
  Vartotojai iš viso negali tiesiogiai bendrauti su modeliu
  Pavyzdžiai: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Prieiga per prieglobą
  Vartotojai gali sąveikauti tik per konkrečią programėlę ar sąsają, pavyzdžiui, mobiliosios pokalbių su AI programėlės sąsają
  Pavyzdžiai: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb Prieiga prie API modeliui
  Naudotojai gali siųsti užklausas modeliui per kodą, todėl jį galima naudoti išorinėse taikomose programose
  Pavyzdžiai: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb Prieiga prie API, skirta derinimui (fine-tuning)
  Naudotojai gali papildomai pritaikyti modelį pagal savo konkrečius poreikius
  Pavyzdžiai: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Atvirojo svorio: svoriai, prieinami atsisiuntimui
  Naudotojai gali atsisiųsti ir paleisti modelį savo kompiuteriuose
  Pavyzdžiai: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Svorio koeficientai, duomenys ir kodas prieinami atsisiuntimui su naudojimo apribojimais
  Vartotojai gali atsisiųsti ir paleisti modelį, taip pat išvadų ir mokymo kodą, tačiau taikomi tam tikri licencijos naudojimo apribojimai
  Pavyzdžiai: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Visiškai atvira: svoriai, duomenys ir kodas prieinami atsisiųsti be naudojimo apribojimų
  Naudotojai turi visišką laisvę atsisiųsti, naudoti ir modifikuoti modelį, visą kodą ir duomenis
  Pavyzdžiai: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Stalo 3.9: Modelio dalijimosi parinktys nuo visiškai uždarų iki visiškai atvirų
>white|black||9|11|br Pavyzdinis modelio dalijimosi galimybių pasirinkimas – nuo visiškai uždarų modelių (modeliai yra privatūs ir laikomi tik nuosavam, patentiniam naudojimui) iki visiškai atvirų ir atvirojo kodo modelių (modelio svoriai, duomenys ir kodas yra laisvai ir viešai prieinami be naudojimo, modifikavimo ir dalijimosi apribojimų). Modeliai, patenkantys į pirmas keturias kategorijas, dažnai vadinami „uždarais“. Šiame skyriuje dėmesys skiriamas trims apatiniams stulpeliams. Šaltinis: pritaikyta iš Bommasani, 2024 (‡1317).


###@ Privalumai ir rizikos

>white|orangered|left|14|15.5|bb Atviro kodo modeliai gali būti lengviau pritaikomi ir vertinami

Atviro kodo svorio modeliai suteikia reikšmingų privalumų moksliniams tyrimams, inovacijoms ir prieinamumui. Kaip aptarta 1.1 skyriuje „Kas yra bendrosios paskirties DI?“, bendrosios paskirties DI modelių mokymas yra itin brangus – pažangiausi modeliai kainuoja šimtus milijonų dolerių, kad būtų sukurti. Atvirai išleidžiant modelių svorius, mažiau išteklių turintys veikėjai gali juos atkartoti, tirti ir plėtoti esamas sistemas. Be tokios prieigos bendruomenės mažai išteklių turinčiuose regionuose rizikuoja būti neįtrauktos į DI naudą, todėl atviri svoriai yra kritiškai svarbūs siekiant sudaryti sąlygas globaliai daugumos dalyvauti DI kūrime (‡1322). Tolesni kūrėjai gali pritaikyti modelius (fine-tune) įvairioms reikmėms, pavyzdžiui, pritaikyti juos nepakankamai išteklių turinčioms mažumų kalboms arba optimizuoti našumą konkrečioms užduotims, tokioms kaip teisinio dokumento rengimas ar medicininių pastabų įrašymas (‡1323, ‡1324*). Tokiu būdu atviro svorio modeliai gali leisti daugiau žmonių ir bendruomenių naudotis DI bei gauti iš jo naudos, nei būtų įmanoma kitu atveju (‡1325). Kalbant apie modelius, kurie nėra pakankamai pajėgūs, kad būtų pavojingi, šie privalumai gali nusverti papildomą atvirai išleidžiamų svorių keliamą riziką, nors tai priklauso nuo atitinkamų sprendimus priimančių asmenų rizikos tolerancijos.

Atvirojo svorio išleidimas taip pat išplečia kūrėjų ir tyrėjų, galinčių tirti modelį, įvertinti jo galimybes, testuoti pažeidžiamumus ir iteratyviai diegti patobulinimus (‡1326, ‡1327), ratą. Dėl to didesnė tikimybė, kad bus identifikuotos naudingos taikymo sritys ir žalingi trūkumai, nors tai nėra užtikrinta (‡1328, ‡1329). Be to, naudotojai gali paleisti atvirojo svorio modelius savo įrenginiuose, taip išlaikydami kontrolę over jautrius duomenis ir išvengdami jų siuntimo trečiųjų šalių serveriams.

Yra papildomų privalumų, kai kūrėjai dalijasi informacija, tokia kaip mokymo duomenys, kodas, vertinimo įrankiai ir dokumentacija, taip pat modelio svoriai (‡1320, ‡1330, ‡1331, ‡1332*). Turint daugiau informacijos, tolesni kūrėjai ir kiti tyrėjai gali geriau suprasti atviro svorio modelius ir pritaikyti juos naujoms taikymo sritims.

>white|orangered|left|14|15.5|bb Atviro svorio modelių saugiklius lengviau pašalinti, todėl gali kilti potencialus piktnaudžiavimas

Atviro kodo modeliai taip pat kelia papildomų rizikų, nes jų apsaugos yra lengviau pašalinamos. Nors ir atviro, ir uždarų modelių atveju galima taikyti apsaugas, kad būtų atsisakoma vykdyti kenksmingus vartotojų prašymus, šios apsaugos atvirose svorio versijose yra kur kas lengviau pašalinamos. Kenksmingi veikėjai gali papildomai apmokyti (fine-tune) modelį, kad jis optimizuotų veikimą kenksmingiems tikslams, pašalinti kodo dalis, skirtas užkirsti kelią kenksmingam naudojimui, arba atšaukti ankstesnį saugos papildomą apmokymą (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Dėl to atvirų modelių svoriai gali sustiprinti piktnaudžiavimo rizikas, aptartas §2.1. Rizikos dėl piktnaudžiavimo kenkėjiškais tikslais, nes leidžiama daugiau veikėjų pasinaudoti ir išplėsti esamus gebėjimus kenksmingiems tikslams, netaikant priežiūros (‡1122, ‡1315). Nors daugelis naudotojų neturės įgūdžių arba paskatos pašalinti apsaugas atviruose modeliuose, išlieka susirūpinimas dėl labai motyvuotų kenkėjiškų veikėjų. Be to, kenkėjiški veikėjai taip pat gali pasinaudoti atvirų svorio modeliais, kad identifikuotų pažeidžiamumus panašiuose uždaruose modeliuose (‡1055*). Tokius trūkumus sunkiau aptikti vien tik paleidžiant uždarus modelius, nes uždarų modelių teikėjai gali įgyvendinti didesnę kontrolę ir stebėsenos priemones.

>white|orangered|left|14|15.5|bb Modelio svorių dalijimasis yra negrįžtamas

Kai modelio svoriai tampa prieinami viešam atsisiuntimui, nebėra būdo įgyvendinti visuotinio visų esamų kopijų atsaukties (rollback). Interneto talpinimo platformos, tokios kaip GitHub ir Hugging Face, gali pašalinti modelius iš savo platformų, todėl kai kuriems veikėjams tampa sunkiau rasti atsisiunčiamas kopijas, ir tai sukuria reikšmingą barjerą daugeliui atsitiktinių blogų veiksmų vykdytojų (‡1339). Vis dėlto motyvuoti veikėjai vis dar gali gauti kopijas, jei modelis buvo atsisiųstas ir per talpintą iš naujo arba saugomas lokaliai. Be to, tolesni kūrėjai, kurie integruoja atviro svorio modelius į savo sistemas, taip pat perima bet kokius trūkumus, pavyzdžiui, pažeidžiamumus, susijusius su priešiškomis atakomis (‡1055), arba modelio gebėjimus apeiti stebėsenos sistemas (žr. §2.2.2. Kontrolės praradimas) (‡1315). Skirtingai nuo uždarų modelių, kai prieglobos paslaugų teikėjai gali visapusiškai diegti pataisas, atviro svorio modelių kūrėjai negali užtikrinti, kad atnaujinimai bus priimti naudotojų.

###@ Atnaujinimai

Nuo paskutinės ataskaitos paskelbimo (2025 m. sausis) lyderiaujančių atviro svorio ir uždarų modelių gebėjimų atotrūkis sumažėjo. Ypač svarbiais atviro svorio modelių tiekėjais tapo Kinijos kūrėjai. 2025 m. sausį „DeepSeek“ išleido savo R1 modelį, kuris daugelyje vertinimo kriterijų (‡1340) pasiekė panašų našumą kaip „OpenAI“ o1. „Alibaba“ „Qwen“ modeliai taip pat įgijo pagreitį – nuo 2025 m. rugpjūčio jie užėmė pirmąją vietą „Chatbot Arena“ (plačiai naudojamas našumo vertinimo kriterijus) tarp atviro svorio modelių (‡1341, ‡1342*). 2025 m. rugpjūčio mėn. „OpenAI“ išleido pirmuosius atviro svorio modelius nuo GPT-2 išleidimo 2019 m. – „gpt-oss-120b“ ir „gpt-oss-20b“. „Meta“ toliau leidžia „Llama“ modelius su atviromis svorio reikšmėmis. Šiuo metu lyderiaujančių uždarų modelių galimybės, vertinant pagal reikšmingus AI vertinimo kriterijus, prognozuojamos kaip mažiau nei vienerių metų pranašumas palyginti su lyderiaujančiais atviro svorio modeliais (Figūra 3.10).

###@ Įrodymų spragos

Svarbiausias įrodymų spragos aspektas susijęs su realaus pasaulio veiksmingumu, t. y. ar techniniai sprendimai iš tiesų gali užkirsti kelią netinkamam atvirų svorių modelių naudojimui. Tyrėjai pasiūlė įvairių metodų, kaip padaryti modelius atsparius tamperinimui. Tai apima naujas mokymo technikas, skirtas tam, kad modeliai būtų atsparūs žalingam modifikavimui (‡1276), žalingo turinio filtravimą iš mokymo duomenų (‡55) ir gynybą nuo jailbreak’ų (‡675, ‡676). Šios technikos dabar diegiamos realaus pasaulio išleidimuose iš didžiųjų kūrėjų. Pavyzdžiui, OpenAI taikė kai kurias iš šių technikų savo gpt-oss modeliuose, pranešdama, kad adversarially fine-tuned versijos nepasiekė aukštų gebėjimų slenksčių (‡1344*). Vis dėlto tyrimai parodė, kad blogi veikėjai gali išjungti saugiklius, perkurdami modelius žalingais pavyzdžiais (‡1345, ‡1346). Be to, vis dar sudėtinga patikimai įvertinti saugiklių atsparumą, todėl jų veiksmingumas prieš atakas realiame pasaulyje išlieka neaiškus (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Figūra 3.10: Pajėgumų spraga tarp pirmaujančių atvirojo svorio ir uždarų AI modelių
>white|black||9|11|br Epoch Capabilities Index (ECI) įverčiai geriausiai pasirodžiusių atviro svorio (tamsiai mėlyna) ir uždarų (šviesiai mėlyna) modelių laikui bėgant. ECI sujungia 39 vertinimo kriterijų įverčius į vieną bendrų gebėjimų skalę. Geriausi atviro svorio modeliai atsilieka maždaug vienerius metus nuo uždarų modelių. Šaltinis: Epoch AI, 2025 (‡1343).


###@ Šalinimai

Techninės priemonės atviros prieigos svorių modelių keliamoms rizikoms mažinti veikia viso AI kūrimo ir diegimo proceso metu (‡1141, ‡1195, ‡1347). Pavyzdžiui, kai modeliai kuriami, kūrėjai ir tolesni adapteriai gali filtruoti jautrų turinį iš mokymo duomenų, kad sumažintų žalingas galimybes. Pašalinus žalingus pavyzdžius iš modelio mokymo duomenų, galima užkirsti kelią priešiškam tolesniam mokymui 10 kartų efektyviau nei taikant gynybą, pridėtą po mokymo, nors tai taip pat gali paveikti naudingas galimybes (‡55). AI taikomųjų programų teikėjai taip pat gali įdiegti incidentų pranešimo ir reagavimo mechanizmus (‡1348).

Be to, prieglobos platformos, tokios kaip HuggingFace ir GitHub, gali nustatyti platformos naudojimo sąlygas, kad būtų pašalinti modeliai, modifikuoti kenksmingiems tikslams (‡1141, ‡1324). Modelių kūrėjai gali suteikti auditoriųams visišką prieigą prieš išleidimą arba pasirinkti „pakopinio“ išleidimo strategiją – išleisti modelius palaipsniui vis didesnėms grupėms (‡1086). Tai gali padėti nustatyti galimus veikimo sutrikimus ar pažeidžiamumus prieš modeliui tapus plačiai prieinamam (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ 3.1 dėžutė: Modelio svorio saugumas
>oldlace|black|left|13|15|hb Pastaba 3.1: Modelio svorio saugumas
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Šiame skyriuje aptariamos rizikos daro prielaidą, kad modelio svoriai išleidžiami sąmoningai. Tačiau uždari modelio svoriai taip pat gali tapti prieinami dėl vagystės ar nutekėjimo. Uždari modeliai kainuoja šimtus milijonų dolerių, kad būtų sukurti (§1.1. Kas yra bendros paskirties dirbtinis intelektas?), ir vidutiniškai yra pajėgesni už atviro svorio modelius (‡1343). Dėl to jie tampa patraukliais taikiniais veikėjams nuo mėgėjiškų įsilaužėlių iki valstybių, siekiančių gauti pažangiausius AI modelius.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Pavogti uždarojo modelio svorio failai keltų rizikas, panašias į tas, kurios aprašytos aukščiau atvirų svorių modeliams, tačiau galbūt be jokių sušvelninimų. Kenkėjiški veikėjai galėtų pašalinti apsaugos priemones iš pačių pajėgiausių modelių. Skirtingai nei teisėti kūrėjai, tokie veikėjai nesusidurtų su reputacijos, teisiniais ar komerciniais suvaržymais, kurie šiuo metu skatina pažangiausio AI bendroves diegti savo modelius saugiai.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Dabartiniai saugumo lygiai skiriasi visoje pramonėje ir gali būti nepakankami prieš išmanius atakuotojus. Kai kurie kūrėjai įsipareigoja apsaugoti modelių svorius nuo kibernetinių nusikaltėlių sindikatų ir vidinių grėsmių (‡582), o kiti nebuvo pateikę jokių viešų saugumo įsipareigojimų (‡1109, ‡1349). Tyrimai rodo, kad AI duomenų centrai gali nesugebėti atlaikyti atakų, kurias vykdo patys išmaniausi ir gerai ištekliais aprūpinti veikėjai (‡582, ‡1350, ‡1351). Nuo 2025 m. gruodžio nėra patvirtintų, viešai dokumentuotų modelių svorių vagystės atvejų. Tačiau buvo pranešta apie kitas saugumo spragas pirmaujančiose AI įmonėse, įskaitant įsiskverbimą į Microsoft el. pašto sistemas (‡1352).
>oldlace|black||11|15|br      
00000140244775356544|Šių saugumo spragų uždarymas pareikalautų didelių investicijų į aparatinę įrangą, programinę įrangą, personalą ir patalpų saugumą. Kai kuriuos saugumo patobulinimus būtų galima įgyvendinti palyginti greitai, koordinuojant veiksmus (‡1122). Tačiau kitos svarbios priemonės, tokios kaip aparatūros tiekimo grandinių ir patalpų apsaugojimas, greičiausiai užtruktų kelerius metus (‡1122). Privatūs
verslai taip pat gali neturėti išteklių ar informacijos, kad vieni galėtų sukurti tinkamas apsaugas. Pavyzdžiui, AI kūrėjai neturi prieigos prie įslaptintos grėsmių žvalgybos, kurią turi vyriausybės (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Iššūkiai politikos formuotojams

Pagrindinis politikos formuotojų iššūkis – užtikrinti atviro svorio (open-weight) modelių dalijimosi teikiamą naudą, nepagažiai nepadidinant rizikos. Kad būtų išvengta katastrofiškos žalos, atviro svorio modelių kūrėjai neturėtų išleisti modelių neįvertinę rizikų, taikydami ir nusistovėjusius vertinimo metodus, naudojamus uždaro svorio (closed) modeliams, ir papildomus testus, atsižvelgiant į tai, kad blogi veikėjai (bad actors) gali papildomai tobulinti (fine-tune) modelius ir pašalinti saugos apsaugas. Praktikoje tai gali būti sudėtinga, nes gebėjimų (capability) tobulėjimas gali būti nenuspėjamas, atviro svorio išleidimai yra negrįžtami, o vertinimo pastangos reikalingos tam, kad būtų galima prognozuoti, kada išleidimas kelia reikšmingą potencialią žalą. Vienas požiūris – įvertinti atvirų išleidimų „ribinę riziką“ (marginal risk): mastą, kuriuo išleidimas kontrfaktiškai padidina visuomeninę riziką, palyginti su rizika, kurią

5

5

5

57) (žr. §3.2. Rizikos valdymo praktikos). Tačiau prognozuoti, kaip sistema padidins ar sumažins riziką vėlesnėje grandyje po to, kai ji bus įdiegta, yra sudėtinga ir priklauso nuo konteksto. Laipsniški rizikos didėjimai su kiekvienu nauju išleidimu gali laikui bėgant sudaugėti į reikšmingus bendros rizikos padidėjimus, net jei kiekvieno konkretaus išleidimo ribinė rizika atrodo priimtina (‡1356, ‡1357). Dvigubo panaudojimo (dual-use) AI gebėjimų pobūdis dar labiau apsunkina valdymą: savybės, leidžiančios naudingus pritaikymus medicinoje ar moksliniuose tyrimuose, gali būti pernaudotos žalai, o kai svoriai (weights) tampa vieši, atskirti teisėtus nuo kenkėjiškų panaudojimų gali būti sunku. Taip pat neaišku, kas turėtų būti laikomas atsakingu, kai atviro svorio modeliai modifikuojami siekiant žalos.

