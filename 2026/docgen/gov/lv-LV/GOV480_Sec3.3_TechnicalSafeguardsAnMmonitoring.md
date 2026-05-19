##########
>white|orangered|left|14|30|hr 3.3. sadaļa
### 3.3. Tehniskie drošības pasākumi un uzraudzība
>white|orangered|left|24|30|hb Tehniskie drošības pasākumi un uzraudzība

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Svarīga informācija
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Plašs tehnisko aizsargmehānismu klāsts tiek izmantots dažādos AI izstrādes un izmantošanas posmos. Tas ietver paņēmienus, kas tiek lietoti modeļa izstrādes laikā, lai padarītu sistēmas noturīgākas un izturīgākas pret ļaunprātīgu izmantošanu (piemēram, datu sagatavošana), izvietošanas laikā veikto uzraudzību un kontroli (piemēram, satura filtrēšana un cilvēka uzraudzība), kā arī pēc izvietošanas pieejamus rīkus, lai uzraudzītu plašāku AI ekosistēmu (piemēram, izcelsmes noteikšana un satura atpazīšana).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Tehniskie drošības pasākumiem ir ierobežojumi un tie ne vienmēr ticami novērš kaitniecisku rīcību visos kontekstos. Piemēram, lietotāji dažkārt var iegūt kaitīgus iznākumus, pārfrazējot pieprasījumus vai sadalot tos mazākos soļos. Līdzīgi arī rīki, piemēram, ūdenszīmešana, kas ir paredzēti, lai identificētu ar AI ģenerētu saturu, bieži vien ir iespējams noņemt vai modificēt, kas samazina to uzticamību.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Individuālo aizsardzības pasākumu ierobežojumi nozīmē, ka, lai novērstu noteiktus kaitīgus iznākumus, var būt nepieciešams “aizsardzība dziļumā”. Piemēram, sistēma var apvienot ar drošību apmācītu modeli ar ievades filtriem, izvades filtriem un satura uzraugiem.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kopš pēdējā ziņojuma publicēšanas (January 2025) pētnieki ir panākuši progresu, uzlabojot aizsargmehānismus, taču pastāv pamatierobežojumi. Piemēram, uzbrukumu, kas izstrādāti, lai apietu aizsargmehānismus, sekmju rādītājs ir samazinājies, tomēr joprojām ir salīdzinoši augsts. Pastāv arī pamatierobežojumi, cik rūpīgi atvērtā svaru modeļus (open-weight models) var nodrošināt ar aizsardzību.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Viens no galvenajiem izaicinājumiem politikas veidotājiem ir ierobežotie pierādījumi par to, cik efektīvas ir aizsardzības sargkārtas dažādos reālās pasaules vispārējas nozīmes AI sistēmu pielietojumos. AI izstrādātāji ļoti atšķiras ar to, cik daudz informācijas viņi atklāj par savām sargkārtām un uzraudzību. Vēl viens izaicinājums ir iespējamie kompromisi starp stingrāku aizsargkārtu piemērošanu un sistēmas veiktspējas vai lietderīguma saglabāšanu.
>oldlace|black||11|15|br      


