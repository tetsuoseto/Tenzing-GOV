##########
>white|orangered|left|14|30|hr 3.3 skyrius
### 3.3. Techninės apsaugos priemonės ir stebėsena
>white|orangered|left|24|30|hb Techninės apsaugos priemonės ir stebėsena

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Svarbiausia informacija
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Plačiu spektru techninių apsaugos priemonių naudojama skirtingais AI kūrimo ir naudojimo etapais. Tai apima metodus, taikomus modelio kūrimo metu, siekiant, kad sistemos būtų patvaresnės ir atsparios piktnaudžiavimui (pvz., duomenų atranka), diegimo metu atliekamą stebėseną ir kontrolę (pvz., turinio filtravimą ir žmogišką priežiūrą) bei po diegimo naudojamus įrankius platesnei AI ekosistemos stebėsenai (pvz., kilmės nustatymą ir turinio aptikimą).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Techninės apsaugos priemonės turi ribotumų ir nepatikimai užkerta kelią žalingam elgesiui visais atvejais. Pavyzdžiui, naudotojai kartais gali gauti žalingus atsakymus perfrazuodami užklausas arba suskaidydami jas į mažesnius veiksmus. Panašiai, tokios priemonės kaip vandens ženklinimas, kurios skirtos identifikuoti dirbtinio intelekto sugeneruotą turinį, dažnai gali būti pašalinamos arba pakeistos, todėl jų patikimumas mažėja.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Individualių apsaugos priemonių ribotumas reiškia, kad tam tikriems žalingiems rezultatams išvengti gali prireikti „gynybos sluoksniais“ (defence-in-depth). Pavyzdžiui, sistema gali sujungti saugai pritaikytą modelį su įvesties filtrais, išvesties filtrais ir turinio stebėsenos priemonėmis.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Nuo paskutinės Ataskaitos paskelbimo (2025 m. sausis) tyrėjai padarė pažangą tobulindami apsaugos priemones, tačiau išlieka esminiai apribojimai. Pavyzdžiui, atakų, skirtų apsaugos priemonėms apeiti, sėkmės rodiklis mažėjo, bet vis dar išlieka gana aukštas. Taip pat yra esminių apribojimų, kiek nuodugniai atvirojo svorio modeliai gali būti apsaugoti.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Pagrindinis politikos formuotojų iššūkis yra riboti įrodymai, kaip veiksmingos apsaugos priemonės yra įvairiuose realiuose bendrosios paskirties AI sistemų naudojimo atvejais. AI kūrėjai labai skiriasi tuo, kiek informacijos jie dalijasi apie savo apsaugos priemones ir stebėseną. Kitas iššūkis – galimi kompromisai tarp griežtesnių apsaugos priemonių taikymo ir sistemos našumo arba naudingumo išlaikymo.
>oldlace|black||11|15|br      


Dirbtinio intelekto kūrėjai gali naudoti kelias naudingas, bet netobulas technines apsaugos priemones, kad mažintų ir valdytų rizikas, kylančias iš bendrosios paskirties dirbtinio intelekto sistemų, tačiau išlieka atsparumo (robustumo) iššūkiai. Kūrėjai vis dar negali visiškai užkirsti kelio bendrosios paskirties dirbtinio intelekto sistemoms atlikti net gerai žinomus ir akivaizdžiai žalingus veiksmus, pavyzdžiui, pateikti naudotojams instrukcijas, kaip įvykdyti nusikaltimus. Pavyzdžiui, tyrėjai parodė, kad pažangiausias apsaugas galima apeiti naudojant priešiškus raginimo (prompt) metodus (t. y. „jailbreaks“) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), kai modeliai suskaido sudėtingas žalingas užduotis į žingsnius (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), ir pasitelkiant paprastus modelio pakeitimus (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Tyrėjai ir toliau dirba kurdami apsaugas nuo gedimų (malfunction) ir netinkamo naudojimo (‡690). Šie metodai labai skiriasi savo paskirtimi ir veiksmingumu, o jų poveikis galiausiai priklauso nuo platesnio socialtechninio ir valdymo konteksto, kuriame dirbtinio intelekto sistemos yra kuriamos ir diegiamos.

Techninės apsaugos gali būti plačiai suskirstytos į tris kategorijas: metodai, skirti kurti saugesnius modelius; metodai, naudojami diegimo metu stebėsenai ir kontrolei; ir metodai, kurie palaiko stebėsenos ekosistemos stebėjimą po diegimo. Stalo 3.6 apibendrina aptartas technines apsaugas, jų veiksmingumą ir atvirus iššūkius.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Kuriant saugesnius modelius
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Duomenų tvarkymas (‡1167)
  Kenksmingų duomenų pašalinimas, kad modelis neišmoktų pavojingų gebėjimų. Šie metodai gali būti naudingi, įskaitant kuriant atviro svorio modelius, kurie neturi kenksmingų gebėjimų ir atsparūs kenksmingam papildomam mokymui (‡55). Tačiau yra iššūkių dėl atrankos (kuravimo) klaidų ir mastelio didinimo (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Stiprinamasis mokymasis iš žmogaus grįžtamojo ryšio (‡64*)
  Mokyti modelį atitinkamai nurodytais tikslais, pavyzdžiui, būti naudingam ir nekenksmingam. Tai veiksmingas būdas priversti modelius išmokti naudingų elgsenų (‡64*). Tačiau per didelis optimizavimas siekiant žmonių pritarimo gali priversti modelius elgtis apgaulingai arba pataikaujant (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Plurališkos lygiavimo technikos (‡1170)
  Mokymas modelį integruoti kelias skirtingas perspektyvas dėl to, kaip jis turėtų elgtis. Šios technikos padeda sumažinti mastą, kuriuo modeliai teikia pirmenybę konkrečioms perspektyvoms (‡1170). Tačiau nepaisant šių technikų, žmogaus nesutarimai yra neišvengiami, ir sunku sukurti plačiai pripažįstamus būdus, kaip subalansuoti konkuruojančias perspektyvas (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adversarinis mokymas (‡677)
  Modelio mokymas atsisakyti daryti žalos (net ir neįprastose situacijose) ir atsispirti išpuoliams, kuriuos vykdo piktybiški naudotojai (pvz., „jailbreaks“). Tai veiksmingas metodas, padedantis modeliams atsispirti bandymams piktnaudžiauti (‡1064), tačiau atsparumo iššūkiai išlieka (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mašinos „užmiršimas“ (‡1175, ‡1176)
  Mokymo modelis naudojant specializuotus algoritmus reiškia aktyviai slopinti žalingus gebėjimus (pvz., žinias apie biologinius pavojus). Šios technikos suteikia tikslingą būdą pašalinti iš modelių žalingus gebėjimus (‡1175, ‡1176), tačiau dabartiniai neatmokymo (unlearning) algoritmai gali būti nepatikimi ir turėti nenumatytų poveikių kitiems gebėjimams (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Interpretavimo ir saugumo patikros įrankiai (‡1177)
  Įvairi dizaino ir patikros metodų šeima, skirta suteikti griežtesnį patikinimą, kad modeliai turi konkrečių su sauga susijusių savybių. Ji leidžia vertintojams užtikrinti didesnio pasitikėjimo saugos garantijas (‡1177), tačiau dabartiniai metodai remiasi prielaidomis ir praktikoje retai pasižymi konkurencingu našumu (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Stebėsena ir valdymas
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Aparatine įranga paremtos stebėsenos mechanizmai (‡1179, ‡1180, ‡1181)
  Patvirtinama, kad įgalioti procesai veikia aparatūroje, siekiant ištirti saugumo grėsmes arba laikytis reguliavimo reikalavimų. Šie mechanizmai suteikia išskirtinių būdų stebėti, kokie skaičiavimai yra vykdomi aparatūroje ir kieno atliekami (‡1181). Tačiau aparatinės įrangos mechanizmai negali stebėti visų rūšių grėsmių, o kai kurioms technikoms reikalinga specializuota aparatūra (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vartotojo sąveikos stebėjimo įrankiai (‡1154, ‡1166)
  Stebėti naudotojų sąveikas dėl kenkėjiško naudojimo požymių gali padėti kūrėjams nutraukti paslaugą kenkėjiškai besinaudojantiems naudotojams (‡1154, ‡1166). Tačiau taikymas gali netyčia trukdyti naudingu saugos tyrimams (‡689), o kai kurios piktnaudžiavimo formos yra sunkiai aptinkamos (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vartotojo sąveikos stebėjimas (‡1154, ‡1166)
  Naudotojų sąveikų stebėjimas dėl kenkėjiško naudojimo požymių gali padėti kūrėjams nutraukti paslaugą kenkėjiškai besinaudojantiems naudotojams (‡1154, ‡1166). Tačiau vykdymo priemonės gali netyčia trukdyti naudingiems saugos tyrimams (‡689), o kai kurios piktnaudžiavimo formos yra sunkiai aptinkamos (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Turinio filtrai (‡65*, ‡725)
  Filtruoti potencialiai žalingus modelio įvesties ir išvesties duomenis yra labai veiksmingas būdas sumažinti atsitiktinės žalos ir piktnaudžiavimo rizikas (‡725). Tačiau filtrai reikalauja papildomo skaičiavimo resursų ir yra pažeidžiami kai kurių atakų (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modelio vidiniai skaičiavimų monitoriai (‡744, ‡1183, ‡1184)
  Modelių apgaulės požymių ar kitų žalingų vidinių pažinimo formų stebėsena gali būti efektyvus būdas aptikti apgaulę (‡744, ‡1183, ‡1184). Tačiau esami metodai pasižymi nepakankamu patikimumu ir tvirtumu (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pagrindimo grandinės stebėsenos priemonės (‡430, ‡435)
  Modelio „chain-of-thought“ (mąstymo grandinės) teksto stebėjimas dėl apgaulingo elgesio požymių arba kito žalingo samprotavimo yra veiksmingas būdas suprasti ir pastebėti trūkumus, kaip modeliai samprotauja (‡435). Tačiau tai gali būti nepatikima (‡752, ‡753, ‡1186), o jei modeliai yra mokomi generuoti gerybinį „chain of thought“, jie gali išmokti apgaulingą elgesį (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Žmogus kilpoje (‡1187, ‡1188, ‡1189)
  Žmogiška priežiūra ir sistemos sprendimų nepaisymo galimybės yra būtinos kai kuriose su sauga susijusiose kritinėse taikomosiose srityse (‡1187). Tačiau šias technikas riboja automatizavimo šališkumas ir žmogaus sprendimų priėmimo greičio ribos (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Smėliavimas (‡1192)
  Dirbtinio intelekto agento neleidimas tiesiogiai daryti įtakos pasauliui yra veiksmingas būdas apriboti žalą, kurią jis gali sukelti (‡1192). Tačiau sandboxingas (izoliavimas smėlio dėžėje) riboja sistemos galimybes tiesiogiai atlikti tam tikras užduotis (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Įrankiai ekosistemos stebėsenai palengvinti
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb AI modelių identifikavimo metodai (‡1193*, ‡1194)
  Modelius, arba atskirus modelių egzempliorius, lengviau atpažinti realaus pasaulio naudojimo atvejais padeda atliekant skaitmeninę forensiką ir didinant ekosistemos suvokimą (‡1195). Tačiau šias technikas galima apeiti atlikus tam tikrus modelio pakeitimus (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb AI modelio paveldo atvaizdavimas (‡1197)
  Šios technikos leidžia tyrėjams ištirti, kaip modeliai yra keičiami AI ekosistemoje, ypač atviro svorio (open-weight) modeliuose. Jos padeda skaitmeninei kriminalistikai ir ekosistemos išmanymui (‡1198), tačiau reikėtų didelio masto projektų, kad būtų kruopščiai išt kartografuota atviro svorio modelių ekosistema (‡1198).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vandens ženklai ir metaduomenys (‡1199, ‡1200, ‡1201*)
  Šios technikos palengvina nustatyti, kada tam tikras tekstas, vaizdas, vaizdo įrašas ir t. t. buvo sugeneruotas naudojant AI arba modifikuotas, ir kokia sistema tai atliko. Jos palengvina geresnį ekosistemos suvokimą (‡1199, ‡1200, ‡1201*). Tačiau vandens ženklus ir metaduomenis galima suklastoti arba pašalinti taikant tam tikrus turinio pakeitimus (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb AI sugeneruoto turinio aptikimas (‡1203, ‡1204, ‡1205*)
  Gerėjimo, kai vartotojai gali atskirti AI sugeneruotą ir tikrą turinį, stiprinimas padeda skaitmeninei forensikai ir ekosistemos suvokimui (‡1203, ‡1204). Tačiau klasifikatoriai gali būti nepatikimi (‡1205*) ir jų veikimas gali skirtis tarp skirtingų modalumų.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.6 lentelė: Šioje dalyje aptartos techninės apsaugos priemonės
>white|black||9|11|br Šioje dalyje aptartų techninių saugiklių santrauka, suskirstyta į metodus, skirtus kurti saugesnius modelius, stebėsenos ir kontrolės priemones diegimo metu, ir technikas ekosistemos stebėsenai palengvinti.


###@ Kuriant saugesnius modelius

Pirmoji gynybos linija nuo žalos, kurią gali sukelti bendrosios paskirties AI sistemos, yra padaryti pagrindinį modelį saugesnį. Šis poskirsnis aprašo apsaugos priemones, kurios „įdiegtos modelio parametrų lygyje“ modeliavimo kūrimo proceso metu (Figūra 3.6).

>white|orangered|left|14|15.5|bb Kuravimo būdu atrinkti mokymo duomenys gali apriboti potencialiai pavojingų gebėjimų vystymą

Bendrosios paskirties AI modeliai yra naudingi būtent dėl to, kad apdoroję mokymo duomenis jie sukuria platų žinių ir gebėjimų spektrą, tačiau kai kurie mokymo duomenų tipai neproporcingai prisideda prie galimai pavojingų gebėjimų ugdymo. Pavyzdžiui, AI modelis, parengtas virusologijos straipsniais, gali geriau gebėti suteikti pagalbą potencialiai žalingoms biologinėms užduotims (‡549, ‡1206*) (taip pat žr. §2.1.4. Biologinės ir cheminės rizikos). Be to, vaizdų / vaizdo generatoriai, apmokyti pagal žmogaus nuogybės vaizdus, taip pat gali būti piktnaudžiaujami kuriant neprieštaraujančius intymius deepfake’us (‡308, ‡319) (taip pat žr. §2.1.1. AI generuotas turinys ir nusikalstama veikla).

Treniruotės duomenų filtravimas yra veiksminga šalinimo priemonė nuo kai kurių nepageidaujamų gebėjimų (‡319, ‡1167, ‡1207, ‡1208). Tačiau gali būti sunku filtruoti didelius rinkinius, naudojamus bendros paskirties dirbtinio intelekto modeliams mokyti (‡1168), dėl didelių sąnaudų (‡1209), filtravimo klaidų (‡1210) ir neigiamo poveikio duomenų rinkinio kokybei (‡1211). Šie iššūkiai dar labiau sustiprėja dėl daugiakalbės interneto teksto prigimties (‡1212), kultūrinių turinio moderavimo paklaidų (‡1211, ‡1213, ‡1214, ‡1215) ir to, kad tai, ar konkretūs duomenys yra „žalingi“, priklauso nuo kontekstinių veiksnių (‡1216). Vis dėlto potencialiai žalingos medžiagos filtravimas iš treniruotės duomenų rodo pažadą, kad modeliai taptų patikimiau saugūs, įskaitant tai, kad atviros prieigos (open-weight) modeliai būtų atsparesni žalingam sugadinimui (‡55). Ryšiai tarp treniruotės duomenų turinio ir išryškėjančių modelio gebėjimų dar nėra visiškai suprasti (‡1195), o filtravimas, regis, yra veiksmingesnis ribojant žalingus gebėjimus, kai taikomas plačioms žinių sritims (‡55), palyginti su siauresniu elgesiu (‡1206, ‡1217). Žr. §3.4 skyrių. Daugiau aptarimo pateikiama apie atviros prieigos (open-weight) modelius.

![figure 3.6](images/fig3.6_safeguards.png)

##### Figūra 3.6: Kur taikyti technines apsaugos priemones
>white|black||9|11|br Techninės apsaugos gali būti taikomos skirtingais modelio kūrimo etapais. Duomenų paruošimas formuoja, ko modeliai mokosi per išankstinį mokymą ir tikslinimą (fine-tuning). Mokymu pagrįsti metodai, tokie kaip sustiprinimo mokymasis iš žmogaus grįžtamojo ryšio ir patikimumo mokymas, koreguoja modelio elgseną. Testavimo metodai, pavyzdžiui, priešiškos atakos, identifikuoja likusias pažeidžiamybes. Kai kurios technikos, tokios kaip į saugumą orientuoti (safe-by- design) algoritmai, apima kelis etapus. Šaltinis: Tarptautinė AI saugos ataskaita 2026.


>white|orangered|left|14|15.5|bb Bendrosios paskirties AI modelių mokymo metodai, skirti tam, kad jie būtų naudingi ir nekenksmingi, daugiausia remiasi žmogaus grįžtamuoju ryšiu.

Sunku treniruoti ir įvertinti modelius, kad jie patikimai atitiktų aukšto lygio principus, tokius kaip naudingumas, nekenksmingumas ir sąžiningumas. Praktikoje kūrėjai siekia to pasiekti tikslindami AI modelius naudodami demonstracijas ir žmonių grįžtamąjį ryšį. Pavyzdžiui, pagrindinė AI modelių tikslinimo paradigma, žinoma kaip „mokymasis pagal žmogaus grįžtamąjį ryšį“, grindžiama mokymu, kad modeliai generuotų išvestis, kurias žmogaus anotatoriai įvertina teigiamai (‡1218). Tačiau teigiamas žmonių grįžtamasis ryšys yra ydingas naudingam elgesiui tinkamas pakaitalas (‡737, ‡878, ‡1219, ‡1220) ir yra ribojamas žmogaus klaidų bei šališkumo (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Dėl to kyla kelios problemos: modeliai, kurie buvo papildomai mokomi pagal pastiprinimo mokymąsi iš žmogaus grįžtamojo ryšio, kartais pataikauja vartotojui, t. y. elgesys, žinomas kaip „pataikūniškumas“ (‡358, ‡740, ‡1226, ‡1227); pateikia atsakymus, kurie kai kuriuose kontekstuose yra naudingi, bet kitur žalingi (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); pateikia atsakymus, kuriuos sunku įvertinti dėl teisingumo (‡1233); arba atlieka veiksmus, kurių naudingumas ar žalingumas priklauso nuo nuomonės (‡1234). Stalo 3.7 pateikia šių problemų pavyzdžius. Kai kurie tyrimai siekia sukurti metodus, padedančius žmonėms geriau įvertinti sudėtingų užduočių sprendimus su AI pagalba (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Tačiau šie metodai šiuo metu pasižymi ribotu patikimumu, o tai, kokiu mastu jie naudojami šiandien pažangiausių AI modelių mokymui, viešai nežinoma.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Išsitepimas/lošimas (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Paaiškinimas:
>white|black|left|11|13|br Modelis teikia tik teigiamą grįžtamąjį ryšį, neįvardydamas teisingos 5-7-5 haiku skiemenų struktūros trūkumo.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kai kurie veiksmai yra naudingi kai kuriuose kontekstuose, bet žalingi kituose (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Paaiškinimas:
>white|black|left|11|13|br Informacija apie biologinę riziką gali būti naudojama švietimui ir gynybai, bet taip pat siekiant informuoti kenkėjiškus veikėjus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tinkamą elgesį sunku patikrinti (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Paaiškinimas:
>white|black||11|13|br Šio atsakymo teisingumą sunku įvertinti, nes tam reikalinga medicininė kvalifikacija. Net patyrusiam gydytojui, vertinant tokio pobūdžio atsakymus, reikia laiko ir atidaus dėmesio detalėms.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Žmonės nesutaria dėl to, kas yra teisinga (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Paaiškinimas:
>white|black|left|11|13|br Žmonės reikšmingai nesutaria dėl to, koks atsakymas yra teisingas.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Stalo 3.7: Vartotojo užklausa ir AI modelio atsakymas
>white|black||9|11|br Pavyzdžiai iššūkių, susijusių su AI modelių naudingų veiksmų nurodymu ir skatinimu.


>white|orangered|left|14|15.5|bb Žmonės ne visada sutaria, kokie elgesio būdai yra pageidautini, todėl reikia metodų, kurie subalansuotų konkuruojančius pageidavimus

Žmonės ne visada sutaria dėl to, kokius atsakymus ar veiksmus AI modeliai turėtų arba neturėtų pateikti (‡1006). Dėl to iš esmės sudėtinga kurti modelius, kurių veiksmai ir poveikis būtų plačiai suderinti su visuomenės interesais (‡420). Kai kurie tyrėjai nagrinėja, kurių pageidavimai atsispindi AI sistemose (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249), ir kuria „pliuralistinio suderinimo“ (pluralistic alignment) metodus, kuriais siekiama rasti pusiausvyrą tarp konkuruojančių pageidavimų (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Pavyzdžiui, AI kūrėjai gali suprojektuoti sistemas, kad jos nevykdytų kontroversiškų atsakymų generavimo atsisakydamos reaguoti į tam tikrus prašymus, arba suderinti su vidurine nuomone tam tikrame atitinkamų žmonių pavyzdyje, arba personalizuoti sistemas atskiriems naudotojams.

Dažnas šių požiūrių iššūkis yra tas, kad apskritai AI sistemos negali vienodai suderėti su kiekvieno pageidavimais, o jų tolesnis poveikis visuomenei skirtingoms žmonių grupėms pasireikš nevienodai. Kai kurie tyrėjai teigė, kad dauguma techninių pliuralistinio suderinimo (alignment) požiūrių neadresuoja ir galbūt net nukreipia nuo gilesnių iššūkių, tokių kaip sisteminiai šališkumai (biases), socialinės galios dinamika ir turto bei įtakos koncentracija (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb Dirbtinio intelekto kūrėjai naudoja „adversarial training“ , kad pagerintų modelio atsparumą

Užtikrinti, kad AI modeliai patikimai perduotų naudingą elgseną, kurią jie išmoksta mokymo metu, į realaus pasaulio diegimo kontekstus, yra sudėtinga. Net modeliai, apmokyti pagal „tobulą“ mokymosi signalą, gali nesugebėti sėkmingai generalizuoti į visus neregėtus kontekstus (‡738, ‡739, ‡1255, ‡1256, ‡1257). Pavyzdžiui, kai kurie tyrėjai nustatė, kad pokalbių robotai dažniau imasi žalingų veiksmų kalbose, kurios yra menkai atstovaujamos jų mokymo duomenyse (‡159, ‡880, ‡1258*, ‡1259), įskaitant daug kalbų, daugiausia vartojamų Globaliojo Pietų regione.

Pastaraisiais metais tyrėjai taip pat sukūrė didelį „adversarial attack“ (adversarinės atakos) metodų rinkinį, kurį galima naudoti tam, kad modeliai generuotų potencialiai žalingus atsakymus (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Pavyzdžiui, neseniai vykdyta iniciatyva pasitelkė minią ir surinko daugiau nei 60,000 įvairių pavyzdžių, kaip sėkmingai įvykdyti atakas prieš pažangiausius AI modelius, dėl kurių jie pažeidė savo įmonių politiką dėl priimtino modelių elgesio (‡1149). 3.8 Stalo pavyzdžiuose pateikiamos „jailbreak“ (pertrūkio) technikos, kurias tyrėjai parodė, kad gali priversti modelius vykdyti žalingus prašymus.

Vienas iš metodų, padedančių didinti modelių atsparumą, vadinamas „adversariniu mokymu“ (‡1064). Jis apima „atakų“ (pvz., jailbreakų) konstravimą, skirtą priversti modelį elgtis nepageidaujamai, ir modelio mokymą tinkamai tvarkyti šias atakas. Tačiau adversarinis mokymas yra netobulas (‡1260, ‡1261). Užpuolikai nuolat sugeba sukurti naujas sėkmingas atakas prieš pažangiausius (state-of-the-art) modelius (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Kadangi kūrėjams reikia konkrečių nesėkmės režimų (failure modes) pavyzdžių, kad jie galėtų mokytis kovoti su jais (‡512, ‡1263), rezultatas yra nuolatinis „katės ir pelės“ žaidimas, kuriame kūrėjai nuolat atnaujina modelius reaguodami į naujai atrastas pažeidžiamybes, o priešininkai nuolat ieško naujų atakų. Kai kurie tyrėjai siūlė didesnio masto adversarinį mokymą (‡1264, ‡1265) arba naujus algoritmus (‡675, ‡676, ‡1263, ‡1266, ‡1267), kad būtų geriau didinamas atsparumas, tačiau šiuolaikinės AI sistemos išlieka nuolat pažeidžiamos.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategija: Kurkite žalingus prašymus šifruotu tekstu, pvz., morzės abėcėle (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategija: paruoškite sistemą pavyzdžiais, kaip atitinkančiai reaguoti į žalingus prašymus (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategija: Pateikite žalingus prašymus mažai išteklių turinčiomis kalbomis, kurios greičiausiai bus rečiau naudojamos mokymuose (pvz., svahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategija: Skaidykite žalingą užduotį į kelias nekaltas smulkesnes užduotis (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.8 lentelė: įsilaužimo strategijos
>white|black||9|11|br Piktadariai ir „raudonosios komandos“ naudojo įvairių tipų „jailbreak“ metodus, kad priverstų dirbtinio intelekto modelius vykdyti žalingus prašymus, kurių jie paprastai atsisakytų dėl apsaugos priemonių. Pavyzdinius išvesties rezultatus „Ataskaitos“ autoriai pateikė tik iliustraciniais tikslais. Daugelis dabartinių aukščiausio lygio (state-of-the-art) dirbtinio intelekto modelių dabar atsilaiko prieš daugumą šių metodų, tačiau vis randama naujų „jailbreak“ technikų.


>white|orangered|left|14|15.5|bb „Pamiršimo“ metodai gali sušvelninti konkrečias kenksmingas modelio galimybes

Kita strategija, kaip mažinti rizikas iš bendrosios paskirties AI, yra tikslingai parinkti (fine-tune) modelius taip, kad jie neturėtų gebėjimų konkrečiose didelės rizikos srityse (‡1175, ‡1176). Pavyzdžiui, tyrėjai kuria „machine unlearning“ algoritmus, kurie galėtų specialiai slopinti gebėjimus, susijusius su biologinėmis grėsmėmis, arba su fotorealistinių nuogybių vaizdų generavimu, vaizduojant žmogaus kūnus (‡903, ‡1272, ‡1273). Šie metodai gali reikšmingai padaryti modelius saugesnius, tačiau prarandant dalį teigiamų panaudojimų, susijusių su neįsisavinamais (unlearned) gebėjimais. Taip pat siūloma riboti AI modelių žinias žalingose srityse kaip būdą kurti „tamper-resistant“ atviro svorio (open-weight) modelius, kurie galėtų atsispirti žalingam tikslingam pritaikymui (harmful fine-tuning) (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Tačiau iki šiol tai padaryti patikimai (robustly) buvo sudėtinga (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Daugiau informacijos rasite §3.4. Open-weight models.

>white|orangered|left|14|15.5|bb Kai kurie tyrėjai dirba metodais, kaip užtikrinti tvirtesnes saugos garantijas, interpretuojant modelio vidines būsenas arba atliekant matematinį patvirtinimą

Kai kurie tyrėjai kuria metodus, kaip nuosekliau patikrinti su sauga susijusias modelių savybes. Vienu požiūriu tyrėjai siekia interpretuoti vidinius modelių skaičiavimus, kad arba nustatytų rizikas, arba pateiktų įtikinamesnius argumentus, kad modelis yra saugus (‡1285, ‡1286). Pavyzdžiui, proof of concept atveju tyrėjai parodė, kad įrankiai, skirti analizuoti kalbos modelio vidinius skaičiavimus, galėtų padėti vertintojams nustatyti žalingą elgesį (‡1287). 2025 m. „Anthropic“ taip pat pradėjo analizuoti modelių vidines sandaras, kaip būdą tirti modelio situacinį suvokimą ir „intent“ (‡2). Tačiau šie metodai šiuo metu nėra dažni arba nėra žinoma, kad jie būtų konkurencingi su kitomis vertinimo technikomis.

Kitas požiūris, siekiant užtikrinti tvirtesnes saugos garantijas, apima matematinių įrodymų konstravimą, kad modelis atitiktų tam tikras saugos sąlygas (‡1177, ‡1282, ‡1288). Tačiau šie įrodymai prisiima, kad testavimo kontekstas sutampa su diegimo kontekstu, ir nėra patikrinti prieš daugelio tipų priešininkus.

Jie taip pat šiuo metu negali būti pritaikyti dideliems modeliams. Apskritai, ekspertų tarpe vyksta reikšmingos diskusijos dėl interpretavimo pažadų ir formalaus patikrinimo metodų.

###@ Diegimo metu atliekamas stebėjimas ir valdymas

Be apsaugų, įdiegtų modelio kūrimo metu, antra gynybos linija nuo žalingo elgesio yra išorinės apsaugos, kurios dėmesį skiria modelio arba sistemos veiksmų stebėjimui ir valdymui diegimo metu. Tokios apsaugos padeda sumažinti netinkamų veikimo atvejų ir piktnaudžiavimo riziką, pavyzdžiui, išgalvotų (hallucinated) išvesčių ir žalingų instrukcijų.

>white|orangered|left|14|15.5|bb Modelio diegėjai gali naudoti įvairius įrankius, kad nustatytų ir spręstų didelės rizikos modelio elgsenas

Kai AI sistema veikia, diegėjas gali stebėti rizikos požymius ir įsikišti, jei jie atsiranda. Pavyzdžiui, jis gali patikrinti modelio įvestis, ar jose nėra požymių, kad vykdomi priešiški išpuoliai, filtruoti netinkamą turinį iš išvesčių arba stebėti sistemos grandinę mintyse, ar joje nėra žalingų planų požymių. Vietos, kuriose diegėjai gali stebėti ir įsikišti į tai, kaip žmonės naudojasi savo sistemomis, apima aparatinę įrangą (‡1180, ‡1181), vartotojo sąveikas (‡1154, ‡1166), įvestis ir išvestis (‡65, ‡725, ‡1182), vidinius skaičiavimus (‡744, ‡1183, ‡1184) ir grandinę mintyse (‡430, ‡435). Taip pat yra keli veiksmai, kuriuos diegėjai gali atlikti, kai nustatoma rizika. Tai apima informacijos registravimą, žalingo turinio filtravimą/keitimą, neįprastos veiklos pažymėjimą, sistemos išjungimus arba apsauginių mechanizmų (failsafes) suaktyvinimą. 3.7 pav. pateikia įprastų stebėsenos ir valdymo mechanizmų pavyzdžius.

Kadangi šie mechanizmai yra universalūs ir dažnai veiksmingi, jie yra plačiai naudojami ir gali užkirsti kelią daugeliui nenumatytos žalos rūšių (‡725, ‡751, ‡1289). Vis dėlto šios apsaugos yra netobulos, ypač vykstant piktybiškiems išpuoliams, optimizuotiems taip, kad jos suveiktų neveiksmingai (‡752, ‡1182). Naujausi tyrimai taip pat nagrinėjo, kaip stebėjimas gali būti nepatikimas, jei sistema optimizuojama naudojant stebėtojo (monitoriaus) balus, pavyzdžiui, padarant samprotavimo grandinę mažiau patikimą (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Figūra 3.7: Stebėsenos ir valdymo metodai
>white|black||9|11|br Stebėjimo ir valdymo metodai veikia keliuose taškuose: filtruojant įvestis ir išvestis dėl žalingo turinio, stebint vidines modelio būsenas, ribojant išorinius veiksmus taikant smėlio dėžės (sandboxing) aplinką ir užtikrinant žmogaus priežiūrą. Šaltinis: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Žmonės kilpoje leidžia užtikrinti tiesioginę kontrolę didelės svarbos situacijose

Norėdami sumažinti nesėkmių tikimybę dėl AI agentų (žr. §2.2.1. Patikimumo iššūkiai), diegėjai gali siekti kurti AI sistemas, kurios veikia bendradarbiaudamos su žmonėmis, o ne visiškai autonomiškai (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Tai svarbu tais atvejais, kai neteisingi sprendimai gali sukelti didelę žalą, pavyzdžiui, finansuose, sveikatos priežiūroje ar policijoje. Tačiau turėti „žmogų kilpoje“ dažnai yra nepraktiška. Kartais sprendimų priėmimas vyksta per greitai, pavyzdžiui, pokalbių programėlėse su milijonais naudotojų. Kitais atvejais, žmogaus šališkumas ir klaidos gali padidinti rizikas dėl klaidų kumuliavimo (‡1187). Žmonės taip pat kilpoje dažnai linkę rodyti „automatizavimo šališkumą“, t. y. jiems dažnai kyla didesnis pasitikėjimas AI sistema, nei tai pagrįsta (‡1190, ‡1191) (žr. §2.3.2. Rizikos žmogaus autonomijai).

>white|orangered|left|14|15.5|bb „Smėliavimas“ apsaugo nuo rizikų, kylančių dėl autonominio elgesio

AI agentai, kurie gali savarankiškai veikti be apribojimų žiniatinklyje ar fiziniame pasaulyje, kelia padidėjusią riziką (žr. §2.2.1. Patikimumo iššūkiai). „Smėliadėžė“ reiškia būdų, kuriais AI agentai gali tiesiogiai daryti įtaką pasauliui, apribojimą, todėl juos daug lengviau prižiūrėti ir valdyti (‡640, ‡1192, ‡1295). Pavyzdžiui, apribojus AI sistemos galimybę skelbti internete arba redaguoti kompiuterio failų sistemą, galima išvengti netikėtų žalos atvejų dėl netikėtų veiksmų (‡1296). Tačiau šių metodų ne visada galima taikyti tais atvejais, kai AI sistema turi neišvengiamai veikti tiesiogiai pasaulyje.

###@ Ecosistemos stebėsenos įrankiai: modelio ir duomenų kilmės patikimumas

Modelio ir duomenų kilmės patikros įrankiai yra techniniai įrankiai, skirti tirti AI ekosistemą, siekiant didinti informuotumą apie tolesnį AI sistemų panaudojimą ir poveikį.

>white|orangered|left|14|15.5|bb AI sistemos kilmės nustatymo metodai padeda atsekti sistemų naudojimą ir poveikį

Kūrėjai ir diegėjai gali naudoti įvairias technikas, kad ištirtų modelio naudojimą ir jo plitimą „lauke“. Pavyzdžiui, jie gali pateikti modeliams unikalius identifikuojančius elgsenos požymius (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) arba taikyti unikalius atskirų atvirojo kodo (open-weight) modelių svorių modelius (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Tačiau padaryti šias technikas atsparesnes modelio modifikacijoms yra atviras klausimas (‡1195, ‡1196*). Tyrėjai taip pat kuria metodus, kaip „išvesti modelio kilmę“ (‡1197, ‡1198, ‡1305, ‡1306), padedančius atsakyti į klausimus, panašius į: „Ar modelis X buvo modelio Y papildomai (fine-tuned) pritaikyta ar distiliuota versija?“ Galiausiai kai kurie kūrėjai dirba prie protokolų ir infrastruktūros AI agentams, kad sąveikaujant su išorinėmis sistemomis būtų palengvintas identifikavimas ir patikra (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Figūra 3.8: Vandenženkliai įterpia nepastebimus trikdžius į vaizdus ir garsą
>white|black||9|11|br Vandens ženklai į vaizdus ir garsą įterpia nepastebimas modifikacijas, kurios leidžia aptikimo įrankiams identifikuoti AI sugeneruotą turinį. Šioje Figūra abu – ir vaizdo, ir garso – vandens ženklai paryškinti, kad būtų geriau matomi. Šaltinis: „Chameleon“ vaizdas iš Unsplash (‡1313*). Kiti elementai sukurti Report autorių. Tarptautinė AI saugos ataskaita 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Figūra 3.9: Promptų injekcijos atakų sėkmės rodikliai
>white|black||9|11|br Promptų įsilaužimo atakų sėkmės rodikliai, kaip pranešė AI kūrėjai pagrindiniams modeliams, išleistiems laikotarpiu nuo 2024 m. gegužės iki 2025 m. rugpjūčio. Kiekvienas taškas reiškia sėkmingų atakų dalį iš 10 bandymų prieš konkretų modelį netrukus po išleidimo. Praneštas tokių atakų sėkmės rodiklis laikui bėgant mažėjo, tačiau išlieka gana aukštas. Šaltinis: Zou et al. 2025 (‡1149), cituota Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb AI turinio aptikimo metodai padeda stebėti AI sugeneruoto turinio sklaidą ir poveikį

Vandenženkliai, metaduomenys ir kiti AI turinio detektoriai gali padėti tyrėjams stebėti ir analizuoti realaus pasaulio poveikį, kurį daro AI sugeneruotas turinys. 

Pirmiausia, duomenų vandens ženklai yra subtilūs, bet aiškūs motyvai, įterpiami į skaitmeninę medžiagą, kurie gali koduoti informaciją apie jų kilmę (‡1199, ‡1200, ‡1201*). Tekstui jie paprastai įgauna subtilių paklaidų žodžių pasirinkime ir stiliuje (‡1308, ‡1309); vaizdams ir vaizdo įrašui – subtilius pikselių raštus (‡1310); o garsui – subtilius garso bangų raštus (‡1311). Figūra 3.8 tai iliustruoja.

Be vandens ženklų, AI sugeneruotą turinį taip pat galima išsaugoti naudojant failų formatus, kurie saugo metaduomenis apie tai, kaip jis buvo sugeneruotas. Pavyzdžiui, daugelis mobiliųjų įrenginių vaizdo ir garso failus išsaugo tokiu failo formatu, kuris gali talpinti informaciją apie kameros nustatymus, laiką, vietą ir pan. (‡1312). Panašūs metaduomenys gali būti naudojami informacijai apie tai, ar duomenis sugeneravo AI sistema, saugoti. Kaip ir pirštų atspaudų nustatymas baudžiamojoje forenzikoje, vandens ženklai ir metaduomenys gali būti sugadinti arba pašalinti, tačiau vis tiek yra naudingi.

Tyrėjai taip pat kuria AI sugeneruoto turinio detektorius (‡1203, ‡1204, ‡1205*), kad padėtų realioje aplinkoje nustatyti AI sugeneruotą turinį, net jei nėra paslėpto ženklinimo (watermark) ar metaduomenų. Tačiau šios identifikavimo technikos pasižymi ribotu sėkmingumo lygiu.

###@ Atnaujinimai

Nuo paskutinės ataskaitos paskelbimo (2025 m. sausis) buvo padaryta pažanga kuriant AI sistemas su keliais veiksmingais saugiklių sluoksniais. Kaip aptarta §3.2. Rizikos valdymo praktikos, gynyba į gylį yra pagrindinis rizikos valdymo principas (‡1314). Pavyzdžiui, AI sistemos, kurios jungia saugumui pritaikytus modelius su įvesties filtrais, išvesties filtrais ir kitais turinio stebėtojais, vis dažniau tiriamos ir diegiamos (‡32, ‡65, ‡1182*). Neseniai atlikti tyrimai taip pat parodė, kad nors modelių kūrėjai padarė pažangą didindami atsparumą bandymams apeiti saugiklius, atakų vykdytojams vis dar pavyksta labai dažnai (3.9 pav.).

###@ Įrodymų spragos

Reikia daugiau įrodymų, kad tyrėjai galėtų suprasti ir įvertinti esamų požiūrių apribojimus. Techninės AI sistemų apsaugos priemonės yra tobulinamos, tačiau metodai susiduria su apribojimais. Pavyzdžiui, pažanga gerinant bendrosios paskirties AI sistemų blogiausio atvejo patikimumą buvo lėta, o yra esminių apribojimų, kiek kruopščiai atvirų svorių (open-weight) modeliai gali būti apsaugoti ir stebimi (‡1195, ‡1315, ‡1316) (žr. ir §3.4. Atvirų svorių modeliai). Tuo tarpu ne visos techninės apsaugos priemonės yra vienodai dažnos, vienodai veiksmingos ar vienodai patvirtintos realiame pasaulyje. Pavyzdžiui, adversarinis mokymas beveik visur naudojamas šiuolaikiniuose (state-of-the-art) modeliuose (‡64*, ‡677), o modelio interpretabilumo ir formalaus patikrinimo metodai iki šiol mažai naudoti produkcinėse sistemose (‡1177, ‡1285).

###@ Iššūkiai politikos formuotojams

Pagrindiniai politikos formuotojų iššūkiai apima sprendimą, ar ir kaip jie turėtų remti tyrimus, plėtrą, vertinimą ir techninių saugiklių bei stebėsenos metodų diegimą. Tai sudėtinga, nes mokslininkų supratimas apie tai, kaip geriausia praktiškai užtikrinti mechanizmus, vis dar kinta, o gerosios praktikos dar nėra nusistovėjusios. Pavyzdžiui, skirtingi kūrėjai taiko skirtingus saugiklius, o jų požiūriai į techninės rizikos mažinimą plačiau labai skiriasi (‡1116). Galiausiai, veiksmingų techninių saugiklių buvimas savaime negarantuoja saugos, nes diegimas ir įgyvendinimas gali skirtis tarp kūrėjų ir priklausomai nuo diegimo konteksto.