AI izstrādātāji var izmantot vairākus noderīgus, taču nepilnīgus tehniskus aizsargmehānismus, lai mazinātu un pārvaldītu riskus, ko rada vispārējas nozīmes AI sistēmas, tomēr noturības problēmas joprojām pastāv. Izstrādātāji joprojām nevar pilnībā novērst to, ka vispārējas nozīmes AI sistēmas veic pat labi zināmas un atklāti kaitīgas darbības, piemēram, piedāvā lietotājiem instrukcijas noziegumu izdarīšanai. Piemēram, pētnieki ir parādījuši, ka jaunākā līmeņa aizsargmehānismus var apiet, izmantojot adversariālas (t.i., “jailbreak”) pieprasījumu veidošanas metodes (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), panākot, ka modeļi sadala sarežģītus kaitīgus uzdevumus soļos (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), un izmantojot vienkāršas modeļa modifikācijas (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Pētnieki turpina strādāt pie aizsargmehānismiem pret darbības traucējumiem un ļaunprātīgu izmantošanu (‡690). Šīs metodes būtiski atšķiras pēc mērķa un efektivitātes, un to ietekme galu galā ir atkarīga no plašā sociotehniskā un pārvaldības (governance) konteksta, kurā AI sistēmas tiek izstrādātas un ieviestas.

Tehniskos drošības pasākumus plaši var iedalīt trīs kategorijās: paņēmieni drošāku modeļu izstrādei; paņēmieni, kas tiek izmantoti izvietošanas laikā uzraudzībai un kontrolei; un paņēmieni, kas atbalsta ekosistēmas uzraudzību pēc izvietošanas. Tabula 3.6 apkopo apspriestos tehniskos drošības pasākumus, to efektivitāti un neatrisinātās problēmas.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Izstrādājot drošākus modeļus
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Datu sagatavošana (‡1167)
  Kaitīgu datu noņemšana, lai neļautu modelim apgūt bīstamas spējas. Šīs metodes var būt noderīgas, tostarp izstrādājot atvērto svaru modeļus, kuriem trūkst kaitīgu spēju, un kas spēj pretoties kaitīgai pielāgotai apmācībai (‡55). Tomēr pastāv izaicinājumi saistībā ar datu atlases kļūdām un mērogošanu (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mācīšanās ar pastiprinājumu no cilvēku atgriezeniskās saites (‡64*)
  Apmācot modeli, lai tas atbilstu noteiktajiem mērķiem, piemēram, būt noderīgam un nekaitīgam. Tas ir efektīvs veids, kā modeļiem iemācīt izdevīgas uzvedības modeļus (‡64*). Tomēr pārmērīga optimizācija cilvēku apstiprinājumam var likt modeļiem uzvesties maldinoši vai pārmērīgi piekļāvīgi (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pluralistiskas saskaņošanas tehnikas (‡1170)
  Mācot modeli integrēt vairākus atšķirīgus viedokļus par to, kā tam vajadzētu rīkoties. Šīs metodes palīdz samazināt pakāpi, kādā modeļi dod priekšroku konkrētiem viedokļiem (‡1170). Tomēr, neraugoties uz šīm metodēm, cilvēku domstarpības ir neizbēgamas, un ir grūti izstrādāt plaši pieņemtus veidus, kā līdzsvarot konkurējošus uzskatus (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adversarial apmācība (‡677)
  Apmācot modeli atteikties nodarīt kaitējumu (pat nepazīstamos apstākļos) un pretoties uzbrukumiem no ļaunprātīgiem lietotājiem (piem., “jailbreaks”). Šī ir efektīva metode, lai panāktu, ka modeļi pretojas mēģinājumiem ļaunprātīgi izmantot sistēmu (‡1064), taču robustuma izaicinājumi joprojām pastāv (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mašīnas “atmācīšanās” (‡1175, ‡1176)
  Modeļa apmācība, izmantojot specializētus algoritmus, nozīmē aktīvi apspiest kaitīgas iespējas (piem., zināšanas par bioloģiskajiem apdraudējumiem). Šīs metodes piedāvā mērķtiecīgu veidu, kā no modeļiem noņemt kaitīgas iespējas (‡1175, ‡1176), taču pašreizējie “unlearning” algoritmi var būt neuzticami un tiem var būt neparedzētas sekas uz citām iespējām (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Interpretējamības un drošības verifikācijas rīki (‡1177)
  Dažādu projektēšanas un verifikācijas metožu kopums, kas domāts, lai nodrošinātu stingrāku pārliecību par to, ka modeļiem ir noteiktas ar drošību saistītas īpašības. Tie ļauj vērtētājiem sniegt augstāka līmeņa drošības garantijas (‡1177), taču pašreizējās metodes balstās uz pieņēmumiem un praksē reti ir konkurētspējīgas veiktspējas ziņā (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Uzraudzība un kontrole
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Aparatūras uzraudzības mehānismi (‡1179, ‡1180, ‡1181)
  Pārbauda, ka autorizēti procesi darbojas aparatūrā, lai pētītu drošības apdraudējumus vai atbilstību normatīvajām prasībām. Šie mehānismi piedāvā unikālus veidus, kā uzraudzīt, kādi aprēķini tiek izpildīti aparatūrā un kas tos izpilda (‡1181). Tomēr aparatūras mehānismi nevar uzraudzīt visu veidu apdraudējumus, un dažas metodes prasa specializētu aparatūru (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Lietotāja mijiedarbības uzraugi (‡1154, ‡1166)
  Lietotāju mijiedarbības uzraudzība, lai konstatētu ļaunprātīgas izmantošanas pazīmes, var palīdzēt izstrādātājiem pārtraukt pakalpojumu ļaunprātīgiem lietotājiem (‡1154, ‡1166). Tomēr izpilde var neapzināti kavēt lietderīgus drošības pētījumus (‡689), un dažas ļaunprātīgas izmantošanas formas ir grūti atklāt (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Lietotāja mijiedarbības monitori (‡1154, ‡1166)
  Lietotāju mijiedarbību uzraudzīšana, lai pamanītu ļaunprātīgas izmantošanas pazīmes, var palīdzēt izstrādātājiem pārtraukt pakalpojumu sniegšanu ļaunprātīgiem lietotājiem (‡1154, ‡1166). Tomēr īstenošana var netīšām kavēt lietderīgu pētniecību par drošību (‡689), un dažas ļaunprātīgas izmantošanas formas ir grūti noteikt (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Satura filtri (‡65*, ‡725)
  Filtrēšana, kas varētu kaitēt modeļa ievadēm un izvadei, ir ļoti efektīvs veids, kā samazināt nejaušu kaitējumu un ļaunprātīgas izmantošanas riskus (‡725). Tomēr filtri prasa papildu skaitļošanas jaudu un ir ievainojami pret dažiem uzbrukumiem (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modeļa iekšējās aprēķinu uzraudzības (‡744, ‡1183, ‡1184)
  Modeļu maldināšanas pazīmju vai citu kaitīgu iekšējo domāšanas formu uzraudzība var būt efektīvs veids, kā atklāt maldināšanu (‡744, ‡1183, ‡1184). Tomēr pašreizējās metodes trūkst noturības un uzticamības (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ķēdes domāšanas uzraugi (‡430, ‡435)
  Modeļu ķēdes domāšanas teksta uzraudzīšana, lai konstatētu maldinošas uzvedības pazīmes vai citu kaitniecisku spriešanu, ir efektīvs veids, kā saprast un pamanīt nepilnības tajā, kā modeļi spriež (‡435). Tomēr tie var būt neuzticami (‡752, ‡753, ‡1186), un, ja modeļi tiek apmācīti ģenerēt labdabīgu ķēdes domāšanu, tie var apgūt maldinošu uzvedību (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cilvēks cilpē (‡1187, ‡1188, ‡1189)
  Cilvēka uzraudzība un atcelšanas iespējas sistēmas lēmumiem ir būtiskas dažās drošībai kritiskās lietojumprogrammās (‡1187). Tomēr šīs metodes ir ierobežotas ar automatizācijas aizspriedumiem un cilvēka lēmumu pieņemšanas ātruma ierobežojumiem (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Izolēšana smilškastē (‡1192)
  AI aģenta tiešas ietekmēšanas uz pasauli novēršana ir efektīvs veids, kā ierobežot kaitējumu, ko tas var radīt (‡1192). Tomēr saskarņu izolācija (sandboxing) ierobežo sistēmas spēju tieši izpildīt noteiktus uzdevumus (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Rīki ekosistēmas uzraudzības atvieglošanai
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb AI modeļu identifikācijas paņēmieni (‡1193*, ‡1194)
  Padarīt modeļus, vai atsevišķas modeļu instances, vieglāk identificējamus reālās vides izmantošanas gadījumos palīdz digitālajai kriminālistikai un ekosistēmas izpratnei (‡1195). Tomēr šīs metodes var apiet ar dažiem modeļu modifikāciju veidiem (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb AI modeļa mantojuma inferēšana (‡1197)
  Šīs metodes ļauj pētniekiem pētīt, kā AI ekosistēmā tiek modificēti modeļi, īpaši atvērtā svaru (open-weight) modeļi. Tās palīdz digitālajā kriminālistikā un ekosistēmas apzināšanā (‡1198), taču būtu nepieciešami liela mēroga projekti, lai rūpīgi kartētu atvērtā svaru modeļu ekosistēmu (‡1198).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ūdenszīmes un metadati (‡1199, ‡1200, ‡1201*)
  Šīs metodes atvieglo noteikt, kad kāds teksts, attēls, video u.tml. ir ģenerēts ar AI vai arī modificēts, un ar kādu sistēmu. Tās sekmē labāku ekosistēmas apziņu (‡1199, ‡1200, ‡1201*). Tomēr ūdenszīmes un metadati var tikt viltoti vai noņemti ar dažām satura modifikācijām (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb AI ģenerēta satura noteikšana (‡1203, ‡1204, ‡1205*)
  Lietotāju spēja atšķirt ar AI ģenerētu un autentisku saturu uzlabo digitālo kriminālistiku un ekosistēmas izpratni (‡1203, ‡1204). Tomēr klasifikatori var būt neuzticami (‡1205*) un tiem var būt mainīga veiktspēja dažādās modalitātēs.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabula 3.6: Tehniskie drošības pasākumi, kas aplūkoti šajā sadaļā
>white|black||9|11|br Šīs sadaļas ietvaros apspriesto tehnisko aizsargpasākumu kopsavilkums, sadalot tos metodēs drošāku modeļu izstrādei, uzraudzības un kontroles īstenošanas laikā un metodēs, kas atvieglo ekosistēmas uzraudzību.


###@ Izstrādājot drošākus modeļus

Pirmajai aizsardzības līnijai pret kaitējumiem, ko rada vispārējas nozīmes AI sistēmas, ir jābūt drošākam pamatmodelim. Šī apakšsadaļa aptver drošības pasākumus, kas ir “iebūvēti modeļa parametros” modeļa izstrādes procesā (Figūra 3.6).

>white|orangered|left|14|15.5|bb Kvalitatīvu apmācības datu atlasīšana var ierobežot tādu potenciāli bīstamu spēju attīstību

Vispārējas nozīmes AI modeļi ir noderīgi tieši tāpēc, ka pēc apmācības datu apstrādes tie attīsta plašu zināšanu un spēju klāstu, taču daži apmācības datu veidi nesamērīgi lielā mērā ir atbildīgi par potenciāli bīstamu spēju attīstību. Piemēram, uz viroloģijas publikācijām apmācīts AI modelis var labāk spēt sniegt palīdzību potenciāli kaitīgos bioloģijas uzdevumos (‡549, ‡1206*) (skat. arī §2.1.4. Bioloģiskie un ķīmiskie riski). Turklāt attēlu/video ģeneratori, kas apmācīti uz cilvēka kailuma attēliem, var tikt ļaunprātīgi izmantoti arī nekonsensuālu intīmo deepfake izveidei (‡308, ‡319) (skat. arī §2.1.1. AI ģenerēts saturs un noziedzīga darbība).

Datu filtrēšana apmācībai ir efektīvs mazināšanas pasākums pret dažām nevēlamām spējām (‡319, ‡1167, ‡1207, ‡1208). Tomēr var būt grūti filtrēt lielos datu kopumus, ko izmanto vispārējas nozīmes AI modeļu apmācībai (‡1168), jo ir augstas izmaksas (‡1209), filtrēšanas kļūdas (‡1210) un negatīva ietekme uz datu kopas kvalitāti (‡1211). Šos izaicinājumus pastiprina interneta teksta daudzvalodīgais raksturs (‡1212), kultūras aizspriedumi satura moderēšanā (‡1211, ‡1213, ‡1214, ‡1215) un fakts, ka tas, vai konkrēts datu elements ir “kaitīgs”, ir atkarīgs no konteksta faktoriem (‡1216). Tomēr potenciāli kaitīga satura filtrēšana no apmācības datiem liecina par solījumu padarīt modeļus drošākus un uzticamākus, tostarp padarīt atvērtās svara daļas modeļus noturīgākus pret kaitniecisku iejaukšanos (‡55). Saistības starp apmācības datu saturu un emergentajām modeļu spējām vēl nav pilnībā izprastas (‡1195), un filtrēšana, šķiet, ir efektīvāka kaitīgu spēju ierobežošanā, ja to piemēro plašām zināšanu jomām (‡55), salīdzinot ar šaurākām uzvedībām (‡1206, ‡1217). Skatīt §3.4. Atvērtās svara daļas modeļi turpmākai diskusijai.

![figure 3.6](images/fig3.6_safeguards.png)

##### Figūra 3.6: Kur piemērot tehniskos drošības pasākumus
>white|black||9|11|br Tehniskās drošības garantijas var piemērot dažādos modeļa izstrādes posmos. Datu sagatavošana ietekmē to, ko modeļi apgūst pirmapmācības un smalkas pielāgošanas laikā. Apmācīšanā balstītas metodes, piemēram, pastiprināšanas mācīšanās no cilvēka atgriezeniskās saites un noturības apmācība, pielāgo modeļa uzvedību. Pārbaudes metodes, piemēram, pretinieku uzbrukumi, identificē atlikušās ievainojamības. Dažas tehnikas, piemēram, drošuma pēc konstrukcijas algoritmi, aptver vairākus posmus. Avots: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Vispārējas nozīmes AI modeļu apmācības metodes, lai tie būtu noderīgi un nekaitīgi, galvenokārt balstās uz cilvēku atsauksmēm

Ir grūti apmācīt un izvērtēt modeļus tā, lai tie uzticami atbilstu augsta līmeņa principiem, piemēram, būt noderīgiem, nekaitīgiem un godīgiem. Praksē izstrādātāji cenšas to panākt, veicot AI modeļu smalkpielāgošanu, izmantojot demonstrējumus un cilvēku atgriezenisko saiti. Piemēram, galvenais smalkpielāgošanas paradigmas veids AI modeļiem, kas pazīstams kā “pastiprināšanas mācīšanās no cilvēku atgriezeniskās saites”, balstās uz modeļu apmācīšanu, lai tie ģenerētu izvades, kuras cilvēku anotētāji vērtē pozitīvi (‡1218). Tomēr pozitīva cilvēku atgriezeniskā saite ir kļūdains aizstājējrādītājs uzvedībai, kas ir patiešām noderīga (‡737, ‡878, ‡1219, ‡1220), un to ierobežo cilvēku kļūdas un aizspriedumi (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Tas rada vairākus izaicinājumus: modeļi, kurus ar pastiprinājuma apmācību, izmantojot cilvēka atgriezenisko saiti, dažkārt pārmērīgi cenšas iepriecināt lietotāju, uzvedību, kas pazīstama kā ‘sikofānija’ (‡358, ‡740, ‡1226, ‡1227); sniegt atbildes, kas dažos kontekstos ir noderīgas, bet citos — kaitīgas (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); sniegt atbildes, kuras ir grūti novērtēt pēc pareizības (‡1233); vai veikt darbības, kuru lietderība vai kaitīgums ir viedokļa jautājums (‡1234). 3.7. tabula sniedz šo izaicinājumu piemērus. Daļa pētījumu mērķē izstrādāt metodes, lai palīdzētu cilvēkiem labāk novērtēt risinājumus sarežģītiem uzdevumiem ar AI asistenci (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Tomēr šīm metodēm pašlaik ir ierobežota uzticamība, un tas, cik lielā mērā tās tiek izmantotas, lai apmācītu mūsdienu vismodernākos AI modeļus, nav publiski zināms.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Padevība/iepriecināšana (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Paskaidrojums:
>white|black|left|11|13|br Modelis sniedz tikai pozitīvu atgriezenisko saiti, neizceļot trūkumu, ka nav pareizas 5-7-5 haiku zilbju struktūras.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dažas darbības dažos kontekstos ir noderīgas, bet citos - kaitīgas (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Paskaidrojums:
>white|black|left|11|13|br Informāciju par bioloģisko risku var izmantot izglītībai un aizsardzībai, taču arī, lai informētu ļaunprātīgus aktorus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pareizu darbību ir grūti pārbaudīt (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Paskaidrojums:
>white|black||11|13|br Šīs atbildes pareizību ir grūti novērtēt, jo tam ir nepieciešamas medicīniskas zināšanas. Pat pieredzējušam ārstam šādu atbilžu izvērtēšanai ir vajadzīgs laiks un rūpīga uzmanība detaļām.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Cilvēki nepiekrīt tam, kas ir pareizi (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Paskaidrojums:
>white|black|left|11|13|br Cilvēki būtiski nesaskan par to, kāda ir pareizā atbilde.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabula 3.7: Lietotāja pieprasījums un AI modeļa atbilde
>white|black||9|11|br Piemēri izaicinājumiem, kas saistīti ar tādu izdevīgu rīcību norādīšanu un stimulēšanu, kuras jāveic AI modeļiem.


>white|orangered|left|14|15.5|bb Cilvēki ne vienmēr vienojas par to, kuras uzvedības ir vēlamas, tādēļ ir nepieciešamas metodes, lai līdzsvarotu konkurējošas vēlmes.

Cilvēki ne vienmēr vienojas par to, kādām atbildēm vai darbībām AI modeļiem vajadzētu vai nevajadzētu izvadīt (‡1006). Tas būtiski apgrūtina tādu modeļu izstrādi, kuru rīcība un ietekme plaši atbilst sabiedrības interesēm (‡420). Daži pētnieki pēta, kuru vēlmes atspoguļojas AI sistēmās (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249), un strādā pie tā, lai izstrādātu “plurālistiskas saskaņošanas” (pluralistic alignment) paņēmienus, kuru mērķis ir panākt līdzsvaru starp konkurējošām vēlmēm (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Piemēram, AI izstrādātāji var projektēt sistēmas, lai tās neģenerētu pretrunīgas atbildes, atsakoties atbildēt uz noteiktiem pieprasījumiem, vai saskaņotos ar attiecīgajā cilvēku izlasē atbilstošo mediānas uzskatu, vai pielāgotu sistēmas atsevišķiem lietotājiem.

Viena no biežākajām šo pieeju problēmām ir tā, ka kopumā AI sistēmas nespēj vienlīdzīgi saskaņoties ar ikviena vēlmēm, un to tālākie sociālie iespaidi ietekmēs dažādas cilvēku grupas atšķirīgi. Daži pētnieki ir apgalvojuši, ka lielākā daļa tehnisko pieeju plurālistiskajai saskaņošanai neaptver un iespējams pat novērš uzmanību no dziļākām problēmām, piemēram, no sistemātiskām novirzēm, sociālās varas dinamikas un turības un ietekmes koncentrācijas (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb AI izstrādātāji izmanto “adversarial training”, lai uzlabotu modeļa noturību

Ir grūti nodrošināt, lai AI modeļi robusti pārnestu apmācības laikā iemācīto labvēlīgo uzvedību uz reālās pasaules izvietošanas kontekstiem. Pat modeļi, kas apmācīti ar “perfektu” mācību signālu, var neizdoties veiksmīgi vispārināt uz visiem līdz šim neredzētajiem kontekstiem (‡738, ‡739, ‡1255, ‡1256, ‡1257). Piemēram, daži pētnieki ir atklājuši, ka tērzēšanas roboti, visticamāk, veiks kaitīgas darbības valodās, kuras viņu apmācības datos ir nepietiekami pārstāvētas (‡159, ‡880, ‡1258*, ‡1259), tostarp daudzās valodās, kuras galvenokārt runā Global South.

Pēdējos gados pētnieki ir izveidojuši arī plašu rīkkopu “adversarial attack” paņēmienu, kurus var izmantot, lai panāktu, ka modeļi ģenerē potenciāli kaitīgas atbildes (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Piemēram, nesen izveidotā iniciatīva ieguva vairāk nekā 60,000 dažādu piemēru par veiksmīgiem uzbrukumiem valsts-of-the-art AI modeļiem, kas lika tiem pārkāpt savu uzņēmumu politikas par pieļaujamu modeļu uzvedību (‡1149). Tabula 3.8 parāda “jailbreak” paņēmienu piemērus, kurus pētnieki ir parādījuši, ka tie var panākt, lai modeļi izpilda kaitīgas prasības.

Viens no veidiem, kā uzlabot modeļu noturību, ir pazīstams kā “adversariālā apmācība” (‡1064). Tā ietver “uzbrukumu” (piem., jailbreaku) konstruēšanu, kas ir izstrādāti, lai panāktu, ka modelis rīkojas nevēlamā veidā, un modeļa apmācību, lai tas šos uzbrukumus spētu apstrādāt atbilstoši. Tomēr adversariālā apmācība nav perfekta (‡1260, ‡1261). Uzbrucēji pastāvīgi spēj izstrādāt jaunus veiksmīgus uzbrukumus pret jaunākās paaudzes (state-of-the-art) modeļiem (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Tā kā izstrādātājiem ir nepieciešami konkrēti piemēri par atteices režīmiem, lai varētu pret tiem apmācīt (‡512, ‡1263), rezultāts ir nepārtraukta “kaķa un peles” spēle, kurā izstrādātāji pastāvīgi atjaunina modeļus, reaģējot uz tikko atklātām ievainojamībām, un pretinieki pastāvīgi meklē jaunus uzbrukumus. Daži pētnieki ir ierosinājuši plašāka mēroga adversariālo apmācību (‡1264, ‡1265) vai jaunus algoritmus (‡675, ‡676, ‡1263, ‡1266, ‡1267), lai uzlabotu noturību, taču mūsdienu AI sistēmas joprojām paliek pastāvīgi ievainojamas.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Stratēģija: Padarīt kaitīgus pieprasījumus šifrētā tekstā, piemēram, morzes kodu (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Stratēģija: sagatavojiet sistēmu ar atbilstošu atbilžu piemēriem uz kaitīgiem pieprasījumiem (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Stratēģija: Veikt kaitnieciskus pieprasījumus zemas resursu valodās, kuras, visticamāk, netiks izmantotas apmācībā tik bieži (piemēram, svahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Stratēģija: Sašķeliet kaitīgu uzdevumu vairākos nevainīgos apakšuzdevumos (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.8. tabula: džailsbreikošanas stratēģijas
>white|black||9|11|br Ļaundabīgi aktori un “red teams” ir izmantojuši dažāda veida “jailbreaks”, lai liktu AI modeļiem izpildīt kaitnieciskus pieprasījumus, kurus tie parasti atteiktu drošības pasākumu dēļ. Piemēra izvades ir sagatavojuši ziņojuma autori tikai ilustratīviem nolūkiem. Daudzi mūsdienu jaunākā līmeņa AI modeļi tagad spēj pretoties lielākajai daļai šo metožu, taču turpina tikt atklātas jaunas jailbreakošanas metodes.


>white|orangered|left|14|15.5|bb “Neapgūšanas” metodes var mazināt konkrētas kaitīgas modeļa spējas

Vēl viena stratēģija, lai mazinātu riskus no vispārējas nozīmes AI, ir pielāgot modeļus tā, lai tiem trūktu spēju konkrētās īpaši augsta riska jomās (‡1175, ‡1176). Piemēram, pētnieki strādā pie tādu algoritmu izstrādes, ko dēvē par “machine unlearning”, un kuru mērķis ir tieši nomākt spējas, kas saistītas ar bioloģiskajiem draudiem, vai spējas ģenerēt fotoreālistiskus kailu cilvēka ķermeņu attēlus (‡903, ‡1272, ‡1273). Šīs metodes var padarīt modeļus būtiski drošākus, taču uz ierobežojumu rēķina attiecībā uz dažām pozitīvām un apzināti lietderīgām iespējām, ko dod “unlearned” spējas. AI modeļu zināšanu ierobežošana kaitīgās jomās ir ierosināta arī kā veids, kā izstrādāt “tamper-resistant” atvērtā svaru (open-weight) modeļus, kas var pretoties kaitīgai pielāgošanai (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Tomēr līdz šim to ir bijis grūti paveikt robusti (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Sk. §3.4. Open-weight models, lai iegūtu plašāku apspriešanu.

>white|orangered|left|14|15.5|bb Daži pētnieki izstrādā metodes drošākām drošības garantijām, interpretējot modeļa iekšējās stāvokļus vai veicot matemātisku verifikāciju

Daži pētnieki strādā pie metodēm, lai stingrāk pārbaudītu ar drošību saistītas modeļu īpašības. Vienā pieejā pētnieki cenšas interpretēt modeļu iekšējos aprēķinus, lai vai nu identificētu riskus, vai arī izteiktu pārliecinošākus argumentus par to, ka modelis ir drošs (‡1285, ‡1286). Piemēram, pierādījuma par koncepciju ietvaros pētnieki parādīja, ka rīki, kas analizē valodas modeļa iekšējo aprēķinu, var palīdzēt vērtētājiem identificēt kaitējošu rīcību (‡1287). 2025. gadā arī Anthropic sāka analizēt modeļu iekšējās struktūras kā veidu, kā pētīt modeļa situatīvo apzināšanos un “nodomu” (‡2). Tomēr šāda veida metodes pašlaik nav izplatītas vai arī nav zināms, ka tās būtu konkurētspējīgas ar citām vērtēšanas metodēm.

Cits piegājiens drošības garantiju stiprināšanai ietver matemātisku pierādījumu konstruēšanu, ka modelis izpildīs noteiktus drošības nosacījumus (‡1177, ‡1282, ‡1288). Tomēr šie pierādījumi pieņem, ka testēšanas konteksts atbilst izvietošanas kontekstam, un tie nav pārbaudīti pret daudzām pretinieku (adversaries) tipoloģijām.

Tās arī pašlaik nevar mērogot līdz lieliem modeļiem. Kopumā ekspertu vidū notiek ievērojamas diskusijas par interpretējamības un formālās verifikācijas metožu solījumu.

###@ Uzraudzība un kontrole izpildes laikā

Papildus aizsardzības pasākumiem, kas ieviesti modeļa izstrādes laikā, otrā aizsardzības līnija pret kaitīgu rīcību ir ārējie aizsardzības pasākumi, kas vērsti uz modeļa vai sistēmas darbību uzraudzību un kontroli ieviešanas (deployment) laikā. Šādi aizsardzības pasākumi palīdz mazināt darbības traucējumus un ļaunprātīgu izmantošanu, piemēram, halucinētas izvades un kaitīgas instrukcijas.

>white|orangered|left|14|15.5|bb Modeļa izvēršanas veicēji var izmantot dažādus rīkus, lai identificētu un novērstu augsta riska modeļa uzvedību

Kad AI sistēma darbojas, izdevējs var uzraudzīt riska pazīmes un iejaukties, ja tās parādās. Piemēram, viņi var pārbaudīt modeļa ievades par pazīmēm, kas liecina par ļaunprātīgiem uzbrukumiem, filtrēt nepiemērotu saturu no izvades vai uzraudzīt sistēmas domu ķēdi, lai pamanītu pazīmes par kaitīgiem plāniem. Vietas, kur izdevēji var uzraudzīt un iejaukties tajā, kā cilvēki izmanto savas sistēmas, ietver aparatūru (‡1180, ‡1181), lietotāju mijiedarbības (‡1154, ‡1166), ievades un izvades (‡65, ‡725, ‡1182), iekšējos aprēķinus (‡744, ‡1183, ‡1184) un domu ķēdi (‡430, ‡435). Ir arī vairākas darbības, kuras izdevēji var veikt, ja tiek identificēti riski. Tās ietver informācijas reģistrēšanu, kaitīga satura filtrēšanu/modificēšanu, neparastas aktivitātes iezīmēšanu, sistēmas izslēgšanu vai drošības mehānismu aktivizēšanu. Figūra 3.7 parāda kopīgu uzraudzības un kontroles mehānismu piemērus.

Tā kā šie mehānismi ir daudzpusīgi un bieži vien efektīvi, tos plaši izmanto, un tie var novērst daudzus nejaušas kaitējuma veidus (‡725, ‡751, ‡1289). Tomēr šīs aizsardzības ir nepilnīgas, īpaši ļaunprātīgos uzbrukumos, kas optimizēti tā, lai tās liktu izgāzties (‡752, ‡1182). Jaunākie pētījumi ir arī aplūkojuši, kā uzraudzība var būt neuzticama, ja sistēma tiek optimizēta, izmantojot monitora rādītājus, piemēram, padarot ķēdes domāšanu mazāk uzticamu (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Figūra 3.7: Uzraudzības un kontroles paņēmieni
>white|black||9|11|br Uzraudzības un kontroles metodes darbojas vairākos punktos: ievades un izvades datu pārbaude attiecībā uz kaitīgu saturu, iekšējo modeļa stāvokļu uzraudzīšana, ārējo darbību ierobežošana, izmantojot smilškastes (sandboxing), un cilvēka pārraudzības nodrošināšana. Avots: Starptautiskais AI drošības ziņojums 2026.


>white|orangered|left|14|15.5|bb Cilvēki cilpā ļauj veikt tiešu uzraudzību augsta riska situācijās.

Lai samazinātu AI aģentu kļūmju iespējamību (sk. §2.2.1. Uzticamības problēmas), izvietotāji var tiekties izstrādāt AI sistēmas, kas darbojas sadarbībā ar cilvēkiem, nevis pilnībā autonomi (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Tas ir svarīgi lietošanas gadījumos, kuros nepareizi lēmumi var radīt būtisku kaitējumu, piemēram, finansēs, veselības aprūpē vai policijā. Tomēr “cilvēks cilpā” bieži vien ir nepraktiski. Dažkārt lēmumu pieņemšana notiek pārāk ātri, piemēram, tērzēšanas lietotnēs ar miljoniem lietotāju. Citos gadījumos cilvēku aizspriedumi un kļūdas var pastiprināt riskus, jo kļūdas savstarpēji kumulējas (‡1187). Cilvēki cilpā arī mēdz demonstrēt “automatizācijas aizspriedumu”, kas nozīmē, ka viņi bieži uzticas AI sistēmai vairāk, nekā tas ir pamatoti (‡1190, ‡1191) (sk. §2.3.2. Risi cilvēka autonomijai).

>white|orangered|left|14|15.5|bb “Izolēšana” pasargā no riskiem, ko rada autonomas uzvedības

AI aģenti, kas var rīkoties autonomi bez ierobežojumiem tīmeklī vai fiziskajā pasaulē, rada paaugstinātus riskus (skat. §2.2.1 Uzticamības izaicinājumi). “Sandboxes” ietver to, ka tiek ierobežoti veidi, kādos AI aģenti var tieši ietekmēt pasauli, tādējādi tos ir daudz vieglāk uzraudzīt un pārvaldīt (‡640, ‡1192, ‡1295). Piemēram, ierobežojot AI sistēmas spēju publicēt informāciju internetā vai rediģēt datora failu sistēmu, var novērst neparedzētu kaitējumu no neparedzētām darbībām (‡1296). Tomēr šīs pieejas ne vienmēr var izmantot lietojumprogrammās, kur AI sistēmai obligāti jāiedarbojas tieši pasaulē.

###@ Ekosistēmas uzraudzības rīki: modeļa un datu izcelsme

Modeļu un datu izcelsmes (provenance) rīki ir tehniski rīki, kas paredzēti AI ekosistēmas izpētei, lai uzlabotu izpratni par AI sistēmu turpmāko izmantojumu un ietekmēm.

>white|orangered|left|14|15.5|bb AI sistēmu izcelsmes (provenance) tehnikas palīdz izsekot sistēmu izmantošanai un ietekmei

Izstrādātāji un izvietošanas veicēji var izmantot dažādas metodes, lai pētītu modeļa izmantošanu un izplatīšanos “savvaļā”. Piemēram, viņi var piešķirt modeļiem unikālas identifikējošas uzvedības (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) vai piemērot unikālus modeļus atsevišķu atvērtā svaru modeļu svariem (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Tomēr padarīt šīs metodes izturīgākas pret modeļa modifikācijām ir atklāta problēma (‡1195, ‡1196*). Pētnieki arī strādā pie metodēm “modeļa mantojuma” noteikšanai (‡1197, ‡1198, ‡1305, ‡1306), kas palīdz atbildēt uz tādiem jautājumiem kā: “Vai modelis X bija uz smalkregulēšanas (fine-tuning) vai destilēšanas (distilled) balstīta versija no modeļa Y?” Visbeidzot, daži izstrādātāji strādā pie protokoliem un infrastruktūras AI aģentiem, lai mijiedarbībā ar ārējām sistēmām atvieglotu identifikāciju un verifikāciju (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### 3.8. attēls: Ūdenszīmes attēlos un audio iegulda nemanāmas perturbācijas
>white|black||9|11|br Ūdenszīmes iegulda attēlos un audio failos nemanāmas perturbācijas, kas ļauj ar noteikšanas rīkiem identificēt ar AI ģenerētu saturu. Šajā figūrā gan attēla, gan audio ūdenszīmes ir izceltas, lai nodrošinātu redzamību. Avots: Chameleon attēls no Unsplash (‡1313*). Citi elementi, ko izveidojuši ziņojuma autori. Starptautiskais AI drošības ziņojums 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Figūra 3.9: Piekļuves ļaunprātīgas ievadīšanas uzbrukuma panākumu rādītāji
>white|black||9|11|br Promptinjekcijas uzbrukumu veiksmju rādītāji, kā ziņojuši AI izstrādātāji par galvenajiem modeļiem, kas izlaisti laika posmā no 2024. gada maija līdz 2025. gada augustam. Katrs punkts attēlo veiksmīgo uzbrukumu īpatsvaru 10 mēģinājumos pret konkrēto modeli neilgi pēc izlaišanas. Ziņotais šādu uzbrukumu veiksmju rādītājs laika gaitā ir samazinājies, taču joprojām ir salīdzinoši augsts. Avots: Zou et al. 2025 (‡1149), citēts Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb AI satura noteikšanas paņēmieni palīdz uzraudzīt ar AI ģenerēta satura izplatību un ietekmi

Ūdenszīmes, metadati un citi AI satura detektori var palīdzēt pētniekiem izsekot un pētīt ar AI ģenerēta satura reālo ietekmi uz pasauli. 

Vispirms, datu ūdenszīmes ir smalki, bet atšķirīgi motīvi, kas tiek ievietoti digitālajos materiālos un var kodēt informāciju par to izcelsmi (‡1199, ‡1200, ‡1201*). Tekstam tās parasti izpaužas kā smalkas novirzes vārdu izvēlē un stilā (‡1308, ‡1309); attēliem un video — kā smalki raksti pa pikseļiem (‡1310); un audio gadījumā — kā smalki raksti audio viļņos (‡1311). Figūra 3.8 ilustrē šos piemērus.

Papildus ūdenszīmēm, ar AI ģenerēts saturs var tikt saglabāts arī failu formātos, kas ietver metadatus par to, kā tas tika ģenerēts. Piemēram, daudzi mobilie tālruņi saglabā attēlu un audio failus failu formātā, kas var glabāt informāciju par kameras iestatījumiem, laiku, atrašanās vietu u.tml. (‡1312). Līdzīgus metadatus var izmantot, lai glabātu informāciju par to, vai dati tika ģenerēti ar AI sistēmu. Līdzīgi kā pirkstu nospiedumu noteikšana kriminālistikā, ūdenszīmes un metadati var tikt manipulēti vai noņemti, taču tie tomēr ir noderīgi.

Pētnieki arī strādā pie AI ģenerēta satura detektoru izstrādes (‡1203, ‡1204, ‡1205*), lai palīdzētu identificēt AI ģenerētu saturu “savvaļā”, pat ja nav pieejams ne ūdenszīmes, ne metadatu. Tomēr šīm identifikācijas metodēm ir ierobežots panākumu līmenis.

###@ Atjauninājumi

Kopš pēdējā Ziņojuma publicēšanas (2025. gada janvāris) ir panākts progress mākslīgā intelekta sistēmu izstrādē ar vairākiem iedarbīgiem aizsardzības slāņiem. Kā apspriests 3.2. Risku pārvaldības prakses sadaļā, aizsardzība pa dziļumu ir galvenais riska pārvaldības princips (‡1314). Piemēram, tiek arvien vairāk pētītas un ieviestas AI sistēmas, kas apvieno ar drošumu apmācītus modeļus ar ievades filtriem, izvades filtriem un citiem satura uzraugiem (‡32, ‡65, ‡1182*). Jaunākie pētījumi arī ir parādījuši, ka, lai gan modeļu izstrādātāji ir panākuši progresu, palielinot noturību pret mēģinājumiem apiet aizsargpasākumus, uzbrucēji joprojām panāk panākumus augstā īpatsvarā (3.9. attēls).

###@ Pierādījumu trūkumi

Ir nepieciešami papildu pierādījumi, lai palīdzētu pētniekiem izprast un ņemt vērā esošo pieeju ierobežojumus. Tehniskās drošības garantijas AI sistēmām tiek uzlabotas, taču metodes saskaras ar ierobežojumiem. Piemēram, progress vispārējas nozīmes AI sistēmu sliktākā gadījuma noturības uzlabošanā ir bijis lēns, un pastāv fundamentāli ierobežojumi, cik rūpīgi atvērtā svara modeļus var nodrošināt ar drošības pasākumiem un uzraudzīt (‡1195, ‡1315, ‡1316) (skat. arī §3.4. Atvērta svara modeļi). Tikmēr ne visas tehniskās drošības garantijas ir tikpat bieži sastopamas, tikpat efektīvas vai tikpat labi pierādītas reālajā pasaulē. Piemēram, pretinieka (adversarial) apmācība gandrīz visur tiek izmantota jaunākā līmeņa (state-of-the-art) modeļos (‡64*, ‡677), kamēr modeļu interpretējamība un formālās verificēšanas metodes līdz šim ražošanas sistēmās ir izmantotas maz (‡1177, ‡1285).

###@ Izaicinājumi politikas veidotājiem

Galvenie izaicinājumi politikas veidotājiem ir saistīti ar to, vai un kā viņiem būtu jāatbalsta pētniecība, izstrāde, izvērtēšana un tehnisko aizsargmehānismu un uzraudzības metožu ieviešana. Tas ir sarežģīti, jo zinātnieku izpratne par to, kā vislabāk praktiski nodrošināt mehānismu aizsardzību, joprojām attīstās, un labākā prakse vēl nav izveidota. Piemēram, dažādi izstrādātāji piemēro dažādus aizsargmehānismus, un viņu pieejas tehnisko risku mazināšanai kopumā būtiski atšķiras (‡1116). Visbeidzot, efektīvu tehnisko aizsargmehānismu esamība pati par sevi negarantē drošību, jo ieviešana un īstenošana var atšķirties starp izstrādātājiem un izvietošanas kontekstiem.

